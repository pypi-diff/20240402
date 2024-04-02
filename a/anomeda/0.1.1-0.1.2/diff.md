# Comparing `tmp/anomeda-0.1.1.tar.gz` & `tmp/anomeda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomeda-0.1.1.tar", last modified: Mon Feb 26 15:45:39 2024, max compression
+gzip compressed data, was "anomeda-0.1.2.tar", last modified: Tue Apr  2 12:16:29 2024, max compression
```

## Comparing `anomeda-0.1.1.tar` & `anomeda-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 15:45:39.266024 anomeda-0.1.1/
--rw-rw-rw-   0        0        0     1094 2024-02-09 13:38:25.000000 anomeda-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8506 2024-02-26 15:45:39.266024 anomeda-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7860 2024-02-26 14:06:30.000000 anomeda-0.1.1/README.md
--rw-rw-rw-   0        0        0      722 2024-02-26 15:35:24.000000 anomeda-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-26 15:45:39.271112 anomeda-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-26 15:45:39.171561 anomeda-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-26 15:45:39.217707 anomeda-0.1.1/src/anomeda/
--rw-rw-rw-   0        0        0    24122 2024-02-26 15:42:08.000000 anomeda-0.1.1/src/anomeda/DataFrame.py
--rw-rw-rw-   0        0        0     1455 2024-02-23 10:11:32.000000 anomeda-0.1.1/src/anomeda/__init__.py
--rw-rw-rw-   0        0        0    51473 2024-02-26 15:32:54.000000 anomeda-0.1.1/src/anomeda/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-26 15:45:39.261591 anomeda-0.1.1/src/anomeda.egg-info/
--rw-rw-rw-   0        0        0     8506 2024-02-26 15:45:39.000000 anomeda-0.1.1/src/anomeda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-02-26 15:45:39.000000 anomeda-0.1.1/src/anomeda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 15:45:39.000000 anomeda-0.1.1/src/anomeda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-26 15:45:39.000000 anomeda-0.1.1/src/anomeda.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-26 15:45:39.246117 anomeda-0.1.1/tests/
--rw-rw-rw-   0        0        0    13454 2024-02-26 15:44:44.000000 anomeda-0.1.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.361674 anomeda-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2024-02-09 13:38:25.000000 anomeda-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8784 2024-04-02 12:16:29.355133 anomeda-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8138 2024-04-02 12:14:34.000000 anomeda-0.1.2/README.md
+-rw-rw-rw-   0        0        0      722 2024-04-02 12:12:43.000000 anomeda-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:16:29.364113 anomeda-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.213108 anomeda-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.270801 anomeda-0.1.2/src/anomeda/
+-rw-rw-rw-   0        0        0    24164 2024-03-29 14:25:00.000000 anomeda-0.1.2/src/anomeda/DataFrame.py
+-rw-rw-rw-   0        0        0     1455 2024-02-23 10:11:32.000000 anomeda-0.1.2/src/anomeda/__init__.py
+-rw-rw-rw-   0        0        0    64895 2024-04-02 12:05:17.000000 anomeda-0.1.2/src/anomeda/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.345378 anomeda-0.1.2/src/anomeda.egg-info/
+-rw-rw-rw-   0        0        0     8784 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.331799 anomeda-0.1.2/tests/
+-rw-rw-rw-   0        0        0    13469 2024-04-02 12:04:18.000000 anomeda-0.1.2/tests/test_main.py
```

### Comparing `anomeda-0.1.1/LICENSE` & `anomeda-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.1/PKG-INFO` & `anomeda-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,15 @@
 
 ```python
 trends = anomeda.fit_trends(
     anomeda_df,
     trend_fitting_conf={'max_trends': 'auto', 'min_var_reduction': 0.75}, # set the number of trends automatically,
                                                                           # try to reduce error variance compared to error of estimating values by 1-line trend by 75%
     breakdown='all-clusters', # fit trends for clusters extracted from all possible sets of measures
-    mettic_propagte='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
+    metric_propagate='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
     min_cluster_size=3 # skip small clusters, they all will be combined into 'skipped' cluster
 )
 ```
 
 Typically you will see something like this:
 
 ![anomeda.fit_trends method](docs/img/anomeda_fit_trends_1.png "anomeda.fit_trends method")
@@ -91,14 +91,20 @@
 anomeda.plot_trends(anomeda_df, clusters=['`country`=="Germany"'])
 ```
 
 The output will look like this:
 
 ![anomeda.plot_trends method](docs/img/anomeda_plot_trends_1.png "anomeda.plot_trends method")
 
+If you don't need to *fit trends* since it's a complicated procedure, but you need to take a brief look at the clusters, you may run a different command which simply plots the clusters:
+
+```python
+anomeda.plot_clusters(anomeda_df, clusters=['`country`=="Germany"'])
+```
+
 Of course, you may have no idea which cluster caused the problem and what to plot. Almost always you know only that there is a decrease of an overall metric and you need to find the culprits. Let's utilize another method -- `anomeda.compare_clusters`.
 
 ```python
 anomeda.compare_clusters(
     anomeda_df,
     period1='date < "2024-01-30"',
     period2='date >= "2024-01-30"'
```

### Comparing `anomeda-0.1.1/README.md` & `anomeda-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ```python
 trends = anomeda.fit_trends(
     anomeda_df,
     trend_fitting_conf={'max_trends': 'auto', 'min_var_reduction': 0.75}, # set the number of trends automatically,
                                                                           # try to reduce error variance compared to error of estimating values by 1-line trend by 75%
     breakdown='all-clusters', # fit trends for clusters extracted from all possible sets of measures
-    mettic_propagte='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
+    metric_propagate='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
     min_cluster_size=3 # skip small clusters, they all will be combined into 'skipped' cluster
 )
 ```
 
 Typically you will see something like this:
 
 ![anomeda.fit_trends method](docs/img/anomeda_fit_trends_1.png "anomeda.fit_trends method")
@@ -77,14 +77,20 @@
 anomeda.plot_trends(anomeda_df, clusters=['`country`=="Germany"'])
 ```
 
 The output will look like this:
 
 ![anomeda.plot_trends method](docs/img/anomeda_plot_trends_1.png "anomeda.plot_trends method")
 
+If you don't need to *fit trends* since it's a complicated procedure, but you need to take a brief look at the clusters, you may run a different command which simply plots the clusters:
+
+```python
+anomeda.plot_clusters(anomeda_df, clusters=['`country`=="Germany"'])
+```
+
 Of course, you may have no idea which cluster caused the problem and what to plot. Almost always you know only that there is a decrease of an overall metric and you need to find the culprits. Let's utilize another method -- `anomeda.compare_clusters`.
 
 ```python
 anomeda.compare_clusters(
     anomeda_df,
     period1='date < "2024-01-30"',
     period2='date >= "2024-01-30"'
```

### Comparing `anomeda-0.1.1/pyproject.toml` & `anomeda-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anomeda"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Anton Saroka", email="anton.soroka.1313@gmail.com" },
 ]
 description = "Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `anomeda-0.1.1/src/anomeda/DataFrame.py` & `anomeda-0.1.2/src/anomeda/DataFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,17 @@
         index_name = kwargs.get('index_name')
    
         curr_indeces = list(filter(lambda x: x is not None, self.index.names))
         if index_name is None: 
             if len(curr_indeces) >= 1:
                 self._index_name = curr_indeces
                 try:
-                    self.index = pd.to_datetime(self.index)
+                    self.index = self.index.astype('str').astype('int64')
                 except BaseException:
