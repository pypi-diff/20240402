# Comparing `tmp/pandas-plots-0.9.6.tar.gz` & `tmp/pandas-plots-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-plots-0.9.6.tar", last modified: Sun Mar 24 16:35:59 2024, max compression
+gzip compressed data, was "pandas-plots-0.9.7.tar", last modified: Tue Apr  2 12:00:41 2024, max compression
```

## Comparing `pandas-plots-0.9.6.tar` & `pandas-plots-0.9.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-03-24 16:35:59.818195 pandas-plots-0.9.6/
--rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.6/LICENSE
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-03-24 16:35:59.818121 pandas-plots-0.9.6/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.6/README.md
--rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.6/pyproject.toml
--rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-03-24 16:35:59.818465 pandas-plots-0.9.6/setup.cfg
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-03-24 16:35:59.814168 pandas-plots-0.9.6/src/
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-03-24 16:35:59.816361 pandas-plots-0.9.6/src/pandas_plots/
--rw-r--r--   0 dexter     (501) staff       (20)     6838 2024-03-23 21:38:50.000000 pandas-plots-0.9.6/src/pandas_plots/hlp.py
--rw-r--r--   0 dexter     (501) staff       (20)    28501 2024-03-24 09:29:35.000000 pandas-plots-0.9.6/src/pandas_plots/pls.py
--rw-r--r--   0 dexter     (501) staff       (20)    22656 2024-03-24 16:29:18.000000 pandas-plots-0.9.6/src/pandas_plots/tbl.py
--rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.6/src/pandas_plots/ven.py
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-03-24 16:35:59.817797 pandas-plots-0.9.6/src/pandas_plots.egg-info/
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-03-24 16:35:59.000000 pandas-plots-0.9.6/src/pandas_plots.egg-info/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)      337 2024-03-24 16:35:59.000000 pandas-plots-0.9.6/src/pandas_plots.egg-info/SOURCES.txt
--rw-r--r--   0 dexter     (501) staff       (20)        1 2024-03-24 16:35:59.000000 pandas-plots-0.9.6/src/pandas_plots.egg-info/dependency_links.txt
--rw-r--r--   0 dexter     (501) staff       (20)      119 2024-03-24 16:35:59.000000 pandas-plots-0.9.6/src/pandas_plots.egg-info/requires.txt
--rw-r--r--   0 dexter     (501) staff       (20)       13 2024-03-24 16:35:59.000000 pandas-plots-0.9.6/src/pandas_plots.egg-info/top_level.txt
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.114824 pandas-plots-0.9.7/
+-rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.7/LICENSE
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 12:00:41.114709 pandas-plots-0.9.7/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.7/README.md
+-rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.7/pyproject.toml
+-rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-04-02 12:00:41.115187 pandas-plots-0.9.7/setup.cfg
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.108644 pandas-plots-0.9.7/src/
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.112101 pandas-plots-0.9.7/src/pandas_plots/
+-rw-r--r--   0 dexter     (501) staff       (20)     8490 2024-04-02 11:57:08.000000 pandas-plots-0.9.7/src/pandas_plots/hlp.py
+-rw-r--r--   0 dexter     (501) staff       (20)    28671 2024-04-02 11:13:22.000000 pandas-plots-0.9.7/src/pandas_plots/pls.py
+-rw-r--r--   0 dexter     (501) staff       (20)    22775 2024-04-02 11:33:47.000000 pandas-plots-0.9.7/src/pandas_plots/tbl.py
+-rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.7/src/pandas_plots/ven.py
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.114315 pandas-plots-0.9.7/src/pandas_plots.egg-info/
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)      337 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 dexter     (501) staff       (20)        1 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 dexter     (501) staff       (20)      119 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/requires.txt
+-rw-r--r--   0 dexter     (501) staff       (20)       13 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/top_level.txt
```

### Comparing `pandas-plots-0.9.6/LICENSE` & `pandas-plots-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.6/PKG-INFO` & `pandas-plots-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.6
+Version: 0.9.7
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

### Comparing `pandas-plots-0.9.6/README.md` & `pandas-plots-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.6/pyproject.toml` & `pandas-plots-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.6/setup.cfg` & `pandas-plots-0.9.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pandas-plots
-version = 0.9.6
+version = 0.9.7
 author = smeisegeier
 author_email = dexterDSDo@googlemail.com
 description = A collection of helper for table handling and vizualization
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE
```

### Comparing `pandas-plots-0.9.6/src/pandas_plots/hlp.py` & `pandas-plots-0.9.7/src/pandas_plots/hlp.py`

 * *Files 15% similar despite different names*

```diff
@@ -175,30 +175,69 @@
 
 
 def create_barcode_from_url(
     url: str,
     output_path: str | None = None,
     show_image: bool = False,
 ):
+    """
+    Create a barcode from the given URL. Uses "QR Code" from DENSO WAVE INCORPORATED.
+
+    Args:
+        url (str): The URL to encode in the barcode.
+        output_path (str | None, optional): The path to save the barcode image. Defaults to None.
+        show_image (bool, optional): Whether to display the barcode image. Defaults to False.
+    """
     WIDTH = 400
     HEIGHT = 400
 
     if not re.match(URL_REGEX, url):
-        print("❌ Not a valid URL")
-        return
+        print("💡 Not a valid URL")
 
     image = requests.get(
-        f"https://chart.googleapis.com/chart?chs={WIDTH}x{HEIGHT}&cht=qr&chl={url}"
+        # f"https://chart.googleapis.com/chart?chs={WIDTH}x{HEIGHT}&cht=qr&chl={url}"
+        f"https://api.qrserver.com/v1/create-qr-code/?size={WIDTH}x{HEIGHT}&data={url}"
     )
     image.raise_for_status()
 
     # * write binary content to file
     if output_path:
         with open(output_path, "wb") as qr:
             qr.write(image.content)
 
     # * Load the image from the response content
     if show_image:
         img = Image.open(BytesIO(image.content))
         plt.imshow(img)
         # plt.axis('off')  # Turn off axis numbers
         plt.show()
