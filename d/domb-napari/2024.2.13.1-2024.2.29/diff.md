# Comparing `tmp/domb-napari-2024.2.13.1.tar.gz` & `tmp/domb-napari-2024.2.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domb-napari-2024.2.13.1.tar", last modified: Tue Feb 13 18:11:53 2024, max compression
+gzip compressed data, was "domb-napari-2024.2.29.tar", last modified: Thu Feb 29 18:55:16 2024, max compression
```

## Comparing `domb-napari-2024.2.13.1.tar` & `domb-napari-2024.2.29.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/src/domb_napari/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/src/domb_napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/src/domb_napari/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-13 18:11:42.000000 domb-napari-2024.2.13.1/src/domb_napari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:11:53.095522 domb-napari-2024.2.13.1/src/domb_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 18:11:53.000000 domb-napari-2024.2.13.1/src/domb_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/src/domb_napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/src/domb_napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/src/domb_napari/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-29 18:55:05.000000 domb-napari-2024.2.29/src/domb_napari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:55:16.224167 domb-napari-2024.2.29/src/domb_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 18:55:16.000000 domb-napari-2024.2.29/src/domb_napari.egg-info/top_level.txt
```

### Comparing `domb-napari-2024.2.13.1/LICENSE` & `domb-napari-2024.2.29/LICENSE`

 * *Files identical despite different names*

### Comparing `domb-napari-2024.2.13.1/PKG-INFO` & `domb-napari-2024.2.29/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domb-napari
-Version: 2024.2.13.1
+Version: 2024.2.29
 Summary: napari plugin for analyzing fluorescence-labeled proteins redistribution
 Author: Borys Olifirov
 Author-email: omnia.fatum@gmail.com
 License: MIT
 Project-URL: Documentation, https://domb.bio/
 Project-URL: Source Code, https://github.com/wisstock/domb-napari
 Project-URL: Bug Tracker, https://github.com/wisstock/domb-napari/issues
@@ -26,106 +26,119 @@
 License-File: LICENSE
 Requires-Dist: napari
 Requires-Dist: domb
 
 domb-napari
 ===========
 
-[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg)](https://vshymanskyy.github.io/StandWithUkraine/)
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/domb-napari)](https://napari-hub.org/plugins/domb-napari)
 ![PyPI - Version](https://img.shields.io/pypi/v/domb-napari)
 ![PyPI - License](https://img.shields.io/pypi/l/domb-napari)
 ![Website](https://img.shields.io/website?up_message=domb.bio%2Fnapari&up_color=%2323038C93&url=https%3A%2F%2Fdomb.bio%2Fnapari%2F)
 
 __napari Toolkit of Department of Molecular Biophysics <br /> Bogomoletz Institute of Physiology of NAS of Ukraine, Kyiv,  Ukraine__
 
 napari plugin for analyzing fluorescence-labeled proteins redistribution. Offers widgets designed for analyzing the redistribution of fluorescence-labeled proteins in widefield epifluorescence time-lapse acquisitions. Particularly useful for studying various phenomena such as calcium-dependent translocation of neuronal calcium sensors, synaptic receptor traffic during long-term plasticity induction, and membrane protein tracking.
 
 ![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/translocation.gif)
 __Hippocalcin (neuronal calcium sensor) redistributes in dendritic branches upon NMDA application__
 
+
+
 # Detection of fluorescence redistributions
 A set of widgets designed for detecting fluorescence intensity redistribution through the analysis of differential image series (red-green detection).
 
 Inspired by [Dovgan et al., 2010](https://pubmed.ncbi.nlm.nih.gov/20704590/) and [Osypenko et al., 2019](https://www.sciencedirect.com/science/article/pii/S0969996119301974?via%3Dihub).
 
 ## Image preprocessing
 Provides functions for preprocessing multi-channel fluorescence acquisitions:
 - If the input image has 4 dimensions (time, channel, x-axis, y-axis), channels will be split into individual 3 dimensions images (time, x-axis, y-axis) with the `_ch%index%` suffix.
 - If the `gaussian blur` option is selected, the image will be blurred with a Gaussian filter using sigma=`gaussian sigma`.
 - If the `photobleaching correction` option is selected, the image will undergo correction with exponential (method `exp`) or bi-exponential (method `bi_exp`) fitting.
+- If the `crop ch` option is selected, only a selected range of channel frames will be saved (corresponding to start and stop indexes from `crop range`).
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_0.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_00.png)
 
 ## Red-green series
 Primary method for detecting fluorescent-labeled targets redistribution in time. Returns a series of differential images representing the intensity difference between the current frame and the previous one as new image with the `_red-green` suffix.
 
 Parameters:
 
 - `left frames` - number of previous frames for pixel-wise averaging.
 - `space frames` - number of frames between the last left and first right frames.
 - `right frames` - number of subsequent frames for pixel-wise averaging.
-- `save mask series` - if selected, a series of labels will be created for each frame of the differential image with the threshold `insertion threshold`.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_1.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_11.png)
 
 ## Up masking
 Generates labels for insertion sites (regions with increasing intensity) based on `-red-green` images. Returns labels layer with `_up-labels` suffix.
 
 Parameters:
 
 - `detection img index` - index of the frame from `-red-green` image used for insertion sites detection.
 - `insertion threshold` - threshold value for insertion site detection, intensity on selected `_red-green` frame normalized in -1 - 0 range.
+- `opening footprint` - footprint size in pixels for mask filtering with morphology opening (disabled if 0).
 - `save mask` - if selected, a total up mask (containing all ROIs) will be created with the `_up-mask` suffix.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_2.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_22.png)
 
 ## Intensity masking
 Extension of __Up Masking__ widget. Detects regions with increasing (`masking mode` - `up`) or decreasing (`masking mode` - `down`) intensity in `-red-green` images. Returns a labels layer with either `_up-labels` or `_down-labels` suffix, depending on the mode.
 
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_33.png)
+
+
+# Traffic monitoring with pH-sensitive tag
+A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
+
+Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
+
+## SEP image preprocessing
+Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). `pH 1st frame` option indicates the 1st frame pH. By default frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
+
+If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+
+The `calc projections` option allows obtaining individual pH series projections (pixel-wise series MIP - pixel-wise series average) for the detection of individual exo/endocytosis events.
 
