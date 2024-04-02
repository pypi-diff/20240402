# Comparing `tmp/onvo-0.1.0.tar.gz` & `tmp/onvo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvo-0.1.0.tar", last modified: Thu Mar  7 18:50:03 2024, max compression
+gzip compressed data, was "onvo-0.2.0.tar", last modified: Tue Apr  2 13:20:35 2024, max compression
```

## Comparing `onvo-0.1.0.tar` & `onvo-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.672484 onvo-0.1.0/
--rw-r--r--   0 bryan      (501) staff       (20)     1067 2024-02-15 22:07:05.000000 onvo-0.1.0/LICENSE
--rw-r--r--   0 bryan      (501) staff       (20)      672 2024-03-07 18:50:03.672134 onvo-0.1.0/PKG-INFO
--rw-r--r--   0 bryan      (501) staff       (20)       65 2024-03-06 20:49:50.000000 onvo-0.1.0/README.txt
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.663462 onvo-0.1.0/onvo/
--rw-r--r--   0 bryan      (501) staff       (20)       27 2024-02-15 22:07:05.000000 onvo-0.1.0/onvo/__init__.py
--rw-r--r--   0 bryan      (501) staff       (20)     1711 2024-03-07 13:35:09.000000 onvo-0.1.0/onvo/base_resource.py
--rw-r--r--   0 bryan      (501) staff       (20)     1888 2024-03-07 18:33:18.000000 onvo-0.1.0/onvo/onvo.py
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.668161 onvo-0.1.0/onvo/resources/
--rw-r--r--   0 bryan      (501) staff       (20)      210 2024-02-29 07:03:30.000000 onvo-0.1.0/onvo/resources/accounts.py
--rw-r--r--   0 bryan      (501) staff       (20)      482 2024-02-29 07:03:42.000000 onvo-0.1.0/onvo/resources/automations.py
--rw-r--r--   0 bryan      (501) staff       (20)      280 2024-02-29 22:37:41.000000 onvo-0.1.0/onvo/resources/dashboard.py
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.669112 onvo-0.1.0/onvo/resources/dashboard_resources/
--rw-r--r--   0 bryan      (501) staff       (20)        0 2024-02-29 22:35:06.000000 onvo-0.1.0/onvo/resources/dashboard_resources/__init__.py
--rw-r--r--   0 bryan      (501) staff       (20)      231 2024-02-29 11:56:19.000000 onvo-0.1.0/onvo/resources/dashboard_resources/base_resource.py
--rw-r--r--   0 bryan      (501) staff       (20)      575 2024-02-29 22:44:22.000000 onvo-0.1.0/onvo/resources/dashboard_resources/datasources.py
--rw-r--r--   0 bryan      (501) staff       (20)      476 2024-02-29 07:03:51.000000 onvo-0.1.0/onvo/resources/dashboards.py
--rw-r--r--   0 bryan      (501) staff       (20)      673 2024-02-29 07:03:58.000000 onvo-0.1.0/onvo/resources/datasources.py
--rw-r--r--   0 bryan      (501) staff       (20)      480 2024-02-29 07:04:09.000000 onvo-0.1.0/onvo/resources/embed_users.py
--rw-r--r--   0 bryan      (501) staff       (20)      543 2024-03-07 09:24:05.000000 onvo-0.1.0/onvo/resources/questions.py
--rw-r--r--   0 bryan      (501) staff       (20)      576 2024-03-04 10:27:45.000000 onvo-0.1.0/onvo/resources/sessions.py
--rw-r--r--   0 bryan      (501) staff       (20)      201 2024-02-29 07:04:20.000000 onvo-0.1.0/onvo/resources/teams.py
--rw-r--r--   0 bryan      (501) staff       (20)     1600 2024-03-07 17:46:47.000000 onvo-0.1.0/onvo/resources/widgets.py
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.671817 onvo-0.1.0/onvo.egg-info/
--rw-r--r--   0 bryan      (501) staff       (20)      672 2024-03-07 18:50:03.000000 onvo-0.1.0/onvo.egg-info/PKG-INFO
--rw-r--r--   0 bryan      (501) staff       (20)      780 2024-03-07 18:50:03.000000 onvo-0.1.0/onvo.egg-info/SOURCES.txt
--rw-r--r--   0 bryan      (501) staff       (20)        1 2024-03-07 18:50:03.000000 onvo-0.1.0/onvo.egg-info/dependency_links.txt
--rw-r--r--   0 bryan      (501) staff       (20)        5 2024-03-07 18:50:03.000000 onvo-0.1.0/onvo.egg-info/top_level.txt
--rw-r--r--   0 bryan      (501) staff       (20)      661 2024-03-07 18:49:20.000000 onvo-0.1.0/pyproject.toml
--rw-r--r--   0 bryan      (501) staff       (20)       38 2024-03-07 18:50:03.672537 onvo-0.1.0/setup.cfg
--rw-r--r--   0 bryan      (501) staff       (20)       69 2024-03-06 20:49:42.000000 onvo-0.1.0/setup.py
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-07 18:50:03.671417 onvo-0.1.0/tests/
--rw-r--r--   0 bryan      (501) staff       (20)      321 2024-02-22 08:55:57.000000 onvo-0.1.0/tests/test_accounts.py
--rw-r--r--   0 bryan      (501) staff       (20)     1708 2024-03-07 18:37:39.000000 onvo-0.1.0/tests/test_automations.py
--rw-r--r--   0 bryan      (501) staff       (20)     1095 2024-03-07 18:39:01.000000 onvo-0.1.0/tests/test_dashboards.py
--rw-r--r--   0 bryan      (501) staff       (20)     1589 2024-03-07 18:40:26.000000 onvo-0.1.0/tests/test_datasources.py
--rw-r--r--   0 bryan      (501) staff       (20)     1321 2024-03-07 18:44:11.000000 onvo-0.1.0/tests/test_embed_users.py
--rw-r--r--   0 bryan      (501) staff       (20)      309 2024-02-28 15:02:09.000000 onvo-0.1.0/tests/test_teams.py
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.712641 onvo-0.2.0/
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1067 2024-03-26 15:59:27.000000 onvo-0.2.0/LICENSE
+-rw-r--r--   0 bryan      (501) staff       (20)     4727 2024-04-02 13:20:35.712348 onvo-0.2.0/PKG-INFO
+-rwxr-xr-x   0 bryan      (501) staff       (20)     4121 2024-04-02 13:17:17.000000 onvo-0.2.0/README.md
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.705417 onvo-0.2.0/onvo/
+-rwxr-xr-x   0 bryan      (501) staff       (20)       27 2024-03-26 15:59:27.000000 onvo-0.2.0/onvo/__init__.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     4616 2024-04-01 19:01:47.000000 onvo-0.2.0/onvo/base_resource.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     2726 2024-03-29 20:03:45.000000 onvo-0.2.0/onvo/onvo.py
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.709126 onvo-0.2.0/onvo/resources/
+-rwxr-xr-x   0 bryan      (501) staff       (20)      627 2024-03-27 16:46:26.000000 onvo-0.2.0/onvo/resources/accounts.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1970 2024-04-01 17:16:20.000000 onvo-0.2.0/onvo/resources/automations.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)      696 2024-03-26 15:59:27.000000 onvo-0.2.0/onvo/resources/dashboard.py
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.709852 onvo-0.2.0/onvo/resources/dashboard_resources/
+-rwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-03-26 15:59:27.000000 onvo-0.2.0/onvo/resources/dashboard_resources/__init__.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)      313 2024-04-01 17:18:39.000000 onvo-0.2.0/onvo/resources/dashboard_resources/base_resource.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1291 2024-04-01 17:18:51.000000 onvo-0.2.0/onvo/resources/dashboard_resources/datasources.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1993 2024-04-01 17:16:11.000000 onvo-0.2.0/onvo/resources/dashboards.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     2473 2024-04-01 17:16:28.000000 onvo-0.2.0/onvo/resources/datasources.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1594 2024-04-01 17:16:34.000000 onvo-0.2.0/onvo/resources/embed_users.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1414 2024-04-01 17:16:46.000000 onvo-0.2.0/onvo/resources/questions.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1882 2024-04-01 17:16:55.000000 onvo-0.2.0/onvo/resources/sessions.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1095 2024-03-27 16:46:26.000000 onvo-0.2.0/onvo/resources/teams.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     4135 2024-04-01 17:17:57.000000 onvo-0.2.0/onvo/resources/widgets.py
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.712008 onvo-0.2.0/onvo.egg-info/
+-rw-r--r--   0 bryan      (501) staff       (20)     4727 2024-04-02 13:20:35.000000 onvo-0.2.0/onvo.egg-info/PKG-INFO
+-rw-r--r--   0 bryan      (501) staff       (20)      779 2024-04-02 13:20:35.000000 onvo-0.2.0/onvo.egg-info/SOURCES.txt
+-rw-r--r--   0 bryan      (501) staff       (20)        1 2024-04-02 13:20:35.000000 onvo-0.2.0/onvo.egg-info/dependency_links.txt
+-rw-r--r--   0 bryan      (501) staff       (20)        5 2024-04-02 13:20:35.000000 onvo-0.2.0/onvo.egg-info/top_level.txt
+-rwxr-xr-x   0 bryan      (501) staff       (20)      657 2024-04-02 13:19:57.000000 onvo-0.2.0/pyproject.toml
+-rw-r--r--   0 bryan      (501) staff       (20)       38 2024-04-02 13:20:35.712687 onvo-0.2.0/setup.cfg
+-rwxr-xr-x   0 bryan      (501) staff       (20)       69 2024-03-26 15:59:27.000000 onvo-0.2.0/setup.py
+drwxr-xr-x   0 bryan      (501) staff       (20)        0 2024-04-02 13:20:35.711670 onvo-0.2.0/tests/
+-rwxr-xr-x   0 bryan      (501) staff       (20)      321 2024-03-27 06:52:07.000000 onvo-0.2.0/tests/test_accounts.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1975 2024-03-29 09:56:34.000000 onvo-0.2.0/tests/test_automations.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1271 2024-03-27 16:46:26.000000 onvo-0.2.0/tests/test_dashboards.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1932 2024-03-28 17:05:26.000000 onvo-0.2.0/tests/test_datasources.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)     1321 2024-03-29 09:42:38.000000 onvo-0.2.0/tests/test_embed_users.py
+-rwxr-xr-x   0 bryan      (501) staff       (20)      614 2024-03-27 16:46:26.000000 onvo-0.2.0/tests/test_teams.py
```

### Comparing `onvo-0.1.0/LICENSE` & `onvo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvo-0.1.0/onvo.egg-info/SOURCES.txt` & `onvo-0.2.0/onvo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.txt
+README.md
 pyproject.toml
 setup.py
 onvo/__init__.py
 onvo/base_resource.py
 onvo/onvo.py
 onvo.egg-info/PKG-INFO
 onvo.egg-info/SOURCES.txt
