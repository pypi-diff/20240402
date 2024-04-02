# Comparing `tmp/ookcatalog-0.2.0.tar.gz` & `tmp/ookcatalog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ookcatalog-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ookcatalog-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ookcatalog-0.2.0.tar` & `ookcatalog-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6567 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/README.md
--rw-r--r--   0        0        0     2039 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/ookcatalog/__init__.py
--rw-r--r--   0        0        0     1651 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/ookcatalog/catalog.py
--rw-r--r--   0        0        0     3549 2024-03-24 17:14:54.231014 ookcatalog-0.2.0/ookcatalog/commands.py
--rw-r--r--   0        0        0    19204 2024-04-01 13:09:11.388778 ookcatalog-0.2.0/ookcatalog/db.py
--rw-r--r--   0        0        0     1673 2024-04-01 11:03:40.686560 ookcatalog-0.2.0/ookcatalog/templates/home.html
--rw-r--r--   0        0        0     1736 2024-04-01 10:23:07.451392 ookcatalog-0.2.0/ookcatalog/templates/layout.html
--rw-r--r--   0        0        0      791 2024-03-21 20:22:07.828265 ookcatalog-0.2.0/ookcatalog/templates/search.html
--rw-r--r--   0        0        0     1770 2024-03-22 18:53:21.298932 ookcatalog-0.2.0/ookcatalog/templates/table.html
--rw-r--r--   0        0        0     1653 2024-03-24 14:39:13.706038 ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2693 2024-03-24 14:39:04.366052 ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      742 2024-04-01 13:13:04.482602 ookcatalog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7142 1970-01-01 00:00:00.000000 ookcatalog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6567 2024-03-25 22:00:50.388439 ookcatalog-0.2.1/README.md
+-rw-r--r--   0        0        0     2039 2024-03-25 22:00:50.388439 ookcatalog-0.2.1/ookcatalog/__init__.py
+-rw-r--r--   0        0        0     1651 2024-03-25 22:00:50.388439 ookcatalog-0.2.1/ookcatalog/catalog.py
+-rw-r--r--   0        0        0     3549 2024-03-24 17:14:54.231014 ookcatalog-0.2.1/ookcatalog/commands.py
+-rw-r--r--   0        0        0    19252 2024-04-02 16:21:27.974022 ookcatalog-0.2.1/ookcatalog/db.py
+-rw-r--r--   0        0        0     1673 2024-04-01 11:03:40.686560 ookcatalog-0.2.1/ookcatalog/templates/home.html
+-rw-r--r--   0        0        0     1736 2024-04-01 10:23:07.451392 ookcatalog-0.2.1/ookcatalog/templates/layout.html
+-rw-r--r--   0        0        0      791 2024-03-21 20:22:07.828265 ookcatalog-0.2.1/ookcatalog/templates/search.html
+-rw-r--r--   0        0        0     1770 2024-03-22 18:53:21.298932 ookcatalog-0.2.1/ookcatalog/templates/table.html
+-rw-r--r--   0        0        0     1653 2024-03-24 14:39:13.706038 ookcatalog-0.2.1/ookcatalog/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2693 2024-03-24 14:39:04.366052 ookcatalog-0.2.1/ookcatalog/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      742 2024-04-02 16:24:19.649675 ookcatalog-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7142 1970-01-01 00:00:00.000000 ookcatalog-0.2.1/PKG-INFO
```

### Comparing `ookcatalog-0.2.0/README.md` & `ookcatalog-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/__init__.py` & `ookcatalog-0.2.1/ookcatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/catalog.py` & `ookcatalog-0.2.1/ookcatalog/catalog.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/commands.py` & `ookcatalog-0.2.1/ookcatalog/commands.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/db.py` & `ookcatalog-0.2.1/ookcatalog/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
     """
     with db.cursor() as cur:
         # Reading the schemas from the information schema
         cur.execute(
             """
             SELECT table_schema                                                   as schema_name,
                    obj_description(to_regnamespace(table_schema), 'pg_namespace') as schema_description,
-                   array_agg(array [table_name, obj_description(to_regclass(table_schema || '.' || table_name), 'pg_class')]
+                   array_agg(array [table_name::text,
+                                    obj_description(to_regclass(table_schema || '.' || table_name), 'pg_class')::text]
                              order by table_name)::text[][]                       as tables
             FROM information_schema.tables
             WHERE table_schema NOT IN ('information_schema', 'pg_catalog', 'topology')
             GROUP BY schema_name
             ORDER BY schema_name;
             """
         )
```

### Comparing `ookcatalog-0.2.0/ookcatalog/templates/home.html` & `ookcatalog-0.2.1/ookcatalog/templates/home.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/templates/layout.html` & `ookcatalog-0.2.1/ookcatalog/templates/layout.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/templates/search.html` & `ookcatalog-0.2.1/ookcatalog/templates/search.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/templates/table.html` & `ookcatalog-0.2.1/ookcatalog/templates/table.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.mo` & `ookcatalog-0.2.1/ookcatalog/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.po` & `ookcatalog-0.2.1/ookcatalog/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.2.0/pyproject.toml` & `ookcatalog-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ookcatalog"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Moté", email="automates@petitmote.fr"}
 ]
 description = "Light and hassle-free PostgreSQL data catalog"
 readme = "README.md"
 licens = {file = "LICENSE.txt"}
 requires-python = ">=3.8"
```

### Comparing `ookcatalog-0.2.0/PKG-INFO` & `ookcatalog-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ookcatalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: Light and hassle-free PostgreSQL data catalog
 Author-email: Moté <automates@petitmote.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

