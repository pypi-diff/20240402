# Comparing `tmp/stellate_strawberry-1.0.0.tar.gz` & `tmp/stellate_strawberry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellate_strawberry-1.0.0.tar", max compression
+gzip compressed data, was "stellate_strawberry-1.1.0.tar", max compression
```

## Comparing `stellate_strawberry-1.0.0.tar` & `stellate_strawberry-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1576 2024-03-26 17:09:51.573223 stellate_strawberry-1.0.0/README.md
--rw-r--r--   0        0        0      342 2024-03-28 13:15:06.079833 stellate_strawberry-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3991 2024-03-26 17:13:35.060662 stellate_strawberry-1.0.0/stellate_strawberry/__init__.py
--rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 stellate_strawberry-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1580 2024-04-02 08:50:33.967589 stellate_strawberry-1.1.0/README.md
+-rw-r--r--   0        0        0      342 2024-04-02 08:50:33.968212 stellate_strawberry-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4332 2024-04-02 08:50:33.968520 stellate_strawberry-1.1.0/stellate_strawberry/__init__.py
+-rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 stellate_strawberry-1.1.0/PKG-INFO
```

### Comparing `stellate_strawberry-1.0.0/README.md` & `stellate_strawberry-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```sh
 pip install stellate-strawberry
 ```
 
 ## Set Up
 
-Before you can make use of this gem, you need to [set up a Stellate service](https://stellate.co/docs/quickstart#1-create-stellate-service) and [create a logging token](https://stellate.co/docs/graphql-metrics/metrics-get-started#create-your-own-logging-token).
+Before you can make use of this library, you need to [set up a Stellate service](https://stellate.co/docs/quickstart#1-create-stellate-service) and [create a logging token](https://stellate.co/docs/graphql-metrics/metrics-get-started#create-your-own-logging-token).
 
 After that, add the Stellate extension when initializing your `strawberry.Schema` object in order to add [Stellate Metrics Logging](https://stellate.co/docs/graphql-metrics/metrics-get-started#metrics-collection):
 
 ```py
 from stellate_strawberry import create_stellate_extension
 
 service_name = "my-service"  # The name of your Stellate service
```

### Comparing `stellate_strawberry-1.0.0/stellate_strawberry/__init__.py` & `stellate_strawberry-1.1.0/stellate_strawberry/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,23 +55,28 @@
 
             request = self.execution_context.context["request"] if self.execution_context.context else None
             response = self.execution_context.context["response"] if self.execution_context.context else None
 
             forwarded_for = request.headers.get('x-forwarded-for') if request != None else None
             ips = forwarded_for.split(',') if forwarded_for != None and len(forwarded_for) > 0 else []
 
+            graphql_client_name = request.headers.get('x-graphql-client-name') if request != None else None
+            graphql_client_version = request.headers.get('x-graphql-client-version') if request != None else None
+
             payload = {
               "operation": self.execution_context.query,
               "method": self.execution_context.context["request"].method if self.execution_context.context else "POST",
               "responseSize": len(result_json),
               "responseHash": create_blake3_hash(result_json),
               "elapsed": round((end - start) * 1_000),
               "operationName": self.execution_context.provided_operation_name,
               "variablesHash": create_blake3_hash(json.dumps(self.execution_context.variables or {})),
               "ip": ips[0] if len(ips) > 0 else request.headers.get('true-client-ip') or request.headers.get('x-real-ip') if request != None else None,
+              "graphqlClientName": graphql_client_name,
+              "graphqlClientVersion": graphql_client_version,
               "errors": self.execution_context.errors,
               "statusCode": self.execution_context.context["response"].status_code or 200 if self.execution_context.context != None else 200,
               "userAgent": request.headers.get("user-agent") if request != None else None,
               "referer": request.headers.get("referer") if request != None else None,
               "hasSetCookie": "set-cookie" in response.headers.keys() if response != None else None,
             }
             t.queue.put(payload)
```

### Comparing `stellate_strawberry-1.0.0/PKG-INFO` & `stellate_strawberry-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellate-strawberry
-Version: 1.0.0
+Version: 1.1.0
 Summary: Integrate Stellate with your Strawberry GraphQL API
 Author: Stellate
 Author-email: eng@stellate.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 
 ```sh
 pip install stellate-strawberry
 ```
 
 ## Set Up
 
-Before you can make use of this gem, you need to [set up a Stellate service](https://stellate.co/docs/quickstart#1-create-stellate-service) and [create a logging token](https://stellate.co/docs/graphql-metrics/metrics-get-started#create-your-own-logging-token).
+Before you can make use of this library, you need to [set up a Stellate service](https://stellate.co/docs/quickstart#1-create-stellate-service) and [create a logging token](https://stellate.co/docs/graphql-metrics/metrics-get-started#create-your-own-logging-token).
 
 After that, add the Stellate extension when initializing your `strawberry.Schema` object in order to add [Stellate Metrics Logging](https://stellate.co/docs/graphql-metrics/metrics-get-started#metrics-collection):
 
 ```py
 from stellate_strawberry import create_stellate_extension
 
 service_name = "my-service"  # The name of your Stellate service
```