```

### Comparing `onvo-0.1.0/pyproject.toml` & `onvo-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onvo"
-version = "0.1.0"
+version = "0.2.0"
 authors = [{ name = "Bryan Davis", email = "bryandavis999.dev@gmail.com" }]
 description = "Communicate with the Onvo platform."
-readme = "README.txt"
+readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-  "Development Status :: 1 - Planning",
+  "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
 keywords = ["python", "onvo"]
```

### Comparing `onvo-0.1.0/tests/test_automations.py` & `onvo-0.2.0/tests/test_automations.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,54 +2,64 @@
 
 SAMPLE_DASHBOARD_PARAMS = {
     "description": "Sample dashboard for widget testing",
     "title": "Widget Testing Dashboard",
 }
 
 SAMPLE_AUTOMATION_PARAMS = {
-    "created_by": "197302e5-88e2-49f4-bbe7-92b5a4dc4264",
     "description": "A sample description",
     "email_format": "This is an automation from Onvo",
     "email_subject": "This is an automation from Onvo",
     "enabled": "false",
     "output_format": "link",
     "recipient_type": "internal",
+    "recipients": [],
     "schedule": "",
+    "timezone": "Asia/Calcutta",
     "title": "API datasource test",
 }
 
 
 class TestAutomations(BaseTest):
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
-        cls.sampleDashboardId = cls.onvoSDK.dashboards.create(SAMPLE_DASHBOARD_PARAMS)[
-            "id"
-        ]
+        cls.sample_dashboard_id = cls.onvoSDK.dashboards.create(
+            SAMPLE_DASHBOARD_PARAMS
+        )["id"]
         # Skipping test create
