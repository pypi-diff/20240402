# Comparing `tmp/uma-sdk-1.0.2.zip` & `tmp/uma-sdk-1.0.3.zip`

## zipinfo {}

```diff
@@ -1,49 +1,49 @@
-Zip file size: 39669 bytes, number of entries: 47
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/uma/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/
--rwxr-xr-x  2.0 unx       87 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/setup.py
--rw-r--r--  2.0 unx      648 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/setup.cfg
--rw-r--r--  2.0 unx      133 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/README.md
--rw-r--r--  2.0 unx    11352 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/LICENSE
--rw-r--r--  2.0 unx       81 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/pyproject.toml
--rw-r--r--  2.0 unx      631 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/
--rw-r--r--  2.0 unx     2160 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/cert_utils.py
--rw-r--r--  2.0 unx     3407 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/JSONable.py
--rw-r--r--  2.0 unx      284 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/uma_invoice_creator.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/py.typed
--rw-r--r--  2.0 unx    30116 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/uma.py
--rw-r--r--  2.0 unx      266 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/urls.py
--rw-r--r--  2.0 unx     2061 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/nonce_cache.py
--rw-r--r--  2.0 unx     2878 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/version.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/public_key_cache.py
--rw-r--r--  2.0 unx      868 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/exceptions.py
--rw-r--r--  2.0 unx      239 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/type_utils.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v0/
--rw-r--r--  2.0 unx      557 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/counterparty_data.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/__init__.py
--rw-r--r--  2.0 unx     1724 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/post_tx_callback.py
--rw-r--r--  2.0 unx     4498 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/pubkey_response.py
--rw-r--r--  2.0 unx      231 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/kyc_status.py
--rw-r--r--  2.0 unx     4609 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/currency.py
--rw-r--r--  2.0 unx      132 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/payee_data.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/lnurlp_response.py
--rw-r--r--  2.0 unx     2307 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/payer_data.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/lnurlp_request.py
--rw-r--r--  2.0 unx     6309 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/payreq.py
--rw-r--r--  2.0 unx     8829 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/payreq_response.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v1/__init__.py
--rw-r--r--  2.0 unx     2702 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v1/currency.py
--rw-r--r--  2.0 unx     4289 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v1/payreq.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v0/__init__.py
--rw-r--r--  2.0 unx     1950 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v0/currency.py
--rw-r--r--  2.0 unx     1788 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma/protocol/v0/payreq.py
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       30 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/top_level.txt
--rw-r--r--  2.0 unx      924 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      631 b- defN 24-Mar-27 17:21 uma-sdk-1.0.2/uma_sdk.egg-info/PKG-INFO
-47 files, 105382 bytes uncompressed, 32841 bytes compressed:  68.8%
+Zip file size: 39674 bytes, number of entries: 47
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/
+-rwxr-xr-x  2.0 unx       87 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/setup.py
+-rw-r--r--  2.0 unx      648 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/setup.cfg
+-rw-r--r--  2.0 unx      133 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/README.md
+-rw-r--r--  2.0 unx    11352 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/LICENSE
+-rw-r--r--  2.0 unx       81 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/pyproject.toml
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/
+-rw-r--r--  2.0 unx     2160 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/cert_utils.py
+-rw-r--r--  2.0 unx     3407 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/JSONable.py
+-rw-r--r--  2.0 unx      284 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/uma_invoice_creator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/py.typed
+-rw-r--r--  2.0 unx    30116 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/uma.py
+-rw-r--r--  2.0 unx      266 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/urls.py
+-rw-r--r--  2.0 unx     2061 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/nonce_cache.py
+-rw-r--r--  2.0 unx     2878 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/version.py
+-rw-r--r--  2.0 unx     1624 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/public_key_cache.py
+-rw-r--r--  2.0 unx      868 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/exceptions.py
+-rw-r--r--  2.0 unx      239 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/type_utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/
+-rw-r--r--  2.0 unx      557 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/counterparty_data.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/__init__.py
+-rw-r--r--  2.0 unx     1724 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/post_tx_callback.py
+-rw-r--r--  2.0 unx     4498 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/pubkey_response.py
+-rw-r--r--  2.0 unx      231 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/kyc_status.py
+-rw-r--r--  2.0 unx     4609 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/currency.py
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payee_data.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/lnurlp_response.py
+-rw-r--r--  2.0 unx     2307 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payer_data.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/lnurlp_request.py
+-rw-r--r--  2.0 unx     6328 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payreq.py
+-rw-r--r--  2.0 unx     8829 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payreq_response.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/__init__.py
+-rw-r--r--  2.0 unx     2702 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/currency.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/payreq.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/__init__.py
+-rw-r--r--  2.0 unx     1950 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/currency.py
+-rw-r--r--  2.0 unx     1788 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/payreq.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       30 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO
+47 files, 105406 bytes uncompressed, 32846 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,142 +1,142 @@
-Filename: uma-sdk-1.0.2/
+Filename: uma-sdk-1.0.3/
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/
+Filename: uma-sdk-1.0.3/uma/
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/
 Comment: 
 
-Filename: uma-sdk-1.0.2/setup.py
+Filename: uma-sdk-1.0.3/setup.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/setup.cfg
+Filename: uma-sdk-1.0.3/setup.cfg
 Comment: 
 
-Filename: uma-sdk-1.0.2/README.md
+Filename: uma-sdk-1.0.3/README.md
 Comment: 
 
-Filename: uma-sdk-1.0.2/LICENSE
+Filename: uma-sdk-1.0.3/LICENSE
 Comment: 
 
-Filename: uma-sdk-1.0.2/pyproject.toml
+Filename: uma-sdk-1.0.3/pyproject.toml
 Comment: 
 
-Filename: uma-sdk-1.0.2/PKG-INFO
+Filename: uma-sdk-1.0.3/PKG-INFO
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/
+Filename: uma-sdk-1.0.3/uma/protocol/
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/__init__.py
+Filename: uma-sdk-1.0.3/uma/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/cert_utils.py
+Filename: uma-sdk-1.0.3/uma/cert_utils.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/JSONable.py
+Filename: uma-sdk-1.0.3/uma/JSONable.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/uma_invoice_creator.py
+Filename: uma-sdk-1.0.3/uma/uma_invoice_creator.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/py.typed
+Filename: uma-sdk-1.0.3/uma/py.typed
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/uma.py
+Filename: uma-sdk-1.0.3/uma/uma.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/urls.py
+Filename: uma-sdk-1.0.3/uma/urls.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/nonce_cache.py
+Filename: uma-sdk-1.0.3/uma/nonce_cache.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/version.py
+Filename: uma-sdk-1.0.3/uma/version.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/public_key_cache.py
+Filename: uma-sdk-1.0.3/uma/public_key_cache.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/exceptions.py
+Filename: uma-sdk-1.0.3/uma/exceptions.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/type_utils.py
+Filename: uma-sdk-1.0.3/uma/type_utils.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v1/
+Filename: uma-sdk-1.0.3/uma/protocol/v1/
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v0/
+Filename: uma-sdk-1.0.3/uma/protocol/v0/
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/counterparty_data.py
+Filename: uma-sdk-1.0.3/uma/protocol/counterparty_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/__init__.py
+Filename: uma-sdk-1.0.3/uma/protocol/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/post_tx_callback.py
+Filename: uma-sdk-1.0.3/uma/protocol/post_tx_callback.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/pubkey_response.py
+Filename: uma-sdk-1.0.3/uma/protocol/pubkey_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/kyc_status.py
+Filename: uma-sdk-1.0.3/uma/protocol/kyc_status.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/currency.py
+Filename: uma-sdk-1.0.3/uma/protocol/currency.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/payee_data.py
+Filename: uma-sdk-1.0.3/uma/protocol/payee_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/lnurlp_response.py
+Filename: uma-sdk-1.0.3/uma/protocol/lnurlp_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/payer_data.py
+Filename: uma-sdk-1.0.3/uma/protocol/payer_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/lnurlp_request.py
+Filename: uma-sdk-1.0.3/uma/protocol/lnurlp_request.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/payreq.py
+Filename: uma-sdk-1.0.3/uma/protocol/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/payreq_response.py
+Filename: uma-sdk-1.0.3/uma/protocol/payreq_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v1/__init__.py
+Filename: uma-sdk-1.0.3/uma/protocol/v1/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v1/currency.py
+Filename: uma-sdk-1.0.3/uma/protocol/v1/currency.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v1/payreq.py
+Filename: uma-sdk-1.0.3/uma/protocol/v1/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v0/__init__.py
+Filename: uma-sdk-1.0.3/uma/protocol/v0/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v0/currency.py
+Filename: uma-sdk-1.0.3/uma/protocol/v0/currency.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma/protocol/v0/payreq.py
+Filename: uma-sdk-1.0.3/uma/protocol/v0/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/dependency_links.txt
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/dependency_links.txt
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/requires.txt
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/requires.txt
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/top_level.txt
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/top_level.txt
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/SOURCES.txt
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt
 Comment: 
 
-Filename: uma-sdk-1.0.2/uma_sdk.egg-info/PKG-INFO
+Filename: uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `uma-sdk-1.0.2/setup.cfg` & `uma-sdk-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uma-sdk
-version = 1.0.2
+version = 1.0.3
 description = Python SDK for UMA (universal money address)
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lightspark Group, Inc.
 author_email = info@lightspark.com
 license = Apache-2.0
 license_files = LICENSE
