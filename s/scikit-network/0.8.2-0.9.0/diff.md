# Comparing `tmp/scikit-network-0.8.2.tar.gz` & `tmp/scikit-network-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-network-0.8.2.tar", last modified: Fri Jul 19 09:53:54 2019, max compression
+gzip compressed data, was "dist/scikit-network-0.9.0.tar", last modified: Wed Jul 24 16:21:50 2019, max compression
```

## Comparing `scikit-network-0.8.2.tar` & `scikit-network-0.9.0.tar`

### file list

```diff
@@ -1,131 +1,142 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-07-19 09:52:29.000000 scikit-network-0.8.2/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/authors.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/tutorials/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/tutorials/hierarchy/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/tutorials/hierarchy/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/tutorials/clustering/
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/tutorials/clustering/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/tutorials/ranking/
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/tutorials/ranking/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/docs/reference/
--rw-rw-r--   0 travis    (2000) travis    (2000)      634 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/clustering.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1192 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/utils.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      772 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/hierarchy.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/loader.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      482 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/embedding.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/ranking.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/introduction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      170 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/toy_graphs.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      692 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/reference/linalg.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5423 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/genindex.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2019-07-19 09:52:29.000000 scikit-network-0.8.2/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)     3555 2019-07-19 09:52:29.000000 scikit-network-0.8.2/CONTRIBUTING.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/
--rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/loader/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4189 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/loader/parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/loader/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/loader/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2225 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/loader/tests/test_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/loader/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/hierarchy/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17332 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/paris.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/cuts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5727 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/hierarchy/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      772 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/tests/test_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2020 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/tests/test_paris.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/hierarchy/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/linalg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5758 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/svd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5190 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/eig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15282 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/randomized_matrix_factorization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4163 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/sparse_lowrank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/auto_mode.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/linalg/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/tests/test_sparse_lowrank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1962 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/tests/test_eig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/tests/test_svd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/linalg/tests/test_randomized_matrix_factorization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/clustering/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6244 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5740 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/bilouvain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/postprocessing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18835 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/louvain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      221 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/clustering/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/tests/test_louvain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/tests/test_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/tests/test_bilouvain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/clustering/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6558 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/checks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2732 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/preprocessing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2538 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/lazy_property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3928 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/adjacency_formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      935 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/algorithm_base_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/projection_simplex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/utils/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      641 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/tests/test_projection_simplex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/tests/test_preprocessing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/tests/test_algorithm_base_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/tests/test_formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/utils/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/ranking/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2793 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/diffusion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3708 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/pagerank.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/ranking/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1223 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/tests/test_diffusion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      799 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/tests/test_pagerank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/ranking/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/sknetwork.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/toy_graphs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3933 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/block_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/toy_graphs/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      890 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/tests/test_block_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      707 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/tests/test_graph_imports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16332 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/toy_graphs/graph_data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/embedding/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6375 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6293 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/spectral.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/sknetwork/embedding/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2062 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/tests/test_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/tests/test_embeddings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/tests/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5332 2019-07-19 09:52:29.000000 scikit-network-0.8.2/sknetwork/embedding/gsvd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-07-19 09:53:54.000000 scikit-network-0.8.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-07-19 09:52:29.000000 scikit-network-0.8.2/AUTHORS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     3259 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-07-19 09:53:54.000000 scikit-network-0.8.2/scikit_network.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      451 2019-07-19 09:53:54.000000 scikit-network-0.8.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1231 2019-07-19 09:52:29.000000 scikit-network-0.8.2/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2019-07-19 09:52:29.000000 scikit-network-0.8.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2019-07-19 09:52:29.000000 scikit-network-0.8.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2019-07-19 09:52:29.000000 scikit-network-0.8.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-19 09:53:54.000000 scikit-network-0.8.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2019-07-19 09:52:29.000000 scikit-network-0.8.2/tests/test_sknetwork.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-07-24 16:19:37.000000 scikit-network-0.9.0/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/authors.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/loader/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/tutorials/loader/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/hierarchy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/tutorials/hierarchy/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/clustering/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/tutorials/clustering/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/ranking/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/tutorials/ranking/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/tutorials/embedding/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/tutorials/embedding/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/docs/reference/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      634 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/clustering.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/utils.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      772 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/hierarchy.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/loader.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/embedding.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/ranking.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/introduction.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      181 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      593 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/toy_graphs.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      692 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/linalg.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2292 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/reference/basics.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5423 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/genindex.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      771 2019-07-24 16:19:37.000000 scikit-network-0.9.0/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3555 2019-07-24 16:19:37.000000 scikit-network-0.9.0/CONTRIBUTING.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/basics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2618 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/search.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/structure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2081 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/shortest_path.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/basics/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1803 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/tests/test_structure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/basics/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/cli.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/loader/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4969 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/loader/parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/loader/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/loader/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2253 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/loader/tests/test_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/loader/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/hierarchy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17332 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/paris.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/cuts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5727 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      190 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/hierarchy/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      772 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/tests/test_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2020 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/tests/test_paris.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/hierarchy/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/linalg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5758 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/svd_solver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5190 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/spectral_solver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15282 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/randomized_matrix_factorization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4163 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/sparse_lowrank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/auto_mode.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/linalg/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/tests/test_sparse_lowrank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1962 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/tests/test_eig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/tests/test_svd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/linalg/tests/test_randomized_matrix_factorization.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/clustering/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6244 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5740 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/bilouvain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      670 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/postprocessing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18835 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/louvain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/clustering/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/tests/test_louvain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/tests/test_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/tests/test_bilouvain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/clustering/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6544 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/checks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2538 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/lazy_property.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3928 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/adjacency_formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      935 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/algorithm_base_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/projection_simplex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/utils/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      641 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/tests/test_projection_simplex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/tests/test_algorithm_base_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/tests/test_formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/utils/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/ranking/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2887 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/diffusion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3719 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/pagerank.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/ranking/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1223 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/tests/test_diffusion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      799 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/tests/test_pagerank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/ranking/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       44 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/sknetwork.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/toy_graphs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3933 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/block_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/toy_graphs/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      890 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/tests/test_block_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      707 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/tests/test_graph_imports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16829 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/toy_graphs/graph_data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/embedding/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6185 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/metrics.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5557 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/svd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6568 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/spectral.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/sknetwork/embedding/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/tests/test_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1997 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/tests/test_embeddings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-07-24 16:19:37.000000 scikit-network-0.9.0/sknetwork/embedding/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4318 2019-07-24 16:21:50.000000 scikit-network-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-07-24 16:19:37.000000 scikit-network-0.9.0/AUTHORS.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4318 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3489 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-07-24 16:21:50.000000 scikit-network-0.9.0/scikit_network.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      451 2019-07-24 16:21:50.000000 scikit-network-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1508 2019-07-24 16:19:37.000000 scikit-network-0.9.0/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2019-07-24 16:19:37.000000 scikit-network-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2019-07-24 16:19:37.000000 scikit-network-0.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2019-07-24 16:19:37.000000 scikit-network-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-07-24 16:21:50.000000 scikit-network-0.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2019-07-24 16:19:37.000000 scikit-network-0.9.0/tests/test_sknetwork.py
```

### Comparing `scikit-network-0.8.2/docs/Makefile` & `scikit-network-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/reference/clustering.rst` & `scikit-network-0.9.0/docs/reference/clustering.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/reference/utils.rst` & `scikit-network-0.9.0/docs/reference/utils.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 .. autofunction:: sknetwork.utils.adjacency_formats.bipartite2directed
 
 .. autofunction:: sknetwork.utils.adjacency_formats.bipartite2undirected
 
 .. autofunction:: sknetwork.utils.adjacency_formats.directed2undirected
 
 
-Preprocessing
--------------
-
-.. autofunction:: sknetwork.utils.preprocessing.largest_connected_component
-
-
 Projection
 ----------
 
 .. autofunction:: sknetwork.utils.projection_simplex
 
 
 Checks
```

### Comparing `scikit-network-0.8.2/docs/reference/hierarchy.rst` & `scikit-network-0.9.0/docs/reference/hierarchy.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/reference/introduction.rst` & `scikit-network-0.9.0/docs/reference/introduction.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/reference/toy_graphs.rst` & `scikit-network-0.9.0/docs/reference/toy_graphs.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/reference/linalg.rst` & `scikit-network-0.9.0/docs/reference/linalg.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/conf.py` & `scikit-network-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/installation.rst` & `scikit-network-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/docs/make.bat` & `scikit-network-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/CONTRIBUTING.rst` & `scikit-network-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/loader/parser.py` & `scikit-network-0.9.0/sknetwork/loader/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Dec 5, 2018
 @author: Quentin Lutz <qlutz@enst.fr>, Nathan de Lara <ndelara@enst.fr>
 """
 
-import numpy as np
-from numpy import zeros, unique, argmax, int32, int64, ones, concatenate
+from numpy import zeros, unique, argmax, ones, concatenate
 from scipy import sparse
 from typing import Tuple, Union
 from csv import reader
 
 
 def parse_tsv(file: str, directed: bool = False, bipartite: bool = False, weighted: bool = None,
-              labeled: bool = None, comment: str = '%#', delimiter: str = None) ->Tuple[sparse.csr_matrix,
-                                                                                        Union[np.ndarray, None]]:
+              labeled: bool = None, comment: str = '%#', delimiter: str = None) -> Union[sparse.csr_matrix,
+                                                                                         Tuple[sparse.csr_matrix, dict],
+                                                                                         Tuple[sparse.csr_matrix, dict,
+                                                                                               dict]]:
     """
     A parser for Tabulation-Separated, Comma-Separated or Space-Separated (or other) Values datasets.
 
     Parameters
     ----------
     file : str
