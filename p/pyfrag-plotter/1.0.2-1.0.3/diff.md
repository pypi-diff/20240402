# Comparing `tmp/pyfrag_plotter-1.0.2.tar.gz` & `tmp/pyfrag_plotter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrag_plotter-1.0.2.tar", last modified: Sun Feb 25 10:54:04 2024, max compression
+gzip compressed data, was "pyfrag_plotter-1.0.3.tar", last modified: Tue Apr  2 08:53:17 2024, max compression
```

## Comparing `pyfrag_plotter-1.0.2.tar` & `pyfrag_plotter-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4339 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.622195 pyfrag_plotter-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.622195 pyfrag_plotter-1.0.2/src/pyfrag_plotter/
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/pyfrag_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/read_inputfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/read_resultsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/plot_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/processing_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter/pyfrag_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-25 10:54:04.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-25 10:54:04.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 10:54:04.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 10:54:04.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 10:54:04.000000 pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:54:04.626195 pyfrag_plotter-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/tests/test_get_pyfrag_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/tests/test_processing_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-25 10:53:56.000000 pyfrag_plotter-1.0.2/tests/test_read_inputfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4339 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.495837 pyfrag_plotter-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/src/pyfrag_plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/pyfrag_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/read_inputfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/read_resultsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/plot_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/processing_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter/pyfrag_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-02 08:53:17.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 08:53:17.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:53:17.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 08:53:17.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 08:53:17.000000 pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:53:17.499837 pyfrag_plotter-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/tests/test_get_pyfrag_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/tests/test_processing_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-02 08:53:09.000000 pyfrag_plotter-1.0.3/tests/test_read_inputfile.py
```

### Comparing `pyfrag_plotter-1.0.2/LICENSE.txt` & `pyfrag_plotter-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/PKG-INFO` & `pyfrag_plotter-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrag_plotter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for plotting pyfrag calculations using the AMS driver and plams
 Author-email: Siebe Lekanne Deprez <s.j.lekanne.deprez@vu.nl>
 Maintainer-email: Siebe Lekanne Deprez <s.j.lekanne.deprez@vu.nl>
 License: MIT
 Project-URL: repository, https://github.com/SiebeLeDe/pyfrag_plot
 Project-URL: documentation, https://siebelede.github.io/pyfrag_plot/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyfrag_plotter-1.0.2/README.md` & `pyfrag_plotter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/pyproject.toml` & `pyfrag_plotter-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/__init__.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 from pyfrag_plotter.config.config_handler import Config
 
 # Global variable that contains the config file. It is first empty, but will be filled in the |init| function
 config: Config = Config(cp.ConfigParser())
 
 
 def initialize_pyfrag_plotter(user_config_file: Optional[str] = None) -> None:
-    """Initializes the PyFrag plotter configuration.
+    """
+    Initializes the PyFrag plotter configuration.
 
-    Reads the standard configuration file provided in the module and sets the config as global variable that is read throughout the program.
-    May be overwritten by providing a custom configuration file.
+    This function reads the standard configuration file provided in the module and sets the config as a global variable
+    that is read throughout the program. The standard configuration can be overwritten by providing a custom configuration file.
 
     Args:
-        user_config_file (Optional[str]): The path to a custom configuration file. Defaults to None.
+        user_config_file (Optional[str]): The path to a custom configuration file. If provided, the settings in this file
+        will overwrite the standard configuration. Defaults to None.
 
     Returns:
         None
 
+    Raises:
+        ValueError: If the log level specified in the configuration is invalid.
     """
     global config
 
     # Get the absolute path of the directory one level above the current directory
     current_dir = os.path.abspath(os.path.dirname(__file__))
 
     # Construct the path to the configuration file
@@ -53,18 +57,23 @@
 
     # Initialize the log level and plot parameters
     _initialize_plot_parameters()
     logging.log(logging.INFO, "Initialized PyFrag plotter Succesfully")
 
 
 def _initialize_plot_parameters() -> None:
-    """Applies plot-specific parameters to matplotlib and is called by :func:`pyfrag_plotter.initialize_pyfrag_plotter`.
+    """
+    Applies plot-specific parameters to matplotlib.
 
-    This function sets various parameters for matplotlib, such as the figure size, font family, and font size.
+    This function is called by `initialize_pyfrag_plotter` and sets various parameters for matplotlib, such as the figure size,
+    font family, and font size. It also tries to use the interactive backend for matplotlib, and falls back to the non-interactive
+    backend if the interactive backend is not available.
 
+    Returns:
+        None
     """
     import matplotlib as mpl
 
     # In some occations matplotlib cannot use the interactive backend, so we try to use the non-interactive backend
     try:
         mpl.use("TkAgg")
         import matplotlib.pyplot as plt
