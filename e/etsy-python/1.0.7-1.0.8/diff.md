# Comparing `tmp/etsy-python-1.0.7.tar.gz` & `tmp/etsy-python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-python-1.0.7.tar", last modified: Fri Feb 16 07:09:14 2024, max compression
+gzip compressed data, was "etsy-python-1.0.8.tar", last modified: Sat Feb 17 17:22:48 2024, max compression
```

## Comparing `etsy-python-1.0.7.tar` & `etsy-python-1.0.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.806961 etsy-python-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-16 07:09:02.000000 etsy-python-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40498 2024-02-16 07:09:14.806961 etsy-python-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39731 2024-02-16 07:09:02.000000 etsy-python-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.794961 etsy-python-1.0.7/etsy_python/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.794961 etsy-python-1.0.7/etsy_python/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.794961 etsy-python-1.0.7/etsy_python/v3/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/auth/OAuth.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.798961 etsy-python-1.0.7/etsy_python/v3/common/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/common/Env.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/common/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/common/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.798961 etsy-python-1.0.7/etsy_python/v3/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/Listing.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/ListingInventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/ShippingProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/ShopReceipt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.798961 etsy-python-1.0.7/etsy_python/v3/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/exceptions/BaseAPIException.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/exceptions/RequestException.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.798961 etsy-python-1.0.7/etsy_python/v3/models/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/FileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/ShippingProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/ShopReturnPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.806961 etsy-python-1.0.7/etsy_python/v3/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingInventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingOffering.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingTranslation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingVariationImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ListingVideo.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/PaymentLedgerEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ReceiptTransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Review.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ShippingProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ShopProductionPartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ShopReturnPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/ShopSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/Taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/User.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/UserAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.806961 etsy-python-1.0.7/etsy_python/v3/resources/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/enums/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/enums/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/resources/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.806961 etsy-python-1.0.7/etsy_python/v3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:02.000000 etsy-python-1.0.7/etsy_python/v3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:09:14.806961 etsy-python-1.0.7/etsy_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40498 2024-02-16 07:09:14.000000 etsy-python-1.0.7/etsy_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-16 07:09:14.000000 etsy-python-1.0.7/etsy_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 07:09:14.000000 etsy-python-1.0.7/etsy_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 07:09:14.000000 etsy-python-1.0.7/etsy_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-16 07:09:14.000000 etsy-python-1.0.7/etsy_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 07:09:14.806961 etsy-python-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-16 07:09:02.000000 etsy-python-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.766142 etsy-python-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-17 17:22:38.000000 etsy-python-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40498 2024-02-17 17:22:48.766142 etsy-python-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39731 2024-02-17 17:22:38.000000 etsy-python-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.754142 etsy-python-1.0.8/etsy_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.754142 etsy-python-1.0.8/etsy_python/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.754142 etsy-python-1.0.8/etsy_python/v3/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/auth/OAuth.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.758142 etsy-python-1.0.8/etsy_python/v3/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/common/Env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/common/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/common/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.758142 etsy-python-1.0.8/etsy_python/v3/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/Listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/ListingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/ShippingProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/ShopReceipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.758142 etsy-python-1.0.8/etsy_python/v3/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/exceptions/BaseAPIException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/exceptions/RequestException.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.762142 etsy-python-1.0.8/etsy_python/v3/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/FileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/ShippingProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/ShopReturnPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.766142 etsy-python-1.0.8/etsy_python/v3/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingOffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingTranslation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingVariationImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ListingVideo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/PaymentLedgerEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ReceiptTransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ShippingProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ShopProductionPartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ShopReturnPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/ShopSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/Taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/UserAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.766142 etsy-python-1.0.8/etsy_python/v3/resources/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/enums/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/enums/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/resources/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.766142 etsy-python-1.0.8/etsy_python/v3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:38.000000 etsy-python-1.0.8/etsy_python/v3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 17:22:48.766142 etsy-python-1.0.8/etsy_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40498 2024-02-17 17:22:48.000000 etsy-python-1.0.8/etsy_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-17 17:22:48.000000 etsy-python-1.0.8/etsy_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 17:22:48.000000 etsy-python-1.0.8/etsy_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-17 17:22:48.000000 etsy-python-1.0.8/etsy_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-17 17:22:48.000000 etsy-python-1.0.8/etsy_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 17:22:48.766142 etsy-python-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-17 17:22:38.000000 etsy-python-1.0.8/setup.py
```

### Comparing `etsy-python-1.0.7/LICENSE` & `etsy-python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/PKG-INFO` & `etsy-python-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etsy-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: Etsy API Client Library for Python
 Author: Amit Ray
 Author-email: mail@amitray.dev
 Project-URL: Documentation, https://github.com/amitray007/etsy-python-sdk/blob/master/README.md
 Project-URL: Source code, https://github.com/amitray007/etsy-python-sdk
 Project-URL: Issues, https://github.com/amitray007/etsy-python-sdk/issues
 Keywords: python,etsy,api