-                    self.index = self.index.astype('int64')
+                    self.index = pd.to_datetime(self.index)
             else:
                 self._index_name = None
             self.set_index_type()
         else:
             self.set_index(index_name, inplace=True)
         
         measures_names = kwargs.get('measures_names')
@@ -479,22 +479,22 @@
             index_name = [index_name]
 
         if index_name != curr_indeces:
             resp = super().reset_index()
             resp = super().set_index(*args, **kwargs)
             if resp is not None:
                 try:
-                    resp.index = pd.to_datetime(resp.index)
+                    self.index = self.index.astype('str').astype('int64')
                 except BaseException:
-                    resp.index = resp.index.astype('int64')
+                    self.index = pd.to_datetime(self.index)
                 return self.replace_df(resp, inplace=False)
             try:
-                self.index = pd.to_datetime(self.index)
+                self.index = self.index.astype('str').astype('int64')
             except BaseException:
-                self.index = self.index.astype('int64')
+                self.index = pd.to_datetime(self.index)
             index_names = list(filter(lambda x: x is not None, self.index.names))
             if len(index_names) >= 1:
                 self._index_name = index_names
             self.set_index_type()
         else:
             self._index_name = curr_indeces
             self.set_index_type()
```

### Comparing `anomeda-0.1.1/src/anomeda/__init__.py` & `anomeda-0.1.2/src/anomeda/__init__.py`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.1/src/anomeda/utils.py` & `anomeda-0.1.2/src/anomeda/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,14 +90,74 @@
         + __regularizer(ratio2) * np.var(np.abs(y_pred2 - y_true2)) * np.quantile(np.abs(y_pred2 - y_true2), 0.9)
         
         metric_vals.append(metric)
     
     return points_candidates[np.argmin(metric_vals)]
 
 
+def _propagate_metric(
+    x : 'numpy.ndarray[int] | numpy.ndarray[datetime]', 
+    y : 'numpy.ndarray[float]', 
+    strategy : '"zeros" | "ffil" | None',
+    freq: 'frequency unit for pandas.DatetimeIndex' = None
+):
+    
+    if len(x) != len(y):
+        raise ValueError('Lengths of x and y must be the same for the propagation')
+
+    if len(x) == 0 or len(y) == 0:
+        return x, y
+    
+    if type(x[0]) in [pd.Timestamp, datetime, np.datetime64]:
+        x = pd.to_datetime(x)
+
+    if type(x) == pd.DatetimeIndex:
+        x_is_numeric = False
+        if freq is None:
+            raise ValueError('If x is pandas.DatetimeIndex, frequency must be provided')
+    else:
+        x_is_numeric = True
+        
+    if x_is_numeric:
+        x_prop = np.arange(x.min(), x.max() + 1)
+        y_prop = np.zeros(x.max() - x.min() + 1)
+        x_formatted = x
+        x_prop_int = x_prop
+    else:
+        x_datetime = pd.to_datetime(x)
+        x_prop = pd.date_range(start=x_datetime.min(), end=x_datetime.max(), freq=freq)
+        y_prop = np.zeros(len(x_prop))
+
+        x_formatted = x_datetime
+        x_prop_int = np.arange(len(x_prop))
+
+    if strategy is None:
+        if not x_is_numeric:
+            x_prop_int = []
+            init_i = 0
+            for i in range(len(x_prop)):
+                if x_prop[i] == x_formatted[init_i]:
+                    x_prop_int.append(i)
+                    init_i += 1
+            x_prop_int = np.array(x_prop_int)
+
+        return x_formatted, x_prop_int, y
+
+    init_i = 0
+    for i in range(len(x_prop)):
+        if x_prop[i] == x_formatted[init_i]:
+            y_prop[i] = y[init_i]
+            init_i += 1
+        else:
+            if strategy == 'ffil':
+                y_prop[i] = y[init_i - 1]
+
+    return x_prop, x_prop_int, y_prop
+
+
 def extract_trends(
     x : 'numpy.ndarray[int] | pandas.DatetimeIndex', 
     y : 'numpy.ndarray[float]', 
     freq: 'frequency unit for pandas.DatetimeIndex' = None,
     propagation_strategy: '"zeros" | "ffil" | None' = None,
     max_trends : "int | 'auto'"='auto', 
     min_var_reduction : 'float[0, 1] | None'=0.5, 
@@ -161,82 +221,24 @@
                                                                       # consisting of 2 samples, 
                                                                       # metric mean over date points is 10.8,
                                                                       # mae for fitting trend over date points is 0.0
                                                                       # sum for all metric values is 21.6
         1: (4, 6, (-0.2999999999999998, 4.6), (2, 3.25, 0.0, 6.5))
     }
     """
-    def propagate_metric(
-        x : 'numpy.ndarray[int] | numpy.ndarray[datetime]', 
-        y : 'numpy.ndarray[float]', 
-        strategy : '"zeros" | "ffil" | None',
-        freq: 'frequency unit for pandas.DatetimeIndex' = None
-    ):
-        
-        if len(x) != len(y):
-            raise ValueError('Lengths of x and y must be the same for the propagation')
-
-        if len(x) == 0 or len(y) == 0:
-            return x, y
-        
-        if type(x[0]) in [pd.Timestamp, datetime, np.datetime64]:
-            x = pd.to_datetime(x)
-
-        if type(x) == pd.DatetimeIndex:
-            x_is_numeric = False
-            if freq is None:
-                raise ValueError('If x is pandas.DatetimeIndex, frequency must be provided')
-        else:
-            x_is_numeric = True
-            
-        if x_is_numeric:
-            x_prop = np.arange(x.min(), x.max() + 1)
-            y_prop = np.zeros(x.max() - x.min() + 1)
-            x_formatted = x
-            x_prop_int = x_prop
-        else:
-            x_datetime = pd.to_datetime(x)
-            x_prop = pd.date_range(start=x_datetime.min(), end=x_datetime.max(), freq=freq)
-            y_prop = np.zeros(len(x_prop))
-
-            x_formatted = x_datetime
-            x_prop_int = np.arange(len(x_prop))
-
-        if strategy is None:
-            if not x_is_numeric:
-                x_prop_int = []
-                init_i = 0
-                for i in range(len(x_prop)):
-                    if x_prop[i] == x_formatted[init_i]:
-                        x_prop_int.append(i)
-                        init_i += 1
-                x_prop_int = np.array(x_prop_int)
-
-            return x_formatted, x_prop_int, y
-
-        init_i = 0
-        for i in range(len(x_prop)):
-            if x_prop[i] == x_formatted[init_i]:
-                y_prop[i] = y[init_i]
-                init_i += 1
-            else:
-                if strategy == 'ffil':
-                    y_prop[i] = y[init_i - 1]
-
-        return x_prop, x_prop_int, y_prop
     
     if max_trends == 'auto':
         if min_var_reduction is None:
             raise ValueError("Either max_trends or min_var_reduction parameters must be set. max_trends='auto' and min_var_reduction=None at the same time is not permitted.")
         max_trends = np.inf
 
     if min_var_reduction is None:
         min_var_reduction = np.inf
 
-    x_prop, x_prop_int, y_prop = propagate_metric(x, y, strategy=propagation_strategy, freq=freq)
+    x_prop, x_prop_int, y_prop = _propagate_metric(x, y, strategy=propagation_strategy, freq=freq)
 
     x_int_val_map = {x_int: x_val for (x_int, x_val) in zip(x_prop_int, x_prop)}
     if type(x_prop) == pd.DatetimeIndex:
         x_int_val_map[x_prop_int[-1] + 1] = x_prop[-1] + pd.Timedelta(1, unit=freq)
     else:
         x_int_val_map[x_prop_int[-1] + 1] = x_prop[-1] + 1
 
@@ -373,83 +375,67 @@
     return trends
 
 
 def compare_clusters(
     data: 'anomeda.DataFrame',
     period1: 'str',
     period2: 'str',
-    breakdown : "'no' | 'all-clusters' | list[str]" = 'no',
-    clusters : 'list' = None
+    breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no'
 ):
     """Compare metric values for 2 periods.
     
     The method generates pandas.DataFrame object with descriptions for two periods, for each cluster. 
     You can use it to identify the cluster or set of clusters caused the differences in the overall metric values between two periods.
     
     Parameters
     ----------
     data : anomeda.DataFrame
         Object containing data to be analyzed
     period1 : str
         Query to filter the first period. For example, 'dt < 10'.
-    period2 s: str
+    period2 : str
         Query to filter the second period. For example, 'dt >= 10'.
-    breakdown : 'no' | 'all-clusters' | list[str], default 'no'
-        If 'no', the metric is grouped by date points only. If 'all-clusters', then all combinations of measures are used to create clusters for fitting trends within them. If list[str], then only combinations of measures specified in the list are used.
-    clusters : list, default None
-        List of clusters to use in the comparison. The objects in the list are queries used in pandas.DataFrame.query.
-        If None, all clusters are used. Default is None.
+    breakdowns : 'no' | 'all' | list[str], default 'no'
+        If 'no', the metric is grouped by date points only. 
+        If 'all', all combinations of measures are used to extract and plot clusters. 
+        If list[str], then only specific clusters specified in the list are plotted. 
+        If list[list[str]] then each internal list is a list of measures used to extract clusters.
         
     Returns
     -------
     output : pandas.DataFrame
         Object describing the clusters and the changes in the metric behavior between them. 
 
     Examples
     --------
     ```python
     anomeda.compare_clusters(
         data,
         period1='dt < 10',
         period2='dt >= 10',
-        breakdown='no'
+        breakdowns='no'
     )
     ```
     """
     if type(data) != DataFrame:
         raise TypeError(INVALID_DATA_TYPE_MSG.format('data', type(data)))
-        
-    if data.get_measures_names() is None:
-        raise KeyError('not-None "measure_names" must be set for anomeda.DataFrame object')
-    measures_names = data.get_measures_names()
-
-    if clusters is not None:
-        clusters = clusters.copy()
-        for i in range(len(clusters)):
-            if clusters[i] not in ['total', 'skipped']:
-                clusters[i] = ' and '.join(sorted(clusters[i].split(' and '), key=lambda v: measures_names.index(v.split('==')[0].replace('`', ''))))
 