-        the path to the dataset in TSV format
+        The path to the dataset in TSV format
     directed : bool
-        ensures the adjacency matrix is symmetric if False
+        If False, considers the graph as undirected.
     bipartite : bool
-        if True, returns the biadjacency matrix of shape (n1, n2)
+        If True, returns a biadjacency matrix of shape (n, p).
     weighted : Union[NoneType, bool]
-        retrieves the weights in the third field of the file. None makes a guess based on the first lines
+        Retrieves the weights in the third field of the file. None makes a guess based on the first lines.
     labeled : Union[NoneType, bool]
-        retrieves the names given to the nodes and renumbers them. Returns an additional array. None makes a guess
-        based on the first lines
+        Retrieves the names given to the nodes and renumbers them. Returns an additional array. None makes a guess
+        based on the first lines.
     comment : str
-        set of characters denoting lines to ignore
+        Set of characters denoting lines to ignore.
     delimiter : str
         delimiter used in the file. None makes a guess
 
     Returns
     -------
     adjacency : csr_matrix
-        the adjacency matrix of the adjacency
-    labels : numpy.array
-        an array such that labels[k] is the label or the new index given to the k-th node, None if no labels
-
+        Adjacency or biadjacency matrix of the graph.
+    labels : dict, optional
+        Label of each node.
+    feature_labels : dict, optional
+        Label of each feature node (for bipartite graph).
     """
     reindex = False
     header_len = -1
     possible_delimiters = ['\t', ',', ' ']
     del_count = zeros(3, dtype=int)
     lines = []
     row = comment
@@ -83,37 +85,43 @@
                     cols.append(row[1])
                 else:
                     rows.append(int(row[0]))
                     cols.append(int(row[1]))
                 if weighted:
                     dat.append(float(row[2]))
     n_edges = len(rows)
-    nodes = concatenate((rows, cols), axis=None)
-    labels, new_nodes = unique(nodes, return_inverse=True)
-    n_nodes = len(labels)
-    if labeled:
-        rows = new_nodes[:n_edges]
-        cols = new_nodes[n_edges:]
+    if bipartite:
+        labels, rows = unique(rows, return_inverse=True)
+        feature_labels, cols = unique(cols, return_inverse=True)
+        n_nodes = len(labels)
+        n_feature_nodes = len(feature_labels)
+        if not weighted:
+            dat = ones(n_edges, dtype=bool)
+        biadjacency = sparse.csr_matrix((dat, (rows, cols)), shape=(n_nodes, n_feature_nodes))
+        if labeled:
+            labels = {i: l for i, l in enumerate(labels)}
+            feature_labels = {i: l for i, l in enumerate(feature_labels)}
+            return biadjacency, labels, feature_labels
+        else:
+            return biadjacency
     else:
-        if not all(labels == range(len(labels))):
-            reindex = True
+        nodes = concatenate((rows, cols), axis=None)
+        labels, new_nodes = unique(nodes, return_inverse=True)
+        n_nodes = len(labels)
+        if labeled:
             rows = new_nodes[:n_edges]
             cols = new_nodes[n_edges:]
-    if not weighted:
-        dat = ones(n_edges, dtype=bool)
-
-    if n_nodes < 2 * 10e9:
-        dtype = int32
-    else:
-        dtype = int64
-
-    if bipartite:
-        adjacency = sparse.csr_matrix((dat, (rows, cols)), dtype=dtype)
-    else:
-        adjacency = sparse.csr_matrix((dat, (rows, cols)), shape=(n_nodes, n_nodes), dtype=dtype)
+        else:
+            if not all(labels == range(len(labels))):
+                reindex = True
+                rows = new_nodes[:n_edges]
+                cols = new_nodes[n_edges:]
+        if not weighted:
+            dat = ones(n_edges, dtype=bool)
+        adjacency = sparse.csr_matrix((dat, (rows, cols)), shape=(n_nodes, n_nodes))
         if not directed:
             adjacency += adjacency.transpose()
-    if labeled or reindex:
-        return adjacency, labels
-    else:
-        return adjacency, None
-
+        if labeled or reindex:
+            labels = {i: l for i, l in enumerate(labels)}
+            return adjacency, labels
+        else:
+            return adjacency
```

### Comparing `scikit-network-0.8.2/sknetwork/loader/tests/test_parser.py` & `scikit-network-0.9.0/sknetwork/loader/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 """tests for parser.py"""
 
 
 import unittest
 from os import remove
 from sknetwork.loader import parser
+import numpy as np
 
 
 class TestTSVParser(unittest.TestCase):
 
     def setUp(self):
         self.stub_data_1 = 'stub_1.txt'
         text_file = open(self.stub_data_1, "w")
@@ -34,29 +35,28 @@
     def tearDown(self):
         remove(self.stub_data_1)
         remove(self.stub_data_2)
         remove(self.stub_data_3)
         remove(self.stub_data_4)
 
     def test_unlabeled_unweighted(self):
-        adj, labels = parser.parse_tsv(self.stub_data_1)
+        adj = parser.parse_tsv(self.stub_data_1)
         self.assertEqual(sum(adj.indices == [2, 3, 0, 1, 5, 4]), 6)
         self.assertEqual(sum(adj.indptr == [0, 1, 2, 3, 4, 5, 6]), 7)
         self.assertEqual(sum(adj.data == [1, 1, 1, 1, 1, 1]), 6)
-        self.assertIsNone(labels)
 
     def test_labeled_weighted(self):
         adj, labels = parser.parse_tsv(self.stub_data_2)
         self.assertEqual(sum(adj.indices == [4, 3, 5, 1, 0, 2]), 6)
         self.assertEqual(sum(adj.indptr == [0, 1, 2, 3, 4, 5, 6]), 7)
         self.assertEqual(sum(adj.data == [1, 6, 5, 6, 1, 5]), 6)
-        self.assertEqual(sum(labels == [' b', ' d', ' e', 'a', 'c', 'f']), 6)
+        self.assertEqual(sum(np.array(list(labels.values())) == [' b', ' d', ' e', 'a', 'c', 'f']), 6)
 
     def test_auto_reindex(self):
         adj, labels = parser.parse_tsv(self.stub_data_4)
         self.assertEqual(sum(adj.indices == [1, 0, 3, 2, 5, 4]), 6)
         self.assertEqual(sum(adj.indptr == [0, 1, 2, 3, 4, 5, 6]), 7)
         self.assertEqual(sum(adj.data == [1, 1, 1, 1, 1, 1]), 6)
-        self.assertEqual(sum(labels == [0, 12, 14, 31, 42, 50]), 6)
+        self.assertEqual(sum(np.array(list(labels.values())) == [0, 12, 14, 31, 42, 50]), 6)
 
-    def test_poor_format(self):
+    def test_wrong_format(self):
         self.assertRaises(ValueError, parser.parse_tsv, self.stub_data_3)
```

### Comparing `scikit-network-0.8.2/sknetwork/hierarchy/paris.py` & `scikit-network-0.9.0/sknetwork/hierarchy/paris.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/hierarchy/cuts.py` & `scikit-network-0.9.0/sknetwork/hierarchy/cuts.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/hierarchy/metrics.py` & `scikit-network-0.9.0/sknetwork/hierarchy/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/hierarchy/tests/test_metrics.py` & `scikit-network-0.9.0/sknetwork/hierarchy/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/hierarchy/tests/test_paris.py` & `scikit-network-0.9.0/sknetwork/hierarchy/tests/test_paris.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/svd.py` & `scikit-network-0.9.0/sknetwork/linalg/svd_solver.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/eig.py` & `scikit-network-0.9.0/sknetwork/linalg/spectral_solver.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/randomized_matrix_factorization.py` & `scikit-network-0.9.0/sknetwork/linalg/randomized_matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/sparse_lowrank.py` & `scikit-network-0.9.0/sknetwork/linalg/sparse_lowrank.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/auto_mode.py` & `scikit-network-0.9.0/sknetwork/linalg/auto_mode.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/tests/test_sparse_lowrank.py` & `scikit-network-0.9.0/sknetwork/linalg/tests/test_sparse_lowrank.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/tests/test_eig.py` & `scikit-network-0.9.0/sknetwork/linalg/tests/test_eig.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/tests/test_svd.py` & `scikit-network-0.9.0/sknetwork/linalg/tests/test_svd.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/linalg/tests/test_randomized_matrix_factorization.py` & `scikit-network-0.9.0/sknetwork/linalg/tests/test_randomized_matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/metrics.py` & `scikit-network-0.9.0/sknetwork/clustering/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/bilouvain.py` & `scikit-network-0.9.0/sknetwork/clustering/bilouvain.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/postprocessing.py` & `scikit-network-0.9.0/sknetwork/clustering/postprocessing.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/louvain.py` & `scikit-network-0.9.0/sknetwork/clustering/louvain.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/tests/test_louvain.py` & `scikit-network-0.9.0/sknetwork/clustering/tests/test_louvain.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/tests/test_metrics.py` & `scikit-network-0.9.0/sknetwork/clustering/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/clustering/tests/test_bilouvain.py` & `scikit-network-0.9.0/sknetwork/clustering/tests/test_bilouvain.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/checks.py` & `scikit-network-0.9.0/sknetwork/utils/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         err = entry.dot(np.ones(n_features)) - np.ones(n_samples)
         return has_nonnegative_entries(entry) and np.isclose(np.linalg.norm(err), 0)
     else:
         raise TypeError('Entry must be one or two-dimensional array.')
 
 
 def is_square(adjacency: Union[sparse.csr_matrix, np.ndarray]) -> bool:
-    """
-    Checks whether the matrix is square.
+    """Checks whether the matrix is square.
     """
     return adjacency.shape[0] == adjacency.shape[1]
 
 
 def is_symmetric(adjacency: Union[sparse.csr_matrix, np.ndarray], tol: float = 1e-10) -> bool:
     """Checks whether the matrix is symmetric.
     """
