# Comparing `tmp/ottu-py-1.3.0.tar.gz` & `tmp/ottu-py-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ottu-py-1.3.0.tar", last modified: Thu Mar 14 09:03:41 2024, max compression
+gzip compressed data, was "ottu-py-1.4.0.tar", last modified: Tue Apr  2 04:32:22 2024, max compression
```

## Comparing `ottu-py-1.3.0.tar` & `ottu-py-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.489655 ottu-py-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-14 09:03:36.000000 ottu-py-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-03-14 09:03:41.489655 ottu-py-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-03-14 09:03:36.000000 ottu-py-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-14 09:03:36.000000 ottu-py-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 09:03:41.489655 ottu-py-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.485655 ottu-py-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.485655 ottu-py-1.3.0/src/ottu/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/cards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.485655 ottu-py-1.3.0/src/ottu/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.489655 ottu-py-1.3.0/src/ottu/contrib/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.489655 ottu-py-1.3.0/src/ottu/contrib/django/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/core/ottu.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.489655 ottu-py-1.3.0/src/ottu/contrib/django/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/contrib/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/ottu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    25392 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/session.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-14 09:03:36.000000 ottu-py-1.3.0/src/ottu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:03:41.489655 ottu-py-1.3.0/src/ottu_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-03-14 09:03:41.000000 ottu-py-1.3.0/src/ottu_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-14 09:03:41.000000 ottu-py-1.3.0/src/ottu_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 09:03:41.000000 ottu-py-1.3.0/src/ottu_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-14 09:03:41.000000 ottu-py-1.3.0/src/ottu_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-14 09:03:41.000000 ottu-py-1.3.0/src/ottu_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.274658 ottu-py-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-02 04:32:12.000000 ottu-py-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-04-02 04:32:22.274658 ottu-py-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19469 2024-04-02 04:32:12.000000 ottu-py-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-02 04:32:12.000000 ottu-py-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:32:22.274658 ottu-py-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.266658 ottu-py-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.270658 ottu-py-1.4.0/src/ottu/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/cards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.270658 ottu-py-1.4.0/src/ottu/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.270658 ottu-py-1.4.0/src/ottu/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.274658 ottu-py-1.4.0/src/ottu/contrib/django/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/core/ottu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.274658 ottu-py-1.4.0/src/ottu/contrib/django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/contrib/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/ottu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26609 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-02 04:32:12.000000 ottu-py-1.4.0/src/ottu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:32:22.274658 ottu-py-1.4.0/src/ottu_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-04-02 04:32:22.000000 ottu-py-1.4.0/src/ottu_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 04:32:22.000000 ottu-py-1.4.0/src/ottu_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:32:22.000000 ottu-py-1.4.0/src/ottu_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-02 04:32:22.000000 ottu-py-1.4.0/src/ottu_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 04:32:22.000000 ottu-py-1.4.0/src/ottu_py.egg-info/top_level.txt
```

### Comparing `ottu-py-1.3.0/LICENSE` & `ottu-py-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/PKG-INFO` & `ottu-py-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ottu-py
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python bindings for the Ottu Checkout API
 Author-email: Jerin Peter George <jerinpetergeorge@gmail.com>
 Project-URL: Homepage, https://github.com/ottuco/ottu-py
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -160,14 +160,44 @@
     pg_codes=["mpgs", "ottu_pg"],
     customer_phone="+96550000000",
     order_no="1234567890",
     ...
 )
 print(response)
 ```
+#### Checkout API with dynamic argument(s)
+
+Developers can pass any number of dynamic arguments to the `checkout(...)` method. The dynamic arguments will be passed to the API as it is.
+
+```python
+from ottu import Ottu
+from ottu.auth import APIKeyAuth
+from ottu.enums import TxnType
+
+ottu = Ottu(
+    merchant_id="merchant.id.ottu.dev",
+    auth=APIKeyAuth("your-secret-api-key"),
+    customer_id="your-customer-id"
+)
+response = ottu.checkout(
+    txn_type=TxnType.PAYMENT_REQUEST,
+    amount="20.23",
+    currency_code="KWD",
+    pg_codes=["mpgs", "ottu_pg"],
+    customer_phone="+96550000000",
+    order_no="1234567890",
+
+    extra_name="John", # dynamic argument 1
+    extra_age="25", # dynamic argument 2
+    extra_country="Kuwait", # dynamic argument 3
+)
+print(response)
+```
+Here, `extra_name`, `extra_age`, and `extra_country` are the dynamic arguments which are not supported by the SDK, but may be supported by the API.
+```python
 
 ### Session Retrieve
 
 ```python
 from ottu import Ottu
 from ottu.auth import APIKeyAuth
```

