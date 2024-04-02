# Comparing `tmp/obsinthe-0.0.1.tar.gz` & `tmp/obsinthe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsinthe-0.0.1.tar", max compression
+gzip compressed data, was "obsinthe-0.0.2.tar", max compression
```

## Comparing `obsinthe-0.0.1.tar` & `obsinthe-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    10767 2024-03-12 08:34:34.610560 obsinthe-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2024-03-16 20:49:21.445270 obsinthe-0.0.1/obsinthe/alerts/__init__.py
--rw-r--r--   0        0        0     2597 2024-03-16 21:26:02.968241 obsinthe-0.0.1/obsinthe/alerts/grouping.py
--rw-r--r--   0        0        0      461 2024-03-16 20:51:58.249890 obsinthe-0.0.1/obsinthe/deps.py
--rw-r--r--   0        0        0     1683 2024-03-12 08:34:34.610560 obsinthe-0.0.1/obsinthe/openshift/symptoms.py
--rw-r--r--   0        0        0       82 2024-03-12 08:34:34.610560 obsinthe-0.0.1/obsinthe/prometheus/__init__.py
--rw-r--r--   0        0        0     6125 2024-03-12 08:34:34.611560 obsinthe-0.0.1/obsinthe/prometheus/client.py
--rw-r--r--   0        0        0    13391 2024-03-16 20:44:24.926432 obsinthe-0.0.1/obsinthe/prometheus/data.py
--rw-r--r--   0        0        0     6415 2024-03-15 14:22:32.490265 obsinthe-0.0.1/obsinthe/prometheus/loader.py
--rw-r--r--   0        0        0      220 2024-03-13 08:48:30.757290 obsinthe-0.0.1/obsinthe/testing/prometheus/__init__.py
--rw-r--r--   0        0        0     3641 2024-03-15 14:22:32.493265 obsinthe-0.0.1/obsinthe/testing/prometheus/alerts.py
--rw-r--r--   0        0        0     6985 2024-03-14 15:58:16.316398 obsinthe-0.0.1/obsinthe/testing/prometheus/builder.py
--rw-r--r--   0        0        0     1765 2024-03-13 16:36:00.559546 obsinthe-0.0.1/obsinthe/testing/prometheus/client.py
--rw-r--r--   0        0        0      418 2024-03-12 08:34:34.611560 obsinthe-0.0.1/obsinthe/utils/jupyter.py
--rw-r--r--   0        0        0     3857 2024-03-13 12:58:00.771010 obsinthe-0.0.1/obsinthe/utils/time.py
--rw-r--r--   0        0        0     1241 2024-03-16 21:25:10.376036 obsinthe-0.0.1/obsinthe/vis/alerts.py
--rw-r--r--   0        0        0      807 2024-03-16 21:26:02.997240 obsinthe-0.0.1/obsinthe/vis/clustering.py
--rw-r--r--   0        0        0     1249 2024-03-18 12:16:29.381746 obsinthe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 obsinthe-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10767 2024-03-12 08:34:34.610560 obsinthe-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-16 20:49:21.445270 obsinthe-0.0.2/obsinthe/alerts/__init__.py
+-rw-r--r--   0        0        0     2597 2024-03-16 21:26:02.968241 obsinthe-0.0.2/obsinthe/alerts/grouping.py
+-rw-r--r--   0        0        0      461 2024-03-16 20:51:58.249890 obsinthe-0.0.2/obsinthe/deps.py
+-rw-r--r--   0        0        0     1683 2024-03-12 08:34:34.610560 obsinthe-0.0.2/obsinthe/openshift/symptoms.py
+-rw-r--r--   0        0        0       82 2024-03-12 08:34:34.610560 obsinthe-0.0.2/obsinthe/prometheus/__init__.py
+-rw-r--r--   0        0        0     6125 2024-03-12 08:34:34.611560 obsinthe-0.0.2/obsinthe/prometheus/client.py
+-rw-r--r--   0        0        0    14504 2024-04-02 16:13:31.363148 obsinthe-0.0.2/obsinthe/prometheus/data.py
+-rw-r--r--   0        0        0     6684 2024-04-02 16:13:31.364148 obsinthe-0.0.2/obsinthe/prometheus/loader.py
+-rw-r--r--   0        0        0      220 2024-03-13 08:48:30.757290 obsinthe-0.0.2/obsinthe/testing/prometheus/__init__.py
+-rw-r--r--   0        0        0     3641 2024-03-15 14:22:32.493265 obsinthe-0.0.2/obsinthe/testing/prometheus/alerts.py
+-rw-r--r--   0        0        0     6985 2024-03-14 15:58:16.316398 obsinthe-0.0.2/obsinthe/testing/prometheus/builder.py
+-rw-r--r--   0        0        0     1765 2024-03-13 16:36:00.559546 obsinthe-0.0.2/obsinthe/testing/prometheus/client.py
+-rw-r--r--   0        0        0      418 2024-03-12 08:34:34.611560 obsinthe-0.0.2/obsinthe/utils/jupyter.py
+-rw-r--r--   0        0        0     3857 2024-03-13 12:58:00.771010 obsinthe-0.0.2/obsinthe/utils/time.py
+-rw-r--r--   0        0        0     1241 2024-03-16 21:25:10.376036 obsinthe-0.0.2/obsinthe/vis/alerts.py
+-rw-r--r--   0        0        0      807 2024-03-18 17:49:01.381766 obsinthe-0.0.2/obsinthe/vis/clustering.py
+-rw-r--r--   0        0        0     1249 2024-04-02 16:13:35.799167 obsinthe-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 obsinthe-0.0.2/PKG-INFO
```

### Comparing `obsinthe-0.0.1/LICENSE` & `obsinthe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/alerts/grouping.py` & `obsinthe-0.0.2/obsinthe/alerts/grouping.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/openshift/symptoms.py` & `obsinthe-0.0.2/obsinthe/openshift/symptoms.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/prometheus/client.py` & `obsinthe-0.0.2/obsinthe/prometheus/client.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/prometheus/data.py` & `obsinthe-0.0.2/obsinthe/prometheus/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,59 +86,61 @@
         df = pd.DataFrame(data=data)
         if df.empty:
             return None
 
         return RangeDataset(df)
 
     def to_range_intervals_ds(
-        self, threshold: timedelta = DEFAULT_RESOLUTION
+        self, resolution: timedelta = DEFAULT_RESOLUTION
     ) -> "RangeIntervalsDataset":
         """Convert into RangeIntervalsDataset.
 
+        Args:
+            resolution (int, optional): The resolution value used to determine the
+            intervals. Defaults to `DEFAULT_RESOLUTION`.
+
         It doesn't use the TS values, just determines the intervals for times
         the values were present.
 
         It preserves the original rows, just replaces the values column with the
         intervals.
 
-        Args:
-            threshold (int, optional): The threshold value used to determine the
-            intervals in seconds. Defaults to `DEFAULT_RESOLUTION`.
+        The end of each interval is calculated as last timestamp + resolution.
 
         Returns:
             RangeIntervalsDataset: A new RangeIntervalsDataset instance.
         """
 
         df = self.df.copy()
 