@@ -60,15 +59,15 @@
     """Returns an array of weights from a matrix and a desired distribution.
 
        Parameters
        ----------
        distribution:
            Distribution for node sampling. Only ``'degree'`` or ``'uniform'`` are accepted.
        adjacency:
-           The adjacency matrix of the adjacency.
+           The adjacency matrix of the graph.
 
        Returns
        -------
        node_weights: np.ndarray
            Valid weights of nodes.
 
     """
@@ -100,16 +99,15 @@
         engine = 'python'
     else:
         raise ValueError('Engine must be default, python or numba.')
     return engine
 
 
 def check_format(adjacency: Union[sparse.csr_matrix, np.ndarray]) -> sparse.csr_matrix:
-    """
-    Checks whether the matrix is an instance of a supported type (NumPy array or Scipy CSR matrix) and returns
+    """Checks whether the matrix is an instance of a supported type (NumPy array or Scipy CSR matrix) and returns
     the corresponding Scipy CSR matrix.
     """
     if type(adjacency) not in {sparse.csr_matrix, np.ndarray}:
         raise TypeError('Adjacency must be in Scipy CSR format or Numpy ndarray format.')
     else:
         return sparse.csr_matrix(adjacency)
 
@@ -129,15 +127,15 @@
     """Checks whether the weights are a valid distribution for the adjacency and returns a probability vector.
 
     Parameters
     ----------
     weights:
         Probabilities for node sampling in the null model. ``'degree'``, ``'uniform'`` or custom weights.
     adjacency:
-        The adjacency matrix of the adjacency.
+        The adjacency matrix of the graph.
     positive_entries:
         If true, the weights must all be positive, if False, the weights must be nonnegative.
 
     Returns
     -------
     node_weights: np.ndarray
         Valid weights of nodes.
@@ -162,15 +160,16 @@
             raise ValueError('Node weights must be non-negative with positive sum.')
 
     return node_weights_vec
 
 
 def check_probs(weights: Union['str', np.ndarray], adjacency: Union[sparse.csr_matrix, sparse.csc_matrix],
                 positive_entries: bool = False) -> np.ndarray:
-    """Checks whether the weights are a valid distribution for the adjacency and returns a normalized probability vector.
+    """Checks whether the weights are a valid distribution for the adjacency
+    and returns a normalized probability vector.
     """
     weights = check_weights(weights, adjacency, positive_entries)
     return weights / np.sum(weights)
 
 
 def check_random_state(random_state: Optional[Union[np.random.RandomState, int]]):
     """Checks whether the argument is a seed or a NumPy random state. If None, numpy.random is used by default.
```

### Comparing `scikit-network-0.8.2/sknetwork/utils/lazy_property.py` & `scikit-network-0.9.0/sknetwork/utils/lazy_property.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/adjacency_formats.py` & `scikit-network-0.9.0/sknetwork/utils/adjacency_formats.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/algorithm_base_class.py` & `scikit-network-0.9.0/sknetwork/utils/algorithm_base_class.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/projection_simplex.py` & `scikit-network-0.9.0/sknetwork/utils/projection_simplex.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/tests/test_projection_simplex.py` & `scikit-network-0.9.0/sknetwork/utils/tests/test_projection_simplex.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/tests/test_preprocessing.py` & `scikit-network-0.9.0/sknetwork/basics/tests/test_structure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 # -*- coding: utf-8 -*-
 # tests for metrics.py
-""""tests for preprocessing.py"""
+""""tests for structure.py"""
 
 import unittest
 import numpy as np
-from sknetwork.utils.preprocessing import largest_connected_component
+from sknetwork.basics.structure import largest_connected_component, is_bipartite
+from sknetwork.utils.adjacency_formats import bipartite2undirected
+from sknetwork.toy_graphs import star_wars_villains, rock_paper_scissors
 
 
-class TestPreprocessing(unittest.TestCase):
+class TestStructure(unittest.TestCase):
     def setUp(self):
-        self.adjacency = np.array([[0, 0, 1], [0, 1, 0], [1, 0, 0]])
-        self.biadjacency = np.array([[0, 1], [1, 0], [0, 1]])
+        self.adjacency = rock_paper_scissors()
+        self.adjacency += self.adjacency.T
+        self.biadjacency = star_wars_villains()
+        self.undirected_bipartite = bipartite2undirected(self.biadjacency)
 
     def test_largest_cc(self):
         largest_cc, indices = largest_connected_component(self.adjacency, return_labels=True)
-        self.assertAlmostEqual(np.linalg.norm(largest_cc.toarray() - np.array([[0, 1], [1, 0]])), 0)
-        self.assertEqual(np.linalg.norm(indices - np.array([0, 2])), 0)
+        self.assertAlmostEqual(np.linalg.norm(largest_cc.toarray() - np.array([[0, 1, 1], [1, 0, 1], [1, 1, 0]])), 0)
+        self.assertEqual(np.linalg.norm(indices - np.array([0, 1, 2])), 0)
         largest_cc, indices = largest_connected_component(self.biadjacency, return_labels=True)
-        self.assertAlmostEqual(np.linalg.norm(largest_cc.toarray() - np.array([[1], [1]])), 0)
-        self.assertEqual(np.linalg.norm(indices[0] - np.array([0, 2])), 0)
-        self.assertEqual(np.linalg.norm(indices[1] - np.array([1])), 0)
+        self.assertAlmostEqual(np.linalg.norm(largest_cc.toarray() - np.array([[1, 0, 1],
+                                                                              [1, 0, 0],
+                                                                              [1, 1, 1],
+                                                                              [0, 1, 1]])), 0)
+        self.assertEqual(np.linalg.norm(indices[0] - np.array([0, 1, 2, 3])), 0)
+        self.assertEqual(np.linalg.norm(indices[1] - np.array([0, 1, 2])), 0)
+
+    def test_is_bipartite(self):
+        bipartite, biadjacency = is_bipartite(self.undirected_bipartite, return_biadjacency=True)
+        self.assertEqual(bipartite, True)
+        self.assertEqual(np.all(biadjacency.data == self.biadjacency.data), True)
```

### Comparing `scikit-network-0.8.2/sknetwork/utils/tests/test_algorithm_base_class.py` & `scikit-network-0.9.0/sknetwork/utils/tests/test_algorithm_base_class.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/utils/tests/test_formats.py` & `scikit-network-0.9.0/sknetwork/utils/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/ranking/diffusion.py` & `scikit-network-0.9.0/sknetwork/ranking/diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,17 @@
                 b = personalization
                 border = personalization.astype(bool)
             else:
                 raise ValueError('Personalization must be a dictionary or a vector'
                                  ' of length equal to the number of nodes.')
 
             diag_out: sparse.csr_matrix = sparse.diags(adjacency.dot(np.ones(n)), shape=(n, n), format='csr')
