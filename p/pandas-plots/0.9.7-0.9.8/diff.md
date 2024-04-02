# Comparing `tmp/pandas-plots-0.9.7.tar.gz` & `tmp/pandas-plots-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-plots-0.9.7.tar", last modified: Tue Apr  2 12:00:41 2024, max compression
+gzip compressed data, was "pandas-plots-0.9.8.tar", last modified: Tue Apr  2 13:01:05 2024, max compression
```

## Comparing `pandas-plots-0.9.7.tar` & `pandas-plots-0.9.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.114824 pandas-plots-0.9.7/
--rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.7/LICENSE
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 12:00:41.114709 pandas-plots-0.9.7/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.7/README.md
--rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.7/pyproject.toml
--rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-04-02 12:00:41.115187 pandas-plots-0.9.7/setup.cfg
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.108644 pandas-plots-0.9.7/src/
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.112101 pandas-plots-0.9.7/src/pandas_plots/
--rw-r--r--   0 dexter     (501) staff       (20)     8490 2024-04-02 11:57:08.000000 pandas-plots-0.9.7/src/pandas_plots/hlp.py
--rw-r--r--   0 dexter     (501) staff       (20)    28671 2024-04-02 11:13:22.000000 pandas-plots-0.9.7/src/pandas_plots/pls.py
--rw-r--r--   0 dexter     (501) staff       (20)    22775 2024-04-02 11:33:47.000000 pandas-plots-0.9.7/src/pandas_plots/tbl.py
--rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.7/src/pandas_plots/ven.py
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 12:00:41.114315 pandas-plots-0.9.7/src/pandas_plots.egg-info/
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)      337 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/SOURCES.txt
--rw-r--r--   0 dexter     (501) staff       (20)        1 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/dependency_links.txt
--rw-r--r--   0 dexter     (501) staff       (20)      119 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/requires.txt
--rw-r--r--   0 dexter     (501) staff       (20)       13 2024-04-02 12:00:41.000000 pandas-plots-0.9.7/src/pandas_plots.egg-info/top_level.txt
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.332556 pandas-plots-0.9.8/
+-rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.8/LICENSE
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 13:01:05.332484 pandas-plots-0.9.8/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.8/README.md
+-rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.8/pyproject.toml
+-rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-04-02 13:01:05.332853 pandas-plots-0.9.8/setup.cfg
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.329413 pandas-plots-0.9.8/src/
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.331068 pandas-plots-0.9.8/src/pandas_plots/
+-rw-r--r--   0 dexter     (501) staff       (20)     8508 2024-04-02 12:59:41.000000 pandas-plots-0.9.8/src/pandas_plots/hlp.py
+-rw-r--r--   0 dexter     (501) staff       (20)    28671 2024-04-02 11:13:22.000000 pandas-plots-0.9.8/src/pandas_plots/pls.py
+-rw-r--r--   0 dexter     (501) staff       (20)    22826 2024-04-02 12:27:14.000000 pandas-plots-0.9.8/src/pandas_plots/tbl.py
+-rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.8/src/pandas_plots/ven.py
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.332224 pandas-plots-0.9.8/src/pandas_plots.egg-info/
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)      337 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 dexter     (501) staff       (20)        1 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 dexter     (501) staff       (20)      119 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/requires.txt
+-rw-r--r--   0 dexter     (501) staff       (20)       13 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/top_level.txt
```

### Comparing `pandas-plots-0.9.7/LICENSE` & `pandas-plots-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.7/PKG-INFO` & `pandas-plots-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.7
+Version: 0.9.8
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

### Comparing `pandas-plots-0.9.7/README.md` & `pandas-plots-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.7/pyproject.toml` & `pandas-plots-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.7/setup.cfg` & `pandas-plots-0.9.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pandas-plots
-version = 0.9.7
+version = 0.9.8
 author = smeisegeier
 author_email = dexterDSDo@googlemail.com
 description = A collection of helper for table handling and vizualization
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE
```

### Comparing `pandas-plots-0.9.7/src/pandas_plots/hlp.py` & `pandas-plots-0.9.8/src/pandas_plots/hlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,36 +208,36 @@
     if show_image:
         img = Image.open(BytesIO(image.content))
         plt.imshow(img)
         # plt.axis('off')  # Turn off axis numbers
         plt.show()
 
 def add_datetime_columns(df: pd.DataFrame, date_column: str = None) -> pd.DataFrame:
+    df_= df.copy()
     if not date_column:
-        date_column = [col for col in df.columns if pd.api.types.is_datetime64_any_dtype(df[col])][0]
+        date_column = [col for col in df_.columns if pd.api.types.is_datetime64_any_dtype(df_[col])][0]
+    else:
+        df_[date_column] = pd.to_datetime(df_[date_column])
 
-    if not date_column or not pd.api.types.is_datetime64_any_dtype(df[date_column]):
+    if not date_column or not pd.api.types.is_datetime64_any_dtype(df_[date_column]):
         print("❌ No datetime column found")
         return
     
-    if [col for col in df.columns if "YYYY-WW" in col]:
+    if [col for col in df_.columns if "YYYY-WW" in col]:
         print("❌ Added datetime columns already exist")
         return
     
     print(f"⏳ Adding datetime columns basing off of: {date_column}")
-    df_= df.copy()
-
-    df_[date_column] = pd.to_datetime(df_[date_column])
 
     df_["YYYY"] = df_[date_column].dt.year
     df_["MM"] = df_[date_column].dt.month
     df_["Q"] = df_[date_column].dt.quarter
 
     df_["YYYY-MM"] = df_[date_column].dt.to_period("M").astype(str)
     df_["YYYYQ"] = df_[date_column].dt.to_period("Q").astype(str)
     df_["YYYY-WW"] = (
-        df_[date_column].dt.isocalendar().year.astype(str) + "-" +
+        df_[date_column].dt.isocalendar().year.astype(str) + "-W" +
         df_[date_column].dt.isocalendar().week.astype(str).str.zfill(2)
     )
     df_["DDD"] = df_[date_column].dt.weekday.map({0: "Mon", 1: "Tue", 2: "Wed", 3: "Thu", 4: "Fri", 5: "Sat", 6: "Sun"})
     
     return df_
```

### Comparing `pandas-plots-0.9.7/src/pandas_plots/pls.py` & `pandas-plots-0.9.8/src/pandas_plots/pls.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.7/src/pandas_plots/tbl.py` & `pandas-plots-0.9.8/src/pandas_plots/tbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,14 +438,16 @@
     cmap_heat = "Blues" if theme == "light" else "copper"
 
     # * apply data bar coloring
     if data_bar_axis:
         out.bar(
             color=f"{color_highlight}",
             axis=0 if data_bar_axis == "x" else 1 if data_bar_axis == "y" else None,
+            width=100,
+            # align="zero",
         )
 
     
     def get_kpi(val: float, col: str) -> str:
         """
         Function to calculate and return the appropriate icon based on the given value and key performance indicator (KPI) mode.
```

### Comparing `pandas-plots-0.9.7/src/pandas_plots/ven.py` & `pandas-plots-0.9.8/src/pandas_plots/ven.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.7/src/pandas_plots.egg-info/PKG-INFO` & `pandas-plots-0.9.8/src/pandas_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.7
+Version: 0.9.8
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