-    
     new_df1 = data.to_pandas().reset_index().query(period1).set_index(data.get_index_name())
     if new_df1.shape[0] == 0:
         raise ValueError(f'Failed to find data for period {period1}')
 
     new_df2 = data.to_pandas().reset_index().query(period2).set_index(data.get_index_name())
     if new_df2.shape[0] == 0:
         raise ValueError(f'Failed to find data for period {period2}')
 
     data1 = data.replace_df(new_df1, keep_discretization=True)
     data2 = data.replace_df(new_df2, keep_discretization=True)
 
-    clusters_info_1 = fit_trends(data1, trend_fitting_conf={'max_trends': 1}, breakdown=breakdown, plot=False, df=True)
-    clusters_info_2 = fit_trends(data2, trend_fitting_conf={'max_trends': 1}, breakdown=breakdown, plot=False, df=True)
-    
-    if clusters is not None:
-        clusters_info_1 = clusters_info_1[clusters_info_1['cluster'].isin(clusters)]
-        clusters_info_2 = clusters_info_2[clusters_info_2['cluster'].isin(clusters)]
+    clusters_info_1 = fit_trends(data1, trend_fitting_conf={'max_trends': 1}, breakdowns=breakdowns, plot=False, df=True)
+    clusters_info_2 = fit_trends(data2, trend_fitting_conf={'max_trends': 1}, breakdowns=breakdowns, plot=False, df=True)
     
     joined_info = clusters_info_1.merge(clusters_info_2, on='cluster', how='outer')
 
     joined_info = joined_info[[
         'cluster',
         'trend_start_dt_x', 'trend_end_dt_x', 
         'trend_start_dt_y', 'trend_end_dt_y',
@@ -462,31 +448,33 @@
     ]]
 
     return joined_info
 
 
 def find_anomalies(
     data: 'anomeda.DataFrame | (numpy.ndarray[int], numpy.ndarray[float])', 
-    clusters: 'list' = None, 
+    breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
     anomalies_conf : 'dict' = {'p_large': 1, 'p_low': 1, 'n_neighbors': 3},
     return_all_points : 'bool' = False,
     trend_fitting_conf : 'dict' = None
 ):
     """Find metric anomalies by looking for the most extreme metric changes.
     
     The method finds differences between real metric and a fitted trends, find points with extreme differences and marks them as anomalies. 
     You can find anomalies for automatically extracted clusters only if passing an anomeda.DataFrame.
     
     Parameters
     ----------
     data : anomeda.DataFrame | (numpy.ndarray[int], numpy.ndarray[float])
         Object containing metric values to be analyzed. Trends must be fitted for the object with anomeda.fit_trends() method if anomeda.DataFrame is passed.
-    clusters : list, default None
-        List of clusters to plot. The objects in the list are queries used in pandas.DataFrame.query.
-        Make sure you pass the cluster names exactly as they they appear in the fitted trends.
+    breakdowns : 'no' | 'all' | list[str], default 'no'
+        If 'no', the metric is grouped by date points only. 
+        If 'all', all combinations of measures are used to extract and plot clusters. 
+        If list[str], then only specific clusters specified in the list are plotted. 
+        If list[list[str]] then each internal list is a list of measures used to extract clusters.
     anomalies_conf : dict, default {'p_large': 1., 'p_low': 1., 'n_neighbors': 3}
         Dict containing 'p_large' and 'p_low' values. Both are float values between 0 and 1 corresponding to the % of the anomalies with largest and lowest metric values to be returned.
         For example, if you set 'p_low' to 0, no points with abnormally low metric values will be returned; if 0.5, then 50% of points with abnormally values will be returned, etc. 
         If some of the keys is not present or None, 1 is assumed.
         'n_neighbors' means number of neighbors parameter for sklearn.neighbors.LocalOutlierFactor class. The class is used to find points with abnormally large MAE. The more the parameter, typically, the less sensitive the model to anomalies.
     return_all_points : bool, default False
         If False, only anomaly points are returned. If True, all points with anomalies marks are returned. Default False.
@@ -535,37 +523,83 @@
         if metric_name is None:
             raise KeyError('not-None "metric_name" must be set for anomeda.DataFrame object')
         
         agg_func = data.get_agg_func()
         if agg_func is None:
             raise KeyError('not-None "agg_func" must be set for anomeda.DataFrame object')
 
-        if data.get_measures_names() is None:
-            raise KeyError('not-None "measure_names" must be set for anomeda.DataFrame object')
         measures_names = data.get_measures_names()
-        
-        if clusters is None:
-            clusters = df['cluster'].drop_duplicates()
-
-        if trend_fitting_conf is not None:
-            raise ValueError('trend_fitting_conf is not used if anomeda.DataFrame is specified. Please remove the argument or set it to None to avoid confusion.')
+        if measures_names is None:
+            measures_names = []
 
+        clusters_calculated = False
+        if breakdowns == 'all':
+            measures_to_iterate = [[]]
+            if measures_names is not None and len(measures_names) > 0:
+                for i in range(1, len(measures_names) + 1):
+                    for el in combinations(measures_names, i):
+                        measures_to_iterate.append(list(el))
+        elif type(breakdowns) == list:
+            if len(breakdowns) > 0:
+                if type(breakdowns[0]) == list:
+                    measures_names = data.get_measures_names()
+                    measures_to_iterate = breakdowns.copy()
+                elif type(breakdowns[0]) == str:
+                    clusters = breakdowns.copy()
+                    clusters_calculated = True
+                else:
+                    raise ValueError('If breakdowns is a list, then it must be either [[measure_name, ..], ..] (list of lists) or [cluster_1, ..] (list of queries used to extract clusters)')
+            else:
+                measures_to_iterate = [[]]
+        elif breakdowns == 'no':
+            measures_to_iterate = [[]]
+        else:
+            raise ValueError('Breakdown must be either "all", "no" or list')
+        
         data_pandas = data.to_pandas().sort_index().reset_index()
         measures_types = data.get_measures_types()
         if measures_types is not None and 'continuous' in measures_types:
             for measure in measures_types['continuous']:
                 data_pandas[measure] = data.get_discretized_measures()[measure]
+        
+        if not clusters_calculated:
+            clusters = []
+            if len(measures_to_iterate) == 0:
+                query = 'total'
+                clusters.append(query)
+            else:
+                for measures_set in measures_to_iterate:
+                    if len(measures_set) == 0:
+                        query = 'total'
+                        clusters.append(query)
+                    else:
+                        for measures_values in data_pandas[measures_set].drop_duplicates().values:
+                            str_arr = []
+                            for (measure_name, measure_value) in zip(measures_set, measures_values):
+                                quote = '"' if type(measure_value) == str else ''
+                                str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
+                            query = ' and '.join(str_arr)
+                            clusters.append(query)
+
+        if trend_fitting_conf is not None:
+            raise ValueError('trend_fitting_conf is not used if anomeda.DataFrame is specified. Please remove the argument or set it to None to avoid confusion.')
 
         resp = []
         
         for c in clusters:
 
-            # reorder features names in accordance to how they sorted in measures names
+             # reorder features names in accordance to how they sorted in measures names 
             if c not in ['total', 'skipped']:
-                c = ' and '.join(sorted(c.split(' and '), key=lambda v: measures_names.index(v.split('==')[0].replace('`', ''))))
+                try:
+                    c = ' and '.join(sorted(c.split(' and '), key=lambda v: measures_names.index(v.split('==')[0].strip().replace('`', ''))))
+                except ValueError:
+                    raise ValueError('Some feature from the cluster {} is not a measure'.format(c))
+                
+            if c not in df['cluster'].values:
+                continue
 
             df_tmp = df[df['cluster'] == c]
 
             if df_tmp.shape[0] == 0:
                 raise ValueError(f'Failed to find cluster {c}. Make sure such a breakdown was set during trends fitting.')
 
             yindex = data._clusters[c]['index']
@@ -653,16 +687,14 @@
 
         resp = pd.concat(resp).reset_index(drop=True)
         if not return_all_points:
             resp = resp[resp['anomaly']].reset_index(drop=True)
 
         return resp
     elif type(data) == tuple and type(data[0]) == np.ndarray and type(data[1]) == np.ndarray:
-        if clusters is not None:
-            raise ValueError('Clusters may be specified only if passing an anomeda.DataFrame object')
 
         yindex, ydata = data
 
         if type(yindex[0]) == int:
             yindex_int = yindex
         else:
             yindex_int = np.arange(len(yindex))
@@ -760,31 +792,31 @@
         return resp
     else:
         raise TypeError('Data parameter must be either anomeda.DataFrame or (numpy.ndarray[int], numpy.ndarray[float]) tuple')
         
 
 def plot_trends(
     data: 'anomeda.DataFrame | pandas.DataFrame returned from anomeda.fit_trends()', 
-    clusters: 'list' = None, 
-    colors: 'dict' = None, 
-    show_metric=True
+    breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
+    show_metric=True,
+    colors : 'dict' = None
 ):
     """Plot fitted trends.
     
     Plot trends either from anomeda.DataFrame instance or using a response from anomeda.fit_trends().
     
     Parameters
     ----------
     data : anomeda.DataFrame | pandas.DataFrame returned from anomeda.fit_trends()
         Object containing trends to be plotted.