```

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/config_handler.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/config_handler.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/config/validate.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/config/validate.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/errors.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/errors.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/pyfrag_files.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/pyfrag_files.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/read_inputfile.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/read_inputfile.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/input/read_resultsfile.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/input/read_resultsfile.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/interpolate.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/interpolate.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 from scipy.interpolate import BSpline, make_interp_spline
 
 from pyfrag_plotter import config
 from pyfrag_plotter.errors import PyFragInterpolationError
 from pyfrag_plotter.pyfrag_object import Array1D, PyFragResultsObject
 
 
-def interpolate_plot(x_axis: np.ndarray, y_axis: np.ndarray, x_range: Optional[Sequence[float]] = None) -> Tuple[np.ndarray, BSpline]:
+def interpolate_plot(x_axis: np.ndarray, y_axis: np.ndarray, x_range: Optional[Sequence[float]] = None) -> Union[Tuple[np.ndarray, BSpline], Tuple[np.ndarray, np.ndarray]]:
     """
     Interpolates the data to a finer grid for plotting purposes using the scipy spline library.
 
     Args:
         x_axis (np.ndarray): The x-axis data to interpolate.
         y_axis (np.ndarray): The y-axis data to interpolate.
         x_range (Optional[Sequence[float]], optional): The range of x-axis values to interpolate over. Defaults to None.
 
     Returns:
         Tuple[np.ndarray, BSpline]: The interpolated x-axis and y-axis data.
     """
     n_interpolation_points = config.get("SHARED", "n_interpolation_points")
     reverse_axis = config.get("SHARED", "reverse_x_axis")
+
+    # This option is used to disable interpolation, which is useful for non-strictly increasing (of decreasing) data
+    if n_interpolation_points == 0:
+        return x_axis, y_axis
+
     if x_range is None:
         x_min, x_max = x_axis.min(), x_axis.max()
     else:
         x_min, x_max = x_range[0], x_range[1]
 
     mask = (x_axis >= x_min) & (x_axis <= x_max)
     x_filtered = x_axis[mask] if not reverse_axis else x_axis[mask][::-1]
```

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/plot_details.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/plot_details.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,26 +51,35 @@
     fig: Optional[matplotlib.figure.Figure] = None,
     title: Optional[str] = None,
     savefig: Optional[str] = None,
     show_plot: bool = False,
     clear_plot: bool = False,
     tight_layout: bool = True,
 ) -> None:
-    """Specifies figure options for making a shorter and cleaner code.
+    """
+    Modifies the provided figure according to the specified options.
+
+    This function can remove empty subplots, adjust layout, add a title, save the figure to a file,
+    display the plot, and clear the plot.
 
     Args:
-        fig (Optional[matplotlib.figure.Figure], optional): The figure to modify. Defaults to None.
-        title (Optional[str], optional): The title of the figure. Defaults to None.
-        savefig (Optional[str], optional): The filename to save the figure to. Defaults to None.
-        show_plot (bool, optional): Whether to show the plot. Defaults to False.
-        clear_plot (bool, optional): Whether to clear the plot. Defaults to False.
-        tight_layout (bool, optional): Whether to use tight layout. Defaults to True.
+        fig (Optional[matplotlib.figure.Figure], optional): The figure to modify. If None, the current figure is used. Defaults to None.
+        title (Optional[str], optional): The title of the figure. If provided, it is added to the figure. Defaults to None.
+        savefig (Optional[str], optional): The filename to save the figure to. If provided, the figure is saved as a .png file. Defaults to None.
+        show_plot (bool, optional): Whether to display the plot. If True, the plot is displayed. Defaults to False.
+        clear_plot (bool, optional): Whether to clear the plot. If True, the current plot is cleared. Defaults to False.
+        tight_layout (bool, optional): Whether to adjust the padding between and around the subplots. If True, the padding is adjusted. Defaults to True.
     """
     fig = plt.gcf() if fig is None else fig
 
+    # Removes the empty axes from the figure
+    for ax in fig.axes:
+        if not ax.lines and not ax.patches:
+            fig.delaxes(ax)
+
     # Fixes the large padding between the axes and the labels of the axes
     if tight_layout:
         fig.tight_layout()
 
     # Adds a title to the figure
     if title is not None:
         fig.suptitle(title, fontweight="bold", y=1.00)
@@ -92,30 +101,34 @@
     x_label: str = r"$\Delta$r / \u00c5",
     y_label: str = r"$\Delta\it{E}$ / kcal mol$^{-1}$",  # type: ignore # noqa: W605 since it is a LaTeX string
     y_lim: Optional[Tuple[float, float]] = None,
     n_max_x_ticks: int = 6,
     n_max_y_ticks: int = 5,
     plot_legend: bool = True,
     line_style_labels: Optional[Sequence[str]] = None,
-    title: str | None = None,
+    title: Optional[str] = None,
     vline: float = 0.0,
 ) -> None:
-    r"""Specifies axes options for making a shorter and cleaner code.
+    r"""
+    Specifies axes options for making a shorter and cleaner code.
+
+    This function modifies the provided axes according to the specified options. It sets the labels, limits, ticks,
+    title, and line styles of the axes. It also draws a vertical line at a specified x-coordinate and a horizontal line at y=0.
 
     Args:
-        ax (Optional[plt.Axes], optional): The axes to modify. Defaults to None.
+        ax (Optional[plt.Axes], optional): The axes to modify. If None, the current axes is used. Defaults to None.
         x_label (str, optional): The label for the x-axis. Defaults to "$\Delta$ r / A" (dr / A).
         y_label (str, optional): The label for the y-axis. Defaults to "$\Delta \it{E}$ / kcal mol$^{-1}$" (dE / kcal mol-1).
-        y_lim (Optional[Tuple[float, float]], optional): The y-axis limits. Defaults to None.
+        y_lim (Optional[Tuple[float, float]], optional): The y-axis limits. If None, the default y-axis limits are used. Defaults to None.
         n_max_x_ticks (int, optional): The maximum number of x-axis ticks. Defaults to 6.
         n_max_y_ticks (int, optional): The maximum number of y-axis ticks. Defaults to 5.
-        plot_legend (bool, optional): Whether to plot the legend. Defaults to True.
-        line_style_labels (Optional[Sequence[str]], optional): The legend for the line styles. Defaults to None.
-        title (str, optional): The title of the subplot. Defaults to "".
-        vline (float, optional): The x-coordinate of the vertical line. Defaults to 0.0.
+        plot_legend (bool, optional): Whether to plot the legend. If True, a legend is plotted. Defaults to True.
+        line_style_labels (Optional[Sequence[str]], optional): The labels for the line styles. If provided, these labels are used in the legend. Defaults to None.
+        title (str | None, optional): The title of the subplot. If provided, this title is set. Defaults to None.
+        vline (float | None, optional): The x-coordinate of the vertical line. If provided, a vertical line is drawn at this x-coordinate. Defaults to 0.0.
     """
     ax = plt.gca() if ax is None else ax
 
     # Plot labels
     ax.set_xlabel(x_label, labelpad=20)
     ax.set_ylabel(y_label, labelpad=20)
 
@@ -143,37 +156,38 @@
     for line in ax.lines:
         x, y = line.get_data()
         X_, Y_ = interpolate_plot(x, y)
         line.set_data(X_, Y_)
 
     # Draws a vertical line at the specified point
     # First check for user input, else check for config file input
-    vline = config.get("SHARED", "vline") if math.isclose(vline, 0.0) else vline
-    ax.vlines(
-        vline,
-        ax.get_ylim()[0],
-        ax.get_ylim()[1],
-        colors=["grey"],
-        linestyles="dashed",
-    )
+    vline = config.get("SHARED", "vline") if vline is None else vline
+    if not math.isclose(vline, 0.0):
+        ax.vlines(
+            vline,
+            ax.get_ylim()[0],
+            ax.get_ylim()[1],
+            colors=["grey"],
+            linestyles="dashed",
+        )
 
     # Draws a horizontal line at y=0 (indicating the 'zero line')
     ax.hlines(0, ax.get_xlim()[0], ax.get_xlim()[1], colors=["grey"], linewidth=0.2)
 
     # Set the y-axis formatter to round to one decimal place
     ax.xaxis.set_major_formatter(FormatStrFormatter("%.1f"))
     ax.yaxis.set_major_formatter(FormatStrFormatter("%.1f"))
 
     # Axes adjustments: tick markers and number of ticks
     ax.tick_params(which="both", width=1.5)
     ax.tick_params(which="major", length=7)
 
     ax.xaxis.set_major_locator(MaxNLocator(n_max_x_ticks))
     # ax.yaxis.set_major_locator(MaxNLocator(n_max_y_ticks))
