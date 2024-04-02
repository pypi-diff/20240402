# Comparing `tmp/heaserver-organizations-1.0.2.tar.gz` & `tmp/heaserver-organizations-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-organizations-1.0.2.tar", last modified: Thu Mar 21 23:25:26 2024, max compression
+gzip compressed data, was "heaserver-organizations-1.1.0.tar", last modified: Tue Apr  2 21:16:58 2024, max compression
```

## Comparing `heaserver-organizations-1.0.2.tar` & `heaserver-organizations-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.573277 heaserver-organizations-1.0.2/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver-organizations-1.0.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver-organizations-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4740 2024-03-21 23:25:26.572277 heaserver-organizations-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3350 2024-03-19 20:57:21.000000 heaserver-organizations-1.0.2/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/RELEASING.md
--rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver-organizations-1.0.2/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.419243 heaserver-organizations-1.0.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.419243 heaserver-organizations-1.0.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.504276 heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10600 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    14644 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-21 23:25:26.574277 heaserver-organizations-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1911 2024-03-21 23:24:45.000000 heaserver-organizations-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.421242 heaserver-organizations-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.420242 heaserver-organizations-1.0.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.517278 heaserver-organizations-1.0.2/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.0.2/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    28104 2024-03-21 00:29:59.000000 heaserver-organizations-1.0.2/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.526277 heaserver-organizations-1.0.2/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    22356 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.571276 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     4740 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 23:25:26.000000 heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.421242 heaserver-organizations-1.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.422242 heaserver-organizations-1.0.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:25:26.569275 heaserver-organizations-1.0.2/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.0.2/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     6736 2023-12-18 21:21:27.000000 heaserver-organizations-1.0.2/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.433461 heaserver-organizations-1.1.0/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4812 2024-04-02 21:16:58.432460 heaserver-organizations-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3422 2024-04-02 21:14:43.000000 heaserver-organizations-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver-organizations-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.249726 heaserver-organizations-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.250314 heaserver-organizations-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.354195 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10600 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    14644 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 21:16:58.433461 heaserver-organizations-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2024-04-02 21:15:46.000000 heaserver-organizations-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.252311 heaserver-organizations-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.251312 heaserver-organizations-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.366250 heaserver-organizations-1.1.0/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    29224 2024-03-28 18:53:37.000000 heaserver-organizations-1.1.0/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.379253 heaserver-organizations-1.1.0/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    22622 2024-03-28 17:02:30.000000 heaserver-organizations-1.1.0/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.431460 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     4812 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.252311 heaserver-organizations-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.253311 heaserver-organizations-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.429459 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     6736 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver-organizations-1.0.2/Dockerfile` & `heaserver-organizations-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/LICENSE` & `heaserver-organizations-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/PKG-INFO` & `heaserver-organizations-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.0.2
+Version: 1.1.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-organizations-1.0.2/README.md` & `heaserver-organizations-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-organizations-1.0.2/RELEASING.md` & `heaserver-organizations-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/run-swaggerui.py` & `heaserver-organizations-1.1.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/setup.py` & `heaserver-organizations-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.0.2',
+    version='1.1.0',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.0.8'],
+    install_requires=['heaserver~=1.1.2'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-organizations-1.0.2/src/heaserver/organization/service.py` & `heaserver-organizations-1.1.0/src/heaserver/organization/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 The HEA Server Organization provides ...
 """
 import asyncio
 
 from aiohttp import hdrs
+from heaobject.error import DeserializeException
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import mongo, mongoservicelib
 from heaserver.service.wstl import builder_factory, action
 from heaserver.service.appproperty import HEA_DB
 from heaserver.service.oidcclaimhdrs import SUB
-from heaserver.service.heaobjectsupport import type_to_resource_url
+from heaserver.service.heaobjectsupport import type_to_resource_url, new_heaobject_from_type
 from heaserver.service import response, client
 from heaobject.organization import Organization
 from heaobject.account import AWSAccount
 from heaobject.volume import AWSFileSystem, Volume
 from heaobject.person import Person
-from heaobject.root import DesktopObjectDict
-from heaobject.project import AWSS3Project
+from heaobject.user import NONE_USER
 from collections.abc import AsyncGenerator
 from yarl import URL
 from asyncio import gather
 from itertools import chain
 from functools import partial
 import logging
 
@@ -582,14 +582,35 @@
       '204':
         $ref: '#/components/responses/204'
       '400':
         $ref: '#/components/responses/400'
       '404':
         $ref: '#/components/responses/404'
     """
+    sub = request.headers.get(SUB, NONE_USER)
+    old = await mongoservicelib.get_dict(request, MONGODB_ORGANIZATION_COLLECTION)
+    if old is not None:
+        old_org = Organization()
+        old_org.from_dict(old)
+        try:
+            new_org = await new_heaobject_from_type(request, Organization)
+        except DeserializeException as e:
+            return response.status_bad_request(str(e))
+        if old_org.admin_ids != new_org.admin_ids and \
+            sub != old_org.owner and \
+            sub != old_org.principal_investigator_id and \
+            sub not in old_org.admin_ids:
+            return response.status_bad_request('You have insufficient permissions to change the administrator list')
+        if old_org.manager_ids != new_org.manager_ids and \
+            sub != old_org.owner and \
+            sub != old_org.principal_investigator_id and \
+            sub not in old_org.manager_ids and \
+            sub not in old_org.admin_ids:
+            return response.status_bad_request('You have insufficient permissions to change the manager list')
+
     return await mongoservicelib.put(request, MONGODB_ORGANIZATION_COLLECTION, Organization)
 
 
 @routes.delete('/organizations/{id}')
 async def delete_organization(request: web.Request) -> web.Response:
     """
     Deletes the organization with the specified id.
```

### Comparing `heaserver-organizations-1.0.2/src/heaserver/organization/wstl/all.json` & `heaserver-organizations-1.1.0/src/heaserver/organization/wstl/all.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999964077066011%*

 * *Differences: {"'wstl'": "{'actions': {7: {'inputs': {15: {'hea': {'display': False}}, 16: {'hea': {'display': "*

 * *           "False}, 'suggest': {insert: [(6, OrderedDict([('value', 'CHECK_DYNAMIC'), ('text', "*

 * *           "'Uses member info')]))]}}}}, 8: {'inputs': {16: {'suggest': {insert: [(6, "*

 * *           "OrderedDict([('value', 'CHECK_DYNAMIC'), ('text', 'Uses member info')]))]}}}}}}"}*

```diff
@@ -196,14 +196,15 @@
                     },
                     {
                         "name": "source",
                         "prompt": "Source"
                     },
                     {
                         "hea": {
+                            "display": false,
                             "optionsFromUrl": {
                                 "path": "people/",
                                 "text": "display_name",
                                 "value": "id"
                             },
                             "section": "shares",
                             "sectionPrompt": "Shares"
@@ -212,14 +213,15 @@
                         "prompt": "User",
                         "required": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
+                            "display": false,
                             "section": "shares"
                         },
                         "name": "permissions",
                         "prompt": "Permissions",
                         "suggest": [
                             {
                                 "text": "Co-owner",
@@ -240,14 +242,18 @@
                             {
                                 "text": "Sharer",
                                 "value": "SHARER"
                             },
                             {
                                 "text": "Viewer",
                                 "value": "VIEWER"
+                            },
+                            {
+                                "text": "Uses member info",
+                                "value": "CHECK_DYNAMIC"
                             }
                         ],
                         "type": "select"
                     },
                     {
                         "hea": {
                             "display": false,
@@ -468,14 +474,18 @@
                             {
                                 "text": "Sharer",
                                 "value": "SHARER"
                             },
                             {
                                 "text": "Viewer",
                                 "value": "VIEWER"
+                            },
+                            {
+                                "text": "Uses member info",
+                                "value": "CHECK_DYNAMIC"
                             }
                         ],
                         "type": "select"
                     },
                     {
                         "hea": {
                             "display": false,
```

### Comparing `heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.0.2
+Version: 1.1.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-organizations-1.0.2/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/tests/heaserver/organizationtest/test_all.py` & `heaserver-organizations-1.1.0/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.2/tests/heaserver/organizationtest/testcase.py` & `heaserver-organizations-1.1.0/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

