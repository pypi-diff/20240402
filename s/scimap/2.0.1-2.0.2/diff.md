# Comparing `tmp/scimap-2.0.1.tar.gz` & `tmp/scimap-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-2.0.1.tar", max compression
+gzip compressed data, was "scimap-2.0.2.tar", max compression
```

## Comparing `scimap-2.0.1.tar` & `scimap-2.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.774355 scimap-2.0.1/LICENSE
--rw-r--r--   0        0        0     2718 2024-04-02 17:08:14.223496 scimap-2.0.1/README.md
--rw-r--r--   0        0        0     2522 2024-04-02 17:01:35.106945 scimap-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      391 2024-04-01 23:22:15.513728 scimap-2.0.1/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-2.0.1/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-2.0.1/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-2.0.1/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-2.0.1/scimap/cli/test.py
--rw-r--r--   0        0        0        0 2024-04-01 23:21:46.158522 scimap-2.0.1/scimap/external/__init__.py
--rw-r--r--   0        0        0      297 2024-03-20 19:13:27.572207 scimap-2.0.1/scimap/helpers/__init__.py
--rw-r--r--   0        0        0     7715 2024-03-20 20:49:48.491605 scimap-2.0.1/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.000000 scimap-2.0.1/scimap/helpers/addROI_omero.py
--rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.615795 scimap-2.0.1/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.511793 scimap-2.0.1/scimap/helpers/animate.py
--rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.029603 scimap-2.0.1/scimap/helpers/classify.py
--rw-r--r--   0        0        0     1897 2024-03-20 19:41:09.893157 scimap-2.0.1/scimap/helpers/downloadDemoData.py
--rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.533825 scimap-2.0.1/scimap/helpers/dropFeatures.py
--rw-r--r--   0        0        0     4944 2024-03-20 13:25:21.701481 scimap-2.0.1/scimap/helpers/merge_adata_obs.py
--rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.298072 scimap-2.0.1/scimap/helpers/rename.py
--rw-r--r--   0        0        0     6194 2024-03-20 01:42:22.133668 scimap-2.0.1/scimap/helpers/scimap_to_csv.py
--rw-r--r--   0        0        0      766 2024-03-19 18:17:18.230168 scimap-2.0.1/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16939 2024-03-18 19:56:58.653382 scimap-2.0.1/scimap/plotting/addROI_image.py
--rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.790600 scimap-2.0.1/scimap/plotting/cluster_plots.py
--rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.580935 scimap-2.0.1/scimap/plotting/densityPlot2D.py
--rw-r--r--   0        0        0     8772 2024-03-20 13:51:51.354626 scimap-2.0.1/scimap/plotting/distPlot.py
--rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.870855 scimap-2.0.1/scimap/plotting/foldchange.py
--rw-r--r--   0        0        0    11059 2024-03-02 02:00:19.435779 scimap-2.0.1/scimap/plotting/gate_finder.py
--rw-r--r--   0        0        0    11207 2024-03-18 18:24:57.598183 scimap-2.0.1/scimap/plotting/groupCorrelation.py
--rw-r--r--   0        0        0    18210 2024-03-18 18:41:06.721737 scimap-2.0.1/scimap/plotting/heatmap.py
--rw-r--r--   0        0        0     9423 2024-03-02 02:00:12.303252 scimap-2.0.1/scimap/plotting/image_viewer.py
--rw-r--r--   0        0        0    10417 2024-03-18 18:24:52.838506 scimap-2.0.1/scimap/plotting/markerCorrelation.py
--rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.476562 scimap-2.0.1/scimap/plotting/pie.py
--rw-r--r--   0        0        0    12242 2024-03-19 18:32:03.627202 scimap-2.0.1/scimap/plotting/spatialInteractionNetwork.py
--rw-r--r--   0        0        0    10165 2024-03-19 01:23:30.046016 scimap-2.0.1/scimap/plotting/spatial_distance.py
--rw-r--r--   0        0        0    11795 2024-03-19 12:21:07.752382 scimap-2.0.1/scimap/plotting/spatial_interaction.py
--rw-r--r--   0        0        0     5060 2024-03-19 19:10:54.724495 scimap-2.0.1/scimap/plotting/spatial_pscore.py
--rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.182943 scimap-2.0.1/scimap/plotting/spatial_scatterPlot.py
--rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.424269 scimap-2.0.1/scimap/plotting/stacked_barplot.py
--rw-r--r--   0        0        0    12547 2024-03-18 18:34:47.607355 scimap-2.0.1/scimap/plotting/umap.py
--rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.302280 scimap-2.0.1/scimap/plotting/voronoi.py
--rw-r--r--   0        0        0      129 2024-03-17 18:13:28.725249 scimap-2.0.1/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.817117 scimap-2.0.1/scimap/preprocessing/combat.py
--rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.795915 scimap-2.0.1/scimap/preprocessing/log1p.py
--rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.000000 scimap-2.0.1/scimap/preprocessing/mcmicro_to_scimap.py
--rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.438422 scimap-2.0.1/scimap/preprocessing/ngraph.py
--rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.005842 scimap-2.0.1/scimap/preprocessing/rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-2.0.1/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-2.0.1/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-2.0.1/scimap/tests/_data/phenotype_workflow.csv
--rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.375137 scimap-2.0.1/scimap/tests/test_helpers.py
--rw-r--r--   0        0        0      982 2024-03-02 02:50:46.201820 scimap-2.0.1/scimap/tests/test_preprocessing.py
--rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.903918 scimap-2.0.1/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      568 2024-03-02 02:44:25.945510 scimap-2.0.1/scimap/tools/__init__.py
--rw-r--r--   0        0        0    20200 2024-03-19 23:48:54.910997 scimap-2.0.1/scimap/tools/cluster.py
--rw-r--r--   0        0        0    10598 2024-03-18 21:08:47.269456 scimap-2.0.1/scimap/tools/foldchange.py
--rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.563795 scimap-2.0.1/scimap/tools/phenotype_cells.py
--rw-r--r--   0        0        0    12714 2024-03-19 20:32:33.950090 scimap-2.0.1/scimap/tools/spatial_aggregate.py
--rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.502620 scimap-2.0.1/scimap/tools/spatial_cluster.py
--rw-r--r--   0        0        0     9097 2024-03-19 23:43:08.527959 scimap-2.0.1/scimap/tools/spatial_count.py
--rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.522643 scimap-2.0.1/scimap/tools/spatial_distance.py
--rw-r--r--   0        0        0    13752 2024-03-20 01:28:34.142208 scimap-2.0.1/scimap/tools/spatial_expression.py
--rw-r--r--   0        0        0    12059 2024-03-19 12:11:34.371207 scimap-2.0.1/scimap/tools/spatial_interaction.py
--rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.631718 scimap-2.0.1/scimap/tools/spatial_lda.py
--rw-r--r--   0        0        0    12452 2024-03-19 18:49:22.715271 scimap-2.0.1/scimap/tools/spatial_pscore.py
--rw-r--r--   0        0        0    18461 2024-03-19 21:36:08.728628 scimap-2.0.1/scimap/tools/spatial_similarity_search.py
--rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.518742 scimap-2.0.1/scimap/tools/umap.py
--rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 scimap-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-12-22 12:20:25.774355 scimap-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2759 2024-04-02 17:41:31.643157 scimap-2.0.2/README.md
+-rw-r--r--   0        0        0     2522 2024-04-02 18:18:28.489630 scimap-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      391 2024-04-01 23:22:15.513728 scimap-2.0.2/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-2.0.2/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-2.0.2/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-2.0.2/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-2.0.2/scimap/cli/test.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:21:46.158522 scimap-2.0.2/scimap/external/__init__.py
+-rw-r--r--   0        0        0      297 2024-03-20 19:13:27.572207 scimap-2.0.2/scimap/helpers/__init__.py
+-rw-r--r--   0        0        0     7715 2024-03-20 20:49:48.491605 scimap-2.0.2/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     6938 2024-03-12 20:54:07.000000 scimap-2.0.2/scimap/helpers/addROI_omero.py
+-rw-r--r--   0        0        0     3141 2023-11-21 19:42:38.615795 scimap-2.0.2/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0    17024 2024-03-01 20:05:28.511793 scimap-2.0.2/scimap/helpers/animate.py
+-rw-r--r--   0        0        0     7031 2024-03-01 20:14:20.029603 scimap-2.0.2/scimap/helpers/classify.py
+-rw-r--r--   0        0        0     1897 2024-03-20 19:41:09.893157 scimap-2.0.2/scimap/helpers/downloadDemoData.py
+-rw-r--r--   0        0        0     5065 2024-03-01 20:24:14.533825 scimap-2.0.2/scimap/helpers/dropFeatures.py
+-rw-r--r--   0        0        0     4944 2024-03-20 13:25:21.701481 scimap-2.0.2/scimap/helpers/merge_adata_obs.py
+-rw-r--r--   0        0        0     3601 2024-03-01 20:40:16.298072 scimap-2.0.2/scimap/helpers/rename.py
+-rw-r--r--   0        0        0     6194 2024-03-20 01:42:22.133668 scimap-2.0.2/scimap/helpers/scimap_to_csv.py
+-rw-r--r--   0        0        0      766 2024-03-19 18:17:18.230168 scimap-2.0.2/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16939 2024-03-18 19:56:58.653382 scimap-2.0.2/scimap/plotting/addROI_image.py
+-rw-r--r--   0        0        0     6564 2024-03-02 01:59:56.790600 scimap-2.0.2/scimap/plotting/cluster_plots.py
+-rw-r--r--   0        0        0     8369 2024-03-02 01:55:48.580935 scimap-2.0.2/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     8772 2024-03-20 13:51:51.354626 scimap-2.0.2/scimap/plotting/distPlot.py
+-rw-r--r--   0        0        0     6709 2024-03-02 01:59:44.870855 scimap-2.0.2/scimap/plotting/foldchange.py
+-rw-r--r--   0        0        0    11271 2024-04-02 18:18:12.032282 scimap-2.0.2/scimap/plotting/gate_finder.py
+-rw-r--r--   0        0        0    11207 2024-03-18 18:24:57.598183 scimap-2.0.2/scimap/plotting/groupCorrelation.py
+-rw-r--r--   0        0        0    18210 2024-03-18 18:41:06.721737 scimap-2.0.2/scimap/plotting/heatmap.py
+-rw-r--r--   0        0        0     9552 2024-04-02 18:18:20.828150 scimap-2.0.2/scimap/plotting/image_viewer.py
+-rw-r--r--   0        0        0    10417 2024-03-18 18:24:52.838506 scimap-2.0.2/scimap/plotting/markerCorrelation.py
+-rw-r--r--   0        0        0     7419 2024-03-02 01:59:15.476562 scimap-2.0.2/scimap/plotting/pie.py
+-rw-r--r--   0        0        0    12242 2024-03-19 18:32:03.627202 scimap-2.0.2/scimap/plotting/spatialInteractionNetwork.py
+-rw-r--r--   0        0        0    10165 2024-03-19 01:23:30.046016 scimap-2.0.2/scimap/plotting/spatial_distance.py
+-rw-r--r--   0        0        0    11795 2024-03-19 12:21:07.752382 scimap-2.0.2/scimap/plotting/spatial_interaction.py
+-rw-r--r--   0        0        0     5060 2024-03-19 19:10:54.724495 scimap-2.0.2/scimap/plotting/spatial_pscore.py
+-rw-r--r--   0        0        0    12601 2024-03-17 15:26:02.182943 scimap-2.0.2/scimap/plotting/spatial_scatterPlot.py
+-rw-r--r--   0        0        0     7727 2024-03-02 01:58:34.424269 scimap-2.0.2/scimap/plotting/stacked_barplot.py
+-rw-r--r--   0        0        0    12547 2024-03-18 18:34:47.607355 scimap-2.0.2/scimap/plotting/umap.py
+-rw-r--r--   0        0        0    18847 2024-03-02 01:58:10.302280 scimap-2.0.2/scimap/plotting/voronoi.py
+-rw-r--r--   0        0        0      129 2024-03-17 18:13:28.725249 scimap-2.0.2/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4929 2024-03-01 22:07:39.817117 scimap-2.0.2/scimap/preprocessing/combat.py
+-rw-r--r--   0        0        0     3979 2024-03-17 19:14:56.795915 scimap-2.0.2/scimap/preprocessing/log1p.py
+-rw-r--r--   0        0        0    11153 2024-03-13 21:27:02.000000 scimap-2.0.2/scimap/preprocessing/mcmicro_to_scimap.py
+-rw-r--r--   0        0        0     3642 2024-03-18 00:27:18.438422 scimap-2.0.2/scimap/preprocessing/ngraph.py
+-rw-r--r--   0        0        0    17838 2024-02-29 22:11:30.005842 scimap-2.0.2/scimap/preprocessing/rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-2.0.2/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-2.0.2/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-2.0.2/scimap/tests/_data/phenotype_workflow.csv
+-rw-r--r--   0        0        0     1265 2024-03-02 02:51:31.375137 scimap-2.0.2/scimap/tests/test_helpers.py
+-rw-r--r--   0        0        0      982 2024-03-02 02:50:46.201820 scimap-2.0.2/scimap/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     4675 2024-03-02 02:49:28.903918 scimap-2.0.2/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      568 2024-03-02 02:44:25.945510 scimap-2.0.2/scimap/tools/__init__.py
+-rw-r--r--   0        0        0    20200 2024-03-19 23:48:54.910997 scimap-2.0.2/scimap/tools/cluster.py
+-rw-r--r--   0        0        0    10598 2024-03-18 21:08:47.269456 scimap-2.0.2/scimap/tools/foldchange.py
+-rw-r--r--   0        0        0    18754 2024-03-01 13:54:09.563795 scimap-2.0.2/scimap/tools/phenotype_cells.py
+-rw-r--r--   0        0        0    12714 2024-03-19 20:32:33.950090 scimap-2.0.2/scimap/tools/spatial_aggregate.py
+-rw-r--r--   0        0        0     8731 2024-03-02 03:07:59.502620 scimap-2.0.2/scimap/tools/spatial_cluster.py
+-rw-r--r--   0        0        0     9097 2024-03-19 23:43:08.527959 scimap-2.0.2/scimap/tools/spatial_count.py
+-rw-r--r--   0        0        0     6224 2024-03-01 14:13:55.522643 scimap-2.0.2/scimap/tools/spatial_distance.py
+-rw-r--r--   0        0        0    13752 2024-03-20 01:28:34.142208 scimap-2.0.2/scimap/tools/spatial_expression.py
+-rw-r--r--   0        0        0    12059 2024-03-19 12:11:34.371207 scimap-2.0.2/scimap/tools/spatial_interaction.py
+-rw-r--r--   0        0        0    11333 2024-03-01 18:59:27.631718 scimap-2.0.2/scimap/tools/spatial_lda.py
+-rw-r--r--   0        0        0    12452 2024-03-19 18:49:22.715271 scimap-2.0.2/scimap/tools/spatial_pscore.py
+-rw-r--r--   0        0        0    18461 2024-03-19 21:36:08.728628 scimap-2.0.2/scimap/tools/spatial_similarity_search.py
+-rw-r--r--   0        0        0     3830 2024-03-01 19:23:35.518742 scimap-2.0.2/scimap/tools/umap.py
+-rw-r--r--   0        0        0     4780 1970-01-01 00:00:00.000000 scimap-2.0.2/PKG-INFO
```

### Comparing `scimap-2.0.1/LICENSE` & `scimap-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/README.md` & `scimap-2.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -23,21 +23,27 @@
 ```
 # If you have conda installed
 conda create --name scimap python=3.10
 conda activate scimap
 ```
 
 Install `scimap` directly into an activated virtual environment:
