# Comparing `tmp/drivelinepy-1.5.1.tar.gz` & `tmp/drivelinepy-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drivelinepy-1.5.1.tar", last modified: Wed Mar 27 03:02:43 2024, max compression
+gzip compressed data, was "drivelinepy-1.6.1.tar", last modified: Tue Apr  2 18:15:06 2024, max compression
```

## Comparing `drivelinepy-1.5.1.tar` & `drivelinepy-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:02:43.411455 drivelinepy-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-27 03:02:43.407455 drivelinepy-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:02:43.407455 drivelinepy-1.5.1/drivelinepy/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/base_api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/brightpearl_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:02:43.407455 drivelinepy-1.5.1/drivelinepy/brightpearl_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/brightpearl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/brightpearl_utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/slack_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/traq_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/virtuagym_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/zoho_billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/drivelinepy/zoho_crm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:02:43.407455 drivelinepy-1.5.1/drivelinepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-27 03:02:43.000000 drivelinepy-1.5.1/drivelinepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-27 03:02:43.000000 drivelinepy-1.5.1/drivelinepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 03:02:43.000000 drivelinepy-1.5.1/drivelinepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 03:02:43.000000 drivelinepy-1.5.1/drivelinepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 03:02:43.000000 drivelinepy-1.5.1/drivelinepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 03:02:43.411455 drivelinepy-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-27 03:02:33.000000 drivelinepy-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/base_api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/slack_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/traq_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/virtuagym_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/zoho_billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/zoho_crm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/setup.py
```

### Comparing `drivelinepy-1.5.1/LICENSE` & `drivelinepy-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/PKG-INFO` & `drivelinepy-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drivelinepy
-Version: 1.5.1
+Version: 1.6.1
 Summary: A Python package for Driveline Baseball API interactions
 Home-page: https://github.com/drivelineresearch/drivelinepy
 Author: Garrett York
 Author-email: garrett@drivelinebaseball.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drivelinepy-1.5.1/drivelinepy/base_api_wrapper.py` & `drivelinepy-1.6.1/drivelinepy/base_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/brightpearl_api.py` & `drivelinepy-1.6.1/drivelinepy/brightpearl_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/brightpearl_utils/helper_functions.py` & `drivelinepy-1.6.1/drivelinepy/brightpearl_utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/slack_api.py` & `drivelinepy-1.6.1/drivelinepy/slack_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/traq_api.py` & `drivelinepy-1.6.1/drivelinepy/traq_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/virtuagym_api.py` & `drivelinepy-1.6.1/drivelinepy/virtuagym_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/zoho_billing_api.py` & `drivelinepy-1.6.1/drivelinepy/zoho_billing_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/drivelinepy/zoho_crm_api.py` & `drivelinepy-1.6.1/drivelinepy/zoho_crm_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,41 +176,45 @@
         self.logger.info(f"Exiting _fetch_data() with total {len(all_data_list)} {data_key} fetched")
         return all_data_list
     
     #-----------------------------------------------------------------
     # Method - Get Customer Records
     #-----------------------------------------------------------------
 
-    def get_customer_records(self, module, customer_id=None, first_name=None, last_name=None, email=None, converted_leads=None, page=1):
+    def get_customer_records(self, module, customer_id=None, first_name=None, last_name=None, email=None, converted_leads=None, attachments=None, page=1):
         """
         Fetches customer records from the Zoho CRM API based on the specified criteria.
         :param module: The module to fetch records from.
         :param customer_id: The ID of the customer to fetch.
         :param first_name: The first name of the customer to fetch.
         :param last_name: The last name of the customer to fetch.
         :param email: The email of the customer to fetch.
         :param page: The page number to fetch.
         :param converted_leads: If True, fetch converted leads only.
+        :param attachments: If True, fetch attachments.
+
         """
         self.logger.info("Entering get_customer_records()")
 
         # check if module in supported modules
         if module in self.SUPPORTED_MODULES:
             endpoint = module
         else:
             self.logger.error("Invalid module provided.")
             return None
         
         params = {}
         data_key = "data"
 
-        
         if customer_id:
             # Fetch a specific customer by ID
             endpoint += f"/{customer_id}"
+            # If attachments are requested, add the parameter to the endpoint
+            if attachments:
+                endpoint += "/Attachments"
         else:
             # Search for customers based on provided criteria or fetch all if no criteria
             criteria_list = []
             if first_name:
                 criteria_list.append(f"(First_Name:equals:{first_name})")
             if last_name:
                 criteria_list.append(f"(Last_Name:equals:{last_name})")
```

### Comparing `drivelinepy-1.5.1/drivelinepy.egg-info/PKG-INFO` & `drivelinepy-1.6.1/drivelinepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drivelinepy
-Version: 1.5.1
+Version: 1.6.1
 Summary: A Python package for Driveline Baseball API interactions
 Home-page: https://github.com/drivelineresearch/drivelinepy
 Author: Garrett York
 Author-email: garrett@drivelinebaseball.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drivelinepy-1.5.1/drivelinepy.egg-info/SOURCES.txt` & `drivelinepy-1.6.1/drivelinepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.5.1/setup.py` & `drivelinepy-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='drivelinepy',
-    version='1.5.1',
+    version='1.6.1',
     author='Garrett York',
     author_email='garrett@drivelinebaseball.com',
     description='A Python package for Driveline Baseball API interactions',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/drivelineresearch/drivelinepy',
     packages=find_packages(),
```

