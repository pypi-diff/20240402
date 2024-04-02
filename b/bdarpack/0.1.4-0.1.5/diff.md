# Comparing `tmp/bdarpack-0.1.4.tar.gz` & `tmp/bdarpack-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdarpack-0.1.4.tar", last modified: Fri Feb 23 07:05:03 2024, max compression
+gzip compressed data, was "bdarpack-0.1.5.tar", last modified: Tue Apr  2 02:00:32 2024, max compression
```

## Comparing `bdarpack-0.1.4.tar` & `bdarpack-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 07:05:03.564661 bdarpack-0.1.4/
--rw-rw-rw-   0        0        0     1087 2023-04-13 04:35:30.000000 bdarpack-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4964 2024-01-09 02:35:48.000000 bdarpack-0.1.4/LICENSE-BSL
--rw-rw-rw-   0        0        0     5143 2024-02-23 07:05:03.561661 bdarpack-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4312 2023-12-07 03:28:05.000000 bdarpack-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 07:05:03.494950 bdarpack-0.1.4/bdarpack/
--rw-rw-rw-   0        0        0    44868 2024-02-23 07:00:21.000000 bdarpack-0.1.4/bdarpack/CleanData.py
--rw-rw-rw-   0        0        0    12346 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/Constraints.py
--rw-rw-rw-   0        0        0     9809 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/GaussianCopula.py
--rw-rw-rw-   0        0        0    37178 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/MarginalDist.py
--rw-rw-rw-   0        0        0    17783 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/PrivacyMetric.py
--rw-rw-rw-   0        0        0    65637 2023-11-28 05:43:41.000000 bdarpack-0.1.4/bdarpack/TabulaCopula.py
--rw-rw-rw-   0        0        0    25885 2023-11-28 01:17:39.000000 bdarpack-0.1.4/bdarpack/Transformer.py
--rw-rw-rw-   0        0        0    16290 2024-02-02 01:33:23.000000 bdarpack-0.1.4/bdarpack/VIsualPlot.py
--rw-rw-rw-   0        0        0        6 2023-11-28 01:10:33.000000 bdarpack-0.1.4/bdarpack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 07:05:03.555661 bdarpack-0.1.4/bdarpack/tests/
--rw-rw-rw-   0        0        0        0 2023-10-27 05:15:16.000000 bdarpack-0.1.4/bdarpack/tests/__init__.py
--rw-rw-rw-   0        0        0     2808 2023-08-17 04:15:08.000000 bdarpack-0.1.4/bdarpack/tests/definitions.py
--rw-rw-rw-   0        0        0     3315 2023-07-20 03:59:39.000000 bdarpack-0.1.4/bdarpack/tests/definitions_date.py
--rw-rw-rw-   0        0        0    32365 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/tests/script_nhanes_constraints.py
--rw-rw-rw-   0        0        0     9307 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/tests/test_clean.py
--rw-rw-rw-   0        0        0     4597 2023-11-28 01:19:52.000000 bdarpack-0.1.4/bdarpack/tests/test_transformer.py
--rw-rw-rw-   0        0        0    17805 2024-02-07 08:13:15.000000 bdarpack-0.1.4/bdarpack/utils_.py
-drwxrwxrwx   0        0        0        0 2024-02-23 07:05:03.559661 bdarpack-0.1.4/bdarpack.egg-info/
--rw-rw-rw-   0        0        0     5143 2024-02-23 07:05:03.000000 bdarpack-0.1.4/bdarpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-02-23 07:05:03.000000 bdarpack-0.1.4/bdarpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 07:05:03.000000 bdarpack-0.1.4/bdarpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-02-23 07:05:03.000000 bdarpack-0.1.4/bdarpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-23 07:05:03.000000 bdarpack-0.1.4/bdarpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 07:05:03.565730 bdarpack-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1724 2024-02-07 05:42:50.000000 bdarpack-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.740197 bdarpack-0.1.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 04:35:30.000000 bdarpack-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4964 2024-01-09 02:35:48.000000 bdarpack-0.1.5/LICENSE-BSL
+-rw-rw-rw-   0        0        0     5143 2024-04-02 02:00:32.737694 bdarpack-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4312 2023-12-07 03:28:05.000000 bdarpack-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.678010 bdarpack-0.1.5/bdarpack/
+-rw-rw-rw-   0        0        0    56701 2024-03-27 07:17:25.000000 bdarpack-0.1.5/bdarpack/CleanData.py
+-rw-rw-rw-   0        0        0    19421 2024-03-27 07:49:07.000000 bdarpack-0.1.5/bdarpack/Constraints.py
+-rw-rw-rw-   0        0        0     9809 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/GaussianCopula.py
+-rw-rw-rw-   0        0        0    37178 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/MarginalDist.py
+-rw-rw-rw-   0        0        0    17783 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/PrivacyMetric.py
+-rw-rw-rw-   0        0        0    65915 2024-04-02 01:28:38.000000 bdarpack-0.1.5/bdarpack/TabulaCopula.py
+-rw-rw-rw-   0        0        0    25885 2023-11-28 01:17:39.000000 bdarpack-0.1.5/bdarpack/Transformer.py
+-rw-rw-rw-   0        0        0    16379 2024-04-01 07:05:58.000000 bdarpack-0.1.5/bdarpack/VIsualPlot.py
+-rw-rw-rw-   0        0        0        6 2023-11-28 01:10:33.000000 bdarpack-0.1.5/bdarpack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.730510 bdarpack-0.1.5/bdarpack/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-27 05:15:16.000000 bdarpack-0.1.5/bdarpack/tests/__init__.py
+-rw-rw-rw-   0        0        0     2808 2023-08-17 04:15:08.000000 bdarpack-0.1.5/bdarpack/tests/definitions.py
+-rw-rw-rw-   0        0        0     3315 2023-07-20 03:59:39.000000 bdarpack-0.1.5/bdarpack/tests/definitions_date.py
+-rw-rw-rw-   0        0        0    32365 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/script_nhanes_constraints.py
+-rw-rw-rw-   0        0        0     9307 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/test_clean.py
+-rw-rw-rw-   0        0        0     4597 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/test_transformer.py
+-rw-rw-rw-   0        0        0    19262 2024-03-27 09:05:57.000000 bdarpack-0.1.5/bdarpack/utils_.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.736066 bdarpack-0.1.5/bdarpack.egg-info/
+-rw-rw-rw-   0        0        0     5143 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 02:00:32.740498 bdarpack-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2024-04-02 02:00:15.000000 bdarpack-0.1.5/setup.py
```

### Comparing `bdarpack-0.1.4/LICENSE` & `bdarpack-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/LICENSE-BSL` & `bdarpack-0.1.5/LICENSE-BSL`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/PKG-INFO` & `bdarpack-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdarpack
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for tabular synthetic data
 Home-page: https://biomeddar.github.io/copula-tabular/
 Author: MZ Tan
 Author-email: tan_ming_zhen@bii.a-star.edu.sg
 License: MIT
 Keywords: synthetic data copula
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bdarpack-0.1.4/README.md` & `bdarpack-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/GaussianCopula.py` & `bdarpack-0.1.5/bdarpack/GaussianCopula.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/MarginalDist.py` & `bdarpack-0.1.5/bdarpack/MarginalDist.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/PrivacyMetric.py` & `bdarpack-0.1.5/bdarpack/PrivacyMetric.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/TabulaCopula.py` & `bdarpack-0.1.5/bdarpack/TabulaCopula.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,25 +178,29 @@
         self._update_defaults(var_to_update="output_type_dict", new_value="OUTPUT_TYPE_DICT", definitions=definitions)
 
         # Update defaults for privacy leakage testing
         self._update_defaults(var_to_update="sampling", new_value="SAMPLING", definitions=definitions)
         self._update_defaults(var_to_update="privacy_batch_n", new_value="PRIVACY_BATCH_N", definitions=definitions)
 
         self.prefix_path = definitions.PREFIX_PATH
+        self.prefix_path = self.prefix_path.replace("\\","/")
 
         self.trainxlsx = definitions.TRAINXLSX
         self.traindictxlsx = definitions.TRAINDICTXLSX
 
         self.train_data_path = self.prefix_path + self.folder_trainData + "\\"
+        self.train_data_path = self.train_data_path.replace("\\","/")
         self.train_data_filename = self.train_data_path + definitions.TRAINXLSX
         self.train_data_dict_filename = self.train_data_path + definitions.TRAINDICTXLSX
 
         self.syn_data_path = self.prefix_path + self.folder_synData + "\\"
-        self.privacyMetrics_path = self.prefix_path + self.folder_privacyMetrics + "\\"
+        self.syn_data_path = self.syn_data_path.replace("\\","/")
 
+        self.privacyMetrics_path = self.prefix_path + self.folder_privacyMetrics + "\\"
+        self.privacyMetrics_path = self.privacyMetrics_path.replace("\\","/")
 
         self.train_df = None #initialise training data (dataframe)
         self.dict_df = None #initialise data dictionary (dataframe)
         self.var_list = None #list of all variables (column headers) found in input data
         self.processed_var_list = None #list of all variables (column headers) that have been transformed
         self.transformed_df = None #initialise transformed training data (dataframe) / replaced with transformed data after sampling (disjoint with self.control_df)
         self.control_df = None # the dataframe that is not sampled for training (left as control for privacy leakage testing)
@@ -274,15 +278,14 @@
         except ValueError as e:
             raise ValueError('Could not read sheet in excel file: ' + str(e)) from None
         
         # Convert columns to "string" type based on data dictionary settings
         var_names = [row[self.dict_var_varname] for index, row in self.dict_df.iterrows() if row[self.dict_var_vartype] == 'string']
         self.train_df[var_names] = self.train_df[var_names].astype("str")
 
-
         if (self.debug):
             print(f"Input data loaded.")
 
         # Initialise list of variables found in input dataset
         self.var_list = list(self.train_df.columns)
 
         if (self.debug):
```

