# Comparing `tmp/dvcx-0.71.0.tar.gz` & `tmp/dvcx-0.72.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.71.0.tar", last modified: Wed Mar 20 03:14:59 2024, max compression
+gzip compressed data, was "dvcx-0.72.0.tar", last modified: Tue Apr  2 04:20:17 2024, max compression
```

## Comparing `dvcx-0.71.0.tar` & `dvcx-0.72.0.tar`

### file list

```diff
@@ -1,213 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.110302 dvcx-0.71.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-20 03:14:36.000000 dvcx-0.71.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 03:14:36.000000 dvcx-0.71.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.070302 dvcx-0.71.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.070302 dvcx-0.71.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.074302 dvcx-0.71.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-20 03:14:36.000000 dvcx-0.71.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-20 03:14:36.000000 dvcx-0.71.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-20 03:14:36.000000 dvcx-0.71.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.074302 dvcx-0.71.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-20 03:14:36.000000 dvcx-0.71.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-20 03:14:36.000000 dvcx-0.71.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-20 03:14:36.000000 dvcx-0.71.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-20 03:14:36.000000 dvcx-0.71.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-20 03:14:36.000000 dvcx-0.71.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.074302 dvcx-0.71.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-03-20 03:14:36.000000 dvcx-0.71.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-20 03:14:36.000000 dvcx-0.71.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-03-20 03:14:36.000000 dvcx-0.71.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-20 03:14:59.110302 dvcx-0.71.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-20 03:14:36.000000 dvcx-0.71.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.074302 dvcx-0.71.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-20 03:14:36.000000 dvcx-0.71.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.078302 dvcx-0.71.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.078302 dvcx-0.71.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.078302 dvcx-0.71.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.078302 dvcx-0.71.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-20 03:14:36.000000 dvcx-0.71.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-20 03:14:36.000000 dvcx-0.71.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-03-20 03:14:36.000000 dvcx-0.71.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 03:14:59.110302 dvcx-0.71.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.066302 dvcx-0.71.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.082302 dvcx-0.71.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-20 03:14:58.000000 dvcx-0.71.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.086302 dvcx-0.71.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68446 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    28492 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.086302 dvcx-0.71.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/client/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.086302 dvcx-0.71.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44781 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    30635 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33230 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.090302 dvcx-0.71.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.090302 dvcx-0.71.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    51254 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.090302 dvcx-0.71.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.090302 dvcx-0.71.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.094302 dvcx-0.71.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.094302 dvcx-0.71.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.094302 dvcx-0.71.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-03-20 03:14:36.000000 dvcx-0.71.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.102302 dvcx-0.71.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-20 03:14:59.000000 dvcx-0.71.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.094302 dvcx-0.71.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.094302 dvcx-0.71.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.098302 dvcx-0.71.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   104056 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    25265 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.102302 dvcx-0.71.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.102302 dvcx-0.71.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/lib/test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.102302 dvcx-0.71.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:14:59.102302 dvcx-0.71.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-20 03:14:36.000000 dvcx-0.71.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.378401 dvcx-0.72.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 04:20:12.000000 dvcx-0.72.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 04:20:12.000000 dvcx-0.72.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.338401 dvcx-0.72.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.338401 dvcx-0.72.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-02 04:20:12.000000 dvcx-0.72.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 04:20:12.000000 dvcx-0.72.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 04:20:12.000000 dvcx-0.72.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 04:20:12.000000 dvcx-0.72.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-02 04:20:12.000000 dvcx-0.72.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-02 04:20:12.000000 dvcx-0.72.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-02 04:20:17.378401 dvcx-0.72.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-02 04:20:12.000000 dvcx-0.72.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-02 04:20:12.000000 dvcx-0.72.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-02 04:20:12.000000 dvcx-0.72.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-02 04:20:12.000000 dvcx-0.72.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:20:17.378401 dvcx-0.72.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.334401 dvcx-0.72.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.350401 dvcx-0.72.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.354401 dvcx-0.72.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69026 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.354401 dvcx-0.72.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.358401 dvcx-0.72.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33325 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53799 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.370401 dvcx-0.72.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34568 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/utils.py
```

### Comparing `dvcx-0.71.0/.cruft.json` & `dvcx-0.72.0/.cruft.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'80e68ce58293580b73e5de011f71b2ce5fbd9dda'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "e4ec95f4cfd03d4af0a8604d462ee11d07d63b42",
+    "commit": "80e68ce58293580b73e5de011f71b2ce5fbd9dda",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Dmitry Petrov",
             "copyright_year": "2022",
             "development_status": "Development Status :: 2 - Pre-Alpha",
             "docs": "False",
```

### Comparing `dvcx-0.71.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.72.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.72.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/.github/workflows/release.yml` & `dvcx-0.72.0/.github/workflows/release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,19 @@
           fetch-depth: 0
 
       - name: Set up Python 3.10
         uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
-      - name: Upgrade pip and nox
+      - name: Upgrade nox and uv
         run: |
-          pip install --upgrade pip nox
-          pip --version
+          python -m pip install --upgrade 'nox[uv]'
           nox --version
+          uv --version
 
       - name: Build package
         run: nox -s build
 
       - name: Upload package
         if: github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dvcx-0.71.0/.github/workflows/tests.yml` & `dvcx-0.72.0/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -24,95 +24,98 @@
           fetch-depth: 0
 
       - name: Set up Python 3.9
         uses: actions/setup-python@v5
         with:
           python-version: '3.9'
           cache: 'pip'
-          cache-dependency-path: 'pyproject.toml'
 
-      - name: Upgrade pip and nox
+      - name: Upgrade nox and uv
         run: |
-          python -m pip install --upgrade pip nox
-          pip --version
+          python -m pip install --upgrade 'nox[uv]'
           nox --version
+          uv --version
+
+      - name: Cache mypy
+        uses: actions/cache@v4
+        with:
+          path: .mypy_cache
+          key: mypy-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}
+
+      - name: Cache pre-commit hooks
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pre-commit
+          key: pre-commit-3|${{ env.pythonLocation }}|${{ hashFiles('.pre-commit-config.yaml') }}
 
       - name: Lint code and check dependencies
         run: nox -s lint
 
   tests:
     timeout-minutes: 25
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-20.04]
+        os: [ubuntu-latest-8-cores]
         pyv: ['3.9', '3.10', '3.11', '3.12']
         include:
           - os: macos-latest
             pyv: '3.9'
-          - os: macos-latest
+          - os: macos-14
             pyv: '3.12'
-          - os: windows-latest
+          - os: windows-latest-8-cores
             pyv: '3.9'
-          - os: windows-latest
+          - os: windows-latest-8-cores
             pyv: '3.12'
 
     steps:
 
       # https://github.com/iterative/pytest-servers/pull/122
       # https://github.com/abiosoft/colima/issues/468
       # https://github.com/abiosoft/colima/blob/main/docs/FAQ.md#cannot-connect-to-the-docker-daemon-at-unixvarrundockersock-is-the-docker-daemon-running
       # colima v0.5.6 seems to run more stable than the latest - that has occasional network failures (ports are not open)
       # see: https://github.com/abiosoft/colima/issues/962
       - name: Use colima as default docker host on MacOS
-        if: matrix.os == 'macos-latest'
+        if: runner.os == 'macOS'
         run: |
-          brew install docker
-          brew unlink colima
-          curl -L -o /usr/local/bin/colima https://github.com/abiosoft/colima/releases/download/v0.5.6/colima-Darwin-x86_64
+          brew install docker lima || true # avoid non-zero exit code if brew link fails
+          sudo curl -L -o /usr/local/bin/colima https://github.com/abiosoft/colima/releases/download/v0.5.6/colima-Darwin-x86_64
           sudo chmod +x /usr/local/bin/colima
           colima start
           sudo ln -vsf "${HOME}"/.colima/default/docker.sock /var/run/docker.sock
+        env:
+          HOMEBREW_NO_AUTO_UPDATE: true
+          HOMEBREW_NO_INSTALL_CLEANUP: true
+          HOMEBREW_NO_INSTALLED_DEPENDENTS_CHECK: true
+          HOMEBREW_NO_INSTALL_UPGRADE: true
 
       - name: Check out the repository
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python ${{ matrix.pyv }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.pyv }}
           cache: 'pip'
-          cache-dependency-path: 'pyproject.toml'
-
-      - name: Cache .nox
-        uses: actions/cache@v4
-        id: cache-nox
-        with:
-          path: .nox
-          key: nox-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('noxfile.py') }}
-
-      - name: Skip installing dependencies if .nox directory is cached
-        shell: bash
-        run: echo SKIP_DEPS_INSTALL="${{ steps.cache-nox.outputs.cache-hit }}" >> $GITHUB_ENV
 
-      - name: Upgrade pip and nox
+      - name: Upgrade nox and uv
         run: |
-          python -m pip install --upgrade pip nox
-          pip --version
+          python -m pip install --upgrade 'nox[uv]'
           nox --version
+          uv --version
 
       - name: Skip flaky azure, gcs remotes if unavailable on macos
-        if: matrix.os == 'macos-latest'
+        if: runner.os == 'macOS'
         run: echo 'DVCX_TEST_SKIP_MISSING_REMOTES=azure,gcs' >> "$GITHUB_ENV"
 
       - name: Run tests
-        run: nox -s tests-${{ matrix.nox_pyv || matrix.pyv }} -- --cov-report=xml --durations=10
+        run: nox -s tests-${{ matrix.pyv }}
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: coverage.xml
           flags: dvcx
```

### Comparing `dvcx-0.71.0/.gitignore` & `dvcx-0.72.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/.pre-commit-config.yaml` & `dvcx-0.72.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,24 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
         exclude: '^LICENSES/'
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.1.13'
+    rev: 'v0.3.5'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.12.0
+    rev: v2.13.0
     hooks:
       - id: pretty-format-toml
         args: [--autofix, --no-sort]
       - id: pretty-format-yaml
         args: [--autofix, --indent, '2', '--offset', '2', --preserve-quotes]
```

### Comparing `dvcx-0.71.0/CODE_OF_CONDUCT.rst` & `dvcx-0.72.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/CONTRIBUTING.rst` & `dvcx-0.72.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/LICENSE` & `dvcx-0.72.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/LICENSES/Apache-2.0.txt` & `dvcx-0.72.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.72.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/LICENSES/Python-2.0.txt` & `dvcx-0.72.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/PKG-INFO` & `dvcx-0.72.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.71.0
+Version: 0.72.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,14 +31,15 @@
 Requires-Dist: dill==0.3.8
 Requires-Dist: ujson==5.9.0
 Requires-Dist: types-ujson==5.9.0.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
 Requires-Dist: torch>=2.1.0; extra == "cv"
+Requires-Dist: torchvision; extra == "cv"
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: transformers>=4.36.0; extra == "cv"
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4.0; extra == "pandas"
 Provides-Extra: remote
 Requires-Dist: dvcx[pandas]; extra == "remote"
 Requires-Dist: lz4; extra == "remote"
@@ -51,17 +52,18 @@
 Requires-Dist: scipy; extra == "vector"
 Provides-Extra: tests
 Requires-Dist: dvcx[cv,pandas,remote,vector]; extra == "tests"
 Requires-Dist: pytest<9,>=8; extra == "tests"
 Requires-Dist: pytest-sugar>=0.9.6; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-mock>=3.12.0; extra == "tests"
-Requires-Dist: pytest-servers[all]>=0.4.0; extra == "tests"
+Requires-Dist: pytest-servers[all]>=0.5.1; extra == "tests"
 Requires-Dist: pytest-benchmark[histogram]; extra == "tests"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "tests"
+Requires-Dist: pytest-xdist>=3.3.1; extra == "tests"
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
```

### Comparing `dvcx-0.71.0/README.rst` & `dvcx-0.72.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/docs/udfs.md` & `dvcx-0.72.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/blip2_image_desc_lib.py` & `dvcx-0.72.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/common_sql_functions.py` & `dvcx-0.72.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/dir_expansion.py` & `dvcx-0.72.0/examples/dir_expansion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This script provides an example of the dir expansion query available
 for datasets and storage indices. It prints the results, some summary
 stats and verifies that the result is the same both for a dataset and
 for a storage index with the same entries.
 """
+
 import sys
 
 import sqlalchemy as sa
 
 from dvcx.catalog import get_catalog
 from dvcx.error import DatasetNotFoundError
 from dvcx.query import DatasetQuery
```

### Comparing `dvcx-0.71.0/examples/hf_pipeline.py` & `dvcx-0.72.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/llava2_image_desc_lib.py` & `dvcx-0.72.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/neurips/README` & `dvcx-0.72.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/neurips/distance_to_query.py` & `dvcx-0.72.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/neurips/llm_chat.py` & `dvcx-0.72.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/neurips/single_query.py` & `dvcx-0.72.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/neurips/text_loaders.py` & `dvcx-0.72.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/openai_image_desc_lib.py` & `dvcx-0.72.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/openimage-detect.py` & `dvcx-0.72.0/examples/openimage-detect.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import pandas as pd
 from PIL import Image
 
 from dvcx.lib.dataset import Dataset
 from dvcx.lib.feature import ShallowFeature
 from dvcx.lib.feature_udf import FeatureAggregator
-from dvcx.lib.stream import FileInfo, FileStream
+from dvcx.lib.file import File, FileInfo
 from dvcx.query.schema import C
 from dvcx.sql.functions import path
 
 
 class BBox(ShallowFeature):
     x_min: int
     x_max: int
     y_min: int
     y_max: int
 
 
 class OpenImageDetect(FeatureAggregator):
     def __init__(self):
-        super().__init__(FileStream, [FileInfo, BBox])
+        super().__init__(File, [FileInfo, BBox])
 
     def process(self, args):
         if len(args) != 2:
             raise ValueError("Group jpg-json mismatch")
 
         stream_jpg = args[0]
         stream_json = args[1]
```

### Comparing `dvcx-0.71.0/examples/pose_detection.py` & `dvcx-0.72.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/torch-loader.py` & `dvcx-0.72.0/examples/torch-loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,38 @@
 # pip install Pillow torchvision
 
 import torch
-from PIL import Image
 from torch import nn, optim
-from torch.utils.data import DataLoader, IterableDataset
-from torchvision import transforms
+from torch.utils.data import DataLoader
+from torchvision.transforms import v2
 
-from dvcx.query import C, DatasetQuery, Object, udf
+from dvcx.lib.param import Image, Label
+from dvcx.lib.pytorch import DvcxDataset
+from dvcx.query import C, DatasetQuery, udf
 from dvcx.sql.types import String
 
 STORAGE = "gcs://dvcx-datalakes/dogs-and-cats/"
 
 # Define transformation for data preprocessing
-transform = transforms.Compose(
+transform = v2.Compose(
     [
-        transforms.Resize((64, 64)),
-        transforms.ToTensor(),
-        transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
+        v2.Resize((64, 64)),
+        v2.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
     ]
 )
 
 
-def load_img(buf):
-    return Image.open(buf).convert("RGB")
+CLASSES = ["cat", "dog"]
 
 
 @udf(params=("name",), output={"label": String})
 def extract_label(name):
     return (name[:3],)
 
 
-CLASSES = ["cat", "dog"]
-
-
-class DvcxDataset(IterableDataset):
-    def __init__(self, storage, transform):
-        self.storage = storage
-        self.transform = transform
-
-    def __iter__(self):
-        q = (
-            DatasetQuery(self.storage)
-            .filter(C.name.glob("*.jpg"))
-            .add_signals(extract_label)
-        )
-        for img, label in q.extract(Object(load_img), "label", cache=True):
-            class_idx = CLASSES.index(label)
-            yield self.transform(img), class_idx
-
-
-train_loader = DataLoader(DvcxDataset(STORAGE, transform=transform), batch_size=16)
-
-
 # Define torch model
 class CNN(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv1 = nn.Conv2d(3, 16, kernel_size=3, stride=2, padding=1)
         self.conv2 = nn.Conv2d(16, 32, kernel_size=3, stride=2, padding=1)
         self.conv3 = nn.Conv2d(32, 64, kernel_size=3, stride=2, padding=1)
@@ -68,29 +45,47 @@
         x = torch.relu(self.conv3(x))
         x = x.view(-1, 64 * 8 * 8)
         x = torch.relu(self.fc1(x))
         x = self.fc2(x)
         return x
 
 
-model = CNN()
-criterion = nn.CrossEntropyLoss()
-optimizer = optim.Adam(model.parameters(), lr=0.001)
-
-# Train the model
-num_epochs = 10
-for epoch in range(num_epochs):
-    for i, data in enumerate(train_loader):
-        inputs, labels = data
-        optimizer.zero_grad()
-
-        # Forward pass
-        outputs = model(inputs)
-        loss = criterion(outputs, labels)
-
-        # Backward pass and optimize
-        loss.backward()
-        optimizer.step()
+if __name__ == "__main__":
+    q = (
+        DatasetQuery(STORAGE)
+        .filter(C.name.glob("*.jpg"))
+        .add_signals(extract_label)
+        .save("cats-and-dogs")
+    )
+
+    train_loader = DataLoader(
+        DvcxDataset(
+            params=[Image(), Label("label", CLASSES)],
+            name="cats-and-dogs",
+            cache=True,
+            transform=transform,
+        ),
+        batch_size=16,
+    )
+
+    model = CNN()
+    criterion = nn.CrossEntropyLoss()
+    optimizer = optim.Adam(model.parameters(), lr=0.001)
+
+    # Train the model
+    num_epochs = 10
+    for epoch in range(num_epochs):
+        for i, data in enumerate(train_loader):
+            inputs, labels = data
+            optimizer.zero_grad()
+
+            # Forward pass
+            outputs = model(inputs)
+            loss = criterion(outputs, labels)
+
+            # Backward pass and optimize
+            loss.backward()
+            optimizer.step()
 
-        print("[%d, %5d] loss: %.3f" % (epoch + 1, i + 1, loss.item()))
+            print("[%d, %5d] loss: %.3f" % (epoch + 1, i + 1, loss.item()))
 
-print("Finished Training")
+    print("Finished Training")
```

### Comparing `dvcx-0.71.0/examples/udfs/batching.py` & `dvcx-0.72.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/udfs/image_transformation.py` & `dvcx-0.72.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/udfs/parallel.py` & `dvcx-0.72.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/udfs/simple.py` & `dvcx-0.72.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/udfs/stateful.py` & `dvcx-0.72.0/examples/udfs/stateful.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """
 To install dependencies:
 
   pip install imgbeddings
 
 """
+
 import uuid
 
 from imgbeddings import imgbeddings
-from PIL import Image
 
-from dvcx.query import C, DatasetQuery, Object, udf
+from dvcx.lib.param import Image
+from dvcx.query import C, DatasetQuery, udf
 from dvcx.sql.types import Array, Float32
 
 
-def load_image(raw):
-    img = Image.open(raw)
-    img.load()
-    return img
-
-
 @udf(
-    params=(Object(load_image),),
+    params=(Image(),),
     output={"embedding": Array(Float32)},
     method="embedding",
 )
 class ImageEmbeddings:
     def __init__(self):
         self.emb = imgbeddings()
 
@@ -33,19 +28,16 @@
         return (emb[0].tolist(),)
 
 
 if __name__ == "__main__":
     ds_name = uuid.uuid4().hex
     print(f"Saving to dataset: {ds_name}")
     # Save as a new dataset
-    DatasetQuery(
-        path="gcs://dvcx-datalakes/dogs-and-cats/",
-        client_config={"aws_anon": True},
-    ).filter(C.name.glob("*cat*.jpg")).limit(5).add_signals(ImageEmbeddings).save(
-        ds_name
-    )
+    DatasetQuery(path="gcs://dvcx-datalakes/dogs-and-cats/").filter(
+        C.name.glob("*cat*.jpg")
+    ).limit(5).add_signals(ImageEmbeddings).save(ds_name)
 
     for row in DatasetQuery(name=ds_name).results()[:2]:
         print("default columns: ", row[:-1])
         print("embedding[:10]:  ", row[-1][:10])
         print(f"type: {type(row[-1]).__name__}, len: {len(row[-1])}")
         print()
```

### Comparing `dvcx-0.71.0/examples/udfs/stateful_similarity.py` & `dvcx-0.72.0/examples/udfs/stateful_similarity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 """
 To install dependencies:
 
   pip install imgbeddings
 
 """
+
 import uuid
 
 from imgbeddings import imgbeddings
-from PIL import Image
 from sqlalchemy import tuple_
 
-from dvcx.query import C, DatasetQuery, Object, udf
+from dvcx.lib.param import Image
+from dvcx.query import C, DatasetQuery, udf
 from dvcx.sql.functions.array import cosine_distance, euclidean_distance
 from dvcx.sql.types import Array, Float32
 
 
-def load_image(raw):
-    img = Image.open(raw)
-    img.load()
-    return img
-
-
 @udf(
-    params=(Object(load_image),),
+    params=(Image(),),
     output={"embedding": Array(Float32)},
     method="embedding",
 )
 class ImageEmbeddings:
     def __init__(self):
         self.emb = imgbeddings()
 
@@ -35,18 +30,15 @@
         return (emb[0].tolist(),)
 
 
 ds1_name = uuid.uuid4().hex
 print(f"Saving embeddings to dataset: {ds1_name}")
 # Save as a new dataset
 (
-    DatasetQuery(
-        path="gcs://dvcx-datalakes/dogs-and-cats/",
-        client_config={"aws_anon": True},
-    )
+    DatasetQuery(path="gcs://dvcx-datalakes/dogs-and-cats/")
     .filter(C.name.glob("*cat*.jpg"))
     .add_signals(ImageEmbeddings)
     .save(ds1_name)
 )
 
 ds2_name = uuid.uuid4().hex
 source, parent, name, embedding = (
```

### Comparing `dvcx-0.71.0/examples/unstructured-text.py` & `dvcx-0.72.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/wds.py` & `dvcx-0.72.0/examples/wds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import pandas as pd
 
-from dvcx.lib.dataset import Dataset
+from dvcx.lib.dataset import C, Dataset
+from dvcx.lib.file import FileInfo
 from dvcx.lib.webdataset import WebDataset
-from dvcx.lib.webdataset_meta import MergeParquetAndNpz
-from dvcx.query.schema import C, DatasetRow
+from dvcx.lib.webdataset_laion import WDSLaion
+from dvcx.lib.webdataset_meta import LaionMeta, MergeParquetAndNpz
 from dvcx.sql.functions import path
 
-threads = 8
-
 wds = (
     Dataset("gcs://dvcx-datacomp-small/shards")
-    .filter(C.name.glob("0000000*.tar"))
-    .generate(WebDataset(extensions=["json"]), parallel=threads)
+    .filter(C.name.glob("00000000.tar"))
+    .generate(WebDataset(spec=WDSLaion), cache=True)
 )
 
 meta = (
     Dataset("gcs://dvcx-datacomp-small/metadata")
     .filter(C.name.glob("0020f*"))
-    .aggregate(
-        MergeParquetAndNpz(), partition_by=path.file_stem(C.name), parallel=threads
-    )
-    .select_except(*DatasetRow.schema.keys())
+    .aggregate(MergeParquetAndNpz(), partition_by=path.file_stem(C.name), cache=True)
+    .select_except(FileInfo)
 )
 
-res = wds.join(meta, "uid")
-
-ds_name = "laion_wds"
-res.save(ds_name)
+res = wds.merge(meta, on=WDSLaion.json.uid, right_on=LaionMeta.uid)
 
-df = Dataset(name=ds_name).limit(50).to_pandas()
+df = res.limit(10).to_pandas()
 with pd.option_context("display.max_columns", None):
     print(df)
```

### Comparing `dvcx-0.71.0/examples/wds_filtered.py` & `dvcx-0.72.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/examples/wds_meta.py` & `dvcx-0.72.0/examples/wds_meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pandas as pd
 
 from dvcx.lib.dataset import C, Dataset
-from dvcx.lib.stream import FileStream
+from dvcx.lib.file import File
 from dvcx.lib.webdataset_meta import LaionMeta, parse_wds_meta
 
 ds = Dataset("s3://dvcx-datacomp-small", client_config={"aws_anon": True})
 ds = ds.filter(C.name.glob("0020f*"))
 ds = ds.apply(parse_wds_meta)
 
 ds = ds.select(
-    FileStream.name,
-    FileStream.parent,
+    File.name,
+    File.parent,
     LaionMeta.uid,
     LaionMeta.original_width,
     LaionMeta.face_bboxes,
     LaionMeta.b32_img,
     LaionMeta.dedup,
 )
```

### Comparing `dvcx-0.71.0/examples/zalando/zalando_clip.py` & `dvcx-0.72.0/examples/zalando/zalando_clip.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 fashion-clip UDF, using the
 [fashion-clip](https://pypi.org/project/fashion-clip/#description) package.
 
 Generated embeddings are stored json-encoded.
 
 To install script dependencies: pip install tabulate fashion-clip
 """