```

### Comparing `etsy-python-1.0.7/README.md` & `etsy-python-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/auth/OAuth.py` & `etsy-python-1.0.8/etsy_python/v3/auth/OAuth.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/common/Env.py` & `etsy-python-1.0.8/etsy_python/v3/common/Env.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/common/Utils.py` & `etsy-python-1.0.8/etsy_python/v3/common/Utils.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/enums/Listing.py` & `etsy-python-1.0.8/etsy_python/v3/enums/Listing.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/enums/ShippingProfile.py` & `etsy-python-1.0.8/etsy_python/v3/enums/ShippingProfile.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/Listing.py` & `etsy-python-1.0.8/etsy_python/v3/models/Listing.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/Receipt.py` & `etsy-python-1.0.8/etsy_python/v3/models/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/Request.py` & `etsy-python-1.0.8/etsy_python/v3/models/Request.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/ShippingProfile.py` & `etsy-python-1.0.8/etsy_python/v3/models/ShippingProfile.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/Shop.py` & `etsy-python-1.0.8/etsy_python/v3/models/Shop.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/ShopReturnPolicy.py` & `etsy-python-1.0.8/etsy_python/v3/models/ShopReturnPolicy.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/models/__init__.py` & `etsy-python-1.0.8/etsy_python/v3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Listing.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Listing.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingFile.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingFile.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingImage.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingImage.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingInventory.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingInventory.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingOffering.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingOffering.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingProduct.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingProduct.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingTranslation.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingTranslation.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingVariationImages.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingVariationImages.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ListingVideo.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ListingVideo.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Miscellaneous.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Payment.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Payment.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/PaymentLedgerEntry.py` & `etsy-python-1.0.8/etsy_python/v3/resources/PaymentLedgerEntry.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Receipt.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ReceiptTransactions.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ReceiptTransactions.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Review.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Review.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Session.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Session.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,16 +132,21 @@
                 response.headers["X-Remaining-This-Second"],
                 response.headers["X-Limit-Per-Day"],
                 response.headers["X-Remaining-Today"],
             )
 
         response_json = response.json()
         if is_error:
-            error_message = response_json.get("error")
-            error_description = response_json.get("error_description")
+            error_response = (
+                response_json
+                if isinstance(response_json, dict)
+                else dict(error=response_json)
+            )
+            error_message = error_response.get("error")
+            error_description = error_response.get("error_description")
             raise RequestException(
                 response.status_code,
                 error_message,
                 error_description,
                 rate_limits=rate_limits,
             )
         return Response(
```

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ShippingProfile.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ShippingProfile.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Shop.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Shop.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ShopProductionPartner.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ShopProductionPartner.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ShopReturnPolicy.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ShopReturnPolicy.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/ShopSection.py` & `etsy-python-1.0.8/etsy_python/v3/resources/ShopSection.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/Taxonomy.py` & `etsy-python-1.0.8/etsy_python/v3/resources/Taxonomy.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/User.py` & `etsy-python-1.0.8/etsy_python/v3/resources/User.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/UserAddress.py` & `etsy-python-1.0.8/etsy_python/v3/resources/UserAddress.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python/v3/resources/__init__.py` & `etsy-python-1.0.8/etsy_python/v3/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/etsy_python.egg-info/PKG-INFO` & `etsy-python-1.0.8/etsy_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etsy-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: Etsy API Client Library for Python
 Author: Amit Ray
 Author-email: mail@amitray.dev
 Project-URL: Documentation, https://github.com/amitray007/etsy-python-sdk/blob/master/README.md
 Project-URL: Source code, https://github.com/amitray007/etsy-python-sdk
 Project-URL: Issues, https://github.com/amitray007/etsy-python-sdk/issues
 Keywords: python,etsy,api
```

### Comparing `etsy-python-1.0.7/etsy_python.egg-info/SOURCES.txt` & `etsy-python-1.0.8/etsy_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etsy-python-1.0.7/setup.py` & `etsy-python-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 DESCRIPTION = "Etsy API Client Library for Python"
 
 # Setting up
 setup(
     name="etsy-python",
     version=VERSION,
     author="Amit Ray",
```