-    clusters : list, default None
-        List of clusters to plot. The objects in the list are queries used in pandas.DataFrame.query.
-        Make sure you pass the cluster names exactly as they they appear in the fitted trends.
-    colors : dict, default None
-        Dictionary with a mapping between clusters and colors used in matplotlib.
+    breakdowns : 'no' | 'all' | list[str], default 'no'
+        If 'no', the metric is grouped by date points only. 
+        If 'all', all combinations of measures are used to extract and plot clusters. 
+        If list[str], then only specific clusters specified in the list are plotted. 
+        If list[list[str]] then each internal list is a list of measures used to extract clusters.
     show_metric : bool, default True
         Indicator if to show actual metric on plots.
         
     Returns
     -------
     None
 
@@ -795,38 +827,123 @@
     """
     if type(data) == DataFrame:
         if hasattr(data, '_trends'):
             df = data._trends.copy()
         if not hasattr(data, '_trends') or not hasattr(data, '_clusters'):
             raise NotFittedError('The anomeda.DataFrame instance has no fitted trends or clusters. Run anomeda.fit_trends() with save_trends=True and prefered parameters first')
     
+        if df is None or len(df) == 0:
+            return None 
+        
+        index_name = data.get_index_name()
+        if index_name is None:
+            raise KeyError('not-None "index_name" must be set for anomeda.DataFrame object')
+        
+        metric_name = data.get_metric_name()
+        if metric_name is None:
+            raise KeyError('not-None "metric_name" must be set for anomeda.DataFrame object')
+        
+        agg_func = data.get_agg_func()
+        if agg_func is None:
+            raise KeyError('not-None "agg_func" must be set for anomeda.DataFrame object')
+        
         measures_names = data.get_measures_names()
         if measures_names is None:
-            raise KeyError('not-None "measures_names" must be set for anomeda.DataFrame object')
-    elif type(data) == pd.DataFrame:
+            measures_names = []
+
+        clusters_calculated = False
+        if breakdowns == 'all':
+            measures_to_iterate = [[]]
+            if measures_names is not None and len(measures_names) > 0:
+                for i in range(1, len(measures_names) + 1):
+                    for el in combinations(measures_names, i):
+                        measures_to_iterate.append(list(el))
+        elif type(breakdowns) == list:
+            if len(breakdowns) > 0:
+                if type(breakdowns[0]) == list:
+                    measures_names = data.get_measures_names()
+                    measures_to_iterate = breakdowns.copy()
+                elif type(breakdowns[0]) == str:
+                    clusters = breakdowns.copy()
+                    clusters_calculated = True
+                else:
+                    raise ValueError('If breakdowns is a list, then it must be either [[measure_name, ..], ..] (list of lists) or [cluster_1, ..] (list of queries used to extract clusters)')
+            else:
+                measures_to_iterate = [[]]
+        elif breakdowns == 'no':
+            measures_to_iterate = [[]]
+        else:
+            raise ValueError('Breakdown must be either "all", "no" or list')
+        
+        data_pandas = data.to_pandas().sort_index().reset_index()
+        measures_types = data.get_measures_types()
+        if measures_types is not None and 'continuous' in measures_types:
+            for measure in measures_types['continuous']:
+                data_pandas[measure] = data.get_discretized_measures()[measure]
+        
+        if not clusters_calculated:
+            clusters = []
+            if len(measures_to_iterate) == 0:
+                query = 'total'
+                clusters.append(query)
+            else:
+                for measures_set in measures_to_iterate:
+                    if len(measures_set) == 0:
+                        query = 'total'
+                        clusters.append(query)
+                    else:
+                        for measures_values in data_pandas[measures_set].drop_duplicates().values:
+                            str_arr = []
+                            for (measure_name, measure_value) in zip(measures_set, measures_values):
+                                quote = '"' if type(measure_value) == str else ''
+                                str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
+                            query = ' and '.join(str_arr)
+                            clusters.append(query)
+    elif pd.DataFrame:
         df = data.copy()
+        clusters = df['cluster'].drop_duplicates().values
+
+        if breakdowns == 'all':
+            pass
+        if breakdowns == 'no':
+            if 'total' in clusters:
+                clusters = ['total']
+        if type(breakdowns) == list:
+            if type(breakdowns[0]) == list:
+                filtered_clusters = []
+                for measures_set in breakdowns:
+                    for c in clusters:
+                        c_measures = list(map(lambda x: x.split('==')[0].strip(), c.split(' and ')))
+                        if len(set(c_measures).intersection(set(measures_set))) == len(set(c_measures)):
+                            filtered_clusters.append(c)
+                clusters = filtered_clusters.copy()
+            elif type(breakdowns[0]) == str:
+                existing_clusters = set(df['clusters'].values)
+                provided_clusters = set(breakdowns)
+                clusters = existing_clusters.intersection(provided_clusters)
+            else:
+                raise ValueError('In case data is pandas.DataFrame returned from anomeda.fit_trends, breakdowns must be either "all", "no" list of measures to iterate or list of specific clusters')
     else:
         raise ValueError('"data" argument must be either anomeda.DataFrame or pandas.DataFrame returned by anomeda.fit_trends()')
-    
-    if df is None or len(df) == 0:
-        return None 
-    
-    if clusters is None:
-        clusters = df['cluster'].drop_duplicates()
-    
+
     if colors is None:
-        replace = len(clusters) >= len(TABLEAU_COLORS)
-        cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
+            replace = len(clusters) >= len(TABLEAU_COLORS)
+            cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
     
     for c in clusters:
         
-        # reorder features names in accordance to how they sorted in measures names
-        if type(data) == DataFrame: 
-            if c not in ['total', 'skipped']:
-                c = ' and '.join(sorted(c.split(' and '), key=lambda v: measures_names.index(v.split('==')[0].replace('`', ''))))
+        # reorder features names in accordance to how they sorted in measures names 
+        if c not in ['total', 'skipped']:
+            try:
+                c = ' and '.join(sorted(c.split(' and '), key=lambda v: measures_names.index(v.split('==')[0].strip().replace('`', ''))))
+            except ValueError:
+                raise ValueError('Some feature from the cluster {} is not a measure'.format(c))
+            
+        if c not in df['cluster'].values:
+            continue
 
         df_tmp = df[df['cluster'] == c].sort_values(by='trend_start_dt')
 
         if df_tmp.shape[0] == 0:
             raise ValueError(f'Failed to find cluster {c}. Make sure such a breakdown was set during trends fitting.')
         
         x_cluster = []
@@ -855,19 +972,187 @@
         if show_metric and type(data) == DataFrame:
             cluster_info = data._clusters[c]
             plt.plot(cluster_info['index'], cluster_info['values'], color=cluster_c[cluster])
         
     plt.legend()
 
 
+def plot_clusters(
+    data : 'anomeda.DataFrame', 
+    breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
+    metric_propagate : '"zeros" | "ffil" | None' = None,
+    min_cluster_size : 'int | None' = None,
+    max_cluster_size : 'int | None' = None,
+    colors : 'dict' = None
+):
+    """Plot metric in clusters.
+    
+    Plot metric extracted from clusters from anomeda.DataFrame instance.
+    
+    Parameters
+    ----------
+    data : anomeda.DataFrame
+        Object containing clusters to be plotted.
+    breakdowns : 'no' | 'all' | list[str], default 'no'
+        If 'no', the metric is grouped by date points only. 
+        If 'all', all combinations of measures are used to extract and plot clusters. 
+        If list[str], then only specific clusters specified in the list are plotted. 
+        If list[list[str]] then each internal list is a list of measures used to extract clusters.
+    metric_propagate : '"zeros" | "ffil" | None' = None
+        How to propogate aggregated time-series for missing index values.
+        - zeros: 
+            Let metric for missing index be equal 0. For example, aggregated metric values
+                '2024-01-01': 1
+                '2024-01-03': 2
+            Will be propagated as
+                '2024-01-01': 1 
+                '2024-01-02': 0
+                '2024-01-03': 2
+        - ffil: 
+            Let metric for missing index be equal the last observed value. For example, aggregated metric values 
+                '2024-01-01': 1
+                '2024-01-03': 2
+            Will be propagated as
+                '2024-01-01': 1
+                '2024-01-02': 1 
+                '2024-01-03': 2
+        - None: 
+            Use only present metric and index values.
+    min_cluster_size : int, default None
+        Skip clusters whose total size among all date points is less than the value.
+    max_cluster_size : int, default None
+        Skip clusters whose total size among all date points is more than the value.
+    colors : dict, default None
+        Dictionary with a mapping between clusters and colors used in matplotlib.
+        
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> anomeda.plot_clusters(
+    >>>     data, # anomeda.DataFrame
+    >>>     breakdowns=[['measure_a'], ['measure_a', 'measure_b']] # plot clusters extracted using measure_a and a combination of measure_a and measure_b 
+    >>> )
+
+    >>> anomeda.plot_clusters(
+    >>>     data, # anomeda.DataFrame
+    >>>     breakdowns=['measure_a==1', 'measure_a == 1 and measure_b == 2'] # plot two specified clusters 
+    >>> )
+
+    >>> anomeda.plot_clusters(
+    >>>     data, # anomeda.DataFrame
+    >>>     breakdowns='no' # plot a metric grouped by index values only
+    >>> )
+    """
+    if type(data) == DataFrame:
+        pass
+    else:
+        raise ValueError('"data" argument must be an anomeda.DataFrame instance')
+    
+    if data is None or len(data) == 0:
+        return None
+    
+    if min_cluster_size is None:
+        min_cluster_size = -np.inf
+    if max_cluster_size is None:
+        max_cluster_size = np.inf
+    
+    index_name = data.get_index_name()
+    if index_name is None:
+        raise KeyError('not-None "index_name" must be set for anomeda.DataFrame object')
+    
+    metric_name = data.get_metric_name()
+    if metric_name is None:
+        raise KeyError('not-None "metric_name" must be set for anomeda.DataFrame object')
+    
+    agg_func = data.get_agg_func()
+    if agg_func is None:
+        raise KeyError('not-None "agg_func" must be set for anomeda.DataFrame object')
+
+    clusters_calculated = False
+    if breakdowns == 'all':
+        measures_names = data.get_measures_names()
+        measures_to_iterate = [[]]
+        if measures_names is not None and len(measures_names) > 0:
+            for i in range(1, len(measures_names) + 1):
+                for el in combinations(measures_names, i):
+                    measures_to_iterate.append(list(el))
+    elif type(breakdowns) == list:
+        if len(breakdowns) > 0:
+            if type(breakdowns[0]) == list:
+                measures_names = data.get_measures_names()
+                measures_to_iterate = breakdowns.copy()
+            elif type(breakdowns[0]) == str:
+                clusters = breakdowns.copy()
+                clusters_calculated = True
+            else:
+                raise ValueError('If breakdowns is a list, then it must be either [[measure_name, ..], ..] (list of lists) or [cluster_1, ..] (list of queries used to extract clusters)')
+        else:
+            measures_to_iterate = [[]]
+    elif breakdowns == 'no':
+        measures_to_iterate = [[]]
+    else:
+        raise ValueError('Breakdown must be either "all", "no" or list')
+
+    data_pandas = data.to_pandas().sort_index().reset_index()
+    measures_types = data.get_measures_types()
+    if measures_types is not None and 'continuous' in measures_types:
+        for measure in measures_types['continuous']:
+            data_pandas[measure] = data.get_discretized_measures()[measure]
+    columns_to_use = np.append(index_name, metric_name)
+
+    if not clusters_calculated:
+        clusters = []
+        if len(measures_to_iterate) == 0:
+            query = 'total'
+            clusters.append(query)
+        else:
+            for measures_set in measures_to_iterate:
+                if len(measures_set) == 0:
+                    query = 'total'
+                    clusters.append(query)
+                else:
+                    for measures_values in data_pandas[measures_set].drop_duplicates().values:
+                        str_arr = []
+                        for (measure_name, measure_value) in zip(measures_set, measures_values):
+                            quote = '"' if type(measure_value) == str else ''
+                            str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
+                        query = ' and '.join(str_arr)
+                        clusters.append(query)
+
+    if colors is None:
+        replace = len(clusters) >= len(TABLEAU_COLORS)
+        cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
+    
+    for query in clusters:
+        if query == 'total':
+            yseries = data_pandas[columns_to_use].groupby(index_name).agg(agg_func)[metric_name]
+        else:
+            yseries = data_pandas.query(query)[columns_to_use].groupby(index_name).agg(agg_func)[metric_name]
+        
+        if len(yseries) >= min_cluster_size and len(yseries) <= max_cluster_size:
+            yindex = yseries.index.values
+            ydata = yseries.values
+            
+            if metric_propagate is not None:
+                freq = data._index_freq
+                yindex, _, ydata = _propagate_metric(yindex, ydata, strategy=metric_propagate, freq=freq)
+            
+            plt.plot(yindex, ydata, label=query, color=cluster_c[query])
+    if len(clusters) > 0:
+        plt.legend()
+
+
 def fit_trends(
     data : 'anomeda.DataFrame | (numpy.ndarray[int], numpy.ndarray[float]) | (pandas.DatetimeIndex, numpy.ndarray[float])', 
     trend_fitting_conf : 'dict' = {'max_trends': 'auto', 'min_var_reduction': 0.75},
     save_trends : 'bool' = True,
-    breakdown : "'no' | 'all-clusters' | list[str]" = 'no',
+    breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
     metric_propagate : '"zeros" | "ffil" | None' = None,
     min_cluster_size : 'int | None' = None,
     max_cluster_size : 'int | None' = None,
     plot : 'bool' = False,
     df : 'bool' = True,
     verbose : 'bool' = False
 ):
@@ -882,16 +1167,19 @@
     ----------
     data : anomeda.DataFrame | (numpy.ndarray[int], numpy.ndarray[float]) | (pandas.DatetimeIndex, numpy.ndarray[float])
         Object containing metric values. If numpy.ndarray, a tuple of arrays corresponding to x (data points) and y (metric values) respectively.
     trend_fitting_conf : dict, default {'max_trends': 'auto', 'min_var_reduction': 0.75}
         Parameters for calling anomeda.extract_trends() function. It consists of 'max_trends' parameter, which is responsible for the maximum number of trends that you want to identify, and 'min_var_reduction' parameter, which describes what part of variance must be reduced by estimating trends. Values close to 1 will produce more trends since more trends reduce variance more signigicantly. Default is {'max_trends': 'auto', 'min_var_reduction': 0.75}.
     save_trends : 'bool', default True
         If False, return pandas.DataFrame with trends description without assigning it to the anomeda.DataFrame._trends.
-    breakdown : 'no' | 'all-clusters' | list[str], default 'no'
-        If 'no', the metric is grouped by date points only. If 'all-clusters', then all combinations of measures are used to create clusters for fitting trends within them. If list[str], then only combinations of measures specified in the list are used.
+    breakdowns : 'no' | 'all' | list[str], default 'no'
+        If 'no', the metric is grouped by date points only. 
+        If 'all', all combinations of measures are used to extract and plot clusters. 
+        If list[str], then only specific clusters specified in the list are plotted. 
+        If list[list[str]] then each internal list is a list of measures used to extract clusters.
     metric_propagate : '"zeros" | "ffil" | None' = None
         How to propogate aggregated time-series for missing index values.
         - zeros: 
             Let metric for missing index be equal 0. For example, aggregated metric values
                 '2024-01-01': 1
                 '2024-01-03': 2
             Will be propagated as
@@ -925,14 +1213,15 @@
         An object containing information about trends
 
     Examples
     --------
     >>> fitted_trends = anomeda.fit_trends(
             data, 
             trend_fitting_conf={'max_trends': 3}, 
+            breakdowns='all',
             metric_propagate='zeros',
             min_cluster_size=3, 
             plot=True, 
             df=True
         )
     """
     def resp_to_df(resp):
