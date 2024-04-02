# Comparing `tmp/mojo_testplus-1.3.8.tar.gz` & `tmp/mojo_testplus-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_testplus-1.3.8.tar", max compression
+gzip compressed data, was "mojo_testplus-1.3.9.tar", max compression
```

## Comparing `mojo_testplus-1.3.8.tar` & `mojo_testplus-1.3.9.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:54:17.756237 mojo_testplus-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      295 2024-01-26 02:54:17.756358 mojo_testplus-1.3.8/README.rst
--rw-r--r--   0        0        0     1319 2024-02-20 01:47:54.196919 mojo_testplus-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      538 2024-01-26 02:54:17.757715 mojo_testplus-1.3.8/source/packages/mojo/factories/testplusfactory.py
--rw-r--r--   0        0        0     1786 2024-01-26 02:54:17.757817 mojo_testplus-1.3.8/source/packages/mojo/testplus/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:17.757894 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:17.757977 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      859 2024-01-26 02:54:17.758125 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
--rw-r--r--   0        0        0     3535 2024-01-26 02:54:17.758211 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
--rw-r--r--   0        0        0     6287 2024-01-26 02:54:17.758268 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
--rw-r--r--   0        0        0     5676 2024-01-26 02:54:17.758353 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
--rw-r--r--   0        0        0    14245 2024-02-20 01:47:34.716285 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
--rw-r--r--   0        0        0      591 2024-01-26 02:54:17.758565 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/utilities/__init__.py
--rw-r--r--   0        0        0      566 2024-01-26 02:54:17.758642 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/utilities/timestamp.py
--rw-r--r--   0        0        0     1555 2024-01-26 02:54:17.758723 mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/testplus_command.py
--rw-r--r--   0        0        0     1941 2024-01-26 02:54:17.758819 mojo_testplus-1.3.8/source/packages/mojo/testplus/constraints.py
--rw-r--r--   0        0        0      572 2024-01-26 02:54:17.758884 mojo_testplus-1.3.8/source/packages/mojo/testplus/diagnostics.py
--rw-r--r--   0        0        0     5127 2024-02-11 04:21:50.026593 mojo_testplus-1.3.8/source/packages/mojo/testplus/entrypoints.py
--rw-r--r--   0        0        0      714 2024-01-26 02:54:17.759050 mojo_testplus-1.3.8/source/packages/mojo/testplus/exceptions.py
--rw-r--r--   0        0        0     4370 2024-01-26 02:54:17.759125 mojo_testplus-1.3.8/source/packages/mojo/testplus/expressions.py
--rw-r--r--   0        0        0      446 2024-01-26 02:54:17.759189 mojo_testplus-1.3.8/source/packages/mojo/testplus/extensionprotocols.py
--rw-r--r--   0        0        0     2081 2024-02-19 04:16:55.786084 mojo_testplus-1.3.8/source/packages/mojo/testplus/initialize.py
--rw-r--r--   0        0        0     3144 2024-01-26 02:54:17.759354 mojo_testplus-1.3.8/source/packages/mojo/testplus/queries.py
--rw-r--r--   0        0        0     1359 2024-01-26 02:54:17.759437 mojo_testplus-1.3.8/source/packages/mojo/testplus/reflection.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:17.759494 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/__init__.py
--rw-r--r--   0        0        0     3232 2024-01-26 02:54:17.759694 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencermodulescope.py
--rw-r--r--   0        0        0     3392 2024-01-26 02:54:17.759756 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencerscopebase.py
--rw-r--r--   0        0        0     3011 2024-01-26 02:54:17.759827 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencersessionscope.py
--rw-r--r--   0        0        0     6546 2024-01-26 02:54:17.759902 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencertestscope.py
--rw-r--r--   0        0        0    31040 2024-02-16 01:13:16.187507 mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/testsequencer.py
--rwxr-xr-x   0        0        0      959 2024-01-26 02:54:17.760130 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/__init__.py
--rw-r--r--   0        0        0     2449 2024-01-26 02:54:17.760266 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/prism.css
--rw-r--r--   0        0        0    54704 2024-01-26 02:54:17.760551 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/prism.js
--rw-r--r--   0        0        0  1144941 2024-01-26 02:54:17.761501 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/test-report-banner-background-image.png
--rw-r--r--   0        0        0    15098 2024-01-26 02:54:17.761997 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/testsummary.css
--rw-r--r--   0        0        0    53851 2024-01-26 02:54:17.762193 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/testsummary.js
--rw-r--r--   0        0        0    23424 2024-01-26 02:54:17.762330 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/w3.css
--rw-r--r--   0        0        0     3190 2024-01-26 02:54:17.762597 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/tabs/tab-images.html
--rw-r--r--   0        0        0     3385 2024-01-26 02:54:17.762662 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/tabs/tab-sounds.html
--rwxr-xr-x   0        0        0     8630 2024-01-26 02:54:17.762744 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/testsummary.html
--rw-r--r--   0        0        0     2449 2024-01-26 02:54:17.762883 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/prism.css
--rw-r--r--   0        0        0    54704 2024-01-26 02:54:17.763143 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/prism.js
--rw-r--r--   0        0        0  1144941 2024-01-26 02:54:17.763904 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/test-report-banner-background-image.png
--rw-r--r--   0        0        0     4624 2024-01-26 02:54:17.763997 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testhelpers.js
--rw-r--r--   0        0        0    15098 2024-01-26 02:54:17.764076 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testsummary.css
--rw-r--r--   0        0        0    49988 2024-01-26 02:54:17.764172 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testsummary.js
--rw-r--r--   0        0        0    23424 2024-01-26 02:54:17.764300 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/w3.css
--rw-r--r--   0        0        0     3190 2024-01-26 02:54:17.764389 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/tabs/tab-images.html
--rw-r--r--   0        0        0     3385 2024-01-26 02:54:17.764444 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/tabs/tab-sounds.html
--rwxr-xr-x   0        0        0     8712 2024-01-26 02:54:17.764508 mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/testsummary.html
--rwxr-xr-x   0        0        0     9272 2024-01-26 02:54:17.764604 mojo_testplus-1.3.8/source/packages/mojo/testplus/testcollector.py
--rw-r--r--   0        0        0     1264 2024-01-26 02:54:17.764677 mojo_testplus-1.3.8/source/packages/mojo/testplus/testgroup.py
--rwxr-xr-x   0        0        0    20479 2024-01-26 02:54:17.764818 mojo_testplus-1.3.8/source/packages/mojo/testplus/testjob.py
--rwxr-xr-x   0        0        0     1874 2024-01-26 02:54:17.764912 mojo_testplus-1.3.8/source/packages/mojo/testplus/testref.py
--rwxr-xr-x   0        0        0     6046 2024-01-26 02:54:17.764998 mojo_testplus-1.3.8/source/packages/mojo/testplus/utilities.py
--rw-r--r--   0        0        0     9064 2024-01-26 02:54:17.765081 mojo_testplus-1.3.8/source/packages/mojo/testplus/validation.py
--rw-r--r--   0        0        0    19195 2024-01-26 02:54:17.765185 mojo_testplus-1.3.8/source/packages/mojo/testplus/verification.py
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 mojo_testplus-1.3.8/setup.py
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 mojo_testplus-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:54:17.756237 mojo_testplus-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      295 2024-01-26 02:54:17.756358 mojo_testplus-1.3.9/README.rst
+-rw-r--r--   0        0        0     1320 2024-02-21 22:53:52.222045 mojo_testplus-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      538 2024-01-26 02:54:17.757715 mojo_testplus-1.3.9/source/packages/mojo/factories/testplusfactory.py
+-rw-r--r--   0        0        0     2013 2024-02-21 21:48:41.096493 mojo_testplus-1.3.9/source/packages/mojo/testplus/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:17.757894 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:17.757977 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      859 2024-01-26 02:54:17.758125 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
+-rw-r--r--   0        0        0     3535 2024-01-26 02:54:17.758211 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
+-rw-r--r--   0        0        0     6287 2024-01-26 02:54:17.758268 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
+-rw-r--r--   0        0        0     5676 2024-01-26 02:54:17.758353 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
+-rw-r--r--   0        0        0    14245 2024-02-20 01:47:34.716285 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
+-rw-r--r--   0        0        0      591 2024-01-26 02:54:17.758565 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/utilities/__init__.py
+-rw-r--r--   0        0        0      566 2024-01-26 02:54:17.758642 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/utilities/timestamp.py
+-rw-r--r--   0        0        0     1555 2024-01-26 02:54:17.758723 mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/testplus_command.py
+-rw-r--r--   0        0        0      572 2024-01-26 02:54:17.758884 mojo_testplus-1.3.9/source/packages/mojo/testplus/diagnostics.py
+-rw-r--r--   0        0        0     5127 2024-02-11 04:21:50.026593 mojo_testplus-1.3.9/source/packages/mojo/testplus/entrypoints.py
+-rw-r--r--   0        0        0      714 2024-01-26 02:54:17.759050 mojo_testplus-1.3.9/source/packages/mojo/testplus/exceptions.py
+-rw-r--r--   0        0        0     4370 2024-01-26 02:54:17.759125 mojo_testplus-1.3.9/source/packages/mojo/testplus/expressions.py
+-rw-r--r--   0        0        0      717 2024-02-21 21:45:50.451696 mojo_testplus-1.3.9/source/packages/mojo/testplus/extensionprotocols.py
+-rw-r--r--   0        0        0     2352 2024-02-21 21:45:55.393145 mojo_testplus-1.3.9/source/packages/mojo/testplus/initialize.py
+-rw-r--r--   0        0        0     3144 2024-01-26 02:54:17.759354 mojo_testplus-1.3.9/source/packages/mojo/testplus/queries.py
+-rw-r--r--   0        0        0     1359 2024-01-26 02:54:17.759437 mojo_testplus-1.3.9/source/packages/mojo/testplus/reflection.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:17.759494 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/__init__.py
+-rw-r--r--   0        0        0     3232 2024-01-26 02:54:17.759694 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencermodulescope.py
+-rw-r--r--   0        0        0     3392 2024-01-26 02:54:17.759756 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencerscopebase.py
+-rw-r--r--   0        0        0     3011 2024-01-26 02:54:17.759827 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencersessionscope.py
+-rw-r--r--   0        0        0     6546 2024-01-26 02:54:17.759902 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencertestscope.py
+-rw-r--r--   0        0        0    31324 2024-02-21 22:12:49.621733 mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/testsequencer.py
+-rwxr-xr-x   0        0        0      959 2024-01-26 02:54:17.760130 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/__init__.py
+-rw-r--r--   0        0        0     2449 2024-01-26 02:54:17.760266 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/prism.css
+-rw-r--r--   0        0        0    54704 2024-01-26 02:54:17.760551 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/prism.js
+-rw-r--r--   0        0        0  1144941 2024-01-26 02:54:17.761501 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/test-report-banner-background-image.png
+-rw-r--r--   0        0        0    15098 2024-01-26 02:54:17.761997 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/testsummary.css
+-rw-r--r--   0        0        0    53851 2024-01-26 02:54:17.762193 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/testsummary.js
+-rw-r--r--   0        0        0    23424 2024-01-26 02:54:17.762330 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/w3.css
+-rw-r--r--   0        0        0     3190 2024-01-26 02:54:17.762597 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2024-01-26 02:54:17.762662 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     8630 2024-01-26 02:54:17.762744 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/testsummary.html
+-rw-r--r--   0        0        0     2449 2024-01-26 02:54:17.762883 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/prism.css
+-rw-r--r--   0        0        0    54704 2024-01-26 02:54:17.763143 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/prism.js
+-rw-r--r--   0        0        0  1144941 2024-01-26 02:54:17.763904 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/test-report-banner-background-image.png
+-rw-r--r--   0        0        0     4624 2024-01-26 02:54:17.763997 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testhelpers.js
+-rw-r--r--   0        0        0    15098 2024-01-26 02:54:17.764076 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testsummary.css
+-rw-r--r--   0        0        0    49988 2024-01-26 02:54:17.764172 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testsummary.js
+-rw-r--r--   0        0        0    23424 2024-01-26 02:54:17.764300 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/w3.css
+-rw-r--r--   0        0        0     3190 2024-01-26 02:54:17.764389 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2024-01-26 02:54:17.764444 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     8712 2024-01-26 02:54:17.764508 mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/testsummary.html
+-rwxr-xr-x   0        0        0     9272 2024-01-26 02:54:17.764604 mojo_testplus-1.3.9/source/packages/mojo/testplus/testcollector.py
+-rw-r--r--   0        0        0     1264 2024-01-26 02:54:17.764677 mojo_testplus-1.3.9/source/packages/mojo/testplus/testgroup.py
+-rwxr-xr-x   0        0        0    20407 2024-02-21 21:43:43.363110 mojo_testplus-1.3.9/source/packages/mojo/testplus/testjob.py
+-rwxr-xr-x   0        0        0     1780 2024-02-21 21:44:53.878269 mojo_testplus-1.3.9/source/packages/mojo/testplus/testref.py
+-rwxr-xr-x   0        0        0     6046 2024-01-26 02:54:17.764998 mojo_testplus-1.3.9/source/packages/mojo/testplus/utilities.py
+-rw-r--r--   0        0        0     9064 2024-01-26 02:54:17.765081 mojo_testplus-1.3.9/source/packages/mojo/testplus/validation.py
+-rw-r--r--   0        0        0    19195 2024-01-26 02:54:17.765185 mojo_testplus-1.3.9/source/packages/mojo/testplus/verification.py
+-rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 mojo_testplus-1.3.9/setup.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 mojo_testplus-1.3.9/PKG-INFO
```

### Comparing `mojo_testplus-1.3.8/LICENSE.txt` & `mojo_testplus-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/pyproject.toml` & `mojo_testplus-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-testplus"
 description = "Automation Mojo TestPlus Test Framework"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -25,15 +25,15 @@
 debugpy = "^1.6.5"
 click = "^8.1.3"
 requests = "<=2.31.0"
 mojo-errors = ">=1.3.1 <1.4.0"
 mojo-collections = ">=1.3.1 <1.4.0"
 mojo-config = ">=1.3.4 <1.4.0"
 mojo-extension = ">=1.3.7 <1.4.0"