-            diag_out.data = 1 / diag_out.data * (1 - border)
-            diffusion_matrix = diag_out.dot(adjacency)
+            diag_out.data = 1 / diag_out.data
+            interior: sparse.csr_matrix = sparse.diags(1 - border, shape=(n, n), format='csr')
+            diffusion_matrix = interior.dot(diag_out.dot(adjacency))
 
             a = sparse.eye(n, format='csr') - diffusion_matrix
             self.score_ = spsolve(a, b)
 
         else:
             self.score_ = np.zeros(n)
```

### Comparing `scikit-network-0.8.2/sknetwork/ranking/pagerank.py` & `scikit-network-0.9.0/sknetwork/ranking/pagerank.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 if type(personalization) == np.ndarray and len(personalization) == n \
                         and has_nonnegative_entries(personalization) and np.sum(personalization):
                     restart_prob = personalization.astype(float) / np.sum(personalization)
                 else:
                     raise ValueError('Personalization must be None or a non-negative, non-null vector or a dictionary.')
 
             a = sparse.eye(n, format='csr') - self.damping_factor * transition_matrix.T
-            b = (1 - self.damping_factor * diag_out.data.astype(bool)) * restart_prob
+            b = (1 - self.damping_factor * diag_out.dot(np.ones(n)).astype(bool)) * restart_prob
             x = spsolve(a, b)
 
             self.score_ = abs(x.real) / abs(x.real).sum()
         else:
             self.score_ = np.zeros(n)
 
         return self
```

### Comparing `scikit-network-0.8.2/sknetwork/ranking/tests/test_diffusion.py` & `scikit-network-0.9.0/sknetwork/ranking/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/ranking/tests/test_pagerank.py` & `scikit-network-0.9.0/sknetwork/ranking/tests/test_pagerank.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/__init__.py` & `scikit-network-0.9.0/sknetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """Top-level package for scikit-network"""
 
 __author__ = """scikit-network team"""
 __email__ = "bonald@enst.fr"
-__version__ = '0.8.2'
+__version__ = '0.9.0'
 
 import numpy as np
 
 import warnings
 
 warnings.filterwarnings("default", category=DeprecationWarning)
 try:
```

### Comparing `scikit-network-0.8.2/sknetwork/toy_graphs/block_model.py` & `scikit-network-0.9.0/sknetwork/toy_graphs/block_model.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/toy_graphs/tests/test_block_model.py` & `scikit-network-0.9.0/sknetwork/toy_graphs/tests/test_block_model.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/toy_graphs/tests/test_graph_imports.py` & `scikit-network-0.9.0/sknetwork/toy_graphs/tests/test_graph_imports.py`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/sknetwork/toy_graphs/graph_data.py` & `scikit-network-0.9.0/sknetwork/toy_graphs/graph_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,41 +204,50 @@
     """
     row = np.array([0, 0, 1, 1, 2, 3])
     col = np.array([1, 4, 2, 4, 3, 4])
     adjacency = sparse.csr_matrix((np.ones(len(row), dtype=int), (row, col)), shape=(5, 5))
     return adjacency + adjacency.T
 
 
-def karate_club():
+def karate_club(return_labels: bool = False) -> Union[Tuple[sparse.csr_matrix, np.ndarray], sparse.csr_matrix]:
     """
     Zachary's Karate Club Graph
 
-    Data file from: http://vlado.fmf.uni-lj.si/pub/networks/data/Ucinet/UciData.htm
-
     34 nodes, 78 edges
 
+    Parameters
+    ----------
+    return_labels: bool
+        If True, returns the labels of the nodes.
     Returns
     -------
     adjacency: sparse.csr_matrix
         Adjacency matrix of the graph.
+    labels: np.ndarray
+        Label of each node (community in the karate club).
     """
     row = np.array(
         [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
          1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3,
          3, 4, 4, 5, 5, 5, 6, 8, 8, 8, 9, 13, 14, 14, 15, 15, 18,
          18, 19, 20, 20, 22, 22, 23, 23, 23, 23, 23, 24, 24, 24, 25, 26, 26,
          27, 28, 28, 29, 29, 30, 30, 31, 31, 32])
     col = np.array(
         [1, 2, 3, 4, 5, 6, 7, 8, 10, 11, 12, 13, 17, 19, 21, 31, 2,
          3, 7, 13, 17, 19, 21, 30, 3, 7, 8, 9, 13, 27, 28, 32, 7, 12,
          13, 6, 10, 6, 10, 16, 16, 30, 32, 33, 33, 33, 32, 33, 32, 33, 32,
          33, 33, 32, 33, 32, 33, 25, 27, 29, 32, 33, 25, 27, 31, 31, 29, 33,
          33, 31, 33, 32, 33, 32, 33, 32, 33, 33])
     adjacency = sparse.csr_matrix((np.ones(len(row), dtype=int), (row, col)), shape=(34, 34))
-    return adjacency + adjacency.T
+    if return_labels:
+        labels = np.array([1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 0, 0, 1, 1, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+                           0, 0, 0])
+        return adjacency + adjacency.T, labels
+    else:
+        return adjacency + adjacency.T
 
 
 def rock_paper_scissors():
     """
     A toy directed cycle graph from Rock Paper Scissors victory rule.
 
     3 nodes, 3 edges
@@ -258,52 +267,56 @@
     Bipartite graph connecting some Star Wars villains to the movies in which they appear.
 
     7 nodes (4 villains, 3 movies), 8 edges
 
     Parameters
     ----------
     return_labels: bool
-        Whether to return the labels of the nodes as dictionaries.
+        If True, returns the labels of the nodes as dictionaries.
 
     Returns
     -------
     biadjacency: sparse.csr_matrix
         Biadjacency matrix of the graph.
+    villains: dict
+        Names of villains (rows)
+    movies: dict
+        Names of movies (columns)
     """
     row = np.array([0, 0, 1, 2, 2, 2, 3, 3])
     col = np.array([0, 2, 0, 0, 1, 2, 1, 2])
     biadjacency = sparse.csr_matrix((np.ones(len(row), dtype=int), (row, col)))
 
     if return_labels:
-        row_labels = {0: 'Jabba', 1: 'Greedo', 2: 'Vador', 3: 'Boba'}
-        col_labels = {0: 'A_New_Hope', 1: 'The_Empire_Strikes_Back', 2: 'Return_Of_The_Jedi'}
-        return biadjacency, row_labels, col_labels
+        villains = {0: 'Jabba', 1: 'Greedo', 2: 'Vador', 3: 'Boba'}
+        movies = {0: 'A_New_Hope', 1: 'The_Empire_Strikes_Back', 2: 'Return_Of_The_Jedi'}
+        return biadjacency, villains, movies
     else:
         return biadjacency
 
 
 def movie_actor(return_labels: bool = False) -> Union[Tuple[sparse.csr_matrix, dict, dict], sparse.csr_matrix]:
     """
     Bipartite graph connecting movies to some actors starring in them.
 
     31 nodes (15 movies, 16 actors), 41 edges
 
     Parameters
     ----------
     return_labels: bool
-        Whether to return the labels of the nodes as dictionaries.
+        If True, returns the labels of the nodes as dictionaries.
 
     Returns
     -------
     biadjacency: sparse.csr_matrix
         Biadjacency matrix of the graph.
-    col_labels: dict
-        Labels of rows (movies)
-    col_labels: dict
-        Labels of columns (actors)
+    movies: dict
+        Names of movies (rows)
+    actors: dict
+        Names of actors (columns)
     """
     edges = {
         0: [0, 1, 2],
         1: [1, 2, 3],
         2: [3, 4, 5, 8],
         3: [4, 6],
         4: [0, 6],
@@ -321,15 +334,15 @@
     row, col = [], []
     for key, item in edges.items():
         row += [key] * len(item)
         col += item
     biadjacency = sparse.csr_matrix((np.ones(len(row), dtype=int), (row, col)))
 
     if return_labels:
-        row_labels = {
+        movies = {
             0: 'Inception',
             1: 'The Dark Knight Rises',
             2: 'The Big Short',
             3: 'Drive',
             4: 'The Great Gatsby',
             5: 'La La Land',
             6: 'Crazy Stupid Love',
@@ -338,15 +351,15 @@
             9: 'Aviator',
             10: '007 Spectre',
             11: 'Inglourious Basterds',
             12: 'Midnight In Paris',
             13: 'Murder on the Orient Express',
             14: 'Fantastic Beasts 2'
         }
-        col_labels = {
+        actors = {
             0: 'Leonardo DiCaprio',
             1: 'Marion Cotillard',
             2: 'Joseph Gordon Lewitt',
             3: 'Christian Bale',
             4: 'Ryan Gosling',
             5: 'Brad Pitt',
             6: 'Carey Mulligan',
@@ -356,15 +369,15 @@
             10: 'Ralph Fiennes',
             11: 'Jude Law',
             12: 'Willem Dafoe',
             13: 'Christophe Waltz',
             14: 'Johnny Depp',
             15: 'Owen Wilson'
         }
-        return biadjacency, row_labels, col_labels
+        return biadjacency, movies, actors
     else:
         return biadjacency
 
 
 def painters(return_labels: bool = False) -> Union[sparse.csr_matrix, Tuple[sparse.csr_matrix, dict]]:
     """
     Directed graph of some famous painters with links on Wikipedia.
```