### Comparing `ottu-py-1.3.0/README.md` & `ottu-py-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,44 @@
     pg_codes=["mpgs", "ottu_pg"],
     customer_phone="+96550000000",
     order_no="1234567890",
     ...
 )
 print(response)
 ```
+#### Checkout API with dynamic argument(s)
+
+Developers can pass any number of dynamic arguments to the `checkout(...)` method. The dynamic arguments will be passed to the API as it is.
+
+```python
+from ottu import Ottu
+from ottu.auth import APIKeyAuth
+from ottu.enums import TxnType
+
+ottu = Ottu(
+    merchant_id="merchant.id.ottu.dev",
+    auth=APIKeyAuth("your-secret-api-key"),
+    customer_id="your-customer-id"
+)
+response = ottu.checkout(
+    txn_type=TxnType.PAYMENT_REQUEST,
+    amount="20.23",
+    currency_code="KWD",
+    pg_codes=["mpgs", "ottu_pg"],
+    customer_phone="+96550000000",
+    order_no="1234567890",
+
+    extra_name="John", # dynamic argument 1
+    extra_age="25", # dynamic argument 2
+    extra_country="Kuwait", # dynamic argument 3
+)
+print(response)
+```
+Here, `extra_name`, `extra_age`, and `extra_country` are the dynamic arguments which are not supported by the SDK, but may be supported by the API.
+```python
 
 ### Session Retrieve
 
 ```python
 from ottu import Ottu
 from ottu.auth import APIKeyAuth
```

### Comparing `ottu-py-1.3.0/pyproject.toml` & `ottu-py-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ottu-py"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
     { name = "Jerin Peter George", email = "jerinpetergeorge@gmail.com" },
 ]
 description = "Python bindings for the Ottu Checkout API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ottu-py-1.3.0/src/ottu/auth.py` & `ottu-py-1.4.0/src/ottu/auth.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/cards.py` & `ottu-py-1.4.0/src/ottu/cards.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/admin.py` & `ottu-py-1.4.0/src/ottu/contrib/django/admin.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/conf.py` & `ottu-py-1.4.0/src/ottu/contrib/django/conf.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/core/ottu.py` & `ottu-py-1.4.0/src/ottu/contrib/django/core/ottu.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/core/session.py` & `ottu-py-1.4.0/src/ottu/contrib/django/core/session.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/migrations/0001_initial.py` & `ottu-py-1.4.0/src/ottu/contrib/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/models.py` & `ottu-py-1.4.0/src/ottu/contrib/django/models.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/contrib/django/views.py` & `ottu-py-1.4.0/src/ottu/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/errors.py` & `ottu-py-1.4.0/src/ottu/errors.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/mixins.py` & `ottu-py-1.4.0/src/ottu/mixins.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/ottu.py` & `ottu-py-1.4.0/src/ottu/ottu.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         return self._session
 
     def _update_session(self, session: Session) -> None:
         self._session = session
 
     def checkout(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         pg_codes: list[str],
         payment_type: str = "one_off",
         customer_id: typing.Optional[str] = None,
         customer_email: typing.Optional[str] = None,
@@ -91,14 +92,16 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        **kwargs,
     ) -> dict:
         """
         a proxy method to `Session.create(...)`
         """
         return self.session.create(
             txn_type=txn_type,
             amount=amount,
@@ -126,14 +129,16 @@
             product_type=product_type,
             redirect_url=redirect_url,
             shopping_address=shopping_address,
             shortify_attachment_url=shortify_attachment_url,
             shortify_checkout_url=shortify_checkout_url,
             vendor_name=vendor_name,
             webhook_url=webhook_url,
+            include_sdk_setup_preload=include_sdk_setup_preload,
+            **kwargs,
         )
 
     def auto_debit(
         self,
         token: str,
         session_id: str,
     ):
