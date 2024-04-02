# Comparing `tmp/LSVcherwellAPI-1.3.9.1.tar.gz` & `tmp/LSVcherwellAPI-1.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LSVcherwellAPI-1.3.9.1.tar", last modified: Thu Mar 28 20:27:32 2024, max compression
+gzip compressed data, was "LSVcherwellAPI-1.3.9.2.tar", last modified: Tue Apr  2 02:16:58 2024, max compression
```

## Comparing `LSVcherwellAPI-1.3.9.1.tar` & `LSVcherwellAPI-1.3.9.2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 20:27:32.344358 LSVcherwellAPI-1.3.9.1/
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)      984 2024-03-28 20:27:32.343358 LSVcherwellAPI-1.3.9.1/PKG-INFO
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)      997 2024-03-28 20:26:58.000000 LSVcherwellAPI-1.3.9.1/pyproject.toml
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)       38 2024-03-28 20:27:32.344358 LSVcherwellAPI-1.3.9.1/setup.cfg
-drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 20:27:32.340358 LSVcherwellAPI-1.3.9.1/src/
-drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 20:27:32.341358 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     7662 2024-03-28 19:24:51.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/BusinessObjects.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     6437 2024-03-28 19:29:34.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Cache.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)    42905 2024-03-28 19:23:54.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/CherwellClient.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)    42064 2024-03-28 20:22:04.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/CherwellClientServer.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1334 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/CherwellCredentials.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     5402 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Filter.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     4948 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Token.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)      937 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/CherwellAPI/__init__.py
-drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 20:27:32.343358 LSVcherwellAPI-1.3.9.1/src/Examples/
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2315 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Create_CI_With_Dynamic_Attributes.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2449 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Cache.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1496 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateEncryptedCredentials.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2468 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateIncident.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1892 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateIncident_with_BusinessObject.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2722 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Create_New_Custom_Business_Object.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1999 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Delete_Incident_with_BusinessObjects.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1037 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_GetInternalName.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1004 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Get_Summary.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1008 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Get_Template.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1372 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_RunSavedSearch.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2013 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Searches.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1674 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Searches_with_BusinessObjects.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     3538 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Token Usage.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1993 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/Example_Update_Incident_with_BusinessObjects.py
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 00:37:00.000000 LSVcherwellAPI-1.3.9.1/src/Examples/__init__.py
-drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-28 20:27:32.343358 LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)      984 2024-03-28 20:27:32.000000 LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/PKG-INFO
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1156 2024-03-28 20:27:32.000000 LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/SOURCES.txt
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)        1 2024-03-28 20:27:32.000000 LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/dependency_links.txt
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)       27 2024-03-28 20:27:32.000000 LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/top_level.txt
--rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1214 2024-03-28 20:27:14.000000 LSVcherwellAPI-1.3.9.1/src/setup.py
+drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-04-02 02:16:58.290978 LSVcherwellAPI-1.3.9.2/
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1040 2024-04-02 02:16:58.290978 LSVcherwellAPI-1.3.9.2/PKG-INFO
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1073 2024-04-01 15:58:17.000000 LSVcherwellAPI-1.3.9.2/pyproject.toml
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)       38 2024-04-02 02:16:58.290978 LSVcherwellAPI-1.3.9.2/setup.cfg
+drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-04-02 02:16:58.279977 LSVcherwellAPI-1.3.9.2/src/
+drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-04-02 02:16:58.282977 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     7773 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/BusinessObjects.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     6655 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Cache.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)    43471 2024-04-01 15:59:01.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/CherwellClient.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1334 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/CherwellCredentials.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     5402 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Filter.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     4948 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Token.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)      937 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/CherwellAPI/__init__.py
+drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-04-02 02:16:58.289978 LSVcherwellAPI-1.3.9.2/src/Examples/
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2315 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Create_CI_With_Dynamic_Attributes.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2449 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Cache.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1496 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateEncryptedCredentials.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2468 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateIncident.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1892 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateIncident_with_BusinessObject.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2722 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Create_New_Custom_Business_Object.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1999 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Delete_Incident_with_BusinessObjects.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1037 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_GetInternalName.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1004 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Get_Summary.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1008 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Get_Template.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1372 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_RunSavedSearch.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     2013 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Searches.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1674 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Searches_with_BusinessObjects.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     3538 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Token Usage.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1993 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/Example_Update_Incident_with_BusinessObjects.py
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-03-29 21:58:02.000000 LSVcherwellAPI-1.3.9.2/src/Examples/__init__.py
+drwxr-xr-x   0 1-witt0928 (1679227713) domain users (1679200513)        0 2024-04-02 02:16:58.290978 LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1040 2024-04-02 02:16:58.000000 LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/PKG-INFO
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1116 2024-04-02 02:16:58.000000 LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)        1 2024-04-02 02:16:58.000000 LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)       27 2024-04-02 02:16:58.000000 LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/top_level.txt
+-rw-r--r--   0 1-witt0928 (1679227713) domain users (1679200513)     1214 2024-03-29 23:52:32.000000 LSVcherwellAPI-1.3.9.2/src/setup.py
```

### Comparing `LSVcherwellAPI-1.3.9.1/PKG-INFO` & `LSVcherwellAPI-1.3.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: LSVcherwellAPI
-Version: 1.3.9.1
+Version: 1.3.9.2
 Summary: A Python library wrapper, abstracting the Cherwell REST API
