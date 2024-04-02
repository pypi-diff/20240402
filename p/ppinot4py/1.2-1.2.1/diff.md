# Comparing `tmp/ppinot4py-1.2.tar.gz` & `tmp/ppinot4py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppinot4py-1.2.tar", last modified: Mon Nov  1 08:53:43 2021, max compression
+gzip compressed data, was "ppinot4py-1.2.1.tar", last modified: Tue Apr  2 09:52:11 2024, max compression
```

## Comparing `ppinot4py-1.2.tar` & `ppinot4py-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.133491 ppinot4py-1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-11-01 08:53:28.000000 ppinot4py-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18465 2021-11-01 08:53:43.133491 ppinot4py-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17984 2021-11-01 08:53:28.000000 ppinot4py-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.129491 ppinot4py-1.2/ppinot4py/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.129491 ppinot4py-1.2/ppinot4py/computers/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/conditions_computer.py
--rw-r--r--   0 runner    (1001) docker     (121)    16629 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/metrics_computer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.129491 ppinot4py-1.2/ppinot4py/computers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8856 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/tests/test_conditions_computer.py
--rw-r--r--   0 runner    (1001) docker     (121)    28012 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/computers/tests/test_metrics_computer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.129491 ppinot4py-1.2/ppinot4py/model/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7514 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/measures.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/states.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.133491 ppinot4py-1.2/ppinot4py/model/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-11-01 08:53:28.000000 ppinot4py-1.2/ppinot4py/model/tests/test_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 08:53:43.129491 ppinot4py-1.2/ppinot4py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18465 2021-11-01 08:53:42.000000 ppinot4py-1.2/ppinot4py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-11-01 08:53:42.000000 ppinot4py-1.2/ppinot4py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 08:53:42.000000 ppinot4py-1.2/ppinot4py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-01 08:53:42.000000 ppinot4py-1.2/ppinot4py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-11-01 08:53:42.000000 ppinot4py-1.2/ppinot4py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-01 08:53:43.133491 ppinot4py-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-11-01 08:53:28.000000 ppinot4py-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18524 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17984 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.270609 ppinot4py-1.2.1/ppinot4py/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.270609 ppinot4py-1.2.1/ppinot4py/computers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/conditions_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/metrics_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.270609 ppinot4py-1.2.1/ppinot4py/computers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/tests/test_conditions_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33314 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/computers/tests/test_metrics_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/ppinot4py/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/ppinot4py/model/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/ppinot4py/model/tests/test_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/ppinot4py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18524 2024-04-02 09:52:11.000000 ppinot4py-1.2.1/ppinot4py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 09:52:11.000000 ppinot4py-1.2.1/ppinot4py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:52:11.000000 ppinot4py-1.2.1/ppinot4py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 09:52:11.000000 ppinot4py-1.2.1/ppinot4py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 09:52:11.000000 ppinot4py-1.2.1/ppinot4py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:52:11.274608 ppinot4py-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 09:52:01.000000 ppinot4py-1.2.1/setup.py
```

### Comparing `ppinot4py-1.2/LICENSE` & `ppinot4py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ppinot4py-1.2/PKG-INFO` & `ppinot4py-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ppinot4py
-Version: 1.2
+Version: 1.2.1
 Summary: PPINOT for Python (ppinot4py)
 Home-page: https://github.com/isa-group/ppinot4py
 Author: ISA Group
 Author-email: resinas@us.es
 License: GPL 3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: business-duration
 
 # What is PPINot4Py?
 
 PPINot4Py is a Python implementation of [PPINot](https://github.com/isa-group/ppinot), used to compute process performance indicators (PPIs) for event logs.
 
 **A quick example**
 
@@ -454,8 +456,7 @@
 
 ``` python
 create_fine_to_send_fine = TimeMeasure('`concept:name` == "Create Fine"', '`concept:name` == "Send Fine"')
 create_to_send_fine_90_days= DerivedMeasure("create_to_send_fine < days90", 
                                     {"create_to_send_fine":   create_fine_to_send_fine, "days90": pd.Timedelta(days=90)})
 measure_computer(avg_create_to_send_fine_90_days, df, time_grouper=pd.Grouper(freq='1Y'))
 ```
-
```

### Comparing `ppinot4py-1.2/README.md` & `ppinot4py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ppinot4py-1.2/ppinot4py/computers/conditions_computer.py` & `ppinot4py-1.2.1/ppinot4py/computers/conditions_computer.py`

 * *Files identical despite different names*

### Comparing `ppinot4py-1.2/ppinot4py/computers/metrics_computer.py` & `ppinot4py-1.2.1/ppinot4py/computers/metrics_computer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from ppinot4py.computers.conditions_computer import condition_computer
 from ppinot4py.model import (
     CountMeasure, 
     DataMeasure, 
     TimeMeasure, 
     AggregatedMeasure,
-    DerivedMeasure,
-    BusinessDuration  
+    DerivedMeasure
 )
-from ppinot4py.model.measures import _MeasureDefinition
+from ppinot4py.model.measures import _MeasureDefinition, RollingWindow
 
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from pandas.api.types import is_timedelta64_dtype as is_timedelta
 from pandas.api.types import is_numeric_dtype, is_bool_dtype
 import numpy as np
 from copy import copy
@@ -40,16 +39,16 @@
         self.activity_column = activity_column
 
 
 def measure_computer(measure, dataframe, log_configuration: LogConfiguration = None, time_grouper = None):
     """ General computer.
     
     Args:    
-        - measure: Measure, it will call different computers depending on the type.
-        - dataframe: Base dataframe we want to use.
+        - measure: The measure definition that will be computed
+        - dataframe: Dataframe that contains the event log to compute the measure
         - log_configuration (optional): LogConfiguration that specifies the names of special columns of the log
         - time_grouper (optional): Time grouper (https://pandas.pydata.org/docs/user_guide/timeseries.html)
             without the key. If the measure is aggregated, it groups the result by instance end time
             
     Returns:
         - Series: Series with pairs of case ID - Data
 
@@ -105,14 +104,20 @@
 def time_compute(dataframe, measure, log_configuration):
     operation = measure.single_instance_agg_function
     precondition = measure.precondition
     time_measure_type = measure.time_measure_type
     from_condition = measure.from_condition
     to_condition = measure.to_condition
     is_first = measure.first_to
+    time_unit = measure.time_unit
+    
+    id_case = log_configuration.id_case
+    transition_column = log_configuration.transition_column
+    activity_column = log_configuration.activity_column
+    time_column = log_configuration.time_column
     
     id_case = log_configuration.id_case
     transition_column = log_configuration.transition_column
     activity_column = log_configuration.activity_column
     time_column = log_configuration.time_column
     
 
@@ -128,16 +133,21 @@
     removed_timezones = pd.to_datetime(filtered_dataframe[time_column], utc=True)
     dataframe_to_work = pd.DataFrame({'id':filtered_dataframe[id_case], 't': removed_timezones})
 
     if(time_measure_type == 'LINEAR'): 
         final_result = _linear_time_compute(dataframe_to_work, A_condition, B_condition, is_first, 'id', 't', measure)   
     elif(time_measure_type == 'CYCLIC'):
         final_result = _cyclic_time_compute(dataframe_to_work, A_condition, B_condition, operation, 'id', 't', measure)
-       
-    return final_result.reindex(dataframe[id_case].unique())
+
+    result_reindex = final_result.reindex(dataframe[id_case].unique())
+
+    if(time_unit != None):
+        return result_reindex/ np.timedelta64(1, time_unit.value)
+    else:
+        return result_reindex
 
 def _linear_time_compute(dataframeToWork, from_condition, to_condition, is_first, id_case, time_column, measure):
     filtered_dataframe_A = dataframeToWork[from_condition]
     from_values = filtered_dataframe_A.groupby(id_case)[time_column].first()
     
     if(is_first):
         to_values = _first_to_after_from(from_condition, to_condition, dataframeToWork[id_case], dataframeToWork[time_column])
@@ -204,15 +214,18 @@
 
 def _apply_aggregation(operation, grouped_df):
 
     if not isinstance(operation, str):
         raise ValueError('Aggregation function must be a string: sum, min, max, avg or groupby')
 
     if(operation.upper() == 'SUM'):
-        result = grouped_df.sum(min_count=1)
+        if isinstance(grouped_df, pd.core.window.rolling.Rolling):
+            result = grouped_df.sum()
+        else:
+            result = grouped_df.sum(min_count=1)
 
     elif(operation.upper() == "MIN"):
         result = grouped_df.min()
 
     elif(operation.upper() == "MAX"):
         result = grouped_df.max()
 
@@ -282,33 +295,37 @@
     base_measure = measure.base_measure
     filter_to_apply = measure.filter_to_apply
     operation = measure.single_instance_agg_function
     data_grouper = measure.grouper
     id_case = log_configuration.id_case
     time_column = log_configuration.time_column
 
+    if ((data_grouper is not None) and (len(data_grouper) > 0)) and (isinstance(time_grouper, RollingWindow)):
+        raise ValueError('A rolling time_grouper cannot be used with an AggregatedMeasure with group by')
+
     is_time = False
 
     base_values = measure_computer(base_measure, dataframe, log_configuration)
     
     case_end = dataframe.groupby(id_case)[time_column].last()
+
     
     if((filter_to_apply is not None) and filter_to_apply != ""):
         filter_condition = measure_computer(filter_to_apply, dataframe, log_configuration)
         # We assume the filtered_condition is fine. Maybe we could do
         # some sanity checking here.
         base_values = base_values[filter_condition]
         case_end = case_end[filter_condition]
 
     # Case end could also be configurable
-    internal_df = pd.DataFrame({'data':base_values, 'case_end':case_end})
+    internal_df = pd.DataFrame({'data':base_values, 'case_end':case_end}).sort_values(by='case_end')
 
     if not is_datetime(internal_df['case_end']):
         internal_df['case_end'] = pd.to_datetime(internal_df['case_end'], utc=True)
-    
+      
     if is_timedelta(internal_df['data'].dtype):
         internal_df['data'] = internal_df['data'].dt.total_seconds()
         #internal_df['data_seconds'] = internal_df['data_seconds'].fillna(0).astype(float)
         is_time = True
 
     groupers = []
     if (data_grouper is not None):
@@ -323,39 +340,67 @@
             
                 internal_df[gr_key] = measure_computer(gr, dataframe, log_configuration)
                 groupers.append(gr_key)
             else:
                 groupers.append(gr)
 
     if time_grouper is not None:
-        internal_time_grouper = copy(time_grouper)
-        internal_time_grouper.key = 'case_end'
-        groupers.append(internal_time_grouper)
+        temp_grouper = None
+        if isinstance(time_grouper, str):
+            temp_grouper = pd.Grouper(freq=time_grouper)
+        elif isinstance(time_grouper, RollingWindow):
+            if not time_grouper.apply_to_cases:
+                offset = pd.tseries.frequencies.to_offset(time_grouper.window)
+                temp_grouper = pd.Grouper(freq=offset.base)
+        else:
+            temp_grouper = time_grouper
 
+        if temp_grouper is not None:
+            internal_time_grouper = copy(temp_grouper)
+            internal_time_grouper.key = 'case_end'
+            groupers.append(internal_time_grouper)
+    
     if len(groupers) > 0:
         result_grouped = internal_df.groupby(groupers)
     else:
         result_grouped = internal_df
 
-    final_result = _apply_aggregation(operation, result_grouped)
+    if not isinstance(time_grouper, RollingWindow):
+        final_result = _apply_aggregation(operation, result_grouped["data"])
+    else:
+        roll_window = time_grouper.window
+        roll_min_period = time_grouper.min_period
+        roll_closed = time_grouper.closed
+        if time_grouper.apply_to_cases:
+            rolling_result = result_grouped.rolling(roll_window, min_periods=roll_min_period, on='case_end', closed=roll_closed)
+            final_result = _apply_aggregation(operation, rolling_result)
+        else:
+            if operation.upper() == 'AVG':
+                rolling_sum = result_grouped.sum().rolling(roll_window, min_periods=roll_min_period, closed=roll_closed).sum()
+                rolling_count = result_grouped.count().rolling(roll_window, min_periods=roll_min_period, closed=roll_closed).sum()
+                final_result = rolling_sum / rolling_count
+            else:   
+                agg_result = _apply_aggregation(operation, result_grouped)
+                rolling_result = agg_result.rolling(roll_window, min_periods=roll_min_period, closed=roll_closed)
+                final_result = _apply_aggregation(operation, rolling_result)
 
     if(operation.upper() == "GROUPBY"):
         is_time = False
 
-    if len(final_result) > 1:
+    if isinstance(final_result, pd.DataFrame):
+        final_result = final_result['data']
+
+    if isinstance(final_result, pd.Series):   
         if is_time == True:
-            final_result = final_result['data'].apply(lambda x: datetime.timedelta(seconds = x) if not np.isnan(x) else np.nan)
-        else:
-            final_result = final_result['data']
-        #final_result = final_result.drop('case_end', axis=0, errors='ignore')
+            final_result = final_result.apply(lambda x: datetime.timedelta(seconds = x) if not np.isnan(x) else np.nan)
+            #final_result = final_result.drop('case_end', axis=0, errors='ignore')
     else:
         if is_time == True:
-            final_result = datetime.timedelta(seconds = final_result['data']) if not np.isnan(final_result['data']) else np.nan
-        else:
-            final_result = final_result['data']
+            final_result = datetime.timedelta(seconds = final_result) if not np.isnan(final_result) else np.nan
+
 
     return final_result
 
 def derived_compute(dataframe, measure, log_configuration, time_grouper=None):
     
     function = measure.function_expression
     measure_map = measure.measure_map
```

### Comparing `ppinot4py-1.2/ppinot4py/computers/tests/test_conditions_computer.py` & `ppinot4py-1.2.1/ppinot4py/computers/tests/test_conditions_computer.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,9 +195,7 @@
 
         precondition = TimeInstantCondition(RuntimeState.START, AppliesTo.ACTIVITY, "'Queued'")
 
         with pytest.raises(ValueError):
                 condition_computer(dataframeLinear, "case:concept:name", precondition, 'concept:name', 'lifecycle:transition')
 
         
-
-
```

### Comparing `ppinot4py-1.2/ppinot4py/model/__init__.py` & `ppinot4py-1.2.1/ppinot4py/model/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 from .measures import (
     CountMeasure,
     TimeMeasure,
     DataMeasure,
     AggregatedMeasure, 
     DerivedMeasure,
-    BusinessDuration
+    BusinessDuration,
+    RollingWindow,
+    TimeUnit
 )
 
 from .states import (
     DataObjectState,
     RuntimeState
 )
 
@@ -25,11 +27,13 @@
     'DataCondition',
     'SeriesCondition',
     'CountMeasure',
     'TimeMeasure',
     'DataMeasure',
     'AggregatedMeasure',
     'DerivedMeasure',
+    'TimeUnit',
     'BusinessDuration',
+    'RollingWindow',
     'DataObjectState',
     'RuntimeState'
 ]
```

### Comparing `ppinot4py-1.2/ppinot4py/model/conditions.py` & `ppinot4py-1.2.1/ppinot4py/model/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#Possibly not needed
 from .states import DataObjectState
 import enum
 
 class AppliesTo(enum.Enum):
     PROCESS = 1
     DATA = 2
     ACTIVITY = 3
```

### Comparing `ppinot4py-1.2/ppinot4py/model/measures.py` & `ppinot4py-1.2.1/ppinot4py/model/measures.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .conditions import TimeInstantCondition
 import datetime
+import enum
 
 def _time_instance_auto_wrap(condition):
     if condition is None:
         return None
 
     if isinstance(condition, str):
         condition = TimeInstantCondition(condition)
@@ -16,14 +17,21 @@
     if agg == "MIN":
         return "minimum"
     if agg == "MAX":
         return "maximum"
     if agg == "SUM":
         return "sum"
 
+class TimeUnit(enum.Enum):
+    WEEK = "W"
+    DAY = "D"
+    HOUR = "h"
+    MINUTE = "m"
+    SECOND = "s"
+
 class _MeasureDefinition():
     def __init__(self):
         super().__init__()
         self.id = None
 
 class CountMeasure(_MeasureDefinition):
     """Measure to calc how many times a condition happened.
@@ -66,39 +74,41 @@
         return f"the {first_text} value of {self.data_content_selection}{precondition_text}"
 
 class TimeMeasure(_MeasureDefinition):
     """Measure to calc the time elapsed between A condition and B condition.
     
     Args:
     
-            - from_condition: Condition where you want to start counting, defined as A
-            - to_condition: End condition, defined as B
-            - time_measure_type: Linear in case just want a simple A-B calc, Cyclic in case you want to count 
-                all pairs A-B appearances
-            - single_instance_agg_function: Only in Cyclic mode. Type of operation applied to our dataset, 
-                can be MAX, MIN, SUM, or AVG. 
-            - first_to: Only in Linear mode. True to take first appareance of B, false to take last appareance of B
-            - precondition: Filter to previusly apply to our dataset. Note that, in this case, this precondition
-                            is not a time instant condition, but a data condition (i.e., it is directly checked with
-                            the values of the attributes of each event)
-            - business_duration: Business days specifications
+        - from_condition: Condition where you want to start counting, defined as A
+        - to_condition: End condition, defined as B
+        - time_measure_type: Linear in case just want a simple A-B calc, Cyclic in case you want to count 
+            all pairs A-B appearances
+        - single_instance_agg_function: Only in Cyclic mode. Type of operation applied to our dataset, 
+            can be MAX, MIN, SUM, or AVG. 
+        - first_to: Only in Linear mode. True to take first appareance of B, false to take last appareance of B
+        - precondition: Filter to previusly apply to our dataset. Note that, in this case, this precondition
+                        is not a time instant condition, but a data condition (i.e., it is directly checked with
+                        the values of the attributes of each event)
+        - business_duration: Business days and hours specification
+        - time_unit: The time unit used to return the value.
     """
 
     def __init__(self, from_condition, to_condition, 
                     time_measure_type = 'LINEAR', single_instance_agg_function = 'SUM', 
-                         first_to = False, precondition = None, business_duration = None):
+                         first_to = False, precondition = None, business_duration = None, time_unit = None):
         super().__init__()
   
         self.from_condition = _time_instance_auto_wrap(from_condition)
         self.to_condition = _time_instance_auto_wrap(to_condition)
         self.time_measure_type = time_measure_type
         self.single_instance_agg_function = single_instance_agg_function
         self.precondition = precondition
         self.first_to = first_to
         self.business_duration = business_duration