+  
+**By default, we recommend installing scimap alongside napari for visualization purposes. Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following napari's documentation.**
 
 ```python
+pip install scimap[napari]
+```
+
+**If installation fails due to pyqt6; install scimap without napari.**
+
+```python
+
 pip install scimap
 
-# Install scimap with napari for visualization
-# Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following their own documentation, and make sure to add them into the same virtual environment, instead of using this command.
-pip install scimap[napari]
 ```
 
 After installation, the package can be imported as:
 
 ```python
 $ python
 >>> import scimap as sm
```

### Comparing `scimap-2.0.1/pyproject.toml` & `scimap-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "SCIMAP"
-version = "2.0.1"
+version = "2.0.2"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `scimap-2.0.1/scimap/cli/_scimap_mcmicro.py` & `scimap-2.0.2/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/cli/test.py` & `scimap-2.0.2/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/_classify.py` & `scimap-2.0.2/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/addROI_omero.py` & `scimap-2.0.2/scimap/helpers/addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/add_roi_scatter.py` & `scimap-2.0.2/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/animate.py` & `scimap-2.0.2/scimap/helpers/animate.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/classify.py` & `scimap-2.0.2/scimap/helpers/classify.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/downloadDemoData.py` & `scimap-2.0.2/scimap/helpers/downloadDemoData.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/dropFeatures.py` & `scimap-2.0.2/scimap/helpers/dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/merge_adata_obs.py` & `scimap-2.0.2/scimap/helpers/merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/rename.py` & `scimap-2.0.2/scimap/helpers/rename.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/helpers/scimap_to_csv.py` & `scimap-2.0.2/scimap/helpers/scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/__init__.py` & `scimap-2.0.2/scimap/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/addROI_image.py` & `scimap-2.0.2/scimap/plotting/addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/cluster_plots.py` & `scimap-2.0.2/scimap/plotting/cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/densityPlot2D.py` & `scimap-2.0.2/scimap/plotting/densityPlot2D.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/distPlot.py` & `scimap-2.0.2/scimap/plotting/distPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/foldchange.py` & `scimap-2.0.2/scimap/plotting/foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/gate_finder.py` & `scimap-2.0.2/scimap/plotting/gate_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import numpy as np
 
 import dask.array as da
 from dask.cache import Cache
 import zarr
 import os
 
-cache = Cache(2e9)  # Leverage two gigabytes of memory
-cache.register()
+# cache = Cache(2e9)  # Leverage two gigabytes of memory
+# cache.register()
 
 
 def gate_finder(
     image_path,
     adata,
     marker_of_interest,
     layer='raw',
@@ -48,92 +48,92 @@
     point_size=10,
     imageid='imageid',
     subset=None,
     seg_mask=None,
     **kwargs,
 ):
     """
-Parameters:
-        image_path (str):
-            Path to the high-resolution image file (supports formats like TIFF, OME.TIFF).
+    Parameters:
+            image_path (str):
+                Path to the high-resolution image file (supports formats like TIFF, OME.TIFF).
 
-        adata (anndata.AnnData):
-            The annotated data matrix.
+            adata (anndata.AnnData):
+                The annotated data matrix.
 
-        marker_of_interest (str):
-            The target marker for which the gating threshold is to be determined.
+            marker_of_interest (str):
+                The target marker for which the gating threshold is to be determined.
 
-        layer (str, optional):
-            Specifies the layer in `adata` containing expression data. Defaults to 'raw' for `adata.raw.X`.
+            layer (str, optional):
+                Specifies the layer in `adata` containing expression data. Defaults to 'raw' for `adata.raw.X`.
 
-        log (bool, optional):
-            Applies log transformation to expression data if set to True. 
+            log (bool, optional):
+                Applies log transformation to expression data if set to True.
 
-        from_gate (int, optional):
-            Starting gate threshold value for the marker of interest. 
+            from_gate (int, optional):
+                Starting gate threshold value for the marker of interest.
 
-        to_gate (int, optional):
-            Ending gate threshold value for the marker of interest. 
+            to_gate (int, optional):
+                Ending gate threshold value for the marker of interest.
 
-        increment (float, optional):
-            Incremental step size between `from_gate` and `to_gate`. 
+            increment (float, optional):
+                Incremental step size between `from_gate` and `to_gate`.
 
-        markers (list, optional):
-            A list of additional markers to include in visualization for context.
+            markers (list, optional):
+                A list of additional markers to include in visualization for context.
 
-        channel_names (list or str, optional):
-            Names of the channels in the image, in order. Defaults to 'default', using `adata.uns['all_markers']`.
+            channel_names (list or str, optional):
+                Names of the channels in the image, in order. Defaults to 'default', using `adata.uns['all_markers']`.
 
-        flip_y (bool, optional):
-            Inverts the Y-axis to match image coordinates if set to True. Defaults to True.
+            flip_y (bool, optional):
+                Inverts the Y-axis to match image coordinates if set to True. Defaults to True.
 
-        x_coordinate, y_coordinate (str, optional):
-            Columns in `adata.obs` specifying cell coordinates. Defaults are 'X_centroid' and 'Y_centroid'.
+            x_coordinate, y_coordinate (str, optional):
+                Columns in `adata.obs` specifying cell coordinates. Defaults are 'X_centroid' and 'Y_centroid'.
 
-        point_size (int, optional):
-            Size of points in the visualization. 
+            point_size (int, optional):
+                Size of points in the visualization.
 
-        imageid (str, optional):
-            Column in `adata.obs` identifying images for datasets with multiple images. 
+            imageid (str, optional):
+                Column in `adata.obs` identifying images for datasets with multiple images.
 
-        subset (str, optional):
-            Specific image identifier for targeted analysis, typically an image ID. 
+            subset (str, optional):
+                Specific image identifier for targeted analysis, typically an image ID.
 
-        seg_mask (str, optional):
-            Path to a segmentation mask file to overlay.
+            seg_mask (str, optional):
+                Path to a segmentation mask file to overlay.
 
-        **kwargs:
-            Additional arguments passed to the visualization tool.
+            **kwargs:
+                Additional arguments passed to the visualization tool.
 
-Returns:
-        Image (napari): 
-            Displays the visualization using napari viewer.
+    Returns:
+            Image (napari):
+                Displays the visualization using napari viewer.
 
-Example:
-    ```python
-    
-    # Visualize gating thresholds for CD45 on a specific image
-    sm.pl.gate_finder(
-        image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD45',
-        from_gate=4, to_gate=10, increment=0.2, flip_y=False, point_size=12,
-        subset='Sample1', seg_mask='/path/to/seg_mask.tif')
+    Example:
+        ```python
 
-    # Log-transformed gating for a marker with additional markers and custom channel names
-    sm.pl.gate_finder(
-        image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD3',
-        log=True, from_gate=3, to_gate=7, increment=0.1, markers=['CD19', 'CD4'],
-        channel_names=['DAPI', 'CD3', 'CD19', 'CD4'], point_size=15)
+        # Visualize gating thresholds for CD45 on a specific image
+        sm.pl.gate_finder(
+            image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD45',
+            from_gate=4, to_gate=10, increment=0.2, flip_y=False, point_size=12,
+            subset='Sample1', seg_mask='/path/to/seg_mask.tif')
 
-    # Explore gating for multiple markers across different segments
-    sm.pl.gate_finder(
-        image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD8',
-        layer='expression', from_gate=5, to_gate=9, increment=0.05, markers=['CD8', 'PD1'],
-        subset='TumorRegion', seg_mask='/path/to/tumor_seg_mask.tif')
-    
-    ```
+        # Log-transformed gating for a marker with additional markers and custom channel names
+        sm.pl.gate_finder(
+            image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD3',
+            log=True, from_gate=3, to_gate=7, increment=0.1, markers=['CD19', 'CD4'],
+            channel_names=['DAPI', 'CD3', 'CD19', 'CD4'], point_size=15)
+
+        # Explore gating for multiple markers across different segments
+        sm.pl.gate_finder(
+            image_path='/path/to/image.ome.tif', adata=adata, marker_of_interest='CD8',
+            layer='expression', from_gate=5, to_gate=9, increment=0.05, markers=['CD8', 'PD1'],
+            subset='TumorRegion', seg_mask='/path/to/tumor_seg_mask.tif')
+
+        ```
     """
 
     # If no raw data is available make a copy
     if adata.raw is None:
         adata.raw = adata
 
     # subset data if neede
```

