# Comparing `tmp/AstroToolkit-1.3.3.tar.gz` & `tmp/AstroToolkit-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroToolkit-1.3.3.tar", last modified: Fri Mar 29 18:19:49 2024, max compression
+gzip compressed data, was "AstroToolkit-1.3.4.tar", last modified: Sun Mar 31 10:50:05 2024, max compression
```

## Comparing `AstroToolkit-1.3.3.tar` & `AstroToolkit-1.3.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.633625 AstroToolkit-1.3.3/
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 AstroToolkit-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    39225 2024-03-29 18:19:49.632625 AstroToolkit-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    38214 2024-03-24 21:49:15.000000 AstroToolkit-1.3.3/README.md
--rw-rw-rw-   0        0        0     1034 2024-03-29 18:19:19.000000 AstroToolkit-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 18:19:49.634625 AstroToolkit-1.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.489592 AstroToolkit-1.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.498595 AstroToolkit-1.3.3/src/AstroToolkit/
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.588616 AstroToolkit-1.3.3/src/AstroToolkit/Data/
--rw-rw-rw-   0        0        0    14952 2024-03-28 11:05:05.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/data.py
--rw-rw-rw-   0        0        0     6292 2024-03-24 13:18:55.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/imaging.py
--rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/lightcurve_sigma_clip.py
--rw-rw-rw-   0        0        0    23068 2024-03-25 11:41:13.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/lightcurves.py
--rw-rw-rw-   0        0        0    10503 2024-03-24 13:13:06.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/overlays.py
--rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/photometry.py
--rw-rw-rw-   0        0        0     2534 2024-03-24 15:05:20.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/reddening.py
--rw-rw-rw-   0        0        0     4300 2024-01-18 17:10:19.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/sed.py
--rw-rw-rw-   0        0        0     1974 2024-03-29 17:46:17.000000 AstroToolkit-1.3.3/src/AstroToolkit/Data/spectra.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.592616 AstroToolkit-1.3.3/src/AstroToolkit/Datapages/
--rw-rw-rw-   0        0        0     2747 2024-01-17 22:56:29.000000 AstroToolkit-1.3.3/src/AstroToolkit/Datapages/buttons.py
--rw-rw-rw-   0        0        0     3785 2024-03-24 00:14:23.000000 AstroToolkit-1.3.3/src/AstroToolkit/Datapages/grid.py
--rw-rw-rw-   0        0        0     8232 2024-01-17 22:58:42.000000 AstroToolkit-1.3.3/src/AstroToolkit/Datapages/metadata.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.593616 AstroToolkit-1.3.3/src/AstroToolkit/Examples/
--rw-rw-rw-   0        0        0     3135 2024-03-24 00:18:21.000000 AstroToolkit-1.3.3/src/AstroToolkit/Examples/datapage_creation.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.601617 AstroToolkit-1.3.3/src/AstroToolkit/Misc/
--rw-rw-rw-   0        0        0     2388 2024-02-07 17:32:05.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/ProperMotionCorrection.py
--rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/coord_conversion.py
--rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/file_handling.py
--rw-rw-rw-   0        0        0     4207 2024-03-24 13:13:35.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/file_naming.py
--rw-rw-rw-   0        0        0     2764 2024-03-09 16:01:36.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/input_validation.py
--rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 AstroToolkit-1.3.3/src/AstroToolkit/Misc/read_fits.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.610620 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/
--rw-rw-rw-   0        0        0     4600 2024-03-28 15:23:03.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/HRD.py
--rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
--rw-rw-rw-   0        0        0     4576 2024-03-24 13:19:53.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/imaging.py
--rw-rw-rw-   0        0        0     5609 2024-03-23 23:37:51.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/lightcurves.py
--rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/powspec.py
--rw-rw-rw-   0        0        0     2629 2024-02-27 18:54:15.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/sed.py
--rw-rw-rw-   0        0        0     3676 2024-03-23 22:29:45.000000 AstroToolkit-1.3.3/src/AstroToolkit/Plotting/spectra.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.611620 AstroToolkit-1.3.3/src/AstroToolkit/Settings/
--rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 AstroToolkit-1.3.3/src/AstroToolkit/Settings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.628624 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/
--rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/README - Windows.txt
--rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/README.txt
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/__init__.py
--rw-rw-rw-   0        0        0   167936 2024-01-14 17:57:05.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aov.f90
--rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aovconst.f90
--rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aovsub.f90
--rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/build.sh
--rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/buildwin.bat
--rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/pyaov.pdf
--rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/pyaov.py
--rw-rw-rw-   0        0        0    31562 2024-02-03 22:59:58.000000 AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/ztfanalysis.py
--rw-rw-rw-   0        0        0    33163 2024-03-29 18:07:32.000000 AstroToolkit-1.3.3/src/AstroToolkit/Tools.py
-drwxrwxrwx   0        0        0        0 2024-03-29 18:19:49.631625 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/
--rw-rw-rw-   0        0        0    39225 2024-03-29 18:19:49.000000 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1784 2024-03-29 18:19:49.000000 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 18:19:49.000000 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2024-03-29 18:19:49.000000 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-29 18:19:49.000000 AstroToolkit-1.3.3/src/AstroToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.630785 AstroToolkit-1.3.4/
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 AstroToolkit-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    39258 2024-03-31 10:50:05.629784 AstroToolkit-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    38214 2024-03-24 21:49:15.000000 AstroToolkit-1.3.4/README.md
+-rw-rw-rw-   0        0        0     1058 2024-03-31 10:47:21.000000 AstroToolkit-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-31 10:50:05.630785 AstroToolkit-1.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.483751 AstroToolkit-1.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.500756 AstroToolkit-1.3.4/src/AstroToolkit/
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.587775 AstroToolkit-1.3.4/src/AstroToolkit/Data/
+-rw-rw-rw-   0        0        0    14952 2024-03-28 11:05:05.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/data.py
+-rw-rw-rw-   0        0        0     6292 2024-03-24 13:18:55.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/imaging.py
+-rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/lightcurve_sigma_clip.py
+-rw-rw-rw-   0        0        0    23058 2024-03-30 19:21:54.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/lightcurves.py
+-rw-rw-rw-   0        0        0    10503 2024-03-24 13:13:06.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/overlays.py
+-rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/photometry.py
+-rw-rw-rw-   0        0        0     2534 2024-03-24 15:05:20.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/reddening.py
+-rw-rw-rw-   0        0        0     4300 2024-01-18 17:10:19.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/sed.py
+-rw-rw-rw-   0        0        0     1974 2024-03-29 17:46:17.000000 AstroToolkit-1.3.4/src/AstroToolkit/Data/spectra.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.592777 AstroToolkit-1.3.4/src/AstroToolkit/Datapages/
+-rw-rw-rw-   0        0        0     2747 2024-01-17 22:56:29.000000 AstroToolkit-1.3.4/src/AstroToolkit/Datapages/buttons.py
+-rw-rw-rw-   0        0        0     3785 2024-03-24 00:14:23.000000 AstroToolkit-1.3.4/src/AstroToolkit/Datapages/grid.py
+-rw-rw-rw-   0        0        0     8232 2024-01-17 22:58:42.000000 AstroToolkit-1.3.4/src/AstroToolkit/Datapages/metadata.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.593777 AstroToolkit-1.3.4/src/AstroToolkit/Examples/
+-rw-rw-rw-   0        0        0     3135 2024-03-24 00:18:21.000000 AstroToolkit-1.3.4/src/AstroToolkit/Examples/datapage_creation.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.599778 AstroToolkit-1.3.4/src/AstroToolkit/Misc/
+-rw-rw-rw-   0        0        0     2388 2024-02-07 17:32:05.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/ProperMotionCorrection.py
+-rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/coord_conversion.py
+-rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/file_handling.py
+-rw-rw-rw-   0        0        0     4207 2024-03-24 13:13:35.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/file_naming.py
+-rw-rw-rw-   0        0        0     2764 2024-03-09 16:01:36.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/input_validation.py
+-rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 AstroToolkit-1.3.4/src/AstroToolkit/Misc/read_fits.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.612781 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/
+-rw-rw-rw-   0        0        0     4600 2024-03-28 15:23:03.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/HRD.py
+-rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
+-rw-rw-rw-   0        0        0     4576 2024-03-24 13:19:53.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/imaging.py
+-rw-rw-rw-   0        0        0     5609 2024-03-23 23:37:51.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/lightcurves.py
+-rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/powspec.py
+-rw-rw-rw-   0        0        0     2629 2024-02-27 18:54:15.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/sed.py
+-rw-rw-rw-   0        0        0     3676 2024-03-23 22:29:45.000000 AstroToolkit-1.3.4/src/AstroToolkit/Plotting/spectra.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.613782 AstroToolkit-1.3.4/src/AstroToolkit/Settings/
+-rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 AstroToolkit-1.3.4/src/AstroToolkit/Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.627784 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/
+-rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/README - Windows.txt
+-rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/README.txt
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/__init__.py
+-rw-rw-rw-   0        0        0   167936 2024-01-14 17:57:05.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aov.f90
+-rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aovconst.f90
+-rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aovsub.f90
+-rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/build.sh
+-rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/buildwin.bat
+-rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/pyaov.pdf
+-rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/pyaov.py
+-rw-rw-rw-   0        0        0    31562 2024-02-03 22:59:58.000000 AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/ztfanalysis.py
+-rw-rw-rw-   0        0        0    33153 2024-03-31 10:44:09.000000 AstroToolkit-1.3.4/src/AstroToolkit/Tools.py
+drwxrwxrwx   0        0        0        0 2024-03-31 10:50:05.628784 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/
+-rw-rw-rw-   0        0        0    39258 2024-03-31 10:50:05.000000 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1784 2024-03-31 10:50:05.000000 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-31 10:50:05.000000 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2024-03-31 10:50:05.000000 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-31 10:50:05.000000 AstroToolkit-1.3.4/src/AstroToolkit.egg-info/top_level.txt
```

### Comparing `AstroToolkit-1.3.3/PKG-INFO` & `AstroToolkit-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroToolkit
-Version: 1.3.3
+Version: 1.3.4
 Summary: A package for the gathering and plotting of astronomical data.
 Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
 Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -21,14 +21,15 @@
 Requires-Dist: pandas==2.0.3
 Requires-Dist: Pillow==10.2.0
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: PyQt5_sip==12.13.0
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn==1.3.2
 Requires-Dist: scipy==1.10.1
