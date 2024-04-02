# Comparing `tmp/dyff-client-0.2.0.tar.gz` & `tmp/dyff-client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-client-0.2.0.tar", last modified: Tue Mar  5 04:12:17 2024, max compression
+gzip compressed data, was "dyff-client-0.2.1.tar", last modified: Tue Apr  2 15:52:28 2024, max compression
```

## Comparing `dyff-client-0.2.0.tar` & `dyff-client-0.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.052041 dyff-client-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1666 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-05 04:12:11.000000 dyff-client-0.2.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-03-05 04:12:11.000000 dyff-client-0.2.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-03-05 04:12:11.000000 dyff-client-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-05 04:12:11.000000 dyff-client-0.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-03-05 04:12:17.052041 dyff-client-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-03-05 04:12:11.000000 dyff-client-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.038042 dyff-client-0.2.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.043042 dyff-client-0.2.0/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.045042 dyff-client-0.2.0/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.046042 dyff-client-0.2.0/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.047042 dyff-client-0.2.0/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   542099 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.048041 dyff-client-0.2.0/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   581216 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    60744 2024-03-05 04:12:11.000000 dyff-client-0.2.0/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.051041 dyff-client-0.2.0/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-03-05 04:12:17.000000 dyff-client-0.2.0/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-03-05 04:12:17.000000 dyff-client-0.2.0/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 04:12:17.000000 dyff-client-0.2.0/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-03-05 04:12:17.000000 dyff-client-0.2.0/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-05 04:12:17.000000 dyff-client-0.2.0/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-05 04:12:11.000000 dyff-client-0.2.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-03-05 04:12:11.000000 dyff-client-0.2.0/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-03-05 04:12:11.000000 dyff-client-0.2.0/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-03-05 04:12:11.000000 dyff-client-0.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.040042 dyff-client-0.2.0/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.050042 dyff-client-0.2.0/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.051041 dyff-client-0.2.0/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-03-05 04:12:11.000000 dyff-client-0.2.0/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 04:12:17.052041 dyff-client-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 04:12:17.051041 dyff-client-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-03-05 04:12:11.000000 dyff-client-0.2.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.130877 dyff-client-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-02 15:52:22.000000 dyff-client-0.2.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-02 15:52:22.000000 dyff-client-0.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-02 15:52:22.000000 dyff-client-0.2.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-02 15:52:28.130877 dyff-client-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-02 15:52:22.000000 dyff-client-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.116877 dyff-client-0.2.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.121877 dyff-client-0.2.1/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.123877 dyff-client-0.2.1/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.124877 dyff-client-0.2.1/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.125877 dyff-client-0.2.1/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   542099 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.127877 dyff-client-0.2.1/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   581216 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    60716 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.130877 dyff-client-0.2.1/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-02 15:52:22.000000 dyff-client-0.2.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-02 15:52:22.000000 dyff-client-0.2.1/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-02 15:52:22.000000 dyff-client-0.2.1/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-02 15:52:22.000000 dyff-client-0.2.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.118877 dyff-client-0.2.1/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.128877 dyff-client-0.2.1/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.129877 dyff-client-0.2.1/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 15:52:28.130877 dyff-client-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.129877 dyff-client-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-02 15:52:22.000000 dyff-client-0.2.1/tests/test_import.py
```

### Comparing `dyff-client-0.2.0/.gitlab-ci.yml` & `dyff-client-0.2.1/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,29 @@
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
     ref: 0.1.0
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
-    ref: 0.2.0
+    ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.7.2
+    ref: 0.9.1
     file:
       - python-autoflake.yml
       - python-black.yml
       - python-isort.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-pyroma.yml
       - python-pytest.yml
       - python-twine-upload.yml
+      - python-docformatter.yml
   - project: buildgarden/pipelines/skywalking-eyes
     ref: 0.2.0
     file:
       - license-eye-header-check.yml
 
 variables:
   PYTHON_PACKAGE: dyff/client
