# Comparing `tmp/re_gpt-3.0.1.tar.gz` & `tmp/re_gpt-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_gpt-3.0.1.tar", last modified: Sat Jan  6 19:30:52 2024, max compression
+gzip compressed data, was "re_gpt-4.0.0.tar", last modified: Tue Apr  2 17:01:16 2024, max compression
```

## Comparing `re_gpt-3.0.1.tar` & `re_gpt-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zaieem    (1000) zaieem    (1000)        0 2024-01-06 19:30:52.205952 re_gpt-3.0.1/
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)    11357 2023-11-08 10:27:51.000000 re_gpt-3.0.1/LICENSE
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)     7862 2024-01-06 19:30:52.205952 re_gpt-3.0.1/PKG-INFO
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)     7487 2024-01-02 15:56:08.000000 re_gpt-3.0.1/README.md
-drwxr-xr-x   0 zaieem    (1000) zaieem    (1000)        0 2024-01-06 19:30:52.201952 re_gpt-3.0.1/re_gpt/
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)       78 2023-12-09 19:22:23.000000 re_gpt-3.0.1/re_gpt/__init__.py
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)    17181 2024-01-06 19:26:18.000000 re_gpt-3.0.1/re_gpt/async_chatgpt.py
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)     1619 2024-01-06 19:26:18.000000 re_gpt-3.0.1/re_gpt/errors.py
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)    14901 2024-01-06 19:26:52.000000 re_gpt-3.0.1/re_gpt/sync_chatgpt.py
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)     4162 2024-01-06 19:26:18.000000 re_gpt-3.0.1/re_gpt/utils.py
-drwxr-xr-x   0 zaieem    (1000) zaieem    (1000)        0 2024-01-06 19:30:52.205952 re_gpt-3.0.1/re_gpt.egg-info/
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)     7862 2024-01-06 19:30:52.000000 re_gpt-3.0.1/re_gpt.egg-info/PKG-INFO
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)      274 2024-01-06 19:30:52.000000 re_gpt-3.0.1/re_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)        1 2024-01-06 19:30:52.000000 re_gpt-3.0.1/re_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)       17 2024-01-06 19:30:52.000000 re_gpt-3.0.1/re_gpt.egg-info/requires.txt
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)        7 2024-01-06 19:30:52.000000 re_gpt-3.0.1/re_gpt.egg-info/top_level.txt
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)       38 2024-01-06 19:30:52.205952 re_gpt-3.0.1/setup.cfg
--rw-r--r--   0 zaieem    (1000) zaieem    (1000)      537 2024-01-06 19:27:43.000000 re_gpt-3.0.1/setup.py
+drwxr-xr-x   0 zai       (1000) zai       (1001)        0 2024-04-02 17:01:16.442639 re_gpt-4.0.0/
+-rw-r--r--   0 zai       (1000) zai       (1001)    11357 2024-04-02 16:01:00.000000 re_gpt-4.0.0/LICENSE
+-rw-r--r--   0 zai       (1000) zai       (1001)     7969 2024-04-02 17:01:16.442639 re_gpt-4.0.0/PKG-INFO
+-rw-r--r--   0 zai       (1000) zai       (1001)     7562 2024-04-02 16:01:00.000000 re_gpt-4.0.0/README.md
+drwxr-xr-x   0 zai       (1000) zai       (1001)        0 2024-04-02 17:01:16.438639 re_gpt-4.0.0/re_gpt/
+-rw-r--r--   0 zai       (1000) zai       (1001)       78 2024-04-02 16:01:00.000000 re_gpt-4.0.0/re_gpt/__init__.py
+-rw-r--r--   0 zai       (1000) zai       (1001)    23290 2024-04-02 16:46:38.000000 re_gpt-4.0.0/re_gpt/async_chatgpt.py
+-rw-r--r--   0 zai       (1000) zai       (1001)     1619 2024-04-02 16:01:00.000000 re_gpt-4.0.0/re_gpt/errors.py
+-rw-r--r--   0 zai       (1000) zai       (1001)    20887 2024-04-02 16:01:00.000000 re_gpt-4.0.0/re_gpt/sync_chatgpt.py
+-rw-r--r--   0 zai       (1000) zai       (1001)     4209 2024-04-02 16:01:00.000000 re_gpt-4.0.0/re_gpt/utils.py
+drwxr-xr-x   0 zai       (1000) zai       (1001)        0 2024-04-02 17:01:16.442639 re_gpt-4.0.0/re_gpt.egg-info/
+-rw-r--r--   0 zai       (1000) zai       (1001)     7969 2024-04-02 17:01:15.000000 re_gpt-4.0.0/re_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 zai       (1000) zai       (1001)      274 2024-04-02 17:01:16.000000 re_gpt-4.0.0/re_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 zai       (1000) zai       (1001)        1 2024-04-02 17:01:16.000000 re_gpt-4.0.0/re_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 zai       (1000) zai       (1001)       34 2024-04-02 17:01:16.000000 re_gpt-4.0.0/re_gpt.egg-info/requires.txt
+-rw-r--r--   0 zai       (1000) zai       (1001)        7 2024-04-02 17:01:16.000000 re_gpt-4.0.0/re_gpt.egg-info/top_level.txt
+-rw-r--r--   0 zai       (1000) zai       (1001)       38 2024-04-02 17:01:16.442639 re_gpt-4.0.0/setup.cfg
+-rw-r--r--   0 zai       (1000) zai       (1001)      557 2024-04-02 16:56:29.000000 re_gpt-4.0.0/setup.py
```

### Comparing `re_gpt-3.0.1/LICENSE` & `re_gpt-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_gpt-3.0.1/PKG-INFO` & `re_gpt-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-Metadata-Version: 2.1
-Name: re_gpt
-Version: 3.0.1
-Summary: Unofficial reverse-engineered ChatGPT API in Python.
-Home-page: https://github.com/Zai-Kun/reverse-engineered-chatgpt
-Author: Zai-Kun
-Project-URL: Bug Tracker, https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: curl_cffi==0.5.9
-
 <div align="center">
   <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt">  </a>
 
 <h1 align="center">Reverse Engineered <a href="https://openai.com/blog/chatgpt">ChatGPT</a> API</h1>
 
   <p align="center">
     Use OpenAI ChatGPT in your Python code without an API key
 
 [![Stargazers][stars-badge]][stars-url]
 [![Forks][forks-badge]][forks-url]
 [![Discussions][discussions-badge]][discussions-url]
 [![Issues][issues-badge]][issues-url]
 [![MIT License][license-badge]][license-url]
 
+  English | [简体中文](./docs/zh-README.md)
+
   </p>
     <p align="center">
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt"></a>
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues">Report Bug</a>
     |
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/discussions">Request Feature</a>
   </p>
