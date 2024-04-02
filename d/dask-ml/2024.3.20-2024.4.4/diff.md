# Comparing `tmp/dask-ml-2024.3.20.tar.gz` & `tmp/dask_ml-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-ml-2024.3.20.tar", last modified: Wed Mar 20 12:59:31 2024, max compression
+gzip compressed data, last modified: Tue Apr  2 02:31:39 2024, max compression
```

## Comparing `dask-ml-2024.3.20.tar` & `dask_ml-2024.4.4.tar`

### file list

```diff
@@ -1,143 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.136087 dask-ml-2024.3.20/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.108087 dask-ml-2024.3.20/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.112087 dask-ml-2024.3.20/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.github/workflows/upstream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-20 12:59:31.136087 dask-ml-2024.3.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.116087 dask-ml-2024.3.20/dask_ml/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.116087 dask-ml-2024.3.20/dask_ml/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/cluster/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19491 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/cluster/k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/cluster/spectral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.116087 dask-ml-2024.3.20/dask_ml/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/compose/_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.120087 dask-ml-2024.3.20/dask_ml/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/extmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/decomposition/truncated_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.120087 dask-ml-2024.3.20/dask_ml/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/ensemble/_blockwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.120087 dask-ml-2024.3.20/dask_ml/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/feature_extraction/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/impute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.120087 dask-ml-2024.3.20/dask_ml/linear_model/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/linear_model/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/linear_model/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/linear_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.120087 dask-ml-2024.3.20/dask_ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/metrics/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/metrics/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.124087 dask-ml-2024.3.20/dask_ml/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25510 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_hyperband.py
--rw-r--r--   0 runner    (1001) docker     (127)    51360 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    54713 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/_successive_halving.py
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/model_selection/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.124087 dask-ml-2024.3.20/dask_ml/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/preprocessing/_block_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/preprocessing/_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    38508 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/preprocessing/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/preprocessing/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    19975 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24157 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/dask_ml/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/dask_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-20 12:59:31.000000 dask-ml-2024.3.20/dask_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-20 12:59:31.000000 dask-ml-2024.3.20/dask_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 12:59:31.000000 dask-ml-2024.3.20/dask_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-20 12:59:31.000000 dask-ml-2024.3.20/dask_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 12:59:31.000000 dask-ml-2024.3.20/dask_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.124087 dask-ml-2024.3.20/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.128087 dask-ml-2024.3.20/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/clustering.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/compose.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/glm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/hyper-parameter-search.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)   107761 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/dimensions_of_scale.png
--rw-r--r--   0 runner    (1001) docker     (127)   596328 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/dimensions_of_scale.svg
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/merged_grid_search_graph.dot
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/merged_grid_search_graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/scaling-patience-true.svg
--rw-r--r--   0 runner    (1001) docker     (127)   168995 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/synthetic-dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    36605 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/synthetic-final-acc.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38861 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/synthetic-val-acc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/unmerged_grid_search_graph.dot
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/images/unmerged_grid_search_graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/incremental.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/joblib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/keras.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/meta-estimators.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/modules/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/docs/source/modules/generted/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/modules/generted/dask_ml.compose.ColumnTransformer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/modules/generted/dask_ml.compose.make_column_transformer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/naive-bayes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/pytorch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/roadmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/docs/source/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/class_with_call.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/class_without_init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/deprecated_class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/deprecated_class_with_call.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/deprecated_class_without_init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/deprecated_function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/templates/numpydoc_docstring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/docs/source/xgboost.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/licenses/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:59:31.132087 dask-ml-2024.3.20/licenses/scikit-learn/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/licenses/scikit-learn/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-20 12:59:31.136087 dask-ml-2024.3.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-20 12:59:17.000000 dask-ml-2024.3.20/setup.py
+-rw-r--r--   0        0        0      162 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/__init__.py
+-rw-r--r--   0        0        0     2253 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/_compat.py
+-rw-r--r--   0        0        0     6046 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/_partial.py
+-rw-r--r--   0        0        0      712 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/_typing.py
+-rw-r--r--   0        0        0     3122 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/_utils.py
+-rw-r--r--   0        0        0      417 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/_version.py
+-rw-r--r--   0        0        0     6633 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/base.py
+-rw-r--r--   0        0        0    14543 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/datasets.py
+-rw-r--r--   0        0        0     3056 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/impute.py
+-rw-r--r--   0        0        0     4571 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/naive_bayes.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/neural_network.py
+-rw-r--r--   0        0        0    20075 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/utils.py
+-rw-r--r--   0        0        0    24157 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/wrappers.py
+-rw-r--r--   0        0        0      254 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/xgboost.py
+-rw-r--r--   0        0        0      127 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/cluster/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/cluster/_compat.py
+-rw-r--r--   0        0        0    19491 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/cluster/k_means.py
+-rw-r--r--   0        0        0    13373 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/cluster/spectral.py
+-rw-r--r--   0        0        0      282 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/compose/__init__.py
+-rw-r--r--   0        0        0     9303 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/compose/_column_transformer.py
+-rw-r--r--   0        0        0      129 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/_compat.py
+-rw-r--r--   0        0        0     3628 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/extmath.py
+-rw-r--r--   0        0        0    16625 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/incremental_pca.py
+-rw-r--r--   0        0        0    17928 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/pca.py
+-rw-r--r--   0        0        0     8461 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/decomposition/truncated_svd.py
+-rw-r--r--   0        0        0      156 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/ensemble/__init__.py
+-rw-r--r--   0        0        0    10008 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/ensemble/_blockwise.py
+-rw-r--r--   0        0        0       93 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     9565 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/feature_extraction/text.py
+-rw-r--r--   0        0        0      267 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/linear_model/__init__.py
+-rw-r--r--   0        0        0    10439 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/linear_model/glm.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/linear_model/perceptron.py
+-rw-r--r--   0        0        0     2394 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/linear_model/utils.py
+-rw-r--r--   0        0        0      405 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/metrics/__init__.py
+-rw-r--r--   0        0        0     4440 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/metrics/classification.py
+-rw-r--r--   0        0        0     6251 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/metrics/pairwise.py
+-rw-r--r--   0        0        0     6655 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/metrics/regression.py
+-rw-r--r--   0        0        0     2484 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/metrics/scorer.py
+-rw-r--r--   0        0        0      742 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/__init__.py
+-rw-r--r--   0        0        0    25510 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_hyperband.py
+-rw-r--r--   0        0        0    51360 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_incremental.py
+-rw-r--r--   0        0        0     2485 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_normalize.py
+-rw-r--r--   0        0        0    54713 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_search.py
+-rw-r--r--   0        0        0    17857 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_split.py
+-rw-r--r--   0        0        0    11347 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/_successive_halving.py
+-rw-r--r--   0        0        0    14160 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/methods.py
+-rw-r--r--   0        0        0    10588 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/utils.py
+-rw-r--r--   0        0        0     7879 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/model_selection/utils_test.py
+-rw-r--r--   0        0        0      596 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3685 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/preprocessing/_block_transformer.py
+-rw-r--r--   0        0        0    10520 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/preprocessing/_encoders.py
+-rw-r--r--   0        0        0    38508 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/preprocessing/data.py
+-rw-r--r--   0        0        0    10940 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/dask_ml/preprocessing/label.py
+-rw-r--r--   0        0        0     1610 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/.gitignore
+-rw-r--r--   0        0        0     1479 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/README.rst
+-rw-r--r--   0        0        0     2310 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5949 2024-04-02 02:31:39.000000 dask_ml-2024.4.4/PKG-INFO
```

### Comparing `dask-ml-2024.3.20/LICENSE.txt` & `dask_ml-2024.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/README.rst` & `dask_ml-2024.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/_compat.py` & `dask_ml-2024.4.4/dask_ml/_compat.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/_partial.py` & `dask_ml-2024.4.4/dask_ml/_partial.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/_typing.py` & `dask_ml-2024.4.4/dask_ml/_typing.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/_utils.py` & `dask_ml-2024.4.4/dask_ml/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/base.py` & `dask_ml-2024.4.4/dask_ml/base.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/cluster/k_means.py` & `dask_ml-2024.4.4/dask_ml/cluster/k_means.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/cluster/spectral.py` & `dask_ml-2024.4.4/dask_ml/cluster/spectral.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-"""Algorithms for spectral clustering
-"""
+"""Algorithms for spectral clustering"""
+
 import logging
 
 import dask.array as da
 import numpy as np
 import sklearn.cluster
 from dask import delayed
 from scipy.linalg import pinv, svd