@@ -64,7 +65,11 @@
 
 python-twine-upload-pypi:
   extends: python-twine-upload
   variables:
     TWINE_USERNAME: __token__
     TWINE_PASSWORD: $PYPI_API_TOKEN
     TWINE_REPOSITORY_URL: https://upload.pypi.org/legacy/
+
+python-docformatter:
+  variables:
+    PYTHON_DOCFORMATTER_EXCLUDE: _generated
```

### Comparing `dyff-client-0.2.0/.licenserc.yaml` & `dyff-client-0.2.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/.pre-commit-config.yaml` & `dyff-client-0.2.1/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -9,51 +9,58 @@
         args: ["--maxkb=600"]
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: trailing-whitespace
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: "v2.3.0"
+    rev: "v2.3.1"
     hooks:
       - id: autoflake
         args:
           - "--in-place"
           - "--expand-star-imports"
           - "--remove-duplicate-keys"
           - "--remove-unused-variables"
           - "--remove-all-unused-imports"
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
 
+  - repo: https://github.com/PyCQA/docformatter
+    rev: v1.7.5
+    hooks:
+      - id: docformatter
+        additional_dependencies: [tomli]
+        args: ["--in-place", "--black", "--config", "./pyproject.toml"]
+
   - repo: https://gitlab.com/buildgarden/pipelines/skywalking-eyes
     rev: "0.2.0"
     hooks:
       - id: license-eye-header-fix
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
 
   - repo: https://gitlab.com/buildgarden/tools/badgie
-    rev: "0.11.0"
+    rev: "0.11.2"
     hooks:
       - id: badgie
 
   - repo: https://gitlab.com/buildgarden/tools/cici-tools
-    rev: "0.6.0"
+    rev: "0.7.0"
     hooks:
       - id: cici-update
 
   - repo: https://github.com/yelp/detect-secrets
     rev: v1.4.0
     hooks:
       - id: detect-secrets
```

### Comparing `dyff-client-0.2.0/.secrets.baseline` & `dyff-client-0.2.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/CODE_OF_CONDUCT.md` & `dyff-client-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/LICENSE` & `dyff-client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/PKG-INFO` & `dyff-client-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.0/README.md` & `dyff-client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/__init__.py` & `dyff-client-0.2.1/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/_client.py` & `dyff-client-0.2.1/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/_configuration.py` & `dyff-client-0.2.1/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/_patch.py` & `dyff-client-0.2.1/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/_serialization.py` & `dyff-client-0.2.1/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/_vendor.py` & `dyff-client-0.2.1/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/__init__.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/_client.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/_configuration.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/_patch.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/_vendor.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/operations/__init__.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/operations/_operations.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/aio/operations/_patch.py` & `dyff-client-0.2.1/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/operations/__init__.py` & `dyff-client-0.2.1/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/operations/_operations.py` & `dyff-client-0.2.1/dyff/client/_generated/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/_generated/operations/_patch.py` & `dyff-client-0.2.1/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/dyff/client/client.py` & `dyff-client-0.2.1/dyff/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,18 +116,17 @@
     elif x.id is not None:
         return x.id
     else:
         raise ValueError(".id attribute not set")
 
 
 def _encode_labels(labels: Optional[dict[str, str]]) -> Optional[str]:
-    """The Python client accepts 'annotations' and 'labels' as dicts, but
-    they need to be json-encoded so that they can be forwarded as part of
-    the HTTP query parameters.
-    """
+    """The Python client accepts 'annotations' and 'labels' as dicts, but they need to
+    be json-encoded so that they can be forwarded as part of the HTTP query
+    parameters."""
     if labels is None:
         return None
     # validate
     for k, v in labels.items():
         try:
             Label(key=k, value=v)
         except Exception as ex:
@@ -209,17 +208,17 @@
         self._client = httpx.Client(
             timeout=httpx.Timeout(5, read=None), verify=verify_ssl_certificates
         )
 
     def infer(self, body: Any) -> Any:
         """Make an inference request.
 
-        The input and output are arbitrary JSON objects. The required format
-        depends on the endpoint and input/output adapters specified when
-        creating the inference client.
+        The input and output are arbitrary JSON objects. The required format depends on
+        the endpoint and input/output adapters specified when creating the inference
+        client.
 
         :param Any body: A JSON object containing the inference input.
         :returns: A JSON object containing the inference output.
         """
         url = httpx.URL(
             f"{self._dyff_api_endpoint}/inferencesessions"
             f"/{self._session_id}/infer/{self._inference_endpoint}"
@@ -283,16 +282,16 @@
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Audit]:
-        """Get all Audits matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
+        """Get all Audits matching a query. The query is a set of equality constraints
+        specified as key-value pairs.
 
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
@@ -315,16 +314,16 @@
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
         ]
 
     def label(self, audit_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Audit with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Audit with key-value pairs (stored in the ``.labels``
+        field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param audit_id: The ID of the Audit to label.
@@ -463,16 +462,16 @@
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Dataset]:
-        """Get all Datasets matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
+        """Get all Datasets matching a query. The query is a set of equality constraints
+        specified as key-value pairs.
 
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
@@ -495,16 +494,16 @@
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
         ]
 
     def label(self, dataset_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Dataset with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Dataset with key-value pairs (stored in the ``.labels``
+        field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param dataset_id: The ID of the Dataset to label.
@@ -617,16 +616,16 @@
             name=name,
             artifacts=artifacts,
             schema=schema,
         )
         return self.create(request)
 
     def upload_arrow_dataset(self, dataset: Dataset, dataset_directory: str) -> None:
-        """Uploads the data files in an existing Arrow dataset for which a
-        Dataset resource has already been created.
+        """Uploads the data files in an existing Arrow dataset for which a Dataset
+        resource has already been created.
 
         Typical usage::
 
             dataset = client.datasets.create_arrow_dataset(dataset_directory, ...)
             client.datasets.upload_arrow_dataset(dataset, dataset_directory)
 
         :param dataset: The Dataset resource for the Arrow dataset.
@@ -743,16 +742,16 @@
                 inference_service_name=inferenceServiceName,
                 model=model,
                 model_name=modelName,
             )
         ]
 
     def label(self, evaluation_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Evaluation with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Evaluation with key-value pairs (stored in the
+        ``.labels`` field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param evaluation_id: The ID of the Evaluation to label.
@@ -855,16 +854,16 @@
                 name=name,
                 model=model,
                 model_name=modelName,
             )
         ]
 
     def label(self, service_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified InferenceService with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified InferenceService with key-value pairs (stored in the
+        ``.labels`` field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param service_id: The ID of the InferenceService to label.
@@ -981,16 +980,16 @@
                 inference_service_name=inferenceServiceName,
                 model=model,
                 model_name=modelName,
             )
         ]
 
     def label(self, session_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified InferenceSession with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified InferenceSession with key-value pairs (stored in the
+        ``.labels`` field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param session_id: The ID of the InferenceSession to label.
@@ -1027,16 +1026,16 @@
         token: str,
         *,
         interface: Optional[InferenceInterface] = None,
         endpoint: Optional[str] = None,
         input_adapter: Optional[Adapter] = None,
         output_adapter: Optional[Adapter] = None,
     ) -> InferenceSessionClient:
-        """Create an InferenceSessionClient that interacts with the given
-        inference session. The token should be one returned either from
+        """Create an InferenceSessionClient that interacts with the given inference
+        session. The token should be one returned either from
         ``Client.inferencesessions.create()`` or from
         ``Client.inferencesessions.token(session_id)``.
 
         The inference endpoint in the session must also be specified, either
         directly through the ``endpoint`` argument or by specifying an
         ``interface``. Specifying ``interface`` will also use the input and
         output adapters from the interface. You can also specify these
@@ -1167,16 +1166,16 @@
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Model]:
-        """Get all Models matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
+        """Get all Models matching a query. The query is a set of equality constraints
+        specified as key-value pairs.
 
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
@@ -1199,16 +1198,16 @@
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
         ]
 
     def label(self, model_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Model with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Model with key-value pairs (stored in the ``.labels``
+        field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param model_id: The ID of the Model to label.
@@ -1277,16 +1276,16 @@
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Module]:
-        """Get all Modules matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
+        """Get all Modules matching a query. The query is a set of equality constraints
+        specified as key-value pairs.
 
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
@@ -1309,16 +1308,16 @@
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
         ]
 
     def label(self, module_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Module with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Module with key-value pairs (stored in the ``.labels``
+        field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param module_id: The ID of the Module to label.
@@ -1342,16 +1341,15 @@
         :return: A full Module entity with .id and other properties set.
         """
         return Module.parse_obj(self._raw_ops.create(module_request.dict()))
 
     def create_package(
         self, package_directory: str, *, account: str, name: str
     ) -> Module:
-        """Create a Module resource describing a package structured as a
-        directory tree.
+        """Create a Module resource describing a package structured as a directory tree.
 
         Internally, constructs a ``ModuleCreateRequest`` using information
         obtained from the directory tree, then calls ``create()`` with the
         constructed request.
 
         Typical usage::
 
@@ -1392,16 +1390,16 @@
             account=account,
             name=name,
             artifacts=artifacts,
         )
         return self.create(request)
 
     def upload_package(self, module: Module, package_directory: str) -> None:
-        """Uploads the files in a package directory for which a Module resource
-        has already been created.
+        """Uploads the files in a package directory for which a Module resource has
+        already been created.
 
         Typical usage::
 
             module = client.modules.create_package(package_directory, ...)
             client.modules.upload_package(module, package_directory)
 
         :param module: The Module resource for the package.
@@ -1474,16 +1472,16 @@
         labels: Optional[dict[str, str]] = None,
         report: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inferenceService: Optional[str] = None,
         model: Optional[str] = None,
     ) -> list[Report]:
-        """Get all Reports matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
+        """Get all Reports matching a query. The query is a set of equality constraints
+        specified as key-value pairs.
 
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
@@ -1518,16 +1516,16 @@
                 evaluation=evaluation,
                 inference_service=inferenceService,
                 model=model,
             )
         ]
 
     def label(self, report_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Report with key-value pairs (stored in
-        the ``.labels`` field of the resource).
+        """Label the specified Report with key-value pairs (stored in the ``.labels``
+        field of the resource).
 
         Providing ``None`` for the value deletes the label.
 
         See :class:`~dyff.schema.platform.Label` for a description of the
         constraints on label keys and values.
 
         :param report_id: The ID of the Report to label.
@@ -1608,15 +1606,15 @@
             Defaults to the UL DSRI-hosted Dyff instance.
         :param bool verify_ssl_certificates: You can disable certificate
             verification for testing; you should do this only if you have
             also changed ``endpoint`` to point to a trusted local server.
         """
 
         if endpoint is None:
-            endpoint = "https://apis.alignmentlabs.ai/dyff/v0"
+            endpoint = "https://api.dyff.io/v0"
         credential = _APIKeyCredential(api_key=api_key)
         authentication_policy = BearerTokenCredentialPolicy(credential)
         self._raw = RawClient(
             endpoint=endpoint,
             credential=credential,
             authentication_policy=authentication_policy,
         )
```

### Comparing `dyff-client-0.2.0/dyff_client.egg-info/PKG-INFO` & `dyff-client-0.2.1/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.0/dyff_client.egg-info/SOURCES.txt` & `dyff-client-0.2.1/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/makefile` & `dyff-client-0.2.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/pyproject.toml` & `dyff-client-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff-client-0.2.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff-client-0.2.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/scripts/models/databricks--dolly-v2-3b.py` & `dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/scripts/models/tiiuae--falcon-7b.py` & `dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.0/tests/test_import.py` & `dyff-client-0.2.1/tests/test_import.py`

 * *Files identical despite different names*