### Comparing `bdarpack-0.1.4/bdarpack/Transformer.py` & `bdarpack-0.1.5/bdarpack/Transformer.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/VIsualPlot.py` & `bdarpack-0.1.5/bdarpack/VIsualPlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if 'Python is not installed as a framework.' in e.message:
         import matplotlib
         matplotlib.use('PS')   # Avoid crash on macos
         import matplotlib.pyplot as plt
 
 
 
-def hist(data_1d, fig=None, ax=None, position=None, title=None, alpha=0.8, color='blue', label=''):
+def hist(data_1d, fig=None, ax=None, position=None, title=None, alpha=0.8, color='blue', label='', bins='auto'):
     """Function to generate a histogram plot.
 
     Parameters:
         data_1d (array-like): 1 dimensional numerical data
         fig (matplotlib figure): Matplotlib figure to plot
         ax (axis object): Axis object on the figure
         position (tuple, int): Position of the axis on the figure
@@ -37,40 +37,40 @@
     if isinstance(position, tuple):
         ax = ax or fig.add_subplot(position[0], position[1], position[2])
     else:
         ax = ax or fig.add_subplot(position)
 
     data_dropped_na = data_1d.dropna()
 
-    ax.hist(data_dropped_na, density=True, bins='auto', alpha=alpha, color=color, label=label)
+    (n, bins, patches) = ax.hist(data_dropped_na, density=True, bins=bins, alpha=alpha, color=color, label=label)
 
     ax.legend(loc='best', frameon=False)
     ax.set_title(title, fontsize=8)
 
     return ax, fig
 
-def hist_compare(real_data, syn_data, var_list, no_cols=2):
+def hist_compare(real_data, syn_data, var_list, no_cols=2, bins='auto'):
 
     no_rows = len(var_list) // no_cols + math.ceil(len(var_list) % no_cols)
     ax_hist = []
     for index, var in enumerate(var_list):
         x_real = real_data[var]
         x_syn = syn_data[var]
 
         # position_tuple = int(str(no_rows) + str(no_cols) + str(index+1))
         position_tuple = (int(no_rows), int(no_cols), int(index+1))
 
         if (index == 0):
-            (ax_hist_out, fig_histogram) = hist(x_real, position = position_tuple, label=f"Original: n = {len(x_real)}")
+            (ax_hist_out, fig_histogram) = hist(x_real, position = position_tuple, bins=bins, label=f"Original: n = {len(x_real)}")
             ax_hist.append(ax_hist_out)
-            (ax_hist[index], fig_histogram) = hist(x_syn, ax=ax_hist[index], fig=fig_histogram, color='grey', title=f'Histogram Plot for {var}', label=f"Synthetic: n={len(x_syn)}")
+            (ax_hist[index], fig_histogram) = hist(x_syn, ax=ax_hist[index], fig=fig_histogram, color='grey', title=f'Histogram Plot for {var}', bins=bins, label=f"Synthetic: n={len(x_syn)}")
         else:
-            (ax_hist_out, fig_histogram) = hist(x_real, fig=fig_histogram, position = position_tuple, label=f"Original: n = {len(x_real)}")
+            (ax_hist_out, fig_histogram) = hist(x_real, fig=fig_histogram, position = position_tuple, bins=bins, label=f"Original: n = {len(x_real)}")
             ax_hist.append(ax_hist_out)
-            (ax_hist[index], fig_histogram) = hist(x_syn, ax=ax_hist[index], fig=fig_histogram, color='grey', title=f'Histogram Plot for {var}', label=f"Synthetic: n={len(x_syn)}")
+            (ax_hist[index], fig_histogram) = hist(x_syn, ax=ax_hist[index], fig=fig_histogram, color='grey', title=f'Histogram Plot for {var}', bins=bins, label=f"Synthetic: n={len(x_syn)}")
 
     return ax_hist, fig_histogram
 
 
 def corrMatrix(data, fig=None, position=None, title=None, x_label_rot=None, options={}):
     """Build single correlation matrix of data.