+
+
+# Intensty profiles building and data frame saving
 ## Individual labels profiles
-Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `raw intensity` is selected) or relative intensities (ΔF/F0).
+Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `absolute intensity` is selected) or relative intensities (ΔF/F0).
 
 The `time scale` sets the number of seconds between frames for x-axis scaling.
 
-The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`).
+The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`). You could filter ROIs by minimum and maximum ΔF/F0 amplitudes with the `ΔF aplitude lim` option.
 
-Filters ROIs by minimum (`min amplitude`) and maximum (`max amplitude`) intensity amplitudes.
+_Note: amplitude filtering working with ΔF/F0 profiles only._
 
-_Note: Intensity filtering is most relevant for ΔF/F0 profiles._
+If the `profiles crop` option is selected, only a selected range of intensity profiles indexes will be plotted (corresponding to start and stop indexes from `profiles range`).
 
 Additionally, you can save ROI intensity profiles as .csv using the `save data frame` option and specifying the `saving path`. The output data frames `%img_name%_lab_prof.csv` will contain the following columns:
 
 - __id__ - unique image ID, the name of the input `napari.Image` object.
 - __roi__ - ROI number, consecutively numbered starting from 1.
 - __int__ - ROI mean intensity, raw or ΔF/F0 according to the `raw intensity` option.
 - __index__ - frame index
 - __time__ - frame time point according to the `time scale`.
 
-_Note: The data frame will contain information for all ROIs; filtering options pertain to plotting only._
+_Note: The data frame will contain information for all ROIs; amplitude filtering and crop options pertain to plotting only._
+
+Absolute intensity         | ΔF/F0
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_44.png)|![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_55.png)
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_3.png)
 
-## Labels profile
+## Labels stat profiles
 Builds a plot with the averaged intensity of all ROIs in `labels`. Can take two images (`img 0` and `img 1`) as input if `two profiles` are selected.
 
 The `time scale` and `ΔF win` are the same as in the __Individual Labels Profiles__.
 
-The `stat method` provides methods for calculating intensity errors:
+The `stat method` provides methods for estimation intensity and errors:
 
 - `se` - standard error of mean.
 - `iqr` - interquartile range.
 - `ci` - 95% confidence interval for t-distribution.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_4.png)
-
-# Traffic monitoring with pH-sensitive tag
-A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
-
-Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/), [Gao et al., 2018](https://www.beilstein-journals.org/bjnano/articles/9/79) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
-
-## SEP image preprocessing
-Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). Frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
-
-If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_66.png)
```

### Comparing `domb-napari-2024.2.13.1/README.md` & `domb-napari-2024.2.29/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,115 @@
 domb-napari
 ===========
 
-[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg)](https://vshymanskyy.github.io/StandWithUkraine/)
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/domb-napari)](https://napari-hub.org/plugins/domb-napari)
 ![PyPI - Version](https://img.shields.io/pypi/v/domb-napari)
 ![PyPI - License](https://img.shields.io/pypi/l/domb-napari)
 ![Website](https://img.shields.io/website?up_message=domb.bio%2Fnapari&up_color=%2323038C93&url=https%3A%2F%2Fdomb.bio%2Fnapari%2F)
 
 __napari Toolkit of Department of Molecular Biophysics <br /> Bogomoletz Institute of Physiology of NAS of Ukraine, Kyiv,  Ukraine__
 
 napari plugin for analyzing fluorescence-labeled proteins redistribution. Offers widgets designed for analyzing the redistribution of fluorescence-labeled proteins in widefield epifluorescence time-lapse acquisitions. Particularly useful for studying various phenomena such as calcium-dependent translocation of neuronal calcium sensors, synaptic receptor traffic during long-term plasticity induction, and membrane protein tracking.
 
 ![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/translocation.gif)
 __Hippocalcin (neuronal calcium sensor) redistributes in dendritic branches upon NMDA application__
 
+
+
 # Detection of fluorescence redistributions
 A set of widgets designed for detecting fluorescence intensity redistribution through the analysis of differential image series (red-green detection).
 
 Inspired by [Dovgan et al., 2010](https://pubmed.ncbi.nlm.nih.gov/20704590/) and [Osypenko et al., 2019](https://www.sciencedirect.com/science/article/pii/S0969996119301974?via%3Dihub).
 
 ## Image preprocessing
 Provides functions for preprocessing multi-channel fluorescence acquisitions:
 - If the input image has 4 dimensions (time, channel, x-axis, y-axis), channels will be split into individual 3 dimensions images (time, x-axis, y-axis) with the `_ch%index%` suffix.
 - If the `gaussian blur` option is selected, the image will be blurred with a Gaussian filter using sigma=`gaussian sigma`.
 - If the `photobleaching correction` option is selected, the image will undergo correction with exponential (method `exp`) or bi-exponential (method `bi_exp`) fitting.
+- If the `crop ch` option is selected, only a selected range of channel frames will be saved (corresponding to start and stop indexes from `crop range`).
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_0.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_00.png)
 
 ## Red-green series
 Primary method for detecting fluorescent-labeled targets redistribution in time. Returns a series of differential images representing the intensity difference between the current frame and the previous one as new image with the `_red-green` suffix.
 
 Parameters:
 
 - `left frames` - number of previous frames for pixel-wise averaging.
 - `space frames` - number of frames between the last left and first right frames.
 - `right frames` - number of subsequent frames for pixel-wise averaging.
-- `save mask series` - if selected, a series of labels will be created for each frame of the differential image with the threshold `insertion threshold`.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_1.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_11.png)
 
 ## Up masking
 Generates labels for insertion sites (regions with increasing intensity) based on `-red-green` images. Returns labels layer with `_up-labels` suffix.
 
 Parameters:
 
 - `detection img index` - index of the frame from `-red-green` image used for insertion sites detection.
 - `insertion threshold` - threshold value for insertion site detection, intensity on selected `_red-green` frame normalized in -1 - 0 range.
+- `opening footprint` - footprint size in pixels for mask filtering with morphology opening (disabled if 0).
 - `save mask` - if selected, a total up mask (containing all ROIs) will be created with the `_up-mask` suffix.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_2.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_22.png)
 
 ## Intensity masking
 Extension of __Up Masking__ widget. Detects regions with increasing (`masking mode` - `up`) or decreasing (`masking mode` - `down`) intensity in `-red-green` images. Returns a labels layer with either `_up-labels` or `_down-labels` suffix, depending on the mode.
 
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_33.png)
+
+
+# Traffic monitoring with pH-sensitive tag
+A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
+
+Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
+
+## SEP image preprocessing
+Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). `pH 1st frame` option indicates the 1st frame pH. By default frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
+
+If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+
+The `calc projections` option allows obtaining individual pH series projections (pixel-wise series MIP - pixel-wise series average) for the detection of individual exo/endocytosis events.
 