@@ -961,127 +1250,137 @@
         
         agg_func = data.get_agg_func()
         if agg_func is None:
             raise KeyError('not-None "agg_func" must be set for anomeda.DataFrame object')
     
         data_pandas = data.to_pandas().sort_index().reset_index()
 
-        if breakdown == 'all-clusters':
+        clusters_calculated = False
+        if breakdowns == 'all':
             measures_names = data.get_measures_names()
-            if measures_names is None:
-                raise KeyError('not-None "measures_names" must be set for anomeda.DataFrame object')
-            measures_to_iterate = []
-            for i in range(1, len(measures_names) + 1):
-                for el in combinations(measures_names, i):
-                    measures_to_iterate.append(list(el))
-        elif type(breakdown) == list:
-            measures_names = data.get_measures_names()
-            measures_to_iterate = breakdown.copy()
-        elif breakdown == 'no':
-            measures_to_iterate = []
+            measures_to_iterate = [[]]
+            if measures_names is not None and len(measures_names) > 0:
+                for i in range(1, len(measures_names) + 1):
+                    for el in combinations(measures_names, i):
+                        measures_to_iterate.append(list(el))
+        elif type(breakdowns) == list:
+            if len(breakdowns) > 0:
+                if type(breakdowns[0]) == list:
+                    measures_names = data.get_measures_names()
+                    measures_to_iterate = breakdowns.copy()
+                elif type(breakdowns[0]) == str:
+                    clusters = breakdowns.copy()
+                    clusters_calculated = True
+                else:
+                    raise ValueError('If breakdowns is a list, then it must be either [[measure_name, ..], ..] (list of lists) or [cluster_1, ..] (list of queries used to extract clusters)')
+            else:
+                measures_to_iterate = [[]]
+        elif breakdowns == 'no':
+            measures_to_iterate = [[]]
         else:
-            raise ValueError('Breakdown must be either "all-clusters", list or "no"')
+            raise ValueError('Breakdown must be either "all", "no" or list')
         
         measures_types = data.get_measures_types()
         if measures_types is not None and 'continuous' in measures_types:
             for measure in measures_types['continuous']:
                 data_pandas[measure] = data.get_discretized_measures()[measure]
+
+        if not clusters_calculated:
+            clusters = []
+            if len(measures_to_iterate) == 0:
+                query = 'total'
+                clusters.append(query)
+            else:
+                for measures_set in measures_to_iterate:
+                    if len(measures_set) == 0:
+                        query = 'total'
+                        clusters.append(query)
+                    else:
+                        for measures_values in data_pandas[measures_set].drop_duplicates().values:
+                            str_arr = []
+                            for (measure_name, measure_value) in zip(measures_set, measures_values):
+                                quote = '"' if type(measure_value) == str else ''
+                                str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
+                            query = ' and '.join(str_arr)
+                            clusters.append(query)
         
         res_values = {}
         skipped_clusters = 0
         skipped_indeces = []
         total_clusters = 0
         columns_to_use = np.append(index_name, metric_name)
         clusters_storage = {}
         hashed_index = {}
-
-        query = 'total'
         
         yseries = data_pandas[columns_to_use]
         cluster_search_index = yseries.index.values
         yseries = yseries.groupby(index_name).agg(agg_func)[metric_name]
         yindex = yseries.index.values
         ydata = yseries.values
 
         if len(ydata) == 0:
             if save_trends:
                 data._trends = {}
                 data._clusters = {}
                 data._trends_conf = {}
             if df:
                 return None
