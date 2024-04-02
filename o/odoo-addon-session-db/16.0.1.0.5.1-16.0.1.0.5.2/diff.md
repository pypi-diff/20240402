# Comparing `tmp/odoo_addon_session_db-16.0.1.0.5.1-py3-none-any.whl.zip` & `tmp/odoo_addon_session_db-16.0.1.0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 23711 bytes, number of entries: 16
--rw-r--r--  2.0 unx     3585 b- defN 23-Sep-03 16:49 odoo/addons/session_db/README.rst
--rw-r--r--  2.0 unx       31 b- defN 23-Sep-03 16:49 odoo/addons/session_db/__init__.py
--rw-r--r--  2.0 unx      251 b- defN 23-Sep-03 16:49 odoo/addons/session_db/__manifest__.py
--rw-r--r--  2.0 unx     4726 b- defN 23-Sep-03 16:49 odoo/addons/session_db/pg_session_store.py
--rw-r--r--  2.0 unx      341 b- defN 23-Sep-03 16:49 odoo/addons/session_db/i18n/session_db.pot
--rw-r--r--  2.0 unx      206 b- defN 23-Sep-03 16:49 odoo/addons/session_db/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx       83 b- defN 23-Sep-03 16:49 odoo/addons/session_db/readme/ROADMAP.rst
--rw-r--r--  2.0 unx      312 b- defN 23-Sep-03 16:49 odoo/addons/session_db/readme/USAGE.rst
--rw-r--r--  2.0 unx     9455 b- defN 23-Sep-03 16:49 odoo/addons/session_db/static/description/icon.png
--rw-r--r--  2.0 unx    13120 b- defN 23-Sep-03 16:49 odoo/addons/session_db/static/description/index.html
--rw-r--r--  2.0 unx       36 b- defN 23-Sep-03 16:49 odoo/addons/session_db/tests/__init__.py
--rw-r--r--  2.0 unx     3057 b- defN 23-Sep-03 16:49 odoo/addons/session_db/tests/test_pg_session_store.py
--rw-r--r--  2.0 unx     4131 b- defN 23-Sep-03 16:50 odoo_addon_session_db-16.0.1.0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-03 16:50 odoo_addon_session_db-16.0.1.0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Sep-03 16:50 odoo_addon_session_db-16.0.1.0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1565 b- defN 23-Sep-03 16:50 odoo_addon_session_db-16.0.1.0.5.1.dist-info/RECORD
-16 files, 40996 bytes uncompressed, 21031 bytes compressed:  48.7%
+Zip file size: 24160 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     3585 b- defN 24-Jan-20 06:26 odoo/addons/session_db/README.rst
+-rw-r--r--  2.0 unx       31 b- defN 24-Jan-20 06:26 odoo/addons/session_db/__init__.py
+-rw-r--r--  2.0 unx      251 b- defN 24-Jan-20 06:26 odoo/addons/session_db/__manifest__.py
+-rw-r--r--  2.0 unx     4726 b- defN 24-Jan-20 06:26 odoo/addons/session_db/pg_session_store.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Jan-20 06:26 odoo/addons/session_db/i18n/it.po
+-rw-r--r--  2.0 unx      341 b- defN 24-Jan-20 06:26 odoo/addons/session_db/i18n/session_db.pot
+-rw-r--r--  2.0 unx      206 b- defN 24-Jan-20 06:26 odoo/addons/session_db/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx       83 b- defN 24-Jan-20 06:26 odoo/addons/session_db/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx      312 b- defN 24-Jan-20 06:26 odoo/addons/session_db/readme/USAGE.rst
+-rw-r--r--  2.0 unx     9455 b- defN 24-Jan-20 06:26 odoo/addons/session_db/static/description/icon.png
+-rw-r--r--  2.0 unx    13120 b- defN 24-Jan-20 06:26 odoo/addons/session_db/static/description/index.html
+-rw-r--r--  2.0 unx       36 b- defN 24-Jan-20 06:26 odoo/addons/session_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3057 b- defN 24-Jan-20 06:26 odoo/addons/session_db/tests/test_pg_session_store.py
+-rw-r--r--  2.0 unx     4131 b- defN 24-Jan-20 06:26 odoo_addon_session_db-16.0.1.0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jan-20 06:26 odoo_addon_session_db-16.0.1.0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Jan-20 06:26 odoo_addon_session_db-16.0.1.0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1654 b- defN 24-Jan-20 06:26 odoo_addon_session_db-16.0.1.0.5.2.dist-info/RECORD
+17 files, 41496 bytes uncompressed, 21338 bytes compressed:  48.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: odoo/addons/session_db/__manifest__.py
 Comment: 
 
 Filename: odoo/addons/session_db/pg_session_store.py
 Comment: 
 
