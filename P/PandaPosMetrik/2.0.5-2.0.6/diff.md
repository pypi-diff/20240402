# Comparing `tmp/PandaPosMetrik-2.0.5.tar.gz` & `tmp/PandaPosMetrik-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandaPosMetrik-2.0.5.tar", last modified: Tue Mar 19 12:39:35 2024, max compression
+gzip compressed data, was "PandaPosMetrik-2.0.6.tar", last modified: Tue Apr  2 13:24:02 2024, max compression
```

## Comparing `PandaPosMetrik-2.0.5.tar` & `PandaPosMetrik-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.282295 PandaPosMetrik-2.0.5/
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.243818 PandaPosMetrik-2.0.5/Metrik/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.0.5/Metrik/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.246814 PandaPosMetrik-2.0.5/Metrik/exceptions/
--rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.0.5/Metrik/exceptions/ObjectDoesNotExists.py
--rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.0.5/Metrik/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.255841 PandaPosMetrik-2.0.5/Metrik/models/
--rw-rw-rw-   0        0        0     1089 2024-03-19 12:35:07.000000 PandaPosMetrik-2.0.5/Metrik/models/ORMModel.py
--rw-rw-rw-   0        0        0     3184 2024-03-19 12:39:22.000000 PandaPosMetrik-2.0.5/Metrik/models/OrmManager.py
--rw-rw-rw-   0        0        0     1586 2024-03-19 12:29:35.000000 PandaPosMetrik-2.0.5/Metrik/models/Ticket.py
--rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.0.5/Metrik/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.256842 PandaPosMetrik-2.0.5/Metrik/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.0.5/Metrik/utils/__init__.py
--rw-rw-rw-   0        0        0       61 2024-03-19 12:39:35.282295 PandaPosMetrik-2.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 12:39:35.282295 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/
--rw-rw-rw-   0        0        0       61 2024-03-19 12:39:34.000000 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-03-19 12:39:35.000000 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:39:34.000000 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-19 12:39:34.000000 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-19 12:39:34.000000 PandaPosMetrik-2.0.5/PandaPosMetrik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 12:39:35.282295 PandaPosMetrik-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      221 2024-03-19 12:39:29.000000 PandaPosMetrik-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.375052 PandaPosMetrik-2.0.6/Metrik/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.0.6/Metrik/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.376803 PandaPosMetrik-2.0.6/Metrik/exceptions/
+-rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.0.6/Metrik/exceptions/ObjectDoesNotExists.py
+-rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.0.6/Metrik/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.383697 PandaPosMetrik-2.0.6/Metrik/models/
+-rw-rw-rw-   0        0        0     1546 2024-04-02 13:18:26.000000 PandaPosMetrik-2.0.6/Metrik/models/ORMModel.py
+-rw-rw-rw-   0        0        0     3205 2024-04-02 13:19:08.000000 PandaPosMetrik-2.0.6/Metrik/models/OrmManager.py
+-rw-rw-rw-   0        0        0     2042 2024-04-02 13:23:41.000000 PandaPosMetrik-2.0.6/Metrik/models/Ticket.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.0.6/Metrik/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.383697 PandaPosMetrik-2.0.6/Metrik/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.0.6/Metrik/utils/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-02 13:24:02.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 13:24:01.000000 PandaPosMetrik-2.0.6/PandaPosMetrik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:24:02.419135 PandaPosMetrik-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      221 2024-04-02 13:23:46.000000 PandaPosMetrik-2.0.6/setup.py
```

### Comparing `PandaPosMetrik-2.0.5/Metrik/models/OrmManager.py` & `PandaPosMetrik-2.0.6/Metrik/models/OrmManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         
         return self
 
     def create(self, **kwargs) -> T:
         cursor = self.connection.cursor()
         
         sql = f"""
-        INSERT INTO {self.owner} ({', '.join(list(kwargs.keys()))}) VALUES ({', '.join(['?']*len(kwargs))})
+        INSERT INTO {self.owner.__tablename_plural__} ({', '.join(list(kwargs.keys()))}) VALUES ({', '.join(['?']*len(kwargs))})
         """
         
         
         cursor.execute(sql, list(kwargs.values()))
         cursor.commit()
         return self.owner(**kwargs)
```

### Comparing `PandaPosMetrik-2.0.5/Metrik/models/Ticket.py` & `PandaPosMetrik-2.0.6/Metrik/models/Ticket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 from Metrik.models.ORMModel import Model
 
 
-class Orders(Model):
+class Order(Model):
     Id: int
     TicketId: int
     WarehouseId: int
     DepartmentId: int
     TerminalId: int
     MenuItemId: int
     MenuItemName: str
@@ -33,15 +33,15 @@
     DisablePortionSelection: bool
     OrderUid: str
     Taxes: str
     OrderTags: str
     OrderStates: str
     
 
-class Tickets(Model):
+class Ticket(Model):
     Id: int
     LastUpdateTime: datetime.datetime
     TicketVersion: datetime.datetime
     TicketUid: str
     TicketNumber: str
     Date: datetime.datetime
     LastOrderDate: datetime.datetime
@@ -62,11 +62,32 @@
     LineSeparators: str
     ExchangeRate: float
     TaxIncluded: bool
     Name: str
     TransactionDocument_Id: int
     IsOpened: bool
     TotalAmountPreTax: float
-    orders: list[Orders]
+    orders: list[Order]
     Status: int
     
 
+class Payment(Model):
+    Id: int
+    TicketId: int
+    PaymentTypeId: int
+    DepartmentId: int
+    Name: str
+    Description: str
+    Date: datetime.datetime
+    AccountTransactionId: int
+    Amount: float
+    TenderedAmount: float
+    UserId: int
+    TerminalId: int
+    ExchangeRate: float
+    PaymentData: str
+    CanAdjustTip: bool
+    AccountTransactionId: int
+    AccountTransaction_AccountTransactionDocumentId: int
+    
+    
+
```