-
-        clusters_storage[query] = {'index': yindex, 'values': ydata}
-
-        hashable_key = ''.join(list(map(str, cluster_search_index)))
-        hashed_index[hashable_key] = [query]
-        
-        trends = extract_trends(
-            yindex, ydata, 
-            propagation_strategy=metric_propagate,
-            freq=data._index_freq,
-            max_trends=trend_fitting_conf.get('max_trends'), 
-            min_var_reduction=trend_fitting_conf.get('min_var_reduction')
-        )
-        res_values[query] = trends.copy()
         
-        for measures_set in measures_to_iterate:
-            for measures_values in data_pandas[measures_set].drop_duplicates().values:
-                str_arr = []
-                for (measure_name, measure_value) in zip(measures_set, measures_values):
-                    quote = '"' if type(measure_value) == str else ''
-                    str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
-                query = ' and '.join(str_arr)
-                total_clusters += 1
-                
+        for query in clusters:
+            total_clusters += 1
+
+            if query == 'total':
+                yseries = data_pandas[columns_to_use]
+            else:
                 yseries = data_pandas.query(query)[columns_to_use]
-                cluster_search_index = yseries.index.values
-                yseries = yseries.groupby(index_name).agg(agg_func)[metric_name]
-                yindex = yseries.index.values
-                ydata = yseries.values
-
-                clusters_storage[query] = {'index': yindex, 'values': ydata}
-
-                hashable_key = ''.join(list(map(str, cluster_search_index)))
-                if hashable_key in hashed_index:
-                    res_values[query] = res_values[hashed_index[hashable_key][0]].copy()
-                    hashed_index[hashable_key].append(query)
-                else:
-                    hashed_index[hashable_key] = [query]
+            
+            cluster_search_index = yseries.index.values
+            yseries = yseries.groupby(index_name).agg(agg_func)[metric_name]
+            yindex = yseries.index.values
+            ydata = yseries.values
 
-                    if ydata.shape[0] >= min_cluster_size and ydata.shape[0] <= max_cluster_size:
-                        if ydata.shape[0] == 1:
-                            if data._index_is_numeric:
-                                res_values[query] = {
-                                    0: (
-                                        yindex[0], yindex[0] + 1, 
-                                        (1, ydata[0]), 
-                                        (1, ydata[0], 0, ydata[0])
-                                    )
-                                }
-                            else:
-                                res_values[query] = {
-                                    0: (
-                                        pd.Timestamp(yindex[0]), pd.Timestamp(yindex[0]) + pd.Timedelta(1, data._index_freq), 
-                                        (1, ydata[0]), 
-                                        (1, ydata[0], 0, ydata[0])
-                                    )
-                                }
+            clusters_storage[query] = {'index': yindex, 'values': ydata}
+
+            hashable_key = ''.join(list(map(str, cluster_search_index)))
+            if hashable_key in hashed_index and hashed_index[hashable_key][0] in res_values:
+                res_values[query] = res_values[hashed_index[hashable_key][0]].copy()
+                hashed_index[hashable_key].append(query)
+            else:
+                hashed_index[hashable_key] = [query]
+
+                if ydata.shape[0] >= min_cluster_size and ydata.shape[0] <= max_cluster_size:
+                    if ydata.shape[0] == 1:
+                        if data._index_is_numeric:
+                            res_values[query] = {
+                                0: (
+                                    yindex[0], yindex[0] + 1, 
+                                    (1, ydata[0]), 
+                                    (1, ydata[0], 0, ydata[0])
+                                )
+                            }
                         else:
-                            trends = extract_trends(
-                                yindex, ydata, 
-                                propagation_strategy=metric_propagate,
-                                freq=data._index_freq,
-                                max_trends=trend_fitting_conf.get('max_trends'), 
-                                min_var_reduction=trend_fitting_conf.get('min_var_reduction')
-                            )
-                            res_values[query] = trends.copy()
+                            res_values[query] = {
+                                0: (
+                                    pd.Timestamp(yindex[0]), pd.Timestamp(yindex[0]) + pd.Timedelta(1, data._index_freq), 
+                                    (1, ydata[0]), 
+                                    (1, ydata[0], 0, ydata[0])
+                                )
+                            }
                     else:
-                        skipped_clusters += 1
-                        skipped_indeces.append(yindex)
+                        trends = extract_trends(
+                            yindex, ydata, 
+                            propagation_strategy=metric_propagate,
+                            freq=data._index_freq,
+                            max_trends=trend_fitting_conf.get('max_trends'), 
+                            min_var_reduction=trend_fitting_conf.get('min_var_reduction')
+                        )
+                        res_values[query] = trends.copy()
+                else:
+                    skipped_clusters += 1
+                    skipped_indeces.append(yindex)
         if skipped_clusters > 0:
             skipped_indeces = np.unique(np.concatenate(skipped_indeces))
 
             query = 'skipped'
 
             yseries = data_pandas.loc[skipped_indeces, columns_to_use].groupby(index_name).agg(agg_func)[metric_name]
             yindex = yseries.index.values
@@ -1120,26 +1419,26 @@
         res_values = resp_to_df(res_values)
         
         if save_trends:
             data._trends = res_values.copy()
             data._clusters = clusters_storage.copy()
             data._trends_conf = {
                 'trend_fitting_conf': trend_fitting_conf.copy(),
-                'breakdown': breakdown,
+                'breakdown': breakdowns,
                 'min_cluster_size': min_cluster_size,
                 'max_cluster_size': max_cluster_size
             }
             data._hashed_index = hashed_index.copy()
         if plot:
             plot_trends(data)
         if df:
             return res_values
 
     elif type(data) == tuple and type(data[0]) in [pd.DatetimeIndex, np.ndarray] and type(data[1]) == np.ndarray:
-        if breakdown is not None and breakdown != 'no':
+        if breakdowns is not None and breakdowns != 'no':
             raise ValueError('Breakdown may be passed only if provided data is anomeda.DataFrame')
         x, y = data
 
         if len(y) == 0:
             return None
         
         if type(x) == np.ndarray:
```

### Comparing `anomeda-0.1.1/src/anomeda.egg-info/PKG-INFO` & `anomeda-0.1.2/src/anomeda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,15 @@
 
 ```python
 trends = anomeda.fit_trends(
     anomeda_df,
     trend_fitting_conf={'max_trends': 'auto', 'min_var_reduction': 0.75}, # set the number of trends automatically,
                                                                           # try to reduce error variance compared to error of estimating values by 1-line trend by 75%
     breakdown='all-clusters', # fit trends for clusters extracted from all possible sets of measures
-    mettic_propagte='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
+    metric_propagate='zeros', # if some index values are missed after aggregation for a cluster, fill them with zeros
     min_cluster_size=3 # skip small clusters, they all will be combined into 'skipped' cluster
 )
 ```
 
 Typically you will see something like this:
 
 ![anomeda.fit_trends method](docs/img/anomeda_fit_trends_1.png "anomeda.fit_trends method")