@@ -268,17 +268,15 @@
         U_A = da.from_delayed(U_A, (n_components, n_components), A2.dtype)
         S_A = da.from_delayed(S_A, (n_components,), A2.dtype)
         V_A = da.from_delayed(V_A, (n_components, n_components), A2.dtype)
 
         # Eq 16. This is OK when V2 is orthogonal
         V2 = da.sqrt(float(n_components) / n) * da.vstack([A2, B2.T]).dot(
             U_A[:, :n_clusters]
-        ).dot(
-            da.diag(1.0 / da.sqrt(S_A[:n_clusters]))
-        )  # (n, k)
+        ).dot(da.diag(1.0 / da.sqrt(S_A[:n_clusters])))  # (n, k)
         _log_array(logger, V2, "V2.1")
 
         if isinstance(B2, da.Array):
             V2 = V2.rechunk((B2.chunks[1][0], n_clusters))
             _log_array(logger, V2, "V2.2")
 
         # normalize (Eq. 4)
@@ -362,16 +360,16 @@
 
     slices = []
     if keep[0] > 0:  # avoid creating empty slices
         slices.append(slice(None, keep[0]))
     slices.append([keep[0]])
     windows = zip(keep[:-1], keep[1:])
 
-    for l, r in windows:
-        if r > l + 1:  # avoid creating empty slices
-            slices.append(slice(l + 1, r))
+    for left, r in windows:
+        if r > left + 1:  # avoid creating empty slices
+            slices.append(slice(left + 1, r))
         slices.append([r])
 
     if keep[-1] < len(array) - 1:  # avoid creating empty slices
         slices.append(slice(keep[-1] + 1, None))
     result = da.concatenate([array[idx[slice_]] for slice_ in slices])
     return result
