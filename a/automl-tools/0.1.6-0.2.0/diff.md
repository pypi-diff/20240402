# Comparing `tmp/automl_tools-0.1.6.tar.gz` & `tmp/automl_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automl_tools-0.1.6.tar", last modified: Mon Feb  1 15:15:36 2021, max compression
+gzip compressed data, was "automl_tools-0.2.0.tar", last modified: Tue Apr  2 05:24:58 2024, max compression
```

## Comparing `automl_tools-0.1.6.tar` & `automl_tools-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-02-01 15:15:36.395418 automl_tools-0.1.6/
--rw-rw-rw-   0        0        0     5512 2021-02-01 15:15:36.396414 automl_tools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3653 2021-01-26 16:09:02.000000 automl_tools-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2021-02-01 15:15:36.352418 automl_tools-0.1.6/automl_tools/
--rw-rw-rw-   0        0        0       63 2021-01-23 19:50:20.000000 automl_tools-0.1.6/automl_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-01 15:15:36.394416 automl_tools-0.1.6/automl_tools/functions/
--rw-rw-rw-   0        0        0        0 2021-01-19 18:16:45.000000 automl_tools-0.1.6/automl_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    10171 2021-02-01 14:47:10.000000 automl_tools-0.1.6/automl_tools/functions/imputation.py
--rw-rw-rw-   0        0        0     4684 2021-01-23 16:46:24.000000 automl_tools-0.1.6/automl_tools/functions/logger.py
--rw-rw-rw-   0        0        0     5060 2021-02-01 14:33:19.000000 automl_tools-0.1.6/automl_tools/functions/modeling.py
--rw-rw-rw-   0        0        0     7806 2021-01-26 16:32:54.000000 automl_tools-0.1.6/automl_tools/functions/optimization_binary.py
--rw-rw-rw-   0        0        0     7892 2021-01-26 16:51:54.000000 automl_tools-0.1.6/automl_tools/functions/optimization_multi_class.py
--rw-rw-rw-   0        0        0     7617 2021-01-26 16:34:47.000000 automl_tools-0.1.6/automl_tools/functions/optimization_regression.py
--rw-rw-rw-   0        0        0     1091 2021-01-26 16:35:40.000000 automl_tools-0.1.6/automl_tools/functions/parameter.py
--rw-rw-rw-   0        0        0     2794 2021-02-01 14:47:10.000000 automl_tools-0.1.6/automl_tools/functions/prepare.py
--rw-rw-rw-   0        0        0     8153 2021-01-25 21:30:36.000000 automl_tools-0.1.6/automl_tools/functions/processing.py
--rw-rw-rw-   0        0        0     6851 2021-01-26 16:01:16.000000 automl_tools-0.1.6/automl_tools/functions/selection.py
--rw-rw-rw-   0        0        0     9909 2021-02-01 14:33:19.000000 automl_tools-0.1.6/automl_tools/functions/utils.py
--rw-rw-rw-   0        0        0     8043 2021-02-01 14:38:51.000000 automl_tools-0.1.6/automl_tools/main.py
-drwxrwxrwx   0        0        0        0 2021-02-01 15:15:36.367418 automl_tools-0.1.6/automl_tools.egg-info/
--rw-rw-rw-   0        0        0     5512 2021-02-01 15:15:35.000000 automl_tools-0.1.6/automl_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2021-02-01 15:15:36.000000 automl_tools-0.1.6/automl_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-01 15:15:35.000000 automl_tools-0.1.6/automl_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      270 2021-02-01 15:15:35.000000 automl_tools-0.1.6/automl_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-02-01 15:15:35.000000 automl_tools-0.1.6/automl_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-02-01 15:15:36.399416 automl_tools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1187 2021-02-01 15:15:14.000000 automl_tools-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-02 05:07:53.000000 automl_tools-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4379 2024-04-02 05:24:58.552757 automl_tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3653 2024-04-02 05:07:53.000000 automl_tools-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.537130 automl_tools-0.2.0/automl_tools/
+-rw-rw-rw-   0        0        0       71 2024-04-02 05:21:14.000000 automl_tools-0.2.0/automl_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/automl_tools/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    10171 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/imputation.py
+-rw-rw-rw-   0        0        0     4684 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/logger.py
+-rw-rw-rw-   0        0        0     5060 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/modeling.py
+-rw-rw-rw-   0        0        0     7806 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_binary.py
+-rw-rw-rw-   0        0        0     7892 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_multi_class.py
+-rw-rw-rw-   0        0        0     7617 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_regression.py
+-rw-rw-rw-   0        0        0     1091 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/parameter.py
+-rw-rw-rw-   0        0        0     2794 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/prepare.py
+-rw-rw-rw-   0        0        0     8153 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/processing.py
+-rw-rw-rw-   0        0        0     6851 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/selection.py
+-rw-rw-rw-   0        0        0     9909 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/utils.py
+-rw-rw-rw-   0        0        0     8043 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/automl_tools.egg-info/
+-rw-rw-rw-   0        0        0     4379 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      253 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      689 2024-04-02 05:24:11.000000 automl_tools-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-02 05:24:58.568383 automl_tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-02 05:22:07.000000 automl_tools-0.2.0/setup.py
```

### Comparing `automl_tools-0.1.6/PKG-INFO` & `automl_tools-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,158 @@
 Metadata-Version: 2.1
 Name: automl_tools