+
+
+# Intensty profiles building and data frame saving
 ## Individual labels profiles
-Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `raw intensity` is selected) or relative intensities (ΔF/F0).
+Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `absolute intensity` is selected) or relative intensities (ΔF/F0).
 
 The `time scale` sets the number of seconds between frames for x-axis scaling.
 
-The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`).
+The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`). You could filter ROIs by minimum and maximum ΔF/F0 amplitudes with the `ΔF aplitude lim` option.
 
-Filters ROIs by minimum (`min amplitude`) and maximum (`max amplitude`) intensity amplitudes.
+_Note: amplitude filtering working with ΔF/F0 profiles only._
 
-_Note: Intensity filtering is most relevant for ΔF/F0 profiles._
+If the `profiles crop` option is selected, only a selected range of intensity profiles indexes will be plotted (corresponding to start and stop indexes from `profiles range`).
 
 Additionally, you can save ROI intensity profiles as .csv using the `save data frame` option and specifying the `saving path`. The output data frames `%img_name%_lab_prof.csv` will contain the following columns:
 
 - __id__ - unique image ID, the name of the input `napari.Image` object.
 - __roi__ - ROI number, consecutively numbered starting from 1.
 - __int__ - ROI mean intensity, raw or ΔF/F0 according to the `raw intensity` option.
 - __index__ - frame index
 - __time__ - frame time point according to the `time scale`.
 
-_Note: The data frame will contain information for all ROIs; filtering options pertain to plotting only._
+_Note: The data frame will contain information for all ROIs; amplitude filtering and crop options pertain to plotting only._
+
+Absolute intensity         | ΔF/F0
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_44.png)|![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_55.png)
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_3.png)
 
-## Labels profile
+## Labels stat profiles
 Builds a plot with the averaged intensity of all ROIs in `labels`. Can take two images (`img 0` and `img 1`) as input if `two profiles` are selected.
 
 The `time scale` and `ΔF win` are the same as in the __Individual Labels Profiles__.
 
-The `stat method` provides methods for calculating intensity errors:
+The `stat method` provides methods for estimation intensity and errors:
 
 - `se` - standard error of mean.
 - `iqr` - interquartile range.
 - `ci` - 95% confidence interval for t-distribution.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_4.png)
-
-# Traffic monitoring with pH-sensitive tag
-A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
-
-Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/), [Gao et al., 2018](https://www.beilstein-journals.org/bjnano/articles/9/79) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
-
-## SEP image preprocessing
-Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). Frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
-
-If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_66.png)
```

### Comparing `domb-napari-2024.2.13.1/setup.cfg` & `domb-napari-2024.2.29/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = domb-napari
-version = 2024.02.13.01
+version = 2024.02.29
 author = Borys Olifirov
 author_email = omnia.fatum@gmail.com
 license = MIT
 description = napari plugin for analyzing fluorescence-labeled proteins redistribution
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls =
```

### Comparing `domb-napari-2024.2.13.1/src/domb_napari/_widget.py` & `domb-napari-2024.2.29/src/domb_napari/_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,277 +1,333 @@
 from magicgui import magic_factory
 
 import napari
 from napari import Viewer
 from napari.layers import Image, Labels
 from napari.utils.notifications import show_info
+from napari.qt.threading import thread_worker
 
 import pathlib
 import os
 
 import numpy as np
 from scipy import ndimage as ndi
 from scipy import stats
 
 from skimage import filters
 from skimage import morphology
 from skimage import measure
+from skimage import restoration
 
 import vispy.color
 
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_qt5agg import FigureCanvas
 
 from domb.utils import masking
 
 
-def _save_img(viewer: Viewer, img:np.ndarray, img_name:str):
-    try: 
-        viewer.layers[img_name].data = img
-    except KeyError:
-        viewer.add_image(img, name=img_name, colormap='turbo')
+def _red_green():
+     """ Red-green colormap
+
+     """
+     return vispy.color.Colormap([[0.0, 1.0, 0.0],
+                                  [0.0, 0.9, 0.0],
+                                  [0.0, 0.5, 0.0],
+                                  [0.0, 0.0, 0.0],
+                                  [0.5, 0.0, 0.0],
+                                  [0.9, 0.0, 0.0],
+                                  [1.0, 0.0, 0.0]])
 
 
 @magic_factory(call_button='Preprocess Image',
                correction_method={"choices": ['exp', 'bi_exp']},)
 def split_channels(viewer: Viewer, img:Image,
-                   gaussian_blur:bool=False, gaussian_sigma=0.5,
+                   gaussian_blur:bool=True, gaussian_sigma=0.75,
                    photobleaching_correction:bool=False,
-                   correction_method:str='exp'):
+                   correction_method:str='exp',
+                   crop_ch:bool=False,
+                   crop_range:list=[0,10]):
     if input is not None:
-        series_dim = img.data.ndim
-        if series_dim == 4:
-            preprocessing_info = f'{img.name}: Ch. split and preprocessing mode'
-            print(preprocessing_info)
-            show_info(preprocessing_info)
-
-            for i in range(img.data.shape[1]):
-                ch_name = img.name + f'_ch{i}'
-                ch_img = img.data[:,i,:,:].astype(float)
+        def _save_ch(params):
+            img = params[0]
+            img_name = params[1]
+            try: 
+                viewer.layers[img_name].data = img
+            except KeyError:
+                new_image = viewer.add_image(img, name=img_name, colormap='turbo')
+
+        @thread_worker(connect={'yielded':_save_ch})
+        def _split_channels():
+            def _preprocessing(ch_img):
                 corr_img = np.mean(ch_img, axis=0)
                 corr_mask = corr_img > filters.threshold_otsu(corr_img)
                 corr_mask = morphology.dilation(corr_mask, footprint=morphology.disk(10))