+        self.time_unit = time_unit
         
     def __repr__(self):
         return f"TimeMeasure ( from={self.from_condition}, to={self.to_condition} )"
 
     def __str__(self):
         precon_text = f" if {self.precondition}" if self.precondition is not None else ""
         first_to_text = "first" if self.first_to else "last"
@@ -186,10 +196,29 @@
         elif(self.unit_hour == 'min'):
             time_delta_type = lambda x: (datetime.timedelta(minutes = x))
         elif(self.unit_hour == 'sec'):
             time_delta_type = lambda x: (datetime.timedelta(seconds = x))
 
         return time_delta_type
 
+class RollingWindow():
+    """Window applied to the data to group with a moving window.
+    
+    Args:
+        - window: Size of the moving window, could be a number or a time expression ('7D'). If it is a number, then apply_to_cases must be true.
+        - apply_to_cases: Returns the moving window for each case instead of based on the window frequency.
+        - min_period: Minimum number of observations in window required to have a value 
+        - closed: Make the interval closed on the ‘right’, ‘left’, ‘both’ or ‘neither’ endpoints.
+    """
+    def __init__(self, window, apply_to_cases=False, min_period=None, closed=None):
+        if (isinstance(window, int) or (isinstance(window,float) and window.is_integer())) and not apply_to_cases:
+            raise ValueError('If window is an integer, apply_to_cases must be True')
+
+        self.window = window
+        self.apply_to_cases = apply_to_cases
+        self.min_period = min_period
+        self.closed = closed
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ppinot4py-1.2/ppinot4py/model/states.py` & `ppinot4py-1.2.1/ppinot4py/model/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,8 @@
   
 RuntimeState.START = RuntimeState('START')
 RuntimeState.END = RuntimeState('END')
 
 class Type(enum.Enum):
     FOLLOWS = 1
     LEADSTO = 2