+Requires-Dist: selenium==4.17.2
 
 # AstroToolkit
 
 AstroToolkit (ATK) is a set of useful tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
```

### Comparing `AstroToolkit-1.3.3/README.md` & `AstroToolkit-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/pyproject.toml` & `AstroToolkit-1.3.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "AstroToolkit"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
   { name="Ethan Moorfield", email="ethan.moorfield@hotmail.co.uk"},
 ]
 description = "A package for the gathering and plotting of astronomical data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -30,12 +30,13 @@
     "pandas==2.0.3",
     "Pillow==10.2.0",
     "PyQt5==5.15.10",
     "PyQt5_sip==12.13.0",
     "Requests==2.31.0",
     "scikit_learn==1.3.2",
     "scipy==1.10.1",
+    "selenium==4.17.2"
 ]
 
 [project.urls]
 Homepage = "https://github.com/WD-planets/AstroToolkit"
 Issues = "https://github.com/WD-planets/AstroToolkit/issues"
```

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/data.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/data.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/imaging.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/imaging.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/lightcurve_sigma_clip.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/lightcurve_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/lightcurves.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/lightcurves.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,15 @@
 		r=requests.post(url=f'{base_url}/api-token-auth/',data={'username':username,'password':password})
 
 		if r.status_code==200:
 			token=r.json()['token']
 			headers={'Authorization':f'Token {token}','Accept':'application/json'}
 			
 		else:
-			print(f'ERROR {r.status_code}.')
-			print(r.json())
+			print(f'Note: Experiencing issues with ATLAS')
 			return f_return
 			
 		task_url=None
 		while not task_url:
 			with requests.Session() as s:
 				if do_correction==True:
 					# mjd = 57174 is June 1st 2015, which is noted on the site as the start of ATLAS observations. Use 60096 for testing (~6 months at time of writing)
@@ -216,17 +215,16 @@
 						waittime=int(t_min[0])
 					else:
 						waittime=10
 					
 					print(f'Waiting {waittime} seconds.')
 					time.sleep(waittime)
 				else:
-					print(f'ERROR {r.status_code}')
-					print(r.json())
-					sys.exit()
+					print(f'Note: Experiencing issues with ATLAS')
+					return f_return
 					
 		result_url=None
 		while not result_url:
 			with requests.Session() as s:
 				r=s.get(task_url,headers=headers)
 				
 				if r.status_code==200:
@@ -237,17 +235,16 @@
 					elif r.json()['starttimestamp']:
 						print(f"Task is running (started at {r.json()['starttimestamp']})")
 					else:
 						print('Waiting for job to start. Checking again in 10 seconds...')
 					time.sleep(10)
 				
 				else:
-					print(f'ERROR {r.status_code}')
-					print(r.json())
-					sys.exit()
+					print(f'Note: Experiencing issues with ATLAS')
+					return f_return
 					
 		with requests.Session() as s:
 			textdata=s.get(result_url,headers=headers).text
 			#s.delete(task_url,headers=headers).json()
 
 		df=pd.read_csv(io.StringIO(textdata.replace('###','')),delim_whitespace=True)
```

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/overlays.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/overlays.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/photometry.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/photometry.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/reddening.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/reddening.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/sed.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/sed.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Data/spectra.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Data/spectra.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Datapages/buttons.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Datapages/buttons.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Datapages/grid.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Datapages/grid.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Datapages/metadata.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Datapages/metadata.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Examples/datapage_creation.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Examples/datapage_creation.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/ProperMotionCorrection.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/ProperMotionCorrection.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/coord_conversion.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/coord_conversion.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/file_handling.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/file_handling.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/file_naming.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/file_naming.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/input_validation.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/input_validation.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Misc/read_fits.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Misc/read_fits.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/HRD.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/HRD.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/imaging.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/imaging.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/lightcurves.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/lightcurves.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/powspec.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/powspec.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/sed.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/sed.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Plotting/spectra.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Plotting/spectra.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/README - Windows.txt` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/README - Windows.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/README.txt` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/README.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aov.f90` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aov.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aovconst.f90` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aovconst.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/aovsub.f90` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/aovsub.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/build.sh` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/build.sh`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/buildwin.bat` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/buildwin.bat`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/pyaov.pdf` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/pyaov.pdf`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/pyaov.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/pyaov.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Timeseries/ztfanalysis.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Timeseries/ztfanalysis.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit/Tools.py` & `AstroToolkit-1.3.4/src/AstroToolkit/Tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 '''
 Changelog:
-- Small changes to HRD overlay layering
-- updated to work with astroquery 0.4.7
-- bug fixes
+- Minor ATLAS error handling improvements
+- fixed dependencies in requirements.txt
 '''
 
 '''
 To-Do:
 HIGH PRIORITY
 - specify versions in requirements
 - check config for if all keys are present, if not then make a new config file with current keys saved
```

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit.egg-info/PKG-INFO` & `AstroToolkit-1.3.4/src/AstroToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroToolkit
-Version: 1.3.3
+Version: 1.3.4
 Summary: A package for the gathering and plotting of astronomical data.
 Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
 Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -21,14 +21,15 @@
 Requires-Dist: pandas==2.0.3
 Requires-Dist: Pillow==10.2.0
 Requires-Dist: PyQt5==5.15.10
 Requires-Dist: PyQt5_sip==12.13.0
 Requires-Dist: Requests==2.31.0
 Requires-Dist: scikit_learn==1.3.2
 Requires-Dist: scipy==1.10.1
+Requires-Dist: selenium==4.17.2
 
 # AstroToolkit
 
 AstroToolkit (ATK) is a set of useful tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
```

### Comparing `AstroToolkit-1.3.3/src/AstroToolkit.egg-info/SOURCES.txt` & `AstroToolkit-1.3.4/src/AstroToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

