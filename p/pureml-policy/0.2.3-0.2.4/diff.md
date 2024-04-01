# Comparing `tmp/pureml_policy-0.2.3.tar.gz` & `tmp/pureml_policy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml_policy-0.2.3.tar", max compression
+gzip compressed data, was "pureml_policy-0.2.4.tar", max compression
```

## Comparing `pureml_policy-0.2.3.tar` & `pureml_policy-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0        0 2023-10-18 00:21:27.590116 pureml_policy-0.2.3/README.md
--rwxr-xr-x   0        0        0       93 2023-11-22 11:03:38.485998 pureml_policy-0.2.3/pureml_policy/__init__.py
--rwxr-xr-x   0        0        0     4867 2024-03-30 08:39:48.841499 pureml_policy-0.2.3/pureml_policy/assignments.py
--rwxr-xr-x   0        0        0     1365 2024-03-22 19:47:15.239380 pureml_policy-0.2.3/pureml_policy/frameworks.py
--rwxr-xr-x   0        0        0     3834 2024-03-30 08:34:59.684132 pureml_policy-0.2.3/pureml_policy/grade.py
--rwxr-xr-x   0        0        0     3751 2024-01-12 06:25:06.372381 pureml_policy-0.2.3/pureml_policy/policy.py
--rwxr-xr-x   0        0        0    14479 2024-03-30 09:23:26.732780 pureml_policy-0.2.3/pureml_policy/policy_eval.py
--rwxr-xr-x   0        0        0     2736 2024-03-22 19:47:15.242909 pureml_policy-0.2.3/pureml_policy/reports.py
--rwxr-xr-x   0        0        0      812 2024-03-28 19:08:35.573960 pureml_policy-0.2.3/pureml_policy/reslut_formation.py
--rwxr-xr-x   0        0        0     3252 2024-03-28 19:08:35.583740 pureml_policy-0.2.3/pureml_policy/schema.py
--rwxr-xr-x   0        0        0      208 2024-02-05 16:00:51.776729 pureml_policy-0.2.3/pureml_policy/utils/routes.py
--rwxr-xr-x   0        0        0     1268 2024-03-30 13:36:11.340883 pureml_policy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 pureml_policy-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2023-10-18 00:21:27.590116 pureml_policy-0.2.4/README.md
+-rwxr-xr-x   0        0        0       93 2023-11-22 11:03:38.485998 pureml_policy-0.2.4/pureml_policy/__init__.py
+-rwxr-xr-x   0        0        0     4867 2024-03-31 07:43:49.649916 pureml_policy-0.2.4/pureml_policy/assignments.py
+-rwxr-xr-x   0        0        0     1365 2024-03-22 19:47:15.239380 pureml_policy-0.2.4/pureml_policy/frameworks.py
+-rwxr-xr-x   0        0        0     3834 2024-03-31 07:43:49.659223 pureml_policy-0.2.4/pureml_policy/grade.py
+-rwxr-xr-x   0        0        0     3751 2024-01-12 06:25:06.372381 pureml_policy-0.2.4/pureml_policy/policy.py
+-rwxr-xr-x   0        0        0    14681 2024-04-01 23:29:37.951197 pureml_policy-0.2.4/pureml_policy/policy_eval.py
+-rwxr-xr-x   0        0        0     2736 2024-03-22 19:47:15.242909 pureml_policy-0.2.4/pureml_policy/reports.py
+-rwxr-xr-x   0        0        0      812 2024-03-31 07:43:49.239857 pureml_policy-0.2.4/pureml_policy/reslut_formation.py
+-rwxr-xr-x   0        0        0     3252 2024-03-31 07:43:49.254088 pureml_policy-0.2.4/pureml_policy/schema.py
+-rwxr-xr-x   0        0        0      208 2024-02-05 16:00:51.776729 pureml_policy-0.2.4/pureml_policy/utils/routes.py
+-rwxr-xr-x   0        0        0     1268 2024-04-01 23:15:26.320352 pureml_policy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 pureml_policy-0.2.4/PKG-INFO
```

### Comparing `pureml_policy-0.2.3/pureml_policy/assignments.py` & `pureml_policy-0.2.4/pureml_policy/assignments.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/frameworks.py` & `pureml_policy-0.2.4/pureml_policy/frameworks.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/grade.py` & `pureml_policy-0.2.4/pureml_policy/grade.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/policy.py` & `pureml_policy-0.2.4/pureml_policy/policy.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/policy_eval.py` & `pureml_policy-0.2.4/pureml_policy/policy_eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,42 +35,43 @@
     dataset: Any = None
     sensitive_features: Union[None, Any] = None
     y_true: Any = None
     y_pred: Any = None
     y_pred_scores: Any = None
     framework_name : Any = None
     model_config = ConfigDict(validate_assignment=True, arbitrary_types_allowed=True)