@@ -91,14 +91,20 @@
 anomeda.plot_trends(anomeda_df, clusters=['`country`=="Germany"'])
 ```
 
 The output will look like this:
 
 ![anomeda.plot_trends method](docs/img/anomeda_plot_trends_1.png "anomeda.plot_trends method")
 
+If you don't need to *fit trends* since it's a complicated procedure, but you need to take a brief look at the clusters, you may run a different command which simply plots the clusters:
+
+```python
+anomeda.plot_clusters(anomeda_df, clusters=['`country`=="Germany"'])
+```
+
 Of course, you may have no idea which cluster caused the problem and what to plot. Almost always you know only that there is a decrease of an overall metric and you need to find the culprits. Let's utilize another method -- `anomeda.compare_clusters`.
 
 ```python
 anomeda.compare_clusters(
     anomeda_df,
     period1='date < "2024-01-30"',
     period2='date >= "2024-01-30"'
```

### Comparing `anomeda-0.1.1/tests/test_main.py` & `anomeda-0.1.2/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         metric_name=metric_name,
         agg_func=agg_func
     )
     
     assert measures_names == anmd_df.get_measures_names()
     assert measures_types == anmd_df.get_measures_types()
     assert index_name == anmd_df.get_index_name()
-    assert anmd_df._index_is_numeric == False
+    assert anmd_df._index_is_numeric == True
     assert metric_name == anmd_df.get_metric_name()
     assert agg_func == anmd_df.get_agg_func()
 
     dummy_df.set_index('dt', inplace=True)
 
     anmd_df = anomeda.DataFrame(
         dummy_df,
@@ -165,15 +165,18 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
     
     dummy_df.set_index(index_name, inplace=True)
-    dummy_df.index = pd.to_datetime(dummy_df.index)
+    try:
+        dummy_df.index.astype('str').astype('int')
+    except BaseException:
+        dummy_df.index = pd.to_datetime(dummy_df.index)
 
     assert dummy_df.equals(anmd_df.to_pandas())
 
 
 def test_find_anomalies():
     
     dummy_df = pd.DataFrame({'dt': [0, 1, 2, 3], 'a': [10, 20, 20, 30], 'b': [0.1, 0.2, 0.3, 0.2], 'metric': [10.5, 12.6, 8.3, 9.8]})
@@ -195,18 +198,18 @@
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     anomeda.fit_trends(anmd_df)
     anomeda.find_anomalies(anmd_df)
     anomeda.find_anomalies(anmd_df, anomalies_conf={'p_large': 1, 'p_low': 1})
-    anomeda.find_anomalies(anmd_df, clusters=['total'])
+    anomeda.find_anomalies(anmd_df, breakdowns=['total'])
 
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters')
-    anomeda.find_anomalies(anmd_df, clusters=['`a`==20'])
+    anomeda.fit_trends(anmd_df, breakdowns='all')
+    anomeda.find_anomalies(anmd_df, breakdowns=['`a`==20'])
     anomeda.find_anomalies(anmd_df, return_all_points=True)
 
     x = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     y = np.array([11.2, 10.4, 10.2, 30.1, 10.2, 10., 11., 10.2, 10.9, 10.5, 11.1])
 
     anomeda.find_anomalies((x, y), trend_fitting_conf={'max_trends': 1, 'n_neighbors': 3})
     anomeda.find_anomalies((x, y), return_all_points=True, trend_fitting_conf={'max_trends': 1, 'n_neighbors': 3})
@@ -231,17 +234,17 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     anomeda.fit_trends(anmd_df)
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters')
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters', metric_propagate='zeros')
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters', metric_propagate='ffil')
+    anomeda.fit_trends(anmd_df, breakdowns='all')
+    anomeda.fit_trends(anmd_df, breakdowns='all', metric_propagate='zeros')
+    anomeda.fit_trends(anmd_df, breakdowns='all', metric_propagate='ffil')
 
     x = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     y = np.array([11.2, 10.4, 10.2, 30.1, 10.2, 10., 11., 10.2, 10.9, 10.5, 11.1])
 
     anomeda.fit_trends((x, y))
     anomeda.fit_trends((x, y), metric_propagate='zeros')
     anomeda.fit_trends((x, y), metric_propagate='ffil')
@@ -282,17 +285,18 @@
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     trends = anomeda.fit_trends(anmd_df)
     anomeda.plot_trends(anmd_df)
-    anomeda.plot_trends(anmd_df, clusters=['total'])
+    anomeda.plot_trends(anmd_df, breakdowns=['total'])
     
     trends = anomeda.fit_trends((x, y))
+    print(trends)
     anomeda.plot_trends(trends)
 
 
 def test_compare_clusters():
 
     dummy_df = pd.DataFrame({'dt': ["2023-12-01", "2023-12-01", "2024-02-01", "2024-02-01"], 'a': [10, 20, 20, 30], 'b': [0.1, 0.2, 0.3, 0.2], 'metric': [10.5, 12.6, 8.3, 9.8]})
     
@@ -312,17 +316,17 @@
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"')
 
-    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', clusters=['total'])
+    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['total'])
 
-    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdown='all-clusters', clusters=['`a`==20'])
+    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['`a`==20'])
 
 
 def test_empty_df():
 
     dummy_df = pd.DataFrame({'dt': [], 'a': [], 'b': [], 'metric': []})
     
     index_name = 'dt'
@@ -340,15 +344,15 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     anomeda.fit_trends(anmd_df)
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters')
+    anomeda.fit_trends(anmd_df, breakdowns='all')
     anomeda.plot_trends(anmd_df)
 
 
 def test_one_element_df():
 
     dummy_df = pd.DataFrame({'dt': [1], 'a': [10], 'b': [0.1], 'metric': [10]})
     
@@ -367,15 +371,15 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     anomeda.fit_trends(anmd_df)
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters')
+    anomeda.fit_trends(anmd_df, breakdowns='all')
     anomeda.plot_trends(anmd_df)
 
 
 def test_two_elements_df():
 
     dummy_df = pd.DataFrame({'dt': [1, 2], 'a': [10, 20], 'b': [0.1, 0.2], 'metric': [10, 20]})
     
@@ -394,15 +398,15 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     anomeda.fit_trends(anmd_df)
-    anomeda.fit_trends(anmd_df, breakdown='all-clusters')
+    anomeda.fit_trends(anmd_df, breakdowns='all')
     anomeda.plot_trends(anmd_df)
 
 
 def test_datetime_index():
 
     df = pd.DataFrame({
         'dt': ['2024-01-01', '2024-01-03', '2024-01-04', '2024-01-05', '2024-01-03', '2024-01-03'],
@@ -420,25 +424,25 @@
         metric_name='metric', # dummy metric, always 1
         agg_func='sum' # function that is used to aggregate metric
     )
 
     anomeda.fit_trends(
         anomeda_df,
         metric_propagate=None,
-        breakdown='all-clusters'
+        breakdowns='all'
     )
     anomeda.fit_trends(
         anomeda_df,
         metric_propagate='zeros',
-        breakdown='all-clusters'
+        breakdowns='all'
     )
     anomeda.fit_trends(
         anomeda_df,
         metric_propagate='ffil',
-        breakdown='all-clusters'
+        breakdowns='all'
     )
 
     anomeda.find_anomalies(anomeda_df)
     anomeda.plot_trends(anomeda_df)
 
 
 def test_anomeda_df_without_measures():
```

