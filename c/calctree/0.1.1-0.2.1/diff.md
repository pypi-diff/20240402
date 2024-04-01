# Comparing `tmp/calctree-0.1.1.tar.gz` & `tmp/calctree-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calctree-0.1.1.tar", max compression
+gzip compressed data, was "calctree-0.2.1.tar", max compression
```

## Comparing `calctree-0.1.1.tar` & `calctree-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-01-25 06:17:32.518074 calctree-0.1.1/LICENSE
--rw-r--r--   0        0        0      953 2024-02-08 04:34:01.045610 calctree-0.1.1/README.md
--rw-r--r--   0        0        0      376 2024-02-14 06:43:21.426182 calctree-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-08 04:34:01.046790 calctree-0.1.1/src/calctree/__init__.py
--rw-r--r--   0        0        0     2885 2024-02-08 04:34:01.047367 calctree-0.1.1/src/calctree/client.py
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 calctree-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-25 06:17:32.518074 calctree-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1373 2024-03-28 05:21:21.983559 calctree-0.2.1/README.md
+-rw-r--r--   0        0        0      376 2024-03-28 05:14:01.768883 calctree-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-08 04:34:01.046790 calctree-0.2.1/src/calctree/__init__.py
+-rw-r--r--   0        0        0     1724 2024-03-28 05:14:01.769466 calctree-0.2.1/src/calctree/calculation_result.py
+-rw-r--r--   0        0        0     2545 2024-03-28 05:14:01.770148 calctree-0.2.1/src/calctree/client.py
+-rw-r--r--   0        0        0       54 2024-03-28 05:14:01.772124 calctree-0.2.1/src/calctree/exceptions.py
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 calctree-0.2.1/PKG-INFO
```

### Comparing `calctree-0.1.1/LICENSE` & `calctree-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calctree-0.1.1/README.md` & `calctree-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,26 +4,39 @@
 The CalcTree Python Client is a Python library that provides a convenient interface for interacting with the CalcTree API. It allows you to perform calculations using CalcTree's powerful calculation engine.
 
 ## Installation
 
 You can install the CalcTree Python Client using pip:
 
 ```bash
-pip install calctree-python-client
+pip install calctree
 ```
 
 # Getting Started
 To use the CalcTree Python Client, you need to obtain an API key from CalcTree. Once you have your API key, you can initialize the client and start running calculations.
 
+Remember to replace YOUR_API_KEY with your actual API key, YOUR_PAGE_ID with the ID of the page you want to run calculations on, and YOUR_PARAM_NAME with the name of the parameter you want to set the value for.
+
 ```python
 import json
 
 from calctree.client import CalcTreeClient
 
 client = CalcTreeClient('YOUR_API_KEY')
 
-res = client.run_calculation("6fd16232-39e3-44a9-aee2-d6ad375698b0",
-                             [{"name": "cylinder_radius", "formula": "1000"}]
+res = client.run_calculation("YOUR_PAGE_ID",
+                             [{"name": "YOUR_PARAM_NAME", "formula": "1000"}]
                              )
-print(res)
+
+print("Result as a dictionary:")
+print(result.to_dict())
+
+print("Value of param 'cylinder_radius':")
+print(result.get_param_value("cylinder_radius"))
+
+print("List of params:")
+print(result.get_params())
+
+print("List of values:")
+print(result.get_values())
 ```
```

### Comparing `calctree-0.1.1/src/calctree/client.py` & `calctree-0.2.1/src/calctree/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from urllib import request
 
+from src.calctree.calculation_result import CalculationResult
+
 
 class CalcTreeClient:
     """Client for interacting with the CalcTree API.
 
     This client allows you to perform calculations using the CalcTree API.
 
     Args:
@@ -15,36 +17,29 @@
     """
 
     def __init__(self, api_key: str):
         self._api_key = api_key
         self._calctree_host = 'https://api.calctree.com'
         self._run_calculation_endpoint = '/api/calctree-cell/run-calculation'
 
-    def run_calculation(self, page_id: str, ct_cells, host: str = 'https://api.calctree.com'):
+    def run_calculation(self, page_id: str, ct_cells, host: str = 'https://api.calctree.com') -> CalculationResult:
         """Run a calculation using the CalcTree API.
 
         Args:
             page_id (str): The ID of the page containing the calculation.
             ct_cells (List[Parameters]): A list of Parameters instances representing the calculation parameters.
                 Each Parameters instance has the following attributes:
                     name (str): The parameter name, the same as on the page.
                     formula (str): The value associated with the parameter.
 
         Returns:
-            List[Attributes]: A list of Attributes instances representing the calculation result.
-                Each Attributes instance has the following attributes:
-                    name (str): The parameter name.
-                    value (str): The value associated with the parameter.
+            CalculationResult: The result of the calculation.
         """  # noqa
         calculation_request_response = self._request_calculation(ct_cells, page_id)
-        return self._process_response(calculation_request_response)
-
-    def _process_response(self, response):
-        calculation_result = json.loads(response)
-        return [{'name': j['title'], 'value': str(j['value'])} for j in calculation_result]
+        return CalculationResult(calculation_request_response)
 
     def _request_calculation(self, ct_cells, page_id: str):
         url = f'{self._calctree_host}{self._run_calculation_endpoint}'
         headers = self._prepare_headers()
         body = self._prepare_body(ct_cells, page_id)
 
         payload = json.dumps(body).encode('utf-8')
```