+                if crop_ch:
+                    if len(crop_range) == 2:
+                        ch_img = ch_img[crop_range[0]:crop_range[-1],:,:]
+                    else:
+                        raise ValueError('List of indexes should has 2 elements!')
                 if gaussian_blur:
                     ch_img = filters.gaussian(ch_img, sigma=gaussian_sigma, channel_axis=0)
-                    print(f'{ch_name}: Img series blured with sigma {gaussian_sigma}')
+                    show_info(f'Img series blured with sigma {gaussian_sigma}')
                 if photobleaching_correction:
                     ch_img,_,r_corr = masking.pb_exp_correction(input_img=ch_img,
                                                                 mask=corr_mask,
                                                                 method=correction_method)
-                    print(f'{ch_name}: Photobleaching correction, r^2={r_corr}')
+                    show_info(f'{correction_method} photobleaching correction, r^2={r_corr}')
+                return ch_img
 
-                _save_img(viewer=viewer, img=ch_img, img_name=ch_name)
-        elif series_dim == 3:
-            preprocessing_info = f'{img.name}: Image already has 3 dimensions, preprocessing only mode'
-            print(preprocessing_info)
-            show_info(preprocessing_info)
-            
-            ch_name = img.name + '_ch0'
-            ch_img = img.data
-            if gaussian_blur:
-                ch_img = filters.gaussian(ch_img, sigma=gaussian_sigma, channel_axis=0)
-                print(f'{ch_name}: Img series blured with sigma {gaussian_sigma}')
-            if photobleaching_correction:
-                corr_img = np.mean(ch_img, axis=0)
-                corr_mask = corr_img > filters.threshold_otsu(corr_img)
-                ch_img,_,r_corr = masking.pb_exp_correction(input_img=ch_img, mask=corr_mask)
-                print(f'{ch_name}: Photobleaching correction, r^2={r_corr}')
-            _save_img(viewer=viewer, img=ch_img, img_name=ch_name)
-        else:
-            raise ValueError('The input image should have 4 dimensions!')
+            if img.data.ndim == 4:
+                show_info(f'{img.name}: Ch. split and preprocessing mode')
+                for i in range(img.data.shape[1]):
+                    show_info(f'{img.name}: Ch. {i} preprocessing')
+                    yield (_preprocessing(ch_img=img.data[:,i,:,:]), img.name + f'_ch{i}')
+            elif img.data.ndim == 3:
+                show_info(f'{img.name}: Image already has 3 dimensions, preprocessing only mode')
+                yield (_preprocessing(ch_img=img.data), img.name + '_ch0')
+            else:
+                raise ValueError('Input image should have 3 or 4 dimensions!')       
         
+        _split_channels()
+
 
-@magic_factory(call_button='Split SEP')
+@magic_factory(call_button='Split SEP',
+               pH_1st_frame={"choices": ['7.3', '6.0']},)
 def split_sep(viewer: Viewer, img:Image,
-              calc_surface_img:bool=False):
+              pH_1st_frame:str='7.3',
+              calc_surface_img:bool=False,
+              calc_projections:bool=False):
     if input is not None:
-        series_dim = img.data.ndim
-        if series_dim == 3:
-            sep_img = img.data.astype(float)
-            total_img = sep_img[0::2,:,:]
-            intra_img = sep_img[1::2,:,:]
-
-            total_name = img.name + '_total'
-            intra_name = img.name + '_intra'
-
-            _save_img(viewer=viewer, img=total_img, img_name=total_name)
-            _save_img(viewer=viewer, img=intra_img, img_name=intra_name)
-
-            if calc_surface_img:
-                surface_img = total_img - intra_img
-                surface_name = img.name + '_surface'
-                _save_img(viewer=viewer, img=surface_img, img_name=surface_name)
+        if img.data.ndim == 3:
+
+            def _save_sep(params):
+                img = params[0]
+                img_name = params[1]
+                cmap_rg = False
+                if len(params) == 3:
+                    cmap_rg = params[2]
+                try: 
+                    viewer.layers[img_name].data = img
+                except KeyError:
+                    new_image = viewer.add_image(img, name=img_name, colormap='turbo')
+                    if cmap_rg:
+                        new_image.colormap = 'red-green', _red_green()
+                    else:
+                        new_image.colormap = 'turbo'
+
+            @thread_worker(connect={'yielded':_save_sep})
+            def _split_sep():
+                sep_img = img.data.astype(float)
+
+                if pH_1st_frame == '7.3':
+                    total_start_i, intra_start_i = 0, 1
+                elif pH_1st_frame == '6.0':
+                    total_start_i, intra_start_i = 1, 0
+
+                total_img = sep_img[total_start_i::2,:,:]  # 0
+                intra_img = sep_img[intra_start_i::2,:,:]  # 1
+
+                total_name = img.name + '_total'
+                intra_name = img.name + '_intra'
+
+                yield (total_img, total_name)
+                yield (intra_img, intra_name)
+
+                if calc_projections:
+                    projections_diff = lambda x: np.max(x, axis=0) - np.mean(x, axis=0)
+                    yield (projections_diff(total_img),
+                           img.name + '_total-projection',
+                           True)
+                    yield (projections_diff(intra_img),
+                           img.name + '_intra-projection',
+                           True)
+                    yield (np.max(intra_img, axis=0),
+                           img.name + '_intra-mip')
+
+                if calc_surface_img:
+                    surface_img = total_img - intra_img
+                    yield (surface_img,
+                           img.name + '_surface')
+                    if calc_projections:
+                        yield (projections_diff(surface_img),
+                               img.name + '_surface-projection',
+                               True)
+            
+            _split_sep()
         else:
             raise ValueError('The input image should have 3 dimensions!')
 
 