+
 import json
 
 from fashion_clip.fashion_clip import FashionCLIP
-from PIL import Image
 from sqlalchemy import JSON
 from tabulate import tabulate
 
-from dvcx.query import C, DatasetQuery, Object, udf
-
-
-def load_image(raw):
-    img = Image.open(raw)
-    img.load()
-    return img
+from dvcx.lib.param import Image
+from dvcx.query import C, DatasetQuery, udf
 
 
 @udf(
-    params=(Object(load_image),),
+    params=(Image(),),
     output={"fclip": JSON},
     method="fashion_clip",
     batch=10,
 )
 class MyFashionClip:
     def __init__(self):
         self.fclip = FashionCLIP("fashion-clip")
```

### Comparing `dvcx-0.71.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.72.0/examples/zalando/zalando_dir_as_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 UDF to create 'class' and 'type' signals from the directory structure.
 
 To install script dependencies: pip install tabulate
 """
+
 from pathlib import Path
 
 from sqlalchemy import Text
 from tabulate import tabulate
 
 from dvcx.query import C, DatasetQuery, udf
```

### Comparing `dvcx-0.71.0/noxfile.py` & `dvcx-0.72.0/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Automation using nox."""
+
 import glob
 import os
 
 import nox
 
+nox.options.default_venv_backend = "uv|virtualenv"
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = "lint", "tests"
 locations = "src", "tests"
 
 
 @nox.session
 def bench(session: nox.Session) -> None:
@@ -18,23 +20,24 @@
         "benchmark",
         "--benchmark-group-by",
         "func",
         *session.posargs,
     )
 
 
-@nox.session(python=["3.9", "3.10", "3.11", "3.12", "pypy3.9"])
+@nox.session(python=["3.9", "3.10", "3.11", "3.12", "pypy3.9", "pypy3.10"])
 def tests(session: nox.Session) -> None:
-    args = ("--no-deps",) if os.getenv("SKIP_DEPS_INSTALL") == "true" else ()
-    session.install("--upgrade", "pip")
-    session.install(".[tests]", *args)
+    session.install(".[tests]")
     session.run(
         "pytest",
         "--cov",
         "--cov-config=pyproject.toml",
+        "--cov-report=xml",
+        "--durations=10",
+        "--numprocesses=logical",
         *session.posargs,
         env={"COVERAGE_FILE": f".coverage.{session.python}"},
     )
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
@@ -52,16 +55,16 @@
     session.install(".[dev]")
     session.install("safety")
     session.run("safety", "check", "--full-report")
 
 
 @nox.session
 def build(session: nox.Session) -> None:
-    session.install("build", "setuptools", "twine")
-    session.run("python", "-m", "build")
+    session.install("build", "twine", "uv")
+    session.run("python", "-m", "build", "--installer", "uv")
     dists = glob.glob("dist/*")
     session.run("twine", "check", *dists, silent=True)
 
 
 @nox.session
 def dev(session: nox.Session) -> None:
     """Sets up a python development environment for the project."""
```

### Comparing `dvcx-0.71.0/pyproject.toml` & `dvcx-0.72.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
   "pydantic>=2,<3"
 ]
 
 [project.optional-dependencies]
 cv = [
   "Pillow>=10.0.0,<11",
   "torch>=2.1.0",
+  "torchvision",
   "numpy",
   "transformers>=4.36.0"
 ]
 pandas = ["pandas>=1.4.0"]
 remote = [
   "dvcx[pandas]",
   "lz4",
@@ -60,17 +61,18 @@
 ]
 tests = [
   "dvcx[cv,pandas,remote,vector]",
   "pytest>=8,<9",
   "pytest-sugar>=0.9.6",
   "pytest-cov>=4.1.0",
   "pytest-mock>=3.12.0",
-  "pytest-servers[all]>=0.4.0",
+  "pytest-servers[all]>=0.5.1",
   "pytest-benchmark[histogram]",
   "pytest-asyncio>=0.23.2",
+  "pytest-xdist>=3.3.1",
   "virtualenv",
   "dulwich",
   "hypothesis",
   "numpy",
   "aiotools>=1.7.0",
   "requests-mock"
 ]
@@ -96,17 +98,21 @@
 
 [tool.setuptools_scm]
 write_to = "src/dvcx/_version.py"
 
 [tool.pytest.ini_options]
 addopts = "-ra -m 'not benchmark'"
 markers = [
-  "benchmark: benchmarks."
+  "benchmark: benchmarks.",
+  "e2e: End-to-end tests"
 ]
 asyncio_mode = "auto"