@@ -190,15 +181,15 @@
 
 Zai-Kun - [Discord Server](https://discord.gg/ymcqxudVJG)
 
 Repo Link: <https://github.com/Zai-Kun/reverse-engineered-chatgpt>
 
 ## Acknowledgments
 
-- [sudoAlphaX](https://github.com/sudoAlphaX)
+- [sudoAlphaX (for writing this readme)](https://github.com/sudoAlphaX)
 
 - [yifeikong (curl-cffi module)](https://github.com/yifeikong/curl_cffi)
 
 - [acheong08 (implementation to obtain arkose_token)](https://github.com/acheong08/funcaptcha)
 
 - [pyca (cryptography module)](https://github.com/pyca/cryptography/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,17 +1,13 @@
-Metadata-Version: 2.1 Name: re_gpt Version: 3.0.1 Summary: Unofficial reverse-
-engineered ChatGPT API in Python. Home-page: https://github.com/Zai-Kun/
-reverse-engineered-chatgpt Author: Zai-Kun Project-URL: Bug Tracker, https://
-github.com/Zai-Kun/reverse-engineered-chatgpt/issues Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: curl_cffi==0.5.9
                  ************ RReevveerrssee EEnnggiinneeeerreedd _CC_hh_aa_tt_GG_PP_TT AAPPII ************
 Use OpenAI ChatGPT in your Python code without an API key [![Stargazers][stars-
      badge]][stars-url] [![Forks][forks-badge]][forks-url] [![Discussions]
 [discussions-badge]][discussions-url] [![Issues][issues-badge]][issues-url] [!
-                  [MIT License][license-badge]][license-url]
+[MIT License][license-badge]][license-url] English | [ç®ä½ä¸­æ](./docs/zh-
+                                  README.md)
                          _R_e_p_o_r_t_ _B_u_g | _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _I_n_s_p_i_r_a_t_i_o_n
           o _H_o_w_ _i_t_ _w_o_r_k_s
           o _B_u_i_l_t_ _u_s_i_n_g
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -73,27 +69,28 @@
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request ## License Distributed under the Apache
 License 2.0. See [`LICENSE`](https://github.com/Zai-Kun/reverse-engineered-
 chatgpt/blob/main/LICENSE) for more information. ## Contact/Bug report Zai-Kun
 - [Discord Server](https://discord.gg/ymcqxudVJG) Repo Link:
-github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments -
-[sudoAlphaX](https://github.com/sudoAlphaX) - [yifeikong (curl-cffi module)]
-(https://github.com/yifeikong/curl_cffi) - [acheong08 (implementation to obtain
-arkose_token)](https://github.com/acheong08/funcaptcha) - [pyca (cryptography
-module)](https://github.com/pyca/cryptography/) - [Legrandin (pycryptodome
-module)](https://github.com/Legrandin/pycryptodome/) - [othneildrew (README
-Template)](https://github.com/othneildrew) [forks-badge]: https://
-img.shields.io/github/forks/Zai-Kun/reverse-engineered-chatgpt [forks-url]:
-https://github.com/Zai-Kun/reverse-engineered-chatgpt/network/members [stars-
-badge]: https://img.shields.io/github/stars/Zai-Kun/reverse-engineered-chatgpt
-[stars-url]: https://github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers
-[issues-badge]: https://img.shields.io/github/issues/Zai-Kun/reverse-
-engineered-chatgpt [issues-url]: https://github.com/Zai-Kun/reverse-engineered-
-chatgpt/issues [discussions-badge]: https://img.shields.io/github/discussions/
-Zai-Kun/reverse-engineered-chatgpt [discussions-url]: https://github.com/Zai-
-Kun/reverse-engineered-chatgpt/discussions [python-badge]: https://
-img.shields.io/badge/Python-blue?logo=python&logoColor=yellow [python-url]:
-https://www.python.org/ [license-badge]: https://img.shields.io/github/license/
-Zai-Kun/reverse-engineered-chatgpt [license-url]: https://github.com/Zai-Kun/
-reverse-engineered-chatgpt/blob/main/LICENSE
+github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments - [sudoAlphaX
+(for writing this readme)](https://github.com/sudoAlphaX) - [yifeikong (curl-
+cffi module)](https://github.com/yifeikong/curl_cffi) - [acheong08
+(implementation to obtain arkose_token)](https://github.com/acheong08/
+funcaptcha) - [pyca (cryptography module)](https://github.com/pyca/
+cryptography/) - [Legrandin (pycryptodome module)](https://github.com/
+Legrandin/pycryptodome/) - [othneildrew (README Template)](https://github.com/
+othneildrew) [forks-badge]: https://img.shields.io/github/forks/Zai-Kun/
+reverse-engineered-chatgpt [forks-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/network/members [stars-badge]: https://img.shields.io/
+github/stars/Zai-Kun/reverse-engineered-chatgpt [stars-url]: https://
+github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers [issues-badge]: https:
+//img.shields.io/github/issues/Zai-Kun/reverse-engineered-chatgpt [issues-url]:
+https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues [discussions-
+badge]: https://img.shields.io/github/discussions/Zai-Kun/reverse-engineered-
+chatgpt [discussions-url]: https://github.com/Zai-Kun/reverse-engineered-
+chatgpt/discussions [python-badge]: https://img.shields.io/badge/Python-
+blue?logo=python&logoColor=yellow [python-url]: https://www.python.org/
+[license-badge]: https://img.shields.io/github/license/Zai-Kun/reverse-
+engineered-chatgpt [license-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/blob/main/LICENSE
```

### Comparing `re_gpt-3.0.1/README.md` & `re_gpt-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+Metadata-Version: 2.1
+Name: re_gpt
+Version: 4.0.0
+Summary: Unofficial reverse-engineered ChatGPT API in Python.
+Home-page: https://github.com/Zai-Kun/reverse-engineered-chatgpt
+Author: Zai-Kun
+Project-URL: Bug Tracker, https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: curl_cffi==0.5.9
+Requires-Dist: websockets==12.0
+
 <div align="center">
   <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt">  </a>
 
 <h1 align="center">Reverse Engineered <a href="https://openai.com/blog/chatgpt">ChatGPT</a> API</h1>
 
   <p align="center">
     Use OpenAI ChatGPT in your Python code without an API key
 
 [![Stargazers][stars-badge]][stars-url]
 [![Forks][forks-badge]][forks-url]
 [![Discussions][discussions-badge]][discussions-url]
 [![Issues][issues-badge]][issues-url]
 [![MIT License][license-badge]][license-url]
 
+  English | [简体中文](./docs/zh-README.md)
+
   </p>
     <p align="center">
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt"></a>
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues">Report Bug</a>
     |
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/discussions">Request Feature</a>
   </p>
@@ -179,15 +193,15 @@
 
 Zai-Kun - [Discord Server](https://discord.gg/ymcqxudVJG)
 
 Repo Link: <https://github.com/Zai-Kun/reverse-engineered-chatgpt>
 
 ## Acknowledgments
 
-- [sudoAlphaX](https://github.com/sudoAlphaX)
+- [sudoAlphaX (for writing this readme)](https://github.com/sudoAlphaX)
 
 - [yifeikong (curl-cffi module)](https://github.com/yifeikong/curl_cffi)
 
 - [acheong08 (implementation to obtain arkose_token)](https://github.com/acheong08/funcaptcha)
 
 - [pyca (cryptography module)](https://github.com/pyca/cryptography/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,12 +1,19 @@
+Metadata-Version: 2.1 Name: re_gpt Version: 4.0.0 Summary: Unofficial reverse-
+engineered ChatGPT API in Python. Home-page: https://github.com/Zai-Kun/
+reverse-engineered-chatgpt Author: Zai-Kun Project-URL: Bug Tracker, https://
+github.com/Zai-Kun/reverse-engineered-chatgpt/issues Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: curl_cffi==0.5.9 Requires-
+Dist: websockets==12.0
                  ************ RReevveerrssee EEnnggiinneeeerreedd _CC_hh_aa_tt_GG_PP_TT AAPPII ************
 Use OpenAI ChatGPT in your Python code without an API key [![Stargazers][stars-
      badge]][stars-url] [![Forks][forks-badge]][forks-url] [![Discussions]
 [discussions-badge]][discussions-url] [![Issues][issues-badge]][issues-url] [!
-                  [MIT License][license-badge]][license-url]
+[MIT License][license-badge]][license-url] English | [ç®ä½ä¸­æ](./docs/zh-
+                                  README.md)
                          _R_e_p_o_r_t_ _B_u_g | _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _I_n_s_p_i_r_a_t_i_o_n
           o _H_o_w_ _i_t_ _w_o_r_k_s
           o _B_u_i_l_t_ _u_s_i_n_g
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -68,27 +75,28 @@
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request ## License Distributed under the Apache
 License 2.0. See [`LICENSE`](https://github.com/Zai-Kun/reverse-engineered-
 chatgpt/blob/main/LICENSE) for more information. ## Contact/Bug report Zai-Kun
 - [Discord Server](https://discord.gg/ymcqxudVJG) Repo Link:
-github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments -
-[sudoAlphaX](https://github.com/sudoAlphaX) - [yifeikong (curl-cffi module)]
-(https://github.com/yifeikong/curl_cffi) - [acheong08 (implementation to obtain
-arkose_token)](https://github.com/acheong08/funcaptcha) - [pyca (cryptography
-module)](https://github.com/pyca/cryptography/) - [Legrandin (pycryptodome
-module)](https://github.com/Legrandin/pycryptodome/) - [othneildrew (README
-Template)](https://github.com/othneildrew) [forks-badge]: https://
-img.shields.io/github/forks/Zai-Kun/reverse-engineered-chatgpt [forks-url]:
-https://github.com/Zai-Kun/reverse-engineered-chatgpt/network/members [stars-
-badge]: https://img.shields.io/github/stars/Zai-Kun/reverse-engineered-chatgpt
-[stars-url]: https://github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers
-[issues-badge]: https://img.shields.io/github/issues/Zai-Kun/reverse-
-engineered-chatgpt [issues-url]: https://github.com/Zai-Kun/reverse-engineered-
-chatgpt/issues [discussions-badge]: https://img.shields.io/github/discussions/
-Zai-Kun/reverse-engineered-chatgpt [discussions-url]: https://github.com/Zai-
-Kun/reverse-engineered-chatgpt/discussions [python-badge]: https://
-img.shields.io/badge/Python-blue?logo=python&logoColor=yellow [python-url]:
-https://www.python.org/ [license-badge]: https://img.shields.io/github/license/
-Zai-Kun/reverse-engineered-chatgpt [license-url]: https://github.com/Zai-Kun/
-reverse-engineered-chatgpt/blob/main/LICENSE
+github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments - [sudoAlphaX
+(for writing this readme)](https://github.com/sudoAlphaX) - [yifeikong (curl-
+cffi module)](https://github.com/yifeikong/curl_cffi) - [acheong08
+(implementation to obtain arkose_token)](https://github.com/acheong08/
+funcaptcha) - [pyca (cryptography module)](https://github.com/pyca/
+cryptography/) - [Legrandin (pycryptodome module)](https://github.com/
+Legrandin/pycryptodome/) - [othneildrew (README Template)](https://github.com/
+othneildrew) [forks-badge]: https://img.shields.io/github/forks/Zai-Kun/
+reverse-engineered-chatgpt [forks-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/network/members [stars-badge]: https://img.shields.io/
+github/stars/Zai-Kun/reverse-engineered-chatgpt [stars-url]: https://
+github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers [issues-badge]: https:
+//img.shields.io/github/issues/Zai-Kun/reverse-engineered-chatgpt [issues-url]:
+https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues [discussions-
+badge]: https://img.shields.io/github/discussions/Zai-Kun/reverse-engineered-
+chatgpt [discussions-url]: https://github.com/Zai-Kun/reverse-engineered-
+chatgpt/discussions [python-badge]: https://img.shields.io/badge/Python-
+blue?logo=python&logoColor=yellow [python-url]: https://www.python.org/
+[license-badge]: https://img.shields.io/github/license/Zai-Kun/reverse-
+engineered-chatgpt [license-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/blob/main/LICENSE
```

### Comparing `re_gpt-3.0.1/re_gpt/async_chatgpt.py` & `re_gpt-4.0.0/re_gpt/sync_chatgpt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,61 @@
-import asyncio
 import ctypes
 import inspect
-import json
+import time
 import uuid
-from typing import AsyncGenerator, Callable, Optional
-
-from curl_cffi.requests import AsyncSession
+import websockets
+from websockets.exceptions import ConnectionClosed
+import json
+import base64
+import asyncio
+from queue import Queue
+from threading import Thread
+from typing import Callable, Generator, Optional
+
+from curl_cffi.requests import Session
+
+from .async_chatgpt import (
+    BACKUP_ARKOSE_TOKEN_GENERATOR,
+    CHATGPT_API,
+    USER_AGENT,
+    AsyncChatGPT,
+    AsyncConversation,
+    MODELS,
+    WS_REGISTER_URL,
+)
 from .errors import (
     BackendError,
     InvalidSessionToken,
     RetryError,
     TokenNotProvided,
     UnexpectedResponseError,
     InvalidModelName,
 )
-from .utils import async_get_binary_path, get_model_slug
+from .utils import sync_get_binary_path, get_model_slug
+
 
-# Constants
-USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
-CHATGPT_API = "https://chat.openai.com/backend-api/{}"
-BACKUP_ARKOSE_TOKEN_GENERATOR = "https://arkose-token-generator.zaieem.repl.co/token"
-MODELS = {
-    "gpt-4": {"slug": "gpt-4", "needs_arkose_token": True},
-    "gpt-3.5": {"slug": "text-davinci-002-render-sha", "needs_arkose_token": False},
-}
-
-
-class AsyncConversation:
-    def __init__(self, chatgpt, conversation_id=None, model=None):
-        self.chatgpt = chatgpt
-        self.conversation_id = conversation_id
-        self.parent_id = None
-        self.model = model
+class SyncConversation(AsyncConversation):
+    def __init__(self, chatgpt, conversation_id: Optional[str] = None, model=None):
+        super().__init__(chatgpt, conversation_id, model)
 
-    async def fetch_chat(self) -> dict:
+    def fetch_chat(self) -> dict:
         """
         Fetches the chat of the conversation from the API.
 
         Returns:
             dict: The JSON response from the API containing the chat if the conversation_id is not none, else returns an empty dict.
 
         Raises:
             UnexpectedResponseError: If the response is not a valid JSON object or if the response json is not in the expected format
         """
         if not self.conversation_id:
             return {}
 
         url = CHATGPT_API.format(f"conversation/{self.conversation_id}")
-        response = await self.chatgpt.session.get(
+        response = self.chatgpt.session.get(
             url=url, headers=self.chatgpt.build_request_headers()
         )
 
         error = None
         try:
             chat = response.json()
             self.parent_id = list(chat.get("mapping", {}))[-1]
@@ -62,43 +66,43 @@
         except Exception as e:
             error = e
         if error is not None:
             raise UnexpectedResponseError(error, response.text)
 
         return chat
 
-    async def chat(self, user_input: str) -> AsyncGenerator[dict, None]:
+    def chat(self, user_input: str) -> Generator[dict, None, None]:
         """
         As the name implies, chat with ChatGPT.
 
         Args:
             user_input (str): The user's input message.
 
         Yields:
             dict: A dictionary representing assistant responses.
 
         Returns:
-            AsyncGenerator[dict, None]: An asynchronous generator object that yields assistant responses.
+            Generator[dict, None]: A generator object that yields assistant responses.
 
         Raises:
             UnexpectedResponseError: If the response is not a valid JSON object or if the response json is not in the expected format
         """
 
-        payload = await self.build_message_payload(user_input)
+        payload = self.build_message_payload(user_input)
 
         server_response = (
             ""  # To store what the server returned for debugging in case of an error
         )
         error = None
         try:
             full_message = None
             while True:
-                response = self.send_message(payload=payload)
-                async for chunk in response:
-                    decoded_chunk = chunk.decode()
+                response = self.send_message(payload=payload) if not self.chatgpt.websocket_mode else self.send_websocket_message(payload=payload)
+                for chunk in response:
+                    decoded_chunk = chunk.decode() if not self.chatgpt.websocket_mode else chunk
 
                     server_response += decoded_chunk
                     for line in decoded_chunk.splitlines():
                         if not line.startswith("data: "):
                             continue
 
                         raw_json_data = line[6:]
@@ -122,72 +126,126 @@
                             full_message = decoded_json
                 self.conversation_id = full_message["conversation_id"]
                 self.parent_id = full_message["message"]["id"]
                 if (
                     full_message["message"]["metadata"]["finish_details"]["type"]
                     == "max_tokens"
                 ):
-                    payload = await self.build_message_continuation_payload()
+                    payload = self.build_message_continuation_payload()
                 else:
                     break
         except Exception as e:
             error = e
 
         # raising the error outside the 'except' block to prevent the 'During handling of the above exception, another exception occurred' error
         if error is not None:
             raise UnexpectedResponseError(error, server_response)
 
-    async def send_message(self, payload: dict) -> AsyncGenerator[bytes, None]:
+    def send_message(self, payload: dict) -> Generator[bytes, None, None]:
         """
         Send a message payload to the server and receive the response.
 
         Args:
             payload (dict): Payload containing message information.
 
         Yields:
             bytes: Chunk of data received as a response.
         """
-        response_queue = asyncio.Queue()
+        response_queue = Queue()
 
-        async def perform_request():
+        def perform_request():
             def content_callback(chunk):
-                response_queue.put_nowait(chunk)
+                response_queue.put(chunk)
 
             url = CHATGPT_API.format("conversation")
-            await self.chatgpt.session.post(
+            headers = self.chatgpt.build_request_headers()
+            # Add Chat Requirements Token
+            chat_requriments_token = self.chatgpt.create_chat_requirements_token()
+            if chat_requriments_token:
+                headers["openai-sentinel-chat-requirements-token"] = chat_requriments_token
+
+            response = self.chatgpt.session.post(
                 url=url,
-                headers=self.chatgpt.build_request_headers(),
+                headers=headers,
                 json=payload,
                 content_callback=content_callback,
             )
-            await response_queue.put(None)
+            response_queue.put(None)
+
+        Thread(target=perform_request).start()
+
+        while True:
+            chunk = response_queue.get()
+            if chunk is None:
+                break
+            yield chunk
+    
+    def send_websocket_message(self, payload: dict) -> Generator[str, None, None]:
+        """
+        Send a message payload via WebSocket and receive the response.
+
+        Args:
+            payload (dict): Payload containing message information.
+
+        Yields:
+            str: Chunk of data received as a response.
+        """
+
+        response_queue = Queue()
+        websocket_request_id = None
 
-        asyncio.create_task(perform_request())
+        def perform_request():
+            nonlocal websocket_request_id
+            
+            url = CHATGPT_API.format("conversation")
+            headers = self.chatgpt.build_request_headers()
+            # Add Chat Requirements Token
+            chat_requriments_token = self.chatgpt.create_chat_requirements_token()
+            if chat_requriments_token:
+                headers["openai-sentinel-chat-requirements-token"] = chat_requriments_token
+
+            response = (self.chatgpt.session.post(
+                url=url,
+                headers=headers,
+                json=payload,
+            )).json()
+
+            websocket_request_id = response.get("websocket_request_id")
+            
+            if websocket_request_id is None:
+                raise UnexpectedResponseError("WebSocket request ID not found in response", response)
+
+            if websocket_request_id not in self.chatgpt.ws_conversation_map:
+                self.chatgpt.ws_conversation_map[websocket_request_id] = response_queue
+            
+        Thread(target=perform_request).start()
 
         while True:
-            chunk = await response_queue.get()
+            chunk = response_queue.get()
             if chunk is None:
                 break
             yield chunk
 
-    async def build_message_payload(self, user_input: str) -> dict:
+        del self.chatgpt.ws_conversation_map[websocket_request_id]
+
+    def build_message_payload(self, user_input: str) -> dict:
         """
         Build a payload for sending a user message.
 
         Returns:
             dict: Payload containing message information.
         """
         if self.conversation_id and (self.parent_id is None or self.model is None):
-            await self.fetch_chat()  # it will automatically fetch the chat and set the parent id
+            self.fetch_chat()  # it will automatically fetch the chat and set the parent id
 
         payload = {
             "conversation_mode": {"conversation_mode": {"kind": "primary_assistant"}},
             "conversation_id": self.conversation_id,
             "action": "next",
-            "arkose_token": await self.arkose_token_generator()
+            "arkose_token": self.arkose_token_generator()
             if self.chatgpt.generate_arkose_token
             or MODELS[self.model]["needs_arkose_token"]
             else None,
             "force_paragen": False,
             "history_and_training_disabled": False,
             "messages": [
                 {
@@ -197,51 +255,54 @@
                     "metadata": {},
                 }
             ],
             "model": MODELS[self.model]["slug"],
             "parent_message_id": str(uuid.uuid4())
             if not self.parent_id
             else self.parent_id,
+            "websocket_request_id": str(uuid.uuid4())
+            if self.chatgpt.websocket_mode
+            else None,
         }
 
         return payload
 
-    async def build_message_continuation_payload(self) -> dict:
+    def build_message_continuation_payload(self) -> dict:
         """
         Build a payload for continuing ChatGPT's cut off response.
 
         Returns:
             dict: Payload containing message information for continuation.
         """
         payload = {
             "conversation_mode": {"conversation_mode": {"kind": "primary_assistant"}},
             "action": "continue",
-            "arkose_token": await self.arkose_token_generator()
+            "arkose_token": self.arkose_token_generator()
             if self.chatgpt.generate_arkose_token
             or MODELS[self.model]["needs_arkose_token"]
             else None,
             "conversation_id": self.conversation_id,
             "force_paragen": False,
             "history_and_training_disabled": False,
             "model": MODELS[self.model]["slug"],
             "parent_message_id": self.parent_id,
             "timezone_offset_min": -300,
         }
 
         return payload
 
-    async def arkose_token_generator(self) -> str:
+    def arkose_token_generator(self) -> str:
         """
         Generate an Arkose token.
 
         Returns:
             str: Arkose token.
         """
         if not self.chatgpt.tried_downloading_binary:
-            self.chatgpt.binary_path = await async_get_binary_path(self.chatgpt.session)
+            self.chatgpt.binary_path = sync_get_binary_path(self.chatgpt.session)
 
             if self.chatgpt.binary_path:
                 self.chatgpt.arkose = ctypes.CDLL(self.chatgpt.binary_path)
                 self.chatgpt.arkose.GetToken.restype = ctypes.c_char_p
 
             self.chatgpt.tried_downloading_binary = True
 
@@ -249,181 +310,146 @@
             try:
                 result = self.chatgpt.arkose.GetToken()
                 return ctypes.string_at(result).decode("utf-8")
             except:
                 pass
 
         for _ in range(5):
-            response = await self.chatgpt.session.get(BACKUP_ARKOSE_TOKEN_GENERATOR)
+            response = self.chatgpt.session.get(BACKUP_ARKOSE_TOKEN_GENERATOR)
             if response.text == "null":
                 raise BackendError(error_code=505)
             try:
                 return response.json()["token"]
             except:
-                await asyncio.sleep(0.7)
+                time.sleep(0.7)
 
         raise RetryError(website=BACKUP_ARKOSE_TOKEN_GENERATOR)
 
-    async def delete(self) -> None:
+    def delete(self) -> None:
         """
         Deletes the conversation.
         """
         if self.conversation_id:
-            await self.chatgpt.delete_conversation(self.conversation_id)
+            self.chatgpt.delete_conversation(self.conversation_id)
 
             self.conversation_id = None
             self.parent_id = None
 
-    @staticmethod
-    def decode_raw_json(raw_json_data: str) -> dict or bool:
-        """
-        Decode JSON.
-
-        Args:
-            raw_json_data (str): JSON as a string.
 
-        Returns:
-            dict: Decoded JSON.
-        """
-        try:
-            decoded_json = json.loads(raw_json_data.strip())
-            return decoded_json
-        except:
-            return False
-
-    @staticmethod
-    def filter_response(response):
-        processed_response = {
-            "content": response["message"]["content"]["parts"][0],
-            "message_id": response["message"]["id"],
-            "parent_id": response["message"]["metadata"]["parent_id"],
-            "conversation_id": response["conversation_id"],
-        }
-
-        return processed_response
-
-
-class AsyncChatGPT:
+class SyncChatGPT(AsyncChatGPT):
     def __init__(
         self,
         proxies: Optional[dict] = None,
         session_token: Optional[str] = None,
         exit_callback_function: Optional[Callable] = None,
         auth_token: Optional[str] = None,
-        generate_arkose_token: Optional[bool] = False,
+        websocket_mode: Optional[bool] = False,
     ):
         """
         Initializes an instance of the class.
 
         Args:
             proxies (Optional[dict]): A dictionary of proxy settings. Defaults to None.
             session_token (Optional[str]): A session token. Defaults to None.
             exit_callback_function (Optional[callable]): A function to be called on exit. Defaults to None.
             auth_token (Optional[str]): An authentication token. Defaults to None.
-            generate_arkose_token (Optional[bool]): Toggle whether to generate and send arkose-token in the payload. Defaults to False.
+            websocket_mode (Optional[bool]): Toggle whether to use WebSocket for chat. Defaults to False.
         """
-        self.proxies = proxies
-        self.exit_callback_function = exit_callback_function
+        super().__init__(
+            proxies=proxies,
+            session_token=session_token,
+            exit_callback_function=exit_callback_function,
+            auth_token=auth_token,
+            websocket_mode=websocket_mode,
+        )
 
-        self.arkose = None
-        self.binary_path = None
-        self.tried_downloading_binary = False
-        self.generate_arkose_token = generate_arkose_token
-
-        self.session_token = session_token
-        self.auth_token = auth_token
-        self.session = None
+        self.stop_websocket_flag = False
+        self.stop_websocket = None
 
-    async def __aenter__(self):
-        self.session = AsyncSession(
+    def __enter__(self):
+        self.session = Session(
             impersonate="chrome110", timeout=99999, proxies=self.proxies
         )
+
         if self.generate_arkose_token:
-            self.binary_path = await async_get_binary_path(self.session)
+            self.binary_path = sync_get_binary_path(self.session)
 
             if self.binary_path:
                 self.arkose = ctypes.CDLL(self.binary_path)
                 self.arkose.GetToken.restype = ctypes.c_char_p
 
             self.tried_downloading_binary = True
 
         if not self.auth_token:
             if self.session_token is None:
                 raise TokenNotProvided
-            self.auth_token = await self.fetch_auth_token()
+            self.auth_token = self.fetch_auth_token()
+            
+        # automaticly check the status of websocket_mode
+        if not self.websocket_mode:
+            self.websocket_mode = self.check_websocket_availability()
+            
+        if self.websocket_mode:
+            def run_websocket():
+                asyncio.run(self.ensure_websocket())
+            self.ws_loop = Thread(target=run_websocket)
+            self.ws_loop.start()
 
         return self
 
-    async def __aexit__(self, *_):
+    def __exit__(self, *args):
         try:
             if self.exit_callback_function and callable(self.exit_callback_function):
                 if not inspect.iscoroutinefunction(self.exit_callback_function):
                     self.exit_callback_function(self)
         finally:
             self.session.close()
 
-    def build_request_headers(self) -> dict:
-        """
-        Build headers for HTTP requests.
-
-        Returns:
-            dict: Request headers.
-        """
-        headers = {
-            "User-Agent": USER_AGENT,
-            "Accept": "text/event-stream",
-            "Accept-Language": "en-US",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.auth_token}",
-            "Origin": "https://chat.openai.com",
-            "Alt-Used": "chat.openai.com",
-            "Connection": "keep-alive",
-        }
-
-        return headers
+        if self.websocket_mode:
+            self.stop_websocket_flag = True
+            self.ws_loop.join()
 
-    def get_conversation(self, conversation_id: str) -> AsyncConversation:
+    def get_conversation(self, conversation_id: str) -> SyncConversation:
         """
         Makes an instance of class Conversation and return it.
 
         Args:
             conversation_id (str): The ID of the conversation to fetch.
 
         Returns:
             Conversation: Conversation object.
         """
 
-        return AsyncConversation(self, conversation_id)
+        return SyncConversation(self, conversation_id)
 
     def create_new_conversation(
         self, model: Optional[str] = "gpt-3.5"
-    ) -> AsyncConversation:
+    ) -> SyncConversation:
         if model not in MODELS:
             raise InvalidModelName(model, MODELS)
-        return AsyncConversation(self, model=model)
+        return SyncConversation(self, model=model)
 
-    async def delete_conversation(self, conversation_id: str) -> dict:
+    def delete_conversation(self, conversation_id: str) -> dict:
         """
         Delete a conversation.
 
         Args:
             conversation_id (str): Unique identifier for the conversation.
 
         Returns:
             dict: Server response json.
         """
         url = CHATGPT_API.format(f"conversation/{conversation_id}")
-        response = await self.session.patch(
+        response = self.session.patch(
             url=url, headers=self.build_request_headers(), json={"is_visible": False}
         )
 
         return response.json()
 
-    async def fetch_auth_token(self) -> str:
+    def fetch_auth_token(self) -> str:
         """
         Fetch the authentication token for the session.
 
         Raises:
             InvalidSessionToken: If the session token is invalid.
 
         Returns: authentication token.
@@ -445,23 +471,23 @@
                 [
                     f"{cookie_key}={cookie_value}"
                     for cookie_key, cookie_value in cookies.items()
                 ]
             ),
         }
 
-        response = await self.session.get(url=url, headers=headers)
+        response = self.session.get(url=url, headers=headers)
         response_json = response.json()
 
         if "accessToken" in response_json:
             return response_json["accessToken"]
 
         raise InvalidSessionToken
 
-    async def set_custom_instructions(
+    def set_custom_instructions(
         self,
         about_user: Optional[str] = "",
         about_model: Optional[str] = "",
         enable_for_new_chats: Optional[bool] = True,
     ) -> dict:
         """
         Set cuteom instructions for ChatGPT.
@@ -475,27 +501,100 @@
         """
         data = {
             "about_user_message": about_user,
             "about_model_message": about_model,
             "enabled": enable_for_new_chats,
         }
         url = CHATGPT_API.format("user_system_messages")
-        response = await self.session.post(
+        response = self.session.post(
             url=url, headers=self.build_request_headers(), json=data
         )
 
         return response.json()
 
-    async def retrieve_chats(
+    def retrieve_chats(
         self, offset: Optional[int] = 0, limit: Optional[int] = 28
     ) -> dict:
         params = {
             "offset": offset,
             "limit": limit,
             "order": "updated",
         }
         url = CHATGPT_API.format("conversations")
-        response = await self.session.get(
+        response = self.session.get(
             url=url, params=params, headers=self.build_request_headers()
         )
 
         return response.json()
+    
+    def check_websocket_availability(self) -> bool:
+        """
+        Check if WebSocket is available.
+
+        Returns:
+            bool: True if WebSocket is available, otherwise False.
+        """
+        url = CHATGPT_API.format("accounts/check/v4-2023-04-27")
+        response = (self.session.get(
+            url=url, headers=self.build_request_headers()
+        )).json()
+        
+        if 'account_ordering' in response and 'accounts' in response:
+            account_id = response['account_ordering'][0]
+            if account_id in response['accounts']:
+                return 'shared_websocket' in response['accounts'][account_id]['features']
+
+        return False
+    
+    async def ensure_websocket(self):
+        ws_url_rsp = self.session.post(WS_REGISTER_URL, headers=self.build_request_headers()).json()
+        ws_url = ws_url_rsp['wss_url']
+        access_token = self.extract_access_token(ws_url)
+        asyncio.create_task(self.ensure_close_websocket())
+        await self.listen_to_websocket(ws_url, access_token)
+        
+    async def ensure_close_websocket(self):
+        while True:
+            if self.stop_websocket_flag:
+                break
+            await asyncio.sleep(1)
+        await self.stop_websocket()
+
+    async def listen_to_websocket(self, ws_url: str, access_token: str):
+        headers = {'Authorization': f'Bearer {access_token}'}
+        async with websockets.connect(ws_url, extra_headers=headers) as websocket:
+            async def stop_websocket():
+                await websocket.close()
+            self.stop_websocket = stop_websocket
+
+            while True:
+                message = None
+                try:
+                    message = await websocket.recv()
+                except ConnectionClosed:
+                    break
+                message_data = json.loads(message)
+                body_encoded = message_data.get("body", "")
+                ws_id = message_data.get("websocket_request_id", "")
+                decoded_body = base64.b64decode(body_encoded).decode('utf-8')
+                response_queue = self.ws_conversation_map.get(ws_id)
+                if response_queue is None:
+                    continue
+                response_queue.put_nowait(decoded_body)
+                if '[DONE]' in decoded_body or '[ERROR]' in decoded_body:
+                    response_queue.put(None)
+                    continue
+
+    def create_chat_requirements_token(self):
+        """
+        Get a chat requirements token from chatgpt server
+
+        Returns:
+            str: chat requirements token
+        """
+        url = CHATGPT_API.format("sentinel/chat-requirements")
+        response = self.session.post(
+            url=url, headers=self.build_request_headers()
+        )
+        body = response.json()
+        token = body.get("token", None)
+        return token
```

### Comparing `re_gpt-3.0.1/re_gpt/errors.py` & `re_gpt-4.0.0/re_gpt/errors.py`

 * *Files identical despite different names*

### Comparing `re_gpt-3.0.1/re_gpt/sync_chatgpt.py` & `re_gpt-4.0.0/re_gpt/async_chatgpt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,63 @@
+import asyncio
+import base64
 import ctypes
 import inspect
-import time
+import json
+import re
 import uuid
-from queue import Queue
-from threading import Thread
-from typing import Callable, Generator, Optional
-
-from curl_cffi.requests import Session
-
-from .async_chatgpt import (
-    BACKUP_ARKOSE_TOKEN_GENERATOR,
-    CHATGPT_API,
-    USER_AGENT,
-    AsyncChatGPT,
-    AsyncConversation,
-    MODELS,
-)
+from typing import AsyncGenerator, Callable, Optional
+
+import websockets
+from curl_cffi.requests import AsyncSession
+
 from .errors import (
     BackendError,
+    InvalidModelName,
     InvalidSessionToken,
     RetryError,
     TokenNotProvided,
     UnexpectedResponseError,
-    InvalidModelName,
 )
-from .utils import sync_get_binary_path, get_model_slug
+from .utils import async_get_binary_path, get_model_slug
 
+# Constants
+USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
+CHATGPT_API = "https://chat.openai.com/backend-api/{}"
+BACKUP_ARKOSE_TOKEN_GENERATOR = "https://arkose-token-generator.zaieem.repl.co/token"
+WS_REGISTER_URL = CHATGPT_API.format("register-websocket")
+
+MODELS = {
+    "gpt-4": {"slug": "gpt-4", "needs_arkose_token": True},
+    "gpt-3.5": {"slug": "text-davinci-002-render-sha", "needs_arkose_token": False},
+}
+
+
+class AsyncConversation:
+    def __init__(self, chatgpt, conversation_id=None, model=None):
+        self.chatgpt = chatgpt
+        self.conversation_id = conversation_id
+        self.parent_id = None
+        self.model = model
 
-class SyncConversation(AsyncConversation):
-    def __init__(self, chatgpt, conversation_id: Optional[str] = None, model=None):
-        super().__init__(chatgpt, conversation_id, model)
-
-    def fetch_chat(self) -> dict:
+    async def fetch_chat(self) -> dict:
         """
         Fetches the chat of the conversation from the API.
 
         Returns:
             dict: The JSON response from the API containing the chat if the conversation_id is not none, else returns an empty dict.
 
         Raises:
             UnexpectedResponseError: If the response is not a valid JSON object or if the response json is not in the expected format
         """
         if not self.conversation_id:
             return {}
 
         url = CHATGPT_API.format(f"conversation/{self.conversation_id}")
-        response = self.chatgpt.session.get(
+        response = await self.chatgpt.session.get(
             url=url, headers=self.chatgpt.build_request_headers()
         )
 
         error = None
         try:
             chat = response.json()
             self.parent_id = list(chat.get("mapping", {}))[-1]
@@ -60,43 +68,49 @@
         except Exception as e:
             error = e
         if error is not None:
             raise UnexpectedResponseError(error, response.text)
 
         return chat
 
-    def chat(self, user_input: str) -> Generator[dict, None, None]:
+    async def chat(self, user_input: str) -> AsyncGenerator[dict, None]:
         """
         As the name implies, chat with ChatGPT.
 
         Args:
             user_input (str): The user's input message.
 
         Yields:
             dict: A dictionary representing assistant responses.
 
         Returns:
-            Generator[dict, None]: A generator object that yields assistant responses.
+            AsyncGenerator[dict, None]: An asynchronous generator object that yields assistant responses.
 
         Raises:
             UnexpectedResponseError: If the response is not a valid JSON object or if the response json is not in the expected format
         """
 
-        payload = self.build_message_payload(user_input)
+        payload = await self.build_message_payload(user_input)
 
         server_response = (
             ""  # To store what the server returned for debugging in case of an error
         )
         error = None
         try:
             full_message = None
             while True:
-                response = self.send_message(payload=payload)
-                for chunk in response:
-                    decoded_chunk = chunk.decode()
+                response = (
+                    self.send_message(payload=payload)
+                    if not self.chatgpt.websocket_mode
+                    else self.send_websocket_message(payload=payload)
+                )
+                async for chunk in response:
+                    decoded_chunk = (
+                        chunk.decode() if isinstance(chunk, bytes) else chunk
+                    )
 
                     server_response += decoded_chunk
                     for line in decoded_chunk.splitlines():
                         if not line.startswith("data: "):
                             continue
 
                         raw_json_data = line[6:]
@@ -120,72 +134,136 @@
                             full_message = decoded_json
                 self.conversation_id = full_message["conversation_id"]
                 self.parent_id = full_message["message"]["id"]
                 if (
                     full_message["message"]["metadata"]["finish_details"]["type"]
                     == "max_tokens"
                 ):
-                    payload = self.build_message_continuation_payload()
+                    payload = await self.build_message_continuation_payload()
                 else:
                     break
         except Exception as e:
             error = e
 
         # raising the error outside the 'except' block to prevent the 'During handling of the above exception, another exception occurred' error
         if error is not None:
             raise UnexpectedResponseError(error, server_response)
 
-    def send_message(self, payload: dict) -> Generator[bytes, None, None]:
+    async def send_message(self, payload: dict) -> AsyncGenerator[bytes, None]:
         """
         Send a message payload to the server and receive the response.
 
         Args:
             payload (dict): Payload containing message information.
 
         Yields:
             bytes: Chunk of data received as a response.
         """
-        response_queue = Queue()
+        response_queue = asyncio.Queue()
 
-        def perform_request():
+        async def perform_request():
             def content_callback(chunk):
-                response_queue.put(chunk)
+                response_queue.put_nowait(chunk)
 
             url = CHATGPT_API.format("conversation")
-            response = self.chatgpt.session.post(
+
+            headers = self.chatgpt.build_request_headers()
+            # Add Chat Requirements Token
+            chat_requriments_token = await self.chatgpt.create_chat_requirements_token()
+            if chat_requriments_token:
+                headers[
+                    "openai-sentinel-chat-requirements-token"
+                ] = chat_requriments_token
+
+            await self.chatgpt.session.post(
                 url=url,
-                headers=self.chatgpt.build_request_headers(),
+                headers=headers,
                 json=payload,
                 content_callback=content_callback,
             )
-            response_queue.put(None)
+            await response_queue.put(None)
 
-        Thread(target=perform_request).start()
+        asyncio.create_task(perform_request())
 
         while True:
-            chunk = response_queue.get()
+            chunk = await response_queue.get()
             if chunk is None:
                 break
             yield chunk
 
-    def build_message_payload(self, user_input: str) -> dict:
+    async def send_websocket_message(self, payload: dict) -> AsyncGenerator[str, None]:
+        """
+        Send a message payload via WebSocket and receive the response.
+
+        Args:
+            payload (dict): Payload containing message information.
+
+        Yields:
+            str: Chunk of data received as a response.
+        """
+        await self.chatgpt.ensure_websocket()
+
+        response_queue = asyncio.Queue()
+        websocket_request_id = None
+
+        async def perform_request():
+            nonlocal websocket_request_id
+
+            url = CHATGPT_API.format("conversation")
+            headers = self.chatgpt.build_request_headers()
+            # Add Chat Requirements Token
+            chat_requriments_token = await self.chatgpt.create_chat_requirements_token()
+            if chat_requriments_token:
+                headers[
+                    "openai-sentinel-chat-requirements-token"
+                ] = chat_requriments_token
+
+            response = (
+                await self.chatgpt.session.post(
+                    url=url,
+                    headers=headers,
+                    json=payload,
+                )
+            ).json()
+
+            websocket_request_id = response.get("websocket_request_id")
+
+            if websocket_request_id is None:
+                raise UnexpectedResponseError(
+                    "WebSocket request ID not found in response", response
+                )
+
+            if websocket_request_id not in self.chatgpt.ws_conversation_map:
+                self.chatgpt.ws_conversation_map[websocket_request_id] = response_queue
+
+        asyncio.create_task(perform_request())
+
+        while True:
+            chunk = await response_queue.get()
+            if chunk is None:
+                break
+            yield chunk
+
+        del self.chatgpt.ws_conversation_map[websocket_request_id]
+
+    async def build_message_payload(self, user_input: str) -> dict:
         """
         Build a payload for sending a user message.
 
         Returns:
             dict: Payload containing message information.
         """
         if self.conversation_id and (self.parent_id is None or self.model is None):
-            self.fetch_chat()  # it will automatically fetch the chat and set the parent id
+            await self.fetch_chat()  # it will automatically fetch the chat and set the parent id
 
         payload = {
             "conversation_mode": {"conversation_mode": {"kind": "primary_assistant"}},
             "conversation_id": self.conversation_id,
             "action": "next",
-            "arkose_token": self.arkose_token_generator()
+            "arkose_token": await self.arkose_token_generator()
             if self.chatgpt.generate_arkose_token
             or MODELS[self.model]["needs_arkose_token"]
             else None,
             "force_paragen": False,
             "history_and_training_disabled": False,
             "messages": [
                 {
@@ -195,51 +273,54 @@
                     "metadata": {},
                 }
             ],
             "model": MODELS[self.model]["slug"],
             "parent_message_id": str(uuid.uuid4())
             if not self.parent_id
             else self.parent_id,
+            "websocket_request_id": str(uuid.uuid4())
+            if self.chatgpt.websocket_mode
+            else None,
         }
 
         return payload
 
-    def build_message_continuation_payload(self) -> dict:
+    async def build_message_continuation_payload(self) -> dict:
         """
         Build a payload for continuing ChatGPT's cut off response.
 
         Returns:
             dict: Payload containing message information for continuation.
         """
         payload = {
             "conversation_mode": {"conversation_mode": {"kind": "primary_assistant"}},
             "action": "continue",
-            "arkose_token": self.arkose_token_generator()
+            "arkose_token": await self.arkose_token_generator()
             if self.chatgpt.generate_arkose_token
             or MODELS[self.model]["needs_arkose_token"]
             else None,
             "conversation_id": self.conversation_id,
             "force_paragen": False,
             "history_and_training_disabled": False,
             "model": MODELS[self.model]["slug"],
             "parent_message_id": self.parent_id,
             "timezone_offset_min": -300,
         }
 
         return payload
 
-    def arkose_token_generator(self) -> str:
+    async def arkose_token_generator(self) -> str:
         """
         Generate an Arkose token.
 
         Returns:
             str: Arkose token.
         """
         if not self.chatgpt.tried_downloading_binary:
-            self.chatgpt.binary_path = sync_get_binary_path(self.chatgpt.session)
+            self.chatgpt.binary_path = await async_get_binary_path(self.chatgpt.session)
 
             if self.chatgpt.binary_path:
                 self.chatgpt.arkose = ctypes.CDLL(self.chatgpt.binary_path)
                 self.chatgpt.arkose.GetToken.restype = ctypes.c_char_p
 
             self.chatgpt.tried_downloading_binary = True
 
@@ -247,126 +328,196 @@
             try:
                 result = self.chatgpt.arkose.GetToken()
                 return ctypes.string_at(result).decode("utf-8")
             except:
                 pass
 
         for _ in range(5):
-            response = self.chatgpt.session.get(BACKUP_ARKOSE_TOKEN_GENERATOR)
+            response = await self.chatgpt.session.get(BACKUP_ARKOSE_TOKEN_GENERATOR)
             if response.text == "null":
                 raise BackendError(error_code=505)
             try:
                 return response.json()["token"]
             except:
-                time.sleep(0.7)
+                await asyncio.sleep(0.7)
 
         raise RetryError(website=BACKUP_ARKOSE_TOKEN_GENERATOR)
 
-    def delete(self) -> None:
+    async def delete(self) -> None:
         """
         Deletes the conversation.
         """
         if self.conversation_id:
-            self.chatgpt.delete_conversation(self.conversation_id)
+            await self.chatgpt.delete_conversation(self.conversation_id)
 
             self.conversation_id = None
             self.parent_id = None
 
+    @staticmethod
+    def decode_raw_json(raw_json_data: str) -> dict or bool:
+        """
+        Decode JSON.
+
+        Args:
+            raw_json_data (str): JSON as a string.
 
-class SyncChatGPT(AsyncChatGPT):
+        Returns:
+            dict: Decoded JSON.
+        """
+        try:
+            decoded_json = json.loads(raw_json_data.strip())
+            return decoded_json
+        except:
+            return False
+
+    @staticmethod
+    def filter_response(response):
+        processed_response = {
+            "content": response["message"]["content"]["parts"][0],
+            "message_id": response["message"]["id"],
+            "parent_id": response["message"]["metadata"]["parent_id"],
+            "conversation_id": response["conversation_id"],
+        }
+
+        return processed_response
+
+
+class AsyncChatGPT:
     def __init__(
         self,
         proxies: Optional[dict] = None,
         session_token: Optional[str] = None,
         exit_callback_function: Optional[Callable] = None,
         auth_token: Optional[str] = None,
+        generate_arkose_token: Optional[bool] = False,
+        websocket_mode: Optional[bool] = False,
     ):
         """
         Initializes an instance of the class.
 
         Args:
             proxies (Optional[dict]): A dictionary of proxy settings. Defaults to None.
             session_token (Optional[str]): A session token. Defaults to None.
             exit_callback_function (Optional[callable]): A function to be called on exit. Defaults to None.
             auth_token (Optional[str]): An authentication token. Defaults to None.
+            generate_arkose_token (Optional[bool]): Toggle whether to generate and send arkose-token in the payload. Defaults to False.
+            websocket_mode (Optional[bool]): Toggle whether to use WebSocket for chat. Defaults to False.
         """
-        super().__init__(
-            proxies=proxies,
-            session_token=session_token,
-            exit_callback_function=exit_callback_function,
-            auth_token=auth_token,
-        )
+        self.proxies = proxies
+        self.exit_callback_function = exit_callback_function
 
-    def __enter__(self):
-        self.session = Session(
+        self.arkose = None
+        self.binary_path = None
+        self.tried_downloading_binary = False
+        self.generate_arkose_token = generate_arkose_token
+
+        self.session_token = session_token
+        self.auth_token = auth_token
+        self.session = None
+
+        self.websocket_mode = websocket_mode
+        self.ws_loop = None
+        self.ws_conversation_map = {}
+
+    async def __aenter__(self):
+        self.session = AsyncSession(
             impersonate="chrome110", timeout=99999, proxies=self.proxies
         )
-
         if self.generate_arkose_token:
-            self.binary_path = sync_get_binary_path(self.session)
+            self.binary_path = await async_get_binary_path(self.session)
 
             if self.binary_path:
                 self.arkose = ctypes.CDLL(self.binary_path)
                 self.arkose.GetToken.restype = ctypes.c_char_p
 
             self.tried_downloading_binary = True
 
         if not self.auth_token:
             if self.session_token is None:
                 raise TokenNotProvided
-            self.auth_token = self.fetch_auth_token()
+            self.auth_token = await self.fetch_auth_token()
+
+        if not self.websocket_mode:
+            self.websocket_mode = await self.check_websocket_availability()
+
+        if self.websocket_mode:
+            await self.ensure_websocket()
 
         return self
 
-    def __exit__(self, *args):
+    async def __aexit__(self, *_):
         try:
             if self.exit_callback_function and callable(self.exit_callback_function):
                 if not inspect.iscoroutinefunction(self.exit_callback_function):
                     self.exit_callback_function(self)
         finally:
-            self.session.close()
+            if inspect.iscoroutinefunction(self.session.close):
+                await self.session.close()
+            else:
+                self.session.close()
+
+    def build_request_headers(self) -> dict:
+        """
+        Build headers for HTTP requests.
+
+        Returns:
+            dict: Request headers.
+        """
+        headers = {
+            "User-Agent": USER_AGENT,
+            "Accept": "text/event-stream",
+            "Accept-Language": "en-US",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.auth_token}",
+            "Origin": "https://chat.openai.com",
+            "Alt-Used": "chat.openai.com",
+            "Connection": "keep-alive",
+        }
+
+        return headers
 
-    def get_conversation(self, conversation_id: str) -> SyncConversation:
+    def get_conversation(self, conversation_id: str) -> AsyncConversation:
         """
         Makes an instance of class Conversation and return it.
 
         Args:
             conversation_id (str): The ID of the conversation to fetch.
 
         Returns:
             Conversation: Conversation object.
         """
 
-        return SyncConversation(self, conversation_id)
+        return AsyncConversation(self, conversation_id)
 
     def create_new_conversation(
         self, model: Optional[str] = "gpt-3.5"
-    ) -> SyncConversation:
+    ) -> AsyncConversation:
         if model not in MODELS:
             raise InvalidModelName(model, MODELS)
-        return SyncConversation(self, model=model)
+        return AsyncConversation(self, model=model)
 
-    def delete_conversation(self, conversation_id: str) -> dict:
+    async def delete_conversation(self, conversation_id: str) -> dict:
         """
         Delete a conversation.
 
         Args:
             conversation_id (str): Unique identifier for the conversation.
 
         Returns:
             dict: Server response json.
         """
         url = CHATGPT_API.format(f"conversation/{conversation_id}")
-        response = self.session.patch(
+        response = await self.session.patch(
             url=url, headers=self.build_request_headers(), json={"is_visible": False}
         )
 
         return response.json()
 
-    def fetch_auth_token(self) -> str:
+    async def fetch_auth_token(self) -> str:
         """
         Fetch the authentication token for the session.
 
         Raises:
             InvalidSessionToken: If the session token is invalid.
 
         Returns: authentication token.
@@ -388,23 +539,23 @@
                 [
                     f"{cookie_key}={cookie_value}"
                     for cookie_key, cookie_value in cookies.items()
                 ]
             ),
         }
 
-        response = self.session.get(url=url, headers=headers)
+        response = await self.session.get(url=url, headers=headers)
         response_json = response.json()
 
         if "accessToken" in response_json:
             return response_json["accessToken"]
 
         raise InvalidSessionToken
 
-    def set_custom_instructions(
+    async def set_custom_instructions(
         self,
         about_user: Optional[str] = "",
         about_model: Optional[str] = "",
         enable_for_new_chats: Optional[bool] = True,
     ) -> dict:
         """
         Set cuteom instructions for ChatGPT.
@@ -418,27 +569,103 @@
         """
         data = {
             "about_user_message": about_user,
             "about_model_message": about_model,
             "enabled": enable_for_new_chats,
         }
         url = CHATGPT_API.format("user_system_messages")
-        response = self.session.post(
+        response = await self.session.post(
             url=url, headers=self.build_request_headers(), json=data
         )
 
         return response.json()
 
-    def retrieve_chats(
+    async def retrieve_chats(
         self, offset: Optional[int] = 0, limit: Optional[int] = 28
     ) -> dict:
         params = {
             "offset": offset,
             "limit": limit,
             "order": "updated",
         }
         url = CHATGPT_API.format("conversations")
-        response = self.session.get(
+        response = await self.session.get(
             url=url, params=params, headers=self.build_request_headers()
         )
 
         return response.json()
+
+    async def check_websocket_availability(self) -> bool:
+        """
+        Check if WebSocket is available.
+
+        Returns:
+            bool: True if WebSocket is available, otherwise False.
+        """
+        url = CHATGPT_API.format("accounts/check/v4-2023-04-27")
+        response = (
+            await self.session.get(url=url, headers=self.build_request_headers())
+        ).json()
+
+        if "account_ordering" in response and "accounts" in response:
+            account_id = response["account_ordering"][0]
+            if account_id in response["accounts"]:
+                return (
+                    "shared_websocket" in response["accounts"][account_id]["features"]
+                )
+
+        return False
+
+    async def ensure_websocket(self):
+        if not self.ws_loop:
+            ws_url_rsp = (
+                await self.session.post(
+                    WS_REGISTER_URL, headers=self.build_request_headers()
+                )
+            ).json()
+            ws_url = ws_url_rsp["wss_url"]
+            access_token = self.extract_access_token(ws_url)
+            self.ws_loop = asyncio.create_task(
+                self.listen_to_websocket(ws_url, access_token)
+            )
+
+    def extract_access_token(self, url):
+        match = re.search(r"access_token=([^&]*)", url)
+        if match:
+            return match.group(1)
+        else:
+            return None
+
+    async def listen_to_websocket(self, ws_url: str, access_token: str):
+        headers = {"Authorization": f"Bearer {access_token}"}
+        async with websockets.connect(ws_url, extra_headers=headers) as websocket:
+            while True:
+                message = await websocket.recv()
+                message_data = json.loads(message)
+                body_encoded = message_data.get("body", "")
+                ws_id = message_data.get("websocket_request_id", "")
+                decoded_body = base64.b64decode(body_encoded).decode("utf-8")
+                response_queue = self.ws_conversation_map.get(ws_id)
+                if response_queue is None:
+                    continue
+                if "title_generation" in decoded_body:
+                    # skip
+                    continue
+                response_queue.put_nowait(decoded_body)
+                if "[DONE]" in decoded_body or "[ERROR]" in decoded_body:
+                    await response_queue.put(None)
+                    continue
+
+    async def create_chat_requirements_token(self):
+        """
+        Get a chat requirements token from chatgpt server
+
+        Returns:
+            str: chat requirements token
+        """
+        url = CHATGPT_API.format("sentinel/chat-requirements")
+        response = await self.session.post(
+            url=url, headers=self.build_request_headers()
+        )
+        body = response.json()
+        token = body.get("token", None)
+        return token
```

### Comparing `re_gpt-3.0.1/re_gpt/utils.py` & `re_gpt-4.0.0/re_gpt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,10 +127,11 @@
 
     return binary_path
 
 
 def get_model_slug(chat):
     for _, message in chat.get("mapping", {}).items():
         if "message" in message:
-            role = message["message"]["author"]["role"]
-            if role == "assistant":
-                return message["message"]["metadata"]["model_slug"]
+            if message["message"]:
+                role = message["message"]["author"]["role"]
+                if role == "assistant":
+                    return message["message"]["metadata"]["model_slug"]
```

### Comparing `re_gpt-3.0.1/re_gpt.egg-info/PKG-INFO` & `re_gpt-4.0.0/re_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: re_gpt
-Version: 3.0.1
+Version: 4.0.0
 Summary: Unofficial reverse-engineered ChatGPT API in Python.
 Home-page: https://github.com/Zai-Kun/reverse-engineered-chatgpt
 Author: Zai-Kun
 Project-URL: Bug Tracker, https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curl_cffi==0.5.9
+Requires-Dist: websockets==12.0
 
 <div align="center">
   <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt">  </a>
 
 <h1 align="center">Reverse Engineered <a href="https://openai.com/blog/chatgpt">ChatGPT</a> API</h1>
 
   <p align="center">
@@ -19,14 +20,16 @@
 
 [![Stargazers][stars-badge]][stars-url]
 [![Forks][forks-badge]][forks-url]
 [![Discussions][discussions-badge]][discussions-url]
 [![Issues][issues-badge]][issues-url]
 [![MIT License][license-badge]][license-url]
 
+  English | [简体中文](./docs/zh-README.md)
+
   </p>
     <p align="center">
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt"></a>
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues">Report Bug</a>
     |
     <a href="https://github.com/Zai-Kun/reverse-engineered-chatgpt/discussions">Request Feature</a>
   </p>
@@ -190,15 +193,15 @@
 
 Zai-Kun - [Discord Server](https://discord.gg/ymcqxudVJG)
 
 Repo Link: <https://github.com/Zai-Kun/reverse-engineered-chatgpt>
 
 ## Acknowledgments
 
-- [sudoAlphaX](https://github.com/sudoAlphaX)
+- [sudoAlphaX (for writing this readme)](https://github.com/sudoAlphaX)
 
 - [yifeikong (curl-cffi module)](https://github.com/yifeikong/curl_cffi)
 
 - [acheong08 (implementation to obtain arkose_token)](https://github.com/acheong08/funcaptcha)
 
 - [pyca (cryptography module)](https://github.com/pyca/cryptography/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 2.1 Name: re_gpt Version: 3.0.1 Summary: Unofficial reverse-
+Metadata-Version: 2.1 Name: re_gpt Version: 4.0.0 Summary: Unofficial reverse-
 engineered ChatGPT API in Python. Home-page: https://github.com/Zai-Kun/
 reverse-engineered-chatgpt Author: Zai-Kun Project-URL: Bug Tracker, https://
 github.com/Zai-Kun/reverse-engineered-chatgpt/issues Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: curl_cffi==0.5.9
+text/markdown License-File: LICENSE Requires-Dist: curl_cffi==0.5.9 Requires-
+Dist: websockets==12.0
                  ************ RReevveerrssee EEnnggiinneeeerreedd _CC_hh_aa_tt_GG_PP_TT AAPPII ************
 Use OpenAI ChatGPT in your Python code without an API key [![Stargazers][stars-
      badge]][stars-url] [![Forks][forks-badge]][forks-url] [![Discussions]
 [discussions-badge]][discussions-url] [![Issues][issues-badge]][issues-url] [!
-                  [MIT License][license-badge]][license-url]
+[MIT License][license-badge]][license-url] English | [ç®ä½ä¸­æ](./docs/zh-
+                                  README.md)
                          _R_e_p_o_r_t_ _B_u_g | _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _I_n_s_p_i_r_a_t_i_o_n
           o _H_o_w_ _i_t_ _w_o_r_k_s
           o _B_u_i_l_t_ _u_s_i_n_g
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -73,27 +75,28 @@
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request ## License Distributed under the Apache
 License 2.0. See [`LICENSE`](https://github.com/Zai-Kun/reverse-engineered-
 chatgpt/blob/main/LICENSE) for more information. ## Contact/Bug report Zai-Kun
 - [Discord Server](https://discord.gg/ymcqxudVJG) Repo Link:
-github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments -
-[sudoAlphaX](https://github.com/sudoAlphaX) - [yifeikong (curl-cffi module)]
-(https://github.com/yifeikong/curl_cffi) - [acheong08 (implementation to obtain
-arkose_token)](https://github.com/acheong08/funcaptcha) - [pyca (cryptography
-module)](https://github.com/pyca/cryptography/) - [Legrandin (pycryptodome
-module)](https://github.com/Legrandin/pycryptodome/) - [othneildrew (README
-Template)](https://github.com/othneildrew) [forks-badge]: https://
-img.shields.io/github/forks/Zai-Kun/reverse-engineered-chatgpt [forks-url]:
-https://github.com/Zai-Kun/reverse-engineered-chatgpt/network/members [stars-
-badge]: https://img.shields.io/github/stars/Zai-Kun/reverse-engineered-chatgpt
-[stars-url]: https://github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers
-[issues-badge]: https://img.shields.io/github/issues/Zai-Kun/reverse-
-engineered-chatgpt [issues-url]: https://github.com/Zai-Kun/reverse-engineered-
-chatgpt/issues [discussions-badge]: https://img.shields.io/github/discussions/
-Zai-Kun/reverse-engineered-chatgpt [discussions-url]: https://github.com/Zai-
-Kun/reverse-engineered-chatgpt/discussions [python-badge]: https://
-img.shields.io/badge/Python-blue?logo=python&logoColor=yellow [python-url]:
-https://www.python.org/ [license-badge]: https://img.shields.io/github/license/
-Zai-Kun/reverse-engineered-chatgpt [license-url]: https://github.com/Zai-Kun/
-reverse-engineered-chatgpt/blob/main/LICENSE
+github.com/Zai-Kun/reverse-engineered-chatgpt> ## Acknowledgments - [sudoAlphaX
+(for writing this readme)](https://github.com/sudoAlphaX) - [yifeikong (curl-
+cffi module)](https://github.com/yifeikong/curl_cffi) - [acheong08
+(implementation to obtain arkose_token)](https://github.com/acheong08/
+funcaptcha) - [pyca (cryptography module)](https://github.com/pyca/
+cryptography/) - [Legrandin (pycryptodome module)](https://github.com/
+Legrandin/pycryptodome/) - [othneildrew (README Template)](https://github.com/
+othneildrew) [forks-badge]: https://img.shields.io/github/forks/Zai-Kun/
+reverse-engineered-chatgpt [forks-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/network/members [stars-badge]: https://img.shields.io/
+github/stars/Zai-Kun/reverse-engineered-chatgpt [stars-url]: https://
+github.com/Zai-Kun/reverse-engineered-chatgpt/stargazers [issues-badge]: https:
+//img.shields.io/github/issues/Zai-Kun/reverse-engineered-chatgpt [issues-url]:
+https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues [discussions-
+badge]: https://img.shields.io/github/discussions/Zai-Kun/reverse-engineered-
+chatgpt [discussions-url]: https://github.com/Zai-Kun/reverse-engineered-
+chatgpt/discussions [python-badge]: https://img.shields.io/badge/Python-
+blue?logo=python&logoColor=yellow [python-url]: https://www.python.org/
+[license-badge]: https://img.shields.io/github/license/Zai-Kun/reverse-
+engineered-chatgpt [license-url]: https://github.com/Zai-Kun/reverse-
+engineered-chatgpt/blob/main/LICENSE
```

### Comparing `re_gpt-3.0.1/setup.py` & `re_gpt-4.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 setup(
     name="re_gpt",
-    version="3.0.1",
+    version="4.0.0",
     author="Zai-Kun",
     description="Unofficial reverse-engineered ChatGPT API in Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Zai-Kun/reverse-engineered-chatgpt",
     project_urls={
         "Bug Tracker": "https://github.com/Zai-Kun/reverse-engineered-chatgpt/issues",
     },
     packages=find_packages(),
-    install_requires=["curl_cffi==0.5.9"],
+    install_requires=["curl_cffi==0.5.9", "websockets==12.0"],
 )
```

