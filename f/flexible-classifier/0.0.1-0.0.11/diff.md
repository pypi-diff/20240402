# Comparing `tmp/flexible_classifier-0.0.1.tar.gz` & `tmp/flexible_classifier-0.0.11.tar.gz`

## Comparing `flexible_classifier-0.0.1.tar` & `flexible_classifier-0.0.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/src/flexible_classifier/__init__.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/src/flexible_classifier/classifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/tests/test.py
--rw-r--r--   0        0        0   131249 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/tests/data/Test.csv
--rw-r--r--   0        0        0   425369 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/tests/data/Train.csv
--rw-r--r--   0        0        0   210076 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/tests/data/ds_salaries.csv
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/LICENSE
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 flexible_classifier-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/src/flexible_classifier/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/src/flexible_classifier/classifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/tests/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/tests/test.py
+-rw-r--r--   0        0        0   131249 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/tests/data/Test.csv
+-rw-r--r--   0        0        0   425369 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/tests/data/Train.csv
+-rw-r--r--   0        0        0   210076 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/tests/data/ds_salaries.csv
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/LICENSE
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 flexible_classifier-0.0.11/PKG-INFO
```

### Comparing `flexible_classifier-0.0.1/src/flexible_classifier/classifier.py` & `flexible_classifier-0.0.11/src/flexible_classifier/classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,34 +56,39 @@
     cv = 3
   logistic_param_grid = {"max_iter": [1000]}
   if df.shape[0] < big_size_dataset:
     logistic_param_grid["C"] = [0.5, 1, 1.5]
   logistic_regression  = GridSearchCV(
     LogisticRegression(max_iter=1000),
     logistic_param_grid,
-    cv = 2
+    cv = 2,
+    refit=True
   )
   models_to_test = [
     ('Logistic Regression', logistic_regression, cv),
   ]
   if df.shape[0] < big_size_dataset:
     random_forest = GridSearchCV(
          RandomForestClassifier(),
          {'n_estimators': [200], 'max_depth' : [4, 8]},
-         cv = 2)
+         cv = 2,
+         refit=True
+         )
     models_to_test.append(('Random Forest', random_forest, cv))
     svm_model = GridSearchCV(
          svm.SVC(),
          {'C': [1, 10]},
-         cv = 2)
+         cv = 2,
+         refit=True)
     models_to_test.append(('SVM', svm_model, cv))
   results = []
   for name, model, cv in models_to_test:
     pipeline = Pipeline(steps=[('preprocessor', preprocessor),
                                 ('model', model)
                               ])
     score = cross_val_score(pipeline, X, y, cv=cv, scoring='accuracy').mean()
+    pipeline.fit(X, y)
     results.append((score, name, pipeline))
   results.sort()
   best_result = results[0]
   print(f"Model is {best_result[1]}. With average accuracy {best_result[0]}")
   return best_result[2]
```

### Comparing `flexible_classifier-0.0.1/tests/data/Test.csv` & `flexible_classifier-0.0.11/tests/data/Test.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/tests/data/Train.csv` & `flexible_classifier-0.0.11/tests/data/Train.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/tests/data/ds_salaries.csv` & `flexible_classifier-0.0.11/tests/data/ds_salaries.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/.gitignore` & `flexible_classifier-0.0.11/.gitignore`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/LICENSE` & `flexible_classifier-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/README.md` & `flexible_classifier-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.1/pyproject.toml` & `flexible_classifier-0.0.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "flexible_classifier"
-version = "0.0.1"
+version = "0.0.11"
 authors = [
   { name="Marko Golovko", email="markgolovko@gmail.com" },
 ]
 description = "Classifier pipeline that can be used to train and evaluate classification models on various datasets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flexible_classifier-0.0.1/PKG-INFO` & `flexible_classifier-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flexible_classifier
-Version: 0.0.1
+Version: 0.0.11
 Summary: Classifier pipeline that can be used to train and evaluate classification models on various datasets
 Project-URL: Homepage, https://github.com/GameRuiner/classifier-pipeline
 Project-URL: Issues, https://github.com/GameRuiner/classifier-pipeline/issues
 Author-email: Marko Golovko <markgolovko@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

