# Comparing `tmp/vitya-0.20.1.tar.gz` & `tmp/vitya-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.20.1.tar", last modified: Wed Mar 27 08:53:52 2024, max compression
+gzip compressed data, was "dist/vitya-0.20.2.tar", last modified: Tue Apr  2 11:45:33 2024, max compression
```

## Comparing `vitya-0.20.1.tar` & `vitya-0.20.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-27 08:53:47.000000 vitya-0.20.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-27 08:53:52.000000 vitya-0.20.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-27 08:53:47.000000 vitya-0.20.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-27 08:53:47.000000 vitya-0.20.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 08:53:52.000000 vitya-0.20.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-27 08:53:47.000000 vitya-0.20.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-27 08:53:47.000000 vitya-0.20.1/tests/test_error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-03-27 08:53:47.000000 vitya-0.20.1/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19337 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/payments/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/typing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-03-27 08:53:47.000000 vitya-0.20.1/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 08:53:52.000000 vitya-0.20.1/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 11:45:25.000000 vitya-0.20.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-02 11:45:33.000000 vitya-0.20.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-02 11:45:25.000000 vitya-0.20.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 11:45:25.000000 vitya-0.20.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:45:33.000000 vitya-0.20.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 11:45:25.000000 vitya-0.20.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-02 11:45:25.000000 vitya-0.20.2/tests/test_error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-02 11:45:25.000000 vitya-0.20.2/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/typing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.20.1/LICENSE` & `vitya-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/PKG-INFO` & `vitya-0.20.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.1
+Version: 0.20.2
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.1/README.md` & `vitya-0.20.2/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/setup.py` & `vitya-0.20.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.20.1',
+    version='0.20.2',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.20.1/tests/test_error_description.py` & `vitya-0.20.2/tests/test_error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/tests/test_vitya.py` & `vitya-0.20.2/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/error_description.py` & `vitya-0.20.2/vitya/error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/errors.py` & `vitya-0.20.2/vitya/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/errors_base.py` & `vitya-0.20.2/vitya/errors_base.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/enums.py` & `vitya-0.20.2/vitya/payment_order/enums.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/errors.py` & `vitya-0.20.2/vitya/payment_order/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/fields.py` & `vitya-0.20.2/vitya/payment_order/fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/payments/checkers.py` & `vitya-0.20.2/vitya/payment_order/payments/checkers.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/payments/checks.py` & `vitya-0.20.2/vitya/payment_order/payments/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,28 +527,28 @@
     payer_status: Optional[PayerStatus],
     uin: Optional[UIN],
     payer_inn: Optional[PayerINN],
 ) -> Optional[DocumentNumber]:
     if not payment_type.is_budget:
         return None
 
+    if payer_status == '31':
+        if value is not None:
+            raise DocumentNumberValidationBOOnlyEmptyError
+        return None
+
     if payment_type == PaymentType.FNS:
         if value is not None:
             raise DocumentNumberValidationFNSOnlyEmptyError
         return None
     elif payment_type == PaymentType.BUDGET_OTHER:
         if payer_status == '33' and date.today().year >= CHANGE_YEAR:
             if value is not None:
                 raise DocumentNumberValidationBOPayerStatus33OnlyEmptyError
             return None
-        if payer_status == '31':
-            if value is not None:
-                raise DocumentNumberValidationBOOnlyEmptyError
-            return None
-
         if payer_status == '24' and payer_inn is None and uin is None and value is None:
             raise DocumentNumberValidationBOEmptyNotAllowed
         if value is not None:
             if len(value) > 15:
                 raise DocumentNumberValidationBOValueLenError
             if len(value) < 3 or value[2] != ';' or value[:2] not in DOCUMENT_NUMBERS:
                 raise DocumentNumberValidationBOValueError
```

### Comparing `vitya-0.20.1/vitya/payment_order/payments/constants.py` & `vitya-0.20.2/vitya/payment_order/payments/constants.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/payments/tools.py` & `vitya-0.20.2/vitya/payment_order/payments/tools.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/payment_order/validators.py` & `vitya-0.20.2/vitya/payment_order/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/pydantic_fields.py` & `vitya-0.20.2/vitya/pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya/validators.py` & `vitya-0.20.2/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.1/vitya.egg-info/PKG-INFO` & `vitya-0.20.2/vitya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.1
+Version: 0.20.2
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.1/vitya.egg-info/SOURCES.txt` & `vitya-0.20.2/vitya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