-@magic_factory(call_button='Calc Red-Green',
-               insertion_threshold={"widget_type": "FloatSlider", 'max': 1},)
+@magic_factory(call_button='Calc Red-Green')
 def der_series(viewer: Viewer, img:Image,
-               left_frames:int=2, space_frames:int=2, right_frames:int=2,
-               save_mask_series:bool=False,
-               insertion_threshold:float=0.2):
+               left_frames:int=2, space_frames:int=2, right_frames:int=2):
     if input is not None:
         if img.data.ndim != 3:
             raise ValueError('The input image should have 3 dimensions!')
-        ref_img = img.data
-
-        der_img = []
-        mask_img = []
-        for i in range(ref_img.shape[0]-(left_frames+right_frames+space_frames)):
-            img_base = np.mean(ref_img[i:i+left_frames+1], axis=0)
-            img_stim = np.mean(ref_img[i+left_frames+right_frames:i+left_frames+right_frames+space_frames+1], axis=0)
-            
-            img_diff = img_stim-img_base
-            img_mask = img_diff >= np.max(np.abs(img_diff)) * insertion_threshold
-
-            der_img.append(img_diff)
-            mask_img.append(img_mask)
+        img_name = img.name + '_red-green'
 
-        der_img = np.asarray(der_img, dtype=float)
-        mask_img = np.asarray(mask_img, dtype=float)
-        der_contrast_lim = np.max(np.abs(der_img)) * 0.75
-        print(f'Derivate series shape: {der_img.shape}')
-
-        red_green_cmap = vispy.color.Colormap([[0.0, 1.0, 0.0],
-                                               [0.0, 0.9, 0.0],
-                                               [0.0, 0.5, 0.0],
-                                               [0.0, 0.0, 0.0],
-                                               [0.5, 0.0, 0.0],
-                                               [0.9, 0.0, 0.0],
-                                               [1.0, 0.0, 0.0]])
+        def _save_rg_img(img):
+            try: 
+                viewer.layers[img_name].data = img
+            except KeyError:
+                c_lim = np.max(np.abs(img)) * 0.75
+                new_image = viewer.add_image(img, name=img_name, contrast_limits=[-c_lim, c_lim])
+                new_image.colormap = 'red-green', _red_green()
+
+        @thread_worker(connect={'yielded':_save_rg_img})
+        def _der_series():
+            ref_img = img.data
+
+            der_img = []
+            # mask_img = []
+            for i in range(ref_img.shape[0]-(left_frames+right_frames+space_frames)):
+                img_base = np.mean(ref_img[i:i+left_frames+1], axis=0)
+                img_stim = np.mean(ref_img[i+left_frames+right_frames:i+left_frames+right_frames+space_frames+1], axis=0)
+                
+                img_diff = img_stim-img_base
+                der_img.append(img_diff)
+                # img_mask = img_diff >= np.max(np.abs(img_diff)) * insertion_threshold
+                # mask_img.append(img_mask)
+
+            der_img = np.asarray(der_img, dtype=float)
+            # mask_img = np.asarray(mask_img, dtype=float)
+            yield der_img
 
-        img_name = img.name + '_red-green'
-        try:
-            viewer.layers[img_name].data = der_img
-        except KeyError:
-            der_layer = viewer.add_image(der_img, name=img_name,
-                                         contrast_limits=[-der_contrast_lim, der_contrast_lim])
-            der_layer.colormap = 'red-green', red_green_cmap
-
-        if save_mask_series:
-            mask_name = img.name + '_red-mask'
-            _save_img(viewer=viewer, img=mask_img, img_name=mask_name)
+        _der_series()
 
 
 @magic_factory(call_button='Build Up Mask',
                insertion_threshold={"widget_type": "FloatSlider", 'max': 1},)  # insertions_threshold={'widget_type': 'FloatSlider', 'max': 1}
 def up_mask_calc(viewer: Viewer, img:Image, detection_img_index:int=2,
                  insertion_threshold:float=0.2,
+                 opening_footprint:int=0,
                  save_mask:bool=False):
     if input is not None:
         if img.data.ndim != 3:
-            raise ValueError('The input image should have 2 dimensions!')
-        input_img = img.data
-        detection_img = input_img[detection_img_index]
-        
-        up_mask = detection_img >= np.max(np.abs(detection_img)) * insertion_threshold
-        up_mask = morphology.opening(up_mask, footprint=morphology.disk(1))
-        up_mask = ndi.binary_fill_holes(up_mask)
-        up_mask = up_mask.astype(int)
-        up_labels = measure.label(up_mask)
-        print(f'Up mask shape: {up_mask.shape}, detected {np.max(up_labels)} labels')
-            
+            raise ValueError('The input image should have 3 dimensions!')
         labels_name = img.name + '_up-labels'
-        try:
-            viewer.layers[labels_name].data = up_labels
-        except KeyError:
-            viewer.add_labels(up_labels, name=labels_name, opacity=0.6)
+        mask_name = img.name + '_up-mask'
 
-        if save_mask:
-            mask_name = img.name + '_up-mask'
+        def _save_up_labels(params):
+            lab = params[0]
+            name = params[1]
             try:
-                viewer.layers[mask_name].data = up_mask
+                viewer.layers[name].data = lab
             except KeyError:
-                viewer.add_labels(up_mask, name=mask_name,
-                                num_colors=1, color={1:(255,0,0,255)},
-                                opacity=0.6)
+                new_labels = viewer.add_labels(lab, name=name, opacity=1)
+                new_labels.contour = 1
+
+        @thread_worker(connect={'yielded':_save_up_labels})
+        def _up_mask_calc():
+            input_img = img.data
+            detection_img = input_img[detection_img_index]
+            
+            up_mask = detection_img >= np.max(np.abs(detection_img)) * insertion_threshold
+            up_mask = morphology.erosion(up_mask, footprint=morphology.disk(2))
+            up_mask = morphology.dilation(up_mask, footprint=morphology.disk(1))
+            up_mask = ndi.binary_fill_holes(up_mask)
+            up_mask = up_mask.astype(int)
+
+            if opening_footprint != 0:
+                up_mask = morphology.opening(up_mask, footprint=morphology.disk(opening_footprint))
+                up_mask = morphology.dilation(up_mask, footprint=morphology.disk(1))
+
+            up_labels = measure.label(up_mask)
+            show_info(f'{img.name}: detected {np.max(up_labels)} labels')
+
+            yield (up_labels, labels_name)
+            if save_mask:
+                yield (up_mask, mask_name)
+
+        _up_mask_calc()                
 
 
 @magic_factory(call_button='Build Mask',
                masking_mode={"choices": ['up', 'down']},)
 def mask_calc(viewer: Viewer, img:Image, detection_frame_index:int=2,
               masking_mode:str='up',
               up_threshold:float=0.2,
-              down_threshold:float=-0.1):
+              down_threshold:float=-0.9,
+              opening_footprint:int=0):
     if input is not None:
         if img.data.ndim != 3:
             raise ValueError('The input image should have 3 dimensions!')
