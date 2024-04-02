# Comparing `tmp/payze-pkg-2.2.3.tar.gz` & `tmp/payze-pkg-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payze-pkg-2.2.3.tar", last modified: Tue Apr  2 08:43:18 2024, max compression
+gzip compressed data, was "payze-pkg-2.3.tar", last modified: Tue Apr  2 07:41:14 2024, max compression
```

## Comparing `payze-pkg-2.2.3.tar` & `payze-pkg-2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.529164 payze-pkg-2.2.3/
--rw-r--r--   0 muhammadali   (501) staff       (20)      330 2024-04-02 08:43:18.529086 payze-pkg-2.2.3/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)     1094 2024-04-02 08:20:07.000000 payze-pkg-2.2.3/README.md
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.493859 payze-pkg-2.2.3/payze/
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.498988 payze-pkg-2.2.3/payze/payze/
--rw-r--r--   0 muhammadali   (501) staff       (20)       48 2024-04-02 06:11:05.000000 payze-pkg-2.2.3/payze/payze/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     2025 2024-04-02 08:42:09.000000 payze-pkg-2.2.3/payze/payze/client.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.501496 payze-pkg-2.2.3/payze/payze/param/
--rw-r--r--   0 muhammadali   (501) staff       (20)      141 2024-04-02 06:10:24.000000 payze-pkg-2.2.3/payze/payze/param/__init__.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.502382 payze-pkg-2.2.3/payze/payze/param/ops/
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-03-30 20:13:36.000000 payze-pkg-2.2.3/payze/payze/param/ops/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      407 2024-04-01 04:19:11.000000 payze-pkg-2.2.3/payze/payze/param/ops/client.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.513340 payze-pkg-2.2.3/payze/payze/param/request/
--rw-r--r--   0 muhammadali   (501) staff       (20)       76 2024-04-01 09:58:49.000000 payze-pkg-2.2.3/payze/payze/param/request/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     5004 2024-04-02 08:16:21.000000 payze-pkg-2.2.3/payze/payze/param/request/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      841 2024-04-02 08:38:13.000000 payze-pkg-2.2.3/payze/payze/param/request/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.526680 payze-pkg-2.2.3/payze/payze/param/response/
--rw-r--r--   0 muhammadali   (501) staff       (20)       60 2024-04-01 04:06:00.000000 payze-pkg-2.2.3/payze/payze/param/response/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     2147 2024-04-02 06:12:04.000000 payze-pkg-2.2.3/payze/payze/param/response/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      200 2024-04-01 10:31:41.000000 payze-pkg-2.2.3/payze/payze/param/response/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.527192 payze-pkg-2.2.3/payze/payze/param/webhook/
--rw-r--r--   0 muhammadali   (501) staff       (20)        0 2024-04-01 04:04:42.000000 payze-pkg-2.2.3/payze/payze/param/webhook/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     1533 2024-04-01 04:05:58.000000 payze-pkg-2.2.3/payze/payze/param/webhook/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 08:43:18.528699 payze-pkg-2.2.3/payze/payze_pkg.egg-info/
--rw-r--r--   0 muhammadali   (501) staff       (20)      330 2024-04-02 08:43:18.000000 payze-pkg-2.2.3/payze/payze_pkg.egg-info/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)      663 2024-04-02 08:43:18.000000 payze-pkg-2.2.3/payze/payze_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        1 2024-04-02 08:43:18.000000 payze-pkg-2.2.3/payze/payze_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-04-02 08:43:18.000000 payze-pkg-2.2.3/payze/payze_pkg.egg-info/requires.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        6 2024-04-02 08:43:18.000000 payze-pkg-2.2.3/payze/payze_pkg.egg-info/top_level.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)      107 2024-04-02 08:43:18.529440 payze-pkg-2.2.3/setup.cfg
--rw-r--r--   0 muhammadali   (501) staff       (20)      537 2024-04-02 08:42:47.000000 payze-pkg-2.2.3/setup.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.720144 payze-pkg-2.3/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-02 07:41:14.720082 payze-pkg-2.3/PKG-INFO
+-rw-r--r--   0 muhammadali   (501) staff       (20)      857 2024-04-01 04:25:57.000000 payze-pkg-2.3/README.md
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.715685 payze-pkg-2.3/payze/
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.716522 payze-pkg-2.3/payze/payze/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       48 2024-04-02 06:11:05.000000 payze-pkg-2.3/payze/payze/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     1883 2024-04-02 07:36:10.000000 payze-pkg-2.3/payze/payze/client.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.716767 payze-pkg-2.3/payze/payze/param/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      141 2024-04-02 06:10:24.000000 payze-pkg-2.3/payze/payze/param/__init__.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.717150 payze-pkg-2.3/payze/payze/param/ops/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-03-30 20:13:36.000000 payze-pkg-2.3/payze/payze/param/ops/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      407 2024-04-01 04:19:11.000000 payze-pkg-2.3/payze/payze/param/ops/client.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.717753 payze-pkg-2.3/payze/payze/param/request/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       76 2024-04-01 09:58:49.000000 payze-pkg-2.3/payze/payze/param/request/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     4994 2024-04-02 07:31:53.000000 payze-pkg-2.3/payze/payze/param/request/base.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      772 2024-04-02 07:32:13.000000 payze-pkg-2.3/payze/payze/param/request/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.718554 payze-pkg-2.3/payze/payze/param/response/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       60 2024-04-01 04:06:00.000000 payze-pkg-2.3/payze/payze/param/response/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     2147 2024-04-02 06:12:04.000000 payze-pkg-2.3/payze/payze/param/response/base.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      200 2024-04-01 10:31:41.000000 payze-pkg-2.3/payze/payze/param/response/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.718904 payze-pkg-2.3/payze/payze/param/webhook/
+-rw-r--r--   0 muhammadali   (501) staff       (20)        0 2024-04-01 04:04:42.000000 payze-pkg-2.3/payze/payze/param/webhook/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     1533 2024-04-01 04:05:58.000000 payze-pkg-2.3/payze/payze/param/webhook/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-02 07:41:14.719851 payze-pkg-2.3/payze/payze_pkg.egg-info/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-02 07:41:14.000000 payze-pkg-2.3/payze/payze_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadali   (501) staff       (20)      663 2024-04-02 07:41:14.000000 payze-pkg-2.3/payze/payze_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)        1 2024-04-02 07:41:14.000000 payze-pkg-2.3/payze/payze_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-04-02 07:41:14.000000 payze-pkg-2.3/payze/payze_pkg.egg-info/requires.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)        6 2024-04-02 07:41:14.000000 payze-pkg-2.3/payze/payze_pkg.egg-info/top_level.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)      107 2024-04-02 07:41:14.720354 payze-pkg-2.3/setup.cfg
+-rw-r--r--   0 muhammadali   (501) staff       (20)      535 2024-04-02 07:41:07.000000 payze-pkg-2.3/setup.py
```

### Comparing `payze-pkg-2.2.3/payze/payze/client.py` & `payze-pkg-2.3/payze/payze/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,32 +48,25 @@
         resp_data: dict,
         resp_class: Any
     ) -> Any:
         return resp_class(**resp_data)
 
     def just_pay(
         self,
-        req_params: payze_req.JustPay,
-        **kwargs
+        req_params: payze_req.JustPay
     ) -> payze_res.JustPay:
         """
         the just pay method implementation
         """
         url = f"{self.url}/v2/api/payment"
 
         req_params = payze_req.JustPay(
             amount=req_params.amount,
             idempotency_key=req_params.idempotency_key,
             metadata=req_params.metadata
         )