```

### Comparing `dask-ml-2024.3.20/dask_ml/compose/_column_transformer.py` & `dask_ml-2024.4.4/dask_ml/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/datasets.py` & `dask_ml-2024.4.4/dask_ml/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/decomposition/extmath.py` & `dask_ml-2024.4.4/dask_ml/decomposition/extmath.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/decomposition/incremental_pca.py` & `dask_ml-2024.4.4/dask_ml/decomposition/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/decomposition/pca.py` & `dask_ml-2024.4.4/dask_ml/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/decomposition/truncated_svd.py` & `dask_ml-2024.4.4/dask_ml/decomposition/truncated_svd.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,17 @@
         """
         self.fit_transform(X)
         return self
 
     def _check_array(self, X):
         if self.n_components >= X.shape[1]:
             raise ValueError(
-                "n_components must be < n_features; "
-                "got {} >= {}".format(self.n_components, X.shape[1])
+                "n_components must be < n_features; " "got {} >= {}".format(
+                    self.n_components, X.shape[1]
+                )
             )
         return X
 
     def fit_transform(self, X, y=None):
         """Fit model to X and perform dimensionality reduction on X.
 
         Parameters
```

### Comparing `dask-ml-2024.3.20/dask_ml/ensemble/_blockwise.py` & `dask_ml-2024.4.4/dask_ml/ensemble/_blockwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             )
 
         estimators = [
             dask.delayed(sklearn.base.clone)(estimatord) for _ in range(len(Xs))
         ]
         results = [
             estimator_.fit(X_, y_, **kwargs)
-            for estimator_, X_, y_, in zip(estimators, Xs, ys)
+            for estimator_, X_, y_ in zip(estimators, Xs, ys)
         ]
         results = list(dask.compute(*results))
         self.estimators_ = results
 
     def _predict(self, X):
         """Collect results from many predict calls"""
         if isinstance(self, ClassifierMixin):
```

### Comparing `dask-ml-2024.3.20/dask_ml/feature_extraction/text.py` & `dask_ml-2024.4.4/dask_ml/feature_extraction/text.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/impute.py` & `dask_ml-2024.4.4/dask_ml/impute.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,17 @@
                 msg = "dask-ml does not currently implement add_indicator" ""
                 raise NotImplementedError(msg)
             self.indicator_ = None
 
         allowed_strategies = ["mean", "median", "most_frequent", "constant"]
         if self.strategy not in allowed_strategies:
             raise ValueError(
-                "Can only use these strategies: {0} "
-                " got strategy={1}".format(allowed_strategies, self.strategy)
+                "Can only use these strategies: {0} " " got strategy={1}".format(
+                    allowed_strategies, self.strategy
+                )
             )
 
         if not (pd.isna(self.missing_values) or self.strategy == "constant"):
             raise ValueError(
                 "dask_ml.preprocessing.Imputer only supports non-NA values for "
                 "'missing_values' when 'strategy=constant'."
             )