-Author-email: David Graupner <david.graupner@streamlinepartners.com.au>, Aaron Cohee <aaron.cohee@streamlinepartners.com.au>, Marty Leaman <marty.leaman@streamlinepartners.com.au>
+Author-email: David Graupner <david.graupner@streamlinepartners.com.au>, Aaron Cohee <aaron.cohee@streamlinepartners.com.au>, Marty Leaman <marty.leaman@streamlinepartners.com.au>, Brandon Wittenburg <brandon.wittenburg@usablelife.com>
 Project-URL: Homepage, https://github.com/bwittenburg/CherwellAPI
 Project-URL: Issues, https://github.com/bwittenburg/CherwellAPI/issues
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `LSVcherwellAPI-1.3.9.1/pyproject.toml` & `LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-[project]
-name = "LSVcherwellAPI"
-version = "1.3.9.1"
-authors = [
-  { name="David Graupner", email="david.graupner@streamlinepartners.com.au" },
-  { name="Aaron Cohee", email="aaron.cohee@streamlinepartners.com.au" },
-  { name="Marty Leaman", email="marty.leaman@streamlinepartners.com.au" }
-]
-description = "A Python library wrapper, abstracting the Cherwell REST API"
-readme = "README.md"
-#requires_python = ">=2.6"
-classifiers = [
-  "Programming Language :: Python :: 2.6",
-  "Programming Language :: Python :: 2.7",
-  "Programming Language :: Python :: 3.4",
-  "Programming Language :: Python :: 3.5",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/bwittenburg/CherwellAPI"
-Issues = "https://github.com/bwittenburg/CherwellAPI/issues"
+Metadata-Version: 2.1
+Name: LSVcherwellAPI
+Version: 1.3.9.2
+Summary: A Python library wrapper, abstracting the Cherwell REST API
+Author-email: David Graupner <david.graupner@streamlinepartners.com.au>, Aaron Cohee <aaron.cohee@streamlinepartners.com.au>, Marty Leaman <marty.leaman@streamlinepartners.com.au>, Brandon Wittenburg <brandon.wittenburg@usablelife.com>
+Project-URL: Homepage, https://github.com/bwittenburg/CherwellAPI
+Project-URL: Issues, https://github.com/bwittenburg/CherwellAPI/issues
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/BusinessObjects.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/BusinessObjects.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,25 +51,26 @@
         
         https_verify : bool
 
             Flag set to verify SSL Certificates during requests API Calls
 
         """
 
-    def __init__(self, type_name, get_header_function, save_uri, delete_uri, busObID, busObRecId="", busObPublicId=""):
+    def __init__(self, type_name, get_header_function, save_uri, delete_uri, busObID, busObRecId="", busObPublicId="", https_verify=False):
 
         self.type_name = type_name
         self.busObId = busObID
         self.busObPublicId = busObPublicId
         self.persist = True
         self.busobj_fields = []
         self.get_header = get_header_function
         self.save_uri = save_uri
         self.delete_uri = delete_uri
         self.busObRecId = busObRecId
+        self.https_verify = https_verify
         self.has_Error = False
         self.error_Message = ""
 
     # Return whether we have an error or not
     def has_error(self):
 
         """ Returns true if the last call to Cherwell returned an error """
@@ -162,15 +163,15 @@
                     field["value"] = self.__dict__[instance_name]
 
         # Build the payload for the save
         save_payload = {"Persist": True, "busObID": self.busObId, "busObPublicId": self.busObPublicId,
                         "busObRecId": self.busObRecId, "fields": self.busobj_fields}
 
         # Attempt to save the record
-        result_save = requests.post(self.save_uri, json=save_payload, headers=self.get_header())
+        result_save = requests.post(self.save_uri, json=save_payload, headers=self.get_header(),verify=self.https_verify)
 
         # Set the business object error states
         self.has_Error = result_save.json()["hasError"]
         self.error_Message = result_save.json()["errorMessage"]
 
         if result_save.status_code == 200:
 
@@ -192,15 +193,15 @@
         # Attempt to delete the current record if it has a busObId and busObRecId
         if self.busObId and self.busObRecId:
 
             # Create the the delete URL
             self.delete_uri = str(self.delete_uri).replace("[busobid]", self.busObId).replace("[busobrecid]", self.busObRecId)
 
             # Execute the delete
-            result_delete = requests.delete(self.delete_uri, headers=self.get_header())
+            result_delete = requests.delete(self.delete_uri, headers=self.get_header(),verify=self.https_verify)
 
             if result_delete.status_code == 200:
 
                 # Successfully saved the record - remove the id's from this BusinessObject
                 self.busObPublicId = ""
                 self.busObRecId = ""
```

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Cache.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,28 +27,33 @@
 
         The base uri of the Cherwell instance
 
     api_key : str
 
         The Cherwell REST API client key used for authorisation
 
