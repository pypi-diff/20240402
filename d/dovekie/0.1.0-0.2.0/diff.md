# Comparing `tmp/dovekie-0.1.0.tar.gz` & `tmp/dovekie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dovekie-0.1.0.tar", last modified: Tue Apr  2 14:51:50 2024, max compression
+gzip compressed data, was "dovekie-0.2.0.tar", last modified: Tue Apr  2 15:18:22 2024, max compression
```

## Comparing `dovekie-0.1.0.tar` & `dovekie-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 14:51:50.042628 dovekie-0.1.0/
--rw-rw-r--   0 cph       (1000) cph       (1000)     1071 2024-04-02 14:50:52.000000 dovekie-0.1.0/LICENSE
--rw-r--r--   0 cph       (1000) cph       (1000)     1984 2024-04-02 14:51:50.042628 dovekie-0.1.0/PKG-INFO
--rw-rw-r--   0 cph       (1000) cph       (1000)     1695 2024-04-02 14:50:52.000000 dovekie-0.1.0/README.md
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 14:51:50.038628 dovekie-0.1.0/dovekie/
--rw-rw-r--   0 cph       (1000) cph       (1000)       35 2024-04-01 22:25:28.000000 dovekie-0.1.0/dovekie/__init__.py
--rw-rw-r--   0 cph       (1000) cph       (1000)      106 2024-04-01 22:25:18.000000 dovekie-0.1.0/dovekie/core.py
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 14:51:50.038628 dovekie-0.1.0/dovekie.egg-info/
--rw-r--r--   0 cph       (1000) cph       (1000)     1984 2024-04-02 14:51:49.000000 dovekie-0.1.0/dovekie.egg-info/PKG-INFO
--rw-rw-r--   0 cph       (1000) cph       (1000)      186 2024-04-02 14:51:49.000000 dovekie-0.1.0/dovekie.egg-info/SOURCES.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)        1 2024-04-02 14:51:49.000000 dovekie-0.1.0/dovekie.egg-info/dependency_links.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)        8 2024-04-02 14:51:49.000000 dovekie-0.1.0/dovekie.egg-info/top_level.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)       38 2024-04-02 14:51:50.042628 dovekie-0.1.0/setup.cfg
--rw-rw-r--   0 cph       (1000) cph       (1000)      457 2024-04-01 22:24:37.000000 dovekie-0.1.0/setup.py
+drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 15:18:22.367656 dovekie-0.2.0/
+-rw-rw-r--   0 cph       (1000) cph       (1000)     1071 2024-04-02 14:50:52.000000 dovekie-0.2.0/LICENSE
+-rw-r--r--   0 cph       (1000) cph       (1000)     1984 2024-04-02 15:18:22.367656 dovekie-0.2.0/PKG-INFO
+-rw-rw-r--   0 cph       (1000) cph       (1000)     1695 2024-04-02 14:50:52.000000 dovekie-0.2.0/README.md
+drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 15:18:22.367656 dovekie-0.2.0/dovekie/
+-rw-rw-r--   0 cph       (1000) cph       (1000)       71 2024-04-02 15:15:53.000000 dovekie-0.2.0/dovekie/__init__.py
+-rw-rw-r--   0 cph       (1000) cph       (1000)      106 2024-04-01 22:25:18.000000 dovekie-0.2.0/dovekie/core.py
+drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-02 15:18:22.367656 dovekie-0.2.0/dovekie.egg-info/
+-rw-r--r--   0 cph       (1000) cph       (1000)     1984 2024-04-02 15:18:22.000000 dovekie-0.2.0/dovekie.egg-info/PKG-INFO
+-rw-rw-r--   0 cph       (1000) cph       (1000)      186 2024-04-02 15:18:22.000000 dovekie-0.2.0/dovekie.egg-info/SOURCES.txt
+-rw-rw-r--   0 cph       (1000) cph       (1000)        1 2024-04-02 15:18:22.000000 dovekie-0.2.0/dovekie.egg-info/dependency_links.txt
+-rw-rw-r--   0 cph       (1000) cph       (1000)        8 2024-04-02 15:18:22.000000 dovekie-0.2.0/dovekie.egg-info/top_level.txt
+-rw-rw-r--   0 cph       (1000) cph       (1000)       38 2024-04-02 15:18:22.367656 dovekie-0.2.0/setup.cfg
+-rw-rw-r--   0 cph       (1000) cph       (1000)      457 2024-04-02 15:17:35.000000 dovekie-0.2.0/setup.py
```

### Comparing `dovekie-0.1.0/LICENSE` & `dovekie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dovekie-0.1.0/PKG-INFO` & `dovekie-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.1.0 Summary: A library that
+Metadata-Version: 2.1 Name: dovekie Version: 0.2.0 Summary: A library that
 defines common SKI combinators from Combinatory Logic. Author: Conor Hoekstra
 Author-email: codereport@outlook.com License: MIT Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _b_a_d_g_e_/_P_y_t_h_o_n_-_3_-_f_f_6_9_b_4_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_l_l_o_w_e_r_s_/
```

### Comparing `dovekie-0.1.0/README.md` & `dovekie-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dovekie-0.1.0/dovekie.egg-info/PKG-INFO` & `dovekie-0.2.0/dovekie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.1.0 Summary: A library that
+Metadata-Version: 2.1 Name: dovekie Version: 0.2.0 Summary: A library that
 defines common SKI combinators from Combinatory Logic. Author: Conor Hoekstra
 Author-email: codereport@outlook.com License: MIT Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _b_a_d_g_e_/_P_y_t_h_o_n_-_3_-_f_f_6_9_b_4_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_l_l_o_w_e_r_s_/
```

