# Comparing `tmp/scimap-1.3.9.tar.gz` & `tmp/scimap-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.3.9.tar", max compression
+gzip compressed data, was "scimap-2.0.0.tar", max compression
```

## Comparing `scimap-1.3.9.tar` & `scimap-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
--rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.774355 scimap-1.3.9/LICENSE
--rw-r--r--   0        0        0     2241 2024-02-29 16:07:24.111652 scimap-1.3.9/README.md
--rw-r--r--   0        0        0     2350 2024-03-18 15:08:44.927142 scimap-1.3.9/pyproject.toml
--rw-r--r--   0        0        0      360 2024-03-13 21:02:44.000000 scimap-1.3.9/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.3.9/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.3.9/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.3.9/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.3.9/scimap/cli/test.py
--rw-r--r--   0        0        0      250 2024-03-02 02:38:53.261836 scimap-1.3.9/scimap/helpers/__init__.py
--rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.000000 scimap-1.3.9/scimap/helpers/addROI_omero.py
--rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.615795 scimap-1.3.9/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.511793 scimap-1.3.9/scimap/helpers/animate.py
--rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.029603 scimap-1.3.9/scimap/helpers/classify.py
--rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.533825 scimap-1.3.9/scimap/helpers/dropFeatures.py
--rw-r--r--   0        0        0     4964 2024-03-01 21:09:54.510700 scimap-1.3.9/scimap/helpers/merge_adata_obs.py
--rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.298072 scimap-1.3.9/scimap/helpers/rename.py
--rw-r--r--   0        0        0     5797 2024-03-01 20:47:13.143655 scimap-1.3.9/scimap/helpers/scimap_to_csv.py
--rw-r--r--   0        0        0      701 2024-03-18 15:05:03.967181 scimap-1.3.9/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16723 2024-03-01 21:09:36.040886 scimap-1.3.9/scimap/plotting/addROI_image.py
--rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.790600 scimap-1.3.9/scimap/plotting/cluster_plots.py
--rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.580935 scimap-1.3.9/scimap/plotting/densityPlot2D.py
--rw-r--r--   0        0        0     8704 2024-03-02 01:56:15.194790 scimap-1.3.9/scimap/plotting/distPlot.py
--rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.870855 scimap-1.3.9/scimap/plotting/foldchange.py
--rw-r--r--   0        0        0    11059 2024-03-02 02:00:19.435779 scimap-1.3.9/scimap/plotting/gate_finder.py
--rw-r--r--   0        0        0    11027 2024-03-18 15:02:51.834247 scimap-1.3.9/scimap/plotting/groupCorrelation.py
--rw-r--r--   0        0        0    18085 2024-03-18 13:53:02.003996 scimap-1.3.9/scimap/plotting/heatmap.py
--rw-r--r--   0        0        0     9423 2024-03-02 02:00:12.303252 scimap-1.3.9/scimap/plotting/image_viewer.py
--rw-r--r--   0        0        0    10237 2024-03-18 15:00:19.955016 scimap-1.3.9/scimap/plotting/markerCorrelation.py
--rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.476562 scimap-1.3.9/scimap/plotting/pie.py
--rw-r--r--   0        0        0    10135 2024-03-02 01:59:05.715760 scimap-1.3.9/scimap/plotting/spatial_distance.py
--rw-r--r--   0        0        0    11732 2024-03-02 01:58:57.524269 scimap-1.3.9/scimap/plotting/spatial_interaction.py
--rw-r--r--   0        0        0     4276 2024-03-02 01:58:48.312234 scimap-1.3.9/scimap/plotting/spatial_pscore.py
--rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.182943 scimap-1.3.9/scimap/plotting/spatial_scatterPlot.py
--rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.424269 scimap-1.3.9/scimap/plotting/stacked_barplot.py
--rw-r--r--   0        0        0    12373 2024-03-02 01:58:21.440795 scimap-1.3.9/scimap/plotting/umap.py
--rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.302280 scimap-1.3.9/scimap/plotting/voronoi.py
--rw-r--r--   0        0        0      129 2024-03-17 18:13:28.725249 scimap-1.3.9/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.817117 scimap-1.3.9/scimap/preprocessing/combat.py
--rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.795915 scimap-1.3.9/scimap/preprocessing/log1p.py
--rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.000000 scimap-1.3.9/scimap/preprocessing/mcmicro_to_scimap.py
--rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.438422 scimap-1.3.9/scimap/preprocessing/ngraph.py
--rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.005842 scimap-1.3.9/scimap/preprocessing/rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.3.9/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.3.9/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.3.9/scimap/tests/_data/phenotype_workflow.csv
--rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.375137 scimap-1.3.9/scimap/tests/test_helpers.py
--rw-r--r--   0        0        0      982 2024-03-02 02:50:46.201820 scimap-1.3.9/scimap/tests/test_preprocessing.py
--rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.903918 scimap-1.3.9/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      568 2024-03-02 02:44:25.945510 scimap-1.3.9/scimap/tools/__init__.py
--rw-r--r--   0        0        0    20189 2024-03-17 19:37:21.220626 scimap-1.3.9/scimap/tools/cluster.py
--rw-r--r--   0        0        0     9980 2024-03-01 13:48:18.792276 scimap-1.3.9/scimap/tools/foldchange.py
--rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.563795 scimap-1.3.9/scimap/tools/phenotype_cells.py
--rw-r--r--   0        0        0    11937 2024-03-01 18:54:08.761602 scimap-1.3.9/scimap/tools/spatial_aggregate.py
--rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.502620 scimap-1.3.9/scimap/tools/spatial_cluster.py
--rw-r--r--   0        0        0     9097 2024-03-01 14:14:37.725516 scimap-1.3.9/scimap/tools/spatial_count.py
--rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.522643 scimap-1.3.9/scimap/tools/spatial_distance.py
--rw-r--r--   0        0        0    13734 2024-03-01 18:57:08.104861 scimap-1.3.9/scimap/tools/spatial_expression.py
--rw-r--r--   0        0        0    12014 2024-03-01 16:14:00.048376 scimap-1.3.9/scimap/tools/spatial_interaction.py
--rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.631718 scimap-1.3.9/scimap/tools/spatial_lda.py
--rw-r--r--   0        0        0    12420 2024-03-01 19:01:05.807122 scimap-1.3.9/scimap/tools/spatial_pscore.py
--rw-r--r--   0        0        0    18433 2024-03-01 19:15:01.285753 scimap-1.3.9/scimap/tools/spatial_similarity_search.py
--rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.518742 scimap-1.3.9/scimap/tools/umap.py
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 scimap-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.774355 scimap-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2351 2024-03-20 21:01:04.568387 scimap-2.0.0/README.md
+-rw-r--r--   0        0        0     2366 2024-04-02 01:05:06.978461 scimap-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      391 2024-04-01 23:22:15.513728 scimap-2.0.0/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-2.0.0/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-2.0.0/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-2.0.0/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-2.0.0/scimap/cli/test.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:21:46.158522 scimap-2.0.0/scimap/external/__init__.py
+-rw-r--r--   0        0        0      297 2024-03-20 19:13:27.572207 scimap-2.0.0/scimap/helpers/__init__.py
+-rw-r--r--   0        0        0     7715 2024-03-20 20:49:48.491605 scimap-2.0.0/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.000000 scimap-2.0.0/scimap/helpers/addROI_omero.py
+-rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.615795 scimap-2.0.0/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.511793 scimap-2.0.0/scimap/helpers/animate.py
+-rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.029603 scimap-2.0.0/scimap/helpers/classify.py
+-rw-r--r--   0        0        0     1897 2024-03-20 19:41:09.893157 scimap-2.0.0/scimap/helpers/downloadDemoData.py
+-rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.533825 scimap-2.0.0/scimap/helpers/dropFeatures.py
+-rw-r--r--   0        0        0     4944 2024-03-20 13:25:21.701481 scimap-2.0.0/scimap/helpers/merge_adata_obs.py
+-rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.298072 scimap-2.0.0/scimap/helpers/rename.py
+-rw-r--r--   0        0        0     6194 2024-03-20 01:42:22.133668 scimap-2.0.0/scimap/helpers/scimap_to_csv.py
+-rw-r--r--   0        0        0      766 2024-03-19 18:17:18.230168 scimap-2.0.0/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16939 2024-03-18 19:56:58.653382 scimap-2.0.0/scimap/plotting/addROI_image.py
+-rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.790600 scimap-2.0.0/scimap/plotting/cluster_plots.py
+-rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.580935 scimap-2.0.0/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     8772 2024-03-20 13:51:51.354626 scimap-2.0.0/scimap/plotting/distPlot.py
+-rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.870855 scimap-2.0.0/scimap/plotting/foldchange.py
+-rw-r--r--   0        0        0    11059 2024-03-02 02:00:19.435779 scimap-2.0.0/scimap/plotting/gate_finder.py
+-rw-r--r--   0        0        0    11207 2024-03-18 18:24:57.598183 scimap-2.0.0/scimap/plotting/groupCorrelation.py
+-rw-r--r--   0        0        0    18210 2024-03-18 18:41:06.721737 scimap-2.0.0/scimap/plotting/heatmap.py
+-rw-r--r--   0        0        0     9423 2024-03-02 02:00:12.303252 scimap-2.0.0/scimap/plotting/image_viewer.py
+-rw-r--r--   0        0        0    10417 2024-03-18 18:24:52.838506 scimap-2.0.0/scimap/plotting/markerCorrelation.py
+-rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.476562 scimap-2.0.0/scimap/plotting/pie.py
+-rw-r--r--   0        0        0    12242 2024-03-19 18:32:03.627202 scimap-2.0.0/scimap/plotting/spatialInteractionNetwork.py
+-rw-r--r--   0        0        0    10165 2024-03-19 01:23:30.046016 scimap-2.0.0/scimap/plotting/spatial_distance.py
+-rw-r--r--   0        0        0    11795 2024-03-19 12:21:07.752382 scimap-2.0.0/scimap/plotting/spatial_interaction.py
+-rw-r--r--   0        0        0     5060 2024-03-19 19:10:54.724495 scimap-2.0.0/scimap/plotting/spatial_pscore.py
+-rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.182943 scimap-2.0.0/scimap/plotting/spatial_scatterPlot.py
+-rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.424269 scimap-2.0.0/scimap/plotting/stacked_barplot.py
+-rw-r--r--   0        0        0    12547 2024-03-18 18:34:47.607355 scimap-2.0.0/scimap/plotting/umap.py
+-rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.302280 scimap-2.0.0/scimap/plotting/voronoi.py
+-rw-r--r--   0        0        0      129 2024-03-17 18:13:28.725249 scimap-2.0.0/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.817117 scimap-2.0.0/scimap/preprocessing/combat.py
+-rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.795915 scimap-2.0.0/scimap/preprocessing/log1p.py
+-rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.000000 scimap-2.0.0/scimap/preprocessing/mcmicro_to_scimap.py
+-rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.438422 scimap-2.0.0/scimap/preprocessing/ngraph.py
+-rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.005842 scimap-2.0.0/scimap/preprocessing/rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-2.0.0/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-2.0.0/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-2.0.0/scimap/tests/_data/phenotype_workflow.csv
+-rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.375137 scimap-2.0.0/scimap/tests/test_helpers.py
+-rw-r--r--   0        0        0      982 2024-03-02 02:50:46.201820 scimap-2.0.0/scimap/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.903918 scimap-2.0.0/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      568 2024-03-02 02:44:25.945510 scimap-2.0.0/scimap/tools/__init__.py
+-rw-r--r--   0        0        0    20200 2024-03-19 23:48:54.910997 scimap-2.0.0/scimap/tools/cluster.py
+-rw-r--r--   0        0        0    10598 2024-03-18 21:08:47.269456 scimap-2.0.0/scimap/tools/foldchange.py
+-rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.563795 scimap-2.0.0/scimap/tools/phenotype_cells.py
+-rw-r--r--   0        0        0    12714 2024-03-19 20:32:33.950090 scimap-2.0.0/scimap/tools/spatial_aggregate.py
+-rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.502620 scimap-2.0.0/scimap/tools/spatial_cluster.py
+-rw-r--r--   0        0        0     9097 2024-03-19 23:43:08.527959 scimap-2.0.0/scimap/tools/spatial_count.py
+-rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.522643 scimap-2.0.0/scimap/tools/spatial_distance.py
+-rw-r--r--   0        0        0    13752 2024-03-20 01:28:34.142208 scimap-2.0.0/scimap/tools/spatial_expression.py
+-rw-r--r--   0        0        0    12059 2024-03-19 12:11:34.371207 scimap-2.0.0/scimap/tools/spatial_interaction.py
+-rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.631718 scimap-2.0.0/scimap/tools/spatial_lda.py
+-rw-r--r--   0        0        0    12452 2024-03-19 18:49:22.715271 scimap-2.0.0/scimap/tools/spatial_pscore.py
+-rw-r--r--   0        0        0    18461 2024-03-19 21:36:08.728628 scimap-2.0.0/scimap/tools/spatial_similarity_search.py
+-rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.518742 scimap-2.0.0/scimap/tools/umap.py
+-rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 scimap-2.0.0/PKG-INFO
```

### Comparing `scimap-1.3.9/LICENSE` & `scimap-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/README.md` & `scimap-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 <br>
 
 [![build: Unix-Mac-Win](https://github.com/ajitjohnson/scimap/actions/workflows/build-unix-mac-win.yml/badge.svg)](https://github.com/ajitjohnson/scimap/actions/workflows/build-unix-mac-win.yml)
 [![Docs](https://github.com/ajitjohnson/scimap/actions/workflows/docs.yml/badge.svg)](https://github.com/ajitjohnson/scimap/actions/workflows/docs.yml)
 [![Downloads](https://pepy.tech/badge/scimap)](https://pepy.tech/project/scimap)
 [![PyPI Version](https://img.shields.io/pypi/v/scimap.svg)](https://pypi.org/project/scimap)
 [![PyPI License](https://img.shields.io/pypi/l/scimap.svg)](https://pypi.org/project/scimap)
-[![Gitter chat](https://badges.gitter.im/scimap_io/community.png)](https://gitter.im/scimap_io/community)
 [![DOI](https://zenodo.org/badge/271099296.svg)](https://zenodo.org/badge/latestdoi/271099296)
 
 <br>
 
 <img src="./docs/assets/scimap_logo.jpg" style="max-width:700px;width:100%" >
 
 <br> 
@@ -39,15 +38,20 @@
 $ python
 >>> import scimap as sm
 ```
 
 
 ## Get Started
 
-
 #### Detailed documentation of `scimap` functions and tutorials are available [here](http://scimap.xyz/).
 
-*SCIMAP* development is led by [Ajit Johnson Nirmal](https://ajitjohnson.com/) at the Laboratory of Systems Pharmacology, Harvard Medical School.
+*SCIMAP* development was led by [Ajit Johnson Nirmal](https://ajitjohnson.com/), Harvard Medical School.  
+Check out other tools from the [Nirmal Lab](https://nirmallab.com/tools/). 
+
+
+## Contibute
+Interested in contributing to the package? Check out our guidelines at [https://scimap.xyz/contribute/](https://scimap.xyz/contribute/) for detailed instructions.
+
 
 ## Funding
-This work is supported by the following NIH grant K99-CA256497
+This work was supported by the following NIH grant K99-CA256497
```

### Comparing `scimap-1.3.9/pyproject.toml` & `scimap-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "SCIMAP"
-version = "1.3.9"
+version = "2.0.0"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -49,20 +49,21 @@
 shapely = "^2.0.2"
 gensim = "^4.3.2"
 mkdocs-material = "^9.4.8"
 napari-ome-zarr = "^0.4.0"
 llvmlite = "^0.41.1"
 combat = "^0.3.3"
 mpl-scatter-density = "^0.7"
+pyqt6 = "^6.6.1"
 
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
-black = "19.10b0"
+black = "24.3.0"
 isort = "4.3.21"
 
 # Linters
 mypy = "^1.7.0"
 pydocstyle = "^6.3.0"
 pylint = "^3.0.2"
```

### Comparing `scimap-1.3.9/scimap/cli/_scimap_mcmicro.py` & `scimap-2.0.0/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/cli/test.py` & `scimap-2.0.0/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/addROI_omero.py` & `scimap-2.0.0/scimap/helpers/addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/add_roi_scatter.py` & `scimap-2.0.0/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/animate.py` & `scimap-2.0.0/scimap/helpers/animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/classify.py` & `scimap-2.0.0/scimap/helpers/classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/dropFeatures.py` & `scimap-2.0.0/scimap/helpers/dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/merge_adata_obs.py` & `scimap-2.0.0/scimap/helpers/merge_adata_obs.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def merge_adata_obs (adata, 
                      output_dir=None,
                      verbose=True):
     
     
     """
 Parameters:
-        adata_list (list of anndata.AnnData or list of str):  
+        adata (list of anndata.AnnData or list of str):  
             A list containing AnnData objects to be merged or paths to AnnData files. 
             Each item in the list should either be an AnnData object already loaded into memory 
             or a string representing the path to an AnnData file.
 
         output_dir (str, optional):  
             The directory where the merged AnnData object should be saved. 
             If specified, the merged object is saved to this directory as 'merged_adata.h5ad'.
@@ -63,21 +63,21 @@
         adata (anndata.AnnData):  
             A single AnnData object resulting from the merger of input AnnData objects or files.
 
 Example:
         ```python
         
         # Example 1: Merge AnnData objects already loaded in memory
-        combined_adata = sm.hl.merge_adata_obs(adata_list=[adata1, adata2])
+        combined_adata = sm.hl.merge_adata_obs(adata=[adata1, adata2])
     
         # Example 2: Merge AnnData objects from file paths
-        combined_adata = sm.hl.merge_adata_obs(adata_list=['./data/adata1.h5ad', './data/adata2.h5ad'])
+        combined_adata = sm.hl.merge_adata_obs(adata=['./data/adata1.h5ad', './data/adata2.h5ad'])
     
         # Example 3: Merge AnnData objects and save the combined object to a specified directory
-        combined_adata = sm.hl.merge_adata_obs(adata_list=[adata1, adata2], output_dir='./merged_data')
+        combined_adata = sm.hl.merge_adata_obs(adata=[adata1, adata2], output_dir='./merged_data')
         
         ```
     """
     
     #adata = ["/Users/aj/Downloads/mcmicro_output.h5ad", "/Users/aj/Downloads/mcmicro_output_1.h5ad"]
```

### Comparing `scimap-1.3.9/scimap/helpers/rename.py` & `scimap-2.0.0/scimap/helpers/rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/helpers/scimap_to_csv.py` & `scimap-2.0.0/scimap/helpers/scimap_to_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         description='Helper function that allows users to save the contents of the `scimap` object as a csv file.'
     )
     parser.add_argument(
         '--adata', required=True, 
         help='AnnData object loaded into memory or path to AnnData object.'
     )
     parser.add_argument(
-        '--data_type', type=str, required=False, default='raw',
+        '--layer', type=str, required=False, default='raw',
         help='Three options are available: 1) `raw` - The raw data will be returned; 2) `log` - The raw data converted to log scale using `np.log1p` will be returned; 3) `scaled` - If you have scaled the data using the `sm.pp.rescale`, that will be returned. Please note, if you have not scaled the data, whatever is within `adata.X` will be returned'
     )
     parser.add_argument(
         '--output_dir', type=str, required=False, default=None,
         help='Path to output directory.'
     )
     parser.add_argument(
@@ -49,30 +49,29 @@
     args = parser.parse_args(argv[1:])
     print(vars(args))
     scimap_to_csv(**vars(args))
     
 
 # Function
 def scimap_to_csv (adata, 
-                   data_type='raw', 
+                   layer='raw', 
                    output_dir=None, 
                    file_name=None, 
                    CellID='CellID',
                    verbose=True):
     """
 Parameters:
         adata (anndata.AnnData):  
             The annotated data matrix to export.
 
-        data_type (str, optional):  
-            Specifies the type of data to export. Options include:
+        layer (str, optional):  
+            Specifies the layer to export:
             - 'raw': Exports the raw data.
             - 'log': Exports the data after applying a log transformation with `np.log1p`.
-            - 'scaled': Exports the data if it has been scaled using `sm.pp.rescale`. 
-              If not scaled, the contents of `adata.X` are exported. 
+            - 'None': Exports the data  in `adata.X`
         
         output_dir (str, optional):  
             The directory where the CSV file will be saved. If not specified, the file is saved in the current working directory.
 
         file_name (str, optional):  
             The name of the output CSV file. If not provided, a default name `scimap_to_csv_file.csv` is used.
 
@@ -86,21 +85,21 @@
         DataFrame (csv):  
             The function does not return a value but saves the specified data to a CSV file in the designated directory.
 
 Example:
     ```python
         
         # Export raw data to CSV
-        sm.hl.scimap_to_csv(adata, data_type='raw', output_dir='/path/to/save', file_name='raw_data.csv')
+        sm.hl.scimap_to_csv(adata, layer='raw', output_dir='/path/to/save', file_name='raw_data.csv')
     
         # Export log-transformed data to CSV, with a custom CellID column name
-        sm.hl.scimap_to_csv(adata, data_type='log', output_dir='/path/to/save', file_name='log_data.csv', CellID='UniqueCellID')
+        sm.hl.scimap_to_csv(adata, layer='log', output_dir='/path/to/save', file_name='log_data.csv', CellID='UniqueCellID')
     
         # Export scaled data to Cobject
-        data = sm.hl.scimap_to_csv(adata, data_type='scaled')
+        data = sm.hl.scimap_to_csv(adata, layer='scaled')
         
     ```
     """
     
     # Load the andata object    
     if isinstance(adata, str):
         if file_name is None:
@@ -111,21 +110,33 @@
     else:
         if file_name is None:
             imid = "scimap_to_csv_file.csv"
         else: 
             imid = str(file_name)
         adata = adata
     
+    
     # Expression matrix
-    if data_type == 'raw':
+    if layer == 'raw':
         data = pd.DataFrame(adata.raw.X, index=adata.obs.index, columns=adata.var.index)
-    if data_type == 'log':
-        data = pd.DataFrame(np.log1p(adata.raw.X), index=adata.obs.index, columns=adata.var.index)
-    if data_type == 'scaled':
+    elif layer is None:
         data = pd.DataFrame(adata.X, index=adata.obs.index, columns=adata.var.index)
+    else:
+        data = pd.DataFrame(adata.layers[layer], index=adata.obs.index, columns=adata.var.index)
+        
+        
+# =============================================================================
+#     # Expression matrix
+#     if data_type == 'raw':
+#         data = pd.DataFrame(adata.raw.X, index=adata.obs.index, columns=adata.var.index)
+#     if data_type == 'log':
+#         data = pd.DataFrame(np.log1p(adata.raw.X), index=adata.obs.index, columns=adata.var.index)
+#     if data_type == 'scaled':
+#         data = pd.DataFrame(adata.X, index=adata.obs.index, columns=adata.var.index)
+# =============================================================================
     
     # Metadata
     meta = pd.DataFrame(adata.obs)
     
     # Merge the two dataframes
     merged = pd.concat([data, meta], axis=1, sort=False)
```

### Comparing `scimap-1.3.9/scimap/plotting/__init__.py` & `scimap-2.0.0/scimap/plotting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from .addROI_image import addROI_image
 from .umap import umap
 from .densityPlot2D import densityPlot2D
 from .distPlot import distPlot
 from .spatial_scatterPlot import spatial_scatterPlot
 from .heatmap import heatmap
 from .markerCorrelation import markerCorrelation
-from .groupCorrelation import groupCorrelation
+from .groupCorrelation import groupCorrelation
+from .spatialInteractionNetwork import spatialInteractionNetwork
```

### Comparing `scimap-1.3.9/scimap/plotting/addROI_image.py` & `scimap-2.0.0/scimap/plotting/addROI_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,17 +371,19 @@
             all_rois['id'] = range(all_rois.shape[0])
             all_rois.index = all_rois['id']
             
         # Find cells within ROI and add it to the dataframe
         def add_roi_internal (roi_id):
             roi_mpatch = all_rois[all_rois['id'] == roi_id]['mpatch'][roi_id]
             inside = sub_data[roi_mpatch.contains_points(sub_data[[x_coordinate, y_coordinate]])]
-            inside['ROI_internal'] = all_rois[all_rois['id'] == roi_id]['ROI'][roi_id]
+            inside_copy = inside.copy()
+            inside_copy['ROI_internal'] = all_rois.loc[all_rois['id'] == roi_id, 'ROI'][roi_id]
+            #inside['ROI_internal'] = all_rois[all_rois['id'] == roi_id]['ROI'][roi_id]
             # return
-            return inside
+            return inside_copy
         
         print("Identifying cells within selected ROI's")
         # all ROI cells
         roi_list = all_rois['id'].unique()
         #final_roi = list()
         #for i in roi_list: 
         #    roi_mpatch = all_rois[all_rois['id'] == i]['mpatch'][i]
@@ -415,14 +417,16 @@
                 combined_roi['ROI_internal'] = combined_roi['ROI_internal'].fillna('Other')     
         else:
             # if label is not present just create a new one
             combined_roi = result.copy()
             combined_roi['ROI_internal'] = combined_roi['ROI_internal'].fillna('Other')     
         
         # Add to adata
-        adata.obs[label] = combined_roi['ROI_internal']    
+        adata.obs[label] = combined_roi['ROI_internal']   
+        
+        print("ROIs saved under adata.obs['" + str(label) + "']")
         
         # return
         return adata
```

### Comparing `scimap-1.3.9/scimap/plotting/cluster_plots.py` & `scimap-2.0.0/scimap/plotting/cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/densityPlot2D.py` & `scimap-2.0.0/scimap/plotting/densityPlot2D.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/distPlot.py` & `scimap-2.0.0/scimap/plotting/distPlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     The `sm.pl.distPlot` function is used to create distribution plots of 
     marker intensity data.
 
 ## Function
 """
 
 import pandas as pd
+import numpy as np
 import math
 import matplotlib.pyplot as plt
 import itertools
 import pathlib
 import matplotlib as mpl
 mpl.rcParams['pdf.fonttype'] = 42
 
@@ -190,23 +191,24 @@
             # Define a color cycle of 10 colors
             color_cycle = itertools.cycle(plt.rcParams['axes.prop_cycle'].by_key()['color'])
             # Assign a different color to each column
             color = {col: next(color_cycle) for col in data.columns}
                 
         # Set the size of the figure
         fig, axes = plt.subplots(nrows=num_rows, ncols=num_cols, figsize=figsize, dpi=dpi)
+        axes = np.atleast_2d(axes)
         # Set the spacing between subplots
         #fig.subplots_adjust(bottom=0.1, hspace=0.1)
 
         # Loop through each column in the DataFrame and plot a KDE with the
         # user-defined color or the default color (grey) in the corresponding subplot
         for i, column in enumerate(data.columns):
             c = color.get(column, 'grey')
             row_idx = i // num_cols
-            col_idx = i % num_cols
+            col_idx = i % num_cols            
             data[column].plot.kde(ax=axes[row_idx, col_idx], label=column, color=c)
             axes[row_idx, col_idx].set_title(column)
             axes[row_idx, col_idx].tick_params(axis='both', which='major', width=1, labelsize=fontsize)
             axes[row_idx, col_idx].set_ylabel('')
             
             if vline == 'auto':
                 axes[row_idx, col_idx].axvline((data[column].max() + data[column].min()) / 2, color='black')
```

### Comparing `scimap-1.3.9/scimap/plotting/foldchange.py` & `scimap-2.0.0/scimap/plotting/foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/gate_finder.py` & `scimap-2.0.0/scimap/plotting/gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/groupCorrelation.py` & `scimap-2.0.0/scimap/plotting/groupCorrelation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 from scipy.cluster.hierarchy import linkage, dendrogram
 import os
 import anndata as ad
 import warnings
 from scipy.stats import zscore
 import argparse
 
+
+plt.rcParams['figure.dpi'] = 100
+plt.rcParams['savefig.dpi']=300
+plt.rcParams['font.family']='sans serif'
+plt.rcParams['font.sans-serif']='Arial'
+plt.rcParams['pdf.fonttype']=42
+
 # function
 def groupCorrelation(adata, 
                      groupBy, 
                      condition,
                      normalize=False,
                      subsetGroups=None, 
                      orderRow=None,
```

### Comparing `scimap-1.3.9/scimap/plotting/heatmap.py` & `scimap-2.0.0/scimap/plotting/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 import os
 from matplotlib.colors import Normalize
 import pandas as pd
 import anndata as ad
 import argparse
 
 
+plt.rcParams['figure.dpi'] = 100
+plt.rcParams['savefig.dpi']=300
+plt.rcParams['font.family']='sans serif'
+plt.rcParams['font.sans-serif']='Arial'
+plt.rcParams['pdf.fonttype']=42
+
+
 # function
 def heatmap (adata,
              groupBy,
              layer=None,
              subsetMarkers=None,
              subsetGroups=None,
              clusterRows=True,
@@ -295,15 +302,14 @@
         # Move the colorbar to the top left corner
         cbar_ax = fig.add_axes([0.125, 0.92, 0.2, 0.02]) # x, y, width, height
         cbar = plt.colorbar(c, cax=cbar_ax, orientation='horizontal')
         cbar_ax.xaxis.set_ticks_position('top')
         cbar_ax.xaxis.set_label_position('top')
         cbar.set_label('Mean expression in group')
         
-        ax.set_title('Heatmap of Marker Values by Category')
         ax.set_xlabel('Markers')
         ax.set_ylabel('Categories')
         
         plt.tight_layout(rect=[0, 0, 0.9, 0.9]) # Adjust the layout
         
         # Saving the figure if saveDir and fileName are provided
         if saveDir and fileName:
```

### Comparing `scimap-1.3.9/scimap/plotting/image_viewer.py` & `scimap-2.0.0/scimap/plotting/image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/markerCorrelation.py` & `scimap-2.0.0/scimap/plotting/markerCorrelation.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 from scipy.spatial.distance import pdist
 from scipy.cluster.hierarchy import linkage, dendrogram
 import os
 import anndata as ad
 import warnings
 import argparse
 
+
+plt.rcParams['figure.dpi'] = 100
+plt.rcParams['savefig.dpi']=300
+plt.rcParams['font.family']='sans serif'
+plt.rcParams['font.sans-serif']='Arial'
+plt.rcParams['pdf.fonttype']=42
+
 def markerCorrelation (adata, 
                        layer='log', 
                        subsetMarkers=None, 
                        orderRow=None, 
                        orderColumn=None, 
                        clusterRows=True, 
                        clusterColumns=True,
```

### Comparing `scimap-1.3.9/scimap/plotting/pie.py` & `scimap-2.0.0/scimap/plotting/pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/spatial_distance.py` & `scimap-2.0.0/scimap/plotting/spatial_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,26 @@
 
     # Method
     if method=='heatmap':
         if heatmap_summarize is True:
             # create the necessary data
             data = pd.DataFrame({'phenotype': adata.obs[phenotype]})
             data = pd.merge(data, diatance_map, how='outer',left_index=True, right_index=True) # merge with the distance map
-            k = data.groupby(['phenotype']).mean() # collapse the whole dataset into mean expression
+            k = data.groupby(['phenotype'],observed=False).mean() # collapse the whole dataset into mean expression
             d = k[k.index]
         else:
             # create new naming scheme for the phenotypes
             non_summary = pd.DataFrame({'imageid': adata.obs[imageid], 'phenotype': adata.obs[phenotype]})
             non_summary['imageid'] = non_summary['imageid'].astype(str) # convert the column to string
             non_summary['phenotype'] = non_summary['phenotype'].astype(str) # convert the column to string
             non_summary['image_phenotype'] = non_summary['imageid'].str.cat(non_summary['phenotype'],sep="_")
             # Merge distance map with phenotype
             data = pd.DataFrame(non_summary[['image_phenotype']])
             data = pd.merge(data, diatance_map, how='outer',left_index=True, right_index=True)
-            k = data.groupby(['image_phenotype']).mean()
+            k = data.groupby(['image_phenotype'],observed=False).mean()
             d = k.sort_index(axis=1)
         # Generate the heatmap
         mask = d.isnull() # identify the NAN's for masking 
         d = d.fillna(0) # replace nan's with 0 so that clustering will work
         # Heatmap
         sns.clustermap(d, cmap=heatmap_cmap, row_cluster=heatmap_row_cluster,
                        col_cluster=heatmap_col_cluster, mask=mask,
```

### Comparing `scimap-1.3.9/scimap/plotting/spatial_interaction.py` & `scimap-2.0.0/scimap/plotting/spatial_interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,16 @@
                         cmap='seismic', binary_view=True, row_cluster=True, col_cluster=False, 
                         figsize=(10, 8), dendrogram_ratio=(.1, .2), cbar_pos=(0, .2, .03, .4))
     ```
     """
     
     # set color for heatmap
     #cmap_updated = copy.copy(matplotlib.cm.get_cmap(cmap))
-    cmap_updated = matplotlib.cm.get_cmap(cmap)
+    #cmap_updated = matplotlib.cm.get_cmap(cmap)
+    cmap_updated = matplotlib.colormaps[cmap]
     cmap_updated.set_bad(color=nonsig_color)
     
 
     # Copy the interaction results from anndata object
     try:
         interaction_map = adata.uns[spatial_interaction].copy()
     except KeyError:
@@ -157,15 +158,15 @@
             interaction_map = interaction_map.reindex(columns=subset_neighbour_phenotype)
             p_val_df = p_val_df.reindex(columns=subset_neighbour_phenotype)
         
         # Plotting heatmap
         mask = p_val_df.isnull() # identify the NAN's for masking 
         im = interaction_map.fillna(0) # replace nan's with 0 so that clustering will work
         # heatmap
-        sns.clustermap(im, cmap=cmap, row_cluster=row_cluster, col_cluster=col_cluster,  mask=mask, **kwargs)
+        sns.clustermap(im, cmap=cmap_updated, row_cluster=row_cluster, col_cluster=col_cluster,  mask=mask, **kwargs)
         
     else:
         if len(interaction_map.columns) < 2:
             raise ValueError('Data for only a single image is available please set summarize_plot=True and try again')
         # convert first two columns to multi-index column
         #interaction_map = interaction_map.set_index(['phenotype','neighbour_phenotype'])
         #p_val_df = p_val_df.set_index(['phenotype','neighbour_phenotype'])
@@ -209,15 +210,15 @@
         # Plotting heatmap
         mask = p_val_df.isnull() # identify the NAN's for masking 
         im = interaction_map.fillna(0) # replace nan's with 0 so that clustering will work
         mask.columns = im.columns
                 
         # covert the first two columns into index
         # Plot
-        sns.clustermap(im, cmap=cmap, row_cluster=row_cluster, col_cluster=col_cluster, mask=mask, **kwargs)
+        sns.clustermap(im, cmap=cmap_updated, row_cluster=row_cluster, col_cluster=col_cluster, mask=mask, **kwargs)
     
     if return_data is True:
         # perpare data for export
         map_data = interaction_map.copy()
         p_val_data = mask.copy()
         map_data.reset_index(inplace=True)
         p_val_data.reset_index(inplace=True)
```

### Comparing `scimap-1.3.9/scimap/plotting/spatial_pscore.py` & `scimap-2.0.0/scimap/plotting/spatial_pscore.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 ## Function
 """
 
 # Library
 import seaborn as sns; sns.set_theme(style='white', color_codes=True)
 import matplotlib.pyplot as plt
 
-import matplotlib as mpl
-mpl.rcParams['pdf.fonttype'] = 42
+plt.rcParams['figure.dpi'] = 100
+plt.rcParams['savefig.dpi']=300
+plt.rcParams['font.family']='sans serif'
+plt.rcParams['font.sans-serif']='Arial'
+plt.rcParams['pdf.fonttype']=42
 
 # Function
 def spatial_pscore (adata, 
                     label='spatial_pscore', 
                     plot_score='both', 
                     order_xaxis = None,
-                    color='grey', **kwargs):
+                    color='grey',
+                    figsize=None,
+                    **kwargs):
     """
 Parameters:
         adata (anndata.AnnData):  
             The annotated data matrix with spatial proximity scores.
 
         label (str, optional):  
             The label/key used to access the spatial proximity scores stored in `adata.uns`. 
@@ -83,24 +88,36 @@
         
 
     # Generate the x and y axis
     x  = data.index
     y_pd = data['Proximity Density'].values
     y_pv = data['Proximity Volume'].values
     
+    if figsize is None:
+        # Dynamically calculate figsize based on the data size
+        figsize_width_scale = 1.0  # Adjust based on your preference and the expected data length
+        figsize_height_scale = 0.5  # Adjust this to change how tall the plots are
+        # For 'both', we might want a wider figure
+        figsize_width = max(12, len(x) * figsize_width_scale)
+        figsize_height = max(8, len(x) * figsize_height_scale)
+        figsize = (figsize_width, figsize_height)
+        
     # Plot what user requests
     if plot_score == 'Proximity Density':
+        plt.figure(figsize=figsize)
         ax = sns.barplot(x=x, y=y_pd, color=color, **kwargs).set_title('Proximity Density')
         ax = plt.xticks(rotation=90)
         plt.tight_layout()
     if plot_score == 'Proximity Volume':
+        plt.figure(figsize=figsize)
         ax = sns.barplot(x=x, y=y_pv, color=color, **kwargs).set_title('Proximity Volume')
         ax = plt.xticks(rotation=90)
         plt.tight_layout()
     if plot_score == 'both':
+        plt.figure(figsize=figsize)
         fig, ax = plt.subplots(1,2)
         sns.barplot(x=x, y=y_pd, color=color, ax=ax[0], **kwargs).set_title('Proximity Density')
         ax[0].tick_params(axis='x', rotation=90)
         sns.barplot(x=x, y=y_pv, color=color, ax=ax[1], **kwargs).set_title('Proximity Volume')
         ax[1].tick_params(axis='x', rotation=90)
         plt.tight_layout()
         fig.show()
```

### Comparing `scimap-1.3.9/scimap/plotting/spatial_scatterPlot.py` & `scimap-2.0.0/scimap/plotting/spatial_scatterPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/stacked_barplot.py` & `scimap-2.0.0/scimap/plotting/stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/plotting/umap.py` & `scimap-2.0.0/scimap/plotting/umap.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,24 @@
 import pandas as pd
 import math
 import itertools
 import matplotlib.colors as colors
 import seaborn as sns
 import matplotlib.patches as mpatches
 
-import matplotlib as mpl
-mpl.rcParams['pdf.fonttype'] = 42
+plt.rcParams['figure.dpi'] = 100
+plt.rcParams['savefig.dpi']=300
+plt.rcParams['font.family']='sans serif'
+plt.rcParams['font.sans-serif']='Arial'
+plt.rcParams['pdf.fonttype']=42
 
 # function
 def umap (adata, 
           color=None, 
-          use_layer=None, 
+          layer=None, 
           use_raw=False, 
           log=False, 
           label='umap',
           cmap='vlag', 
           palette=None, 
           alpha=0.8, 
           figsize=(5, 5), 
@@ -53,15 +56,15 @@
         adata (anndata.AnnData):  
             The annotated data matrix.
 
         color (list, optional):  
             List of keys from `adata.obs.columns` or `adata.var.index` to color the plot. 
             Allows multiple keys for facetted plotting.
 
-        use_layer (str, optional):  
+        layer (str, optional):  
             Specifies the AnnData layer to use for UMAP calculations. Defaults to using `adata.X`.
 
         use_raw (bool, optional):  
             If True, uses `adata.raw.X` for coloring the plot, useful for visualizing gene expression on UMAP.
 
         log (bool, optional):  
             Applies log transformation (`np.log1p`) to the data before plotting. Useful for gene expression data.
@@ -134,22 +137,24 @@
         # identify if all elemets of color are available        
         if set(color).issubset(list(adata.var.index) + list(adata.obs.columns)) is False:
             raise ValueError("Element passed to `color` is not found in adata, please check!")
         
         # organise the data
         if any(item in color for item in list(adata.obs.columns)):
             adataobs = adata.obs.loc[:, adata.obs.columns.isin(color)]
+            adataobs = adataobs.apply(lambda x: x.astype('category'))
+
         else:
             adataobs = None
             
         if any(item in color for item in list(adata.var.index)):
             # find the index of the marker
             marker_index = np.where(np.isin(list(adata.var.index), color))[0]
-            if use_layer is not None:
-                adatavar = adata.layers[use_layer][:, np.r_[marker_index]]
+            if layer is not None:
+                adatavar = adata.layers[layer][:, np.r_[marker_index]]
             elif use_raw is True:
                 adatavar = adata.raw.X[:, np.r_[marker_index]]
             else:
                 adatavar = adata.X[:, np.r_[marker_index]]
             adatavar = pd.DataFrame(adatavar, index=adata.obs.index, columns = list(adata.var.index[marker_index]))
         else:
             adatavar = None
```

### Comparing `scimap-1.3.9/scimap/plotting/voronoi.py` & `scimap-2.0.0/scimap/plotting/voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/preprocessing/combat.py` & `scimap-2.0.0/scimap/preprocessing/combat.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/preprocessing/log1p.py` & `scimap-2.0.0/scimap/preprocessing/log1p.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/preprocessing/mcmicro_to_scimap.py` & `scimap-2.0.0/scimap/preprocessing/mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/preprocessing/ngraph.py` & `scimap-2.0.0/scimap/preprocessing/ngraph.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/preprocessing/rescale.py` & `scimap-2.0.0/scimap/preprocessing/rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/_data/example_data.csv` & `scimap-2.0.0/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/_data/example_data.h5ad` & `scimap-2.0.0/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/_data/phenotype_workflow.csv` & `scimap-2.0.0/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/test_helpers.py` & `scimap-2.0.0/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/test_preprocessing.py` & `scimap-2.0.0/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tests/test_tools.py` & `scimap-2.0.0/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/__init__.py` & `scimap-2.0.0/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/cluster.py` & `scimap-2.0.0/scimap/tools/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if pheno is not None:
             if verbose:
                 print('Kmeans clustering ' + str(pheno))
         else:
             if verbose:
                 print('Kmeans clustering')
         
-        kmeans = KMeans(n_clusters=k, random_state=random_state).fit(data_subset)
+        kmeans = KMeans(n_clusters=k, random_state=random_state, n_init=10).fit(data_subset)
         
         # Rename the labels
         cluster_labels = list(map(str,kmeans.labels_))
         if pheno is not None:
             cluster_labels = list(map(lambda orig_string: pheno + '-' + orig_string, cluster_labels))
                 
         # Make it into a
```

### Comparing `scimap-1.3.9/scimap/tools/foldchange.py` & `scimap-2.0.0/scimap/tools/foldchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,29 +98,38 @@
             subset_phenotype = [subset_phenotype]
         data = data[data[phenotype].isin(subset_phenotype)]
     
     # subset data    
     from_data = data[data[imageid].isin(from_group)]
     if len(from_group) > 1:
         combined_name = '_'.join(from_group)
-        from_data[imageid] = combined_name
-    from_data[imageid] = from_data[imageid].astype('str').astype('category')
-    from_data[phenotype] = from_data[phenotype].astype('str').astype('category')
+        #from_data[imageid] = combined_name
+        from_data.loc[:, imageid] = combined_name
+
+    #from_data[imageid] = from_data[imageid].astype('str').astype('category')
+    #from_data[phenotype] = from_data[phenotype].astype('str').astype('category')
+    from_data.loc[:, imageid] = from_data[imageid].astype('str').astype('category')
+    from_data.loc[:, phenotype] = from_data[phenotype].astype('str').astype('category')
     if to_group is None:
         to_data = data[~data[imageid].isin(from_group)]
     else:
         to_data = data[data[imageid].isin(to_group)]
-    to_data[imageid] = to_data[imageid].astype('str').astype('category')
-    to_data[phenotype] = to_data[phenotype].astype('str').astype('category')
+    to_data.loc[:, imageid] = to_data[imageid].astype('str').astype('category')
+    to_data.loc[:, phenotype] = to_data[phenotype].astype('str').astype('category')
+    #to_data[imageid] = to_data[imageid].astype('str').astype('category')
+    #to_data[phenotype] = to_data[phenotype].astype('str').astype('category')
+    
+    if verbose:
+        print('calculating foldchange')
     
     # consolidated counts dataframe
-    from_data_consolidated = pd.DataFrame(from_data.groupby([imageid,phenotype]).size()).unstack().fillna(0)
+    from_data_consolidated = pd.DataFrame(from_data.groupby([imageid,phenotype],observed=False).size()).unstack().fillna(0)
     from_data_consolidated.columns = np.unique(from_data_consolidated.columns.get_level_values(1))
     
-    to_data_consolidated = pd.DataFrame(to_data.groupby([imageid,phenotype]).size()).unstack().fillna(0)
+    to_data_consolidated = pd.DataFrame(to_data.groupby([imageid,phenotype],observed=False).size()).unstack().fillna(0)
     to_data_consolidated.columns = np.unique(to_data_consolidated.columns.get_level_values(1))
     
     # make backup of the sample names
     from_b = list(from_data_consolidated.index)
     to_b = list(to_data_consolidated.index)
     
     # make sure from_data_consolidated and to_data_consolidated has the same columns
@@ -139,18 +148,21 @@
     to_data_total = abs(to_data_consolidated.sub( to_data_consolidated.sum(axis=1), axis=0))
     
     # 
     if verbose:
         print('calculating P values')
     p_vals = []
     for i in from_data_consolidated.columns:
-        a = from_data_consolidated[i][0]
-        c = from_data_total[i][0]
+        #a = from_data_consolidated[i][0]
+        a = from_data_consolidated[i].iloc[0]
+        #c = from_data_total[i][0]
+        c = from_data_total[i].iloc[0]
         for j in to_data_consolidated.index:
-            b = to_data_consolidated[i][j]
+            #b = to_data_consolidated[i][j]
+            b = to_data_consolidated[i].loc[j]
             d = to_data_total[i][j]
             oddsratio, pvalue = stats.fisher_exact([[a, b], [c, d]])
             p_vals.append(pvalue)
     
     # replace 0 with a small number (1 cell) to avoind inf
     from_data_consolidated_zero = from_data_consolidated.replace(0, 1, inplace=False)
     to_data_consolidated_zero = to_data_consolidated.replace(0, 1, inplace=False)
```

### Comparing `scimap-1.3.9/scimap/tools/phenotype_cells.py` & `scimap-2.0.0/scimap/tools/phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/spatial_aggregate.py` & `scimap-2.0.0/scimap/tools/spatial_aggregate.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,15 +194,34 @@
         #def col_name_mapper (row_data, purity):
         #    p = row_data[row_data >= purity/100]
         #    #phenotype_name = 'non-significant' if len(p.index) == 0 else p.index[0]
         #    phenotype_name = 'non-significant' if len(p.index) == 0 else p.idxmax()
         #    return phenotype_name
         # Apply the iteration function
         #aggregate_pheno = pd.DataFrame(k.apply(lambda x: col_name_mapper(row_data=x,purity=purity), axis=1))
-        aggregate_pheno = pd.DataFrame(k[k>=purity/100].idxmax(axis=1).fillna('non-significant'))
+
+
+        # Within the spatial_aggregate_internal function
+        # Create an empty DataFrame to hold the results
+        aggregate_pheno = pd.DataFrame(index=k.index, columns=[0])
+        
+        # Iterate over rows in DataFrame k
+        for idx, row in k.iterrows():
+            filtered_row = row[row >= purity / 100]  # Apply purity threshold
+            if not filtered_row.empty:  # Check if the filtered row is not empty
+                # If not empty, find the index of the maximum value
+                max_idx = filtered_row.idxmax()
+            else:
+                # If empty, set to 'non-significant'
+                max_idx = 'non-significant'
+            # Store the result
+            aggregate_pheno.at[idx, 0] = max_idx
+        
+        
+        #aggregate_pheno = pd.DataFrame(k[k>=purity/100].idxmax(axis=1).fillna('non-significant'))
         aggregate_pheno.columns = ['spatial_aggregate']
         
         # Return 
         return aggregate_pheno
     
 
     # Subset a particular image if needed
@@ -228,16 +247,16 @@
     # Merge all the results into a single dataframe    
     result = []
     for i in range(len(all_data)):
         result.append(all_data[i])
     result = pd.concat(result, join='outer')  
     
     # Reindex the cells
-    result = result.fillna(0)
     result = result.reindex(adata.obs.index)
+    result = result.fillna('non-significant')
     
     # Add to adata
     adata.obs[label] = result
     
     # Return        
     return adata
```

### Comparing `scimap-1.3.9/scimap/tools/spatial_cluster.py` & `scimap-2.0.0/scimap/tools/spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/spatial_count.py` & `scimap-2.0.0/scimap/tools/spatial_count.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     # Merge all the results into a single dataframe    
     result = []
     for i in range(len(all_data)):
         result.append(all_data[i])
     result = pd.concat(result, join='outer')  
     
     # Reindex the cells
-    result = result.fillna(0)
     result = result.reindex(adata.obs.index)
+    result = result.fillna(0)
     
     # Add to adata
     adata.uns[label] = result
     
     # Return        
     return adata
```

### Comparing `scimap-1.3.9/scimap/tools/spatial_distance.py` & `scimap-2.0.0/scimap/tools/spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/spatial_expression.py` & `scimap-2.0.0/scimap/tools/spatial_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,25 +161,25 @@
         adata (anndata.AnnData):  
             The input `adata` object, updated with the spatial expression results in `adata.uns[label]`.
 
 Example:
         ```python
         
         # Calculate spatial expression using a 30-pixel radius
-        adata = spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
+        adata = sm.tl.spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
                                    method='radius', radius=30, 
                                    label='expression_radius_30')
     
         # Calculate spatial expression using 10 nearest neighbors
-        adata = spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
+        adata = sm.tl.spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
                                    method='knn', knn=10, use_raw=True,
                                    label='expression_knn_10')
     
         # Analyze spatial expression within a specific image using radius method
-        adata = spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
+        adata = sm.tl.spatial_expression(adata, x_coordinate='X_centroid', y_coordinate='Y_centroid',
                                    method='radius', radius=50, imageid='imageid', subset='specific_image',
                                    label='expression_specific_image')
         
         ```
     """
     
     # Load the andata object
```

### Comparing `scimap-1.3.9/scimap/tools/spatial_interaction.py` & `scimap-2.0.0/scimap/tools/spatial_interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,28 +176,28 @@
         # Permutation
         if verbose:
             print('Performing '+ str(permutation) + ' permutations')
     
         def permutation_pval (data):
             data = data.assign(neighbour_phenotype=np.random.permutation(data['neighbour_phenotype']))
             #data['neighbour_phenotype'] = np.random.permutation(data['neighbour_phenotype'])
-            data_freq = data.groupby(['phenotype','neighbour_phenotype']).size().unstack()
+            data_freq = data.groupby(['phenotype','neighbour_phenotype'],observed=False).size().unstack()
             data_freq = data_freq.fillna(0).stack().values 
             return data_freq
         
         # Apply function
         final_scores = Parallel(n_jobs=-1)(delayed(permutation_pval)(data=n) for i in range(permutation)) 
         perm = pd.DataFrame(final_scores).T
         
         # Consolidate the permutation results
         if verbose:
             print('Consolidating the permutation results')
         # Calculate P value
         # real
-        n_freq = n.groupby(['phenotype','neighbour_phenotype']).size().unstack().fillna(0).stack() 
+        n_freq = n.groupby(['phenotype','neighbour_phenotype'],observed=False).size().unstack().fillna(0).stack() 
         # permutation
         mean = perm.mean(axis=1)
         std = perm.std(axis=1)
         # P-value calculation
         if pval_method == 'abs':
             # real value - prem value / no of perm 
             p_values = abs(n_freq.values - mean) / (permutation+1)
@@ -208,15 +208,15 @@
             p_values = scipy.stats.norm.sf(abs(z_scores))*2
             p_values = p_values[~np.isnan(p_values)]
             
         # Compute Direction of interaction (interaction or avoidance)
         direction = ((n_freq.values - mean) / abs(n_freq.values - mean)).fillna(1)
 
         # Normalize based on total cell count
-        k = n.groupby(['phenotype','neighbour_phenotype']).size().unstack().fillna(0)
+        k = n.groupby(['phenotype','neighbour_phenotype'],observed=False).size().unstack().fillna(0)
         # add neighbour phenotype that are not present to make k a square matrix
         columns_to_add = dict.fromkeys(np.setdiff1d(k.index,k.columns), 0)
         k = k.assign(**columns_to_add)
 
         total_cell_count = data['phenotype'].value_counts()
         total_cell_count = total_cell_count[k.columns].values # keep only cell types that are present in the column of k
         # total_cell_count = total_cell_count.reindex(k.columns).values # replaced by above
```

### Comparing `scimap-1.3.9/scimap/tools/spatial_lda.py` & `scimap-2.0.0/scimap/tools/spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/scimap/tools/spatial_pscore.py` & `scimap-2.0.0/scimap/tools/spatial_pscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,25 +236,25 @@
     wh_d[label] = np.where(wh_d.index.isin(proximity_neigh), '_'.join(proximity), "other")
     
     # Define a scoring system
     name = '_'.join(proximity)
     whole_data = wh_d[[score_by, label, phenotype]]
     
     # proximity volume
-    p_v = whole_data.groupby([score_by, label]).size().unstack().fillna(0)
+    p_v = whole_data.groupby([score_by, label], observed=False).size().unstack().fillna(0)
     p_v ['All Cells'] = p_v[name] + p_v["other"]
     p_v['Proximity Volume'] = p_v[name] / p_v['All Cells']
     p_v = p_v.fillna(0) # replace NA
     p_v = p_v.replace([np.inf, -np.inf], 0)
     p_v = p_v.drop(columns = 'other')
     
     # subset the phenotypes of interest
     w_d = whole_data[whole_data[phenotype].isin(proximity)]
     # proximity density
-    p_d = w_d.groupby([score_by, label]).size().unstack().fillna(0)
+    p_d = w_d.groupby([score_by, label], observed=False).size().unstack().fillna(0)
     p_d ['Celltype of interest'] = p_d[name] + p_d["other"]
     p_d['Proximity Density'] = p_d[name] / p_d['Celltype of interest']
     p_d = p_d.fillna(0) # replace NA
     p_d = p_d.replace([np.inf, -np.inf], 0)
     p_d = p_d.drop(columns = ['other', name])
     
     # Merge Promimity volumne and density
```

### Comparing `scimap-1.3.9/scimap/tools/spatial_similarity_search.py` & `scimap-2.0.0/scimap/tools/spatial_similarity_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,18 +184,18 @@
 
         # b) Local radius method
         if method == 'radius':
             if verbose:
                 print("Identifying neighbours within " + str(radius) + " pixels of every cell")
             if z_coordinate is not None:
                 kdt = BallTree(data, metric='euclidean') 
-                ind = kdt.query_radius(data, r=radius, return_distance=True)
+                dist, ind = kdt.query_radius(data, r=radius, return_distance=True)
             else:
                 kdt = BallTree(data, metric='euclidean') 
-                ind = kdt.query_radius(data, r=radius, return_distance=True)
+                dist, ind = kdt.query_radius(data, r=radius, return_distance=True)
 
 # =============================================================================
 #         
 #         if method == 'knn':
 #             print("Identifying the " + str(knn) + " nearest neighbours for every cell")
 #             tree = BallTree(data, leaf_size= 2)
 #             dist, ind = tree.query(data, k=knn, return_distance= True)
@@ -337,15 +337,15 @@
         
     #result = spatial_lag
     #np.max(all_roi_scores)
     #np.min(all_roi_scores)
     
     # for each ROI calculate the median spatial lag
     median_spatial_lag = pd.merge(result.loc[query_neigh.index], query_neigh, left_index=True, right_index=True, how='outer')
-    median_spatial_lag = median_spatial_lag.groupby(ROI_column).median()
+    median_spatial_lag = median_spatial_lag.groupby(ROI_column, observed=False).median()
         
     # apply the distance function to each defined ROI's
     spatial_lag_array = np.array(result)
     median_spatial_lag_array = np.array(median_spatial_lag)
     
     # func
     #all_roi_scores = np.array([distance.euclidean(median_spatial_lag_array[0],x) for x in spatial_lag_array])
```

### Comparing `scimap-1.3.9/scimap/tools/umap.py` & `scimap-2.0.0/scimap/tools/umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.3.9/PKG-INFO` & `scimap-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.3.9
+Version: 2.0.0
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -29,14 +29,15 @@
 Requires-Dist: mpl-scatter-density (>=0.7,<0.8)
 Requires-Dist: napari (>=0.4.18,<0.5.0)
 Requires-Dist: napari-ome-zarr (>=0.4.0,<0.5.0)
 Requires-Dist: numba (>=0.58.1)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
+Requires-Dist: pyqt6 (>=6.6.1,<7.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pytest-xvfb (>=3.0.0,<4.0.0)
 Requires-Dist: scanpy (>=1.9.6,<2.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: shapely (>=2.0.2,<3.0.0)
 Requires-Dist: tifffile (>=2023.9.26,<2024.0.0)
@@ -49,15 +50,14 @@
 <br>
 
 [![build: Unix-Mac-Win](https://github.com/ajitjohnson/scimap/actions/workflows/build-unix-mac-win.yml/badge.svg)](https://github.com/ajitjohnson/scimap/actions/workflows/build-unix-mac-win.yml)
 [![Docs](https://github.com/ajitjohnson/scimap/actions/workflows/docs.yml/badge.svg)](https://github.com/ajitjohnson/scimap/actions/workflows/docs.yml)
 [![Downloads](https://pepy.tech/badge/scimap)](https://pepy.tech/project/scimap)
 [![PyPI Version](https://img.shields.io/pypi/v/scimap.svg)](https://pypi.org/project/scimap)
 [![PyPI License](https://img.shields.io/pypi/l/scimap.svg)](https://pypi.org/project/scimap)
-[![Gitter chat](https://badges.gitter.im/scimap_io/community.png)](https://gitter.im/scimap_io/community)
 [![DOI](https://zenodo.org/badge/271099296.svg)](https://zenodo.org/badge/latestdoi/271099296)
 
 <br>
 
 <img src="./docs/assets/scimap_logo.jpg" style="max-width:700px;width:100%" >
 
 <br> 
@@ -86,16 +86,21 @@
 $ python
 >>> import scimap as sm
 ```
 
 
 ## Get Started
 
-
 #### Detailed documentation of `scimap` functions and tutorials are available [here](http://scimap.xyz/).
 
-*SCIMAP* development is led by [Ajit Johnson Nirmal](https://ajitjohnson.com/) at the Laboratory of Systems Pharmacology, Harvard Medical School.
+*SCIMAP* development was led by [Ajit Johnson Nirmal](https://ajitjohnson.com/), Harvard Medical School.  
+Check out other tools from the [Nirmal Lab](https://nirmallab.com/tools/). 
+
+
+## Contibute
+Interested in contributing to the package? Check out our guidelines at [https://scimap.xyz/contribute/](https://scimap.xyz/contribute/) for detailed instructions.
+
 
 ## Funding
-This work is supported by the following NIH grant K99-CA256497
+This work was supported by the following NIH grant K99-CA256497
```