-    LEADSTOCYCLIC = 3
-
-
+    LEADSTOCYCLIC = 3
```

### Comparing `ppinot4py-1.2/ppinot4py/model/tests/test_measures.py` & `ppinot4py-1.2.1/ppinot4py/model/tests/test_measures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ppinot4py.model import *
+import pytest
 
 def test_count_text():
     c = CountMeasure("ACT == 'open'")
     assert f"{c}" == "the number of times ACT == 'open'"
 
 def test_linear_time_text():
     t = TimeMeasure("ACT == 'open'", "ACT == 'close'")
@@ -18,7 +19,11 @@
     assert f"{a}" == "the average of the number of times ACT == 'open' grouped by the last value of PROJECT"
 
 def test_derived_text():
     c = CountMeasure("ACT == 'open'")
     t = TimeMeasure("ACT == 'open'", "ACT == 'close'", first_to=True)
     d = DerivedMeasure("c/t", {"c": c, "t": t})
     assert f"{d}" == "the function c/t where c is the number of times ACT == 'open', t is the duration between the first time instant when ACT == 'open' and the first time instant when ACT == 'close'"
+
+def test_invalid_rolling_window():
+    with pytest.raises(ValueError):
+        RollingWindow(window=2)
```

### Comparing `ppinot4py-1.2/ppinot4py.egg-info/PKG-INFO` & `ppinot4py-1.2.1/ppinot4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ppinot4py
-Version: 1.2
+Version: 1.2.1
 Summary: PPINOT for Python (ppinot4py)
 Home-page: https://github.com/isa-group/ppinot4py
 Author: ISA Group
 Author-email: resinas@us.es
 License: GPL 3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: business-duration
 
 # What is PPINot4Py?
 
 PPINot4Py is a Python implementation of [PPINot](https://github.com/isa-group/ppinot), used to compute process performance indicators (PPIs) for event logs.
 
 **A quick example**
 
@@ -454,8 +456,7 @@
 
 ``` python
 create_fine_to_send_fine = TimeMeasure('`concept:name` == "Create Fine"', '`concept:name` == "Send Fine"')
 create_to_send_fine_90_days= DerivedMeasure("create_to_send_fine < days90", 
                                     {"create_to_send_fine":   create_fine_to_send_fine, "days90": pd.Timedelta(days=90)})
 measure_computer(avg_create_to_send_fine_90_days, df, time_grouper=pd.Grouper(freq='1Y'))
 ```
-
```

### Comparing `ppinot4py-1.2/ppinot4py.egg-info/SOURCES.txt` & `ppinot4py-1.2.1/ppinot4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppinot4py-1.2/setup.py` & `ppinot4py-1.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ppinot4py", 
-    version="1.2",
+    version="1.2.1",
     author="ISA Group",
     author_email="resinas@us.es",
     description="PPINOT for Python (ppinot4py)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/isa-group/ppinot4py",
     packages=setuptools.find_packages(),
```

