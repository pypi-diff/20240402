# Comparing `tmp/wolta-0.1.2.tar.gz` & `tmp/wolta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.2.tar", last modified: Mon Apr  1 16:20:19 2024, max compression
+gzip compressed data, was "wolta-0.1.3.tar", last modified: Tue Apr  2 19:15:40 2024, max compression
```

## Comparing `wolta-0.1.2.tar` & `wolta-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.097100 wolta-0.1.2/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    13850 2024-04-01 16:20:19.096029 wolta-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    12695 2024-04-01 16:18:46.000000 wolta-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 16:20:19.097100 wolta-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1185 2024-04-01 16:19:12.000000 wolta-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.057578 wolta-0.1.2/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.2/wolta/__init__.py
--rw-rw-rw-   0        0        0     7562 2024-04-01 16:18:15.000000 wolta-0.1.2/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.2/wolta/feature_tools.py
--rw-rw-rw-   0        0        0     4332 2024-03-30 23:38:39.000000 wolta-0.1.2/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.2/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.094949 wolta-0.1.2/wolta.egg-info/
--rw-rw-rw-   0        0        0    13850 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 19:15:40.486689 wolta-0.1.3/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    14041 2024-04-02 19:15:40.486689 wolta-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12883 2024-04-02 19:14:48.000000 wolta-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:15:40.486689 wolta-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2024-04-02 19:15:28.000000 wolta-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:15:40.450525 wolta-0.1.3/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.3/wolta/__init__.py
+-rw-rw-rw-   0        0        0     7564 2024-04-01 19:35:23.000000 wolta-0.1.3/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.3/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0     5858 2024-04-02 19:10:08.000000 wolta-0.1.3/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.3/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:15:40.485669 wolta-0.1.3/wolta.egg-info/
+-rw-rw-rw-   0        0        0    14041 2024-04-02 19:15:40.000000 wolta-0.1.3/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-02 19:15:40.000000 wolta-0.1.3/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:15:40.000000 wolta-0.1.3/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 19:15:40.000000 wolta-0.1.3/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-02 19:15:40.000000 wolta-0.1.3/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.2/LICENSE.txt` & `wolta-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.2/PKG-INFO` & `wolta-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -331,16 +331,19 @@
 ### do_voting
 
 **Returns**: list of 1D numpy arrays
 
 **Parameters**:
 * y_pred_list, _list of 1D numpy arrays_
 * combinations, _list of int lists_, it holds the indexes from y_pred_list for each combination
+* strategy, {'avg', 'mode'}, default by, 'avg'
 
-This function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+If 'avg' is selected then this function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+<br>
+If 'mode' is selected then for every sample, the predicts are collected and then mode is found one by one.
 
 ```python
 import numpy as np
 from wolta.model_tools import do_voting, do_combinations
 
 y_pred_1 = np.load('one.npy')
 y_pred_2 = np.load('two.npy')
```

### Comparing `wolta-0.1.2/README.md` & `wolta-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -310,16 +310,19 @@
 ### do_voting
 
 **Returns**: list of 1D numpy arrays
 
 **Parameters**:
 * y_pred_list, _list of 1D numpy arrays_
 * combinations, _list of int lists_, it holds the indexes from y_pred_list for each combination
+* strategy, {'avg', 'mode'}, default by, 'avg'
 
-This function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+If 'avg' is selected then this function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+<br>
+If 'mode' is selected then for every sample, the predicts are collected and then mode is found one by one.
 
 ```python
 import numpy as np
 from wolta.model_tools import do_voting, do_combinations
 
 y_pred_1 = np.load('one.npy')
 y_pred_2 = np.load('two.npy')
```

### Comparing `wolta-0.1.2/setup.py` & `wolta-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.1.2/wolta/data_tools.py` & `wolta-0.1.3/wolta/data_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import os
-
-
 def col_types(df, print_columns=False):
     types = []
 
     columns = list(df.columns)
     for i in range(len(columns)):
         sub_type = str(type(df.iloc[0, i]))[8: -2].replace('numpy.', '')
         types.append(sub_type)