+filterwarnings = [
+  "ignore:Field name .* shadows an attribute in parent:UserWarning"  # dvcx.lib.feature
+]
 
 [tool.coverage.run]
 branch = true
 source = ["dvcx", "tests"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
@@ -138,14 +144,18 @@
 ignore_missing_imports = true
 files = ["src", "tests"]
 
 [tool.codespell]
 ignore-words-list = " "
 
 [tool.ruff]
+output-format = "full"
+show-fixes = true
+
+[tool.ruff.lint]
 ignore = [
   "S101",  # assert
   "PLR2004",  # magic-value-comparison
   "PLW2901",  # redefined-loop-name
   "PLC0105"  # type-name-incorrect-variance
 ]
 select = [
@@ -160,16 +170,14 @@
   "S",  # flake8-bandit
   "PL",  # pylint
   "TCH",  # flake8-type-checking
   "UP",  # pyupgrade
   "N",  # pep8-naming
   "PIE"  # flake8-pie
 ]
-show-source = true
-show-fixes = true
 
 [tool.ruff.lint.flake8-bugbear]
 # Allow default arguments like, e.g., `data: List[str] = fastapi.Query(None)`.
 extend-immutable-calls = ["dvcx.storage.StorageURI"]
 
 [tool.ruff.lint.flake8-type-checking]
 strict = true
@@ -179,9 +187,9 @@
 
 [tool.ruff.lint.pylint]
 max-args = 16
 max-branches = 16
 max-public-methods = 32
 max-statements = 64
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
```

### Comparing `dvcx-0.71.0/src/dvcx/asyn.py` & `dvcx-0.72.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/cache.py` & `dvcx-0.72.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/catalog/catalog.py` & `dvcx-0.72.0/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from attrs import asdict
 from fsspec.implementations.local import LocalFileSystem
 from sqlalchemy import Column
 from tqdm import tqdm
 
 from dvcx.cache import DVCXCache
 from dvcx.client import Client
+from dvcx.config import get_remote_config, read_config
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.dataset import (
     DATASET_PREFIX,
     QUERY_DATASET_NAME_PREFIX,
     DatasetDependency,
     DatasetRecord,
     DatasetRow,
@@ -64,18 +65,16 @@
 from dvcx.remote.studio import StudioClient
 from dvcx.sql.types import DateTime, SQLType, String
 from dvcx.storage import Status, Storage, StorageStats, StorageURI
 from dvcx.utils import (
     DVCXDir,
     chunk,
     dvcx_paths_join,
-    get_remote_config,
     import_object,
     parse_params_string,
-    read_config,
 )
 
 from .datasource import DataSource
 from .formats import IndexingFormat, apply_processors
 
 if TYPE_CHECKING:
     from dvcx.data_storage import (
@@ -1309,15 +1308,17 @@
         version: Optional[int] = None,
         force: Optional[bool] = False,
     ):
         dataset = self.get_dataset(name)
         if not version and not force:
             raise ValueError(f"Missing dataset version from input for dataset {name}")
         if version and not dataset.has_version(version):
-            raise RuntimeError(f"Dataset {name} doesn't have version {version}")
+            raise DatasetInvalidVersionError(
+                f"Dataset {name} doesn't have version {version}"
+            )
 
         if version:
             self.remove_dataset_version(dataset, version)
             return
 
         for version in dataset.versions.copy():  # type: ignore [assignment, union-attr]
             self.remove_dataset_version(
@@ -1376,20 +1377,22 @@
             # case where we don't create new version, but append to the existing one
             self.warehouse.merge_dataset_rows(
                 src,
                 dst,
                 src_version,
                 dst_version=dst_version,  # type: ignore[arg-type]
             )
-            self.update_dataset(
-                dst,
-                custom_column_types={
-                    **src.custom_column_types_serialized,
-                    **dst.custom_column_types_serialized,
-                },
+            merged_custom_column_types = {
+                **src.custom_column_types_serialized,
+                **dst.custom_column_types_serialized,
+            }
+            self.update_dataset(dst, custom_column_types=merged_custom_column_types)
+            self.metastore.update_dataset_version(
+                dst.get_version(dst_version),  # type: ignore[arg-type]
+                custom_column_types=merged_custom_column_types,
             )
             for dep in src_dep:
                 if dep and dep not in dst_dep:
                     self.metastore.add_dependency(
                         dep,
                         dst.name,
                         dst_version,  # type: ignore[arg-type]
@@ -1689,15 +1692,15 @@
 
     def query(
         self,
         query_script: str,
         envs: Optional[Mapping[str, str]] = None,
         python_executable: Optional[str] = None,
         save: bool = False,
-    ) -> tuple[Optional[DatasetRecord], str]:
+    ) -> tuple[Optional[DatasetRecord], Optional[int], str]:
         """
         Method to run custom user Python script to run a query and, as result,
         creates new dataset from the results of a query.
         Returns tuple of result dataset and script output.
 
         Constraints on query script:
             1. dvcx.query.DatasetQuery should be used in order to create query
@@ -1735,20 +1738,22 @@
             stderr=subprocess.STDOUT,  # merging stderr to stdout
             env=envs,
             check=False,
         )
 
         script_output = ""  # stdout + stderr from user script itself
 
-        # finding returning dataset name from script
-        returned_dataset_name = None
+        # finding returning dataset name and version from script
+        dataset_name = None
+        dataset_version = None
         if result.stdout:
             for line in result.stdout.decode("utf-8").splitlines():
-                if len(line.split(PYTHON_SCRIPT_WRAPPER_CODE)) == 3:
-                    returned_dataset_name = line.split(PYTHON_SCRIPT_WRAPPER_CODE)[1]
+                if len(line.split(PYTHON_SCRIPT_WRAPPER_CODE)) == 4:
+                    dataset_name = line.split(PYTHON_SCRIPT_WRAPPER_CODE)[1]
+                    dataset_version = int(line.split(PYTHON_SCRIPT_WRAPPER_CODE)[2])
                 else:
                     # collecting script output as well to save it to the database
                     # later on for debugging
                     script_output += line + "\n"
 
         if result.returncode:
             if result.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
@@ -1766,37 +1771,39 @@
             raise QueryScriptRunError(
                 f"Query script exited with error code {result.returncode}",
                 return_code=result.returncode,
                 output=script_output,
             )
 
         if not save:
-            return None, script_output
+            return None, None, script_output
 
         # finding returning dataset
         returned_dataset = None
-        if returned_dataset_name:
+        returned_dataset_version = None
+        if dataset_name and dataset_version:
             try:
-                returned_dataset = self.get_dataset(returned_dataset_name)
+                returned_dataset = self.get_dataset(dataset_name)
+                returned_dataset_version = returned_dataset.get_version(dataset_version)
             except DatasetNotFoundError:
                 pass
 
-        if not returned_dataset:
+        if not returned_dataset or not returned_dataset_version:
             raise QueryScriptDatasetNotFound(
                 "No dataset found after running Query script",
                 output=script_output,
             )
 
         returned_dataset = self.update_dataset(
             returned_dataset,
             script_output=script_output,
             query_script=query_script,
         )
 
-        return returned_dataset, script_output
+        return returned_dataset, dataset_version, script_output
 
     def cp(
         self,
         sources: list[str],
         output: str,
         force: bool = False,
         update: bool = False,
```

### Comparing `dvcx-0.71.0/src/dvcx/catalog/datasource.py` & `dvcx-0.72.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/catalog/formats.py` & `dvcx-0.72.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/catalog/loader.py` & `dvcx-0.72.0/src/dvcx/catalog/loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import os
 from importlib import import_module
-from typing import TYPE_CHECKING, Any, Optional
+from typing import Any, Optional
 
 from dvcx.catalog import Catalog
+from dvcx.data_storage import AbstractIDGenerator, AbstractMetastore, AbstractWarehouse
+from dvcx.data_storage.serializer import deserialize
 from dvcx.data_storage.sqlite import SQLiteIDGenerator, SQLiteMetastore, SQLiteWarehouse
 from dvcx.utils import get_envs_by_prefix
 
-if TYPE_CHECKING:
-    from dvcx.data_storage import AbstractIDGenerator
-
-
+ID_GENERATOR_SERIALIZED = "DVCX__ID_GENERATOR"
 ID_GENERATOR_IMPORT_PATH = "DVCX_ID_GENERATOR"
 ID_GENERATOR_ARG_PREFIX = "DVCX_ID_GENERATOR_ARG_"
+METASTORE_SERIALIZED = "DVCX__METASTORE"
 METASTORE_IMPORT_PATH = "DVCX_METASTORE"
 METASTORE_ARG_PREFIX = "DVCX_METASTORE_ARG_"
+WAREHOUSE_SERIALIZED = "DVCX__WAREHOUSE"
 WAREHOUSE_IMPORT_PATH = "DVCX_WAREHOUSE"
 WAREHOUSE_ARG_PREFIX = "DVCX_WAREHOUSE_ARG_"
+DISTRIBUTED_IMPORT_PATH = "DVCX_DISTRIBUTED"
 DISTRIBUTED_ARG_PREFIX = "DVCX_DISTRIBUTED_ARG_"
 
 
-def get_id_generator():
+def get_id_generator() -> "AbstractIDGenerator":
+    id_generator_serialized = os.environ.get(ID_GENERATOR_SERIALIZED)
+    if id_generator_serialized:
+        id_generator_obj = deserialize(id_generator_serialized)
+        if not isinstance(id_generator_obj, AbstractIDGenerator):
+            raise RuntimeError(
+                f"Deserialized ID generator is not an instance of AbstractIDGenerator: "
+                f"{id_generator_obj}"
+            )
+        return id_generator_obj
+
     id_generator_import_path = os.environ.get(ID_GENERATOR_IMPORT_PATH)
     id_generator_arg_envs = get_envs_by_prefix(ID_GENERATOR_ARG_PREFIX)
     # Convert env variable names to keyword argument names by lowercasing them
     id_generator_args = {k.lower(): v for k, v in id_generator_arg_envs.items()}
 
     if id_generator_import_path:
         # ID generator paths are specified as (for example):
@@ -37,15 +49,28 @@
         id_generator = import_module(module_name)
         id_generator_class = getattr(id_generator, class_name)
     else:
         id_generator_class = SQLiteIDGenerator
     return id_generator_class(**id_generator_args)
 
 
-def get_metastore(id_generator: "AbstractIDGenerator"):
+def get_metastore(id_generator: Optional["AbstractIDGenerator"]) -> "AbstractMetastore":
+    metastore_serialized = os.environ.get(METASTORE_SERIALIZED)
+    if metastore_serialized:
+        metastore_obj = deserialize(metastore_serialized)
+        if not isinstance(metastore_obj, AbstractMetastore):
+            raise RuntimeError(
+                f"Deserialized Metastore is not an instance of AbstractMetastore: "
+                f"{metastore_obj}"
+            )
+        return metastore_obj
+
+    if id_generator is None:
+        id_generator = get_id_generator()
+
     metastore_import_path = os.environ.get(METASTORE_IMPORT_PATH)
     metastore_arg_envs = get_envs_by_prefix(METASTORE_ARG_PREFIX)
     # Convert env variable names to keyword argument names by lowercasing them
     metastore_args = {k.lower(): v for k, v in metastore_arg_envs.items()}
 
     if metastore_import_path:
         # Metastore paths are specified as (for example):
@@ -58,15 +83,28 @@
         metastore = import_module(module_name)
         metastore_class = getattr(metastore, class_name)
     else:
         metastore_class = SQLiteMetastore
     return metastore_class(id_generator, **metastore_args)
 
 
-def get_warehouse(id_generator: "AbstractIDGenerator"):
+def get_warehouse(id_generator: Optional["AbstractIDGenerator"]) -> "AbstractWarehouse":
+    warehouse_serialized = os.environ.get(WAREHOUSE_SERIALIZED)
+    if warehouse_serialized:
+        warehouse_obj = deserialize(warehouse_serialized)
+        if not isinstance(warehouse_obj, AbstractWarehouse):
+            raise RuntimeError(
+                f"Deserialized Warehouse is not an instance of AbstractWarehouse: "
+                f"{warehouse_obj}"
+            )
+        return warehouse_obj
+
+    if id_generator is None:
+        id_generator = get_id_generator()
+
     warehouse_import_path = os.environ.get(WAREHOUSE_IMPORT_PATH)
     warehouse_arg_envs = get_envs_by_prefix(WAREHOUSE_ARG_PREFIX)
     # Convert env variable names to keyword argument names by lowercasing them
     warehouse_args = {k.lower(): v for k, v in warehouse_arg_envs.items()}
 
     if warehouse_import_path:
         # Warehouse paths are specified as (for example):
@@ -80,28 +118,29 @@
         warehouse_class = getattr(warehouse, class_name)
     else:
         warehouse_class = SQLiteWarehouse
     return warehouse_class(id_generator, **warehouse_args)
 
 
 def get_distributed_class(**kwargs):
-    distributed_import_path = os.environ.get("DVCX_DISTRIBUTED")
+    distributed_import_path = os.environ.get(DISTRIBUTED_IMPORT_PATH)
     distributed_arg_envs = get_envs_by_prefix(DISTRIBUTED_ARG_PREFIX)
     # Convert env variable names to keyword argument names by lowercasing them
     distributed_args = {k.lower(): v for k, v in distributed_arg_envs.items()}
 
     if not distributed_import_path:
         raise RuntimeError(
-            "DVCX_DISTRIBUTED import path is required for distributed UDF processing."
+            f"{DISTRIBUTED_IMPORT_PATH} import path is required "
+            "for distributed UDF processing."
         )
     # Distributed class paths are specified as (for example):
     # module.classname
     if "." not in distributed_import_path:
         raise RuntimeError(
-            f"Invalid DVCX_DISTRIBUTED import path: {distributed_import_path}"
+            f"Invalid {DISTRIBUTED_IMPORT_PATH} import path: {distributed_import_path}"
         )
     module_name, _, class_name = distributed_import_path.rpartition(".")
     distributed = import_module(module_name)
     distributed_class = getattr(distributed, class_name)
     return distributed_class(**distributed_args | kwargs)
```

### Comparing `dvcx-0.71.0/src/dvcx/cli.py` & `dvcx-0.72.0/src/dvcx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 import shlex
 import sys
 import traceback
 from argparse import SUPPRESS, Action, ArgumentParser, ArgumentTypeError, Namespace
 from collections.abc import Iterable, Iterator, Mapping
 from itertools import chain
 from multiprocessing import freeze_support
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import shtab
 
 from dvcx import __version__, utils
-from dvcx.catalog import Catalog, get_catalog, indexer_formats
 from dvcx.cli_utils import BooleanOptionalAction
-from dvcx.client import Client
-from dvcx.node import DirType, long_line_str
-from dvcx.query.dispatch import udf_entrypoint, udf_worker_entrypoint
-from dvcx.remote.studio import StudioClient
-from dvcx.utils import DVCXDir, get_remote_config, read_config
+from dvcx.utils import DVCXDir
+
+if TYPE_CHECKING:
+    from dvcx.catalog import Catalog
 
 logger = logging.getLogger("dvcx")
 
 TTL_HUMAN = "4h"
 TTL_INT = 4 * 60 * 60
 FIND_COLUMNS = ["du", "name", "owner", "path", "size", "type"]
 
@@ -384,53 +382,47 @@
     )
 
     parse_find = subp.add_parser(
         "find", parents=[parent_parser], help="Search in a directory hierarchy"
     )
     add_sources_arg(parse_find)
     parse_find.add_argument(
-        "-name",
         "--name",
         type=str,
         action="append",
         help="Filename to match pattern.",
     )
     parse_find.add_argument(
-        "-iname",
         "--iname",
         type=str,
         action="append",
         help="Like -name but case insensitive.",
     )
     parse_find.add_argument(
-        "-path",
         "--path",
         type=str,
         action="append",
         help="Path to match pattern.",
     )
     parse_find.add_argument(
-        "-ipath",
         "--ipath",
         type=str,
         action="append",
         help="Like -path but case insensitive.",
     )
     parse_find.add_argument(
-        "-size",
         "--size",
         type=str,
         help=(
             "Filter by size (+ is greater or equal, - is less or equal). "
             "Specified size is in bytes, or use a suffix like K, M, G for "
             "kilobytes, megabytes, gigabytes, etc."
         ),
     )
     parse_find.add_argument(
-        "-type",
         "--type",
         type=str,
         help='File type: "f" - regular, "d" - directory',
     )
     parse_find.add_argument(
         "-c",
         "--columns",
@@ -445,15 +437,15 @@
     parse_index = subp.add_parser(
         "index", parents=[parent_parser], help="Index storage location"
     )
     parse_index.add_argument(
         "--format",
         type=str,
         default=None,
-        choices=indexer_formats.keys(),
+        choices=["tar-files", "json-pair", "webdataset"],
         help="Postprocessing step to apply, after indexing storage.",
     )
     add_sources_arg(parse_index)
     add_storage_parser = subp.add_parser(
         "add-storage", parents=[parent_parser], help="Register local path as storage"
     )
     add_storage_parser.add_argument("uri", type=str, help="Source URI or path")
@@ -534,15 +526,15 @@
     elif args.verbose:
         return logging.DEBUG
     return logging.INFO
 
 
 def ls_urls(
     sources,
-    catalog: Catalog,
+    catalog: "Catalog",
     long: bool = False,
     **kwargs,
 ) -> Iterator[tuple[str, Iterator[str]]]:
     curr_dir = None
     value_iterables = []
     for next_dir, values in _ls_urls_flat(sources, long, catalog, **kwargs):
         if curr_dir is None or next_dir == curr_dir:  # type: ignore[unreachable]
@@ -552,14 +544,16 @@
             value_iterables = [values]
         curr_dir = next_dir
     if curr_dir is not None:
         yield curr_dir, chain(*value_iterables)
 
 
 def _node_data_to_ls_values(row, long_format=False):
+    from dvcx.node import DirType, long_line_str
+
     name = row[0]
     is_dir = row[1] == DirType.DIR
     ending = "/" if is_dir else ""
     value = name + ending
     if long_format:
         last_modified = row[2]
         owner_name = row[3]
@@ -567,17 +561,20 @@
         return long_line_str(value, timestamp, owner_name)
     return value
 
 
 def _ls_urls_flat(
     sources,
     long: bool,
-    catalog: Catalog,
+    catalog: "Catalog",
     **kwargs,
 ) -> Iterator[tuple[str, Iterator[str]]]:
+    from dvcx.client import Client
+    from dvcx.node import long_line_str
+
     for source in sources:
         client_cls = Client.get_implementation(source)
         if client_cls.is_root_url(source):
             buckets = client_cls.ls_buckets(**catalog.client_config)
             if long:
                 values = (long_line_str(b.name, b.created, "") for b in buckets)
             else:
@@ -592,32 +589,36 @@
                 values = (_node_data_to_ls_values(r, long) for r in results)
                 found = True
                 yield data_source.dirname(), values
             if not found:
                 raise FileNotFoundError(f"No such file or directory: {source}")
 
 
-def ls_indexed_storages(catalog: Catalog, long: bool = False) -> Iterator[str]:
+def ls_indexed_storages(catalog: "Catalog", long: bool = False) -> Iterator[str]:
+    from dvcx.node import long_line_str
+
     storage_uris = catalog.ls_storage_uris()
     if long:
         for uri in storage_uris:
             # TODO: add Storage.created so it can be used here
             yield long_line_str(uri, None, "")
     else:
         yield from storage_uris
 
 
 def ls_local(
     sources,
     long: bool = False,
-    catalog: Optional[Catalog] = None,
+    catalog: Optional["Catalog"] = None,
     client_config=None,
     **kwargs,
 ):
     if catalog is None:
+        from .catalog import get_catalog
+
         catalog = get_catalog(client_config=client_config)
     if sources:
         actual_sources = list(ls_urls(sources, catalog=catalog, long=long, **kwargs))
         if len(actual_sources) == 1:
             for _, entries in actual_sources:
                 for entry in entries:
                     print(format_ls_entry(entry))
@@ -648,14 +649,17 @@
 def ls_remote(
     url: str,
     username: str,
     token: str,
     paths: Iterable[str],
     long: bool = False,
 ):
+    from dvcx.node import long_line_str
+    from dvcx.remote.studio import StudioClient
+
     client = StudioClient(url, username, token)
     first = True
     for path, response in client.ls(paths):
         if not first:
             print()
         if not response.ok or response.data is None:
             print(f"{path}:\n  Error: {response.message}\n")
@@ -681,97 +685,107 @@
     sources,
     long: bool = False,
     remote: str = "",
     config: Optional[Mapping[str, str]] = None,
     **kwargs,
 ):
     if config is None:
+        from .config import get_remote_config, read_config
+
         config = get_remote_config(read_config(DVCXDir.find().root), remote=remote)
     remote_type = config["type"]
     if remote_type == "local":
         ls_local(sources, long=long, **kwargs)
     else:
         ls_remote(
             config["url"],
             config["username"],
             config["token"],
             sources,
             long=long,
         )
 
 
-def ls_datasets():
-    for d in get_catalog().ls_datasets():
+def ls_datasets(catalog: "Catalog"):
+    for d in catalog.ls_datasets():
         for v in d.versions:
             print(f"{d.name} (v{v.version})")
 
 
-def ls_dataset_rows(name: str, version: int):
-    for row in get_catalog().ls_dataset_rows(name, version):
+def ls_dataset_rows(catalog: "Catalog", name: str, version: int):
+    for row in catalog.ls_dataset_rows(name, version):
         entry = row.name + ("/" if row.dir_type else "")  # type: ignore[attr-defined]
         print(format_ls_entry(entry))
 
 
-def rm_dataset(name: str, version: Optional[int] = None, force: Optional[bool] = False):
-    get_catalog().remove_dataset(name, version=version, force=force)
+def rm_dataset(
+    catalog: "Catalog",
+    name: str,
+    version: Optional[int] = None,
+    force: Optional[bool] = False,
+):
+    catalog.remove_dataset(name, version=version, force=force)
 
 
 def dataset_stats(
+    catalog: "Catalog",
     name: str,
     version: int,
     show_bytes=False,
     si=False,
 ):
-    stats = get_catalog().dataset_stats(name, version)
+    stats = catalog.dataset_stats(name, version)
 
     if stats:
         print(f"Number of objects: {stats.num_objects}")
         if show_bytes:
             print(f"Total objects size: {stats.size}")
         else:
             print(f"Total objects size: {utils.sizeof_fmt(stats.size, si=si): >7}")
 
 
-def du(sources, show_bytes=False, si=False, **kwargs):
-    for path, size in get_catalog().du(sources, **kwargs):
+def du(catalog: "Catalog", sources, show_bytes=False, si=False, **kwargs):
+    for path, size in catalog.du(sources, **kwargs):
         if show_bytes:
             print(f"{size} {path}")
         else:
             print(f"{utils.sizeof_fmt(size, si=si): >7} {path}")
 
 
 def index(
-    catalog: Catalog,
+    catalog: "Catalog",
     sources,
     indexer_format: Optional[str] = None,
     **kwargs,
 ):
     fmt = None
     if indexer_format:
+        from .catalog import indexer_formats
+
         fmt = indexer_formats.get(indexer_format)
     catalog.index(sources, index_processors=fmt, **kwargs)
 
 
 def query(
-    catalog: Catalog,
+    catalog: "Catalog",
     script: str,
     dataset_name: str,
     parallel: Optional[int] = None,
 ) -> None:
     with open(script, encoding="utf-8") as f:
         script_content = f.read()
     if parallel is not None:
         # This also sets this environment variable for any subprocesses
         os.environ["DVCX_SETTINGS_PARALLEL"] = str(parallel)
-    _, script_output = catalog.query(script_content)
+    _, _, script_output = catalog.query(script_content)
     print(script_output)
 
 
-def clear_cache():
-    get_catalog().cache.clear()
+def clear_cache(catalog: "Catalog"):
+    catalog.cache.clear()
 
 
 def completion(shell: str) -> str:
     return shtab.complete(
         get_parser(),
         shell=shell,
     )
@@ -781,23 +795,29 @@
     # Required for Windows multiprocessing support
     freeze_support()
 
     parser = get_parser()
     args = parser.parse_args(argv)
 
     if args.internal_run_udf:
+        from dvcx.query.dispatch import udf_entrypoint
+
         return udf_entrypoint()
 
     if args.internal_run_udf_worker:
+        from dvcx.query.dispatch import udf_worker_entrypoint
+
         return udf_worker_entrypoint()
 
     if args.command is None:
         parser.print_help()
         return 1
 
+    from .catalog import get_catalog
+
     logger.addHandler(logging.StreamHandler())
     logging_level = get_logging_level(args)
     logger.setLevel(logging_level)
 
     client_config = {
         "aws_endpoint_url": args.aws_endpoint_url,
         "aws_anon": args.aws_anon,
@@ -864,28 +884,30 @@
                 long=bool(args.long),
                 remote=args.remote,
                 ttl=args.ttl,
                 update=bool(args.update),
                 client_config=client_config,
             )
         elif args.command == "ls-datasets":
-            ls_datasets()
+            ls_datasets(catalog)
         elif args.command == "ls-dataset-rows":
-            ls_dataset_rows(args.name, args.version)
+            ls_dataset_rows(catalog, args.name, args.version)
         elif args.command == "rm-dataset":
-            rm_dataset(args.name, version=args.version, force=args.force)
+            rm_dataset(catalog, args.name, version=args.version, force=args.force)
         elif args.command == "dataset-stats":
             dataset_stats(
+                catalog,
                 args.name,
                 args.version,
                 show_bytes=args.bytes,
                 si=args.si,
             )
         elif args.command == "du":
             du(
+                catalog,
                 args.sources,
                 show_bytes=args.bytes,
                 depth=args.depth,
                 si=args.si,
                 ttl=args.ttl,
                 update=bool(args.update),
                 client_config=client_config,
@@ -925,15 +947,15 @@
         elif args.command == "query":
             query(catalog, args.script, args.parallel)
         elif args.command == "apply-udf":
             catalog.apply_udf(
                 args.udf, args.source, args.target, args.parallel, args.udf_params
             )
         elif args.command == "clear-cache":
-            clear_cache()
+            clear_cache(catalog)
         else:
             print(f"invalid command: {args.command}", file=sys.stderr)
             return 1
         return 0
     except BrokenPipeError:
         # Python flushes standard streams on exit; redirect remaining output
         # to devnull to avoid another BrokenPipeError at shutdown
```

### Comparing `dvcx-0.71.0/src/dvcx/cli_utils.py` & `dvcx-0.72.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/client/azure.py` & `dvcx-0.72.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/client/fileslice.py` & `dvcx-0.72.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/client/fsspec.py` & `dvcx-0.72.0/src/dvcx/client/fsspec.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,16 +240,15 @@
     def rel_path(self, path: str) -> str:
         return self.fs.split_path(path)[1]
 
     def get_full_path(self, rel_path: str) -> str:
         return f"{self.PREFIX}{self.name}/{rel_path}"
 
     @abstractmethod
-    def convert_info(self, v: dict[str, Any], parent: str) -> Entry:
-        ...
+    def convert_info(self, v: dict[str, Any], parent: str) -> Entry: ...
 
     def fetch_nodes(
         self,
         nodes,
         shared_progress_bar=None,
     ) -> None:
         fetcher = NodesFetcher(self, self.MAX_THREADS, self.cache)
```

### Comparing `dvcx-0.71.0/src/dvcx/client/gcs.py` & `dvcx-0.72.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/client/local.py` & `dvcx-0.72.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/client/s3.py` & `dvcx-0.72.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.72.0/src/dvcx/data_storage/db_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    ClassVar,
-    Optional,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Union
 
 import sqlalchemy as sa
 from attrs import frozen
 from sqlalchemy.sql.roles import DDLRole
 
+from dvcx.data_storage.serializer import Serializable
+
 if TYPE_CHECKING:
     from sqlalchemy import MetaData, Table
     from sqlalchemy.engine.base import Engine
     from sqlalchemy.engine.interfaces import Dialect
     from sqlalchemy.sql.compiler import Compiled
     from sqlalchemy.sql.elements import ClauseElement
 
@@ -26,31 +21,24 @@
 
 RANDOM_BITS = 63  # size of the random integer field
 
 SELECT_BATCH_SIZE = 100_000  # number of rows to fetch at a time
 
 
 @frozen
-class DatabaseEngine(ABC):
+class DatabaseEngine(ABC, Serializable):
     dialect: ClassVar["Dialect"]
 
     engine: "Engine"
     metadata: "MetaData"
 
     @abstractmethod
     def clone(self) -> "DatabaseEngine":
         """Clones DatabaseEngine implementation."""
 
-    @abstractmethod
-    def clone_params(self) -> tuple[Callable[..., Any], list[Any], dict[str, Any]]:
-        """
-        Returns the class, args, and kwargs needed to instantiate a cloned copy of this
-        DatabaseEngine implementation, for use in separate processes or machines.
-        """
-
     @classmethod
     def compile(cls, statement: "ClauseElement", **kwargs) -> "Compiled":
         """
         Compile a sqlalchemy query or ddl object to a Compiled object.
 
         Use the `string` and `params` properties of this object to get
         the resulting sql string and parameters.
@@ -81,49 +69,40 @@
 
     @abstractmethod
     def execute(
         self,
         query,
         cursor: Optional[Any] = None,
         conn: Optional[Any] = None,
-    ) -> Iterator[tuple[Any, ...]]:
-        ...
+    ) -> Iterator[tuple[Any, ...]]: ...
 
     @abstractmethod
     def executemany(
         self, query, params, cursor: Optional[Any] = None
-    ) -> Iterator[tuple[Any, ...]]:
-        ...
+    ) -> Iterator[tuple[Any, ...]]: ...
 
     @abstractmethod
-    def execute_str(self, sql: str, parameters=None) -> Iterator[tuple[Any, ...]]:
-        ...
+    def execute_str(self, sql: str, parameters=None) -> Iterator[tuple[Any, ...]]: ...
 
     @abstractmethod
-    def insert_dataframe(self, table_name: str, df) -> int:
-        ...
+    def insert_dataframe(self, table_name: str, df) -> int: ...
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     @abstractmethod
-    def transaction(self):
-        ...
+    def transaction(self): ...
 
     def has_table(self, name: str) -> bool:
         """
         Return True if a table exists with the given name
         """
         return sa.inspect(self.engine).has_table(name)
 
     @abstractmethod
-    def create_table(self, table: "Table", if_not_exists: bool = True) -> None:
-        ...
+    def create_table(self, table: "Table", if_not_exists: bool = True) -> None: ...
 
     @abstractmethod
-    def drop_table(self, table: "Table", if_exists: bool = False) -> None:
-        ...
+    def drop_table(self, table: "Table", if_exists: bool = False) -> None: ...
 
     @abstractmethod
-    def rename_table(self, old_name: str, new_name: str):
-        ...
+    def rename_table(self, old_name: str, new_name: str): ...
```

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.72.0/src/dvcx/data_storage/id_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,63 @@
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Callable, Optional
+from typing import TYPE_CHECKING, Optional
 
 from sqlalchemy import Column, Integer, Table, Text
 
+from dvcx.data_storage.serializer import Serializable
+
 if TYPE_CHECKING:
     from sqlalchemy.schema import SchemaItem
 
     from dvcx.data_storage.db_engine import DatabaseEngine
 
 
 logger = logging.getLogger("dvcx")
 
 
-class AbstractIDGenerator(ABC):
+class AbstractIDGenerator(ABC, Serializable):
+    """
+    Abstract ID Generator class. This class is responsible for generating
+    unique IDs for each prefix (e.g. S3 bucket or dataset).
+    """
+
+    @abstractmethod
+    def clone(self) -> "AbstractIDGenerator":
+        """Clones AbstractIDGenerator implementation."""
+
+    def init(self) -> None:  # noqa: B027
+        """Initialize ID generator."""
+
+    def cleanup_for_tests(self):  # noqa: B027
+        """Cleanup for tests."""
+
+    @abstractmethod
+    def init_id(self, uri: str) -> None:
+        """Initializes the ID generator for the given URI with zero last_id."""
+
+    @abstractmethod
+    def get_next_ids(self, uri: str, count: int) -> range:
+        """Returns a range of IDs for the given URI."""
+
+    def get_next_id(self, uri: str) -> int:
+        """Returns the next ID for the given URI."""
+        return self.get_next_ids(uri, 1)[0]
+
+    def delete_uri(self, uri: str):  # noqa: B027
+        """Deletes the given URI."""
+        self.delete_uris([uri])
+
+    def delete_uris(self, uris: Iterable[str]):  # noqa: B027
+        """Deletes the given URIs."""
+
+
+class AbstractDBIDGenerator(AbstractIDGenerator):
     """
     Abstract ID Generator class, to be implemented by any Database Adapters
     for a specific database system. This class is responsible for generating
     unique IDs for each prefix (e.g. S3 bucket or dataset) and storing them
     in a database. It is also responsible for initializing the database
     and creating the necessary tables.
     """
@@ -35,28 +73,20 @@
         table_prefix: Optional[str] = None,
         skip_db_init: bool = False,
     ):
         self._db = db
         self._table_prefix = table_prefix
         self._skip_db_init = skip_db_init
         if db and not skip_db_init:
-            self.init_db()
+            self.init()
 
     @abstractmethod
-    def clone(self) -> "AbstractIDGenerator":
+    def clone(self) -> "AbstractDBIDGenerator":
         """Clones AbstractIDGenerator implementation."""
 
-    @abstractmethod
-    def clone_params(self) -> tuple[Callable[..., Any], list[Any], dict[str, Any]]:
-        """
-        Returns the function, args, and kwargs needed to instantiate a cloned copy
-        of this AbstractIDGenerator implementation, for use in separate processes
-        or machines.
-        """
-
     @property
     def db(self) -> "DatabaseEngine":
         return self._db
 
     @property
     def _columns(self) -> list["SchemaItem"]:
         return [
@@ -68,33 +98,25 @@
     @cached_property
     def _table(self) -> Table:
         table_name = self._base_table_name
         if self._table_prefix:
             table_name = f"{self._table_prefix}_{table_name}"
         return Table(table_name, self.db.metadata, *self._columns, extend_existing=True)
 
-    def init_db(self) -> None:
+    def init(self) -> None:
         self.db.create_table(self._table, if_not_exists=True)
 
     def cleanup_for_tests(self):
         """Cleanup for tests."""
         self.db.drop_table(self._table, if_exists=True)
 
     @abstractmethod
     def init_id(self, uri: str) -> None:
         """Initializes the ID generator for the given URI with zero last_id."""
 
     @abstractmethod
     def get_next_ids(self, uri: str, count: int) -> range:
         """Returns a range of IDs for the given URI."""
 
-    def get_next_id(self, uri: str) -> int:
-        """Returns the next ID for the given URI."""
-        return self.get_next_ids(uri, 1)[0]
-
-    def delete_uri(self, uri: str):
-        """Deletes the given URI from the database."""
-        self.db.execute(self._table.delete().where(self._table.c.uri == uri))
-
     def delete_uris(self, uris: Iterable[str]):
         """Deletes the given URIs from the database."""
         self.db.execute(self._table.delete().where(self._table.c.uri.in_(uris)))
```

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.72.0/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 import logging
 import posixpath
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from datetime import datetime, timezone
 from functools import cached_property, reduce
 from itertools import groupby
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Optional,
-)
+from typing import TYPE_CHECKING, Any, Optional
 
 from sqlalchemy import (
     JSON,
     Boolean,
     Column,
     DateTime,
     ForeignKey,
@@ -25,14 +20,15 @@
     Table,
     Text,
     UniqueConstraint,
     select,
 )
 from sqlalchemy.sql import func
 
+from dvcx.data_storage.serializer import Serializable
 from dvcx.dataset import DatasetDependency, DatasetRecord, DatasetVersion
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, StorageNotFoundError
 from dvcx.sql.types import SQLType
 from dvcx.storage import Status as StorageStatus
 from dvcx.storage import Storage, StorageURI
 from dvcx.utils import is_expired
@@ -43,15 +39,15 @@
     from dvcx.data_storage import AbstractIDGenerator, schema
     from dvcx.data_storage.db_engine import DatabaseEngine
 
 
 logger = logging.getLogger("dvcx")
 
 
-class AbstractMetastore(ABC):
+class AbstractMetastore(ABC, Serializable):
     """
     Abstract Metastore class.
     This manages the storing, searching, and retrieval of indexed metadata.
     """
 
     uri: StorageURI
     partial_id: Optional[int]
@@ -71,21 +67,14 @@
 
     @abstractmethod
     def clone(
         self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
     ) -> "AbstractMetastore":
         """Clones AbstractMetastore implementation for some Storage input."""
 
-    @abstractmethod
-    def clone_params(self) -> tuple[Callable[..., Any], list[Any], dict[str, Any]]:
-        """
-        Returns the class, args, and kwargs needed to instantiate a cloned copy of this
-        AbstractMetastore implementation, for use in separate processes or machines.
-        """
-
     def init(self, uri: StorageURI, partial_id: int) -> None:  # noqa: B027
         """Initialize metastore."""
 
     def close(self) -> None:  # noqa: B027
         """Closes any active database or HTTP connections."""
 
     def cleanup_temp_tables(self, temp_table_names: list[str]):  # noqa: B027
@@ -568,73 +557,68 @@
         )
 
     #
     # Query Starters (These can be overridden by subclasses)
     #
 
     @abstractmethod
