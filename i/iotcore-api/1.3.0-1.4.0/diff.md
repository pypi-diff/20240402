# Comparing `tmp/iotcore_api-1.3.0-py3-none-any.whl.zip` & `tmp/iotcore_api-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18068 bytes, number of entries: 7
+Zip file size: 17986 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 iotcoreapi/__init__.py
 -rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 iotcoreapi/exceptions.py
--rw-r--r--  2.0 unx    57113 b- defN 80-Jan-01 00:00 iotcoreapi/iotcoreapi.py
--rw-r--r--  2.0 unx     1684 b- defN 80-Jan-01 00:00 iotcoreapi/nan_treatment.py
--rw-r--r--  2.0 unx    34780 b- defN 80-Jan-01 00:00 iotcore_api-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 iotcore_api-1.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      543 b- defN 16-Jan-01 00:00 iotcore_api-1.3.0.dist-info/RECORD
-7 files, 95604 bytes uncompressed, 17114 bytes compressed:  82.1%
+-rw-r--r--  2.0 unx    57123 b- defN 80-Jan-01 00:00 iotcoreapi/iotcoreapi.py
+-rw-r--r--  2.0 unx     1206 b- defN 80-Jan-01 00:00 iotcoreapi/nan_treatment.py
+-rw-r--r--  2.0 unx    34780 b- defN 80-Jan-01 00:00 iotcore_api-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 iotcore_api-1.4.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      543 b- defN 16-Jan-01 00:00 iotcore_api-1.4.0.dist-info/RECORD
+7 files, 95136 bytes uncompressed, 17032 bytes compressed:  82.1%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: iotcoreapi/iotcoreapi.py
 Comment: 
 
 Filename: iotcoreapi/nan_treatment.py
 Comment: 
 
-Filename: iotcore_api-1.3.0.dist-info/METADATA
+Filename: iotcore_api-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: iotcore_api-1.3.0.dist-info/WHEEL
+Filename: iotcore_api-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: iotcore_api-1.3.0.dist-info/RECORD
+Filename: iotcore_api-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iotcoreapi/iotcoreapi.py

```diff
@@ -108,15 +108,15 @@
         Returns:
             response: json or dataframe
         """
         if output_format == 'dataframe' or output_format == 'dataframe_table':
             if response:
                 response = self._json_normalize_check(response)
                 if time_format == 'datetime':
-                    response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True)
+                    response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True, errors='coerce')
                 if nan_method is not None:
                     response = nan_treatment(response, nan_method)
                 if output_format == 'dataframe_table':
                     try:
                         response = pd.pivot_table(response, values='value', index='timeStamp', columns=['uid'],
                                                   aggfunc='sum')
                     except:
@@ -737,15 +737,15 @@
                                         output_format: str = 'dataframe',
                                         time_format: str = 'datetime',
                                         nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
-            filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
+            filter_txt: text filters to search tags in installation. If None, will take all tags
             output_format : Result given in 'dataframe' or 'json'or dataframe_table. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             dataframe or json:
                 columns:
```

## iotcoreapi/nan_treatment.py

```diff
@@ -10,42 +10,24 @@
         df: dataframe in wide format
         method: 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'
 
     Returns:
         df
     """
     # Cambiar formato de long a wide para correcto análisis por columnas and set timestamp as index
-    df.set_index('timeStamp', inplace=True)
-    df = df.pivot(columns='uid', values='value')
+    df = df.pivot_table(index='timeStamp', columns='uid', values='value', aggfunc='last', dropna=False)
     numeric_cols = df.select_dtypes(include=np.number).columns
-    def interpolate(df):
-        if df.index.dtype == 'datetime64[ns]' or df.index.dtype == 'timedelta64[ns]':
-            return df.interpolate(method='time')
-        else:
-            return df.interpolate(method='linear')
-
-    def ffill(df):
-        return df.fillna(method='ffill')
-
-    def bfill(df):
-        return df.fillna(method='bfill')
-
-    def mean(df):
-        return df.fillna(value=df.mean())
-
-    def fill_with_zeros(df):
-        return df.fillna(value=0.0)
 
     switch = {
         'interpolate': df[numeric_cols].interpolate(),
-        'bfill': df[numeric_cols].ffill().bfill(),
-        'ffill': df[numeric_cols].ffill().bfill(),
+        'bfill': df[numeric_cols].bfill(),
+        'ffill': df[numeric_cols].ffill(),
         'mean': df[numeric_cols].fillna(value=df.mean()),
         'zerofill': df[numeric_cols].fillna(value=0.0)
     }
     try:
         df[numeric_cols] = switch[method]
         df.reset_index(inplace=True)
         df = df.melt(id_vars=['timeStamp'], var_name='uid', value_name='value')
         return df
     except KeyError:
-        raise ValueError("Invalid method. Please use 'interpolate', 'bfill', 'ffill', 'mean', or 'zerofill'.")
+        raise ValueError("Invalid method. Please use 'interpolate', 'bfill', 'ffill', 'mean', or 'zerofill'.")
```

## Comparing `iotcore_api-1.3.0.dist-info/METADATA` & `iotcore_api-1.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: IoT core connection methods and utilities in Python
 Keywords: iotcoreapi,goaigua
 Author: Ricardo Gomez-Aldaravi
 Author-email: ricardo.gomez.aldaravi@idrica.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

