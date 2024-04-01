# Comparing `tmp/heaobject-1.1.0.tar.gz` & `tmp/heaobject-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.1.0.tar", last modified: Tue Mar 26 22:40:34 2024, max compression
+gzip compressed data, was "heaobject-1.1.1.tar", last modified: Mon Apr  1 23:31:21 2024, max compression
```

## Comparing `heaobject-1.1.0.tar` & `heaobject-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 22:40:34.196409 heaobject-1.1.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4041 2024-03-26 22:40:34.195409 heaobject-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2579 2024-03-22 23:46:04.000000 heaobject-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 22:40:34.196409 heaobject-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2550 2024-03-26 22:39:42.000000 heaobject-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 22:40:34.141394 heaobject-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-26 22:40:34.186410 heaobject-1.1.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15432 2024-01-04 00:00:42.000000 heaobject-1.1.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7499 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9306 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.1.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.1.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.1.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    21224 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4482 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     6696 2024-03-21 03:37:53.000000 heaobject-1.1.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0     7609 2024-03-22 21:50:49.000000 heaobject-1.1.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5045 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.1.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      130 2022-03-11 01:28:08.000000 heaobject-1.1.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24503 2024-03-19 23:51:31.000000 heaobject-1.1.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    73075 2024-03-21 03:37:53.000000 heaobject-1.1.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      505 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-22 18:21:47.000000 heaobject-1.1.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     3994 2023-12-22 03:29:41.000000 heaobject-1.1.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0     9591 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-22 18:59:54.000000 heaobject-1.1.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     5802 2023-12-16 22:23:08.000000 heaobject-1.1.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-03-26 22:40:34.194410 heaobject-1.1.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4041 2024-03-26 22:40:34.000000 heaobject-1.1.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-03-26 22:40:34.000000 heaobject-1.1.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 22:40:34.000000 heaobject-1.1.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-03-26 22:40:34.000000 heaobject-1.1.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-26 22:40:34.000000 heaobject-1.1.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.578748 heaobject-1.1.1/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4251 2024-04-01 23:31:21.577748 heaobject-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2789 2024-03-29 22:37:21.000000 heaobject-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 23:31:21.578748 heaobject-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2550 2024-04-01 23:29:58.000000 heaobject-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.521659 heaobject-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.568697 heaobject-1.1.1/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15432 2024-01-04 00:00:42.000000 heaobject-1.1.1/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7499 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9306 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    21224 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4482 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     6790 2024-03-30 04:52:01.000000 heaobject-1.1.1/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0     7609 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5045 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      130 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24503 2024-03-19 23:51:31.000000 heaobject-1.1.1/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    73318 2024-03-29 00:46:01.000000 heaobject-1.1.1/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      505 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     3994 2023-12-22 03:29:41.000000 heaobject-1.1.1/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0     9591 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     5802 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.576748 heaobject-1.1.1/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4251 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.1.0/LICENSE` & `heaobject-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/PKG-INFO` & `heaobject-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.1.0
+Version: 1.1.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,18 @@
 Requires-Dist: python-dateutil~=2.8.2
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.1.1
+* Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
+should replace CHECK_DYNAMIC with any dynamically computed permissions).
+
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
 * Added source module with system source names (previously was only in heaserver).
 
 ## Version 1.0.2
 * More performance improvements converting to/from a HEAObject and a dictionary.
```

### Comparing `heaobject-1.1.0/README.md` & `heaobject-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.1.1
+* Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
+should replace CHECK_DYNAMIC with any dynamically computed permissions).
+
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
 * Added source module with system source names (previously was only in heaserver).
 
 ## Version 1.0.2
 * More performance improvements converting to/from a HEAObject and a dictionary.
