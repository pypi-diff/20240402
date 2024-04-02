# Comparing `tmp/jaraco.xonsh-0.4.1.tar.gz` & `tmp/jaraco.xonsh-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.xonsh-0.4.1.tar", last modified: Sun Mar 24 16:35:41 2024, max compression
+gzip compressed data, was "jaraco.xonsh-0.5.0.tar", last modified: Tue Apr  2 14:38:12 2024, max compression
```

## Comparing `jaraco.xonsh-0.4.1.tar` & `jaraco.xonsh-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.727307 jaraco.xonsh-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.723307 jaraco.xonsh-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.723307 jaraco.xonsh-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-24 16:35:41.727307 jaraco.xonsh-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.723307 jaraco.xonsh-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.723307 jaraco.xonsh-0.4.1/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/jaraco/xonsh.xsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:35:41.723307 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-24 16:35:41.000000 jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-24 16:35:41.727307 jaraco.xonsh-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-24 16:35:24.000000 jaraco.xonsh-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/jaraco/xonsh.xsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/tox.ini
```

### Comparing `jaraco.xonsh-0.4.1/.github/workflows/main.yml` & `jaraco.xonsh-0.5.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,26 @@
 
 jobs:
   test:
     strategy:
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         # disable PyPy as it breaks CI
         # - python: pypy3.10
         #  platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
       - uses: actions/checkout@v4
```

### Comparing `jaraco.xonsh-0.4.1/LICENSE` & `jaraco.xonsh-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.4.1/NEWS.rst` & `jaraco.xonsh-0.5.0/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.5.0
+======
+
+Features
+--------
+
+- Use another command to get the whole message.
+
+
 v0.4.1
 ======
 
 Bugfixes
 --------
 
 - Slack implements 2FA on a per-workspace arrangement (yuck!).
```

### Comparing `jaraco.xonsh-0.4.1/PKG-INFO` & `jaraco.xonsh-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.4.1
+Version: 0.5.0
 Summary: Xonsh facilities used by jaraco
 Home-page: https://github.com/jaraco/jaraco.xonsh
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: jaraco.clipboard
 Requires-Dist: keyring
 Requires-Dist: xontrib-vox
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
```

### Comparing `jaraco.xonsh-0.4.1/README.rst` & `jaraco.xonsh-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.4.1/docs/conf.py` & `jaraco.xonsh-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.4.1/jaraco/xonsh.xsh` & `jaraco.xonsh-0.5.0/jaraco/xonsh.xsh`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
 	"""
 	Reflect the recent commit message in a news fragment.
 	"""
 	try:
 		type, = args
 	except ValueError:
 		type = 'feature'
-	msg = $(git log -1 --oneline --format=%s)
+	msg = $(git log -1 --pretty=format:%B)
 	(descr, *rest) = msg.splitlines()
 	try:
 		number = re.search(r'#(\d+)', msg).group(1)
 	except AttributeError:
 		number = '+'
 	towncrier create -c @(descr.strip().rstrip('.') + '.') @(number).@(type).rst
 	git add newsfragments
```

### Comparing `jaraco.xonsh-0.4.1/jaraco.xonsh.egg-info/PKG-INFO` & `jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.4.1
+Version: 0.5.0
 Summary: Xonsh facilities used by jaraco
 Home-page: https://github.com/jaraco/jaraco.xonsh
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: jaraco.clipboard
 Requires-Dist: keyring
 Requires-Dist: xontrib-vox
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
```

### Comparing `jaraco.xonsh-0.4.1/setup.cfg` & `jaraco.xonsh-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 install_requires = 
 	jaraco.clipboard
 	keyring
 	xontrib-vox
 
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
 	pytest-mypy
 	pytest-enabler >= 2.2
 	pytest-ruff >= 0.2.1
 docs = 
 	sphinx >= 3.5
```

### Comparing `jaraco.xonsh-0.4.1/tox.ini` & `jaraco.xonsh-0.5.0/tox.ini`

 * *Files identical despite different names*