+    auth_mode : str
+
+        The Cherwell authentication mode used to retrieve the token. Supported modes are Internal (default), LDAP, SAML, and Windows.
+
     """
 
-    def __init__(self, base_uri, api_key):
+    def __init__(self, base_uri, api_key, auth_mode):
 
         # Start the cache
         self.cache = {}
 
         # add the base uri and other attributes
         self.cache["base_uri"] = base_uri
         self.cache["api_key"] = api_key
+        self.cache["auth_mode"] = auth_mode
 
         # Add various uri's for accessing the api
         self.cache["uris"] = {
-            "Token": "{0}/CherwellAPI/token?auth_mode=Windows&api_key={1}".format(base_uri, api_key),
+            "Token": "{0}/CherwellAPI/token?auth_mode={1}&api_key={2}".format(base_uri, auth_mode, api_key),
             "BusinessObjectID": "{0}/CherwellAPI/api/V1/getbusinessobjectsummary/busobname/".format(base_uri),
             "BusinessObjectTemplate": "{0}/CherwellAPI/api/V1/GetBusinessObjectTemplate/".format(base_uri),
             "BusinessObjectSummary": "{0}/CherwellAPI/api/V1/getbusinessobjectsummary/busobname/".format(base_uri),
             "BusinessObjectSave": "{0}/CherwellAPI/api/V1/SaveBusinessObject".format(base_uri),
             "BusinessSearchResults": "{0}/CherwellAPI/api/V1/getsearchresults".format(base_uri),
             "RunSavedSearch": "{0}/CherwellAPI/api/V1/getsearchresults/association/[association]/scope/[scope]/scopeowner/[scopeowner]/searchname/[searchname]?includeschema=[includeschema]&resultsAsSimpleResultsList=[resultsAsSimpleResultsList]".format(base_uri),
             "BusinessObjectDelete": "{0}/CherwellAPI/api/V1/deletebusinessobject/busobid/[busobid]/busobrecid/[busobrecid]".format(base_uri),
```

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/CherwellClient.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/CherwellClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,27 +44,32 @@
 
     token : AccessToken
 
         An instance of the AccessToken class that was previously created or saved/cached. If a AccessToken is not
         provided then this is defaulted to 'None' and a new AccessToken will be created during the first
         interaction to the Cherwell REST API
 
+    auth_mode: str
+
+        The Cherwell authentication mode to use to retrieve the token. Supported modes are Internal (default), LDAP, SAML, and Windows.
+
     https_verify : bool
 
         Flag set to verify SSL Certificates during requests API Calls
 
     """
 
