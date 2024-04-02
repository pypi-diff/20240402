# Comparing `tmp/boomgate-0.0.1a1.tar.gz` & `tmp/boomgate-0.0.1a2.tar.gz`

## Comparing `boomgate-0.0.1a1.tar` & `boomgate-0.0.1a2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/__version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/cached_http.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/cli.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/inspect.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/logging.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/vulnerabilities.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/ecosystems/__init__.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/src/boomgate/ecosystems/pypi.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/README.md
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0    43333 2020-02-02 00:00:00.000000 boomgate-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/__version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/cached_http.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/cli.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/inspect.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/test_cached_http.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/vulnerabilities.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/ecosystems/__init__.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/src/boomgate/ecosystems/pypi.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/README.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0    43720 2020-02-02 00:00:00.000000 boomgate-0.0.1a2/PKG-INFO
```

### Comparing `boomgate-0.0.1a1/src/boomgate/cached_http.py` & `boomgate-0.0.1a2/src/boomgate/cached_http.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/cli.py` & `boomgate-0.0.1a2/src/boomgate/cli.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/inspect.py` & `boomgate-0.0.1a2/src/boomgate/inspect.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/logging.py` & `boomgate-0.0.1a2/src/boomgate/logging.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/vulnerabilities.py` & `boomgate-0.0.1a2/src/boomgate/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/ecosystems/__init__.py` & `boomgate-0.0.1a2/src/boomgate/ecosystems/__init__.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/src/boomgate/ecosystems/pypi.py` & `boomgate-0.0.1a2/src/boomgate/ecosystems/pypi.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/.gitignore` & `boomgate-0.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/LICENSE` & `boomgate-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1a1/README.md` & `boomgate-0.0.1a2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 <h1 align="center">Boomgate</h1>
 <p align="center"><em>
     Identify and mitigate the risks of using third-party libraries.
 </em></p>
 
 <p align="center">
-    <a href="https://pypi.org/project/boomgate/">
-        <img src="https://img.shields.io/pypi/v/boomgate?color=%2334D058&label=PyPI%20package" alt="PyPI version">
-    </a>
-    <a href="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml">
-        <img src="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml/badge.svg" alt="Release workflow status">
-    </a>
+    <a href="https://pypi.org/project/boomgate/"><img src="https://img.shields.io/pypi/v/boomgate?color=%2334D058&label=PyPI%20package" alt="PyPI version"></a>
+    <a href="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml"><img src="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml/badge.svg" alt="Release workflow status"></a>
+    <a href="https://codecov.io/gh/KyeRussell/boomgate" ><img src="https://codecov.io/gh/KyeRussell/boomgate/graph/badge.svg?token=2XY75VWMGK"></a>
+    <a href="https://boomgate.readthedocs.io"><img src="https://readthedocs.org/projects/boomgate/badge/" alt="Documentation on Read The Docs"></a>
 </p>
 
 ---
 
 This project is not remotely ready for anyone to look at, let alone use. It is in a
 very early proof-of-concept stage, focusing on iterative research and development. I
 have not settled on the project's architecture, and I am still exploring the problem
@@ -47,7 +45,13 @@
 Clone the repository and run the following command:
 
 ```bash
 uv pip install -e . -r pyproject.toml --extra=dev --extra=docs
 ```
 
 This will install the project in editable mode with all development dependencies.
+
+### Running tests
+
+```bash
+pytest
+```
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
                             ************ BBoooommggaattee ************
         IIddeennttiiffyy aanndd mmiittiiggaattee tthhee rriisskkss ooff uussiinngg tthhiirrdd--ppaarrttyy lliibbrraarriieess..
-                    _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_R_e_l_e_a_s_e_ _w_o_r_k_f_l_o_w_ _s_t_a_t_u_s_]
+   _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_R_e_l_e_a_s_e_ _w_o_r_k_f_l_o_w_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_K_y_e_R_u_s_s_e_l_l_/
+  _b_o_o_m_g_a_t_e_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_2_X_Y_7_5_V_W_M_G_K_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_n_ _R_e_a_d_ _T_h_e_ _D_o_c_s_]
 --- This project is not remotely ready for anyone to look at, let alone use. It
 is in a very early proof-of-concept stage, focusing on iterative research and
 development. I have not settled on the project's architecture, and I am still
 exploring the problem space. As such, the quality of the code is very poor, and
 things are guaranteed to change. I will not provide support, nor will I accept
 PRs at this time. --- ## Vision I intend for Boomgate to allow you to define a
 policy for your project that describes the risks you are willing to accept when