```

### Comparing `dask-ml-2024.3.20/dask_ml/linear_model/glm.py` & `dask_ml-2024.4.4/dask_ml/linear_model/glm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Generalized Linear Models for large datasets."""
+
 import textwrap
 
 from dask_glm import algorithms, families
 from dask_glm.utils import (
     accuracy_score,
     add_intercept,
     dot,
```

### Comparing `dask-ml-2024.3.20/dask_ml/linear_model/utils.py` & `dask_ml-2024.4.4/dask_ml/linear_model/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-"""
+""" """
 
 import dask.array as da
 import dask.dataframe as dd
 import numpy as np
 from multipledispatch import dispatch
 
 if getattr(dd, "_dask_expr_enabled", lambda: False)():
```

### Comparing `dask-ml-2024.3.20/dask_ml/metrics/classification.py` & `dask_ml-2024.4.4/dask_ml/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/metrics/pairwise.py` & `dask_ml-2024.4.4/dask_ml/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/metrics/regression.py` & `dask_ml-2024.4.4/dask_ml/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/metrics/scorer.py` & `dask_ml-2024.4.4/dask_ml/metrics/scorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     # This is the same as sklearns, only we use our SCORERS dict,
     # and don't have back-compat code
     if isinstance(scoring, str):
         try:
             scorer, kwargs = SCORERS[scoring]
         except KeyError:
             raise ValueError(
-                "{} is not a valid scoring value. "
-                "Valid options are {}".format(scoring, sorted(SCORERS))
+                "{} is not a valid scoring value. " "Valid options are {}".format(
+                    scoring, sorted(SCORERS)
+                )
             )
     else:
         scorer = scoring
         kwargs = {}
 
     kwargs["compute"] = compute
```

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/__init__.py` & `dask_ml-2024.4.4/dask_ml/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_hyperband.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_hyperband.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_incremental.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_incremental.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_normalize.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_normalize.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_search.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_split.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_split.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Utilities for splitting datasets.
-"""
+"""Utilities for splitting datasets."""
 
 import itertools
 import logging
 import numbers
 import warnings
 
 import dask
```

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/_successive_halving.py` & `dask_ml-2024.4.4/dask_ml/model_selection/_successive_halving.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/methods.py` & `dask_ml-2024.4.4/dask_ml/model_selection/methods.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/utils.py` & `dask_ml-2024.4.4/dask_ml/model_selection/utils.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/model_selection/utils_test.py` & `dask_ml-2024.4.4/dask_ml/model_selection/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,24 +167,26 @@
         if self.check_X is not None:
             assert self.check_X(X)
         if self.check_y is not None:
             assert self.check_y(y)
         self.classes_ = np.unique(check_array(y, ensure_2d=False, allow_nd=True))
         if self.expected_fit_params:
             missing = set(self.expected_fit_params) - set(fit_params)
-            assert (
-                len(missing) == 0
-            ), "Expected fit parameter(s) %s not " "seen." % list(missing)
+            assert len(missing) == 0, (
+                "Expected fit parameter(s) %s not " "seen." % list(missing)
+            )
             for key, value in fit_params.items():
