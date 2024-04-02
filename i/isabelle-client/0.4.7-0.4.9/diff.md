# Comparing `tmp/isabelle_client-0.4.7.tar.gz` & `tmp/isabelle_client-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isabelle_client-0.4.7.tar", max compression
+gzip compressed data, was "isabelle_client-0.4.9.tar", max compression
```

## Comparing `isabelle_client-0.4.7.tar` & `isabelle_client-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11358 2024-02-01 20:19:04.875927 isabelle_client-0.4.7/LICENSE
--rw-r--r--   0        0        0     4774 2024-02-01 20:19:04.875927 isabelle_client-0.4.7/README.rst
--rw-r--r--   0        0        0      897 2024-02-01 20:44:46.521564 isabelle_client-0.4.7/isabelle_client/__init__.py
--rw-r--r--   0        0        0     1862 2024-02-01 20:44:46.521564 isabelle_client-0.4.7/isabelle_client/conftest.py
--rw-r--r--   0        0        0    12419 2024-02-01 20:44:46.521564 isabelle_client-0.4.7/isabelle_client/isabelle__client.py
--rw-r--r--   0        0        0     4895 2024-02-01 20:44:46.521564 isabelle_client-0.4.7/isabelle_client/isabelle_connector.py
--rw-r--r--   0        0        0        0 2024-02-01 20:19:04.927926 isabelle_client-0.4.7/isabelle_client/py.typed
--rw-r--r--   0        0        0      295 2024-02-01 20:19:04.927926 isabelle_client-0.4.7/isabelle_client/resources/Cygwin-Isabelle.bat
--rw-r--r--   0        0        0     1247 2024-02-01 20:19:04.927926 isabelle_client-0.4.7/isabelle_client/resources/example.txt
--rwxr-xr-x   0        0        0       79 2024-02-01 20:19:04.927926 isabelle_client-0.4.7/isabelle_client/resources/isabelle
--rw-r--r--   0        0        0        4 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/cancel
--rw-r--r--   0        0        0      123 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/help
--rw-r--r--   0        0        0       90 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/purge_theories
--rw-r--r--   0        0        0      864 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/session_build
--rw-r--r--   0        0        0      337 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/session_start
--rw-r--r--   0        0        0      135 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/session_stop
--rw-r--r--   0        0        0        4 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/shutdown
--rw-r--r--   0        0        0       30 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/unknown
--rw-r--r--   0        0        0      699 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories
--rw-r--r--   0        0        0     1040 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories.Fail
--rw-r--r--   0        0        0     2909 2024-02-01 20:19:04.931926 isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories.Sledgehammer
--rw-r--r--   0        0        0     2542 2024-02-01 20:44:46.521564 isabelle_client-0.4.7/isabelle_client/sledgehammer_connector.py
--rw-r--r--   0        0        0     5443 2024-02-01 20:44:46.525564 isabelle_client-0.4.7/isabelle_client/socket_communication.py
--rw-r--r--   0        0        0     7467 2024-02-01 20:44:46.525564 isabelle_client-0.4.7/isabelle_client/utils.py
--rw-r--r--   0        0        0     3586 2024-02-01 20:44:46.525564 isabelle_client-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     5965 1970-01-01 00:00:00.000000 isabelle_client-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-02-01 20:19:04.875927 isabelle_client-0.4.9/LICENSE
+-rw-r--r--   0        0        0     4774 2024-02-01 20:19:04.875927 isabelle_client-0.4.9/README.rst
+-rw-r--r--   0        0        0      897 2024-04-02 18:51:36.275076 isabelle_client-0.4.9/isabelle_client/__init__.py
+-rw-r--r--   0        0        0     1862 2024-02-01 20:44:46.521564 isabelle_client-0.4.9/isabelle_client/conftest.py
+-rw-r--r--   0        0        0    12419 2024-02-01 20:44:46.521564 isabelle_client-0.4.9/isabelle_client/isabelle__client.py
+-rw-r--r--   0        0        0     4895 2024-02-01 20:44:46.521564 isabelle_client-0.4.9/isabelle_client/isabelle_connector.py
+-rw-r--r--   0        0        0        0 2024-02-01 20:19:04.927926 isabelle_client-0.4.9/isabelle_client/py.typed
+-rw-r--r--   0        0        0      295 2024-02-01 20:19:04.927926 isabelle_client-0.4.9/isabelle_client/resources/Cygwin-Isabelle.bat
+-rw-r--r--   0        0        0     1247 2024-02-01 20:19:04.927926 isabelle_client-0.4.9/isabelle_client/resources/example.txt
+-rwxr-xr-x   0        0        0       79 2024-02-01 20:19:04.927926 isabelle_client-0.4.9/isabelle_client/resources/isabelle
+-rw-r--r--   0        0        0        4 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/cancel
+-rw-r--r--   0        0        0      123 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/help
+-rw-r--r--   0        0        0       90 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/purge_theories
+-rw-r--r--   0        0        0      864 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/session_build
+-rw-r--r--   0        0        0      337 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/session_start
+-rw-r--r--   0        0        0      135 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/session_stop
+-rw-r--r--   0        0        0        4 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/shutdown
+-rw-r--r--   0        0        0       30 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/unknown
+-rw-r--r--   0        0        0      699 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories
+-rw-r--r--   0        0        0     1040 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories.Fail
+-rw-r--r--   0        0        0     2909 2024-02-01 20:19:04.931926 isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories.Sledgehammer
+-rw-r--r--   0        0        0     2542 2024-02-01 20:44:46.521564 isabelle_client-0.4.9/isabelle_client/sledgehammer_connector.py
+-rw-r--r--   0        0        0     5443 2024-02-01 20:44:46.525564 isabelle_client-0.4.9/isabelle_client/socket_communication.py
+-rw-r--r--   0        0        0     7467 2024-02-01 20:44:46.525564 isabelle_client-0.4.9/isabelle_client/utils.py
+-rw-r--r--   0        0        0     3586 2024-04-02 18:51:36.279076 isabelle_client-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5965 1970-01-01 00:00:00.000000 isabelle_client-0.4.9/PKG-INFO
```

### Comparing `isabelle_client-0.4.7/LICENSE` & `isabelle_client-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/README.rst` & `isabelle_client-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/__init__.py` & `isabelle_client-0.4.9/isabelle_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 # noqa: D205
 """A Python client to `Isabelle <https://isabelle.in.tum.de>`__ server."""
 from isabelle_client.isabelle__client import IsabelleClient
 from isabelle_client.socket_communication import IsabelleResponse
 from isabelle_client.utils import get_isabelle_client, start_isabelle_server
 
