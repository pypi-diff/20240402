# Comparing `tmp/saphira-0.0.1.tar.gz` & `tmp/saphira-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.1.tar", last modified: Fri Dec 22 05:35:27 2023, max compression
+gzip compressed data, was "saphira-0.0.2.tar", last modified: Mon Apr  1 23:41:15 2024, max compression
```

## Comparing `saphira-0.0.1.tar` & `saphira-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2023-12-22 05:35:27.954043 saphira-0.0.1/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.1/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1980 2023-12-22 05:35:27.953200 saphira-0.0.1/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.1/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      704 2023-12-22 02:09:37.000000 saphira-0.0.1/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2023-12-22 05:35:27.954138 saphira-0.0.1/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2023-12-22 05:35:27.943918 saphira-0.0.1/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2023-12-22 05:35:27.947027 saphira-0.0.1/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       21 2023-12-19 02:43:04.000000 saphira-0.0.1/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1970 2023-12-22 05:25:19.000000 saphira-0.0.1/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2023-12-22 05:35:27.951252 saphira-0.0.1/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1980 2023-12-22 05:35:27.000000 saphira-0.0.1/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      279 2023-12-22 05:35:27.000000 saphira-0.0.1/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2023-12-22 05:35:27.000000 saphira-0.0.1/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       44 2023-12-22 05:35:27.000000 saphira-0.0.1/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2023-12-22 05:35:27.000000 saphira-0.0.1/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2023-12-22 05:35:27.950132 saphira-0.0.1/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.1/tests/test_jama_server.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.736207 saphira-0.0.2/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.2/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:41:15.735187 saphira-0.0.2/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.2/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-01 23:39:54.000000 saphira-0.0.2/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-01 23:41:15.736683 saphira-0.0.2/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.699806 saphira-0.0.2/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.709811 saphira-0.0.2/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-01 23:39:46.000000 saphira-0.0.2/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2087 2024-01-22 05:10:51.000000 saphira-0.0.2/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.733828 saphira-0.0.2/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.725960 saphira-0.0.2/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1712 2024-03-12 21:02:28.000000 saphira-0.0.2/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.2/tests/test_jama_server.py
```

### Comparing `saphira-0.0.1/LICENSE` & `saphira-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.1/PKG-INFO` & `saphira-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.1
+Version: 0.0.2
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,22 +20,23 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://saphira.ai
+Project-URL: Homepage, https://www.saphira.ai
 Keywords: saphira,parameter,hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `saphira-0.0.1/pyproject.toml` & `saphira-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.1"
+version = "0.0.2"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["saphira", "parameter", "hardware"]
-dependencies = []
+dependencies = ["requests"]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://saphira.ai"
+Homepage = "https://www.saphira.ai"
```

### Comparing `saphira-0.0.1/src/saphira/saphira.py` & `saphira-0.0.2/src/saphira/saphira.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 SAPHIRA_URL = os.getenv('SAPHIRA_URL', 'https://saphira.oavatare1.repl.co')
 
 # TODO: Integrate this into Matlab
 # This registers as a daemon that will re-run the parent program
 # TODO: Move daemon registration to service
 def get_param(datasource: str, name: str, skip_threading=False, local_runtime=False) -> Any:
-    # TODO: Use datasource to route to appropriate multi-tenant
+    # TODO: Call select_project first before selecting datasource 
+    # TODO: Use datasource to route to appropriate multi-tenant (project)
     # Post to service
     url = f'{SAPHIRA_URL}/check_key_and_get_value'
     req = {
         'check_key': name,
         # TODO: Include program name to allow automatic execution
         # 'consumingApplication': inspect.stack()[1].filename
     }
@@ -37,14 +38,14 @@
                     if get_param(datasource, name, skip_threading=True) != result:
                         subprocess.call(['python', consuming_application])
                     sleep(1)
             t = multiprocessing.Process(target=loop)
             t.start()
         else:
             # TODO: Perform proper dependency tracing to also upload any other linked files
-            upload_url = f'{SAPHIRA_URL}/upload'
+            upload_url = f'{SAPHIRA_URL}/upload?project={datasource}&requirement={name}'
             stack = inspect.stack()
             files = {f'file{i}': open(stack[1 + i].filename, 'rb') for i in range(len(stack) - 1)}
             upload_resp = requests.post(upload_url, files=files)
             print(f"{upload_url} responded with status code {upload_resp.status_code}")
 
     return result
```

### Comparing `saphira-0.0.1/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.2/src/saphira.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.1
+Version: 0.0.2
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,22 +20,23 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://saphira.ai
+Project-URL: Homepage, https://www.saphira.ai
 Keywords: saphira,parameter,hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `saphira-0.0.1/tests/test_jama_server.py` & `saphira-0.0.2/tests/test_jama_server.py`

 * *Files identical despite different names*