-    def _storages_insert(self):
-        ...
+    def _storages_insert(self): ...
 
     def _storages_select(self, *columns):
         if not columns:
             return self._storages.select()
         return select(*columns).select_from(self._storages)
 
     def _storages_update(self):
         return self._storages.update()
 
     def _storages_delete(self):
         return self._storages.delete()
 
     @abstractmethod
-    def _partials_insert(self):
-        ...
+    def _partials_insert(self): ...
 
     def _partials_select(self, *columns):
         if not columns:
             return self._partials.select()
         return select(*columns).select_from(self._partials)
 
     def _partials_update(self):
         return self._partials.update()
 
     @abstractmethod
-    def _datasets_insert(self):
-        ...
+    def _datasets_insert(self): ...
 
     def _datasets_select(self, *columns):
         if not columns:
             return self._datasets.select()
         return select(*columns).select_from(self._datasets)
 
     def _datasets_update(self):
         return self._datasets.update()
 
     def _datasets_delete(self):
         return self._datasets.delete()
 
     @abstractmethod
-    def _datasets_versions_insert(self):
-        ...
+    def _datasets_versions_insert(self): ...
 
     def _datasets_versions_select(self, *columns):
         if not columns:
             return self._datasets_versions.select()
         return select(*columns).select_from(self._datasets_versions)
 
     def _datasets_versions_update(self):
         return self._datasets_versions.update()
 
     def _datasets_versions_delete(self):
         return self._datasets_versions.delete()
 
     @abstractmethod
-    def _datasets_dependencies_insert(self):
-        ...
+    def _datasets_dependencies_insert(self): ...
 
     def _datasets_dependencies_select(self, *columns):
         if not columns:
             return self._datasets_dependencies.select()
         return select(*columns).select_from(self._datasets_dependencies)
 
     def _datasets_dependencies_update(self):
```

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/schema.py` & `dvcx-0.72.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.72.0/src/dvcx/data_storage/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from sqlalchemy.schema import CreateIndex, CreateTable, DropTable
 from sqlalchemy.sql import func
 from sqlalchemy.sql.expression import bindparam, cast
 
 import dvcx.sql.sqlite
 from dvcx.data_storage import AbstractDBMetastore, AbstractWarehouse
 from dvcx.data_storage.db_engine import DatabaseEngine
-from dvcx.data_storage.id_generator import AbstractIDGenerator
+from dvcx.data_storage.id_generator import AbstractDBIDGenerator
 from dvcx.data_storage.schema import (
     DefaultSchema,
     SignalsTable,
     convert_rows_custom_column_types,
 )
 from dvcx.dataset import DatasetRecord
 from dvcx.error import DVCXError, InconsistentSignalType
@@ -215,29 +215,29 @@
 
     def rename_table(self, old_name: str, new_name: str):
         comp_old_name = quote_schema(old_name)
         comp_new_name = quote_schema(new_name)
         self.execute_str(f"ALTER TABLE {comp_old_name} RENAME TO {comp_new_name}")
 
 
-class SQLiteIDGenerator(AbstractIDGenerator):
+class SQLiteIDGenerator(AbstractDBIDGenerator):
     _db: "SQLiteDatabaseEngine"
 
     def __init__(
         self,
         db: Optional["SQLiteDatabaseEngine"] = None,
         table_prefix: Optional[str] = None,
         skip_db_init: bool = False,
         db_file: Optional[str] = None,
     ):
         db = db or SQLiteDatabaseEngine.from_db_file(db_file)
 
         super().__init__(db, table_prefix, skip_db_init)
 
-    def clone(self) -> "AbstractIDGenerator":
+    def clone(self) -> "SQLiteIDGenerator":
         """Clones SQLiteIDGenerator implementation."""
         return SQLiteIDGenerator(
             self._db.clone(), self._table_prefix, skip_db_init=True
         )
 
     def clone_params(self) -> tuple[Callable[..., Any], list[Any], dict[str, Any]]:
         """
@@ -245,31 +245,31 @@
         of this SQLiteIDGenerator implementation, for use in separate processes
         or machines.
         """
         return (
             SQLiteIDGenerator.init_after_clone,
             [],
             {
-                "db_params": self._db.clone_params(),
+                "db_clone_params": self._db.clone_params(),
                 "table_prefix": self._table_prefix,
             },
         )
 
     @classmethod
     def init_after_clone(
         cls,
         *,
-        db_params: tuple[Callable, list, dict[str, Any]],
+        db_clone_params: tuple[Callable, list, dict[str, Any]],
         table_prefix: Optional[str] = None,
     ) -> "SQLiteIDGenerator":
         """
         Initializes a new instance of this SQLiteIDGenerator implementation
         using the given parameters, which were obtained from a call to clone_params.
         """
-        (db_class, db_args, db_kwargs) = db_params
+        (db_class, db_args, db_kwargs) = db_clone_params
         return cls(
             db=db_class(*db_args, **db_kwargs),
             table_prefix=table_prefix,
             skip_db_init=True,
         )
 
     @property
@@ -336,19 +336,20 @@
 
 class SQLiteMetastore(AbstractDBMetastore):
     """
     SQLite Metastore uses SQLite3 for storing indexed data locally.
     This is currently used for the local cli.
     """
 
+    id_generator: "SQLiteIDGenerator"
     db: "SQLiteDatabaseEngine"
 
     def __init__(
         self,
-        id_generator: "AbstractIDGenerator",
+        id_generator: "SQLiteIDGenerator",
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
         db: Optional["SQLiteDatabaseEngine"] = None,
         db_file: Optional[str] = None,
     ):
         self.schema: "DefaultSchema" = DefaultSchema()
         super().__init__(id_generator, uri, partial_id)
@@ -384,36 +385,36 @@
         Returns the class, args, and kwargs needed to instantiate a cloned copy of this
         SQLiteDataStorage implementation, for use in separate processes or machines.
         """
         return (
             SQLiteMetastore.init_after_clone,
             [],
             {
-                "id_generator_params": self.id_generator.clone_params(),
+                "id_generator_clone_params": self.id_generator.clone_params(),
                 "uri": self.uri,
                 "partial_id": self.partial_id,
-                "db_params": self.db.clone_params(),
+                "db_clone_params": self.db.clone_params(),
             },
         )
 
     @classmethod
     def init_after_clone(
         cls,
         *,
-        id_generator_params: tuple[Callable, list, dict[str, Any]],
+        id_generator_clone_params: tuple[Callable, list, dict[str, Any]],
         uri: StorageURI,
         partial_id: Optional[int],
-        db_params: tuple[Callable, list, dict[str, Any]],
+        db_clone_params: tuple[Callable, list, dict[str, Any]],
     ) -> "SQLiteMetastore":
         (
             id_generator_class,
             id_generator_args,
             id_generator_kwargs,
-        ) = id_generator_params
-        (db_class, db_args, db_kwargs) = db_params
+        ) = id_generator_clone_params
+        (db_class, db_args, db_kwargs) = db_clone_params
         return cls(
             id_generator=id_generator_class(*id_generator_args, **id_generator_kwargs),
             uri=uri,
             partial_id=partial_id,
             db=db_class(*db_args, **db_kwargs),
         )
 
@@ -497,22 +498,23 @@
 
 class SQLiteWarehouse(AbstractWarehouse):
     """
     SQLite Warehouse uses SQLite3 for storing indexed data locally.
     This is currently used for the local cli.
     """
 
+    id_generator: "SQLiteIDGenerator"
     db: "SQLiteDatabaseEngine"
 
     # Cache for our defined column types to dialect specific TypeEngine relations
     _col_python_type: dict[type, "TypeEngine"] = {}
 
     def __init__(
         self,
-        id_generator: "AbstractIDGenerator",
+        id_generator: "SQLiteIDGenerator",
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
         db: Optional["SQLiteDatabaseEngine"] = None,
         db_file: Optional[str] = None,
     ):
         self.schema: "DefaultSchema" = DefaultSchema()
         super().__init__(id_generator, uri, partial_id)
@@ -548,36 +550,36 @@
         Returns the class, args, and kwargs needed to instantiate a cloned copy of this
         SQLiteDataStorage implementation, for use in separate processes or machines.
         """
         return (
             SQLiteWarehouse.init_after_clone,
             [],
             {
-                "id_generator_params": self.id_generator.clone_params(),
+                "id_generator_clone_params": self.id_generator.clone_params(),
                 "uri": self.uri,
                 "partial_id": self.partial_id,
-                "db_params": self.db.clone_params(),
+                "db_clone_params": self.db.clone_params(),
             },
         )
 
     @classmethod
     def init_after_clone(
         cls,
         *,
-        id_generator_params: tuple[Callable, list, dict[str, Any]],
+        id_generator_clone_params: tuple[Callable, list, dict[str, Any]],
         uri: StorageURI,
         partial_id: Optional[int],
-        db_params: tuple[Callable, list, dict[str, Any]],
+        db_clone_params: tuple[Callable, list, dict[str, Any]],
     ) -> "SQLiteWarehouse":
         (
             id_generator_class,
             id_generator_args,
             id_generator_kwargs,
-        ) = id_generator_params
-        (db_class, db_args, db_kwargs) = db_params
+        ) = id_generator_clone_params
+        (db_class, db_args, db_kwargs) = db_clone_params
         return cls(
             id_generator=id_generator_class(*id_generator_args, **id_generator_kwargs),
             uri=uri,
             partial_id=partial_id,
             db=db_class(*db_args, **db_kwargs),
         )
```

### Comparing `dvcx-0.71.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.72.0/src/dvcx/data_storage/warehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,25 @@
+import json
 import logging
 import posixpath
 from abc import ABC, abstractmethod
 from collections.abc import Generator, Iterable, Iterator, Sequence
 from random import getrandbits
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Optional,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Optional, Union
 from urllib.parse import urlparse
 
 import attrs
 import sqlalchemy as sa
-from sqlalchemy import (
-    Table,
-    and_,
-    case,
-    select,
-)
+from sqlalchemy import Table, and_, case, select
 from sqlalchemy.sql import func
 from sqlalchemy.sql.expression import true
 
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES, SignalsTable
 from dvcx.data_storage.schema import Node as NodeTable
+from dvcx.data_storage.serializer import Serializable
 from dvcx.dataset import DatasetRecord, DatasetRow
 from dvcx.node import DirTypeGroup, Entry, Node, NodeWithPath, get_path
 from dvcx.sql.types import Int, SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import GLOB_CHARS, sql_escape_like
 
 if TYPE_CHECKING:
@@ -54,15 +45,15 @@
 
 # special string to wrap around dataset name in a user query script stdout, which
 # is run in a Python subprocess, so that we can find it later on after script is
 # done since there is no other way to return results from it
 PYTHON_SCRIPT_WRAPPER_CODE = "__ds__"
 
 
-class AbstractWarehouse(ABC):
+class AbstractWarehouse(ABC, Serializable):
     """
     Abstract Warehouse class, to be implemented by any Database Adapters
     for a specific database system. This manages the storing, searching, and
     retrieval of datasets data, and has shared logic for all database
     systems currently in use.
     """
 
@@ -114,41 +105,43 @@
                 item_pyton_type = self.python_type(col_type.item_type)
                 if item_pyton_type != list:
                     if isinstance(val[0], item_pyton_type):
                         return val
                     if item_pyton_type == float and isinstance(val[0], int):
                         return [float(i) for i in val]
                 return [self.convert_type(i, col_type.item_type) for i in val]
+            # special use case with JSON type as we save it as string
+            if col_python_type == dict:
+                if value_type == str:
+                    return val
+                elif value_type in (dict, list):
+                    return json.dumps(val)
+                else:
+                    raise ValueError(
+                        f"Cannot convert value {val!r} with type"
+                        f"{value_type} to JSON"
+                    )
+
             if isinstance(val, col_python_type):
                 return val
             if col_python_type == float and isinstance(val, int):
                 return float(val)
-            # special use case with JSON type as we save it as string
-            if col_python_type == dict and value_type == str:
-                return val
         except Exception as e:
             exc = e
         raise ValueError(
             f"Value {val!r} with type {value_type} incompatible for "
             f"column type {type(col_type).__name__}"
         ) from exc
 
     @abstractmethod
     def clone(
         self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
     ) -> "AbstractWarehouse":
         """Clones Warehouse implementation for some Storage input"""
 
-    @abstractmethod
-    def clone_params(self) -> tuple[Callable[..., Any], list[Any], dict[str, Any]]:
-        """
-        Returns the class, args, and kwargs needed to instantiate a cloned copy of this
-        AbstractWarehouse implementation, for use in separate processes or machines.
-        """
-
     def close(self) -> None:
         """Closes any active database connections."""
         self.db.close()
 
     @abstractmethod
     def init_db(self, uri: StorageURI, partial_id: int) -> None:
         """Initializes database tables for warehouse"""
