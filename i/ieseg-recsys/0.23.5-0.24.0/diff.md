# Comparing `tmp/ieseg_recsys-0.23.5.tar.gz` & `tmp/ieseg_recsys-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieseg_recsys-0.23.5.tar", last modified: Tue Mar 21 16:45:02 2023, max compression
+gzip compressed data, was "ieseg_recsys-0.24.0.tar", last modified: Tue Apr  2 16:07:47 2024, max compression
```

## Comparing `ieseg_recsys-0.23.5.tar` & `ieseg_recsys-0.24.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 16:45:02.331272 ieseg_recsys-0.23.5/
--rw-rw-rw-   0        0        0     1092 2023-03-13 13:21:59.000000 ieseg_recsys-0.23.5/LICENSE.rst
--rw-rw-rw-   0        0        0     1683 2023-03-21 16:45:02.331570 ieseg_recsys-0.23.5/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2023-03-17 13:44:31.000000 ieseg_recsys-0.23.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 16:45:02.301272 ieseg_recsys-0.23.5/ieseg_recsys/
--rw-rw-rw-   0        0        0       32 2023-03-13 14:49:32.000000 ieseg_recsys-0.23.5/ieseg_recsys/__init__.py
--rw-rw-rw-   0        0        0     9814 2023-03-21 16:42:00.000000 ieseg_recsys-0.23.5/ieseg_recsys/eval.py
--rw-rw-rw-   0        0        0     4897 2022-01-19 17:16:56.000000 ieseg_recsys-0.23.5/ieseg_recsys/model.py
--rw-rw-rw-   0        0        0     2743 2023-03-15 09:55:19.000000 ieseg_recsys-0.23.5/ieseg_recsys/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-21 16:45:02.329272 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/
--rw-rw-rw-   0        0        0     1683 2023-03-21 16:45:02.000000 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-03-21 16:45:02.000000 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 16:45:02.000000 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-03-21 16:45:02.000000 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-21 16:45:02.000000 ieseg_recsys-0.23.5/ieseg_recsys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-21 16:45:02.334442 ieseg_recsys-0.23.5/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-03-21 16:44:51.000000 ieseg_recsys-0.23.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:07:47.931964 ieseg_recsys-0.24.0/
+-rw-rw-rw-   0        0        0     1092 2023-03-13 13:21:59.000000 ieseg_recsys-0.24.0/LICENSE.rst
+-rw-rw-rw-   0        0        0     1683 2024-04-02 16:07:47.932961 ieseg_recsys-0.24.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1335 2024-04-02 16:05:38.000000 ieseg_recsys-0.24.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 16:07:47.916018 ieseg_recsys-0.24.0/ieseg_recsys/
+-rw-rw-rw-   0        0        0       32 2023-03-13 14:49:32.000000 ieseg_recsys-0.24.0/ieseg_recsys/__init__.py
+-rw-rw-rw-   0        0        0     9961 2024-04-02 16:04:57.000000 ieseg_recsys-0.24.0/ieseg_recsys/eval.py
+-rw-rw-rw-   0        0        0     4897 2022-01-19 17:16:56.000000 ieseg_recsys-0.24.0/ieseg_recsys/model.py
+-rw-rw-rw-   0        0        0     2743 2023-03-15 09:55:19.000000 ieseg_recsys-0.24.0/ieseg_recsys/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:07:47.929971 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/
+-rw-rw-rw-   0        0        0     1683 2024-04-02 16:07:47.000000 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-02 16:07:47.000000 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 16:07:47.000000 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 16:07:47.000000 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 16:07:47.000000 ieseg_recsys-0.24.0/ieseg_recsys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2024-04-02 16:07:47.936947 ieseg_recsys-0.24.0/setup.cfg
+-rw-rw-rw-   0        0        0      788 2024-04-02 16:05:23.000000 ieseg_recsys-0.24.0/setup.py
```

### Comparing `ieseg_recsys-0.23.5/LICENSE.rst` & `ieseg_recsys-0.24.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ieseg_recsys-0.23.5/PKG-INFO` & `ieseg_recsys-0.24.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg_recsys
-Version: 0.23.5
+Version: 0.24.0
 Summary: Recommendation Systems - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Recommender Systems IESEG
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
         padding-right:1.5cm;
     }
 </style> -->
 
 <!-- HEADER -->
 |  |  |
 |---|---|
-| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2022 & 2023</span> |
+| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2023 & 2024</span> |
 
 <!-- CONTENT -->
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: ieseg_recsys Version: 0.23.5 Summary:
+Metadata-Version: 2.1 Name: ieseg_recsys Version: 0.24.0 Summary:
 Recommendation Systems - IESEG School of Management Home-page: https://
 github.com/pnborchert Author: Philipp Borchert Author-email:
 p.borchert@ieseg.fr License: MIT Keywords: Recommender Systems IESEG
 Description-Content-Type: text/markdown License-File: LICENSE.rst | | | |---|--
 -| | [drawing]|
 Recommendation Systems
 Module
-Class: 2022 & 2023 | --- ## Overview - Model evaluation (`eval.py`): -
+Class: 2023 & 2024 | --- ## Overview - Model evaluation (`eval.py`): -
 Regression metrics - RMSE - MAE - Classification metrics - Precision - Recall -
 F1 - Ranking metrics - NDCG - `eval.evaluate` computes all above mentioned
 metrics - Evaluate Top-N recommendations - HR - MAP - Content based Recommender
 System (`model.py`) - Helper functions (`utils.py`) - `get_top_n`: Compute Top-
 N recommendations from predictions - `predict_user_topn`: Compute Top-
 N recommendations for a user
 | Useful Links | | |---|---| | _[_h_t_t_p_s_:_/_/_s_u_r_p_r_i_s_e_l_i_b_._c_o_m_/_l_o_g_o___w_h_i_t_e_._s_v_g_]|