-        cls.sampleAutomationId = cls.onvoSDK.automations.create(
-            {**SAMPLE_AUTOMATION_PARAMS, "dashboard": cls.sampleDashboardId}
+        cls.sample_automation_id = cls.onvoSDK.automations.create(
+            {
+                **SAMPLE_AUTOMATION_PARAMS,
+                "dashboard": cls.sample_dashboard_id,
+                "created_by": cls.sample_user_id,
+            }
         )["id"]
 
     def test_list(self):
         self.assertShouldRaise(None, self.onvoSDK.automations.list)
 
     def test_get(self):
         self.assertShouldRaise(
-            None, lambda: self.onvoSDK.automations.get(self.sampleAutomationId)
+            None, lambda: self.onvoSDK.automations.get(self.sample_automation_id)
+        )
+
+    def test_get_runs(self):
+        self.assertShouldRaise(
+            None, lambda: self.onvoSDK.automations.get_runs(self.sample_automation_id)
         )
 
     def test_update(self):
         self.assertShouldRaise(
             None,
             lambda: self.onvoSDK.automations.update(
-                self.sampleAutomationId,
+                self.sample_automation_id,
                 {"description": "A New Test Description. Delete if seen."},
             ),
         )
 
     @classmethod
     def tearDownClass(cls) -> None:
-        cls.onvoSDK.dashboards.delete(cls.sampleDashboardId)
-        cls.onvoSDK.automations.delete(cls.sampleAutomationId)  # Skipping test delete
+        cls.onvoSDK.dashboards.delete(cls.sample_dashboard_id)
+        cls.onvoSDK.automations.delete(cls.sample_automation_id)  # Skipping test delete
         super().tearDownClass()
```

### Comparing `onvo-0.1.0/tests/test_dashboards.py` & `onvo-0.2.0/tests/test_dashboards.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,11 +28,17 @@
             None,
             lambda: self.onvoSDK.dashboards.update(
                 self.sampleDashboardId,
                 {"description": "A New Test Description. Delete if seen."},
             ),
         )
 