-        input_img = img.data
-        detection_img = input_img[detection_frame_index]
 
         if masking_mode == 'up':
-            mask = detection_img >= np.max(np.abs(detection_img)) * up_threshold
             labels_name = img.name + '_up-labels'
-            # mask_name = img.name + '_up-mask'
         elif masking_mode == 'down':        
-            mask = detection_img <= np.max(np.abs(detection_img)) * down_threshold
             labels_name = img.name + '_down-labels'
-            # mask_name = img.name + '_down-mask'
-
-        mask = morphology.opening(mask, footprint=morphology.disk(3))
-        mask = ndi.binary_fill_holes(mask)
-        mask = mask.astype(int)
-        labels = measure.label(mask)
-
-        mask_info = f'{img.name}: detected {np.max(labels)} labels'
-        print(mask_info)
-        show_info(mask_info)
-            
-        try:
-            viewer.layers[labels_name].data = labels
-        except KeyError:
-            viewer.add_labels(labels, name=labels_name, opacity=0.6)
 
-        if save_mask:
+        def _save_rg_labels(params):
+            lab = params[0]
+            name = params[1]
             try:
-                viewer.layers[mask_name].data = mask
+                viewer.layers[name].data = lab
             except KeyError:
-                viewer.add_labels(mask, name=mask_name,
-                                num_colors=1, color={1:(255,0,0,255)},
-                                opacity=0.6)
+                new_labels = viewer.add_labels(lab, name=labels_name, opacity=1)
+                new_labels.contour = 1
 
+        @thread_worker(connect={'yielded':_save_rg_labels})
+        def _mask_calc():
+            input_img = img.data
+            detection_img = input_img[detection_frame_index]
+
+            if masking_mode == 'up':
+                mask = detection_img >= np.max(np.abs(detection_img)) * up_threshold
+            elif masking_mode == 'down':        
+                mask = detection_img <= np.max(np.abs(detection_img)) * down_threshold
+
+            mask = morphology.erosion(mask, footprint=morphology.disk(2))
+            mask = morphology.dilation(mask, footprint=morphology.disk(1))
+            mask = ndi.binary_fill_holes(mask)
+            mask = mask.astype(int)
+
+            if opening_footprint != 0:
+                mask = morphology.opening(mask, footprint=morphology.disk(opening_footprint))
+                mask = morphology.dilation(mask, footprint=morphology.disk(1))
+
+            labels = measure.label(mask)
+            show_info(f'{img.name}: detected {np.max(labels)} "{masking_mode}" labels')
+
+            yield (labels, labels_name)
+
+        _mask_calc()
+            
 
 @magic_factory(call_button='Build Profiles',
                saving_path={'mode': 'd'})
 def labels_profile_line(viewer: Viewer, img:Image, labels:Labels,
-                        time_scale:float=2.0,
-                        raw_intensity:bool=True,
+                        time_scale:float=5.0,
+                        absolute_intensity:bool=True,
                         ΔF_win:int=5,
-                        min_amplitude:float=0.0,
-                        max_amplitude:float=5.0,
-                        frame_crop:bool=False,
-                        start_frame:int=0,
-                        stop_frame:int=10,
+                        ΔF_aplitude_lim:list=[10.0, 10.0],
+                        profiles_crop:bool=False,
+                        profiles_range:list=[0,10],
                         save_data_frame:bool=False,
                         saving_path:pathlib.Path = os.getcwd()):
     if input is not None:
         input_img = img.data
         input_labels = labels.data
         df_name = img.name + '_lab_prof'
 
         profile_dF, profile_raw = masking.label_prof_arr(input_label=input_labels,
                                                          input_img_series=input_img,
                                                          f0_win=ΔF_win)
         time_line = np.linspace(0, input_img.shape[0]*time_scale, \
                                 num=input_img.shape[0])
 
-        if frame_crop:
-            profile_dF = profile_dF[start_frame:stop_frame] 
-            profile_raw = profile_raw[start_frame:stop_frame]
-            time_line = time_line[start_frame:stop_frame]
-
-        if raw_intensity:
+        if absolute_intensity:
             profile_to_plot = profile_raw
             ylab = 'Intensity, a.u.'
-            df_name = df_name + '_raw'
+            df_name = df_name + '_absolute'
         else:
             profile_to_plot = profile_dF
             ylab = 'ΔF/F0'
-            df_name = df_name + '_dF'
+            df_name = df_name + '_ΔF'
 
         if save_data_frame:
             import pandas as pd
             output_df = pd.DataFrame(columns=['id','roi','int', 'index', 'time'])
             for num_ROI in range(profile_to_plot.shape[0]):
                 profile_ROI = profile_to_plot[num_ROI]
                 df_ROI = pd.DataFrame({'id':np.full(profile_ROI.shape[0], img.name),
@@ -280,43 +336,52 @@
                                        'index': np.linspace(0, input_img.shape[0], num=input_img.shape[0], dtype=int),
                                        'time':time_line})
                 output_df = pd.concat([output_df.astype(df_ROI.dtypes),
                                        df_ROI.astype(output_df.dtypes)],
                                       ignore_index=True)
             output_df.to_csv(os.path.join(saving_path, df_name+'.csv'))
 