-mojo-xmodules = ">=1.3.6 <1.4.0"
+mojo-xmodules = ">=1.3.12 <1.4.0"
 mojo-runtime = ">=1.3.4 <1.4.0"
 mojo-results = ">=1.3.1 <1.4.0"
 pymongo = {version = "^4.0.0", optional = true}
 couchdb = {version = "^1.2", optional = true}
 
 [tool.poetry.extras]
 mongodb = ["pymongo"]
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/factories/testplusfactory.py` & `mojo_testplus-1.3.9/source/packages/mojo/factories/testplusfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/__init__.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     mark_keywords,
     mark_priority,
     mark_descendent_categories,
     mark_descendent_keywords,
     mark_descendent_priority
 )
 
+from mojo.xmods.injection.constraints import (
+    Constraints,
+    FeatureConstraints
+)
+
+from mojo.xmods.injection.constraintscatalog import ConstraintsCatalog
+
 from mojo.xmods.injection.origination import (
     originate_parameter
 )
 
 from mojo.xmods.injection.decorators.factory import (
     integration,
     resource,
@@ -73,15 +80,18 @@
     mark_descendent_priority,
     originate_parameter,
     param,
     resource,
     scope,
     skip_test,
     validate,
-    validator
+    validator,
+    Constraints,
+    ConstraintsCatalog,
+    FeatureConstraints
 ]
 
 try:
     from mojo.results.model.taskingresult import verify_tasking_results
 
     __all__.append(verify_tasking_results)
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/query.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/query.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/testing/run.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/testing/run.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/utilities/__init__.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/cmdtree/utilities/timestamp.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/cmdtree/utilities/timestamp.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/cli/testplus_command.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/cli/testplus_command.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/diagnostics.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/diagnostics.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/entrypoints.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/entrypoints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/exceptions.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/expressions.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/expressions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/initialize.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/initialize.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+__version__ = "1.0.0"
+__maintainer__ = "Myron Walker"
+__email__ = "myron.walker@gmail.com"
+__status__ = "Development" # Prototype, Development or Production
+__license__ = "MIT"
 
 import os
 
 from mojo.collections.contextpaths import ContextPaths
 from mojo.collections.wellknown import ContextSingleton
 
 from mojo.xmods.xlogging.foundations import logging_initialize
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/queries.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/queries.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/reflection.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/reflection.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencermodulescope.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencermodulescope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencerscopebase.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencerscopebase.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencersessionscope.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencersessionscope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/sequencertestscope.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/sequencertestscope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/sequencing/testsequencer.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/sequencing/testsequencer.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,24 +51,28 @@
 from mojo.results.model.testcontainer import TestContainer
 from mojo.results.model.testresult import TestResult
 
 from mojo.results.recorders.resultrecorder import ResultRecorder
 
 from mojo.runtime.paths import get_path_for_output, get_path_for_diagnostics
 
