# Comparing `tmp/zephony-1.3.1.tar.gz` & `tmp/zephony-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-1.3.1.tar", last modified: Fri Dec 29 07:24:04 2023, max compression
+gzip compressed data, was "zephony-1.4.tar", last modified: Tue Apr  2 11:15:42 2024, max compression
```

## Comparing `zephony-1.3.1.tar` & `zephony-1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 07:24:04.895249 zephony-1.3.1/
--rw-r--r--   0 root         (0) root         (0)      276 2023-12-29 07:24:04.895249 zephony-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2023-12-29 07:23:49.000000 zephony-1.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2023-12-29 07:24:04.895249 zephony-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      408 2023-12-29 07:23:49.000000 zephony-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 07:24:04.895249 zephony-1.3.1/zephony/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18046 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 07:24:04.895249 zephony-1.3.1/zephony/models/
--rw-r--r--   0 root         (0) root         (0)    40257 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7377 2023-12-29 07:23:49.000000 zephony-1.3.1/zephony/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 07:24:04.895249 zephony-1.3.1/zephony.egg-info/
--rw-r--r--   0 root         (0) root         (0)      276 2023-12-29 07:24:04.000000 zephony-1.3.1/zephony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2023-12-29 07:24:04.000000 zephony-1.3.1/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-29 07:24:04.000000 zephony-1.3.1/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-29 07:24:04.000000 zephony-1.3.1/zephony.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-12-29 07:24:04.000000 zephony-1.3.1/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.270118 zephony-1.4/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-02 11:15:42.266118 zephony-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-02 11:15:23.000000 zephony-1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-02 11:15:42.270118 zephony-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-02 11:15:23.000000 zephony-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 11:15:23.000000 zephony-1.4/zephony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-04-02 11:15:23.000000 zephony-1.4/zephony/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-02 11:15:23.000000 zephony-1.4/zephony/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2024-04-02 11:15:23.000000 zephony-1.4/zephony/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony/models/
+-rw-r--r--   0 root         (0) root         (0)    40794 2024-04-02 11:15:23.000000 zephony-1.4/zephony/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2024-04-02 11:15:23.000000 zephony-1.4/zephony/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/top_level.txt
```

### Comparing `zephony-1.3.1/zephony/decorators.py` & `zephony-1.4/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-1.3.1/zephony/exceptions.py` & `zephony-1.4/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-1.3.1/zephony/helpers.py` & `zephony-1.4/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-1.3.1/zephony/models/__init__.py` & `zephony-1.4/zephony/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -927,16 +927,14 @@
         even when a join is not required - might have to fix it later if we
         notice any performance issue).
 
         Ref: https://stackoverflow.com/questions/15897055
         ChatGPT for SQLAlchemy version
         """
 
-        ic('+++++++++++++++++++++')
-
         # q = cls.query
         sub_query = db.session.query(cls.id_)
 
         # Filters related
         if 'is_deleted' not in filters:
             filters['is_deleted'] = False
 
@@ -962,22 +960,31 @@
             )
 
         sub_query = sub_query.subquery('parent_subquery')
         parent_alias = aliased(cls, sub_query)
 
         q = db.session.query(cls).join(sub_query, cls.id_==sub_query.c.id_)
 
-        # Normal joins
-        for join in joins:
+        # NX1 joins (aka. normal joins)
+        for i, join in enumerate(joins):
+            # This alias is required so that if there are multiple columns
+            # being joined to the same table, SQLAlchemy knows which column
+            # join is which.
+            # 
+            # Regarding the naming of the alias, we're just using the model's
+            # class name and joining it with the foreign key column, separated
+            # by an underscore.
+            aliased_model = aliased(join[0], name=f'{join[0].__name__}_{join[1]}')
             q = (
-                q.outerjoin(join[0], getattr(cls, join[1])==join[0].id_)
-                .add_entity(join[0])
+                q.outerjoin(aliased_model, getattr(cls, join[1])==aliased_model.id_)
+                .add_entity(aliased_model)
             )
 
-        # Bridge joins - Join bridge first and then the secondary table
+        # NXN joins - aka. Bridge joins
+        # Join bridge first and then the secondary table
         for join in bridge_joins:
             q = (
                 q.outerjoin(
                     join['bridge_model'],
                     and_(
                         cls.id_==getattr(join['bridge_model'], join['bridge_primary_id']),
                         or_(
@@ -990,15 +997,15 @@
                     join['secondary_model'],
                     getattr(join['bridge_model'], join['bridge_secondary_id'])==join['secondary_model'].id_,
                 )
                 .add_entity(join['bridge_model'])
                 .add_entity(join['secondary_model'])
             )
 
-        # 1XN joins
+        # 1XN joins (aka. list joins)
         for join in list_joins:
             q = (
                 q.outerjoin(
                     join['secondary_model'],
                     and_(
                         cls.id_==getattr(join['secondary_model'], join['back_reference']),
                         or_(
@@ -1088,15 +1095,15 @@
                     secondary_object_details = secondary_object.get_details()
 
                     details[list_join['details_list_key']].append(
                         secondary_object_details
                     )
 
             for join in joins:
-                joined_object = getattr(result, join[0].__name__)
+                joined_object = getattr(result, f'{join[0].__name__}_{join[1]}')
 
                 if joined_object is not None:
                     details[join[2]] = joined_object.get_details()
                 else:
                     details[join[2]] = None
 
         for primary_id, details in primary_objects_map.items():
```

### Comparing `zephony-1.3.1/zephony/validators.py` & `zephony-1.4/zephony/validators.py`

 * *Files identical despite different names*