-        # plotting        
+        # plotting
+        if profiles_crop:
+            profile_to_plot = profile_to_plot[:,profiles_range[0]:profiles_range[1]]
+            time_line = time_line[profiles_range[0]:profiles_range[1]]
+
+        lab_colors = labels.get_color([prop['label'] for prop in measure.regionprops(label_image=input_labels)])
+
+        print(profile_to_plot.shape, time_line.shape, lab_colors.shape)
+
         mpl_fig = plt.figure()
         ax = mpl_fig.add_subplot(111)
         ax.spines['top'].set_visible(False)
         ax.spines['right'].set_visible(False)
-        for num_ROI in range(profile_to_plot.shape[0]):
+        for num_ROI, color in enumerate(lab_colors):
             profile_ROI = profile_to_plot[num_ROI]
-            if raw_intensity:
+            print(profile_ROI.shape, time_line.shape, color.shape)
+            if absolute_intensity:
                 ax.plot(time_line, profile_ROI,
-                         alpha=0.35, marker='o')
-                plt_title = f'{img.name} individual labels raw profiles'
-            elif (profile_ROI.max() > min_amplitude) | (profile_ROI.max() < max_amplitude):
+                         alpha=0.45, marker='o', color=color)
+                plt_title = f'{img.name} absolute intensity profiles, labels {labels.name}'
+            elif (profile_ROI.min() > -ΔF_aplitude_lim[0]) | (profile_ROI.max() < ΔF_aplitude_lim[1]):
                 ax.plot(time_line, profile_ROI,
-                         alpha=0.35, marker='o')
-                plt_title = f'{img.name} individual labels profiles (min={min_amplitude}, max={max_amplitude})'
+                         alpha=0.45, marker='o', color=color)
+                plt_title = f'{img.name} ΔF/F0 profiles (lim -{ΔF_aplitude_lim[0]}, {ΔF_aplitude_lim[1]}), labels {labels.name}'
             else:
                 continue
         ax.grid(color='grey', linewidth=.25)
         ax.set_xlabel('Time, s')
         ax.set_ylabel(ylab)
         plt.title(plt_title)
         viewer.window.add_dock_widget(FigureCanvas(mpl_fig), name=f'{img.name} Profile')
 
 
 @magic_factory(call_button='Build Profile',
                stat_method={"choices": ['se', 'iqr', 'ci']},)
 def labels_profile_stat(viewer: Viewer, img_0:Image, img_1:Image, labels:Labels,
                         two_profiles:bool=False, 
-                        time_scale:float=2,
+                        time_scale:float=5.0,
                         ΔF_win:int=5,
                         stat_method:str='se'):
     if input is not None:
         # mean, se
         arr_se_stat = lambda x: (np.mean(x, axis=0), \
                                 np.std(x, axis=0)/np.sqrt(x.shape[1]))
         # meadian, IQR
```

### Comparing `domb-napari-2024.2.13.1/src/domb_napari/napari.yaml` & `domb-napari-2024.2.29/src/domb_napari/napari.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     - id: domb-napari.mask_calc_widget
       title: Intensity masking
       python_name: domb_napari._widget:mask_calc
     - id: domb-napari.labels_profiles_set_widget
       title: Individual labels profiles
       python_name: domb_napari._widget:labels_profile_line
     - id: domb-napari.labels_profile_widget
-      title: Labels profile
+      title: Labels stat profiles
       python_name: domb_napari._widget:labels_profile_stat
   widgets:
     - command: domb-napari.split_channels_widget
       display_name: Image preprocessing
-    - command: domb-napari.der_series_widget
-      display_name: Red-green series
     - command: domb-napari.split_sep_widget
       display_name: SEP preprocessing
+    - command: domb-napari.der_series_widget
+      display_name: Red-green series
     - command: domb-napari.up_mask_calc_widget
       display_name: Up masking
     - command: domb-napari.mask_calc_widget
       display_name: Intensity masking
     - command: domb-napari.labels_profiles_set_widget
       display_name: Individual labels profiles
     - command: domb-napari.labels_profile_widget
-      display_name: Labels profile
+      display_name: Labels stat profiles
```

### Comparing `domb-napari-2024.2.13.1/src/domb_napari.egg-info/PKG-INFO` & `domb-napari-2024.2.29/src/domb_napari.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domb-napari
-Version: 2024.2.13.1
+Version: 2024.2.29
 Summary: napari plugin for analyzing fluorescence-labeled proteins redistribution
 Author: Borys Olifirov
 Author-email: omnia.fatum@gmail.com
 License: MIT
 Project-URL: Documentation, https://domb.bio/
 Project-URL: Source Code, https://github.com/wisstock/domb-napari
 Project-URL: Bug Tracker, https://github.com/wisstock/domb-napari/issues
@@ -26,106 +26,119 @@
 License-File: LICENSE
 Requires-Dist: napari
 Requires-Dist: domb
 
 domb-napari
 ===========
 