-    ax.set_yticks(np.linspace(ax.get_ylim()[0], ax.get_ylim()[1], 5))
+    ax.set_yticks(np.linspace(ax.get_ylim()[0], ax.get_ylim()[1], n_max_y_ticks))
 
     # Removes the top en right border of the graph
     ax.spines["top"].set_visible(False)
     ax.spines["right"].set_visible(False)
 
     # Makes the x and y axis wider
     ax.spines["left"].set_linewidth(1.5)
```

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/plot/plotter.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/plot/plotter.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,61 +43,82 @@
     irc_coord_label: str
     colours: List[str] = field(factory=lambda: config.get("SHARED", "colours"))
     line_styles: List[str] = field(factory=lambda: config.get("SHARED", "line_styles"))
     peak_type: Optional[str] = field(factory=lambda: config.get("SHARED", "stat_point_type") if config.get("SHARED", "stat_point_type") != "none" else None)
 
 
 class Plotter:
-    """Main class for plotting the results of the PyFrag calculations.
+    """
+    This class provides methods for plotting the results of the PyFrag calculations. It supports plotting of activation
+    strain model terms, energy decomposition terms, and extra strain terms. The plots are saved to a specified directory.
+
+    Additionally, the "standard_plot_routine" method can be used to plot any key (or a combination of) in the PyFragResultsObject and the user may create specicifed functions using this method.
 
     Attributes:
         name (str): The name of the plotter object.
-        objects (Sequence[PyFragResultsObject]): A list of PyFragResultsObject objects.
+        objects (Sequence[PyFragResultsObject]): A list of PyFragResultsObject objects that contain the data to be plotted.
         path (str): The directory to save the plots to.
-        plot_info (PlotInfo): An instance of the PlotInfo class.
+        plot_info (PlotInfo): An instance of the PlotInfo class that contains information about the plot, such as the
+                            line styles and colors.
 
     Note: The plotter object can be used with a "with" statement to ensure that the plot directory is removed if it's empty.
     """
 
     def __init__(self, name: str, plot_dir: str, pyfrag_objects: Sequence[PyFragResultsObject], irc_coord: Sequence[str]):
+        """
+        Initializes the Plotter object.
+
+        Args:
+            name (str): The name of the plotter object.
+            plot_dir (str): The directory to save the plots to.
+            pyfrag_objects (Sequence[PyFragResultsObject]): A list of PyFragResultsObject objects that contain the data to be plotted.
+            irc_coord (Sequence[str]): A sequence of two strings that specify the IRC coordinate and its label.
+        """
         self.name = name
         self.objects = pyfrag_objects
         self.path = opj(plot_dir, name)
         self.plot_info = PlotInfo(irc_coord=irc_coord[0], irc_coord_label=irc_coord[1])
 
     def __enter__(self):
-        """For using the class with an "with" statment.
+        """
+        Prepares the plotter object for use with a "with" statement.
 
-        It checks if the specified directory exists for making plots.
-        If not, creates it (and any parent directories).
+        This method checks if the specified directory exists for making plots. If not, it creates it (and any parent directories).
         """
         if not os.path.isdir(self.path):
             os.makedirs(self.path)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        """Makes sure to close the plotter object and remove the plot directory if it's empty."""
+        """
+        Cleans up the plotter object after use with a "with" statement.
+
+        This method makes sure to close the plotter object and remove the plot directory if it's empty.
+        """
         for root, dirs, files in os.walk(self.path, topdown=False):
             for dir in dirs:
                 dir_path = os.path.join(root, dir)
                 if len(os.listdir(dir_path)) == 0:
                     os.rmdir(dir_path)
 
     # ------------------------------------------------------------------------------------------------------------- #
     # ------------------------------ ASM, EDA and ASM extra strain plotting routines ------------------------------ #
     # ------------------------------------------------------------------------------------------------------------- #
 
     def standard_plot_routine(self, keys: Sequence[str], ax: Optional[plt.Axes] = None, markers: Optional[Sequence[str]] = None):
-        """The plot routine for the EDA, ASM and extra strain plots.
+        """
+        The standard plot routine for the EDA, ASM and extra strain plots.
 
-        Args:
-            plot_key (str): The type of plot to make (eda, asm or extra_strain).
-            keys (list[str]): The keys to plot that should match the keys in the corresponding dictionary type (asm, eda or extra_strain).
-            ax (Optional[plt.Axes], optional): The axes to plot on. Defaults to None.
+        This method plots the specified keys for each PyFragResultsObject in the plotter. It supports plotting of multiple keys
+        on the same axes, and allows for customization of the line styles and markers.
 
+        Args:
+            keys (Sequence[str]): The keys to plot. These should match the keys in the corresponding dictionary type (asm, eda or extra_strain).
+            ax (Optional[plt.Axes], optional): The axes to plot on. If None, the current axes is used. Defaults to None.
+            markers (Optional[Sequence[str]], optional): The markers to use for the lines. If None, no markers are used. Defaults to None.
         """
         ax = plt.gca() if ax is None else ax
         markers = [""] * len(self.objects) if markers is None else markers
 
         x_axes = [obj.get_x_axis(self.plot_info.irc_coord) for obj in self.objects]
         for i, (line_style, term) in enumerate(zip(self.plot_info.line_styles, keys)):
             for x_axis, colour, obj, line_marker in zip(x_axes, self.plot_info.colours, self.objects, markers):
@@ -112,25 +133,27 @@
 
                 # If a peak type is specified, plot the peak
                 if i == 0 and self.plot_info.peak_type is not None:
                     peak_index = obj.get_peak_index(peak=self.plot_info.peak_type)
                     ax.scatter(x_axis[peak_index], term_data[peak_index], color=colour, s=90, zorder=2)
 
     @plot_logger()
-    def plot_asm(self, keys: Optional[List[str]] = None, **kwargs):
-        """Plots the activation strain model terms. The user can specify which terms to plot, otherwise all of them are plotted.
+    def plot_asm(self, keys: Optional[List[str]] = None, **kwargs) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        Plots the activation strain model terms.
+
+        This method plots the specified ASM terms for each PyFragResultsObject in the plotter. If no terms are specified, all terms are plotted.
 
         Args:
-            keys (Optional[List[str]], optional): Keys that are plotted. Defaults to None (plot all keys).
-            **kwargs: Additional keyword arguments to pass to the function.
+            keys (Optional[List[str]], optional): The ASM terms to plot. If None, all terms are plotted. Defaults to None.
+            **kwargs: Additional keyword arguments to pass to the `set_axes_details` and `set_figure_details` functions.
 
         Returns:
             fig (plt.Figure): The figure object.
             ax (plt.Axes): The axes object.
-
         """
         fig = plt.figure()
         ax = fig.add_subplot(111)
 
         # Get the keys to plot. If none are specified, plot all of them
         if keys is None:
             asm_keys: List[str] = config.get("ASM", "asm_keys")
@@ -145,19 +168,23 @@
 
         # Set the key-specific plot details
         set_axes_details(ax=ax, x_label=self.plot_info.irc_coord_label, line_style_labels=labels, **kwargs)
         set_figure_details(fig=fig, title=f"ASM_{'_'.join(asm_keys)}", savefig=opj(self.path, f"ASM_{'_'.join(asm_keys)}.png"), line_style_labels=labels, **kwargs)
         return fig, ax
 
     @plot_logger()
-    def plot_eda(self, keys: Optional[List[str]] = None, **kwargs):
-        """Plots the energy decomposition terms. The user can specify which terms to plot, otherwise all of them are plotted.
+    def plot_eda(self, keys: Optional[List[str]] = None, **kwargs) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        Plots the energy decomposition terms.
+
+        This method plots the specified EDA terms for each PyFragResultsObject in the plotter. If no terms are specified, all terms are plotted.
 
         Args:
-            keys (Optional[List[str]], optional): Keys that are plotted. Defaults to None (plot all keys).
+            keys (Optional[List[str]], optional): The EDA terms to plot. If None, all terms are plotted. Defaults to None.
+            **kwargs: Additional keyword arguments to pass to the `set_axes_details` and `set_figure_details` functions.
 
         Returns:
             fig (plt.Figure): The figure object.
             ax (plt.Axes): The axes object.
         """
         fig = plt.figure()
         ax = fig.add_subplot(111)
@@ -175,23 +202,31 @@
 
         # Set the key-specific plot details
         set_axes_details(ax=ax, x_label=self.plot_info.irc_coord_label, line_style_labels=labels, **kwargs)
         set_figure_details(fig=fig, title=f"EDA_{'_'.join(eda_keys)}", savefig=opj(self.path, f"EDA_{'_'.join(eda_keys)}.png"), **kwargs)
         return fig, ax
 
     @plot_logger()
-    def plot_extra_strain(self, keys: Optional[List[str]] = None, **kwargs):
-        """Plots the extra strain terms. The user can specify which terms to plot, otherwise all of them are plotted.
+    def plot_extra_strain(self, keys: Optional[List[str]] = None, **kwargs) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        Plots the extra strain terms.
+
+        This method plots the specified extra strain terms for each PyFragResultsObject in the plotter. If no terms are specified,
+        all terms are plotted. The plot is saved to the plot directory with a filename that includes the plotted terms.
 
         Args:
-            keys (Optional[List[str]], optional): Keys that are plotted. Defaults to None (plot all keys).
+            keys (Optional[List[str]], optional): The extra strain terms to plot. If None, all terms are plotted. Defaults to None.
+            **kwargs: Additional keyword arguments to pass to the `set_axes_details` and `set_figure_details` functions.
 
         Returns:
             fig (plt.Figure): The figure object.
             ax (plt.Axes): The axes object.
+
+        Raises:
+            ValueError: If any of the specified keys do not exist in the extra strain dictionary.
         """
         fig = plt.figure()
         ax = fig.add_subplot(111)
 
         # Get the keys to plot. If none are specified, plot all of them
         if keys is None:
             extra_strain_keys: List[str] = config.get("ASM", "asm_strain_keys")
@@ -248,25 +283,32 @@
 
         # # Set the plot details
         # set_plot_details(savefig=opj(self.path, "population.png"),
         #                 title="Population",
         #                 x_label=self.plot_info.irc_coord_label)
 
     @plot_logger()
-    def plot_arbitrary_keys(self, title: str, keys: List[str], **kwargs):
-        """Arbitrary plotting function for plotting any key (or a combination of) in the PyFragResultsObject object.
+    def plot_arbitrary_keys(self, title: str, keys: List[str], **kwargs) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        Arbitrary plotting function for plotting any key (or a combination of) in the PyFragResultsObject object.
+
+        This method plots the specified keys for each PyFragResultsObject in the plotter. The plot is saved to the plot directory
+        with a filename that includes the plotted keys. The plot title and other figure and axes details can be customized.
 
         Args:
-            keys (Optional[List[str]], optional): Keys that are plotted. Defaults to None (plot all keys).
-            **kwargs: Additional keyword arguments to pass to the function.
+            title (str): The title of the plot.
+            keys (List[str]): The keys to plot. These should match the keys in the corresponding dictionary type (asm, eda or extra_strain).
+            **kwargs: Additional keyword arguments to pass to the `set_axes_details` and `set_figure_details` functions.
 
         Returns:
             fig (plt.Figure): The figure object.
             ax (plt.Axes): The axes object.
 
+        Raises:
+            ValueError: If any of the specified keys do not exist in the dictionaries of the PyFragResultsObject objects.
         """
         fig = plt.figure()
         ax = fig.add_subplot(111)
 
         self.standard_plot_routine(keys, ax)
 
         labels = self.objects[0].get_plot_labels(keys)
```

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/processing_funcs.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/processing_funcs.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter/pyfrag_object.py` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter/pyfrag_object.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/PKG-INFO` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrag_plotter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for plotting pyfrag calculations using the AMS driver and plams
 Author-email: Siebe Lekanne Deprez <s.j.lekanne.deprez@vu.nl>
 Maintainer-email: Siebe Lekanne Deprez <s.j.lekanne.deprez@vu.nl>
 License: MIT
 Project-URL: repository, https://github.com/SiebeLeDe/pyfrag_plot
 Project-URL: documentation, https://siebelede.github.io/pyfrag_plot/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyfrag_plotter-1.0.2/src/pyfrag_plotter.egg-info/SOURCES.txt` & `pyfrag_plotter-1.0.3/src/pyfrag_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/tests/test_config.py` & `pyfrag_plotter-1.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/tests/test_get_pyfrag_files.py` & `pyfrag_plotter-1.0.3/tests/test_get_pyfrag_files.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/tests/test_processing_data.py` & `pyfrag_plotter-1.0.3/tests/test_processing_data.py`

 * *Files identical despite different names*

### Comparing `pyfrag_plotter-1.0.2/tests/test_read_inputfile.py` & `pyfrag_plotter-1.0.3/tests/test_read_inputfile.py`

 * *Files identical despite different names*