### Comparing `scimap-2.0.1/scimap/plotting/groupCorrelation.py` & `scimap-2.0.2/scimap/plotting/groupCorrelation.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/heatmap.py` & `scimap-2.0.2/scimap/plotting/heatmap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/image_viewer.py` & `scimap-2.0.2/scimap/plotting/image_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import tifffile as tiff
 
 import dask.array as da
 from dask.cache import Cache
 import zarr
 import os
 
-cache = Cache(2e9)  # Leverage two gigabytes of memory
-cache.register()
+# cache = Cache(2e9)  # Leverage two gigabytes of memory
+# cache.register()
 
 
 def image_viewer(
     image_path,
     adata,
     overlay=None,
     flip_y=True,
@@ -45,72 +45,72 @@
     point_color=None,
     subset=None,
     imageid='imageid',
     seg_mask=None,
     **kwargs,
 ):
     """
-Parameters:
-        image_path (str):  
-            Path to the image file. Supports TIFF, OME.TIFF, and ZARR formats.
+    Parameters:
+            image_path (str):
+                Path to the image file. Supports TIFF, OME.TIFF, and ZARR formats.
 
-        adata (anndata.AnnData):  
-            The annotated data matrix.
+            adata (anndata.AnnData):
+                The annotated data matrix.
 
-        overlay (str, optional):  
-            Column in `adata.obs` containing categorical data for visualization, such as phenotypes or clusters.
+            overlay (str, optional):
+                Column in `adata.obs` containing categorical data for visualization, such as phenotypes or clusters.
 
-        flip_y (bool, optional):  
-            If True, inverts the Y-axis to match image coordinates. 
+            flip_y (bool, optional):
+                If True, inverts the Y-axis to match image coordinates.
 
-        overlay_category (list, optional):  
-            Specific categories within `overlay` to display. If None, all categories are shown.
+            overlay_category (list, optional):
+                Specific categories within `overlay` to display. If None, all categories are shown.
 
-        markers (list, optional):  
-            List of markers to include in the visualization. If None, all available markers are displayed.
+            markers (list, optional):
+                List of markers to include in the visualization. If None, all available markers are displayed.
 
-        channel_names (list or str, optional):  
-            Specifies the order of channels in the image. Default uses all markers in `adata.uns['all_markers']`.
+            channel_names (list or str, optional):
+                Specifies the order of channels in the image. Default uses all markers in `adata.uns['all_markers']`.
 
-        x_coordinate, y_coordinate (str, optional):  
-            Columns in `adata.obs` specifying cell coordinates. Default to 'X_centroid' and 'Y_centroid'.
+            x_coordinate, y_coordinate (str, optional):
+                Columns in `adata.obs` specifying cell coordinates. Default to 'X_centroid' and 'Y_centroid'.
 
-        point_size (int, optional):  
-            Size of the points in the visualization. 
+            point_size (int, optional):
+                Size of the points in the visualization.
 
-        point_color (str or dict, optional):  
-            Color(s) for the points. Can specify a single color or a dictionary mapping categories to colors.
+            point_color (str or dict, optional):
+                Color(s) for the points. Can specify a single color or a dictionary mapping categories to colors.
 
-        imageid (str, optional):  
-            Column in `adata.obs` identifying different images in the dataset. Useful for datasets with multiple images.
+            imageid (str, optional):
+                Column in `adata.obs` identifying different images in the dataset. Useful for datasets with multiple images.
 
-        subset (str, optional):  
-            Identifier for a specific image to analyze, used in conjunction with `imageid`.
+            subset (str, optional):
+                Identifier for a specific image to analyze, used in conjunction with `imageid`.
 
-        seg_mask (str, optional):  
-            Path to a segmentation mask file to overlay.
+            seg_mask (str, optional):
+                Path to a segmentation mask file to overlay.
 
-        **kwargs:  
-            Additional arguments passed to the napari viewer.
+            **kwargs:
+                Additional arguments passed to the napari viewer.
 
-Returns:
-        Image (napari): 
-            Displays the visualization using napari viewer.
+    Returns:
+            Image (napari):
+                Displays the visualization using napari viewer.
 
-Example:
-    ```python
-    
-    # Basic visualization with phenotype overlay
-    sm.pl.image_viewer(image_path='/path/to/image.ome.tif', adata=adata, overlay='phenotype', point_size=5)
+    Example:
+        ```python
 
-    # Visualization with segmentation mask and custom point colors
-    sm.pl.image_viewer(image_path='/path/to/image.ome.tif', adata=adata, seg_mask='/path/to/mask.tif',
-                 overlay='phenotype', point_color={'T cell': 'green', 'B cell': 'blue'}, point_size=7)
+        # Basic visualization with phenotype overlay
+        sm.pl.image_viewer(image_path='/path/to/image.ome.tif', adata=adata, overlay='phenotype', point_size=5)
 
-    ```
+        # Visualization with segmentation mask and custom point colors
+        sm.pl.image_viewer(image_path='/path/to/image.ome.tif', adata=adata, seg_mask='/path/to/mask.tif',
+                     overlay='phenotype', point_color={'T cell': 'green', 'B cell': 'blue'}, point_size=7)
+
+        ```
     """
 
     # TODO
     # - ADD Subset markers for ZARR ssection
     # - Ability to use ZARR metadata if available
 
     # adding option to load just the image without an adata object
