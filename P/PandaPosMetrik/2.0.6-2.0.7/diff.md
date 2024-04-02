# Comparing `tmp/PandaPosMetrik-2.0.6.tar.gz` & `tmp/PandaPosMetrik-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandaPosMetrik-2.0.6.tar", last modified: Tue Apr  2 13:24:02 2024, max compression
+gzip compressed data, was "PandaPosMetrik-2.0.7.tar", last modified: Tue Apr  2 13:27:03 2024, max compression
```

## Comparing `PandaPosMetrik-2.0.6.tar` & `PandaPosMetrik-2.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.375052 PandaPosMetrik-2.0.6/Metrik/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.0.6/Metrik/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.376803 PandaPosMetrik-2.0.6/Metrik/exceptions/
--rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.0.6/Metrik/exceptions/ObjectDoesNotExists.py
--rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.0.6/Metrik/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.383697 PandaPosMetrik-2.0.6/Metrik/models/
--rw-rw-rw-   0        0        0     1546 2024-04-02 13:18:26.000000 PandaPosMetrik-2.0.6/Metrik/models/ORMModel.py
--rw-rw-rw-   0        0        0     3205 2024-04-02 13:19:08.000000 PandaPosMetrik-2.0.6/Metrik/models/OrmManager.py
--rw-rw-rw-   0        0        0     2042 2024-04-02 13:23:41.000000 PandaPosMetrik-2.0.6/Metrik/models/Ticket.py
--rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.0.6/Metrik/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.383697 PandaPosMetrik-2.0.6/Metrik/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.0.6/Metrik/utils/__init__.py
--rw-rw-rw-   0        0        0       61 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/
--rw-rw-rw-   0        0        0       61 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-02 13:24:02.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      221 2024-04-02 13:23:46.000000 PandaPosMetrik-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.960098 PandaPosMetrik-2.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.916657 PandaPosMetrik-2.0.7/Metrik/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.0.7/Metrik/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.919024 PandaPosMetrik-2.0.7/Metrik/exceptions/
+-rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.0.7/Metrik/exceptions/ObjectDoesNotExists.py
+-rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.0.7/Metrik/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.929351 PandaPosMetrik-2.0.7/Metrik/models/
+-rw-rw-rw-   0        0        0     1546 2024-04-02 13:18:26.000000 PandaPosMetrik-2.0.7/Metrik/models/ORMModel.py
+-rw-rw-rw-   0        0        0     3205 2024-04-02 13:19:08.000000 PandaPosMetrik-2.0.7/Metrik/models/OrmManager.py
+-rw-rw-rw-   0        0        0     2073 2024-04-02 13:26:51.000000 PandaPosMetrik-2.0.7/Metrik/models/Ticket.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.0.7/Metrik/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.930765 PandaPosMetrik-2.0.7/Metrik/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.0.7/Metrik/utils/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-04-02 13:27:03.960098 PandaPosMetrik-2.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 13:27:03.959455 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-02 13:27:02.000000 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-02 13:27:03.000000 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:27:02.000000 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 13:27:03.000000 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 13:27:03.000000 PandaPosMetrik-2.0.7/PandaPosMetrik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:27:03.960098 PandaPosMetrik-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      221 2024-04-02 13:26:56.000000 PandaPosMetrik-2.0.7/setup.py
```

### Comparing `PandaPosMetrik-2.0.6/Metrik/models/ORMModel.py` & `PandaPosMetrik-2.0.7/Metrik/models/ORMModel.py`

 * *Files identical despite different names*

### Comparing `PandaPosMetrik-2.0.6/Metrik/models/OrmManager.py` & `PandaPosMetrik-2.0.7/Metrik/models/OrmManager.py`

 * *Files identical despite different names*

### Comparing `PandaPosMetrik-2.0.6/Metrik/models/Ticket.py` & `PandaPosMetrik-2.0.7/Metrik/models/Ticket.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     ExchangeRate: float
     TaxIncluded: bool
     Name: str
     TransactionDocument_Id: int
     IsOpened: bool
     TotalAmountPreTax: float
     orders: list[Order]
+    payments: list['Payment']
     Status: int
     
 
 class Payment(Model):
     Id: int
     TicketId: int
     PaymentTypeId: int
```