-
-        if req_params.metadata:
-            req_params.metadata.extra_attributes = [
-                kwargs
-            ]
-
         req_params.hooks = self.hooks
         req_data = json.dumps(req_params.to_dict())
 
         resp_data = self.__send_request(url, req_data, "PUT")
 
         return self._handle_response(resp_data, payze_res.JustPay)
```

### Comparing `payze-pkg-2.2.3/payze/payze/param/request/base.py` & `payze-pkg-2.3/payze/payze/param/request/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,16 +186,16 @@
             self.order = self.order.to_dict()
 
         if self.extra_attributes:
             for item in self.extra_attributes:
                 for key, value in item.items():
                     extra_attributes.append(
                         ExtraAttributes(
-                            key=str(key),
-                            value=str(value)
+                            key=key,
+                            value=value
                         ).to_dict()
                     )
 
         return {
             "Order": self.order,
             "Channel": self.channel,
             "ExtraAttributes": extra_attributes
```

### Comparing `payze-pkg-2.2.3/payze/payze/param/request/just_pay.py` & `payze-pkg-2.3/payze/payze/param/request/just_pay.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,15 @@
     metadata: base.Metadata = None
     idempotency_key: str = str(uuid.uuid4())
 
     def to_dict(self):
         """
         the dict representation.
         """
-        if self.metadata:
-            self.metadata = self.metadata.to_dict()
-
         return {
             "amount": self.amount,
             "currency": self.currency,
             "hooks": self.hooks.to_dict(),
             "idempotencyKey": self.idempotency_key,
             "source": self.source,
-            "metadata": self.metadata
+            "metadata": self.metadata.to_dict()
         }
```

### Comparing `payze-pkg-2.2.3/payze/payze/param/response/base.py` & `payze-pkg-2.3/payze/payze/param/response/base.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2.3/payze/payze/param/webhook/just_pay.py` & `payze-pkg-2.3/payze/payze/param/webhook/just_pay.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2.3/payze/payze_pkg.egg-info/SOURCES.txt` & `payze-pkg-2.3/payze/payze_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2.3/setup.py` & `payze-pkg-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
     name='payze-pkg',
-    version='2.2.3',
+    version='2.3',
     license='MIT',
     author="paytechuz",
     author_email='paytechuz@gmail.com',
     packages=find_packages('payze'),
     package_dir={'': 'payze'},
     url='https://github.com/PayTechUz/payze-pkg',
     keywords='payze-merchant payze-uz payze-pkg payze-python payze-github',
```