```

## Comparing `uma-sdk-1.0.2/LICENSE` & `uma-sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/PKG-INFO` & `uma-sdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma-sdk-1.0.2/uma/__init__.py` & `uma-sdk-1.0.3/uma/__init__.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/cert_utils.py` & `uma-sdk-1.0.3/uma/cert_utils.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/JSONable.py` & `uma-sdk-1.0.3/uma/JSONable.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/uma.py` & `uma-sdk-1.0.3/uma/uma.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/nonce_cache.py` & `uma-sdk-1.0.3/uma/nonce_cache.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/version.py` & `uma-sdk-1.0.3/uma/version.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/public_key_cache.py` & `uma-sdk-1.0.3/uma/public_key_cache.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/exceptions.py` & `uma-sdk-1.0.3/uma/exceptions.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/counterparty_data.py` & `uma-sdk-1.0.3/uma/protocol/counterparty_data.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/post_tx_callback.py` & `uma-sdk-1.0.3/uma/protocol/post_tx_callback.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/pubkey_response.py` & `uma-sdk-1.0.3/uma/protocol/pubkey_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/currency.py` & `uma-sdk-1.0.3/uma/protocol/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/lnurlp_response.py` & `uma-sdk-1.0.3/uma/protocol/lnurlp_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/payer_data.py` & `uma-sdk-1.0.3/uma/protocol/payer_data.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/lnurlp_request.py` & `uma-sdk-1.0.3/uma/protocol/lnurlp_request.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/payreq.py` & `uma-sdk-1.0.3/uma/protocol/payreq.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             return PayRequest(
                 sending_amount_currency_code=v1_payreq.sending_amount_currency_code,
                 receiving_currency_code=v1_payreq.receiving_currency_code,
                 amount=v1_payreq.amount,
                 payer_data=v1_payreq.payer_data,
                 requested_payee_data=v1_payreq.requested_payee_data,
                 comment=v1_payreq.comment,
-                uma_major_version=1,
+                uma_major_version=1 if is_v1 else None,
             )
         v0_payreq = V0PayRequest.from_json(json_encoded)
         return PayRequest(
             sending_amount_currency_code=v0_payreq.currency_code,
             receiving_currency_code=v0_payreq.currency_code,
             amount=v0_payreq.amount,
             payer_data=v0_payreq.payer_data,
```

## Comparing `uma-sdk-1.0.2/uma/protocol/payreq_response.py` & `uma-sdk-1.0.3/uma/protocol/payreq_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/v1/currency.py` & `uma-sdk-1.0.3/uma/protocol/v1/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/v1/payreq.py` & `uma-sdk-1.0.3/uma/protocol/v1/payreq.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         )
         if self.receiving_currency_code is not None:
             receiving_currency = result_dict.pop("receivingCurrencyCode")
             result_dict["convert"] = receiving_currency
         result_dict["amount"] = (
             f"{result_dict['amount']}.{sending_currency}"
             if sending_currency is not None
-            else result_dict["amount"]
+            else f"{result_dict['amount']}"
         )
         return result_dict
 
     @classmethod
     def _from_dict(cls, json_dict: Dict[str, Any]) -> Dict[str, Any]:
         data = super()._from_dict(json_dict)
         if "convert" in json_dict:
```

## Comparing `uma-sdk-1.0.2/uma/protocol/v0/currency.py` & `uma-sdk-1.0.3/uma/protocol/v0/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma/protocol/v0/payreq.py` & `uma-sdk-1.0.3/uma/protocol/v0/payreq.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma_sdk.egg-info/SOURCES.txt` & `uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.2/uma_sdk.egg-info/PKG-INFO` & `uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