### Comparing `scikit-network-0.8.2/sknetwork/embedding/metrics.py` & `scikit-network-0.9.0/sknetwork/embedding/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 from scipy import sparse
 from scipy.stats import hmean
 from sknetwork.utils.checks import check_format
 from typing import Union
 
 
-def linear_fit(adjacency: Union[sparse.csr_matrix, np.ndarray], embedding: np.ndarray, order: int=1,
-               damping: float=0.85) -> tuple:
+def linear_fit(adjacency: Union[sparse.csr_matrix, np.ndarray], embedding: np.ndarray, order: int = 1,
+               damping: float = 0.85) -> tuple:
     """Linear multi order proximity fit and diversity.
 
     Parameters
     ----------
     adjacency:
         Adjacency matrix of the adjacency.
     embedding:
-        Two dimensional array, line i represents the embedding of node i.
+        Embedding of each node.
     order:
         Number of proximity order to consider.
     damping:
         Decay factor for multi-order metrics, only useful if ``order > 1``.
 
     Returns
     -------
@@ -57,78 +57,78 @@
 
     normalization = np.linalg.norm(embedding) ** 2 / np.sqrt(n_nodes * m_nodes)
     fit /= (total_scale * normalization)
     div /= (total_scale * normalization)
     return fit, div
 
 
-def dot_modularity(adjacency, embedding: np.ndarray, features=None, resolution=1., weights='degree',
-                   return_all: bool=False):
+def dot_modularity(adjacency, embedding: np.ndarray, coembedding=None, resolution=1., weights='degree',
+                   return_all: bool = False):
     """
-    Difference of the weighted average dot product between embeddings of pairs of neighbors in the adjacency
-    (fit term) and pairs of nodes in the adjacency (diversity term).
+    Quality metric of an embedding :math:`x` defined by:
 
     :math:`Q = \\sum_{ij}(\\dfrac{A_{ij}}{w} - \\gamma \\dfrac{d_id_j}{w^2})x_i^Tx_j`
 
-    This metric is normalized to lie between -1 and 1.
-    If the embeddings are normalized, this reduces to the cosine modularity.
+    This metric is normalized to lie between -1 and 1 (for :math:`|||gamma = 1`).
+
+    If the embeddings are normalized, this reduces to cosine modularity.
 
     Parameters
     ----------
     adjacency: sparse.csr_matrix or np.ndarray
-        the adjacency matrix of the adjacency
+        Adjacency matrix of the graph.
     embedding: np.ndarray
-        the embedding to evaluate, embedding[i] must represent the embedding of node i
-    features: None or np.ndarray
-        For biadjacency graphs, features should be the embedding of the second part
+        Embedding of the nodes.
+    coembedding: None or np.ndarray
+        For bipartite graphs, coembedding of features.
     resolution: float
-        scaling for first-order approximation
+        Resolution parameter.
     weights: ``'degree'`` or ``'uniform'``
-        prior distribution on the nodes
-
+        Weights of the nodes.
     return_all: bool, default = ``False``
         whether to return (fit, diversity) or fit - diversity
 
     Returns
     -------
     dot_modularity: a float or a tuple of floats.
     """
     adjacency = check_format(adjacency)
     n_nodes, m_nodes = adjacency.shape
     total_weight: float = adjacency.data.sum()
 
-    if features is None:
+    if coembedding is None:
         if n_nodes != m_nodes:
-            raise ValueError('feature cannot be None for non-square adjacency matrices.')
+            raise ValueError('coembedding cannot be None for non-square adjacency matrices.')
         else:
             normalization = np.linalg.norm(embedding) ** 2 / np.sqrt(n_nodes * m_nodes)
-            features = embedding
+            coembedding = embedding
     else:
-        normalization = np.linalg.norm(embedding.dot(features.T)) / np.sqrt(n_nodes * m_nodes)
+        normalization = np.linalg.norm(embedding.dot(coembedding.T)) / np.sqrt(n_nodes * m_nodes)
 
     if weights == 'degree':
         wou = adjacency.dot(np.ones(m_nodes)) / total_weight
         win = adjacency.T.dot(np.ones(n_nodes)) / total_weight
     elif weights == 'uniform':
         wou = np.ones(n_nodes) / n_nodes
         win = np.ones(m_nodes) / m_nodes
     else:
         raise ValueError('weights must be degree or uniform.')
 
-    fit = (np.multiply(embedding, adjacency.dot(features))).sum() / (total_weight * normalization)
-    diversity = (embedding.T.dot(wou)).dot(features.T.dot(win)) / normalization
+    fit = (np.multiply(embedding, adjacency.dot(coembedding))).sum() / (total_weight * normalization)
+    diversity = (embedding.T.dot(wou)).dot(coembedding.T.dot(win)) / normalization
 
     if return_all:
-        return fit, resolution * diversity
+        return fit, diversity, fit - resolution * diversity
     else:
         return fit - resolution * diversity
 
 
-def hscore(adjacency, embedding: np.ndarray, order='second', return_all: bool=False):
-    """Harmonic mean of fit and diversity with respect to first or second order node similarity.
+def hscore(adjacency, embedding: np.ndarray, order='second', return_all: bool = False):
+    """
+    Harmonic mean of fit and diversity with respect to first or second order node similarity.
 
     Parameters
     ----------
     adjacency: sparse.csr_matrix or np.ndarray
         the adjacency matrix of the adjacency
     embedding: np.ndarray
         the embedding to evaluate, embedding[i] must represent the embedding of node i
@@ -149,24 +149,24 @@
         raise ValueError('For fist order similarity, the adjacency matrix must be square.')
     total_weight = adjacency.data.sum()
     # out-degree vector
     dou = adjacency.dot(np.ones(m_nodes))
     # in-degree vector
     din = adjacency.T.dot(np.ones(n_nodes))
 
-    pdhou, pdhin = np.zeros(n_nodes), np.zeros(m_nodes)
-    pdhou[dou.nonzero()] = 1 / np.sqrt(dou[dou.nonzero()])
-    pdhin[din.nonzero()] = 1 / np.sqrt(din[din.nonzero()])
+    prob_out, prob_in = np.zeros(n_nodes), np.zeros(m_nodes)
+    prob_out[dou.nonzero()] = 1 / np.sqrt(dou[dou.nonzero()])
+    prob_in[din.nonzero()] = 1 / np.sqrt(din[din.nonzero()])
 
     normalization = np.linalg.norm(embedding.T * np.sqrt(dou)) ** 2
     if order == 'first':
         fit = (np.multiply(embedding, adjacency.dot(embedding))).sum()
         fit /= total_weight * (np.linalg.norm(embedding) ** 2 / n_nodes)
     elif order == 'second':
-        fit = np.linalg.norm(adjacency.T.dot(embedding).T * pdhin) ** 2 / normalization
+        fit = np.linalg.norm(adjacency.T.dot(embedding).T * prob_in) ** 2 / normalization
     else:
         raise ValueError('The similarity order should be \'first\' or \'second\'.')
     diversity = (np.linalg.norm(embedding.T.dot(dou))) ** 2 / total_weight
     diversity = 1 - diversity / normalization
 
     if return_all:
         return fit, diversity
```

### Comparing `scikit-network-0.8.2/sknetwork/embedding/spectral.py` & `scikit-network-0.9.0/sknetwork/embedding/spectral.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,63 +9,62 @@
 """
 
 import numpy as np
 from scipy import sparse
 from sknetwork.linalg import safe_sparse_dot, SparseLR, EigSolver, HalkoEig, LanczosEig, auto_solver
 from sknetwork.utils.adjacency_formats import bipartite2undirected
 from sknetwork.utils.algorithm_base_class import Algorithm
-from sknetwork.utils.checks import check_format
-from sknetwork.utils.preprocessing import is_connected
+from sknetwork.utils.checks import check_format, is_symmetric
+from sknetwork.basics.structure import is_connected
 from typing import Union