-        threshold_s = threshold.total_seconds()
+        resolution_s = resolution.total_seconds()
+
+        def values_to_intervals(vs):
+            return np_timestamps_to_intervals(vs[0::2], resolution_s)
 
         # we use vs[0::2] as we care only about timestamps: assuming values being all
         # ones as in alerts case.
-        intervals = df["values"].apply(
-            lambda vs: np_timestamps_to_intervals(vs[0::2], threshold_s)
-        )
+        intervals = df["values"].apply(values_to_intervals)
 
         df["intervals"] = intervals
         df.drop(columns=["values"], inplace=True)
         return RangeIntervalsDataset(df)
 
-    def to_intervals_ds(self, threshold: timedelta) -> "IntervalsDataset":
+    def to_intervals_ds(self, resolution: timedelta) -> "IntervalsDataset":
         """Convert into IntervalsDataset.
 
-        It doesn't use the TS values, just determines the intervals for times
-        the values were present.
+        Applies `to_range_intervals_ds` to identify the intervals and then
+        expands them into separate rows.
 
-        It preserves the original rows, just replaces the values column with the
-        intervals.
+        See `to_range_intervals_ds` for arguments details.
 
         Returns:
             IntervalsDataset: A new IntervalsDataset instance.
         """
-        return self.to_range_intervals_ds(threshold).to_intervals_ds()
+        return self.to_range_intervals_ds(resolution).to_intervals_ds()
 
 
 class RangeIntervalsDataset(DatasetBase):
     def to_intervals_ds(self) -> "IntervalsDataset":
         """Expand into a IntervalsDataset.
 
         Each interval is represented as a row in the DataFrame, with the start
@@ -229,14 +231,33 @@
         ).apply(lambda df: list(zip(df["start"], df["end"])))
 
         intervals.reset_index(inplace=True)
         intervals.drop("interval_label", axis=1, inplace=True)
 
         return IntervalsDataset(intervals)
 
+    def correct_for_resolution(self, resolution: timedelta = DEFAULT_RESOLUTION):
+        """Correct the end times of the intervals.
+
+        When turning a time series into intervals, the end times are determined
+        by the last timestamp in the series. In reality, however, the interval
+        ended sometimes after the last timestamp. This method corrects the end,
+        so we avoid zero-length intervals.
+
+        Args:
+            resolution (timedelta, optional): The resolution value used to
+            determine the intervals. Defaults to `DEFAULT_RESOLUTION`.
+
+        Returns:
+            IntervalsDataset: A new IntervalsDataset instance.
+        """
+        df = self.df.copy()
+        df["end"] = df["end"] + resolution
+        return IntervalsDataset(df)
+
 
 class DatasetCollection:
     def __init__(self, datasets: List[DatasetBase]):
         self.datasets = datasets
 
     def __getitem__(self, idx):
         return self.datasets[idx]
@@ -252,14 +273,21 @@
 
     def fmap(self, fn):
         return DatasetCollection([fn(ds) for ds in self.datasets])
 
     def query(self, *args, **kwargs):
         return self.fmap(lambda ds: ds.query(*args, **kwargs))
 
+    def flatten(self):
+        if len(self.datasets) == 0:
+            raise ValueError("No datasets to flatten")
+        df = pd.concat([ds.df for ds in self.datasets], ignore_index=True)
+        cls = type(self.datasets[0])
+        return cls(df)
+
 
 def extract_columns_data(raw_data, columns):
     if columns is None:
         return raw_data
 
     ret, extra = {}, {}
```

### Comparing `obsinthe-0.0.1/obsinthe/prometheus/loader.py` & `obsinthe-0.0.2/obsinthe/prometheus/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from obsinthe.utils import time as time_utils
 
 from .client import Client
 from .data import DatasetCollection
 from .data import DatasetType
 from .data import InstantDataset
+from .data import IntervalsDataset
 from .data import RangeDataset
 from .data import raw_to_ds
 
 
 def digest(string):
     return sha256(string.encode("utf8")).hexdigest()
 
@@ -41,14 +42,15 @@
             return data
 
 
 class ParquetFileCache:
     DS_TYPES = {
         "InstantDataset": InstantDataset,
         "RangeDataset": RangeDataset,
+        "IntervalsDataset": IntervalsDataset,
         "DataFrame": pd.DataFrame,
     }
 
     def __init__(self, cache_dir: str):
         self.cache_dir = cache_dir
 
     def with_cache(self, cache_key: list, func: Callable):
@@ -96,24 +98,41 @@
         if cache_dir:
             self.json_cache = JsonFileCache(cache_dir)
             self.parquet_cache = ParquetFileCache(cache_dir)
         else:
             self.json_cache = None
             self.parquet_cache = None
 
-    def query(self, query, time, ds_type: Optional[DatasetType] = None, cache_key=None):
+    def query(
+        self,
+        query,
+        time,
+        ds_type: Optional[DatasetType] = None,
+        cache_key=None,
+        post_process: Optional[Callable] = None,
+    ):
         if cache_key:
             if not isinstance(cache_key, list):
                 cache_key = [cache_key, time.isoformat()]
-        return self.with_cache(
+        else:
+            cache_key = [None]  # no caching, but keep for consistency
+
+        ds = self.with_cache(
             "parquet",
             cache_key,
             lambda: raw_to_ds(self.client.query(query, time=time), ds_type=ds_type),
         )
 
+        if post_process:
+            ds = self.with_cache(
+                "parquet", cache_key + ["post"], lambda: post_process(ds)
+            )
+
+        return ds
+
     def interval_query(
         self,
         query: str,
         start: str,
         end: str,
         cache_key: Optional[str] = None,
         ds_type: Optional[DatasetType] = None,
@@ -157,34 +176,30 @@
                 cache_keys = [cache_key, interval_end.isoformat(), sub_items]
 
                 ds = self.query(
                     query,
                     interval_end,
                     ds_type,
                     cache_keys,
+                    post_process,
                 )
-                if ds is not None:
-                    # make sure the ds_type is determined: will be used later.
-                    ds_type = type(ds)
-                if post_process:
-                    ds = self.with_cache(
-                        "parquet", cache_keys + ["post"], lambda: post_process(ds)
-                    )
 
                 if ds is not None:
                     day_data.append(ds)
 
             if day_data:
+                # make sure the ds_type is determined: will be used later.
+                ds_type_ = type(day_data[0])
                 day_data_dfs = [ds.df for ds in day_data]
                 df = pd.concat(day_data_dfs, ignore_index=True).copy()
                 if "timestamp" not in df.columns:  # in case of range df
                     df["timestamp"] = pd.to_datetime(interval_end)
-                data.append(ds_type(df))
+                data.append(ds_type_(df))
 
-        return data
+        return DatasetCollection(data)
 
     def with_cache(self, format: str, key: Optional[list], func: Callable):
         if format == "json":
             cache = self.json_cache
         elif format == "parquet":
             cache = self.parquet_cache
         else:
```

### Comparing `obsinthe-0.0.1/obsinthe/testing/prometheus/alerts.py` & `obsinthe-0.0.2/obsinthe/testing/prometheus/alerts.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/testing/prometheus/builder.py` & `obsinthe-0.0.2/obsinthe/testing/prometheus/builder.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/testing/prometheus/client.py` & `obsinthe-0.0.2/obsinthe/testing/prometheus/client.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/utils/time.py` & `obsinthe-0.0.2/obsinthe/utils/time.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/vis/alerts.py` & `obsinthe-0.0.2/obsinthe/vis/alerts.py`

 * *Files identical despite different names*

### Comparing `obsinthe-0.0.1/obsinthe/vis/clustering.py` & `obsinthe-0.0.2/obsinthe/vis/clustering.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,8 +26,8 @@
                 name=f"grouping: {c}",
                 mode="markers",
                 marker=dict(size=2),
                 text=ac.one_hot[c_pts].index,
             )
         )
 
-    fig.show()
+    return fig
```

### Comparing `obsinthe-0.0.1/pyproject.toml` & `obsinthe-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obsinthe"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = []
 packages = [
   {include = "obsinthe"},
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `obsinthe-0.0.1/PKG-INFO` & `obsinthe-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinthe
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
```

