# Comparing `tmp/payze-pkg-2.2.tar.gz` & `tmp/payze-pkg-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payze-pkg-2.2.tar", last modified: Mon Apr  1 09:57:52 2024, max compression
+gzip compressed data, was "payze-pkg-2.3.tar", last modified: Tue Apr  2 07:41:14 2024, max compression
```

## Comparing `payze-pkg-2.2.tar` & `payze-pkg-2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.678645 payze-pkg-2.2/
--rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 09:57:52.678555 payze-pkg-2.2/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)      857 2024-04-01 04:25:57.000000 payze-pkg-2.2/README.md
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.675669 payze-pkg-2.2/payze/
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676374 payze-pkg-2.2/payze/payze/
--rw-r--r--   0 muhammadali   (501) staff       (20)       48 2024-04-01 09:56:33.000000 payze-pkg-2.2/payze/payze/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     1785 2024-04-01 09:56:55.000000 payze-pkg-2.2/payze/payze/client.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676480 payze-pkg-2.2/payze/payze/param/
--rw-r--r--   0 muhammadali   (501) staff       (20)      141 2024-04-01 04:17:05.000000 payze-pkg-2.2/payze/payze/param/__init__.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676737 payze-pkg-2.2/payze/payze/param/ops/
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-03-30 20:13:36.000000 payze-pkg-2.2/payze/payze/param/ops/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      407 2024-04-01 04:19:11.000000 payze-pkg-2.2/payze/payze/param/ops/client.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677110 payze-pkg-2.2/payze/payze/param/request/
--rw-r--r--   0 muhammadali   (501) staff       (20)       76 2024-04-01 04:06:02.000000 payze-pkg-2.2/payze/payze/param/request/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      507 2024-04-01 04:05:59.000000 payze-pkg-2.2/payze/payze/param/request/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      689 2024-04-01 04:26:58.000000 payze-pkg-2.2/payze/payze/param/request/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677460 payze-pkg-2.2/payze/payze/param/response/
--rw-r--r--   0 muhammadali   (501) staff       (20)       60 2024-04-01 04:06:00.000000 payze-pkg-2.2/payze/payze/param/response/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     2076 2024-04-01 03:57:51.000000 payze-pkg-2.2/payze/payze/param/response/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      200 2024-04-01 04:19:43.000000 payze-pkg-2.2/payze/payze/param/response/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677693 payze-pkg-2.2/payze/payze/param/webhook/
--rw-r--r--   0 muhammadali   (501) staff       (20)        0 2024-04-01 04:04:42.000000 payze-pkg-2.2/payze/payze/param/webhook/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     1533 2024-04-01 04:05:58.000000 payze-pkg-2.2/payze/payze/param/webhook/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.678312 payze-pkg-2.2/payze/payze_pkg.egg-info/
--rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)      663 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        1 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/requires.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        6 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/top_level.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)      107 2024-04-01 09:57:52.678937 payze-pkg-2.2/setup.cfg
--rw-r--r--   0 muhammadali   (501) staff       (20)      535 2024-04-01 09:57:36.000000 payze-pkg-2.2/setup.py
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

### Comparing `payze-pkg-2.2/README.md` & `payze-pkg-2.3/README.md`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2/payze/payze/client.py` & `payze-pkg-2.3/payze/payze/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,17 @@
     ) -> payze_res.JustPay:
         """
         the just pay method implementation
         """
         url = f"{self.url}/v2/api/payment"
 
         req_params = payze_req.JustPay(
-            amount=req_params.amount
+            amount=req_params.amount,
+            idempotency_key=req_params.idempotency_key,
+            metadata=req_params.metadata
         )
         req_params.hooks = self.hooks
         req_data = json.dumps(req_params.to_dict())
 
         resp_data = self.__send_request(url, req_data, "PUT")
 
         return self._handle_response(resp_data, payze_res.JustPay)
```

### Comparing `payze-pkg-2.2/payze/payze/param/request/just_pay.py` & `payze-pkg-2.3/payze/payze/param/request/just_pay.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,22 @@
     the paywith card parameters model
     """
     amount: float
     language: str = "UZ"
     source: str = "Card"
     currency: str = "UZS"
     hooks: base.Hooks = None
+    metadata: base.Metadata = None
     idempotency_key: str = str(uuid.uuid4())
 
     def to_dict(self):
         """
         the dict representation.
         """
         return {
             "amount": self.amount,
             "currency": self.currency,
             "hooks": self.hooks.to_dict(),
             "idempotencyKey": self.idempotency_key,
             "source": self.source,
+            "metadata": self.metadata.to_dict()
         }
```

### Comparing `payze-pkg-2.2/payze/payze/param/response/base.py` & `payze-pkg-2.3/payze/payze/param/response/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 the just_pay response model
 """
 from typing import Optional
+
+from pydantic import Field
 from pydantic import BaseModel
 
 
 class CardPaymentDetails(BaseModel):
     """
     the card payment details model.
     """
@@ -52,15 +54,17 @@
     id: int
     idempotencyKey: str
     language: Optional[str]
     lastModifiedDate: str
     metadata: Optional[dict]
     network: Optional[str]
     payer: Optional[dict]
-    paymentUrl: str
+    payment_url: str = Field(
+        alias="paymentUrl"
+    )
     receipt: Optional[str]
     refundedAmount: Optional[int]
     refundedDate: Optional[str]
     rejectReason: Optional[str]
     rejectedDate: Optional[str]
     requesterId: int
     reverseDate: Optional[str]
```

### Comparing `payze-pkg-2.2/payze/payze/param/webhook/just_pay.py` & `payze-pkg-2.3/payze/payze/param/webhook/just_pay.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2/payze/payze_pkg.egg-info/SOURCES.txt` & `payze-pkg-2.3/payze/payze_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.2/setup.py` & `payze-pkg-2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
     name='payze-pkg',
-    version='2.2',
+    version='2.3',
     license='MIT',
     author="paytechuz",
     author_email='paytechuz@gmail.com',
     packages=find_packages('payze'),
     package_dir={'': 'payze'},
     url='https://github.com/PayTechUz/payze-pkg',
     keywords='payze-merchant payze-uz payze-pkg payze-python payze-github',
```