+Filename: odoo/addons/session_db/i18n/it.po
+Comment: 
+
 Filename: odoo/addons/session_db/i18n/session_db.pot
 Comment: 
 
 Filename: odoo/addons/session_db/readme/DESCRIPTION.rst
 Comment: 
 
 Filename: odoo/addons/session_db/readme/ROADMAP.rst
@@ -30,20 +33,20 @@
 
 Filename: odoo/addons/session_db/tests/__init__.py
 Comment: 
 
 Filename: odoo/addons/session_db/tests/test_pg_session_store.py
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.5.1.dist-info/METADATA
+Filename: odoo_addon_session_db-16.0.1.0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.5.1.dist-info/WHEEL
+Filename: odoo_addon_session_db-16.0.1.0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.5.1.dist-info/top_level.txt
+Filename: odoo_addon_session_db-16.0.1.0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.5.1.dist-info/RECORD
+Filename: odoo_addon_session_db-16.0.1.0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addon_session_db-16.0.1.0.5.1.dist-info/METADATA` & `odoo_addon_session_db-16.0.1.0.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-session-db
-Version: 16.0.1.0.5.1
+Version: 16.0.1.0.5.2
 Summary: Store sessions in DB
 Home-page: https://github.com/OCA/server-tools
 Author: Odoo SA,ACSONE SA/NV,Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_session_db-16.0.1.0.5.1.dist-info/RECORD` & `odoo_addon_session_db-16.0.1.0.5.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 odoo/addons/session_db/README.rst,sha256=GTcBUz3EC3eHxANlF-K3wrviVKiKjV3QLAupW5ED0Os,3585
 odoo/addons/session_db/__init__.py,sha256=PVM3bucL2EzItoVUqRcC9hplW7KuhmOTCjv6leqVXWQ,31
 odoo/addons/session_db/__manifest__.py,sha256=ZkG8DZRsV4QTlgCjF84lriUpihTKv1mLl1IbvvhK4Fo,251
 odoo/addons/session_db/pg_session_store.py,sha256=Jlk8nUXM0FvXI2Ik_H2VP-Zw2EsjE9UU29_cbDb4a8o,4726
+odoo/addons/session_db/i18n/it.po,sha256=70bJ8f0IgeWxthAa8dpCCJ2VujuUWH7uSpJBUnYo8GI,411
 odoo/addons/session_db/i18n/session_db.pot,sha256=leB6MlaWiU1sPOdcOTxNVY5KVORnHv0MfD14HgQJIIs,341
 odoo/addons/session_db/readme/DESCRIPTION.rst,sha256=d84Ye-2qA3Vb3-CKkhLDgPrwDzLYcGSHpwsKDqmwDdA,206
 odoo/addons/session_db/readme/ROADMAP.rst,sha256=tjuz6o7GPU_OvBRxMrjauZZ_o_4nBoNy9ZcmEuS-agk,83
 odoo/addons/session_db/readme/USAGE.rst,sha256=3mtjrhdBiktzD_z1Elmw1NAIv5zzjCiXScf7nFPTeO8,312
 odoo/addons/session_db/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/session_db/static/description/index.html,sha256=MjrU48U_623_yrbP7gvpcFJefpIVr6QJH2VSJ9P8LJ4,13120
 odoo/addons/session_db/tests/__init__.py,sha256=T3ue0WvaufnQmExTwvSf9HF6U__NPpbi8HudWcRwTA4,36
 odoo/addons/session_db/tests/test_pg_session_store.py,sha256=1ytD1TOE9pcOAP74BOKa2Gp211T47Tyn567YKN5PKkY,3057
-odoo_addon_session_db-16.0.1.0.5.1.dist-info/METADATA,sha256=RsyzNcmnV2rx_ET4z1kbEzFHhd5793rcQoiYbxhh4lE,4131
-odoo_addon_session_db-16.0.1.0.5.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-odoo_addon_session_db-16.0.1.0.5.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_session_db-16.0.1.0.5.1.dist-info/RECORD,,
+odoo_addon_session_db-16.0.1.0.5.2.dist-info/METADATA,sha256=5a9ChYOpW0THhKiJDO0g8x46aCFH6jnpRrU79pJJq7s,4131
+odoo_addon_session_db-16.0.1.0.5.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo_addon_session_db-16.0.1.0.5.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_session_db-16.0.1.0.5.2.dist-info/RECORD,,
```