```

### Comparing `bdarpack-0.1.4/bdarpack/tests/definitions.py` & `bdarpack-0.1.5/bdarpack/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/tests/definitions_date.py` & `bdarpack-0.1.5/bdarpack/tests/definitions_date.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/tests/script_nhanes_constraints.py` & `bdarpack-0.1.5/bdarpack/tests/script_nhanes_constraints.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/tests/test_clean.py` & `bdarpack-0.1.5/bdarpack/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/tests/test_transformer.py` & `bdarpack-0.1.5/bdarpack/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/bdarpack/utils_.py` & `bdarpack-0.1.5/bdarpack/utils_.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,15 +215,22 @@
     # Update "COLUMN_NUMBER"
     for index, row in df.iterrows():
         # Set the value of the 'COLUMN_NUMBER' column to be one higher than the row's index
         df.loc[index, 'COLUMN_NUMBER'] = index + 1
 
     return df
 
-
+# GENERAL FUNCTIONS FOR DATATYPE
+# check if string is numerical
+def is_numerical(x):
+    try:
+        float(x)
+        return True
+    except:
+        return False
 
 # GENERAL FUNCTIONS FOR FILES
 def get_extension(filename):
   return filename.split(".")[-1]
 
 def change_extension(filename, ext):
     file_split = filename.split(".")