```

### Comparing `heaobject-1.1.0/setup.py` & `heaobject-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.1.0',
+                 version='1.1.1',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.1.0/src/heaobject/__init__.py` & `heaobject-1.1.1/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/account.py` & `heaobject-1.1.1/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/activity.py` & `heaobject-1.1.1/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/aws.py` & `heaobject-1.1.1/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/awss3key.py` & `heaobject-1.1.1/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/bucket.py` & `heaobject-1.1.1/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/data.py` & `heaobject-1.1.1/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/dataadapter.py` & `heaobject-1.1.1/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/datamodel.py` & `heaobject-1.1.1/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/folder.py` & `heaobject-1.1.1/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/keychain.py` & `heaobject-1.1.1/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/organization.py` & `heaobject-1.1.1/src/heaobject/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from heaobject.root import Permission, ShareImpl
 from heaobject.data import DataObject, SameMimeType
 from collections.abc import Iterable, Iterator
 from typing import Optional
 
 permission_id_dict = {
     'admin_ids': [Permission.COOWNER],
-    'manager_ids': [Permission.VIEWER, Permission.CREATOR, Permission.EDITOR, Permission.SHARER, Permission.DELETER],
-    'member_ids': [Permission.VIEWER, Permission.EDITOR, Permission.SHARER]
+    'manager_ids': [Permission.VIEWER, Permission.EDITOR, Permission.SHARER, Permission.DELETER],
+    'member_ids': [Permission.VIEWER, Permission.SHARER]
 }
 
 
 class Organization(DataObject, SameMimeType):
     """
     Represents a directory in the HEA desktop.
     """
@@ -169,14 +169,17 @@
         Returns permissions if the sub is in the member_ids list, or an empty list if not.
 
         :param sub: the user id (required).
         :return: A list containing Permissions or the empty list.
         """
         try:
             perms: set[Permission] = set()
-            for p_id in permission_id_dict:
-                if sub in getattr(self, p_id):
-                    perms.update(permission_id_dict[p_id])
+            if sub == self.principal_investigator_id:
+                perms.add(Permission.COOWNER)
+            else:
+                for p_id in permission_id_dict:
+                    if sub in getattr(self, p_id):
+                        perms.update(permission_id_dict[p_id])
             return list(perms)
         except:
             logging.exception('Permissions are not correctly configured...returning empty permissions set')
             return []
```

### Comparing `heaobject-1.1.0/src/heaobject/person.py` & `heaobject-1.1.1/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/project.py` & `heaobject-1.1.1/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/registry.py` & `heaobject-1.1.1/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/root.py` & `heaobject-1.1.1/src/heaobject/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,17 @@
         :return: a list of Permission enum values, or an empty list to signify no permissions.
         """
         pass
 
     @abc.abstractmethod
     def get_permissions(self, sub: str) -> List[Permission]:
         """
-        Gets the subject's permissions for this object.
+        Gets the subject's permissions for this object. The result includes any permissions computed dynamically if
+        the subject has the CHECK_DYNAMIC permission for the object, omitting CHECK_DYNAMIC in the returned permission
+        list.
 
         :param sub: the user (required).
         :return: a list of Permission enum values, or an empty list to signify no permissions.
         """
         pass
 
     @abc.abstractmethod
@@ -1318,15 +1320,15 @@
         if self.owner == sub:
             return list(p for p in Permission)
 
         result = set(perm for share in self.__shares for perm in share.permissions
                      if share.user == sub or share.user == ALL_USERS)
         if Permission.CHECK_DYNAMIC in result:
             result.update(self.dynamic_permission(sub))
-        return list(result)
+        return list(r for r in result if r is not Permission.CHECK_DYNAMIC)
 
     def has_permissions(self, sub: str, perms: Sequence[Permission] | PermissionGroup) -> bool:
         if sub is None:
             raise ValueError('sub cannot be None')
         if perms is None:
             raise ValueError('perms cannot be None')
```

### Comparing `heaobject-1.1.0/src/heaobject/source2target.py` & `heaobject-1.1.1/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/storage.py` & `heaobject-1.1.1/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/trash.py` & `heaobject-1.1.1/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/user.py` & `heaobject-1.1.1/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject/volume.py` & `heaobject-1.1.1/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.1.1/src/heaobject.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.1.0
+Version: 1.1.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,18 @@
 Requires-Dist: python-dateutil~=2.8.2
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.1.1
+* Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
+should replace CHECK_DYNAMIC with any dynamically computed permissions).
+
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
 * Added source module with system source names (previously was only in heaserver).
 
 ## Version 1.0.2
 * More performance improvements converting to/from a HEAObject and a dictionary.
```

### Comparing `heaobject-1.1.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.1.1/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