-[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg)](https://vshymanskyy.github.io/StandWithUkraine/)
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/domb-napari)](https://napari-hub.org/plugins/domb-napari)
 ![PyPI - Version](https://img.shields.io/pypi/v/domb-napari)
 ![PyPI - License](https://img.shields.io/pypi/l/domb-napari)
 ![Website](https://img.shields.io/website?up_message=domb.bio%2Fnapari&up_color=%2323038C93&url=https%3A%2F%2Fdomb.bio%2Fnapari%2F)
 
 __napari Toolkit of Department of Molecular Biophysics <br /> Bogomoletz Institute of Physiology of NAS of Ukraine, Kyiv,  Ukraine__
 
 napari plugin for analyzing fluorescence-labeled proteins redistribution. Offers widgets designed for analyzing the redistribution of fluorescence-labeled proteins in widefield epifluorescence time-lapse acquisitions. Particularly useful for studying various phenomena such as calcium-dependent translocation of neuronal calcium sensors, synaptic receptor traffic during long-term plasticity induction, and membrane protein tracking.
 
 ![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/translocation.gif)
 __Hippocalcin (neuronal calcium sensor) redistributes in dendritic branches upon NMDA application__
 
+
+
 # Detection of fluorescence redistributions
 A set of widgets designed for detecting fluorescence intensity redistribution through the analysis of differential image series (red-green detection).
 
 Inspired by [Dovgan et al., 2010](https://pubmed.ncbi.nlm.nih.gov/20704590/) and [Osypenko et al., 2019](https://www.sciencedirect.com/science/article/pii/S0969996119301974?via%3Dihub).
 
 ## Image preprocessing
 Provides functions for preprocessing multi-channel fluorescence acquisitions:
 - If the input image has 4 dimensions (time, channel, x-axis, y-axis), channels will be split into individual 3 dimensions images (time, x-axis, y-axis) with the `_ch%index%` suffix.
 - If the `gaussian blur` option is selected, the image will be blurred with a Gaussian filter using sigma=`gaussian sigma`.
 - If the `photobleaching correction` option is selected, the image will undergo correction with exponential (method `exp`) or bi-exponential (method `bi_exp`) fitting.
+- If the `crop ch` option is selected, only a selected range of channel frames will be saved (corresponding to start and stop indexes from `crop range`).
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_0.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_00.png)
 
 ## Red-green series
 Primary method for detecting fluorescent-labeled targets redistribution in time. Returns a series of differential images representing the intensity difference between the current frame and the previous one as new image with the `_red-green` suffix.
 
 Parameters:
 
 - `left frames` - number of previous frames for pixel-wise averaging.
 - `space frames` - number of frames between the last left and first right frames.
 - `right frames` - number of subsequent frames for pixel-wise averaging.
-- `save mask series` - if selected, a series of labels will be created for each frame of the differential image with the threshold `insertion threshold`.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_1.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_11.png)
 
 ## Up masking
 Generates labels for insertion sites (regions with increasing intensity) based on `-red-green` images. Returns labels layer with `_up-labels` suffix.
 
 Parameters:
 
 - `detection img index` - index of the frame from `-red-green` image used for insertion sites detection.
 - `insertion threshold` - threshold value for insertion site detection, intensity on selected `_red-green` frame normalized in -1 - 0 range.
+- `opening footprint` - footprint size in pixels for mask filtering with morphology opening (disabled if 0).
 - `save mask` - if selected, a total up mask (containing all ROIs) will be created with the `_up-mask` suffix.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_2.png)
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_22.png)
 
 ## Intensity masking
 Extension of __Up Masking__ widget. Detects regions with increasing (`masking mode` - `up`) or decreasing (`masking mode` - `down`) intensity in `-red-green` images. Returns a labels layer with either `_up-labels` or `_down-labels` suffix, depending on the mode.
 
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_33.png)
+
+
+# Traffic monitoring with pH-sensitive tag
+A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
+
+Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
+
+## SEP image preprocessing
+Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). `pH 1st frame` option indicates the 1st frame pH. By default frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
+
+If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+
+The `calc projections` option allows obtaining individual pH series projections (pixel-wise series MIP - pixel-wise series average) for the detection of individual exo/endocytosis events.
 
+
+
+# Intensty profiles building and data frame saving
 ## Individual labels profiles
-Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `raw intensity` is selected) or relative intensities (ΔF/F0).
+Builds a plot with mean intensity profiles for each ROI in `labels` using absolute intensity (if `absolute intensity` is selected) or relative intensities (ΔF/F0).
 
 The `time scale` sets the number of seconds between frames for x-axis scaling.
 
-The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`).
+The baseline intensity for ΔF/F0 profiles is estimated as the mean intensity of the initial profile points (`ΔF win`). You could filter ROIs by minimum and maximum ΔF/F0 amplitudes with the `ΔF aplitude lim` option.
 
-Filters ROIs by minimum (`min amplitude`) and maximum (`max amplitude`) intensity amplitudes.
+_Note: amplitude filtering working with ΔF/F0 profiles only._
 
-_Note: Intensity filtering is most relevant for ΔF/F0 profiles._
+If the `profiles crop` option is selected, only a selected range of intensity profiles indexes will be plotted (corresponding to start and stop indexes from `profiles range`).
 
 Additionally, you can save ROI intensity profiles as .csv using the `save data frame` option and specifying the `saving path`. The output data frames `%img_name%_lab_prof.csv` will contain the following columns:
 
 - __id__ - unique image ID, the name of the input `napari.Image` object.
 - __roi__ - ROI number, consecutively numbered starting from 1.
 - __int__ - ROI mean intensity, raw or ΔF/F0 according to the `raw intensity` option.
 - __index__ - frame index
 - __time__ - frame time point according to the `time scale`.
 
-_Note: The data frame will contain information for all ROIs; filtering options pertain to plotting only._
+_Note: The data frame will contain information for all ROIs; amplitude filtering and crop options pertain to plotting only._
+
+Absolute intensity         | ΔF/F0
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_44.png)|![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_55.png)
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_3.png)
 
-## Labels profile
+## Labels stat profiles
 Builds a plot with the averaged intensity of all ROIs in `labels`. Can take two images (`img 0` and `img 1`) as input if `two profiles` are selected.
 
 The `time scale` and `ΔF win` are the same as in the __Individual Labels Profiles__.
 
-The `stat method` provides methods for calculating intensity errors:
+The `stat method` provides methods for estimation intensity and errors:
 
 - `se` - standard error of mean.
 - `iqr` - interquartile range.
 - `ci` - 95% confidence interval for t-distribution.
 
-![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_4.png)
-
-# Traffic monitoring with pH-sensitive tag
-A collection of widgets designed for the analysis of image series containing the pH-sensitive fluorescence protein Superecliptic pHluorin (SEP).
-
-Insipred by [Fujii et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28474392/), [Gao et al., 2018](https://www.beilstein-journals.org/bjnano/articles/9/79) and [Sposini et al., 2020](https://www.nature.com/articles/s41596-020-0371-z).
-
-## SEP image preprocessing
-Processes image series obtained through repetitive pH exchange methods (such as U-tube or ppH approaches). Frames with odd indexes, including index 0, are interpreted as images acquired at pH 7.0, representing total fluorescence intensity (saved with the suffix `_total`). Even frames are interpreted as images obtained at acidic pH (5.5-6.0), representing intracellular fluorescence only (saved with the suffix `_intra`).
-
-If `calc surface img` is selected, an additional total fluorescence image with subtracted intracellular intensity will be saved as the cell surface fluorescence fraction (suffix `_surface`). The input image should be a 3-dimensional single-channel time-lapse.
+![](https://raw.githubusercontent.com/wisstock/domb-napari/master/images/pic_66.png)
```