-                assert len(value) == len(
-                    X
-                ), "Fit parameter %s has length" "%d; expected %d." % (
-                    key,
-                    len(value),
-                    len(X),
+                assert len(value) == len(X), (
+                    "Fit parameter %s has length"
+                    "%d; expected %d."
+                    % (
+                        key,
+                        len(value),
+                        len(X),
+                    )
                 )
         return self
 
     def predict(self, T):
         if self.check_X is not None:
             assert self.check_X(T)
         return self.classes_[np.zeros(_num_samples(T), dtype=np.int32)]
```

### Comparing `dask-ml-2024.3.20/dask_ml/naive_bayes.py` & `dask_ml-2024.4.4/dask_ml/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/preprocessing/__init__.py` & `dask_ml-2024.4.4/dask_ml/preprocessing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Utilties for Preprocessing data.
-"""
+"""Utilties for Preprocessing data."""
 
 from ._block_transformer import BlockTransformer
 from ._encoders import OneHotEncoder
 from .data import (
     Categorizer,
     DummyEncoder,
     MinMaxScaler,
```

### Comparing `dask-ml-2024.3.20/dask_ml/preprocessing/_block_transformer.py` & `dask_ml-2024.4.4/dask_ml/preprocessing/_block_transformer.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/preprocessing/_encoders.py` & `dask_ml-2024.4.4/dask_ml/preprocessing/_encoders.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/preprocessing/data.py` & `dask_ml-2024.4.4/dask_ml/preprocessing/data.py`

 * *Files identical despite different names*

### Comparing `dask-ml-2024.3.20/dask_ml/preprocessing/label.py` & `dask_ml-2024.4.4/dask_ml/preprocessing/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,16 +215,17 @@
 
 
 def _check_and_search_block(arr, uniques, onehot_dtype=None, block_info=None):
     diff = list(np.setdiff1d(arr, uniques, assume_unique=True))
 
     if diff:
         msg = (
-            "Block contains previously unseen values {}.\nBlock info:\n\n"
-            "{}".format(diff, block_info)
+            "Block contains previously unseen values {}.\nBlock info:\n\n" "{}".format(
+                diff, block_info
+            )
         )
         raise ValueError(msg)
 
     label_encoded = np.searchsorted(uniques, arr)
     if onehot_dtype:
         return _construct(label_encoded, uniques)
     else:
```

### Comparing `dask-ml-2024.3.20/dask_ml/utils.py` & `dask_ml-2024.4.4/dask_ml/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 
     left_attrs2 = set(left_attrs) - exclude
     right_attrs2 = set(right_attrs) - exclude
 
     assert left_attrs2 == right_attrs2, left_attrs2 ^ right_attrs2
 
     for attr in left_attrs2:
-        l = getattr(left, attr)
-        r = getattr(right, attr)
-        _assert_eq(l, r, name=attr, **kwargs)
+        lattr = getattr(left, attr)
+        rattr = getattr(right, attr)
+        _assert_eq(lattr, rattr, name=attr, **kwargs)
 
 
 def check_array(
     array,
     *args,
     accept_dask_array=True,
     accept_dask_dataframe=False,
@@ -214,35 +214,35 @@
     elif isinstance(array, pd.DataFrame) and preserve_pandas_dataframe:
         # TODO: validation?
         return array
     else:
         return sk_validation.check_array(array, *args, **kwargs)
 
 
-def _assert_eq(l, r, name=None, **kwargs):
+def _assert_eq(lattr, rattr, name=None, **kwargs):
     array_types = (np.ndarray, da.Array)
     if getattr(dd, "_dask_expr_enabled", lambda: False)():
         from dask_expr import FrameBase
 
         frame_types = (pd.core.generic.NDFrame, FrameBase)
     else:
         frame_types = (pd.core.generic.NDFrame, dd._Frame)
-    if isinstance(l, array_types):
-        assert_eq_ar(l, r, **kwargs)
-    elif isinstance(l, frame_types):
-        assert_eq_df(l, r, **kwargs)
-    elif isinstance(l, Sequence) and any(
-        isinstance(x, array_types + frame_types) for x in l
+    if isinstance(lattr, array_types):
+        assert_eq_ar(lattr, rattr, **kwargs)
+    elif isinstance(lattr, frame_types):
+        assert_eq_df(lattr, rattr, **kwargs)
+    elif isinstance(lattr, Sequence) and any(
+        isinstance(x, array_types + frame_types) for x in lattr
     ):
-        for a, b in zip(l, r):
+        for a, b in zip(lattr, rattr):
             _assert_eq(a, b, **kwargs)
-    elif np.isscalar(r) and np.isnan(r):
-        assert np.isnan(l), (name, l, r)
+    elif np.isscalar(rattr) and np.isnan(rattr):
+        assert np.isnan(lattr), (name, lattr, rattr)
     else:
-        assert l == r, (name, l, r)
+        assert lattr == rattr, (name, lattr, rattr)
 
 
 def check_random_state(random_state):
     if random_state is None:
         return da.random.RandomState()
     elif isinstance(random_state, Integral):
         return da.random.RandomState(random_state)
```

### Comparing `dask-ml-2024.3.20/dask_ml/wrappers.py` & `dask_ml-2024.4.4/dask_ml/wrappers.py`

 * *Files identical despite different names*