-    def __init__(self, base_uri="", client_key="", username="", password="", cache=None, token=None):
+    def __init__(self, base_uri="", client_key="", username="", password="", cache=None, token=None, https_verify=False, auth_mode="Internal"):
 
         """ Connection instance initialisation """
 
         # Set the values we need that were passed in
         self.uri = base_uri
         self.username = username
+        self.auth_mode = auth_mode
         if not password or not client_key:
             try:
                 self.client_key = CherwellCredentials.decrypt_message("cherwell_api_key")
                 self.password = CherwellCredentials.decrypt_message("cherwell_password")
             except:
                 raise Exception("Unable to locate encrypted Cherwell API Key and Password. Please run the function CherwellCrentials.create_encrypted_cherwell_credentials(password, client_key) first or pass in the password and client key in the CherwellClient.Connection Method")
         else:
@@ -74,24 +79,25 @@
         # Initialise a cache object - we can reuse
         if isinstance(cache, ObjectCache):
 
             # we have been passed a saved cache object
             self.cache = cache
         else:
             # We don't have a saved cache object - instantiate a new one
-            self.cache = ObjectCache(self.uri, self.client_key)
+            self.cache = ObjectCache(self.uri, self.client_key, self.auth_mode)
 
         if token is not None and isinstance(token, AccessToken):
 
             # We have been passed an existing token
             self.token = token
         else:
             # Token not correct type - start with no token
             self.token = None
 
+        self.https_verify = https_verify
 
     def cache(self):
 
         """
         Returns the ObjectCache object used by the Connection to avoid repeated round trip to through the Cherwell API
         for data that is largely reused
         """
@@ -113,15 +119,15 @@
         Called internally to Authenticate to Cherwell and retrieves a new Bearer token
         """
 
         token_payload = {"Accept": "application/json", "grant_type": "password", "client_id": self.client_key,
                               "username": self.username, "password": self.password}
 
         # Attempt to get a token
-        token_result = requests.post(self.cache.get_uri("Token"), data=token_payload)
+        token_result = requests.post(self.cache.get_uri("Token"), data=token_payload,verify=self.https_verify)
 
         if token_result.status_code == 200:
             # We were successful  - create a new token using the newly obtained json token
             self.token = AccessToken()
             self.token.load(token_result.json())
         else:
             # We could not get a token - this is bad, generate an exception
@@ -136,15 +142,15 @@
         Called internally to Authenticate to generate a new refreshed token as the existing one has expired
         """
 
         token_refresh_payload = {"Accept": "application/json", "grant_type": "password", "client_id": self.client_key,
                          "username": self.username, "password": self.password, "refresh_token": self.token.refresh_token}
 
         # Attempt to get a token
-        token_refresh_result = requests.post(self.cache.get_uri("Token"), data=token_refresh_payload)
+        token_refresh_result = requests.post(self.cache.get_uri("Token"), data=token_refresh_payload,verify=self.https_verify)
 
         # Get the token details
         if token_refresh_result.status_code == 200:
             # We were successful  - create a new token using the newly obtained json token
             self.token = AccessToken()
             self.token.load(token_refresh_result.json())
         else:
@@ -203,15 +209,15 @@
 
         if not self.cache.get_business_object_id(business_object_name) or refresh:
 
             # Default the return to None
             self.cache.set_business_object_id(business_object_name, None)
 
             # Call the API to get the result
-            result_business_object_id = requests.get(self.cache.get_uri("BusinessObjectID") + business_object_name, headers=self._get_authorisation_header())
+            result_business_object_id = requests.get(self.cache.get_uri("BusinessObjectID") + business_object_name, headers=self._get_authorisation_header(),verify=self.https_verify)
 
             if result_business_object_id.status_code == 200:
 
                 if result_business_object_id.text != "[]":
                     # Success - save the value
                     self.cache.set_business_object_id(business_object_name, result_business_object_id.json()[0]["busObId"])
             else:
@@ -262,15 +268,15 @@
             # Get the object id for the requested object
             object_id = self.get_business_object_id(business_object_name)
 
             # Setup the templateRequest
             template_request = {"busObID": object_id, "includeRequired": "True", "includeAll": "True"}
 
             # Call the API to get the template
-            result_business_object_template = requests.post(self.cache.get_uri("BusinessObjectTemplate"), json=template_request, headers=self._get_authorisation_header())
+            result_business_object_template = requests.post(self.cache.get_uri("BusinessObjectTemplate"), json=template_request, headers=self._get_authorisation_header(),verify=self.https_verify)
 
             if result_business_object_template.status_code == 200:
 
                 # Success - we have the template
                 self.cache.set_business_object_template(business_object_name, result_business_object_template.json())
 
         return self.cache.get_business_object_template(business_object_name)
@@ -375,15 +381,15 @@
 
             # Default the return to None
             self.cache.set_business_object_summary(business_object_name, None)
 
             # Call the API to get the summary
             result_business_object_summary = requests.get("{}{}".format(
                 self.cache.get_uri("BusinessObjectSummary"), business_object_name),
-                headers=self._get_authorisation_header())
+                headers=self._get_authorisation_header(),verify=self.https_verify)
 
             if result_business_object_summary.status_code == 200:
 
                 if result_business_object_summary.text != "[]":
                     # Success - we have the summary
                     self.cache.set_business_object_summary(business_object_name, result_business_object_summary.json())
 
@@ -426,15 +432,15 @@
 
             # Default the return to None
             self.cache.set_business_object_schema(business_object_id, None)
 
             # Call the API to get the schema
             result_business_object_schema = requests.get("{}{}".format(
                 self.cache.get_uri("BusinessObjectSchema"), business_object_id),
-                headers=self._get_authorisation_header())
+                headers=self._get_authorisation_header(),verify=self.https_verify)
 
             if result_business_object_schema.status_code == 200:
 
                 if result_business_object_schema.text != "[]":
                     # Success - we have the schema
                     self.cache.set_business_object_schema(business_object_id, result_business_object_schema.json())
 
@@ -524,15 +530,15 @@
         # Get the object id for the requested object
         business_object_id = self.get_business_object_id(business_object_name)
 
         # Setup the payload
         payload = {"busObID": business_object_id, "fields": template["fields"]}
 
         # Attempt to save the new Business Object
-        result_new = requests.post(self.cache.get_uri("BusinessObjectSave"), json=payload, headers=self._get_authorisation_header())
+        result_new = requests.post(self.cache.get_uri("BusinessObjectSave"), json=payload, headers=self._get_authorisation_header(),verify=self.https_verify)
 
         if result_new.status_code == 200:
             # Success - return the public id and record id
             return str(result_new.json()["busObPublicId"]), str(result_new.json()["busObRecId"]), business_object_id
         else:
             # There was a problem with the API call, generate an exception
             raise Exception("Error creating the new business object '{}'. HTTP:{} '{}' - {}".format(
@@ -665,15 +671,15 @@
         while True:
             # Setup the payload
             payload = {"busObID": business_object_id, "filters": filter_info,
                        "includeAllFields": filter_object.include_all_fields, "pageNumber": page_number}
 
             # Attempt to get the required business object
             result_bus_obj_search = requests.post(self.cache.get_uri("BusinessSearchResults"), json=payload,
-                                   headers=self._get_authorisation_header())
+                                   headers=self._get_authorisation_header(),verify=self.https_verify)
 
             if result_bus_obj_search.status_code == 200:
 
                 search_results = result_bus_obj_search.json()
 
                 # Get how many rows were returned
                 rows = search_results["totalRows"]
@@ -822,15 +828,15 @@
 
         # Setup the payload
         payload = {"busObID": business_object_id, "fields": field_list, "filters": filter_info,
                    "includeAllFields": filter_object.include_all_fields}
 
         # Attempt to get the required business object
         result_search = requests.post(self.cache.get_uri("BusinessSearchResults"), json=payload,
-                               headers=self._get_authorisation_header())
+                               headers=self._get_authorisation_header(),verify=self.https_verify)
 
         if result_search.status_code == 200:
 
             # We have some records
             search_results = result_search.json()
 
             # Get how many rows were returned