```

### Comparing `scimap-2.0.1/scimap/plotting/markerCorrelation.py` & `scimap-2.0.2/scimap/plotting/markerCorrelation.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/pie.py` & `scimap-2.0.2/scimap/plotting/pie.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/spatialInteractionNetwork.py` & `scimap-2.0.2/scimap/plotting/spatialInteractionNetwork.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/spatial_distance.py` & `scimap-2.0.2/scimap/plotting/spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/spatial_interaction.py` & `scimap-2.0.2/scimap/plotting/spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/spatial_pscore.py` & `scimap-2.0.2/scimap/plotting/spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/spatial_scatterPlot.py` & `scimap-2.0.2/scimap/plotting/spatial_scatterPlot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/stacked_barplot.py` & `scimap-2.0.2/scimap/plotting/stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/umap.py` & `scimap-2.0.2/scimap/plotting/umap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/plotting/voronoi.py` & `scimap-2.0.2/scimap/plotting/voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/preprocessing/combat.py` & `scimap-2.0.2/scimap/preprocessing/combat.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/preprocessing/log1p.py` & `scimap-2.0.2/scimap/preprocessing/log1p.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/preprocessing/mcmicro_to_scimap.py` & `scimap-2.0.2/scimap/preprocessing/mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/preprocessing/ngraph.py` & `scimap-2.0.2/scimap/preprocessing/ngraph.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/preprocessing/rescale.py` & `scimap-2.0.2/scimap/preprocessing/rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/_data/example_data.csv` & `scimap-2.0.2/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/_data/example_data.h5ad` & `scimap-2.0.2/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/_data/phenotype_workflow.csv` & `scimap-2.0.2/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/test_helpers.py` & `scimap-2.0.2/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/test_preprocessing.py` & `scimap-2.0.2/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tests/test_tools.py` & `scimap-2.0.2/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/__init__.py` & `scimap-2.0.2/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/cluster.py` & `scimap-2.0.2/scimap/tools/cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/foldchange.py` & `scimap-2.0.2/scimap/tools/foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/phenotype_cells.py` & `scimap-2.0.2/scimap/tools/phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_aggregate.py` & `scimap-2.0.2/scimap/tools/spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_cluster.py` & `scimap-2.0.2/scimap/tools/spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_count.py` & `scimap-2.0.2/scimap/tools/spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_distance.py` & `scimap-2.0.2/scimap/tools/spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_expression.py` & `scimap-2.0.2/scimap/tools/spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_interaction.py` & `scimap-2.0.2/scimap/tools/spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_lda.py` & `scimap-2.0.2/scimap/tools/spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_pscore.py` & `scimap-2.0.2/scimap/tools/spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/spatial_similarity_search.py` & `scimap-2.0.2/scimap/tools/spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/scimap/tools/umap.py` & `scimap-2.0.2/scimap/tools/umap.py`

 * *Files identical despite different names*

### Comparing `scimap-2.0.1/PKG-INFO` & `scimap-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 2.0.1
+Version: 2.0.2
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -72,21 +72,27 @@
 ```
 # If you have conda installed
 conda create --name scimap python=3.10
 conda activate scimap
 ```
 
 Install `scimap` directly into an activated virtual environment:
+  
+**By default, we recommend installing scimap alongside napari for visualization purposes. Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following napari's documentation.**
 
 ```python
+pip install scimap[napari]
+```
+
+**If installation fails due to pyqt6; install scimap without napari.**
+
+```python
+
 pip install scimap
 
-# Install scimap with napari for visualization
-# Please note that napari requires a GUI toolkit like PyQt. If you encounter any errors due to your operating system, you should install scimap and napari separately, following their own documentation, and make sure to add them into the same virtual environment, instead of using this command.
-pip install scimap[napari]
 ```
 
 After installation, the package can be imported as:
 
 ```python
 $ python
 >>> import scimap as sm
```