+
+def add_datetime_columns(df: pd.DataFrame, date_column: str = None) -> pd.DataFrame:
+    if not date_column:
+        date_column = [col for col in df.columns if pd.api.types.is_datetime64_any_dtype(df[col])][0]
+
+    if not date_column or not pd.api.types.is_datetime64_any_dtype(df[date_column]):
+        print("❌ No datetime column found")
+        return
+    
+    if [col for col in df.columns if "YYYY-WW" in col]:
+        print("❌ Added datetime columns already exist")
+        return
+    
+    print(f"⏳ Adding datetime columns basing off of: {date_column}")
+    df_= df.copy()
+
+    df_[date_column] = pd.to_datetime(df_[date_column])
+
+    df_["YYYY"] = df_[date_column].dt.year
+    df_["MM"] = df_[date_column].dt.month
+    df_["Q"] = df_[date_column].dt.quarter
+
+    df_["YYYY-MM"] = df_[date_column].dt.to_period("M").astype(str)
+    df_["YYYYQ"] = df_[date_column].dt.to_period("Q").astype(str)
+    df_["YYYY-WW"] = (
+        df_[date_column].dt.isocalendar().year.astype(str) + "-" +
+        df_[date_column].dt.isocalendar().week.astype(str).str.zfill(2)
+    )
+    df_["DDD"] = df_[date_column].dt.weekday.map({0: "Mon", 1: "Tue", 2: "Wed", 3: "Thu", 4: "Fri", 5: "Sat", 6: "Sun"})
+    
+    return df_
```

### Comparing `pandas-plots-0.9.6/src/pandas_plots/pls.py` & `pandas-plots-0.9.7/src/pandas_plots/pls.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     height: int = 500,
     width: int = 2000,
     title: str = None,
     renderer: Literal["png", "svg", None] = "png",
     caption: str = None,
     sort_values: bool = False,
     show_total: bool = False,
+    precision: int = 0,
 ) -> None:
     """
     Generates a stacked bar plot using the provided DataFrame.
     df *must* comprise the columns (order matters):
     - index axis
     - color axis (legend)
     - values (optional, if absent a simple count is applied)
@@ -131,14 +132,15 @@
     - height: int = 500 - The height of the plot.
     - width: An optional integer indicating the width of the chart. Default is 2000.
     - title: str = None - The title of the plot.
     - renderer: Literal["png", "svg",None] = "png" - The renderer for the plot.
     - caption: An optional string indicating the caption for the chart.
     - sort_values: bool = False - Sort axis by index (default) or values
     - show_total: bool = False - Whether to show the total value
+    - precision: int = 0 - The number of decimal places to round to
 
     Returns:
     None
     """
     BAR_LENGTH_MULTIPLIER = 1.05
 
     # * 2 axis means at least 2 columns
@@ -162,14 +164,17 @@
         df.dropna(inplace=True)
 
     # * strip whitespaces if columns are str
     if df.iloc[:, 0].dtype.kind == "O":
         df.iloc[:, 0] = df.iloc[:, 0].str.strip()
     if df.iloc[:, 1].dtype.kind == "O":
         df.iloc[:, 1] = df.iloc[:, 1].str.strip()
+    
+    # * apply precision
+    df.iloc[:,2] = df.iloc[:,2].round(precision)
 
     # * set index + color col
     col_index = df.columns[0] if not swap else df.columns[1]
     col_color = df.columns[1] if not swap else df.columns[0]
 
     # * add total as aggregation of df
     if show_total:
```

### Comparing `pandas-plots-0.9.6/src/pandas_plots/tbl.py` & `pandas-plots-0.9.7/src/pandas_plots/tbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import pandas as pd
 import plotly.express as px
 from plotly.subplots import make_subplots
 from scipy import stats
 
 from .hlp import wrap_text
 # from devtools import debug
+pd.options.display.colheader_justify = "right"
 # pd.options.mode.chained_assignment = None
 
-
 TOTAL_LITERAL = Literal[
     "sum", "mean", "median", "min", "max", "std", "var", "skew", "kurt"
 ]
 KPI_LITERAL = Literal["rag_abs","rag_rel", "min_max_xy", "max_min_xy", "min_max_x", "max_min_x"]
 
 
 def describe_df(
@@ -359,15 +359,15 @@
     - kpi_rag_list: a list of floats indicating the thresholds for rag lights. The list should have 2 elements.
     - kpi_shape: a Literal indicating the shape of the KPIs ["squad", "circle"]
 
     The function returns a styled representation of the DataFrame.
     """
     # * ensure arguments match parameter definition
     if any([df[col].dtype.kind not in ["i", "u", "f"] for col in df.columns]) == True:
-        print(f"❌ table must contain numeric data only")
+        print(f"❌ table must contain numeric data only. Maybe you forgot to convert this table with pivot or pivot_table first?")
         return
 
     if (
         (pct_axis and pct_axis not in ["x", "xy"])
         or (data_bar_axis and data_bar_axis not in ["x", "y", "xy"])
         or (heatmap_axis and heatmap_axis not in ["x", "y", "xy"])
     ):
```

### Comparing `pandas-plots-0.9.6/src/pandas_plots/ven.py` & `pandas-plots-0.9.7/src/pandas_plots/ven.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.6/src/pandas_plots.egg-info/PKG-INFO` & `pandas-plots-0.9.7/src/pandas_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.6
+Version: 0.9.7
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