-Version: 0.1.6
+Version: 0.2.0
 Summary: automl_tools
-Home-page: https://github.com/jonaqp/automl_tools/
+Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
-Description: # Automl_tools: automl binary classification
-        
-        
-        [![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
-        [![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
-        [![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
-        
-        
-        
-        
-        Automl_tools is a Python library that implements Gradient Boosting
-        ## Installation
-        
-        The code is packaged for PyPI, so that the installation consists in running:
-        ```sh
-        pip install automl-tools
-        ```
-        
-        ## Colab
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10DFkSmzMO1GqLX-mgBWfDjS9OIVmEy6O?usp=sharing)
-        
-        
-        ## Usage
-        
-        Probabilistic binary example on the Boston housing dataset:
-        
-        ```python
-        import pandas as pd
-        from automl_tools import automl_run
-        
-        train = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/train.csv?token=AAN2ZBDWF77QITK4ARSFIFDABUGAU")
-        test = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/test.csv?token=AAN2ZBD6TMUC5XSGRTJNVPDABUGCO")
-        
-        automl_run(train=train,
-                   test=test,
-                   id_col=None, 
-                   target_col="Survived",
-                   imp_num="knn",
-                   imp_cat="knn",
-                   processing="binding",
-                   mutual_information=False,
-                   correlation_drop=False,
-                   model_feature_selection=None,
-                   model_run="LR",
-                   augmentation=True,
-                   Stratified=True,
-                   cv=5)
-        
-        
-        
-        
-        
-        
-        
-        ```
-        
-        ## Parameter
-        ```sh
-        imp_num : "gaussian", "arbitrary", "median", "mean", "random", "knn"
-        imp_cat : "frequent", "constant", "rare", "knn"
-        processing:  "woe", "binding" 
-        ```
-        
-        ## Support Binary
-        ```sh
-        model_feature_selection: 
-            default: ["LR", "RF", "LGB"]
-                LR  : LogisticRegression
-                RF  : RandomForestClassifier
-                SVM : SVC
-                LS  : LASSO
-                RD  : RIDGE
-                NET : Elasticnet
-                DT  : DecisionTreeClassifier
-                ET  : ExtraTreesClassifier
-                GB  : GradientBoostingClassifier
-                AB  : AdaBoostClassifier
-                XGB  : XGBClassifier
-                LGB  : LGBMClassifier
-                CTB  : CatBoostClassifier
-                NGB  : NGBClassifier
-        
-        model_run:
-            default: "LR"
-                LR  : LogisticRegression
-                RF  : RandomForestClassifier
-                SVM : SVC
-                LS  : LASSO
-                RD  : RIDGE
-                NET : Elasticnet
-                DT  : DecisionTreeClassifier
-                ET  : ExtraTreesClassifier
-                GB  : GradientBoostingClassifier
-                AB  : AdaBoostClassifier
-                XGB  : XGBClassifier
-                LGB  : LGBMClassifier
-                CTB  : CatBoostClassifier
-                NGB  : NGBClassifier
-        ```
-        
-        ## License
-        
-        [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
-        
-        
-        ## New features v1.0
-         * multi_class
-         * regression
-         * integrations GCP deploy model CI/CD
-         * integrations AWS deploy model CI/CD
-         
-        ## BugFix
-         - 0.1.5
-           - fix imputer
-           - fix space hyperparameter
-           - update catboost test
-           
-         - 0.1.4
-           - add parameter cv
-           - add confusion Matrix
-           - add comments readme.txt
-           
-         - 0.1.3
-           - add parameter id_col
-           - add comments readme.txt
-        
-        
-        
-        ## Reference
-        
-         - Jonathan Quiza [github](https://github.com/jonaqp).
-         - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
-         - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
-        
-        
-Keywords: automl,binary
+Keywords: automl
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Automl_tools: automl binary classification
+
+
+[![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
+[![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
+[![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
+
+
+
+
+Automl_tools is a Python library that implements Gradient Boosting
+## Installation
+
+The code is packaged for PyPI, so that the installation consists in running:
+```sh
+pip install automl-tools
+```
+
+## Colab
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10DFkSmzMO1GqLX-mgBWfDjS9OIVmEy6O?usp=sharing)
+
+
+## Usage
+
+Probabilistic binary example on the Boston housing dataset:
+
+```python
+import pandas as pd
+from automl_tools import automl_run
+
+train = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/train.csv?token=AAN2ZBDWF77QITK4ARSFIFDABUGAU")
+test = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/test.csv?token=AAN2ZBD6TMUC5XSGRTJNVPDABUGCO")
+
+automl_run(train=train,
+           test=test,
+           id_col=None, 
+           target_col="Survived",
+           imp_num="knn",
+           imp_cat="knn",
+           processing="binding",
+           mutual_information=False,
+           correlation_drop=False,
+           model_feature_selection=None,
+           model_run="LR",
+           augmentation=True,
+           Stratified=True,
+           cv=5)
+
+
+
+
+
+
+
+```
+
+## Parameter
+```sh
+imp_num : "gaussian", "arbitrary", "median", "mean", "random", "knn"
+imp_cat : "frequent", "constant", "rare", "knn"
+processing:  "woe", "binding" 
+```
+
+## Support Binary
+```sh
+model_feature_selection: 
+    default: ["LR", "RF", "LGB"]
+        LR  : LogisticRegression
+        RF  : RandomForestClassifier
+        SVM : SVC
+        LS  : LASSO
+        RD  : RIDGE
+        NET : Elasticnet
+        DT  : DecisionTreeClassifier
+        ET  : ExtraTreesClassifier
+        GB  : GradientBoostingClassifier
+        AB  : AdaBoostClassifier
+        XGB  : XGBClassifier
+        LGB  : LGBMClassifier
+        CTB  : CatBoostClassifier
+        NGB  : NGBClassifier
+
+model_run:
+    default: "LR"
+        LR  : LogisticRegression
+        RF  : RandomForestClassifier
+        SVM : SVC
+        LS  : LASSO
+        RD  : RIDGE
+        NET : Elasticnet
+        DT  : DecisionTreeClassifier
+        ET  : ExtraTreesClassifier
+        GB  : GradientBoostingClassifier
+        AB  : AdaBoostClassifier
+        XGB  : XGBClassifier
+        LGB  : LGBMClassifier
+        CTB  : CatBoostClassifier
+        NGB  : NGBClassifier
+```
+
+## License
+
+[Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
+
+
+## New features v1.0
+ * multi_class
+ * regression
+ * integrations GCP deploy model CI/CD
+ * integrations AWS deploy model CI/CD
+ 
+## BugFix
+ - 0.1.5
+   - fix imputer
+   - fix space hyperparameter
+   - update catboost test
+   
+ - 0.1.4
+   - add parameter cv
+   - add confusion Matrix
+   - add comments readme.txt
+   
+ - 0.1.3
+   - add parameter id_col
+   - add comments readme.txt
+
+
+
+## Reference
+
+ - Jonathan Quiza [github](https://github.com/jonaqp).
+ - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
+ - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
+
+
+
```

### Comparing `automl_tools-0.1.6/README.md` & `automl_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/imputation.py` & `automl_tools-0.2.0/automl_tools/functions/imputation.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/logger.py` & `automl_tools-0.2.0/automl_tools/functions/logger.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/modeling.py` & `automl_tools-0.2.0/automl_tools/functions/modeling.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/optimization_binary.py` & `automl_tools-0.2.0/automl_tools/functions/optimization_binary.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/optimization_multi_class.py` & `automl_tools-0.2.0/automl_tools/functions/optimization_multi_class.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/optimization_regression.py` & `automl_tools-0.2.0/automl_tools/functions/optimization_regression.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/parameter.py` & `automl_tools-0.2.0/automl_tools/functions/parameter.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/prepare.py` & `automl_tools-0.2.0/automl_tools/functions/prepare.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/processing.py` & `automl_tools-0.2.0/automl_tools/functions/processing.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/selection.py` & `automl_tools-0.2.0/automl_tools/functions/selection.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/functions/utils.py` & `automl_tools-0.2.0/automl_tools/functions/utils.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools/main.py` & `automl_tools-0.2.0/automl_tools/main.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.1.6/automl_tools.egg-info/PKG-INFO` & `automl_tools-0.2.0/automl_tools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,158 @@
 Metadata-Version: 2.1
 Name: automl-tools
-Version: 0.1.6
+Version: 0.2.0
 Summary: automl_tools
-Home-page: https://github.com/jonaqp/automl_tools/
+Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
-Description: # Automl_tools: automl binary classification
-        
-        
-        [![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
-        [![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
-        [![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
-        
-        
-        
-        
-        Automl_tools is a Python library that implements Gradient Boosting
-        ## Installation
-        
-        The code is packaged for PyPI, so that the installation consists in running:
-        ```sh
-        pip install automl-tools
-        ```
-        
-        ## Colab
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10DFkSmzMO1GqLX-mgBWfDjS9OIVmEy6O?usp=sharing)
-        
-        
-        ## Usage
-        
-        Probabilistic binary example on the Boston housing dataset:
-        
-        ```python
-        import pandas as pd
-        from automl_tools import automl_run
-        
-        train = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/train.csv?token=AAN2ZBDWF77QITK4ARSFIFDABUGAU")
-        test = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/test.csv?token=AAN2ZBD6TMUC5XSGRTJNVPDABUGCO")
-        
-        automl_run(train=train,
-                   test=test,
-                   id_col=None, 
-                   target_col="Survived",
-                   imp_num="knn",
-                   imp_cat="knn",
-                   processing="binding",
-                   mutual_information=False,
-                   correlation_drop=False,
-                   model_feature_selection=None,
-                   model_run="LR",
-                   augmentation=True,
-                   Stratified=True,
-                   cv=5)
-        
-        
-        
-        
-        
-        
-        
-        ```
-        
-        ## Parameter
-        ```sh
-        imp_num : "gaussian", "arbitrary", "median", "mean", "random", "knn"
-        imp_cat : "frequent", "constant", "rare", "knn"
-        processing:  "woe", "binding" 
-        ```
-        
-        ## Support Binary
-        ```sh
-        model_feature_selection: 
-            default: ["LR", "RF", "LGB"]
-                LR  : LogisticRegression
-                RF  : RandomForestClassifier
-                SVM : SVC
-                LS  : LASSO
-                RD  : RIDGE
-                NET : Elasticnet
-                DT  : DecisionTreeClassifier
-                ET  : ExtraTreesClassifier
-                GB  : GradientBoostingClassifier
-                AB  : AdaBoostClassifier
-                XGB  : XGBClassifier
-                LGB  : LGBMClassifier
-                CTB  : CatBoostClassifier
-                NGB  : NGBClassifier
-        
-        model_run:
-            default: "LR"
-                LR  : LogisticRegression
-                RF  : RandomForestClassifier
-                SVM : SVC
-                LS  : LASSO
-                RD  : RIDGE
-                NET : Elasticnet
-                DT  : DecisionTreeClassifier
-                ET  : ExtraTreesClassifier
-                GB  : GradientBoostingClassifier
-                AB  : AdaBoostClassifier
-                XGB  : XGBClassifier
-                LGB  : LGBMClassifier
-                CTB  : CatBoostClassifier
-                NGB  : NGBClassifier
-        ```
-        
-        ## License
-        
-        [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
-        
-        
-        ## New features v1.0
-         * multi_class
-         * regression
-         * integrations GCP deploy model CI/CD
-         * integrations AWS deploy model CI/CD
-         
-        ## BugFix
-         - 0.1.5
-           - fix imputer
-           - fix space hyperparameter
-           - update catboost test
-           
-         - 0.1.4
-           - add parameter cv
-           - add confusion Matrix
-           - add comments readme.txt
-           
-         - 0.1.3
-           - add parameter id_col
-           - add comments readme.txt
-        
-        
-        
-        ## Reference
-        
-         - Jonathan Quiza [github](https://github.com/jonaqp).
-         - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
-         - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
-        
-        
-Keywords: automl,binary
+Keywords: automl
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Automl_tools: automl binary classification
+
+
+[![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
+[![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
+[![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
+
+
+
+
+Automl_tools is a Python library that implements Gradient Boosting
+## Installation
+
+The code is packaged for PyPI, so that the installation consists in running:
+```sh
+pip install automl-tools
+```
+
+## Colab
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10DFkSmzMO1GqLX-mgBWfDjS9OIVmEy6O?usp=sharing)
+
+
+## Usage
+
+Probabilistic binary example on the Boston housing dataset:
+
+```python
+import pandas as pd
+from automl_tools import automl_run
+
+train = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/train.csv?token=AAN2ZBDWF77QITK4ARSFIFDABUGAU")
+test = pd.read_csv("https://raw.githubusercontent.com/jonaqp/automl_tools/main/automl_tools/examples/test.csv?token=AAN2ZBD6TMUC5XSGRTJNVPDABUGCO")
+
+automl_run(train=train,
+           test=test,
+           id_col=None, 
+           target_col="Survived",
+           imp_num="knn",
+           imp_cat="knn",
+           processing="binding",
+           mutual_information=False,
+           correlation_drop=False,
+           model_feature_selection=None,
+           model_run="LR",
+           augmentation=True,
+           Stratified=True,
+           cv=5)
+
+
+
+
+
+
+
+```
+
+## Parameter
+```sh
+imp_num : "gaussian", "arbitrary", "median", "mean", "random", "knn"
+imp_cat : "frequent", "constant", "rare", "knn"
+processing:  "woe", "binding" 
+```
+
+## Support Binary
+```sh
+model_feature_selection: 
+    default: ["LR", "RF", "LGB"]
+        LR  : LogisticRegression
+        RF  : RandomForestClassifier
+        SVM : SVC
+        LS  : LASSO
+        RD  : RIDGE
+        NET : Elasticnet
+        DT  : DecisionTreeClassifier
+        ET  : ExtraTreesClassifier
+        GB  : GradientBoostingClassifier
+        AB  : AdaBoostClassifier
+        XGB  : XGBClassifier
+        LGB  : LGBMClassifier
+        CTB  : CatBoostClassifier
+        NGB  : NGBClassifier
+
+model_run:
+    default: "LR"
+        LR  : LogisticRegression
+        RF  : RandomForestClassifier
+        SVM : SVC
+        LS  : LASSO
+        RD  : RIDGE
+        NET : Elasticnet
+        DT  : DecisionTreeClassifier
+        ET  : ExtraTreesClassifier
+        GB  : GradientBoostingClassifier
+        AB  : AdaBoostClassifier
+        XGB  : XGBClassifier
+        LGB  : LGBMClassifier
+        CTB  : CatBoostClassifier
+        NGB  : NGBClassifier
+```
+
+## License
+
+[Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
+
+
+## New features v1.0
+ * multi_class
+ * regression
+ * integrations GCP deploy model CI/CD
+ * integrations AWS deploy model CI/CD
+ 
+## BugFix
+ - 0.1.5
+   - fix imputer
+   - fix space hyperparameter
+   - update catboost test
+   
+ - 0.1.4
+   - add parameter cv
+   - add confusion Matrix
+   - add comments readme.txt
+   
+ - 0.1.3
+   - add parameter id_col
+   - add comments readme.txt
+
+
+
+## Reference
+
+ - Jonathan Quiza [github](https://github.com/jonaqp).
+ - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
+ - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
+
+
+
```

### Comparing `automl_tools-0.1.6/automl_tools.egg-info/SOURCES.txt` & `automl_tools-0.2.0/automl_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 automl_tools/__init__.py
 automl_tools/main.py
 automl_tools.egg-info/PKG-INFO
 automl_tools.egg-info/SOURCES.txt
 automl_tools.egg-info/dependency_links.txt
```

### Comparing `automl_tools-0.1.6/setup.py` & `automl_tools-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 from distutils.core import setup
+
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='automl_tools',
     packages=find_packages(),
-    version='0.1.6',
+    version='0.2.0',
     description='automl_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
-    url='https://github.com/jonaqp/automl_tools/',
+    url='https://github.com/jonaqp/automl_tools',
     download_url='https://github.com/jonaqp/automl_tools/archive/main.zip',
-    keywords=['automl', 'binary'],
+    keywords=['automl'],
     install_requires=open(os.path.join(setuppath, 'requirements.txt')).read().splitlines(),
     dependency_links=[],
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
     ],
 )
```