@@ -404,29 +411,29 @@
     if ("ddd" in str): # day of the week, short form (Mon):
         str = str.replace("ddd", r"%a")
 
     if ("dd" in str): # day number with a leading zero
         str = str.replace("dd", r"%d")
     elif ("d" in str): # day number without a leading zero
         if OS_TYPE=='Windows': # use "%-d" for unix, "%#d" for windows
-            str = str.replace("d", r"%#d")
+            str = str.replace("d", r"%d")
         elif OS_TYPE=='Linux' or 'Darwin':
             str = str.replace("d", r"%-d")
 
     if ("mmmm" in str): # month name, full form, (January):
         str = str.replace("mmmm", r"%B")
 
     if ("mmm" in str): # month name, short form, (Jan):
         str = str.replace("mmm", r"%b")
 
     if ("mm" in str): # month number with a leading zero
         str = str.replace("mm", r"%m")
     elif ("m" in str): # month number without a leading zero
         if OS_TYPE=='Windows': # use "%-m" for unix, "%#m" for windows
-            str = str.replace("m", r"%#m")
+            str = str.replace("m", r"%m")
         elif OS_TYPE=='Linux' or 'Darwin':
             str = str.replace("m", r"%-m")
     
     if ("yyyy" in str): # year four digits
         str = str.replace("yyyy", r"%Y")
 
     if ("yy" in str): # year last 2 digits