@@ -17,8 +18,8 @@
 dependencies) require a security audit before they can be used. In this
 example, Boomgate can be configured to block your project's CI/CD pipeline if
 one of these conditions is met by your project's resolved dependencies. See my
 rough list of idea in the [GitHub issues list](https://github.com/KyeRussell/
 boomgate/issues). ## Developing Clone the repository and run the following
 command: ```bash uv pip install -e . -r pyproject.toml --extra=dev --extra=docs
 ``` This will install the project in editable mode with all development
-dependencies.
+dependencies. ### Running tests ```bash pytest ```
```

### Comparing `boomgate-0.0.1a1/pyproject.toml` & `boomgate-0.0.1a2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: Utilities",
 ]
 keywords = ["security", "dependency", "supply chain"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["ruff", "pre-commit", "mypy", "build", "hatch"]
+dev = ["ruff", "pre-commit", "mypy", "build", "hatch", "pytest", "pytest-cov"]
 docs = ["sphinx", "shibuya", "myst-parser"]
 
 [project.scripts]
 boomgate = "boomgate.cli:main"
 
 [project.urls]
 Homepage = "https://boomgate.readthedocs.io"
@@ -42,7 +42,11 @@
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["src/*", "LICENSE"]
 exclude = ["*.json", "pkg/_compat.py"]
+
+[tool.pytest.ini_options]
+minversion = "8.1.1"
+addopts = "--cov=src --cov-report html"
```

### Comparing `boomgate-0.0.1a1/PKG-INFO` & `boomgate-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: boomgate
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A software supply chain risk management tool
 Project-URL: Homepage, https://boomgate.readthedocs.io
 Project-URL: Documentation, https://boomgate.readthedocs.io
 Project-URL: Changelog, https://boomgate.readthedocs.io/en/latest/CHANGELOG.html
 Project-URL: Repository, https://github.com/KyeRussell/boomgate
 Project-URL: Issues, https://github.com/KyeRussell/boomgate/issues
 Author-email: Kye Russell <me@kye.id.au>
@@ -684,33 +684,33 @@
 Requires-Dist: rich
 Requires-Dist: typer
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: shibuya; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Description-Content-Type: text/markdown
 
 <h1 align="center">Boomgate</h1>
 <p align="center"><em>
     Identify and mitigate the risks of using third-party libraries.
 </em></p>
 
 <p align="center">
-    <a href="https://pypi.org/project/boomgate/">
-        <img src="https://img.shields.io/pypi/v/boomgate?color=%2334D058&label=PyPI%20package" alt="PyPI version">
-    </a>
-    <a href="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml">
-        <img src="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml/badge.svg" alt="Release workflow status">
-    </a>
+    <a href="https://pypi.org/project/boomgate/"><img src="https://img.shields.io/pypi/v/boomgate?color=%2334D058&label=PyPI%20package" alt="PyPI version"></a>
+    <a href="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml"><img src="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml/badge.svg" alt="Release workflow status"></a>
+    <a href="https://codecov.io/gh/KyeRussell/boomgate" ><img src="https://codecov.io/gh/KyeRussell/boomgate/graph/badge.svg?token=2XY75VWMGK"></a>
+    <a href="https://boomgate.readthedocs.io"><img src="https://readthedocs.org/projects/boomgate/badge/" alt="Documentation on Read The Docs"></a>
 </p>
 
 ---
 
 This project is not remotely ready for anyone to look at, let alone use. It is in a
 very early proof-of-concept stage, focusing on iterative research and development. I
 have not settled on the project's architecture, and I am still exploring the problem
@@ -744,7 +744,13 @@
 Clone the repository and run the following command:
 
 ```bash
 uv pip install -e . -r pyproject.toml --extra=dev --extra=docs
 ```
 
 This will install the project in editable mode with all development dependencies.
+
+### Running tests
+
+```bash
+pytest
+```
```

