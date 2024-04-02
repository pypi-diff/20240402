# Comparing `tmp/mag_net_hub-0.0.2.tar.gz` & `tmp/mag_net_hub-0.0.3.tar.gz`

## Comparing `mag_net_hub-0.0.2.tar` & `mag_net_hub-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/requirements.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/__init__.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/loss.py
--rw-r--r--   0        0        0    20928 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/paderborn.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/sydney.py
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
--rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/tests/test_paderborn.py
--rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/LICENSE
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/README.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 mag_net_hub-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/__init__.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/loss.py
+-rw-r--r--   0        0        0    20928 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/paderborn.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/sydney.py
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
+-rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/tests/test_paderborn.py
+-rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/README.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 mag_net_hub-0.0.3/PKG-INFO
```

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/loss.py` & `mag_net_hub-0.0.3/src_py/mag_net_hub/loss.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/paderborn.py` & `mag_net_hub-0.0.3/src_py/mag_net_hub/paderborn.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/src_py/mag_net_hub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt` & `mag_net_hub-0.0.3/src_py/mag_net_hub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/tests/test_paderborn.py` & `mag_net_hub-0.0.3/tests/test_paderborn.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv` & `mag_net_hub-0.0.3/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/.gitignore` & `mag_net_hub-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/LICENSE` & `mag_net_hub-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/README.md` & `mag_net_hub-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.2/pyproject.toml` & `mag_net_hub-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "mag_net_hub"
-version = "0.0.2"
+name = "mag-net-hub"
+version = "0.0.3"
 authors = [
     { name = "Wilhelm Kirchgässner" },
 ]
 description = "MagNet Challenge - Certified Models"
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
```

### Comparing `mag_net_hub-0.0.2/PKG-INFO` & `mag_net_hub-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
-Name: mag_net_hub
-Version: 0.0.2
+Name: mag-net-hub
+Version: 0.0.3
 Dynamic: Requires-Dist
 Dynamic: Provides-Extra
 Summary: MagNet Challenge - Certified Models
 Project-URL: Homepage, https://github.com/upb-lea/mag-net-hub
 Project-URL: Issues, https://github.com/upb-lea/mag-net-hub/issues
 Author: Wilhelm Kirchgässner
 License-File: LICENSE
```