-__version__ = "0.4.7"
+__version__ = "0.4.9"
```

### Comparing `isabelle_client-0.4.7/isabelle_client/conftest.py` & `isabelle_client-0.4.9/isabelle_client/conftest.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/isabelle__client.py` & `isabelle_client-0.4.9/isabelle_client/isabelle__client.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/isabelle_connector.py` & `isabelle_client-0.4.9/isabelle_client/isabelle_connector.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/resources/example.txt` & `isabelle_client-0.4.9/isabelle_client/resources/example.txt`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/session_build` & `isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/session_build`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories` & `isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories.Fail` & `isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories.Fail`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/resources/isabelle-responses/use_theories.Sledgehammer` & `isabelle_client-0.4.9/isabelle_client/resources/isabelle-responses/use_theories.Sledgehammer`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/sledgehammer_connector.py` & `isabelle_client-0.4.9/isabelle_client/sledgehammer_connector.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/socket_communication.py` & `isabelle_client-0.4.9/isabelle_client/socket_communication.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/isabelle_client/utils.py` & `isabelle_client-0.4.9/isabelle_client/utils.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.7/pyproject.toml` & `isabelle_client-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isabelle-client"
-version = "0.4.7"
+version = "0.4.9"
 description = "A client to Isabelle proof assistant server"
 authors = ["Boris Shminke <boris@shminke.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/isabelle-client"
 readme = "README.rst"
 classifiers=[
 	"Programming Language :: Python :: 3.12",
@@ -137,15 +137,15 @@
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/isabelle-client/"
 
 [tool.tbump.version]
-current = "0.4.7"
+current = "0.4.9"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `isabelle_client-0.4.7/PKG-INFO` & `isabelle_client-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isabelle-client
-Version: 0.4.7
+Version: 0.4.9
 Summary: A client to Isabelle proof assistant server
 Home-page: https://github.com/inpefess/isabelle-client
 License: Apache-2.0
 Keywords: TCP client,Isabelle proof assistant,interactive theorem prover
 Author: Boris Shminke
 Author-email: boris@shminke.com
 Requires-Python: >=3.8.1,<3.13
```