-
+    metrics_list: Any = None
+    framework_data: Any = None
     def load_dataset(self):
         self.dataset = dataset.fetch(self.label_dataset)
         if self.dataset:
-            logger.info(f"Dataset Fetched Successfully: {self.dataset}")
-            print("[bold green] Succesfully fetched the dataset")
+            logger.info(f"Dataset Fetched Successfully: {self.label_dataset}")
+            print(f"[bold green] Succesfully fetched the Dataset: {self.label_dataset}")
         else:
-            print("[bold red] Dataset not fetched")
+            print(f"[bold red] Dataset not fetched: {self.label_dataset}")
             raise Exception("Dataset fetching failed")
         
     def load_predictor(self):
         module_path = self.predictor_path.replace(".py", "")
         module_import = import_module(module_path)
 
         predictor_class = getattr(module_import, "Predictor")
 
         self.predictor = predictor_class()
         logger.info(f"Predict files fetched successfully: {self.predictor}")
-        print("[bold green] Succesfully fetched the predictor")
+        print(f"[bold green] Succesfully fetched the Predictor")
 
     def load_model(self):
         model_fetching = model.fetch(self.label_model)
         if model_fetching:
             self.predictor.load_models()
-            logger.info(f"Model Fetched Successfully: {self.predictor}")
-            print("[bold green] Succesfully fetched the model")
+            logger.info(f"Model Fetched Successfully: {self.label_model}")
+            print(f"[bold green] Succesfully fetched the Model: {self.label_model}")
         else:
-            print("[bold red] Model not fetched")
+            print(f"[bold red] Model not fetched: {self.label_model}")
             raise Exception("Model fetching failed")
 
         # self.predictor.load_models()
         # logger.info(f"Model Fetched Successfully: {self.predictor}")
         # print("[bold green] Succesfully fetched the model")
 
     
@@ -78,16 +79,17 @@
         #self.framework = get_framework_details(self.framework_name)
         #metrics_data = get_framework_details(self.framework_name)
         #metrics_list = [key.split('.')[-1] for key in metrics_data]
         #self.framework = {metric: 0.8 for metric in metrics_list}
         
         self.framework = framework_list["custom_policy_to_run_all_metrics"]
         #print(f"Metrics: {list(self.framework.keys())}")
+        self.framework_data = list(self.framework.keys())
         print("[bold green] Succesfully fetched the Metrics ")
-        logger.info(f"Metrics Fetched Successfully: {list(self.framework.keys())}")
+        logger.info(f"Metrics Fetched Successfully: {self.framework_data}")
         return list(self.framework.keys())
     
     # def assigning_framework_to_model(self):
     #     complete_features  = ['complete']
     #     sensitive_features = self.load_sensitive_features()
     #     if isinstance(sensitive_features, np.ndarray):
     #         sensitive_features_list = np.unique(sensitive_features)
@@ -145,15 +147,15 @@
         else:
             return None
 
     def evaluate(self):
         y_pred = self.get_y_pred()
         y_true = self.get_y_true()
         sensitive_features = self.get_sensitive_features()
-        policies = self.load_framework()
+        policies = self.framework_data
         grader = Grader(references=y_true, predictions=y_pred,
                         sensitive_features=sensitive_features, framework=self.framework, metrics=policies)
 
         return   grader.compute()
 
     def evaluate_subsets(self):
         if self.sensitive_features is None:  # If No Sensitive Features are given
@@ -181,15 +183,15 @@
                         keys = {'index' : str(int(key))}
 
                 key_tuple  = str(key_tuple)
                 if key_tuple not in values_subsets_all:
                     values_subsets_all[key_tuple] = {'columns' : keys}
 
                 #sensitive_features = self.get_sensitive_features()
-                policies = self.load_framework()
+                policies = self.framework_data
                 if 'disparate_impact' in policies:
                     policies.remove('disparate_impact')
                     new_policies = ['disparate_impact']    
                     subset_name = get_unique_sensitive_for_disparate_impact(sensitive_features)
                     sensitive_features_1 = self.get_sensitive_features()
                     y_pred = self.get_y_pred()
                     y_true = self.get_y_true()
```

### Comparing `pureml_policy-0.2.3/pureml_policy/reports.py` & `pureml_policy-0.2.4/pureml_policy/reports.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/reslut_formation.py` & `pureml_policy-0.2.4/pureml_policy/reslut_formation.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pureml_policy/schema.py` & `pureml_policy-0.2.4/pureml_policy/schema.py`

 * *Files identical despite different names*

### Comparing `pureml_policy-0.2.3/pyproject.toml` & `pureml_policy-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml-policy"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>","Thrinadhreddy Manubothu <m.thrinadhreddy@gmail.com"]
 readme = "README.md"
 
 packages = [{include = "pureml_policy"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pureml_policy-0.2.3/PKG-INFO` & `pureml_policy-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml-policy
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