@@ -143,14 +148,15 @@
     def cards(self) -> Card:
         if self._card is None:
             self._card = Card(ottu=self)
         return self._card
 
     def checkout_autoflow(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         payment_type: str = "one_off",
         customer_id: typing.Optional[str] = None,
         customer_email: typing.Optional[str] = None,
         customer_phone: typing.Optional[str] = None,
@@ -172,14 +178,16 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        checkout_extra_args: typing.Optional[dict] = None,
     ):
         return self.session.checkout_autoflow(
             txn_type=txn_type,
             amount=amount,
             currency_code=currency_code,
             payment_type=payment_type,
             customer_id=customer_id,
@@ -203,18 +211,21 @@
             product_type=product_type,
             redirect_url=redirect_url,
             shopping_address=shopping_address,
             shortify_attachment_url=shortify_attachment_url,
             shortify_checkout_url=shortify_checkout_url,
             vendor_name=vendor_name,
             webhook_url=webhook_url,
+            include_sdk_setup_preload=include_sdk_setup_preload,
+            checkout_extra_args=checkout_extra_args,
         )
 
     def auto_debit_autoflow(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         customer_id: str,
         agreement: dict,
         pg_codes: typing.Optional[list[str]] = None,
         customer_email: typing.Optional[str] = None,
@@ -236,14 +247,16 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        checkout_extra_args: typing.Optional[dict] = None,
         token: typing.Optional[str] = None,
     ):
         return self.session.auto_debit_autoflow(
             txn_type=txn_type,
             amount=amount,
             currency_code=currency_code,
             customer_id=customer_id,
@@ -268,14 +281,16 @@
             product_type=product_type,
             redirect_url=redirect_url,
             shopping_address=shopping_address,
             shortify_attachment_url=shortify_attachment_url,
             shortify_checkout_url=shortify_checkout_url,
             vendor_name=vendor_name,
             webhook_url=webhook_url,
+            include_sdk_setup_preload=include_sdk_setup_preload,
+            checkout_extra_args=checkout_extra_args,
             token=token,
         )
 
     def raw(
         self,
         method: str,
         path: str,
```

### Comparing `ottu-py-1.3.0/src/ottu/request.py` & `ottu-py-1.4.0/src/ottu/request.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu/session.py` & `ottu-py-1.4.0/src/ottu/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import logging
 import typing
 from dataclasses import dataclass
 
 from .decorators import interruption_handler
 from .enums import HTTPMethod, TxnType
 from .errors import APIInterruptError, ValidationError
 from .mixins import AsDictMixin
 from .request import OttuPYResponse
 from .utils import remove_empty_values
 
 if typing.TYPE_CHECKING:
     from .ottu import Ottu
 
+logger = logging.getLogger("ottu-py")
+
 
 @dataclass
 class PaymentMethod(AsDictMixin):
     code: typing.Optional[str] = None
     name: typing.Optional[str] = None
     pg: typing.Optional[str] = None
     type: typing.Optional[str] = None
@@ -131,14 +134,15 @@
         with open(path, "rb") as f:
             content = f.read()
             name = f.name or "attachment.pdf"
         return name, content
 
     def create(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         pg_codes: list[str],
         payment_type: str = "one_off",
         customer_id: typing.Optional[str] = None,
         customer_email: typing.Optional[str] = None,
@@ -161,14 +165,16 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        **kwargs,
     ) -> dict:
         """
         Creates a new checkout session.
         :param txn_type: Transaction type
         :param amount: Amount
         :param currency_code: Currency code
         :param pg_codes: Payment gateway codes
@@ -193,16 +199,25 @@
         :param product_type: Product type
         :param redirect_url: Redirect URL
         :param shopping_address: Shopping address
         :param shortify_attachment_url: Shortify attachment URL
         :param shortify_checkout_url: Shortify checkout URL
         :param vendor_name: Vendor name
         :param webhook_url: Webhook URL
+        :param include_sdk_setup_preload: Include SDK setup preload
+        :param kwargs: Additional arguments supported by the API
         :return: Session
         """
+        if kwargs:
+            msg = (
+                f"The following arguments are not "
+                f"supported by the SDK: {', '.join(kwargs.keys())}"
+            )
+            logger.warning(msg)
+
         customer_id = customer_id or self.ottu.customer_id
         payload = {
             "type": txn_type.value,
             "amount": amount,
             "currency_code": currency_code,
             "pg_codes": pg_codes,
             "payment_type": payment_type,
@@ -226,16 +241,18 @@
             "product_type": product_type,
             "redirect_url": redirect_url,
             "shopping_address": shopping_address,
             "shortify_attachment_url": shortify_attachment_url,
             "shortify_checkout_url": shortify_checkout_url,
             "vendor_name": vendor_name,
             "webhook_url": webhook_url,
+            "include_sdk_setup_preload": include_sdk_setup_preload,
         }
         payload = remove_empty_values(payload)
+        payload.update(kwargs)  # `kwargs` may contain `None` values
         if attachment:
             json_or_form = {
                 "data": payload,
                 "files": {"attachment": self.__path_to_file(path=attachment)},
             }
         else:
             json_or_form = {
@@ -280,14 +297,15 @@
             response = self.retrieve(session_id=session_id)
             if response["success"]:
                 return response
         return None
 
     def update(
         self,
+        *,
         amount: typing.Optional[str] = None,
         currency_code: typing.Optional[str] = None,
         pg_codes: typing.Optional[list[str]] = None,
         customer_id: typing.Optional[str] = None,
         customer_email: typing.Optional[str] = None,
         customer_phone: typing.Optional[str] = None,
         customer_first_name: typing.Optional[str] = None,
@@ -537,14 +555,15 @@
 
     def get_token_from_db(self, agreement, customer_id) -> str:
         raise NotImplementedError("Please implement this method in your subclass")
 
     @interruption_handler
     def checkout_autoflow(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         payment_type: str = "one_off",
         customer_id: typing.Optional[str] = None,
         customer_email: typing.Optional[str] = None,
         customer_phone: typing.Optional[str] = None,
@@ -566,16 +585,19 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        checkout_extra_args: typing.Optional[dict] = None,
     ):
         pg_codes = self.get_pg_codes(plugin=txn_type, currency=currency_code)
+        checkout_extra_args = checkout_extra_args or {}
         return self.create(
             txn_type=txn_type,
             amount=amount,
             currency_code=currency_code,
             pg_codes=pg_codes,
             payment_type=payment_type,
             customer_id=customer_id,
@@ -599,19 +621,22 @@
             product_type=product_type,
             redirect_url=redirect_url,
             shopping_address=shopping_address,
             shortify_attachment_url=shortify_attachment_url,
             shortify_checkout_url=shortify_checkout_url,
             vendor_name=vendor_name,
             webhook_url=webhook_url,
+            include_sdk_setup_preload=include_sdk_setup_preload,
+            **checkout_extra_args,
         )
 
     @interruption_handler
     def auto_debit_autoflow(
         self,
+        *,
         txn_type: TxnType,
         amount: str,
         currency_code: str,
         customer_id: str,
         agreement: dict,
         pg_codes: typing.Optional[list[str]] = None,
         customer_email: typing.Optional[str] = None,
@@ -633,20 +658,23 @@
         product_type: typing.Optional[str] = None,
         redirect_url: typing.Optional[str] = None,
         shopping_address: typing.Optional[dict] = None,
         shortify_attachment_url: typing.Optional[bool] = None,
         shortify_checkout_url: typing.Optional[bool] = None,
         vendor_name: typing.Optional[str] = None,
         webhook_url: typing.Optional[str] = None,
+        include_sdk_setup_preload: typing.Optional[bool] = None,
+        checkout_extra_args: typing.Optional[dict] = None,
         token: typing.Optional[str] = None,
     ):
         """
         Completes the auto debit flow by automatically
         identifying the "latest" payment method and the token.
         """
+        checkout_extra_args = checkout_extra_args or {}
         if not token:
             token = self.get_token_from_db(agreement=agreement, customer_id=customer_id)
         if not pg_codes:
             pg_codes = self.get_auto_debit_pg_codes(
                 plugin=txn_type,
                 currency=currency_code,
             )
@@ -677,12 +705,14 @@
             product_type=product_type,
             redirect_url=redirect_url,
             shopping_address=shopping_address,
             shortify_attachment_url=shortify_attachment_url,
             shortify_checkout_url=shortify_checkout_url,
             vendor_name=vendor_name,
             webhook_url=webhook_url,
+            include_sdk_setup_preload=include_sdk_setup_preload,
+            **checkout_extra_args,
         )
         if not checkout_response["success"]:
             raise APIInterruptError(**checkout_response)
         session_id = checkout_response["response"]["session_id"]
         return self.auto_debit(token=token, session_id=session_id)
```

### Comparing `ottu-py-1.3.0/src/ottu/utils.py` & `ottu-py-1.4.0/src/ottu/utils.py`

 * *Files identical despite different names*

### Comparing `ottu-py-1.3.0/src/ottu_py.egg-info/PKG-INFO` & `ottu-py-1.4.0/src/ottu_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ottu-py
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python bindings for the Ottu Checkout API
 Author-email: Jerin Peter George <jerinpetergeorge@gmail.com>
 Project-URL: Homepage, https://github.com/ottuco/ottu-py
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -160,14 +160,44 @@
     pg_codes=["mpgs", "ottu_pg"],
     customer_phone="+96550000000",
     order_no="1234567890",
     ...
 )
 print(response)
 ```
+#### Checkout API with dynamic argument(s)
+
+Developers can pass any number of dynamic arguments to the `checkout(...)` method. The dynamic arguments will be passed to the API as it is.
+
+```python
+from ottu import Ottu
+from ottu.auth import APIKeyAuth
+from ottu.enums import TxnType
+
+ottu = Ottu(
+    merchant_id="merchant.id.ottu.dev",
+    auth=APIKeyAuth("your-secret-api-key"),
+    customer_id="your-customer-id"
+)
+response = ottu.checkout(
+    txn_type=TxnType.PAYMENT_REQUEST,
+    amount="20.23",
+    currency_code="KWD",
+    pg_codes=["mpgs", "ottu_pg"],
+    customer_phone="+96550000000",
+    order_no="1234567890",
+
+    extra_name="John", # dynamic argument 1
+    extra_age="25", # dynamic argument 2
+    extra_country="Kuwait", # dynamic argument 3
+)
+print(response)
+```
+Here, `extra_name`, `extra_age`, and `extra_country` are the dynamic arguments which are not supported by the SDK, but may be supported by the API.
+```python
 
 ### Session Retrieve
 
 ```python
 from ottu import Ottu
 from ottu.auth import APIKeyAuth
```

### Comparing `ottu-py-1.3.0/src/ottu_py.egg-info/SOURCES.txt` & `ottu-py-1.4.0/src/ottu_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