+import warnings
 
 
 class Spectral(Algorithm):
     """
     Spectral embedding of a graph.
 
     Parameters
     ----------
     embedding_dimension : int, optional
         Dimension of the embedding space
     normalized_laplacian : bool (default = True)
-        whether to use the normalized laplacian, :math:`I - D^{-1/2} A D^{-1/2}`
+        If True, uses the normalized Laplacian, :math:`I - D^{-1/2} A D^{-1/2}`
     regularization : ``None`` or float (default=0.01)
         Implicitly add edges of given weight between all pairs of nodes.
     energy_scaling : bool (default=True)
         If ``True``, rescales each column of the embedding by dividing it by the square-root of the corresponding
         eigenvalue. Only valid if ``node_weights == 'degree'``.
     force_biadjacency : bool (default=False)
-        Only relevant for symmetric inputs. Force the algorithm to treat the adjacency as a biadjacency
-        as it would do for asymmetric inputs.
+        Forces the input matrix to be considered as a biadjacency matrix. Only relevant for a symmetric input matrix.
     solver: 'auto', 'halko', 'lanczos' or EigSolver object
         Which eigenvalue solver to use
 
         * ``'auto'`` calls the auto_solver function
         * ``'halko'``: randomized method, fast but less accurate than 'lanczos' for ill-conditioned matrices
         * ``'lanczos'``: power-iteration based method
         * ``custom``: the user must provide an EigSolver object.
 
     Attributes
     ----------
     embedding_ : array, shape = (n, embedding_dimension)
-        Embedding matrix of the nodes
-    features_ : array, shape = (p, embedding_dimension)
-        Only relevant for asymmetric inputs or if ``force_biadjacency==True``.
+        Embedding of the nodes
+    coembedding_ : array, shape = (p, embedding_dimension)
+        Co-embedding of the feature nodes
+        Only relevant for an asymmetric input matrix or if ``force_biadjacency==True``.
     eigenvalues_ : array, shape = (embedding_dimension)
-        Smallest eigenvalues of the training matrix
+        Smallest eigenvalues
 
     Example
     -------
     >>> from sknetwork.toy_graphs import karate_club
     >>> adjacency = karate_club()
     >>> spectral = Spectral(embedding_dimension=2)
-    >>> spectral.fit(adjacency)
-    Spectral(embedding_dimension=2, normalized_laplacian=True, regularization=0.01, energy_scaling=True,\
- force_biadjacency=False, solver=LanczosEig(which='SM'))
-    >>> spectral.embedding_.shape
+    >>> embedding = spectral.fit(adjacency).embedding_
+    >>> embedding.shape
     (34, 2)
 
     References
     ----------
     Belkin, M. & Niyogi, P. (2003). Laplacian Eigenmaps for Dimensionality Reduction and Data Representation,
     Neural computation.
 
@@ -86,15 +85,15 @@
             self.solver: EigSolver = HalkoEig(which='SM')
         elif solver == 'lanczos':
             self.solver: EigSolver = LanczosEig(which='SM')
         else:
             self.solver = solver
 
         self.embedding_ = None
-        self.features_ = None
+        self.coembedding_ = None
         self.eigenvalues_ = None
 
     def fit(self, adjacency: Union[sparse.csr_matrix, np.ndarray]) -> 'Spectral':
         """Fits the model from data in adjacency_matrix
 
         Parameters
         ----------
@@ -105,54 +104,63 @@
         -------
         self: :class:`Spectral`
         """
 
         adjacency = check_format(adjacency)
         n, p = adjacency.shape
 
+        if p != n or not is_symmetric(adjacency) or self.force_biadjacency:
+            adjacency = bipartite2undirected(adjacency)
+
+        n_ = adjacency.shape[0]
+
         if self.solver == 'auto':
             solver = auto_solver(adjacency.nnz)
             if solver == 'lanczos':
                 self.solver: EigSolver = LanczosEig(which='SM')
             else:
                 self.solver: EigSolver = HalkoEig(which='SM')
 
+        if self.embedding_dimension > n_ - 2:
+            warnings.warn(Warning("The dimension of the embedding must be less than the number of nodes - 1."))
+            n_components = n_ - 2
+        else:
+            n_components = self.embedding_dimension + 1
+
         if self.regularization is None and not is_connected(adjacency):
             if self.energy_scaling:
-                raise ValueError('energy_scaling without low-rank regularization'
-                                 'is not compatible with a disconnected graph.')
+                raise ValueError("The graph is not connected and low-rank regularization is not active."
+                                 "This can cause errors in the computation of the embedding."
+                                 "The parameter energy_scaling must be set to False")
             else:
-                raise Warning("The graph is not connected and low-rank regularization is not active."
-                              "This can cause errors in the computation of the embedding.")
+                warnings.warn(Warning("The graph is not connected and low-rank regularization is not active."
+                                      "This can cause errors in the computation of the embedding."))
+
         if self.regularization:
-            adjacency = SparseLR(adjacency, [(self.regularization * np.ones(n), np.ones(p))])
-        if p != n or self.force_biadjacency:
-            adjacency = bipartite2undirected(adjacency)
+            adjacency = SparseLR(adjacency, [(self.regularization * np.ones(n_), np.ones(n_))])
 
         # builds standard Laplacian
         degrees = adjacency.dot(np.ones(adjacency.shape[1]))
         degree_matrix = sparse.diags(degrees, format='csr')
         laplacian = -(adjacency - degree_matrix)
 
         # applies normalization of the Laplacian
         if self.normalized_laplacian:
-            weight_matrix = sparse.diags(np.sqrt(degrees), format='csr')
-            weight_matrix.data = 1 / weight_matrix.data
-            laplacian = safe_sparse_dot(weight_matrix, safe_sparse_dot(laplacian, weight_matrix))
+            inv_sqrt_degree_matrix = sparse.diags(np.sqrt(degrees), format='csr')
+            inv_sqrt_degree_matrix.data = 1 / inv_sqrt_degree_matrix.data
+            laplacian = safe_sparse_dot(inv_sqrt_degree_matrix, safe_sparse_dot(laplacian, inv_sqrt_degree_matrix))
 
-        # spectral decomposition
-        n_components = min(self.embedding_dimension + 1, min(n, p))
         self.solver.fit(laplacian, n_components)
 
         self.eigenvalues_ = self.solver.eigenvalues_[1:]
         self.embedding_ = self.solver.eigenvectors_[:, 1:]
         if self.normalized_laplacian:
-            self.embedding_ = np.array(weight_matrix.dot(self.embedding_))
+            self.embedding_ = np.array(inv_sqrt_degree_matrix.dot(self.embedding_))
 
         if self.energy_scaling and self.normalized_laplacian:
             self.embedding_ /= np.sqrt(self.eigenvalues_)
 
-        if self.embedding_.shape[0] > n:
-            self.features_ = self.embedding_[n:]
+        if n_ > n:
+            self.coembedding_ = self.embedding_[n:]
             self.embedding_ = self.embedding_[:n]
 
         return self
```

### Comparing `scikit-network-0.8.2/sknetwork/embedding/tests/test_metrics.py` & `scikit-network-0.9.0/sknetwork/embedding/tests/test_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,20 @@
                                                  [1, 0, 1, 0]]))
         self.bipartite = star_wars_villains()
         self.embedding = np.ones((4, 2))
         self.features = np.ones((3, 2))
 
     def test_dot_modularity(self):
         self.assertAlmostEqual(dot_modularity(self.graph, self.embedding), 0.)
-        fit, diversity = dot_modularity(self.graph, self.embedding, return_all=True)
+        fit, diversity, modularity = dot_modularity(self.graph, self.embedding, return_all=True)
         self.assertAlmostEqual(fit, 1.)
         self.assertAlmostEqual(diversity, 1.)
 
         self.assertAlmostEqual(dot_modularity(self.bipartite, self.embedding, self.features), 0.)
-        fit, diversity = dot_modularity(self.bipartite, self.embedding, self.features, return_all=True)
+        fit, diversity, modularity = dot_modularity(self.bipartite, self.embedding, self.features, return_all=True)
         self.assertAlmostEqual(fit, 1.)
         self.assertAlmostEqual(diversity, 1.)
 
     def test_hscore(self):
         self.assertAlmostEqual(hscore(self.graph, self.embedding), 0.)
         fit, diversity = hscore(self.graph, self.embedding, return_all=True)
         self.assertAlmostEqual(fit, 1.)
```

### Comparing `scikit-network-0.8.2/sknetwork/embedding/tests/test_embeddings.py` & `scikit-network-0.9.0/sknetwork/embedding/tests/test_embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """tests for embeddings"""
 
 import unittest
-from sknetwork.embedding import GSVD
+from sknetwork.embedding import SVD
 from sknetwork.embedding import Spectral
 from scipy import sparse
 import numpy as np
 
 
 class TestEmbeddings(unittest.TestCase):
 
@@ -27,21 +27,21 @@
         self.assertTrue(spectral.embedding_.shape == (4, 2))
         self.assertTrue(type(spectral.eigenvalues_) == np.ndarray and len(spectral.eigenvalues_) == 2)
         self.assertTrue(min(spectral.eigenvalues_ >= 0))
         self.assertTrue(max(spectral.eigenvalues_ <= 2))
 
         spectral.fit(self.biadjacency)
         self.assertEqual(spectral.embedding_.shape, (4, 2))
-        self.assertEqual(spectral.features_.shape, (3, 2))
+        self.assertEqual(spectral.coembedding_.shape, (3, 2))
         self.assertTrue(type(spectral.eigenvalues_) == np.ndarray and len(spectral.eigenvalues_) == 2)
 
-    def test_gsvd(self):
-        gsvd = GSVD(2)
-        gsvd.fit(self.adjacency)
-        self.assertTrue(gsvd.embedding_.shape == (4, 2))
-        self.assertTrue(gsvd.features_.shape == (4, 2))
-        self.assertTrue(type(gsvd.singular_values_) == np.ndarray and len(gsvd.singular_values_) == 2)
-
-        gsvd.fit(self.biadjacency)
-        self.assertTrue(gsvd.embedding_.shape == (4, 1))
-        self.assertTrue(gsvd.features_.shape == (3, 1))
-        self.assertTrue(type(gsvd.singular_values_) == np.ndarray and len(gsvd.singular_values_) == 1)
+    def test_svd(self):
+        svd = SVD(2)
+        svd.fit(self.adjacency)
+        self.assertTrue(svd.embedding_.shape == (4, 2))
+        self.assertTrue(svd.coembedding_.shape == (4, 2))
+        self.assertTrue(type(svd.singular_values_) == np.ndarray and len(svd.singular_values_) == 2)
+
+        svd.fit(self.biadjacency)
+        self.assertTrue(svd.embedding_.shape == (4, 1))
+        self.assertTrue(svd.coembedding_.shape == (3, 1))
+        self.assertTrue(type(svd.singular_values_) == np.ndarray and len(svd.singular_values_) == 1)
```

### Comparing `scikit-network-0.8.2/sknetwork/embedding/gsvd.py` & `scikit-network-0.9.0/sknetwork/embedding/svd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu May 31 17:16:22 2018
 @author: Nathan de Lara <ndelara@enst.fr>
+@author: Thomas Bonald <bonald@enst.fr>
 """
 
 import numpy as np
 from scipy import sparse
 from sknetwork.linalg import SparseLR
 from sknetwork.utils.algorithm_base_class import Algorithm
 from sknetwork.utils.checks import check_format, check_weights
 from sknetwork.linalg import SVDSolver, HalkoSVD, LanczosSVD, auto_solver, safe_sparse_dot
 from typing import Union
 
 