@@ -993,15 +999,15 @@
 
         # Get the object id for the requested object
         business_object_id = self.get_business_object_id(association)
 
         saved_search_uri = self.cache.get_uri("RunSavedSearch").replace("[association]", business_object_id).replace("[scope]", scope).replace("[scopeowner]", scope_owner).replace("[searchname]", search_name).replace("[includeschema]", include_schema).replace("[resultsAsSimpleResultsList]", results_as_simple_results_list)
 
         # Attempt to get the required business object
-        result_search = requests.get(saved_search_uri, headers=self._get_authorisation_header())
+        result_search = requests.get(saved_search_uri, headers=self._get_authorisation_header(),verify=self.https_verify)
 
         if result_search.status_code == 200:
 
             # We have some records
             search_results = result_search.json()
 
             # Get how many rows were returned
@@ -1039,15 +1045,15 @@
 
         """
         This method can be used to logout of the Cherwell instance. The user referenced in the authentication token is
         instantly logged out. A new CherwellClient instance and token will be required to login again.
         """
 
         # Attempt to logout
-        response = requests.delete(self.cache.get_uri("Logout"), headers=self._get_authorisation_header())
+        response = requests.delete(self.cache.get_uri("Logout"), headers=self._get_authorisation_header(),verify=self.https_verify)
 
         if response.status_code == 200:
             # Success - Logged out successfully
             return str(response.status_code)
         else:
             # There was a problem with the API call, generate an exception
             raise Exception("Error logging out of Cherwell 'HTTP:{} '{}' - {}".format(
```

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/CherwellCredentials.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/CherwellCredentials.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Filter.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Filter.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/Token.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/Token.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/CherwellAPI/__init__.py` & `LSVcherwellAPI-1.3.9.2/src/CherwellAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Create_CI_With_Dynamic_Attributes.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Create_CI_With_Dynamic_Attributes.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Cache.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Cache.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateEncryptedCredentials.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateEncryptedCredentials.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateIncident.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateIncident.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_CreateIncident_with_BusinessObject.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_CreateIncident_with_BusinessObject.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Create_New_Custom_Business_Object.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Create_New_Custom_Business_Object.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Delete_Incident_with_BusinessObjects.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Delete_Incident_with_BusinessObjects.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_GetInternalName.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_GetInternalName.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Get_Summary.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Get_Summary.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Get_Template.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Get_Template.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_RunSavedSearch.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_RunSavedSearch.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Searches.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Searches.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Searches_with_BusinessObjects.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Searches_with_BusinessObjects.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Token Usage.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Token Usage.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/Examples/Example_Update_Incident_with_BusinessObjects.py` & `LSVcherwellAPI-1.3.9.2/src/Examples/Example_Update_Incident_with_BusinessObjects.py`

 * *Files identical despite different names*

### Comparing `LSVcherwellAPI-1.3.9.1/src/LSVcherwellAPI.egg-info/SOURCES.txt` & `LSVcherwellAPI-1.3.9.2/src/LSVcherwellAPI.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 pyproject.toml
 src/setup.py
 src/CherwellAPI/BusinessObjects.py
 src/CherwellAPI/Cache.py
 src/CherwellAPI/CherwellClient.py
-src/CherwellAPI/CherwellClientServer.py
 src/CherwellAPI/CherwellCredentials.py
 src/CherwellAPI/Filter.py
 src/CherwellAPI/Token.py
 src/CherwellAPI/__init__.py
 src/Examples/Create_CI_With_Dynamic_Attributes.py
 src/Examples/Example_Cache.py
 src/Examples/Example_CreateEncryptedCredentials.py
```

### Comparing `LSVcherwellAPI-1.3.9.1/src/setup.py` & `LSVcherwellAPI-1.3.9.2/src/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "r") as readme_file:
     long_description = readme_file.read()
 
 setuptools.setup(
     name='CherwellAPI',
-    version='1.3.9.1',
+    version='1.3.9.2',
     author='Streamline Partners PTY Ltd',
     author_email='david.graupner@streamlinepartners.com.au, aaron.cohee@streamlinepartners.com.au, marty.leaman@streamlinepartners.com.au',
     description='A Python library wrapper, abstracting the Cherwell REST API',
     url='',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
```