-from mojo.testplus.constraints import Constraints
+from mojo.testplus import Constraints
 from mojo.testplus.diagnostics import DiagnosticLabel, RuntimeConfigPaths
 from mojo.testplus.testcollector import TestCollector
 from mojo.testplus.testgroup import TestGroup
 from mojo.testplus.testref import TestRef
 
 from mojo.testplus.sequencing.sequencersessionscope import SequencerSessionScope
 from mojo.testplus.sequencing.sequencermodulescope import SequencerModuleScope
 from mojo.testplus.sequencing.sequencertestscope import SequencerTestScope, SequencerTestSetupScope
 
+from mojo.testplus import ConstraintsCatalog
+
+constraints_catalog = ConstraintsCatalog()
+
 logger = logging.getLogger()
 
 
 CONSTRAINT_IMPORT_INSERTION_POINT = "# ------- INSERT CONSTRAINT IMPORTS HERE -------"
 
 FACTORY_IMPORT_INSERTION_POINT = "# ------- INSERT FACTORY IMPORTS HERE -------"
 
@@ -82,14 +86,18 @@
 
 __traceback_format_policy__ = "Brief"
 
 import logging
 
 logger = logging.getLogger()
 
+from mojo.testplus import ConstraintsCatalog
+
+constraints_catalog = ConstraintsCatalog()
+
 {}
 
 {}
 
 '''.format(CONSTRAINT_IMPORT_INSERTION_POINT, FACTORY_IMPORT_INSERTION_POINT)
 
 
@@ -628,21 +636,20 @@
             factory_imports.add('from {} import {}'.format(porigin.source_module_name, porigin.source_function.__name__))
 
         # Create the variables with session scope
         for pname, porigin in resource_scope.parameter_originations.items():
 
             sp_parameter_names = [pn for pn in porigin.source_signature.parameters.keys()]
             if 'constraints' in sp_parameter_names:
-                constraints = {}
-                if porigin.constraints is not None:
-                    constraints = porigin.constraints
-                    if issubclass(type(constraints), Constraints):
-                        constraint_imports.add(constraints.get_import_statement())
-                method_lines.append('{}constraints={}'.format(current_indent, repr(constraints)))
-            
+                constraints_key = porigin.constraints_key
+                if constraints_key is not None:
+                    if constraints_catalog.lookup_constraints(constraints_key) is None:
+                        raise RuntimeError(f"Constraint required but not found for contraints_key={constraints_key}")
+                    method_lines.append('{}constraints=constraints_catalog.lookup_constraints({})'.format(current_indent, repr(constraints_key)))
+
             source_func_call = porigin.generate_call()
             method_lines.append('{}for {} in {}:'.format(current_indent, pname, source_func_call))
             child_call_args.append(pname)
             current_indent = current_indent + indent_space
 
         child_name_list = [cnk for cnk in scope_node.children.keys()]
         child_name_list.sort()
@@ -703,20 +710,19 @@
                     # Generate any local parameters
                     for param_name, param_obj in test_local_args:
                         ffuncname = param_obj.source_function_name
                         ffuncsig = param_obj.source_signature
                         ffuncargs = [pn for pn in ffuncsig.parameters]
 
                         if 'constraints' in ffuncargs:
-                            constraints = {}
-                            if param_obj.constraints is not None:
-                                constraints = param_obj.constraints
-                                if issubclass(type(constraints), Constraints):
-                                    constraint_imports.add(constraints.get_import_statement())
-                            method_lines.append('{}constraints={}'.format(current_indent, repr(constraints)))
+                            constraints_key = param_obj.constraints_key
+                            if constraints_key is not None:
+                                if constraints_catalog.lookup_constraints(constraints_key) is None:
+                                    raise RuntimeError(f"Constraint required but not found for contraints_key={constraints_key}")
+                                method_lines.append('{}constraints=constraints_catalog.lookup_constraints({})'.format(current_indent, repr(constraints_key)))
 
                         ffuncargs_str = " ,".join(ffuncargs)
                         method_lines.append("{}for {} in {}({}):".format(current_indent, param_name, ffuncname, ffuncargs_str))
                         notables_map_names.append(param_name)
                         current_indent += indent_space
                 
                     notables_map = ", ".join(map(lambda arg: "'{}': {}".format(arg, arg), notables_map_names))
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/__init__.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/prism.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/prism.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/prism.js` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/prism.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/test-report-banner-background-image.png` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/test-report-banner-background-image.png`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/testsummary.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/testsummary.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/testsummary.js` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/testsummary.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/static/w3.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/static/w3.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/tabs/tab-images.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/tabs/tab-images.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/tabs/tab-sounds.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/tabs/tab-sounds.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v0/testsummary.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v0/testsummary.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/prism.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/prism.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/prism.js` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/prism.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/test-report-banner-background-image.png` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/test-report-banner-background-image.png`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testhelpers.js` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testhelpers.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testsummary.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testsummary.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/testsummary.js` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/testsummary.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/static/w3.css` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/static/w3.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/tabs/tab-images.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/tabs/tab-images.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/tabs/tab-sounds.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/tabs/tab-sounds.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/templates/v1/testsummary.html` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/templates/v1/testsummary.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/testcollector.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/testcollector.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/testgroup.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/testgroup.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/testjob.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/testjob.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import List, Optional
 
-import collections
-import json
 import os
-import sys
 import traceback
 
 from mojo.collections.contextuser import ContextUser
 from mojo.collections.contextpaths import ContextPaths
 
 from mojo.xmods.xformatting import CommandOutputFormat
 from mojo.xmods.xdebugger import WELLKNOWN_BREAKPOINTS, debugger_wellknown_breakpoint_entry
 
 from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 from mojo.runtime.paths import (
     get_summary_html_template_source,
     get_summary_static_resource_dest_dir,
     get_summary_static_resource_src_dir,
-    get_path_for_diagnostics,
     get_path_for_output
 )
 
 from mojo.results.model.buildinfo import BuildInfo
 from mojo.results.model.forwardinginfo import ForwardingInfo
 from mojo.results.model.jobinfo import JobInfo
 from mojo.results.model.pipelineinfo import PipelineInfo
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/testref.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/testref.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,20 @@
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
-from typing import Any, Dict, List, OrderedDict, Optional, Sequence
+from typing import Any, List, OrderedDict
 
 from types import FunctionType
 
 import collections
-import inspect
-import sys
 
-from mojo.xmods.markers import MetaFilter
 from mojo.xmods.injection.injectableref import InjectableRef
 
 class TestRef(InjectableRef):
     """
         The :class:`TestRef` objects are used to refer to a reference to a test.  We use :class:`TestRef` instances
         to reference the tests that are going to be run so we can control the lifespan of test case instances
         and control our memory consumption during test runs with large collections of test cases.
```

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/utilities.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/validation.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/validation.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/source/packages/mojo/testplus/verification.py` & `mojo_testplus-1.3.9/source/packages/mojo/testplus/verification.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-1.3.8/setup.py` & `mojo_testplus-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,27 @@
  'debugpy>=1.6.5,<2.0.0',
  'mojo-collections>=1.3.1,<1.4.0',
  'mojo-config>=1.3.4,<1.4.0',
  'mojo-errors>=1.3.1,<1.4.0',
  'mojo-extension>=1.3.7,<1.4.0',
  'mojo-results>=1.3.1,<1.4.0',
  'mojo-runtime>=1.3.4,<1.4.0',
- 'mojo-xmodules>=1.3.6,<1.4.0',
+ 'mojo-xmodules>=1.3.12,<1.4.0',
  'requests<=2.31.0']
 
 extras_require = \
 {'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo>=4.0.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['testplus = '
                      'mojo.testplus.cli.testplus_command:testplus_root_command']}
 
 setup_kwargs = {
     'name': 'mojo-testplus',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo TestPlus Test Framework',
     'long_description': '\n==========================\nAutomation Mojo - Testplus\n==========================\n \nThis is preliminary release of the \'testplus\' automation framework in a separate package from\nthe AutomationKit.  This release is not ready for public consumption because it is under "very active" development.\n\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_testplus-1.3.8/PKG-INFO` & `mojo_testplus-1.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-testplus
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo TestPlus Test Framework
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -24,15 +24,15 @@
 Requires-Dist: debugpy (>=1.6.5,<2.0.0)
 Requires-Dist: mojo-collections (>=1.3.1,<1.4.0)
 Requires-Dist: mojo-config (>=1.3.4,<1.4.0)
 Requires-Dist: mojo-errors (>=1.3.1,<1.4.0)
 Requires-Dist: mojo-extension (>=1.3.7,<1.4.0)
 Requires-Dist: mojo-results (>=1.3.1,<1.4.0)
 Requires-Dist: mojo-runtime (>=1.3.4,<1.4.0)
-Requires-Dist: mojo-xmodules (>=1.3.6,<1.4.0)
+Requires-Dist: mojo-xmodules (>=1.3.12,<1.4.0)
 Requires-Dist: pymongo (>=4.0.0,<5.0.0) ; extra == "mongodb"
 Requires-Dist: requests (<=2.31.0)
 Project-URL: Repository, https://github.com/automationmojo/testplus
 Description-Content-Type: text/x-rst
 
 
 ==========================
```