-class GSVD(Algorithm):
-    """Generalized Singular Value Decomposition for non-linear dimensionality reduction.
+class SVD(Algorithm):
+    """
+    Graph embedding by Generalized Singular Value Decomposition.
 
     Setting ``weights`` and ``feature_weights`` to ``'uniform'`` leads to the standard SVD.
 
     Parameters
     -----------
     embedding_dimension: int
-        The dimension of the projected subspace.
-    weights: ``'degree'`` or ``'uniform'``
-        Default weighting for the rows.
+        Dimension of the embedding.
+    weights: ``'degree'`` or ``'uniform'`` (default=``'degree'``)
+        Weights of the nodes.
+    feature_weights: ``'degree'`` or ``'uniform'`` (default=``'degree'``)
+        Weights of the feature nodes.
     regularization: ``None`` or float (default=0.01)
         Implicitly add edges of given weight between all pairs of nodes.
     energy_scaling: bool (default=True)
-        If ``True``, rescales each column of the embedding by dividing it by :math:`\\sqrt{1-\\sigma_i^2}`.
+        If ``True``, rescales each dimension of the embedding by the corresponding energy.
         Only valid if ``weights == 'degree'``.
 
     Attributes
     ----------
     embedding_ : np.ndarray, shape = (n_samples, embedding_dimension)
-        Embedding of the samples (rows of the training matrix)
-    features_ : np.ndarray, shape = (n_features, embedding_dimension)
-        Embedding of the features (columns of the training matrix)
+        Embedding of the nodes (rows of the adjacency matrix)
+    coembedding_ : np.ndarray, shape = (n_features, embedding_dimension)
+        Embedding of the feature nodes (columns of the adjacency matrix)
     singular_values_ : np.ndarray, shape = (embedding_dimension)
-        Singular values of the training matrix
+        Generalized singular values of the adjacency matrix
 
     Example
     -------
     >>> from sknetwork.toy_graphs import movie_actor
     >>> adjacency = movie_actor()
-    >>> gsvd = GSVD(embedding_dimension=2)
-    >>> gsvd.fit(adjacency)
-    GSVD(embedding_dimension=2, weights='degree', regularization=0.01, energy_scaling=True, solver=LanczosSVD())
-    >>> gsvd.embedding_.shape
+    >>> svd = SVD(embedding_dimension=2)
+    >>> embedding = svd.fit(adjacency).embedding_
+    >>> embedding.shape
     (15, 2)
 
     References
     ----------
-    * Abdi, H. (2007). Singular value decomposition (SVD) and generalized singular value decomposition.
-      Encyclopedia of measurement and statistics, 907-912.
-      https://www.cs.cornell.edu/cv/ResearchPDF/Generalizing%20The%20Singular%20Value%20Decomposition.pdf
+    Abdi, H. (2007). Singular value decomposition (SVD) and generalized singular value decomposition.
+    Encyclopedia of measurement and statistics, 907-912.
+    https://www.cs.cornell.edu/cv/ResearchPDF/Generalizing%20The%20Singular%20Value%20Decomposition.pdf
     """
 
-    def __init__(self, embedding_dimension=2, weights='degree', regularization: Union[None, float] = 0.01,
-                 energy_scaling: bool = True, solver: Union[str, SVDSolver] = 'auto'):
+    def __init__(self, embedding_dimension=2, weights='degree', feature_weights='degree',
+                 regularization: Union[None, float] = 0.01, energy_scaling: bool = True,
+                 solver: Union[str, SVDSolver] = 'auto'):
         self.embedding_dimension = embedding_dimension
         self.weights = weights
+        self.feature_weights = feature_weights
         self.regularization = regularization
         self.energy_scaling = energy_scaling
         if solver == 'halko':
             self.solver: SVDSolver = HalkoSVD()
         elif solver == 'lanczos':
             self.solver: SVDSolver = LanczosSVD()
         else:
             self.solver = solver
 
         self.embedding_ = None
-        self.features_ = None
+        self.coembedding_ = None
         self.singular_values_ = None
 
-    def fit(self, adjacency: Union[sparse.csr_matrix, np.ndarray]) -> 'GSVD':
-        """Fits the model from data in adjacency_matrix.
+    def fit(self, adjacency: Union[sparse.csr_matrix, np.ndarray]) -> 'SVD':
+        """
+        Computes the generalized SVD of the adjacency matrix.
 
         Parameters
         ----------
         adjacency: array-like, shape = (n, p)
-            Adjacency matrix, where n = p is the number of nodes for a standard directed or undirected adjacency,
-            n, p are the number of nodes in each part for a biadjacency adjacency.
+            Adjacency matrix, where n = p is the number of nodes for a standard directed or undirected graph,
+            n, p are the number of nodes in each part for a bipartite graph.
 
         Returns
         -------
-        self: :class:`GSVD`
+        self: :class:`SVD`
         """
         adjacency = check_format(adjacency)
         n, p = adjacency.shape
 
         if self.solver == 'auto':
             solver = auto_solver(adjacency.nnz)
             if solver == 'lanczos':
@@ -98,36 +104,37 @@
                 self.solver: SVDSolver = HalkoSVD()
 
         if self.regularization:
             adjacency = SparseLR(adjacency, [(self.regularization * np.ones(n), np.ones(p))])
         total_weight = adjacency.dot(np.ones(p)).sum()
 
         w_samp = check_weights(self.weights, adjacency)
-        w_feat = check_weights(self.weights, adjacency.T)
+        w_feat = check_weights(self.feature_weights, adjacency.T)
 
         # pseudo inverse square-root out-degree matrix
         diag_samp = sparse.diags(np.sqrt(w_samp), shape=(n, n), format='csr')
         diag_samp.data = 1 / diag_samp.data
         # pseudo inverse square-root in-degree matrix
         diag_feat = sparse.diags(np.sqrt(w_feat), shape=(p, p), format='csr')
         diag_feat.data = 1 / diag_feat.data
 
         normalized_adj = safe_sparse_dot(diag_samp, safe_sparse_dot(adjacency, diag_feat))
 
         # svd
         n_components = min(self.embedding_dimension + 1, min(n, p) - 1)
         self.solver.fit(normalized_adj, n_components)
 
-        self.singular_values_ = self.solver.singular_values_[1:]
-        self.embedding_ = np.sqrt(total_weight) * diag_samp.dot(self.solver.left_singular_vectors_[:, 1:])
-        self.features_ = np.sqrt(total_weight) * diag_feat.dot(self.solver.right_singular_vectors_[:, 1:])
+        index = np.argsort(-self.solver.singular_values_)
+        self.singular_values_ = self.solver.singular_values_[index[1:]]
+        self.embedding_ = np.sqrt(total_weight) * diag_samp.dot(self.solver.left_singular_vectors_[:, index[1:]])
+        self.coembedding_ = np.sqrt(total_weight) * diag_feat.dot(self.solver.right_singular_vectors_[:, index[1:]])
 
         # rescale to get barycenter property
         self.embedding_ *= self.singular_values_
 
         if self.energy_scaling and self.weights == 'degree':
             energy_levels: np.ndarray = np.sqrt(1 - np.clip(self.singular_values_, 0, 1) ** 2)
             energy_levels[energy_levels > 0] = 1 / energy_levels[energy_levels > 0]
             self.embedding_ *= energy_levels