+    def test_update_cache(self):
+        self.assertShouldRaise(
+            None,
+            lambda: self.onvoSDK.dashboards.update_cache(self.sampleDashboardId),
+        )
+
     @classmethod
     def tearDownClass(cls) -> None:
         cls.onvoSDK.dashboards.delete(cls.sampleDashboardId)  # Skipping test delete
         super().tearDownClass()
```

### Comparing `onvo-0.1.0/tests/test_datasources.py` & `onvo-0.2.0/tests/test_datasources.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .base_test import BaseTest
+import os
 
 SAMPLE_DATASOURCE_PARAMS = {
     "description": "Python Integration Test Data Source. Delete if seen.",
     "title": "Python Integration Test Data Source",
     "source": "api",
     "config": '{"type":"json","method":"GET","transform":"products","url":"https://dummyjson.com/products","headers":"{}"}',
 }
@@ -23,30 +24,37 @@
         self.assertShouldRaise(None, self.onvoSDK.datasources.list)
 
     def test_get(self):
         self.assertShouldRaise(
             None, lambda: self.onvoSDK.datasources.get(self.sampleDatasourceId)
         )
 
-    def test_get_data(self):
+    def test_initialize(self):
         self.assertShouldRaise(
-            None, lambda: self.onvoSDK.datasources.get_data(self.sampleDatasourceId)
+            None, lambda: self.onvoSDK.datasources.initialize(self.sampleDatasourceId)
         )
 
     def test_update(self):
         self.assertShouldRaise(
             None,
             lambda: self.onvoSDK.datasources.update(
                 self.sampleDatasourceId, {"title": "Renaming Test"}
             ),
         )
 
-    def test_populate_columns(self):
-        self.assertShouldRaise(
-            None,
-            lambda: self.onvoSDK.datasources.populate_columns(self.sampleDatasourceId),
-        )
+    # TODO: diagnose and fix 500: Internal server error
+    # def test_upload_file(self):
+    #     test_file_path = os.path.join(os.path.dirname(__file__), "python_onvo_test.csv")
+    #     with open(test_file_path, "ab") as f:
+    #         f.write(b"a,b,c\n1,2,3\n4,5,6\n")
+    #     self.assertShouldRaise(
+    #         None,
+    #         lambda: self.onvoSDK.datasources.upload_file(
+    #             self.sampleDatasourceId, test_file_path
+    #         ),
+    #     )
+    #     os.remove(test_file_path)
 
     @classmethod
     def tearDownClass(cls) -> None:
         cls.onvoSDK.datasources.delete(cls.sampleDatasourceId)  # Skipping test delete
         super().tearDownClass()
```

### Comparing `onvo-0.1.0/tests/test_embed_users.py` & `onvo-0.2.0/tests/test_embed_users.py`

 * *Files identical despite different names*