@@ -251,14 +248,16 @@
             main_df = pd.concat(dfs)
             del dfs
 
         return main_df
 
 
 def create_chunks(path, sample_amount, target_dir=None, print_description=False, chunk_name='part'):
+    import os
+
     with open(path, 'r', newline='') as f:
         lines = f.readlines()
         headers = lines[0]
 
         part = 0
         loc = 1
```

### Comparing `wolta-0.1.2/wolta/feature_tools.py` & `wolta-0.1.3/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.2/wolta/model_tools.py` & `wolta-0.1.3/wolta/model_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,31 +97,83 @@
     return ['acc', 'f1', 'hamming', 'jaccard', 'log', 'mcc', 'precision', 'recall', 'zol']
 
 
 def get_avg_options():
     return ['micro', 'macro', 'binary', 'weighted', 'samples']
 
 
-def do_voting(y_pred_list, combinations):
-    results = []
+def do_voting(y_pred_list, combinations, strategy='avg'):
+    if strategy == 'avg':
+        results = []
+
+        for comb in combinations:
+            y_sum = None
+
+            for index in comb:
+                if y_sum is None:
+                    y_sum = y_pred_list[index]
+                else:
+                    y_sum += y_pred_list[index]
+
+            y_sum = y_sum / len(comb)
+            y_sum = y_sum.astype(int)
+            results.append(y_sum)
+
+        return results
+
+    elif strategy == 'mode':
+        from math import ceil
+        import numpy as np
+
+        results = []
+
+        for comb in combinations:
+            selected = []
+            for index in comb:
+                selected.append(y_pred_list[index])
+
+            stack = np.concatenate(selected, axis=1)
+            del selected
+
+            req_min = ceil(len(list(stack[0])) / 2)
+            length = stack.shape[0]
+            modes = []
+
+            for i in range(length):
+                result = 0
+                max_times = 0
+                min_space = max_times + 1
+                row = list(stack[i])
+
+                while len(row) > 0:
+                    loc = 0
+                    obj = row[0]
+                    times = 0
+
+                    while loc < len(row):
+                        if obj == row[loc]:
+                            del row[loc]
+                            times += 1
+                        else:
+                            loc += 1
+
+                    if times > max_times:
+                        result = obj
+                        max_times = times
+                        min_space = max_times + 1
+
+                    if max_times >= req_min or len(row) < min_space:
+                        break
 
-    for comb in combinations:
-        y_sum = None
+                modes.append(result)
 
-        for index in comb:
-            if y_sum is None:
-                y_sum = y_pred_list[index]
-            else:
-                y_sum += y_pred_list[index]
-
-        y_sum = y_sum / len(comb)
-        y_sum = y_sum.astype(int)
-        results.append(y_sum)
+            modes = np.array(modes)
+            results.append(modes)
 
-    return results
+        return results
 
 
 def do_combinations(indexes, min_item, max_item):
     import itertools
     combinations = []
 
     for i in range(min_item, max_item + 1):
```

### Comparing `wolta-0.1.2/wolta/progressive_tools.py` & `wolta-0.1.3/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.2/wolta.egg-info/PKG-INFO` & `wolta-0.1.3/wolta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -331,16 +331,19 @@
 ### do_voting
 
 **Returns**: list of 1D numpy arrays
 
 **Parameters**:
 * y_pred_list, _list of 1D numpy arrays_
 * combinations, _list of int lists_, it holds the indexes from y_pred_list for each combination
+* strategy, {'avg', 'mode'}, default by, 'avg'
 
-This function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+If 'avg' is selected then this function makes sum of matrices, then divides it the amount of matrices and finally makes whole matrix as int value.
+<br>
+If 'mode' is selected then for every sample, the predicts are collected and then mode is found one by one.
 
 ```python
 import numpy as np
 from wolta.model_tools import do_voting, do_combinations
 
 y_pred_1 = np.load('one.npy')
 y_pred_2 = np.load('two.npy')
```