-            self.features_ *= energy_levels
+            self.coembedding_ *= energy_levels
 
         return self
```

### Comparing `scikit-network-0.8.2/PKG-INFO` & `scikit-network-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-network
-Version: 0.8.2
+Version: 0.9.0
 Summary: Graph algorithms
 Home-page: https://github.com/sknetwork-team/scikit-network
 Author: Scikit-network team
 Author-email: bonald@enst.fr
 License: BSD license
 Description: .. image:: https://perso.telecom-paristech.fr/bonald/logo_sknetwork.png
             :align: right
@@ -44,21 +44,31 @@
         
             $ pip install scikit-network
         
         Import scikit-network in a Python project::
         
             import sknetwork as skn
         
-        See examples in the tutorials.
+        See examples in the tutorials (which can be downloaded here_)
+        
+        .. _here: https://github.com/sknetwork-team/scikit-network/tree/master/docs/tutorials
         
         
         =======
         History
         =======
         
+        0.9.0 (2019-07-24)
+        ------------------
+        
+        * Change parser output
+        * Fix bugs in ranking algorithms (zero-degree nodes)
+        * Add notebooks
+        * Import algorithms from scipy (shortest path, connected components, bfs/dfs)
+        * Change SVD embedding (now in decreasing order of singular values)
         
         0.8.2 (2019-07-19)
         ------------------
         
         * Minor bug
         
         0.8.1 (2019-07-18)
```

### Comparing `scikit-network-0.8.2/scikit_network.egg-info/PKG-INFO` & `scikit-network-0.9.0/scikit_network.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-network
-Version: 0.8.2
+Version: 0.9.0
 Summary: Graph algorithms
 Home-page: https://github.com/sknetwork-team/scikit-network
 Author: Scikit-network team
 Author-email: bonald@enst.fr
 License: BSD license
 Description: .. image:: https://perso.telecom-paristech.fr/bonald/logo_sknetwork.png
             :align: right
@@ -44,21 +44,31 @@
         
             $ pip install scikit-network
         
         Import scikit-network in a Python project::
         
             import sknetwork as skn
         
-        See examples in the tutorials.
+        See examples in the tutorials (which can be downloaded here_)
+        
+        .. _here: https://github.com/sknetwork-team/scikit-network/tree/master/docs/tutorials
         
         
         =======
         History
         =======
         
+        0.9.0 (2019-07-24)
+        ------------------
+        
+        * Change parser output
+        * Fix bugs in ranking algorithms (zero-degree nodes)
+        * Add notebooks
+        * Import algorithms from scipy (shortest path, connected components, bfs/dfs)
+        * Change SVD embedding (now in decreasing order of singular values)
         
         0.8.2 (2019-07-19)
         ------------------
         
         * Minor bug
         
         0.8.1 (2019-07-18)
```

### Comparing `scikit-network-0.8.2/scikit_network.egg-info/SOURCES.txt` & `scikit-network-0.9.0/scikit_network.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,66 +12,75 @@
 docs/contributing.rst
 docs/genindex.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
+docs/reference/basics.rst
 docs/reference/clustering.rst
 docs/reference/embedding.rst
 docs/reference/hierarchy.rst
 docs/reference/index.rst
 docs/reference/introduction.rst
 docs/reference/linalg.rst
 docs/reference/loader.rst
 docs/reference/ranking.rst
 docs/reference/toy_graphs.rst
 docs/reference/utils.rst
 docs/tutorials/clustering/index.rst
+docs/tutorials/embedding/index.rst
 docs/tutorials/hierarchy/index.rst
+docs/tutorials/loader/index.rst
 docs/tutorials/ranking/index.rst
 scikit_network.egg-info/PKG-INFO
 scikit_network.egg-info/SOURCES.txt
 scikit_network.egg-info/dependency_links.txt
 scikit_network.egg-info/entry_points.txt
 scikit_network.egg-info/not-zip-safe
 scikit_network.egg-info/requires.txt
 scikit_network.egg-info/top_level.txt
 sknetwork/__init__.py
 sknetwork/cli.py
 sknetwork/sknetwork.py
+sknetwork/basics/__init__.py
+sknetwork/basics/search.py
+sknetwork/basics/shortest_path.py
+sknetwork/basics/structure.py
+sknetwork/basics/tests/__init__.py
+sknetwork/basics/tests/test_structure.py
 sknetwork/clustering/__init__.py
 sknetwork/clustering/bilouvain.py
 sknetwork/clustering/louvain.py
 sknetwork/clustering/metrics.py
 sknetwork/clustering/postprocessing.py
 sknetwork/clustering/tests/__init__.py
 sknetwork/clustering/tests/test_bilouvain.py
 sknetwork/clustering/tests/test_louvain.py
 sknetwork/clustering/tests/test_metrics.py
 sknetwork/embedding/__init__.py
-sknetwork/embedding/gsvd.py
 sknetwork/embedding/metrics.py
 sknetwork/embedding/spectral.py
+sknetwork/embedding/svd.py
 sknetwork/embedding/tests/__init__.py
 sknetwork/embedding/tests/test_embeddings.py
 sknetwork/embedding/tests/test_metrics.py
 sknetwork/hierarchy/__init__.py
 sknetwork/hierarchy/cuts.py
 sknetwork/hierarchy/metrics.py
 sknetwork/hierarchy/paris.py
 sknetwork/hierarchy/tests/__init__.py
 sknetwork/hierarchy/tests/test_metrics.py
 sknetwork/hierarchy/tests/test_paris.py
 sknetwork/linalg/__init__.py
 sknetwork/linalg/auto_mode.py
-sknetwork/linalg/eig.py
 sknetwork/linalg/randomized_matrix_factorization.py
 sknetwork/linalg/sparse_lowrank.py
-sknetwork/linalg/svd.py
+sknetwork/linalg/spectral_solver.py
+sknetwork/linalg/svd_solver.py
 sknetwork/linalg/tests/__init__.py
 sknetwork/linalg/tests/test_eig.py
 sknetwork/linalg/tests/test_randomized_matrix_factorization.py
 sknetwork/linalg/tests/test_sparse_lowrank.py
 sknetwork/linalg/tests/test_svd.py
 sknetwork/loader/__init__.py
 sknetwork/loader/parser.py
@@ -90,15 +99,13 @@
 sknetwork/toy_graphs/tests/test_block_model.py
 sknetwork/toy_graphs/tests/test_graph_imports.py
 sknetwork/utils/__init__.py
 sknetwork/utils/adjacency_formats.py
 sknetwork/utils/algorithm_base_class.py
 sknetwork/utils/checks.py
 sknetwork/utils/lazy_property.py
-sknetwork/utils/preprocessing.py
 sknetwork/utils/projection_simplex.py
 sknetwork/utils/tests/__init__.py
 sknetwork/utils/tests/test_algorithm_base_class.py
 sknetwork/utils/tests/test_formats.py
-sknetwork/utils/tests/test_preprocessing.py
 sknetwork/utils/tests/test_projection_simplex.py
 tests/test_sknetwork.py
```

### Comparing `scikit-network-0.8.2/HISTORY.rst` & `scikit-network-0.9.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+0.9.0 (2019-07-24)
+------------------
+
+* Change parser output
+* Fix bugs in ranking algorithms (zero-degree nodes)
+* Add notebooks
+* Import algorithms from scipy (shortest path, connected components, bfs/dfs)
+* Change SVD embedding (now in decreasing order of singular values)
 
 0.8.2 (2019-07-19)
 ------------------
 
 * Minor bug
 
 0.8.1 (2019-07-18)
```

### Comparing `scikit-network-0.8.2/LICENSE` & `scikit-network-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-network-0.8.2/README.rst` & `scikit-network-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -36,8 +36,10 @@
 
     $ pip install scikit-network
 
 Import scikit-network in a Python project::
 
     import sknetwork as skn
 
-See examples in the tutorials.
+See examples in the tutorials (which can be downloaded here_)
+
+.. _here: https://github.com/sknetwork-team/scikit-network/tree/master/docs/tutorials
```

### Comparing `scikit-network-0.8.2/setup.py` & `scikit-network-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     name='scikit-network',
     # packages=find_packages(include=['sknetwork']),
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/sknetwork-team/scikit-network',
-    version='0.8.2',
+    version='0.9.0',
     zip_safe=False,
 )
```

### Comparing `scikit-network-0.8.2/tests/test_sknetwork.py` & `scikit-network-0.9.0/tests/test_sknetwork.py`

 * *Files identical despite different names*