```

### Comparing `ieseg_recsys-0.23.5/README.md` & `ieseg_recsys-0.24.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         padding-right:1.5cm;
     }
 </style> -->
 
 <!-- HEADER -->
 |  |  |
 |---|---|
-| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2022 & 2023</span> |
+| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2023 & 2024</span> |
 
 <!-- CONTENT -->
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 | | | |---|---| | [drawing]|
 Recommendation Systems
 Module
-Class: 2022 & 2023 | --- ## Overview - Model evaluation (`eval.py`): -
+Class: 2023 & 2024 | --- ## Overview - Model evaluation (`eval.py`): -
 Regression metrics - RMSE - MAE - Classification metrics - Precision - Recall -
 F1 - Ranking metrics - NDCG - `eval.evaluate` computes all above mentioned
 metrics - Evaluate Top-N recommendations - HR - MAP - Content based Recommender
 System (`model.py`) - Helper functions (`utils.py`) - `get_top_n`: Compute Top-
 N recommendations from predictions - `predict_user_topn`: Compute Top-
 N recommendations for a user
 | Useful Links | | |---|---| | _[_h_t_t_p_s_:_/_/_s_u_r_p_r_i_s_e_l_i_b_._c_o_m_/_l_o_g_o___w_h_i_t_e_._s_v_g_]|
```

### Comparing `ieseg_recsys-0.23.5/ieseg_recsys/eval.py` & `ieseg_recsys-0.24.0/ieseg_recsys/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,19 +185,24 @@
     df_real_sort = {}
     df_pred = pd.DataFrame(prediction)
 
     # sort user preferences by rating
     for user in df_pred["uid"].unique():
         # predicted values
         plist = list(df_pred.loc[df_pred["uid"]==user,:].sort_values("est", ascending=False)["iid"])
-        df_pred_sort[user] = [plist]
         
         # real values
         rlist = list(df_pred.loc[df_pred["uid"]==user,:].sort_values("r_ui", ascending=False)["iid"])
-        df_real_sort[user] = [rlist]
+
+        # plist and rlist should be longer than 0
+        if len(plist) == 0 or len(rlist) == 0: 
+            continue
+        else:
+            df_pred_sort[user] = [plist]
+            df_real_sort[user] = [rlist]
 
     df_pred_sort = pd.DataFrame(df_pred_sort, index=["iid"]).T
     df_real_sort = pd.DataFrame(df_real_sort, index=["iid"]).T
 
     res = {}
 
     res[f'NDCG@{threshold}'] = ndcg(df_real_sort["iid"], df_pred_sort["iid"], threshold)
```

### Comparing `ieseg_recsys-0.23.5/ieseg_recsys/model.py` & `ieseg_recsys-0.24.0/ieseg_recsys/model.py`

 * *Files identical despite different names*

### Comparing `ieseg_recsys-0.23.5/ieseg_recsys/utils.py` & `ieseg_recsys-0.24.0/ieseg_recsys/utils.py`

 * *Files identical despite different names*

### Comparing `ieseg_recsys-0.23.5/ieseg_recsys.egg-info/PKG-INFO` & `ieseg_recsys-0.24.0/ieseg_recsys.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg-recsys
-Version: 0.23.5
+Version: 0.24.0
 Summary: Recommendation Systems - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Recommender Systems IESEG
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
         padding-right:1.5cm;
     }
 </style> -->
 
 <!-- HEADER -->
 |  |  |
 |---|---|
-| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2022 & 2023</span> |
+| <img src="https://www.ieseg.fr/wp-content/uploads/IESEG-Logo-2012-rgb.jpg" alt="drawing" width=100%/> | <span><br>Recommendation Systems<br>Module<br>Class: 2023 & 2024</span> |
 
 <!-- CONTENT -->
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: ieseg-recsys Version: 0.23.5 Summary:
+Metadata-Version: 2.1 Name: ieseg-recsys Version: 0.24.0 Summary:
 Recommendation Systems - IESEG School of Management Home-page: https://
 github.com/pnborchert Author: Philipp Borchert Author-email:
 p.borchert@ieseg.fr License: MIT Keywords: Recommender Systems IESEG
 Description-Content-Type: text/markdown License-File: LICENSE.rst | | | |---|--
 -| | [drawing]|
 Recommendation Systems
 Module
-Class: 2022 & 2023 | --- ## Overview - Model evaluation (`eval.py`): -
+Class: 2023 & 2024 | --- ## Overview - Model evaluation (`eval.py`): -
 Regression metrics - RMSE - MAE - Classification metrics - Precision - Recall -
 F1 - Ranking metrics - NDCG - `eval.evaluate` computes all above mentioned
 metrics - Evaluate Top-N recommendations - HR - MAP - Content based Recommender
 System (`model.py`) - Helper functions (`utils.py`) - `get_top_n`: Compute Top-
 N recommendations from predictions - `predict_user_topn`: Compute Top-
 N recommendations for a user
 | Useful Links | | |---|---| | _[_h_t_t_p_s_:_/_/_s_u_r_p_r_i_s_e_l_i_b_._c_o_m_/_l_o_g_o___w_h_i_t_e_._s_v_g_]|
```

### Comparing `ieseg_recsys-0.23.5/setup.py` & `ieseg_recsys-0.24.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ieseg_recsys',
-    version='0.23.5',
+    version='0.24.0',
     license='MIT',
     author="Philipp Borchert",
     author_email='p.borchert@ieseg.fr',
     packages=find_packages(),
     description = 'Recommendation Systems - IESEG School of Management',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