@@ -205,15 +198,15 @@
         """
         cols = query.selected_columns
         cols_names = [c.name for c in cols]
 
         if not order_by:
             ordering = [cols.source, cols.parent, cols.name, cols.version, cols.etag]
         else:
-            ordering = [cols[c] for c in order_by]
+            ordering = order_by  # type: ignore
 
         # reset query order by and apply new order by id
         paginated_query = query.order_by(None).order_by(*ordering).limit(page_size)
 
         offset = 0
         num_yielded = 0
         while True:
@@ -315,16 +308,15 @@
         Method for fetching dataset rows from database. This is abstract since
         in some DBs we need to use special settings
         """
 
     @abstractmethod
     def get_dataset_sources(
         self, dataset: DatasetRecord, version: int
-    ) -> list[StorageURI]:
-        ...
+    ) -> list[StorageURI]: ...
 
     def get_dataset_rows(
         self,
         dataset: DatasetRecord,
         version: int,
         offset: Optional[int] = 0,
         limit: Optional[int] = 20,
@@ -871,20 +863,23 @@
         n = self.nodes_table(uri, partial_id)
         query = select(sa.func.count(), sa.func.sum(n.c.size)).select_from(
             n.get_table()
         )
         (res,) = self.db.execute(query)
         return res[0], res[1]
 
-    def return_ds_hook(self, name: str) -> None:  # noqa: B027
+    def return_ds_hook(self, name: str, version: int) -> None:
         """
         Hook to be run when a return ds is ready to be saved in a
         DatasetQuery script.
         """
-        print(f"{PYTHON_SCRIPT_WRAPPER_CODE}{name}{PYTHON_SCRIPT_WRAPPER_CODE}")
+        print(
+            f"{PYTHON_SCRIPT_WRAPPER_CODE}{name}{PYTHON_SCRIPT_WRAPPER_CODE}"
+            f"{version}{PYTHON_SCRIPT_WRAPPER_CODE}"
+        )
 
     def create_udf_table(
         self,
         name: str,
         custom_columns: Sequence["sa.Column"] = (),
     ) -> "sa.Table":
         """
```

### Comparing `dvcx-0.71.0/src/dvcx/dataset.py` & `dvcx-0.72.0/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/error.py` & `dvcx-0.72.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/dataset.py` & `dvcx-0.72.0/src/dvcx/lib/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import inspect
 from collections.abc import Sequence
 from typing import Callable, Optional, Union
 
+import sqlalchemy
 from sqlalchemy.sql.elements import ColumnElement
 
+from dvcx.lib.feature import Feature, FeatureClass
 from dvcx.lib.udf import (
     Aggregator,
     BatchMapper,
     Generator,
     GroupMapper,
     Mapper,
     UDFBase,
 )
-from dvcx.query.dataset import DatasetQuery, PartitionByType
+from dvcx.query.dataset import DatasetQuery, JoinPredicateType, PartitionByType, detach
 from dvcx.query.schema import Column
 
 C = Column
 
 
 class Dataset(DatasetQuery):
     """DVCX DataFrame is a 2-dimensional table of rows and columns designed to work
@@ -306,7 +308,74 @@
             msg = (
                 f"'partition_by' argument must be PartitionByType or None"
                 f", {partition_by.__class__.__name__} was given"
             )
 
         if msg:
             raise TypeError(f"Dataset {name} error: {msg}")
+
+    def _args_to_columns(self, *args):
+        return [column for arg in args for column in self._feature_to_columns(arg)]
+
+    @staticmethod
+    def _feature_to_columns(fr: Union[C, FeatureClass, str]):
+        if isinstance(fr, str):
+            return [C(fr)]
+
+        if isinstance(fr, C):
+            return [fr]
+
+        if not issubclass(fr, Feature):
+            raise TypeError(f"feature or column '{fr}' has a wrong type '{type(fr)}'")
+
+        spec = fr._to_udf_spec()
+        return [C(name) for (name, typ) in spec]
+
+    def _extend_features(self, method_name, *args):
+        super_func = getattr(super(), method_name)
+
+        columns = self._args_to_columns(*args)
+        res = super_func(self, *columns)
+        return res
+
+    @detach
+    def select(self, *args) -> "Dataset":
+        return self._extend_features("select", *args)
+
+    @detach
+    def select_except(self, *args) -> "Dataset":
+        return self._extend_features("select_except", *args)
+
+    @detach
+    def merge(
+        self,
+        right_ds: "Dataset",
+        on: Union[JoinPredicateType, Sequence[JoinPredicateType]],
+        right_on: Union[JoinPredicateType, Sequence[JoinPredicateType]] = None,
+        inner=False,
+        rname="{name}_right",
+    ) -> "Dataset":
+        if on is None:
+            raise ValueError("'on' must be specified in merge()")
+
+        on = [on] if not isinstance(on, (list, tuple)) else on
+        on_columns = [cols for item in on for cols in self._args_to_columns(item)]
+
+        if right_on is not None:
+            right_on = (
+                [right_on] if not isinstance(right_on, (list, tuple)) else right_on
+            )
+            right_on_columns = [
+                cols for item in right_on for cols in self._args_to_columns(item)
+            ]
+
+            if len(right_on_columns) != len(on_columns):
+                raise ValueError("'on' and 'right_on' must have the same length'")
+        else:
+            right_on_columns = on_columns
+
+        ops = [
+            self.c(left) == right_ds.c(right)
+            for left, right in zip(on_columns, right_on_columns)
+        ]
+
+        return self.join(right_ds, sqlalchemy.and_(*ops), inner, rname)
```

### Comparing `dvcx-0.71.0/src/dvcx/lib/feature.py` & `dvcx-0.72.0/src/dvcx/lib/feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import inspect
 import re
+import warnings
 from collections.abc import Sequence
 from datetime import datetime
 from types import GenericAlias
 from typing import ClassVar, Union, get_args, get_origin
 
 import attrs
 from pydantic import BaseModel
 
-from dvcx.lib.dataset import C
+from dvcx.query import C
 from dvcx.query.udf import UDFOutputSpec
 from dvcx.sql.types import JSON, Array, Binary, Boolean, DateTime, Float, Int, String
 
 TYPE_TO_DVCX = {
     int: Int,
     str: String,
     float: Float,
@@ -23,23 +24,31 @@
     dict: JSON,
 }
 
 FeatureClass = type["Feature"]
 FeatureClassSeq = Sequence[FeatureClass]
 
 
+# Disable Pydantic warning, see https://github.com/iterative/dvcx/issues/1285
+warnings.filterwarnings(
+    "ignore",
+    message="Field name .* shadows an attribute in parent",
+    category=UserWarning,
+)
+
+
 class Feature(BaseModel):
     """A base class for defining data classes that serve as inputs and outputs for
     DataFrame processing functions like `map()`, `generate()`, etc. Inherits from
     `pydantic`'s BaseModel, allowing for data validation and definition.
     """
 
     _expand_name: ClassVar[bool] = True
     _delimiter: ClassVar[str] = "__"
-    _is_stream: ClassVar[bool] = False
+    _is_file: ClassVar[bool] = False
 
     @classmethod
     def __pydantic_init_subclass__(cls):
         for name, field_info in cls.model_fields.items():
             attr_value = _resolve(cls, name, field_info, cls._prefix())
             setattr(cls, name, RestrictedAttribute(attr_value, cls, name))
 
@@ -237,19 +246,19 @@
     return FeatureAttributeWrapper(anno, new_prefix_value)
 
 
 class ShallowFeature(Feature):
     _expand_name: ClassVar[bool] = False
 
 
-class StreamFeature(ShallowFeature):
-    _is_stream = True
+class FileFeature(ShallowFeature):
+    _is_file = True
 
     def __init__(self, **kwarg):
         super().__init__(**kwarg)
         self._stream = None
 
-    def set_stream(self, stream):
+    def set_file(self, stream):
         self._stream = stream
 
     def open(self):
         return self._stream
```

### Comparing `dvcx-0.71.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.72.0/src/dvcx/lib/feature_udf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,75 @@
+import inspect
+import sys
+import traceback
 from collections.abc import Sequence
-from typing import Union
+from typing import Optional, Union
 
 from dvcx.catalog import get_catalog
 from dvcx.lib.feature import Feature, FeatureClass, FeatureClassSeq
-from dvcx.lib.udf import Aggregator, BatchMapper, Generator, Mapper
+from dvcx.lib.udf import Aggregator, BatchMapper, Generator, Mapper, UDFBase
+from dvcx.lib.utils import DvcxError
 from dvcx.query import Stream
 
 
+class ValidationError(DvcxError):
+    pass
+
+
+class SchemaError(ValidationError):
+    def __init__(self, udf_name: str, context: str, message: str):
+        super().__init__(
+            f"'{udf_name}' {context} " f"schema validation error: {message}"
+        )
+
+
+class OutputError(ValidationError):
+    def __init__(self, udf_name: str, message: str, num: Optional[int] = None):
+        num_str = "" if num is None else f"#{num + 1} "
+        super().__init__(f"Output {num_str}of '{udf_name}' error: {message}")
+
+
+class UserCodeError(DvcxError):
+    def __init__(self, class_name: str, message: str):
+        super().__init__(f"Error in user code in class '{class_name}': {message}")
+
+
 class FeatureConvertor:
     @property
     def udf_params_list(self):
         return self._udf_params_list
 
     @property
     def udf_output_spec(self):
         return self._udf_output_spec
 
     @property
-    def is_single_input(self):
-        return self._is_single_input
-
-    @property
-    def is_single_output(self):
-        return self._is_single_output
-
-    @property
     def has_stream(self):
         return self._has_stream
 
     @property
     def cache(self):
         return self._cache
 
     def __init__(
         self,
+        udf: UDFBase,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
-        is_input_batched: bool = True,
     ):
-        self._is_input_batched = is_input_batched
+        self._udf = udf
 
         self._inputs, self._is_single_input = self._convert_to_sequence(inputs)
         self._outputs, self._is_single_output = self._convert_to_sequence(outputs)
 
         self._validate_schema("params", self._inputs)
         self._validate_schema("output", self._outputs)
 
         self._has_stream = any(
-            f._is_stream  # type: ignore[attr-defined]
+            f._is_file  # type: ignore[attr-defined]
             for f in self._inputs
         )
         self._cache = get_catalog().cache
 
         udf_params_spec = Feature._features_to_udf_spec(self._inputs)
         stream_prm = [Stream()] if self._has_stream else []
         self._udf_params_list = stream_prm + list(udf_params_spec.keys())
@@ -66,138 +84,168 @@
             return [arg], True
         else:
             return arg, False
 
     def deserialize_objs(self, params, args):
         streams = []
         if self._has_stream:
-            for row in args:
-                streams.append(row.pop(0))
+            streams = [arg[0] for arg in args]
+            args = [arg[1:] for arg in args]
 
         obj_rows = [self._params_to_objects(params, arg) for arg in args]
         for row, stream in zip(obj_rows, streams):
             for feature in row:
-                if feature._is_stream:
-                    feature.set_stream(stream)
+                if feature._is_file:
+                    feature.set_file(stream)
                     feature.set_cache(self._cache)
 
         return obj_rows
 
     def _params_to_objects(self, params, args):
         new_params = params if not self._has_stream else params[1:]
         return [cls._unflatten(dict(zip(new_params, args))) for cls in self._inputs]
 
     def _validate_schema(self, context: str, features: FeatureClassSeq):
         for type_ in features:
             if not isinstance(type_, type):
-                raise ValueError(
-                    f"{self.__class__.__name__} does not accept instances as"
-                    f" {context}. A class must be provided"
+                raise SchemaError(
+                    self._udf.name,
+                    context,
+                    "cannot accept objects, a 'Feature' class must be provided",
                 )
             if not issubclass(type_, Feature):
-                raise ValueError(
-                    f"{self.__class__.__name__} does not accept {context} "
-                    f"of type {type_}. It must be subclass of Feature"
+                raise SchemaError(
+                    self._udf.name,
+                    context,
+                    f"cannot accept type '{type_.__name__}', "
+                    f"the type must be a subclass of 'Feature'",
                 )
 
-    def validate_output_obj(self, udf_name, result_objs, *args, **kwargs):
+    def validate_output_obj(self, result_objs, *args, **kwargs):
         for row in result_objs:
+            if not isinstance(row, (list, tuple)) and isinstance(
+                self._outputs, (list, tuple)
+            ):
+                raise OutputError(
+                    self._udf.name,
+                    f"expected list of objects, "
+                    f"but found a single value of type '{type(row).__name__}'",
+                )
+
             if len(row) != len(self._outputs):
-                raise RuntimeError(
-                    f"Output of {udf_name} must have {len(self._outputs)} objects"
-                    f" while {len(row)} were provided"
+                raise OutputError(
+                    self._udf.name,
+                    f"length mismatch - expected {len(self._outputs)} "
+                    f"objects, but {len(row)} were provided",
                 )
 
             for num, (o, type_) in enumerate(zip(row, self._outputs)):
                 if not isinstance(o, type_):
-                    raise RuntimeError(
-                        f"Expected output {num} output of {udf_name} to be"
-                        f" '{type_.__name__}', but found type '{type(o).__name__}'"
+                    raise OutputError(
+                        self._udf.name,
+                        f"expected type '{type_.__name__}',"
+                        f" but found type '{type(o).__name__}'",
+                        num=num,
                     )
 
-    def process_rows(self, udf, rows):
-        obj_rows = self.deserialize_objs(udf.params, rows)
-        if self.is_single_input:
+    def process_rows(self, rows, is_input_batched=True, is_output_batched=True):
+        obj_rows = self.deserialize_objs(self._udf.params, rows)
+        if self._is_single_input:
             obj_rows = [objs[0] for objs in obj_rows]
 
-        if not self._is_input_batched:
+        if not is_input_batched:
             assert (
                 len(obj_rows) == 1
-            ), f"{udf.name} takes {len(obj_rows)} rows while it's not batched"
+            ), f"{self._udf.name} takes {len(obj_rows)} rows while it's not batched"
             obj_rows = obj_rows[0]
 
-        returned_value = udf.process(obj_rows)
-        if self._is_input_batched:
-            result_objs = list(returned_value)
-        else:
-            result_objs = [returned_value]
+        result_objs = self.run_user_code(obj_rows)
+
+        if not is_output_batched:
+            result_objs = [result_objs]
 
-        if self.is_single_output:
+        if self._is_single_output:
             result_objs = [[x] for x in result_objs]
 
-        self.validate_output_obj(udf.name, result_objs)
+        self.validate_output_obj(result_objs)
 
         res = [Feature._flatten_list(objs) for objs in result_objs]
 
-        if not self._is_input_batched:
+        if not is_output_batched:
             assert len(res) == 1, (
-                f"{udf.__class__.__name__} returns {len(obj_rows)} "
+                f"{self._udf.name} returns {len(obj_rows)} "
                 f"rows while it's not batched"
             )
-            return res[0]
+            res = res[0]
         return res
 
+    def run_user_code(self, obj_rows):
+        try:
+            result_objs = self._udf.process(obj_rows)
+            if inspect.isgeneratorfunction(self._udf.process):
+                result_objs = list(result_objs)
+        except Exception as e:
+            msg = (
+                f"============== Error in user code: '{self._udf.name}' =============="
+            )
+            print(msg)
+            exc_type, exc_value, exc_traceback = sys.exc_info()
+            traceback.print_exception(exc_type, exc_value, exc_traceback.tb_next)
+            print("=" * len(msg))
+            raise UserCodeError(self._udf.name, str(e)) from None
+        return result_objs
+
 
 class FeatureAggregator(Aggregator):
     def __init__(
         self,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(inputs, outputs)
+        self._fc = FeatureConvertor(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
-    def __call__(self, args):
-        return self._fc.process_rows(self, args)
+    def __call__(self, rows):
+        return self._fc.process_rows(rows)
 
 
 class FeatureMapper(Mapper):
     def __init__(
         self,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(inputs, outputs, is_input_batched=False)
+        self._fc = FeatureConvertor(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
-    def __call__(self, args):
-        return self._fc.process_rows(self, args)
+    def __call__(self, *row):
+        return self._fc.process_rows([row], False, False)
 
 
 class FeatureBatchMapper(BatchMapper):
     def __init__(
         self,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(inputs, outputs)
+        self._fc = FeatureConvertor(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
-    def __call__(self, args):
-        return self._fc.process_rows(self, args)
+    def __call__(self, rows):
+        return self._fc.process_rows(rows)
 
 
 class FeatureGenerator(Generator):
     def __init__(
         self,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(inputs, outputs)
+        self._fc = FeatureConvertor(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
-    def __call__(self, args):
-        return self._fc.process_rows(self, args)
+    def __call__(self, *row):
+        return self._fc.process_rows([row], False)
```

### Comparing `dvcx-0.71.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.72.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.72.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.72.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/image_transform.py` & `dvcx-0.72.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.72.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/stream.py` & `dvcx-0.72.0/src/dvcx/lib/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from pathlib import Path
 from random import getrandbits
 from typing import Optional
 
 from pydantic import Field
 
 from dvcx.cache import UniqueId
-from dvcx.lib.feature import StreamFeature
+from dvcx.lib.feature import FileFeature
 
 
-class FileStream(StreamFeature):
+class File(FileFeature):
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     version: str = Field(default="")
     etag: str = Field(default="")
     size: int = Field(default=0)
     vtype: str = Field(default="")
-    location: Optional[list[dict]] = Field(default=None)
+    location: Optional[dict] = Field(default=None)
 
     _unique_id_keys = ["source", "parent", "name", "etag", "size", "vtype", "location"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._stream = None
         self._cache = None
@@ -50,19 +50,24 @@
 
     def get_file_ext(self):
         return Path(self.name).suffix.strip(".")
 
     def get_file_stem(self):
         return Path(self.name).stem
 
+    def get_full_name(self):
+        if not self.parent:
+            return self.name
+        return f"{self.parent}/{self.name}"
+
     def get_full_path(self):
-        return f"{self.source}/{self.parent}/{self.name}"
+        return f"{self.source}/{self.get_full_name()}"
 
 
-class FileInfo(StreamFeature):
+class FileInfo(FileFeature):
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     size: int = Field(default=0)
     location: Optional[dict] = Field(default=None)
     vtype: str = Field(default="")
     dir_type: int = Field(default=0)
```

### Comparing `dvcx-0.71.0/src/dvcx/lib/udf.py` & `dvcx-0.72.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/unstructured.py` & `dvcx-0.72.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/lib/utils.py` & `dvcx-0.72.0/src/dvcx/lib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 try:
     import pandas as pd
 except ImportError:
     pd = None
 
 
+class DvcxError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 def row_to_pandas(args, params):
     data = dict(zip([i.name for i in params], args))
     return pd.Series(data, name=data.get("name", None))
 
 
 def row_list_to_pandas(args, params):
     df = pd.DataFrame(args, columns=[i.name for i in params])
```

### Comparing `dvcx-0.71.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.72.0/src/dvcx/lib/webdataset_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,99 @@
+from typing import Optional
+
 import numpy as np
 from pydantic import Field
 
-from dvcx.lib.dataset import C
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import FeatureAggregator
-from dvcx.lib.stream import FileInfo, FileStream
+from dvcx.lib.file import File, FileInfo
+from dvcx.lib.utils import DvcxError
+from dvcx.query import C
 from dvcx.sql.functions import path
 
 try:
     import pandas as pd
 except ImportError:
     pd = None
 
 
+class WDSMetaError(DvcxError):
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
 def parse_wds_meta(ds):
     return ds.aggregate(MergeParquetAndNpz(), partition_by=path.file_stem(C.name))
 
 
 class LaionMeta(Feature):
     uid: str = Field(default="")
     url: str = Field(default="")
     text: str = Field(default="")
     original_width: int = Field(default=-1)
     original_height: int = Field(default=-1)
     clip_b32_similarity_score: float = Field(default=0.0)
     clip_l14_similarity_score: float = Field(default=0.0)
-    face_bboxes: list[list[float]] = Field(default=None)
+    face_bboxes: Optional[list[list[float]]] = Field(default=None)
     sha256: str = Field(default="")
 
     b32_img: list[float] = Field(default=None)
     b32_txt: list[float] = Field(default=None)
     l14_img: list[float] = Field(default=None)
     l14_txt: list[float] = Field(default=None)
     dedup: list[float] = Field(default=None)
 
 
 class MergeParquetAndNpz(FeatureAggregator):
     def __init__(self):
-        super().__init__(FileStream, [FileInfo, LaionMeta])
+        super().__init__(File, [FileInfo, LaionMeta])
 
     def process(self, args):
+        stream_npz, stream_pq = self.get_meta_streams(args)
+
+        with stream_pq.open() as fd_pq, stream_npz.open() as fd_npz:
+            df = pd.read_parquet(fd_pq)
+            npz_file = np.load(fd_npz)
+
+            yield from self.parse_metafiles(npz_file, df, stream_pq)
+
+    @staticmethod
+    def get_meta_streams(args):
         if len(args) != 2:
             filenames = " ".join([f.get_full_path() for f in args])
-            raise ValueError(f"npz-parquet pair mismatch: {filenames}")
-
+            raise WDSMetaError(f"npz-parquet pair mismatch: {filenames}")
         stream_pq = args[0]
         stream_npz = args[1]
         if args[0].get_file_ext() != "parquet":
             stream_pq, stream_npz = stream_npz, stream_pq
+        return stream_npz, stream_pq
 
-        with stream_pq.open() as fd:
-            pq = pd.read_parquet(fd)
-
-        with stream_npz.open() as fd:
-            npz_file = np.load(fd)
-            b32_img = npz_file["b32_img"]
-            b32_txt = npz_file["b32_txt"]
-            l14_img = npz_file["l14_img"]
-            l14_txt = npz_file["l14_txt"]
-            dedup = npz_file["dedup"]
-
-            for idx, (_, row) in enumerate(pq.iterrows()):
-                fstream = FileInfo(
-                    name=str(idx),
-                    source=stream_pq.source,
-                    parent=f"{stream_pq.parent}/{stream_pq.name}",
-                    version=stream_pq.version,
-                    etag=f"{stream_pq.etag}_{stream_pq.etag}",
-                    vtype="parquet",
-                )
-
-                pq_dict = row.to_dict()
-                npz_dict = {
-                    "b32_img": b32_img[idx],
-                    "b32_txt": b32_txt[idx],
-                    "l14_img": l14_img[idx],
-                    "l14_txt": l14_txt[idx],
-                    "dedup": dedup[idx],
-                }
+    @staticmethod
+    def parse_metafiles(npz_file, df, stream_pq):
+        b32_img = npz_file["b32_img"]
+        b32_txt = npz_file["b32_txt"]
+        l14_img = npz_file["l14_img"]
+        l14_txt = npz_file["l14_txt"]
+        dedup = npz_file["dedup"]
+        for idx, (_, row) in enumerate(df.iterrows()):
+            if idx > 1000:
+                break
+
+            fstream = FileInfo(
+                name=str(idx),
+                source=stream_pq.source,
+                parent=f"{stream_pq.get_full_name()}",
+                version=stream_pq.version,
+                etag=f"{stream_pq.etag}_{stream_pq.etag}",
+                vtype="parquet",
+            )
+
+            pq_dict = row.to_dict()
+            npz_dict = {
+                "b32_img": b32_img[idx],
+                "b32_txt": b32_txt[idx],
+                "l14_img": l14_img[idx],
+                "l14_txt": l14_txt[idx],
+                "dedup": dedup[idx],
+            }
 
-                yield fstream, LaionMeta(**(pq_dict | npz_dict))
+            yield fstream, LaionMeta(**(pq_dict | npz_dict))
```

### Comparing `dvcx-0.71.0/src/dvcx/listing.py` & `dvcx-0.72.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/node.py` & `dvcx-0.72.0/src/dvcx/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,17 +74,14 @@
     def is_container(self) -> bool:
         return self.dir_type in DirTypeGroup.SUBOBJ_DIR
 
     @property
     def is_downloadable(self) -> bool:
         return bool(not self.is_dir and self.name)
 
-    def sql_schema(self):
-        return ",".join(["?"] * len(self))
-
     def append_to_file(self, fd, path: str):
         fd.write(f"- name: {path}\n")
         fd.write(f"  etag: {self.etag}\n")
         version = self.version
         if version:
             fd.write(f"  version: {self.version}\n")
         fd.write(f"  last_modified: '{time_to_str(self.last_modified)}'\n")
```

### Comparing `dvcx-0.71.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.72.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.72.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/progress.py` & `dvcx-0.72.0/src/dvcx/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manages progress bars."""
+
 import logging
 import os
 import re
 import sys
 from threading import RLock
 from typing import Any, ClassVar
```

### Comparing `dvcx-0.71.0/src/dvcx/query/batch.py` & `dvcx-0.72.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/query/builtins.py` & `dvcx-0.72.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/query/dataset.py` & `dvcx-0.72.0/src/dvcx/query/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 import string
 import subprocess
 import sys
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Iterator, Sequence
 from copy import copy
+from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Optional,
     Protocol,
     TypeVar,
@@ -71,17 +72,38 @@
 # dependency can be either dataset_name + dataset_version tuple or just storage uri
 # depending what type of dependency we are adding
 DatasetDependencyType = Union[tuple[str, int], StorageURI]
 
 logger = logging.getLogger("dvcx")
 
 
+def detach(method: Callable):
+    """
+    Decorator that needs to be put on a method that modifies existing DatasetQuery
+    which was 100% representing one particular dataset and had name and version of
+    that dataset set, and which returns new instance of it.
+    This kind of DatasetQuery, which represent one whole dataset, we return from
+    .save() method.
+    Example of modifying method is .filter() as that one filters out part
+    of a dataset which means DatasetQuery no longer 100% represents it (in this case
+    it can represents only a part of it)
+    """
+
+    @wraps(method)
+    def _inner(self, *args, **kwargs) -> "DatasetQuery":
+        cloned = method(self, *args, **kwargs)
+        cloned.name = None
+        cloned.version = None
+        return cloned
+
+    return _inner
+
+
 class QueryGeneratorFunc(Protocol):
-    def __call__(self, *columns: ColumnElement) -> "SelectBase":
-        ...
+    def __call__(self, *columns: ColumnElement) -> "SelectBase": ...
 
 
 @frozen
 class QueryGenerator:
     func: QueryGeneratorFunc
     columns: tuple[ColumnElement, ...]
 
@@ -114,16 +136,15 @@
     )
 
 
 class StartingStep(ABC):
     """An initial query processing step, referencing a data source."""
 
     @abstractmethod
-    def apply(self) -> "StepResult":
-        ...
+    def apply(self) -> "StepResult": ...
 
 
 @frozen
 class Step(ABC):
     """A query processing step (filtering, mutation, etc.)"""
 
     @abstractmethod
@@ -131,27 +152,28 @@
         """Apply the processing step."""
 
 
 @frozen
 class QueryStep(StartingStep):
     catalog: "Catalog"
     dataset_name: str
-    dataset_version: Optional[int] = None
+    dataset_version: int
 
     def apply(self):
         """Return the query for the table the query refers to."""
 
         def q(*columns):
             return sqlalchemy.select(*columns)
 
-        ds = self.catalog.get_dataset(self.dataset_name)
-        version = self.dataset_version or ds.latest_version
-        table = self.catalog.warehouse.dataset_rows(ds, version)
+        dataset = self.catalog.get_dataset(self.dataset_name)
+        table = self.catalog.warehouse.dataset_rows(dataset, self.dataset_version)
 
-        return step_result(q, table.c, dependencies=[(ds.name, version)])
+        return step_result(
+            q, table.c, dependencies=[(self.dataset_name, self.dataset_version)]
+        )
 
 
 @frozen
 class IndexingStep(StartingStep):
     path: str
     catalog: "Catalog"
     kwargs: dict[str, Any]
@@ -336,15 +358,15 @@
 ) -> None:
     rows: list["UDFResult"] = []
     for udf_output in udf_results:
         if not udf_output:
             continue
         for row in udf_output:
             rows.append(adjust_outputs(warehouse, row, udf))
-            if len(rows) > batch_size:
+            if len(rows) >= batch_size:
                 for row_chunk in chunk(rows, batch_size):
                     warehouse.insert_rows(udf_table, row_chunk)
                 rows.clear()
 
     if rows:
         for row_chunk in chunk(rows, batch_size):
             warehouse.insert_rows(udf_table, row_chunk)
@@ -421,17 +443,19 @@
                     cache=self.cache,
                 )
             elif processes:
                 # Parallel processing (faster for more CPU-heavy UDFs)
                 udf_info = {
                     "udf": udf,
                     "catalog_init": self.catalog.get_init_params(),
-                    "id_generator_params": self.catalog.id_generator.clone_params(),
-                    "metastore_params": self.catalog.metastore.clone_params(),
-                    "warehouse_params": self.catalog.warehouse.clone_params(),
+                    "id_generator_clone_params": (
+                        self.catalog.id_generator.clone_params()
+                    ),
+                    "metastore_clone_params": self.catalog.metastore.clone_params(),
+                    "warehouse_clone_params": self.catalog.warehouse.clone_params(),
                     "table": udf_table,
                     "query": query,
                     "batching": batching,
                     "processes": processes,
                     "is_generator": self.is_generator,
                     "cache": self.cache,
                 }
@@ -764,16 +788,16 @@
 class SQLCount(SQLClause):
     def apply_sql_clause(self, query):
         return sqlalchemy.select(f.count(1)).select_from(query.subquery())
 
 
 @frozen
 class SQLUnion(Step):
-    query1: "SQLQuery"
-    query2: "SQLQuery"
+    query1: "DatasetQuery"
+    query2: "DatasetQuery"
 
     def apply(self, query_generator):
         q1 = self.query1.apply_steps().select().subquery()
         q2 = self.query2.apply_steps().select().subquery()
         columns1, columns2 = fill_columns(q1.columns, q2.columns)
 
         def q(*columns):
@@ -794,16 +818,16 @@
             columns1,
             dependencies=self.query1.dependencies | self.query2.dependencies,
         )
 
 
 @frozen
 class SQLJoin(Step):
-    query1: "SQLQuery"
-    query2: "SQLQuery"
+    query1: "DatasetQuery"
+    query2: "DatasetQuery"
     predicates: Union[JoinPredicateType, tuple[JoinPredicateType, ...]]
     inner: bool
     rname: str
 
     def validate_expression(self, exp: ColumnElement, q1, q2):
         """
         Checking if columns used in expression actually exist in left / right
@@ -932,33 +956,47 @@
     _row_iter: Iterable[Any]
     columns: list[str]
 
     def __iter__(self):
         yield from self._row_iter
 
 
-SQLQueryT = TypeVar("SQLQueryT", bound="SQLQuery")
-
-
-class SQLQuery:
+class DatasetQuery:
     def __init__(
         self,
-        starting_step: StartingStep,
-        steps: Optional[Iterable["Step"]] = None,
+        path: str = "",
+        name: str = "",
+        version: Optional[int] = None,
         catalog: Optional["Catalog"] = None,
         client_config=None,
+        recursive: Optional[bool] = True,
     ):
-        self.steps: list["Step"] = list(steps) if steps is not None else []
-        self.starting_step: StartingStep = starting_step
+        self.steps: list["Step"] = []
         self.catalog = catalog or get_catalog(client_config=client_config)
         self._chunk_index: Optional[int] = None
         self._chunk_total: Optional[int] = None
         self.temp_table_names: list[str] = []
         self.dependencies: set[DatasetDependencyType] = set()
         self.table = self.get_table()
+        self.starting_step: StartingStep
+        self.name: Optional[str] = None
+        self.version: Optional[int] = None
+
+        if path:
+            self.starting_step = IndexingStep(
+                path, self.catalog, {"client_config": client_config}, recursive
+            )
+        elif name:
+            version = version or self.catalog.get_dataset(name).latest_version
+            self.starting_step = QueryStep(self.catalog, name, version)
+            # attaching to specific dataset
+            self.name = name
+            self.version = version
+        else:
+            raise ValueError("must provide path or name")
 
     def __iter__(self):
         return iter(self.results())
 
     def __or__(self, other):
         return self.union(other)
 
@@ -966,16 +1004,38 @@
     def get_table() -> "Table":
         table_name = "".join(
             random.choice(string.ascii_letters)  # noqa: S311
             for _ in range(16)
         )
         return sqlalchemy.table(table_name)
 
-    def c(self, name: str) -> C:
-        col = sqlalchemy.column(name)
+    @staticmethod
+    def delete(
+        name: str, version: Optional[int] = None, catalog: Optional["Catalog"] = None
+    ) -> None:
+        catalog = catalog or get_catalog()
+        version = version or catalog.get_dataset(name).latest_version
+        catalog.remove_dataset(name, version)
+
+    @property
+    def attached(self) -> bool:
+        """
+        DatasetQuery is considered "attached" to underlying dataset if it represents
+        it completely. If this is the case, name and version of underlying dataset
+        will be defined.
+        DatasetQuery instance can become attached in two scenarios:
+            1. ds = DatasetQuery(name="dogs", version=1) -> ds is attached to dogs
+            2. ds = ds.save("dogs", version=1) -> ds is attached to dogs dataset
+        It can move to detached state if filter or similar methods are called on it,
+        as then it no longer 100% represents underlying datasets.
+        """
+        return self.name is not None and self.version is not None
+
+    def c(self, name: Union[C, str]) -> C:
+        col = sqlalchemy.column(name) if isinstance(name, str) else name
         col.table = self.table
         return col
 
     def apply_steps(self) -> QueryGenerator:
         """
         Apply the steps in the query and return the resulting
         sqlalchemy.SelectBase.
@@ -1060,15 +1120,17 @@
         try:
             query = self.apply_steps().select()
 
             def row_iter() -> Iterable[DatasetRow]:
                 # warehouse isn't threadsafe, we need to clone() it
                 # in the thread that uses the results
                 db = self.catalog.warehouse.clone()
-                yield from db.dataset_select_paginated(query, limit=query._limit)
+                yield from db.dataset_select_paginated(
+                    query, limit=query._limit, order_by=query._order_by_clauses
+                )
 
             async def get_params(row: DatasetRow) -> tuple:
                 return tuple(
                     [
                         await p.get_value_async(self.catalog, row, mapper, **kwargs)
                         for p in actual_params
                     ]
@@ -1077,15 +1139,15 @@
             MapperCls = OrderedMapper if query._order_by_clauses else AsyncMapper  # noqa: N806
             mapper = MapperCls(get_params, row_iter(), workers=workers)
             for params in mapper.iterate():
                 yield params
         finally:
             self.cleanup()
 
-    def to_records(self):
+    def to_records(self) -> list[dict]:
         with self.as_iterable() as result:
             cols = result.columns
             return [dict(zip(cols, row)) for row in result]
 
     def to_pandas(self):
         try:
             import pandas as pd
@@ -1095,33 +1157,34 @@
                 "To install run:\n\n"
                 "  pip install 'dvcx[pandas]'\n"
             ) from exc
 
         records = self.to_records()
         return pd.DataFrame.from_records(records)
 
-    def shuffle(self):
+    def shuffle(self) -> "DatasetQuery":
         # ToDo: implement shaffle based on seed and/or generating random column
         return self.order_by(C.random)
 
-    def show(self, limit=20):
+    def show(self, limit=20) -> None:
         df = self.limit(limit).to_pandas()
         no_footer = re.sub(r"\n\[\d+ rows x \d+ columns\]$", "", str(df))
         print(no_footer.rstrip(" \n"))
         if len(df) == limit:
             print(f"[limited by {limit} objects]")
 
-    def clone(self: SQLQueryT, new_table=True) -> SQLQueryT:
+    def clone(self: "DatasetQuery", new_table=True) -> "DatasetQuery":
         obj = copy(self)
         obj.steps = obj.steps.copy()
         if new_table:
             obj.table = self.get_table()
         return obj
 
-    def select(self, *args, **kwargs):
+    @detach
+    def select(self, *args, **kwargs) -> "DatasetQuery":
         """
         Select the given columns or expressions using a subquery.
 
         If used with no arguments, this simply creates a subquery and
         select all columns from it.
 
         Note that the `save` function expects default dataset columns to
@@ -1133,15 +1196,16 @@
             >>> ds.select(C.name, size10x=C.size * 10).order_by(C.size10x).results()
         """
         named_args = [v.label(k) for k, v in kwargs.items()]
         query = self.clone()
         query.steps.append(SQLSelect((*args, *named_args)))
         return query
 
-    def select_except(self, *args):
+    @detach
+    def select_except(self, *args) -> "DatasetQuery":
         """
         Exclude certain columns from this query using a subquery.
 
         Note that the `save` function expects default dataset columns to
         be present. This function is meant to be followed by a call to
         `results` if used to exclude any default columns.
 
@@ -1152,20 +1216,21 @@
             ...     .select_except(C.size10x)
             ...     .results()
             ... )
         """
 
         if not args:
             raise TypeError("select_except expected at least 1 argument, got 0")
-        args = [c if isinstance(c, str) else c.name for c in args]
+        query_args = [c if isinstance(c, str) else c.name for c in args]
         query = self.clone()
-        query.steps.append(SQLSelectExcept(args))
+        query.steps.append(SQLSelectExcept(query_args))  # type: ignore [arg-type]
         return query
 
-    def select_default(self):
+    @detach
+    def select_default(self) -> "DatasetQuery":
         """
         Select only the default dataset columns using a subquery.
 
         This assumes that none of the default dataset columns have
         already been excluded from this query. This is useful if you've
         added columns with `mutate` or `select` calls for filtering but
         only want the default columns in the final output.
@@ -1178,49 +1243,53 @@
             ...     .results()
             ... )
         """
         query = self.clone()
         query.steps.append(SQLSelect((*DATASET_CORE_COLUMN_NAMES,)))
         return query
 
-    def mutate(self, *args, **kwargs):
+    @detach
+    def mutate(self, *args, **kwargs) -> "DatasetQuery":
         """
         Add new columns to this query.
 
         This function selects all existing columns from this query and
         adds in the new columns specified.
 
         Example:
             >>> ds.mutate(size10x=C.size * 10).order_by(C.size10x).results()
         """
-        args = [v.label(k) for k, v in dict(args, **kwargs).items()]
+        query_args = [v.label(k) for k, v in dict(args, **kwargs).items()]
         query = self.clone()
-        query.steps.append(SQLMutate((*args,)))
+        query.steps.append(SQLMutate((*query_args,)))
         return query
 
-    def filter(self, *args):
+    @detach
+    def filter(self, *args) -> "DatasetQuery":
         query = self.clone(new_table=False)
         steps = query.steps
         if steps and isinstance(steps[-1], SQLFilter):
             steps[-1] = steps[-1] & args
         else:
             steps.append(SQLFilter(args))
         return query
 
-    def order_by(self, *args):
+    @detach
+    def order_by(self, *args) -> "DatasetQuery":
         query = self.clone(new_table=False)
         query.steps.append(SQLOrderBy(args))
         return query
 
-    def limit(self, n: int):
+    @detach
+    def limit(self, n: int) -> "DatasetQuery":
         query = self.clone(new_table=False)
         query.steps.append(SQLLimit(n))
         return query
 
-    def count(self):
+    def count(self) -> int:
         query = self.clone()
         query.steps.append(SQLCount())
         return query.results()[0][0]
 
     def sum(self, col: ColumnElement):
         query = self.clone()
         query.steps.append(SQLSelect((f.sum(col),)))
@@ -1237,33 +1306,36 @@
         return query.results()[0][0]
 
     def max(self, col: ColumnElement):
         query = self.clone()
         query.steps.append(SQLSelect((f.max(col),)))
         return query.results()[0][0]
 
-    def group_by(self, *cols: ColumnElement):
+    @detach
+    def group_by(self, *cols: ColumnElement) -> "DatasetQuery":
         query = self.clone()
         query.steps.append(GroupBy(cols))
         return query
 
-    def union(self, dataset_query: "DatasetQuery"):
+    @detach
+    def union(self, dataset_query: "DatasetQuery") -> "DatasetQuery":
         left = self.clone()
         right = dataset_query.clone()
         new_query = self.clone()
         new_query.steps = [SQLUnion(left, right)]
         return new_query
 
+    @detach
     def join(
         self,
         dataset_query: "DatasetQuery",
         predicates: Union[JoinPredicateType, Sequence[JoinPredicateType]],
         inner=False,
         rname="{name}_right",
-    ):
+    ) -> "DatasetQuery":
         left = self.clone(new_table=False)
         if self.table.name == dataset_query.table.name:
             # for use case where we join with itself, e.g dogs.join(dogs, "name")
             right = dataset_query.clone(new_table=True)
         else:
             right = dataset_query.clone(new_table=False)
 
@@ -1272,56 +1344,30 @@
             predicates
             if isinstance(predicates, (str, ColumnClause, ColumnElement))
             else tuple(predicates)
         )
         new_query.steps = [SQLJoin(left, right, predicates, inner, rname)]
         return new_query
 
-    def chunk(self, index: int, total: int):
+    @detach
+    def chunk(self, index: int, total: int) -> "DatasetQuery":
         """Split a query into smaller chunks for e.g. parallelization.
         Example:
             >>> query = DatasetQuery(...)
             >>> chunk_1 = query._chunk(0, 2)
             >>> chunk_2 = query._chunk(1, 2)
         Note:
             Bear in mind that `index` is 0-indexed but `total` isn't.
             Use 0/3, 1/3 and 2/3, not 1/3, 2/3 and 3/3.
         """
         query = self.clone()
         query._chunk_index, query._chunk_total = index, total
         return query
 
-
-class DatasetQuery(SQLQuery):
-    def __init__(
-        self,
-        path: str = "",
-        name: str = "",
-        version: Optional[int] = None,
-        catalog=None,
-        client_config=None,
-        recursive: Optional[bool] = True,
-    ):
-        if catalog is None:
-            catalog = get_catalog(client_config=client_config)
-
-        starting_step: StartingStep
-        if path:
-            starting_step = IndexingStep(
-                path, catalog, {"client_config": client_config}, recursive
-            )
-        elif name:
-            starting_step = QueryStep(catalog, name, version)
-        else:
-            raise ValueError("must provide path or name")
-
-        super().__init__(
-            starting_step=starting_step, catalog=catalog, client_config=client_config
-        )
-
+    @detach
     def add_signals(
         self,
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
@@ -1351,33 +1397,36 @@
                 workers=workers,
                 min_task_size=min_task_size,
                 cache=cache,
             )
         )
         return query
 
-    def subtract(self, dq: "DatasetQuery"):
+    @detach
+    def subtract(self, dq: "DatasetQuery") -> "DatasetQuery":
         query = self.clone()
         query.steps.append(Subtract(dq, self.catalog))
         return query
 
-    def changed(self, dq: "DatasetQuery"):
+    @detach
+    def changed(self, dq: "DatasetQuery") -> "DatasetQuery":
         query = self.clone()
         query.steps.append(Changed(dq, self.catalog))
         return query
 
+    @detach
     def generate(
         self,
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
         cache: bool = False,
-    ):
+    ) -> "DatasetQuery":
         query = self.clone()
         steps = query.steps
         steps.append(
             RowGenerator(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
@@ -1490,17 +1539,24 @@
     Last statement MUST be instance of DatasetQuery, otherwise script exits with
     error code 10
     """
     if not isinstance(dataset_query, DatasetQuery):
         sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
 
     if isinstance(dataset_query, DatasetQuery):
-        ds_name = dataset_query.catalog.generate_query_dataset_name()
-        dataset_query.catalog.warehouse.return_ds_hook(ds_name)
-        dataset_query.save(ds_name)
+        if dataset_query.attached:
+            dataset_query.catalog.warehouse.return_ds_hook(
+                dataset_query.name,  # type: ignore [arg-type]
+                dataset_query.version,  # type: ignore [arg-type]
+            )
+        else:
+            ds_name = dataset_query.catalog.generate_query_dataset_name()
+            dataset_query.catalog.warehouse.return_ds_hook(ds_name, 1)
+            dataset_query.save(ds_name)
+
     return dataset_query
 
 
 def query_wrapper_print(dataset_query: DatasetQuery) -> DatasetQuery:
     """
     Wrapper function that wraps the last statement of user query script for printing
     results in console.
```

### Comparing `dvcx-0.71.0/src/dvcx/query/dispatch.py` & `dvcx-0.72.0/src/dvcx/query/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     # Load UDF info from stdin
     udf_info = load(stdin.buffer)  # noqa: S301
 
     (
         warehouse_class,
         warehouse_args,
         warehouse_kwargs,
-    ) = udf_info["warehouse_params"]
+    ) = udf_info["warehouse_clone_params"]
     warehouse = warehouse_class(*warehouse_args, **warehouse_kwargs)
 
     # Parallel processing (faster for more CPU-heavy UDFs)
     dispatch = UDFDispatcher(
         udf_info["udf"],
         udf_info["catalog_init"],
-        udf_info["id_generator_params"],
-        udf_info["metastore_params"],
-        udf_info["warehouse_params"],
+        udf_info["id_generator_clone_params"],
+        udf_info["metastore_clone_params"],
+        udf_info["warehouse_clone_params"],
         is_generator=udf_info.get("is_generator", False),
         cache=udf_info["cache"],
     )
 
     query = udf_info["query"]
     batching = udf_info["batching"]
     table = udf_info["table"]
```

### Comparing `dvcx-0.71.0/src/dvcx/query/schema.py` & `dvcx-0.72.0/src/dvcx/query/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 
     def glob(self, glob_str):
         return self.op("GLOB")(glob_str)
 
 
 class UDFParameter(ABC):
     @abstractmethod
-    def get_value(self, catalog: "Catalog", row: "Row", **kwargs) -> Any:
-        ...
+    def get_value(self, catalog: "Catalog", row: "Row", **kwargs) -> Any: ...
 
     async def get_value_async(
         self, catalog: "Catalog", row: "Row", mapper, **kwargs
     ) -> Any:
         return self.get_value(catalog, row, **kwargs)
 
 
@@ -157,15 +156,15 @@
     if isinstance(param, str):
         return ColumnParameter(param)
     elif isinstance(param, Column):
         return ColumnParameter(param.name)
     elif isinstance(param, UDFParameter):
         return param
     else:
-        raise TypeError("Invalid UDF parameter: {param}")
+        raise TypeError(f"Invalid UDF parameter: {param}")
 
 
 class DatasetRow:
     schema = {
         "source": String,
         "parent": String,
         "name": String,
```

### Comparing `dvcx-0.71.0/src/dvcx/query/udf.py` & `dvcx-0.72.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/remote/studio.py` & `dvcx-0.72.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/default/base.py` & `dvcx-0.72.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/functions/array.py` & `dvcx-0.72.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/functions/path.py` & `dvcx-0.72.0/src/dvcx/sql/functions/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module provides generic SQL functions for path logic.
 
 These need to be implemented using dialect-specific compilation rules.
 See https://docs.sqlalchemy.org/en/14/core/compiler.html
 """
+
 from sqlalchemy.sql.functions import GenericFunction
 
 from dvcx.sql.types import String
 from dvcx.sql.utils import compiler_not_implemented
 
 
 class parent(GenericFunction):  # noqa: N801
```

### Comparing `dvcx-0.71.0/src/dvcx/sql/selectable.py` & `dvcx-0.72.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.72.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.72.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/types.py` & `dvcx-0.72.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/sql/utils.py` & `dvcx-0.72.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/src/dvcx/storage.py` & `dvcx-0.72.0/src/dvcx/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,31 +31,27 @@
     PARTIAL = 5
     STALE = 6
 
 
 class AbstractStorage(ABC):
     @property
     @abstractmethod
-    def uri(self) -> StorageURI:
-        ...
+    def uri(self) -> StorageURI: ...
 
     @property
     @abstractmethod
-    def timestamp(self) -> Optional[Union[datetime, str]]:
-        ...
+    def timestamp(self) -> Optional[Union[datetime, str]]: ...
 
     @property
     @abstractmethod
-    def expires(self) -> Optional[Union[datetime, str]]:
-        ...
+    def expires(self) -> Optional[Union[datetime, str]]: ...
 
     @property
     @abstractmethod
-    def status(self) -> int:
-        ...
+    def status(self) -> int: ...
 
     @property
     def type(self):
         return self._parsed_uri.scheme
 
     @property
     def name(self):
```

### Comparing `dvcx-0.71.0/src/dvcx/utils.py` & `dvcx-0.72.0/src/dvcx/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 import importlib.util
 import os
 import os.path as osp
 import random
 import stat
 import sys
 import time
-from collections.abc import Iterable, Mapping, Sequence
+from collections.abc import Iterable, Sequence
 from datetime import datetime, timezone
 from itertools import islice
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Optional,
-    TypeVar,
-    Union,
-)
+from typing import Any, Optional, TypeVar, Union
 
 from dateutil import tz
 from dateutil.parser import isoparse
-from tomlkit import parse
-
-if TYPE_CHECKING:
-    from tomlkit import TOMLDocument
 
 GLOB_CHARS = ["?", "*", "[", "]"]
 NUL = b"\0"
 TIME_ZERO = datetime.fromtimestamp(0, tz=timezone.utc)
 
 T = TypeVar("T", bound="DVCXDir")
 
@@ -80,68 +70,14 @@
             if create:
                 instance.init()
             else:
                 NotADirectoryError(root)
         return instance
 
 
-def read_config(dvcx_root: str) -> Optional["TOMLDocument"]:
-    project_path = osp.join(dvcx_root, "config")
-    if osp.isfile(project_path):
-        with open(project_path, encoding="utf-8") as f:
-            text = f.read()
-        return parse(text)
-    return None
-
-
-def get_remote_config(
-    config: Optional["TOMLDocument"], remote: str = ""
-) -> Mapping[str, str]:
-    if config is None:
-        return {"type": "local"}
-    if not remote:
-        try:
-            remote = config["core"]["default-remote"]  # type: ignore[index,assignment]
-        except KeyError:
-            return {"type": "local"}
-    try:
-        remote_conf: Mapping[str, str] = config["remote"][remote]  # type: ignore[assignment,index]
-    except KeyError:
-        raise Exception(
-            f"missing config section for default remote: remote.{remote}"
-        ) from None
-    except Exception as exc:
-        raise Exception("invalid config") from exc
-
-    if not isinstance(remote_conf, Mapping):
-        raise Exception(f"config section remote.{remote} must be a mapping")
-
-    remote_type = remote_conf.get("type")
-    if remote_type not in ("local", "http"):
-        raise Exception(
-            f'config section remote.{remote} must have "type" with one of: '
-            '"local", "http"'
-        )
-
-    if remote_type == "http":
-        for key in ["url", "username", "token"]:
-            try:
-                remote_conf[key]
-            except KeyError:
-                raise Exception(
-                    f"config section remote.{remote} of type {remote_type} "
-                    f"must contain key {key}"
-                ) from None
-    elif remote_type != "local":
-        raise Exception(
-            f"config section remote.{remote} has invalid remote type {remote_type}"
-        )
-    return remote_conf
-
-
 def human_time_to_int(time: str) -> Optional[int]:
     if not time:
         return None
 
     suffix = time[-1]
     try:
         num = int(time if suffix.isdigit() else time[:-1])
@@ -325,15 +261,15 @@
             while True:
                 try:
                     return f(*args, **kwargs)
                 except Exception:
                     if num_tried == retries:
                         raise
                     sleep = (
-                        backoff_sec * 2**num_tried + random.uniform(0, 1)  # noqa: S311
+                        backoff_sec * 2** num_tried + random.uniform(0, 1)  # noqa: S311
                     )
                     time.sleep(sleep)
                     num_tried += 1
 
         return wrapper
 
     return retry
```

### Comparing `dvcx-0.71.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.72.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.71.0
+Version: 0.72.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,14 +31,15 @@
 Requires-Dist: dill==0.3.8
 Requires-Dist: ujson==5.9.0
 Requires-Dist: types-ujson==5.9.0.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
 Requires-Dist: torch>=2.1.0; extra == "cv"
+Requires-Dist: torchvision; extra == "cv"
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: transformers>=4.36.0; extra == "cv"
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4.0; extra == "pandas"
 Provides-Extra: remote
 Requires-Dist: dvcx[pandas]; extra == "remote"
 Requires-Dist: lz4; extra == "remote"
@@ -51,17 +52,18 @@
 Requires-Dist: scipy; extra == "vector"
 Provides-Extra: tests
 Requires-Dist: dvcx[cv,pandas,remote,vector]; extra == "tests"
 Requires-Dist: pytest<9,>=8; extra == "tests"
 Requires-Dist: pytest-sugar>=0.9.6; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-mock>=3.12.0; extra == "tests"
-Requires-Dist: pytest-servers[all]>=0.4.0; extra == "tests"
+Requires-Dist: pytest-servers[all]>=0.5.1; extra == "tests"
 Requires-Dist: pytest-benchmark[histogram]; extra == "tests"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "tests"
+Requires-Dist: pytest-xdist>=3.3.1; extra == "tests"
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
```

### Comparing `dvcx-0.71.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.72.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 src/dvcx/__init__.py
 src/dvcx/__main__.py
 src/dvcx/_version.py
 src/dvcx/asyn.py
 src/dvcx/cache.py
 src/dvcx/cli.py
 src/dvcx/cli_utils.py
+src/dvcx/config.py
 src/dvcx/dataset.py
 src/dvcx/error.py
 src/dvcx/listing.py
 src/dvcx/node.py
 src/dvcx/nodes_fetcher.py
 src/dvcx/nodes_thread_pool.py
 src/dvcx/progress.py
@@ -90,30 +91,34 @@
 src/dvcx/client/local.py
 src/dvcx/client/s3.py
 src/dvcx/data_storage/__init__.py
 src/dvcx/data_storage/db_engine.py
 src/dvcx/data_storage/id_generator.py
 src/dvcx/data_storage/metastore.py
 src/dvcx/data_storage/schema.py
+src/dvcx/data_storage/serializer.py
 src/dvcx/data_storage/sqlite.py
 src/dvcx/data_storage/warehouse.py
 src/dvcx/lib/__init__.py
 src/dvcx/lib/dataset.py
 src/dvcx/lib/feature.py
 src/dvcx/lib/feature_udf.py
+src/dvcx/lib/file.py
 src/dvcx/lib/gpt4_vision.py
 src/dvcx/lib/hf_image_to_text.py
 src/dvcx/lib/hf_pipeline.py
 src/dvcx/lib/image_transform.py
 src/dvcx/lib/iptc_exif_xmp.py
-src/dvcx/lib/stream.py
+src/dvcx/lib/param.py
+src/dvcx/lib/pytorch.py
 src/dvcx/lib/udf.py
 src/dvcx/lib/unstructured.py
 src/dvcx/lib/utils.py
 src/dvcx/lib/webdataset.py
+src/dvcx/lib/webdataset_laion.py
 src/dvcx/lib/webdataset_meta.py
 src/dvcx/query/__init__.py
 src/dvcx/query/batch.py
 src/dvcx/query/builtins.py
 src/dvcx/query/dataset.py
 src/dvcx/query/dispatch.py
 src/dvcx/query/schema.py
@@ -147,34 +152,41 @@
 tests/func/__init__.py
 tests/func/test_catalog.py
 tests/func/test_client.py
 tests/func/test_dataset_query.py
 tests/func/test_datasets.py
 tests/func/test_ls.py
 tests/func/test_pull.py
+tests/func/test_pytorch.py
 tests/func/test_query.py
 tests/unit/__init__.py
 tests/unit/test_asyn.py
 tests/unit/test_cache.py
 tests/unit/test_catalog.py
 tests/unit/test_catalog_formats.py
+tests/unit/test_catalog_loader.py
 tests/unit/test_cli_parsing.py
 tests/unit/test_client.py
 tests/unit/test_client_s3.py
 tests/unit/test_data_storage.py
 tests/unit/test_database_engine.py
 tests/unit/test_dataset.py
 tests/unit/test_fileslice.py
 tests/unit/test_id_generator.py
 tests/unit/test_listing.py
+tests/unit/test_metastore.py
+tests/unit/test_serializer.py
 tests/unit/test_storage.py
 tests/unit/test_udf.py
 tests/unit/test_utils.py
+tests/unit/test_warehouse.py
 tests/unit/lib/test_feature.py
 tests/unit/lib/test_feature_udf.py
-tests/unit/lib/test_stream.py
+tests/unit/lib/test_file.py
+tests/unit/lib/test_webdataset.py
+tests/unit/lib/test_webdataset_meta.py
 tests/unit/sql/test_array.py
 tests/unit/sql/test_conditional.py
 tests/unit/sql/test_path.py
 tests/unit/sql/test_selectable.py
 tests/unit/sql/test_string.py
 tests/unit/sql/sqlite/test_utils.py
```

### Comparing `dvcx-0.71.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.72.0/src/dvcx.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ujson==5.9.0
 types-ujson==5.9.0.0
 pydantic<3,>=2
 
 [cv]
 Pillow<11,>=10.0.0
 torch>=2.1.0
+torchvision
 numpy
 transformers>=4.36.0
 
 [dev]
 dvcx[tests]
 mypy==1.9.0
 types-python-dateutil
@@ -42,17 +43,18 @@
 
 [tests]
 dvcx[cv,pandas,remote,vector]
 pytest<9,>=8
 pytest-sugar>=0.9.6
 pytest-cov>=4.1.0
 pytest-mock>=3.12.0
-pytest-servers[all]>=0.4.0
+pytest-servers[all]>=0.5.1
 pytest-benchmark[histogram]
 pytest-asyncio>=0.23.2
+pytest-xdist>=3.3.1
 virtualenv
 dulwich
 hypothesis
 numpy
 aiotools>=1.7.0
 requests-mock
```

### Comparing `dvcx-0.71.0/tests/benchmarks/conftest.py` & `dvcx-0.72.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/conftest.py` & `dvcx-0.72.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     monkeypatch_session: MonkeyPatch,
     tmp_path_factory: TempPathFactory,
 ) -> None:
     """
     Make sure we have a clean environment and won't write to userspace.
     """
     working_dir = str(tmp_path_factory.mktemp("default_working_dir"))
-    os.chdir(working_dir)
+    monkeypatch_session.chdir(working_dir)
     monkeypatch_session.delenv(DVCXDir.ENV_VAR, raising=False)
 
     def default_root(cls: type[DVCXDir]) -> str:
         return os.path.join(working_dir, cls.DEFAULT)
 
     monkeypatch_session.setattr(
         "dvcx.utils.DVCXDir.default_root",
```

### Comparing `dvcx-0.71.0/tests/data.py` & `dvcx-0.72.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/func/test_catalog.py` & `dvcx-0.72.0/tests/func/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,22 @@
 @pytest.fixture
 def mock_subprocess_run(cloud_test_catalog, listed_bucket):
     from subprocess import CompletedProcess
 
     with patch("subprocess.run") as mock_run:
         # create dataset which would be created in subprocess
         ds_name = cloud_test_catalog.catalog.generate_query_dataset_name()
+        ds_version = 1
         cloud_test_catalog.catalog.create_dataset_from_sources(
             ds_name,
             [f"{cloud_test_catalog.src_uri}/dogs/*"],
             recursive=True,
         )
         res = CompletedProcess([], 0)
-        std = f"__ds__{ds_name}__ds__\nuser log 1\nuser log 2"
+        std = f"__ds__{ds_name}__ds__{ds_version}__ds__\nuser log 1\nuser log 2"
         res.stdout = str.encode(std)
         mock_run.return_value = res
 
         yield mock_run
 
 
 @pytest.fixture
@@ -937,17 +938,17 @@
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
     DatasetQuery({src_uri!r})
     """
     query_script = dedent(query_script)
 
-    dataset, query_output = catalog.query(query_script, save=True)
+    dataset, version, query_output = catalog.query(query_script, save=True)
     assert dataset
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, 1)} == {
+    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
     assert dataset.query_script == query_script
     assert dataset.sources == ""
```

### Comparing `dvcx-0.71.0/tests/func/test_client.py` & `dvcx-0.72.0/tests/func/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dvcx.asyn import get_loop
 from dvcx.client import Client
 
 from ..data import ENTRIES
 
 
 @pytest.fixture
-def client(cloud_server):
+def client(cloud_server, cloud_server_credentials):
     uri = cloud_server.src_uri
     return Client.get_implementation(uri).from_source(
         uri, cache=None, **cloud_server.client_config
     )
 
 
 def normalize_entries(entries):
```

### Comparing `dvcx-0.71.0/tests/func/test_dataset_query.py` & `dvcx-0.72.0/tests/func/test_dataset_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import io
 import json
 import os
 import pickle
+import random
 import uuid
 from datetime import datetime, timedelta, timezone
 from json import dumps
 from random import getrandbits
 from textwrap import dedent
-from unittest.mock import ANY
+from unittest.mock import ANY, patch
 
 import numpy as np
 import pytest
 import sqlalchemy
 from dateutil.parser import isoparse
 from sqlalchemy import tuple_
 
 from dvcx.catalog import indexer_formats
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.warehouse import RANDOM_BITS
 from dvcx.dataset import DatasetDependencyType
 from dvcx.dataset import Status as DatasetStatus
+from dvcx.error import DatasetInvalidVersionError, DatasetNotFoundError
+from dvcx.lib.param import Label
 from dvcx.node import Node
 from dvcx.query import C, DatasetQuery, DatasetRow, LocalFilename, Object, Stream, udf
 from dvcx.query.builtins import checksum, index_tar
+from dvcx.query.dataset import QueryStep
 from dvcx.sql import functions
 from dvcx.sql.functions.array import cosine_distance, euclidean_distance
 from dvcx.sql.types import (
     JSON,
     Array,
     Binary,
     Boolean,
@@ -68,14 +72,76 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
+def test_delete_dataset(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+    path = f"{cloud_test_catalog.src_uri}/cats"
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=2)
+
+    DatasetQuery.delete("cats", version=1, catalog=catalog)
+    dataset = catalog.get_dataset("cats")
+    assert dataset.versions_values == [2]
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_delete_dataset_latest_version(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+    path = f"{cloud_test_catalog.src_uri}/cats"
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=2)
+
+    DatasetQuery.delete("cats", catalog=catalog)
+    dataset = catalog.get_dataset("cats")
+    assert dataset.versions_values == [1]
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_delete_dataset_only_version(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+    path = f"{cloud_test_catalog.src_uri}/cats"
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
+
+    DatasetQuery.delete("cats", catalog=catalog)
+    with pytest.raises(DatasetNotFoundError):
+        catalog.get_dataset("cats")
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_delete_dataset_missing_version(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+    path = f"{cloud_test_catalog.src_uri}/cats"
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
+    DatasetQuery(path=path, catalog=catalog).save("cats", version=2)
+
+    with pytest.raises(DatasetInvalidVersionError):
+        DatasetQuery.delete("cats", version=5, catalog=catalog)
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
 def test_save_dataset_version_already_exists(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     path = f"{cloud_test_catalog.src_uri}/cats"
     DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
     with pytest.raises(RuntimeError) as exc_info:
         DatasetQuery(path=path, catalog=catalog).save("cats", version=1)
 
@@ -152,29 +218,108 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
-def test_save_returned_dataset(cloud_test_catalog, dogs_cats_dataset):
+def test_instance_returned_after_save(cloud_test_catalog, dogs_cats_dataset):
+    catalog = cloud_test_catalog.catalog
+    ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
+
+    ds2 = ds.save("dogs_cats_2")
+    assert isinstance(ds2, DatasetQuery)
+    assert (
+        {row.name for row in catalog.ls_dataset_rows(dogs_cats_dataset.name, 1)}
+        == {row.name for row in catalog.ls_dataset_rows("dogs_cats_2", 1)}
+        == {"cat1", "cat2", "dog1", "dog2", "dog3", "dog4"}
+    )
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_query_specific_dataset_set_proper_dataset_name_version(
+    cloud_test_catalog, dogs_cats_dataset
+):
+    catalog = cloud_test_catalog.catalog
+    ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
+    assert ds.name == dogs_cats_dataset.name
+    assert ds.version == 1
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_save_set_proper_dataset_name_version(cloud_test_catalog, dogs_cats_dataset):
     catalog = cloud_test_catalog.catalog
     ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
     ds = ds.filter(C.name.glob("dog*"))
     ds2 = ds.save("dogs_small")
 
-    assert isinstance(ds2, DatasetQuery)
+    assert ds2.name == "dogs_small"
+    assert ds2.version == 1
     assert len(ds2.steps) == 0
-    ds2.save("dogs_small_2")
 
-    assert (
-        {row.name for row in catalog.ls_dataset_rows("dogs_small", 1)}
-        == {row.name for row in catalog.ls_dataset_rows("dogs_small_2", 1)}
-        == {"dog1", "dog2", "dog3", "dog4"}
+    # old dataset query remains detached
+    assert ds.name is None
+    assert ds.version is None
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+def test_reset_dataset_name_version_after_filter(cloud_test_catalog, dogs_cats_dataset):
+    catalog = cloud_test_catalog.catalog
+    ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
+    ds2 = ds.save("dogs_small")
+    assert ds2.name == "dogs_small"
+    assert ds2.version == 1
+
+    ds3 = ds2.filter(C.name.glob("dog1"))
+    assert ds3.name is None
+    assert ds3.version is None
+
+    # old ds2 remains attached
+    assert ds2.name == "dogs_small"
+    assert ds2.version == 1
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+@patch("random.randint")
+def test_avoid_recalculation_after_save(randint_mock, cloud_test_catalog):
+    @udf(("name",), {"name_len": Int})
+    def name_len(name):
+        random.randint(1, 5)  #  noqa: S311 using to check how many times we called UDF
+        return (len(name),)
+
+    path = cloud_test_catalog.src_uri
+    catalog = cloud_test_catalog.catalog
+    ds = (
+        DatasetQuery(path=path, catalog=catalog)
+        .filter(C.name == "dog1")
+        .add_signals(name_len)
     )
+    ds2 = ds.save("ds1")
+
+    assert ds2.steps == []
+    assert ds2.dependencies == set()
+    assert isinstance(ds2.starting_step, QueryStep)
+    ds2.save("ds2")
+    assert randint_mock.call_count == 1  # UDF should be called only once
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1072,14 +1217,49 @@
     catalog = cloud_test_catalog.catalog
     q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
     results = list(q.limit(2).extract("name"))
     assert len(results) == 2
 
 
 @pytest.mark.parametrize(
+    "cloud_type, version_aware",
+    [("file", False)],
+    indirect=True,
+)
+def test_extract_order_by(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+    q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
+    results = list(q.order_by("random").extract("name"))
+    pairs = list(q.extract("random", "name"))
+    assert results == [(p[1],) for p in sorted(pairs)]
+
+
+@pytest.mark.parametrize(
+    "cloud_type, version_aware",
+    [("file", False)],
+    indirect=True,
+)
+def test_label_param(cloud_test_catalog, listed_bucket):
+    ctc = cloud_test_catalog
+
+    @udf(params=("name",), output={"label": String})
+    def extract_label(name):
+        return (name[:3],)
+
+    ds = (
+        DatasetQuery(ctc.src_uri, catalog=ctc.catalog)
+        .add_signals(extract_label)
+        .filter(C("label").in_(["cat", "dog"]))
+        .save("cats-dogs")
+    )
+    results = list(ds.order_by("name").extract(Label("label", ["cat", "dog"])))
+    assert results == [(0,)] * 2 + [(1,)] * 4
+
+
+@pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
 def test_union(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     sources = [str(cloud_test_catalog.src_uri)]
```

### Comparing `dvcx-0.71.0/tests/func/test_datasets.py` & `dvcx-0.72.0/tests/func/test_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,17 @@
 from ..utils import dataset_dependency_asdict
 
 
 def add_column(engine, table_name, column, catalog):
     # Simple method that adds new column to a table, with default value if specified
     column_name = column.compile(dialect=engine.dialect)
     column_type = column.type.compile(engine.dialect)
+    query_str = f"ALTER TABLE {table_name} ADD COLUMN {column_name} {column_type}"
     if column.default:
-        query_str = "ALTER TABLE {} ADD COLUMN {} {} DEFAULT {}".format(
-            table_name,
-            column_name,
-            column_type,
-            column.default.arg,
-        )
-    else:
-        query_str = f"ALTER TABLE {table_name} ADD COLUMN {column_name} {column_type}"
+        query_str += f" DEFAULT {column.default.arg}"
     catalog.warehouse.db.execute_str(query_str)
 
 
 @pytest.fixture
 def empty_registered_dataset(listed_bucket, cloud_test_catalog):
     name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
@@ -482,29 +476,43 @@
             target_version=2,
         )
     assert str(exc_info.value) == (
         "Cannot register dataset version in non final status"
     )
 
 
-def test_removing_dataset(cloud_test_catalog, dogs_dataset):
+def test_remove_dataset(cloud_test_catalog, dogs_dataset):
     catalog = cloud_test_catalog.catalog
 
     dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 1)
     assert get_table_row_count(catalog.warehouse.db, dataset_table_name)
 
     catalog.remove_dataset(dogs_dataset.name, force=True)
     with pytest.raises(DatasetNotFoundError):
         catalog.get_dataset(dogs_dataset.name)
 
     assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
 
     assert catalog.metastore.get_direct_dataset_dependencies(dogs_dataset, 1) == []
 
 
+def test_remove_dataset_dataset_not_found(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+
+    with pytest.raises(DatasetNotFoundError):
+        catalog.remove_dataset("wrong_name", force=True)
+
+
+def test_remove_dataset_wrong_version(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+
+    with pytest.raises(DatasetInvalidVersionError):
+        catalog.remove_dataset(dogs_dataset.name, version=100)
+
+
 def test_edit_dataset(cloud_test_catalog, dogs_dataset):
     dataset_old_name = dogs_dataset.name
     dataset_new_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
 
     catalog.edit_dataset(
         dogs_dataset.name,
@@ -704,36 +712,60 @@
     )
 
 
 def test_merge_datasets_existing_pending_version(
     cloud_test_catalog, dogs_dataset, cats_dataset
 ):
     catalog = cloud_test_catalog.catalog
+
+    # adding custom column
+    @udf(
+        (),
+        {"similarity": Float32},
+    )
+    def test_types():
+        return (0.5,)
+
+    (
+        DatasetQuery(name=cats_dataset.name, catalog=catalog)
+        .add_signals(test_types)
+        .save("cats_custom_column")
+    )
+
+    cats_custom_column = catalog.get_dataset("cats_custom_column")
+
     dogs_dataset = catalog.create_new_dataset_version(
         dogs_dataset,
         2,
         create_rows_table=False,
     )
 
     catalog.merge_datasets(
-        cats_dataset,
+        cats_custom_column,
         dogs_dataset,
         1,
         dst_version=2,
     )
 
     dogs_dataset = catalog.get_dataset(dogs_dataset.name)
     assert dogs_dataset.versions_values == [1, 2]
 
+    assert (
+        dogs_dataset.get_version(2).custom_column_types
+        == cats_custom_column.get_version(1).custom_column_types
+    )
+
+    assert "similarity" in dogs_dataset.get_version(2).custom_column_types
+
     assert {r.name for r in catalog.ls_dataset_rows(dogs_dataset.name, 2)} == {
         "cat1",
         "cat2",
     }
 
-    cats_dep = catalog.get_dataset_dependencies(cats_dataset.name, 1)
+    cats_dep = catalog.get_dataset_dependencies(cats_custom_column.name, 1)
     dogs_dep = catalog.get_dataset_dependencies(dogs_dataset.name, 2)
 
     assert set(dogs_dep) == set(cats_dep)
 
 
 @pytest.mark.parametrize("tree", [{str(i): str(i) for i in range(50)}], indirect=True)
 def test_row_random(cloud_test_catalog):
```

### Comparing `dvcx-0.71.0/tests/func/test_ls.py` & `dvcx-0.72.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/func/test_pull.py` & `dvcx-0.72.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/test_cli_e2e.py` & `dvcx-0.72.0/tests/test_cli_e2e.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import os.path
 import subprocess
-import tempfile
 from textwrap import dedent
 
+import pytest
+
 MNT_DATASET_ROWS = dedent(
     """
     01375.png
     07510.png
     08433.png
     mnist-info.txt
     readme.md
@@ -254,19 +255,12 @@
     else:
         assert "Instantiating" not in result.stderr
     files = step.get("files")
     if files:
         verify_files(files)
 
 
-def test_cli_e2e():
+@pytest.mark.e2e
+def test_cli_e2e(tmp_dir):
     """End-to-end CLI Test"""
-
-    original_cwd = os.getcwd()
-
-    with tempfile.TemporaryDirectory() as tempdir:
-        os.chdir(tempdir)
-        try:
-            for step in E2E_STEPS:
-                run_step(step)
-        finally:
-            os.chdir(original_cwd)
+    for step in E2E_STEPS:
+        run_step(step)
```

### Comparing `dvcx-0.71.0/tests/unit/lib/test_feature.py` & `dvcx-0.72.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.72.0/tests/unit/lib/test_feature_udf.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import (
     FeatureAggregator,
     FeatureBatchMapper,
     FeatureGenerator,
     FeatureMapper,
+    OutputError,
+    SchemaError,
+    UserCodeError,
 )
-from dvcx.lib.stream import FileStream
+from dvcx.lib.file import File
 from dvcx.query import Stream
 from dvcx.sql.types import Int
 
 
 class TestInput(Feature):
     name: str
     parent: str = Field(default="")
@@ -35,40 +38,68 @@
         input = row[0]
         output = TestOutput(
             full_path=os.path.join(input.parent, input.name), size_squared=input.size**2
         )
         yield (output,)
 
 
-def test_feature_udf():
+def test_feature_udf_yields_values():
     name = "file.txt"
     path = "dir1/dir2"
     size = 16
     params = ((name, path, size),)
 
     agg = MyAgg()
     res = list(agg(params))
     assert 1 == len(res)
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
+def test_feature_udf_returns_values():
+    class MyAggReturn(FeatureAggregator):
+        def __init__(self):
+            super().__init__([TestInput], [TestOutput])
+
+        def process(self, args):
+            row = args[0]
+            input = row[0]
+            output = TestOutput(
+                full_path=os.path.join(input.parent, input.name),
+                size_squared=input.size**2,
+            )
+            return [(output,)]
+
+    name = "f1.txt"
+    path = "d1/d2/d55"
+    size = 235
+    params = ((name, path, size),)
+
+    agg = MyAggReturn()
+    res = list(agg(params))
+    assert 1 == len(res)
+
+    full_path, size_squared = res[0]
+    assert full_path == os.path.join(path, name)
+    assert size_squared == size**2
+
+
 class MyAggStream(FeatureAggregator):
     def __init__(self):
-        super().__init__([FileStream], [TestOutput])
+        super().__init__([File], [TestOutput])
 
     def process(self, args):
         output = TestOutput(full_path="xx", size_squared=5)
         yield (output,)
 
 
 def test_feature_udf_with_stream():
-    stream = FileStream(name="tmp.jpg")
+    stream = File(name="tmp.jpg")
     args = ([Stream()] + list(stream._flatten()),)
 
     agg = MyAggStream()
     res = list(agg(args))
     assert 1 == len(res)
 
 
@@ -96,37 +127,37 @@
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
 def test_incompatible_params_types():
-    with pytest.raises(ValueError):
+    with pytest.raises(SchemaError):
 
         class MyAggParamInstance(FeatureAggregator):
             def __init__(self):
                 super().__init__(
                     (
                         ("size", Int),
                         ("test", Int),
                     ),
                     TestOutput,
                 )
 
         MyAggParamInstance()
 
-    with pytest.raises(ValueError):
+    with pytest.raises(SchemaError):
 
         class MyAggParamType(FeatureAggregator):
             def __init__(self):
                 super().__init__([Int, Int], TestOutput)
 
         MyAggParamType()
 
-    with pytest.raises(ValueError):
+    with pytest.raises(SchemaError):
 
         class MyAggOutputInstance(FeatureAggregator):
             def __init__(self):
                 super().__init__([Int], TestOutput)
 
         MyAggOutputInstance()
 
@@ -140,29 +171,29 @@
             input = args[0]
             output = TestOutput(
                 full_path=os.path.join(input.parent, input.name),
                 size_squared=input.size**2,
             )
             yield output, output, output
 
-    with pytest.raises(RuntimeError):
+    with pytest.raises(OutputError):
         params = (("file", "dir", 12345),)
         agg = MyAggWrongLength()
         agg(params)
 
 
 def test_output_type_missmatch_with_params_types():
     class MyAggWrongOutputType(FeatureAggregator):
         def __init__(self):
             super().__init__(TestInput, TestOutput)
 
         def process(self, args):
             yield 536
 
-    with pytest.raises(RuntimeError):
+    with pytest.raises(OutputError):
         params = (("file", "dir", 12345),)
         agg = MyAggWrongOutputType()
         agg(params)
 
 
 def test_mapper():
     class MyMap(FeatureMapper):
@@ -175,18 +206,47 @@
                 size_squared=test_input.size**2,
             )
             return output
 
     name = "img001.jpg"
     path = "data/dogs"
     size = 56743
-    params = ((name, path, size),)
+    params = (name, path, size)
 
     agg = MyMap()
-    res = agg(params)
+    res = agg(*params)
+
+    full_path, size_squared = res
+    assert full_path == os.path.join(path, name)
+    assert size_squared == size**2
+
+
+def test_mapper_stream():
+    class MyMapStream(FeatureMapper):
+        def __init__(self):
+            super().__init__([File, TestInput], TestOutput)
+
+        def process(self, inputs):
+            stream, test_input = inputs
+            output = TestOutput(
+                full_path=os.path.join(test_input.parent, test_input.name),
+                size_squared=test_input.size**2,
+            )
+            return output
+
+    stream = File(name="file.jpg")
+    stream_args = tuple([Stream()] + list(stream._flatten()))
+
+    name = "img001.jpg"
+    path = "data/dogs"
+    size = 56743
+    args = stream_args + (name, path, size)
+
+    agg = MyMapStream()
+    res = agg(*args)
 
     full_path, size_squared = res
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
 def test_batch_mapper():
@@ -222,36 +282,94 @@
 
 
 def test_generator():
     class MyGen(FeatureGenerator):
         def __init__(self):
             super().__init__(TestInput, TestOutput)
 
-        def process(self, test_inputs):
-            for test_input in test_inputs:
-                yield TestOutput(
-                    full_path=os.path.join(test_input.parent, test_input.name) + "_1",
-                    size_squared=test_input.size**2,
-                )
+        def process(self, test_input):
+            yield TestOutput(
+                full_path=os.path.join(test_input.parent, test_input.name) + "_1",
+                size_squared=test_input.size**2,
+            )
 
-                yield TestOutput(
-                    full_path=os.path.join(test_input.parent, test_input.name) + "_2",
-                    size_squared=test_input.size**3,
-                )
+            yield TestOutput(
+                full_path=os.path.join(test_input.parent, test_input.name) + "_2",
+                size_squared=test_input.size**3,
+            )
 
     name = "img742.jpg"
     path = "d1/cats"
     size = 384
-    params = ((name, path, size),)
+    params = (name, path, size)
 
     agg = MyGen()
-    res = agg(params)
+    res = agg(*params)
 
     assert 2 == len(res)
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name) + "_1"
     assert size_squared == size**2
 
     full_path, size_squared = res[1]
     assert full_path == os.path.join(path, name) + "_2"
     assert size_squared == size**3
+
+
+def test_feature_udf_output_value_instead_of_list():
+    class MyAggOutputValueInsteadOfList(FeatureMapper):
+        def __init__(self):
+            super().__init__([TestInput], [TestOutput])
+
+        def process(self, args):
+            input = args[0]
+            output = TestOutput(
+                full_path=os.path.join(input.parent, input.name),
+                size_squared=input.size**2,
+            )
+            return output
+
+    name = "file.txt"
+    path = "dir1/dir2"
+    size = 16
+    params = (name, path, size)
+
+    agg = MyAggOutputValueInsteadOfList()
+    with pytest.raises(OutputError):
+        list(agg(*params))
+
+
+def test_feature_udf_output_wrong_type():
+    class MyAggWrongOutputType(FeatureMapper):
+        def __init__(self):
+            super().__init__([TestInput], TestOutput)
+
+        def process(self, args):
+            return 34
+
+    name = "file.txt"
+    path = "dir1/dir2"
+    size = 16
+    params = (name, path, size)
+
+    agg = MyAggWrongOutputType()
+    with pytest.raises(OutputError):
+        list(agg(*params))
+
+
+def test_error_in_user_code():
+    class MyBuggyClass(FeatureMapper):
+        def __init__(self):
+            super().__init__(TestInput, TestOutput)
+
+        def process(self, args):
+            return 3.14 / 0
+
+    name = "file.txt"
+    path = "dir1/dir2"
+    size = 16
+    params = (name, path, size)
+
+    agg = MyBuggyClass()
+    with pytest.raises(UserCodeError):
+        list(agg(*params))
```

### Comparing `dvcx-0.71.0/tests/unit/lib/test_stream.py` & `dvcx-0.72.0/tests/unit/lib/test_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import pytest
 
 from dvcx.cache import DVCXCache, UniqueId
-from dvcx.lib.stream import FileStream
+from dvcx.lib.file import File
 
 
 def test_uid_missing_location():
     name = "my_name"
     vtype = "vt1"
 
-    stream = FileStream(name=name, vtype=vtype)
+    stream = File(name=name, vtype=vtype)
     assert stream.get_uid() == UniqueId("", "", name, "", 0, vtype, None)
 
 
 def test_uid_location():
     name = "na_me"
     vtype = "some_random"
-    loc = [{"e": 42}]
+    loc = {"e": 42}
 
-    stream = FileStream(name=name, vtype=vtype, location=loc)
+    stream = File(name=name, vtype=vtype, location=loc)
     assert stream.get_uid() == UniqueId("", "", name, "", 0, vtype, loc)
 
 
 def test_file_stem():
-    s = FileStream(name=".file.jpg.txt")
+    s = File(name=".file.jpg.txt")
     assert s.get_file_stem() == ".file.jpg"
 
 
 def test_file_ext():
-    s = FileStream(name=".file.jpg.txt")
+    s = File(name=".file.jpg.txt")
     assert s.get_file_ext() == "txt"
 
 
 @pytest.fixture
 def cache(tmp_path):
     return DVCXCache(str(tmp_path / "cache"), str(tmp_path / "tmp"))
 
 
 def test_cache_get_path(cache):
-    stream = FileStream(name="test.txt1", source="s3://mybkt")
+    stream = File(name="test.txt1", source="s3://mybkt")
     stream.set_cache(cache)
 
     uid = stream.get_uid()
     data = b"some data is heRe"
     cache.store_data(uid, data)
 
     path = stream.get_local_path()
     assert path is not None
 
     with open(path, mode="rb") as f:
         assert f.read() == data
 
 
 def test_cache_get_path_without_cache(cache):
-    stream = FileStream(name="test.txt1", source="s3://mybkt")
+    stream = File(name="test.txt1", source="s3://mybkt")
     with pytest.raises(RuntimeError):
         stream.get_local_path()
```

### Comparing `dvcx-0.71.0/tests/unit/sql/test_array.py` & `dvcx-0.72.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/sql/test_conditional.py` & `dvcx-0.72.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/sql/test_path.py` & `dvcx-0.72.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/sql/test_selectable.py` & `dvcx-0.72.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/sql/test_string.py` & `dvcx-0.72.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_asyn.py` & `dvcx-0.72.0/tests/unit/test_asyn.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 async def fake_io(i):
     # print(f"task {i}")
     await asyncio.sleep(i)
     return i
 
 
-def join_all_tasks(loop, timeout=0.1):
+def join_all_tasks(loop, timeout=4):
     tasks = asyncio.all_tasks(loop)
     if tasks:
         coro = asyncio.wait(tasks, timeout=timeout)
         future = asyncio.run_coroutine_threadsafe(coro, loop=loop)
         try:
             # Time out if any tasks are still running
             future.result(timeout=timeout)
@@ -66,15 +66,15 @@
     n_rows = 50
 
     async def process(row):
         await mapper.to_thread(functools.partial(sync, loop, fake_io, row))
         return row
 
     mapper = create_mapper(process, range(n_rows), workers=10, loop=loop)
-    result = [sync(loop, fake_io, i + n_rows) for i in mapper.iterate(timeout=0.1)]
+    result = [sync(loop, fake_io, i + n_rows) for i in mapper.iterate(timeout=4)]
     if mapper.order_preserving:
         assert result == list(range(n_rows, 2 * n_rows))
     else:
         assert set(result) == set(range(n_rows, 2 * n_rows))
 
 
 @pytest.mark.parametrize("create_mapper", [AsyncMapper, OrderedMapper])
@@ -88,15 +88,15 @@
         await mapper.to_thread(functools.partial(sync, loop, fake_io, row))
         return row
 
     class MyError(Exception):
         pass
 
     mapper = create_mapper(process, range(50), workers=10, loop=loop)
-    iterator = mapper.iterate(timeout=0.1)
+    iterator = mapper.iterate(timeout=4)
     next(iterator)
     with pytest.raises(MyError):
         iterator.throw(MyError)
 
 
 @pytest.mark.parametrize("create_mapper", [AsyncMapper, OrderedMapper])
 def test_mapper_exception_while_processing(create_mapper, loop):
@@ -104,15 +104,15 @@
         await mapper.to_thread(functools.partial(sync, loop, fake_io, row))
         if row == 12:
             raise RuntimeError
         return row
 
     mapper = create_mapper(process, range(50), workers=10, loop=loop)
     with pytest.raises(RuntimeError):
-        list(mapper.iterate(timeout=0.1))
+        list(mapper.iterate(timeout=4))
 
 
 @pytest.mark.parametrize("create_mapper", [AsyncMapper, OrderedMapper])
 @settings(deadline=None)
 @given(
     inputs=st.lists(st.integers(min_value=0, max_value=100), max_size=20),
     workers=st.integers(min_value=1, max_value=5),
@@ -122,15 +122,15 @@
         await asyncio.sleep(input)
         return input
 
     loop = get_loop()
     mapper = create_mapper(process, inputs, workers=workers, loop=loop)
     with mock_time(loop):
         try:
-            result = list(mapper.iterate(timeout=1.0))
+            result = list(mapper.iterate(timeout=4))
         finally:
             join_all_tasks(loop)
     if mapper.order_preserving:
         assert result == inputs
     else:
         assert Counter(result) == Counter(inputs)
 
@@ -155,10 +155,10 @@
             return input
 
     loop = get_loop()
     mapper = create_mapper(process, inputs, workers=workers, loop=loop)
     with mock_time(loop):
         try:
             with pytest.raises(RuntimeError):
-                list(mapper.iterate(timeout=1.0))
+                list(mapper.iterate(timeout=4))
         finally:
             join_all_tasks(loop)
```

### Comparing `dvcx-0.71.0/tests/unit/test_cache.py` & `dvcx-0.72.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_catalog.py` & `dvcx-0.72.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_catalog_formats.py` & `dvcx-0.72.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_cli_parsing.py` & `dvcx-0.72.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_client.py` & `dvcx-0.72.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_client_s3.py` & `dvcx-0.72.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_data_storage.py` & `dvcx-0.72.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_dataset.py` & `dvcx-0.72.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_fileslice.py` & `dvcx-0.72.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_id_generator.py` & `dvcx-0.72.0/tests/unit/test_id_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import base64
+import pickle
+
 from sqlalchemy import select
 
-from dvcx.data_storage.sqlite import SQLiteIDGenerator
+from dvcx.data_storage.serializer import deserialize
+from dvcx.data_storage.sqlite import SQLiteDatabaseEngine, SQLiteIDGenerator
 
 
 def get_rows(id_generator):
     uris = id_generator.db.execute(
         select(id_generator._table.c.uri, id_generator._table.c.last_id).select_from(
             id_generator._table
         )
@@ -73,14 +77,48 @@
     assert get_rows(clone) == get_rows(id_generator)
 
     clone.cleanup_for_tests()
     assert not id_generator.db.has_table("id_generator")
     assert not clone.db.has_table("id_generator")
 
 
+def test_serialize():
+    db = SQLiteDatabaseEngine.from_db_file(":memory:")
+
+    obj = SQLiteIDGenerator(db, table_prefix="prefix")
+    assert obj.db == db
+    assert obj._table_prefix == "prefix"
+
+    # Test clone
+    obj2 = obj.clone()
+    assert isinstance(obj2, SQLiteIDGenerator)
+    assert obj2.db.db_file == obj.db.db_file
+    assert obj2._table_prefix == "prefix"
+    assert obj2.clone_params() == obj.clone_params()
+
+    # Test serialization
+    serialized = obj.serialize()
+    assert serialized
+    serialized_pickled = base64.b64decode(serialized.encode())
+    assert serialized_pickled
+    (f, args, kwargs) = pickle.loads(serialized_pickled)  # noqa: S301
+    assert f == SQLiteIDGenerator.init_after_clone
+    assert args == []
+    assert kwargs == {
+        "db_clone_params": db.clone_params(),
+        "table_prefix": "prefix",
+    }
+
+    # Test deserialization
+    obj3 = deserialize(serialized)
+    assert isinstance(obj3, SQLiteIDGenerator)
+    assert obj3.db.db_file == db.db_file
+    assert obj3._table_prefix == "prefix"
+
+
 def test_init_id(id_generator):
     assert get_rows(id_generator) == set()
 
     id_generator.init_id("foo")
     assert get_rows(id_generator) == {("foo", 0)}
 
     assert id_generator.get_next_id("foo") == 1
```

### Comparing `dvcx-0.71.0/tests/unit/test_listing.py` & `dvcx-0.72.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_storage.py` & `dvcx-0.72.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_udf.py` & `dvcx-0.72.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.71.0/tests/unit/test_utils.py` & `dvcx-0.72.0/tests/unit/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,22 @@
             return "Hello!"
     """
     fname.write_text(dedent(code))
     func = import_object(f"{fname}:hello")
     assert func() == "Hello!"
 
 
-def test_import_object_relative(tmp_path):
+def test_import_object_relative(tmp_path, monkeypatch):
     fname = tmp_path / "foo.py"
     code = """\
         def hello():
             return "Hello!"
     """
     fname.write_text(dedent(code))
-    os.chdir(tmp_path)
+    monkeypatch.chdir(tmp_path)
     func = import_object("foo.py:hello")
     assert func() == "Hello!"
 
 
 def test_retry_with_backoff():
     called = 0
     retries = 2
```

### Comparing `dvcx-0.71.0/tests/utils.py` & `dvcx-0.72.0/tests/utils.py`

 * *Files identical despite different names*