@@ -452,29 +459,65 @@
 
     data = strip_string_spaces(data)
     con_data = pd.to_datetime(data, format=format, errors="coerce")
     num_NaT = con_data.isnull().sum()
 
     return num_NaT
 
+def extract_year_month_day(data, format=None):
+    """
+    Function that extracts the year, month, and day from a given date using the specified format.
+
+    Parameters:
+        data (df['col']): The date to extract the year, month, and day from.
+        format (str): The format of the date. If not specified, the function will try to infer the format from the given date.
+
+    Returns:
+        df (pandas.DataFrame): A dataframe containing the extracted year, month, and day from the given date.
+    """
+    
+    if format is None:
+        format = date_format_search(data)
+
+    if isinstance(data, str):
+        datestr = pd.to_datetime(data, format=format)
+        di = {
+            "date": datestr,
+            "year": datestr.year,
+            "month": datestr.month,
+            "day": datestr.day
+        }
+        df = pd.DataFrame(di, index=[0])
+    else:
+        df = pd.DataFrame(columns=[])
+        df["date"] = pd.to_datetime(data, format=format)
+        df["year"] = df["date"].dt.year
+        df["month"] = df["date"].dt.month
+        df["day"] = df["date"].dt.day
+
+    return df
+
+
 # ASCII-compatible
 def convert_to_ascii(data):
     """
     Function to convert all string/object columns in a dataframe to characters that can safely be encoded to ASCII.
     """
     # load unidecode package
     from unidecode import unidecode
   
     # Iterate through columns of the dataframe
     if isinstance(data, pd.DataFrame):
         for col in data.columns:
             # Select only string/object columns
             if data[col].dtype == object or data[col].dtype == "string":
                 # Remove international accents from the column and assign it back to the same column
-                data[col] = data[col].apply(unidecode)
+                # (MZ): 22032024: update to skip <NA> values
+                data[col] = data[col].apply(lambda x: x if pd.isnull(x) else unidecode(x))
+                # data[col] = data[col].apply(unidecode)
                 # data[col] = data[col].str.replace("€", r"\€", regex=True).apply(unidecode)
     elif type(data) == str:
         data = unidecode(data)
     
     return data
```

### Comparing `bdarpack-0.1.4/bdarpack.egg-info/PKG-INFO` & `bdarpack-0.1.5/bdarpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdarpack
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for tabular synthetic data
 Home-page: https://biomeddar.github.io/copula-tabular/
 Author: MZ Tan
 Author-email: tan_ming_zhen@bii.a-star.edu.sg
 License: MIT
 Keywords: synthetic data copula
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bdarpack-0.1.4/bdarpack.egg-info/SOURCES.txt` & `bdarpack-0.1.5/bdarpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.4/setup.py` & `bdarpack-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # create wheel: py -m build --wheel
 # upload distribution to testpypi: twine upload --repository-url https://test.pypy.org/legacy/ dist/<pyexample-0.1.0.tar.gz> or *
 # upload distribution: twine upload dist/*
 # username = __token__, password = <token>
 
 setup(
     name='bdarpack',
-    version='0.1.4',    
+    version='0.1.5',    
     description='A Python package for tabular synthetic data',
     url='https://biomeddar.github.io/copula-tabular/',
     author='MZ Tan',
     author_email='tan_ming_zhen@bii.a-star.edu.sg',
     license='MIT',
     # license='BSL-1.1',
     keywords='synthetic data copula',
```

