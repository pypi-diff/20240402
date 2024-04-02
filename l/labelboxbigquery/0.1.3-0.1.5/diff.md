# Comparing `tmp/labelboxbigquery-0.1.3.tar.gz` & `tmp/labelboxbigquery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelboxbigquery-0.1.3.tar", last modified: Sat Feb 11 00:21:41 2023, max compression
+gzip compressed data, was "labelboxbigquery-0.1.5.tar", last modified: Tue Apr  2 15:54:04 2024, max compression
```

## Comparing `labelboxbigquery-0.1.3.tar` & `labelboxbigquery-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:21:41.740441 labelboxbigquery-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-11 00:21:41.740441 labelboxbigquery-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:21:41.740441 labelboxbigquery-0.1.3/labelboxbigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/labelboxbigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/labelboxbigquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/labelboxbigquery/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:21:41.740441 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-11 00:21:41.000000 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-11 00:21:41.000000 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 00:21:41.000000 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-11 00:21:41.000000 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-11 00:21:41.000000 labelboxbigquery-0.1.3/labelboxbigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 00:21:41.740441 labelboxbigquery-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-11 00:21:31.000000 labelboxbigquery-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:54:04.330910 labelboxbigquery-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-02 15:54:04.330910 labelboxbigquery-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:54:04.330910 labelboxbigquery-0.1.5/labelboxbigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/labelboxbigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35218 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/labelboxbigquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/labelboxbigquery/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:54:04.330910 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-02 15:54:04.000000 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 15:54:04.000000 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:54:04.000000 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 15:54:04.000000 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 15:54:04.000000 labelboxbigquery-0.1.5/labelboxbigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:54:04.330910 labelboxbigquery-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 15:54:01.000000 labelboxbigquery-0.1.5/setup.py
```

### Comparing `labelboxbigquery-0.1.3/LICENSE` & `labelboxbigquery-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `labelboxbigquery-0.1.3/PKG-INFO` & `labelboxbigquery-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: labelboxbigquery
-Version: 0.1.3
+Version: 0.1.5
 Summary: Labelbox Connector for BigQuery
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,bigquery,labelboxbigquery,labelbase
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: labelbox
+Requires-Dist: google-cloud-bigquery
+Requires-Dist: labelbase
 
 # Labelbox Connector for Google BigQuery
 
 Access the Labelbox Connector for Google BigQuery to easily perform the following functionalities:
 - `lbbq.client.create_data_rows_from_table` :   Creates Labelbox data rows (and metadata) given a BigQuery table
 - `lbbq.client.create_table_from_dataset`   :   Creates a BigQuery table given a Labelbox dataset
 - `lbbq.client.upsert_table_metadata`       :   Updates BigQuery table metadata columns given a Labelbox dataset
@@ -38,15 +41,15 @@
 * [Generate a Labelbox API key](https://labelbox.com/docs/api/getting-started#create_api_key)
 
 ## Configuration
 
 Install Labelbox-BigQuery to your Python environment. The installation will also add the Labelbox SDK and BigQuery SDK.
 
 ```
-pip install labelbox-bigquery
+pip install labelboxbigquery
 import labelboxbigquery
 ```
 
 ## Use
 
 The `client` class requires the following arguments:
 - `lb_api_key` = Labelbox API Key
```

### Comparing `labelboxbigquery-0.1.3/README.md` & `labelboxbigquery-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 * [Generate a Labelbox API key](https://labelbox.com/docs/api/getting-started#create_api_key)
 
 ## Configuration
 
 Install Labelbox-BigQuery to your Python environment. The installation will also add the Labelbox SDK and BigQuery SDK.
 
 ```
-pip install labelbox-bigquery
+pip install labelboxbigquery
 import labelboxbigquery
 ```
 
 ## Use
 
 The `client` class requires the following arguments:
 - `lb_api_key` = Labelbox API Key
```

### Comparing `labelboxbigquery-0.1.3/labelboxbigquery/client.py` & `labelboxbigquery-0.1.5/labelboxbigquery/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import labelbox
 from labelbox import Client as labelboxClient
 from labelbox.schema.data_row_metadata import DataRowMetadataKind
-from labelbase.metadata import sync_metadata_fields, get_metadata_schema_to_name_key
+from labelbase.downloader import export_and_flatten_labels
 from google.cloud import bigquery
 from google.oauth2 import service_account
+from uuid import uuid4
+import pandas as pd
+from datetime import datetime
 
 
+# BigQuery limits special characters that can be used in column names and they have to be unicode
+DIVIDER_MAPPINGS = {'&' : '\u0026', '%' : '\u0025', '>' : '\u003E', '#' : '\u0023', '|' : '\u007c'}
+
 class Client:
     """ A LabelBigQuery Client, containing a Labelbox Client and BigQuery Client Object
     Args:
         lb_api_key                  :   Required (str) - Labelbox API Key
         google_key                  :   Required (dict) - Google Service Account Permissions dict, how to create one here: https://cloud.google.com/iam/docs/creating-managing-service-account-keys#creating
         google_project_name         :   Required (str) - Google Project ID / Name
         lb_endpoint                 :   Optinoal (bool) - Labelbox GraphQL endpoint
@@ -32,17 +38,26 @@
         google_project_name=None,
         google_key=None,
         lb_endpoint='https://api.labelbox.com/graphql', 
         lb_enable_experimental=False, 
         lb_app_url="https://app.labelbox.com"):  
 
         self.lb_client = labelboxClient(lb_api_key, endpoint=lb_endpoint, enable_experimental=lb_enable_experimental, app_url=lb_app_url)
-        bq_creds = service_account.Credentials.from_service_account_file(google_key) if google_key else None
-        self.bq_client = bigquery.Client(project=google_project_name, credentials=bq_creds)
-    
+        self.bq_creds = service_account.Credentials.from_service_account_file(google_key) if google_key else None
+        self.bq_client = bigquery.Client(project=google_project_name, credentials=self.bq_creds)
+        self.google_project_name = google_project_name
+
+    def _validate_divider(self, divider):
+        unicode_divider = ''
+        for char in divider:
+            if char not in DIVIDER_MAPPINGS:
+                raise ValueError(f"Restricted character(s) found in divider - {char}. The allowed characters are {[key for key in DIVIDER_MAPPINGS.keys()]}")
+            unicode_divider += DIVIDER_MAPPINGS[char]
+        return unicode_divider
+
     def _sync_metadata_fields(self, bq_table_id, metadata_index={}):
         """ Ensures Labelbox's Metadata Ontology has all necessary metadata fields given a metadata_index
         Args:
             bq_table_id     :   Required (str) - Table ID structured in the following schema: google_project_name.dataset_name.table_name
             metadata_index  :   Optional (dict) - Dictionary where {key=column_name : value=metadata_type} - metadata_type must be one of "enum", "string", "datetime" or "number"
         Returns:
             True if the sync is successful, False if not
@@ -170,29 +185,115 @@
             errors = task.errors
             if errors:
                 print(f'Data Row Creation Error: {errors}')
                 return errors
             else:
                 upload_results.extend(task.result)
         return upload_results   
+    
+    def export_to_BigQuery(self, project, bq_dataset_id:str, bq_table_name:str, create_table:bool=False,
+                           include_metadata:bool=False, include_performance:bool=False, include_agreement:bool=False,
+                           include_label_details:bool=False, verbose:bool=False, mask_method:str="png", divider="|||",
+                           export_filters:dict=None):
+        
+        divider = self._validate_divider(divider)
+        flattened_labels_dict = export_and_flatten_labels(
+            client=self.lb_client, project=project, include_metadata=include_metadata, 
+            include_performance=include_performance, include_agreement=include_agreement,
+            include_label_details=include_label_details, mask_method=mask_method, verbose=verbose, divider=divider,
+            export_filters=export_filters
+        )
+        if len(flattened_labels_dict) == 0:
+            if verbose:
+                print("No labels were found in the project export")
+            return
+
+        #Make sure all 
+        flattened_labels_dict = [{key: str(val) for key, val in dict.items()} for dict in flattened_labels_dict]
+
+        table = pd.DataFrame.from_dict(flattened_labels_dict)
+        label_ids = table['label_id'].to_numpy()
+        labels_str = ""
+        for label_id in label_ids:
+            labels_str += "'" + label_id + "',"
+        labels_str = labels_str[:-1]
+        columns = table.columns.values.tolist()
+        table_schema = [bigquery.SchemaField(col, "STRING") for col in columns]
+        bq_table_name = bq_table_name.replace("-","_") # BigQuery tables shouldn't have "-" in them, as this causes errors when performing SQL updates
+        
+        if create_table:
+            bq_table = self.bq_client.create_table(bigquery.Table(f"{self.google_project_name}.{bq_dataset_id}.{bq_table_name}", schema=table_schema))
+            if verbose:
+                print(f'Created BigQuery Table with ID {bq_table.table_id}')
+            labels_to_insert = flattened_labels_dict
+        else:
+            bq_table = self.bq_client.get_table(bigquery.Table(f"{self.google_project_name}.{bq_dataset_id}.{bq_table_name}"))
+            query = """
+                SELECT updated_at, label_id
+                FROM {0}
+                WHERE label_id in ({1})
+            """
+            query = query.format(f"{self.google_project_name}.{bq_dataset_id}.{bq_table_name}", labels_str)
+            query_job = self.bq_client.query(query)
+            rows = list(query_job.result())
+            labels_to_update = []
+            labels_to_insert = []
+            for label in flattened_labels_dict:
+                label_in_table = False
+                for row in rows:
+                    if label['label_id'] == row[1]:
+                        label_in_table = True
+                        row_time = datetime.strptime(row[0], "%Y-%m-%dT%H:%M:%S.%f%z")
+                        label_time = datetime.strptime(label["updated_at"], "%Y-%m-%dT%H:%M:%S.%f%z")
+                        if label_time > row_time:
+                            labels_to_update.append(label)
+                if not label_in_table:
+                    labels_to_insert.append(label)
+            if len(labels_to_update) > 0:
+                job_config = bigquery.LoadJobConfig(
+                    schema=table_schema,
+                    write_disposition="WRITE_TRUNCATE",
+                )
+                job = self.bq_client.load_table_from_json(
+                    flattened_labels_dict, f"{self.google_project_name}.{bq_dataset_id}.{bq_table_name}", job_config=job_config
+                ) 
+                errors = job.result().errors
+                if not errors and verbose:
+                    print(f'Successfully updated table. {len(labels_to_update)} rows were updated and {len(labels_to_insert)} new rows were inserted')
+                elif verbose:
+                    print(errors)
+                return errors
+        if verbose:
+            print(f"inserting {len(labels_to_insert)} data rows to table")
+        errors = self.bq_client.insert_rows_json(bq_table, labels_to_insert)
+        if not errors and verbose:
+            print(f'Insert job successful')
+        elif verbose:
+            print(f"There are errors present:\n {errors}")
+        return errors
 
-    def create_data_rows_from_table(self, bq_table_id, lb_dataset, row_data_col, global_key_col=None, external_id_col=None, metadata_index={}, attachment_index={}, skip_duplicates=False):
+    def create_data_rows_from_table(
+            self, bq_table_id:str="", lb_dataset:labelbox.schema.dataset.Dataset=None, row_data_col:str="", global_key_col:str=None, 
+            external_id_col:str=None, metadata_index:dict={}, attachment_index:dict={}, skip_duplicates:bool=False, divider:str="|||"):
         """ Creates Labelbox data rows given a BigQuery table and a Labelbox Dataset
         Args:
             bq_table_id       : Required (str) - BigQuery Table ID structured in the following format: "google_project_name.dataset_name.table_name"
             lb_dataset        : Required (labelbox.schema.dataset.Dataset) - Labelbox dataset to add data rows to            
             row_data_col      : Required (str) - Column name where the data row row data URL is located
             global_key_col    : Optional (str) - Column name where the data row global key is located - defaults to the row_data column
             external_id_col   : Optional (str) - Column name where the data row external ID is located - defaults to the row_data column
             metadata_index    : Optional (dict) - Dictionary where {key=column_name : value=metadata_type} - metadata_type must be one of "enum", "string", "datetime" or "number"
             attachment_index  : Optional (dict) - Dictionary where {key=column_name : value=attachment_type} - attachment_type must be one of "IMAGE", "VIDEO", "TEXT", "HTML"
             skip_duplicates   : Optional (bool) - If True, will skip duplicate global_keys, otherwise will generate a unique global_key with a suffix "_1", "_2" and so on
+            divider           : Optional (str) - String delimiter for schema name keys and suffix added to duplocate global keys
         Returns:
             List of errors from data row upload - if successful, is an empty list
         """
+        
+        divider = self._validate_divider(divider)
         # Sync metadata index keys with metadata ontology
         check = self._sync_metadata_fields(bq_table_id, metadata_index)
         if not check:
           return None
         # Create a metadata_schema_dict where {key=metadata_field_name : value=metadata_schema_id}
         lb_mdo = self.lb_client.get_data_row_metadata_ontology()
         metadata_name_key_to_schema = self.__get_metadata_schema_to_name_key(lb_mdo, invert=True)
@@ -236,17 +337,17 @@
                     print(f'Error: No column matching metadata_index key {metadata_field_name}')
                     return None
                 else:
                     col_query+=f', {mdf}'
                     query_lookup[mdf] = index_value
                     index_value += 1
         if attachment_index:
+            attachment_whitelist = ["IMAGE", "VIDEO", "RAW_TEXT", "HTML", "TEXT_URL"]
             for attachment_field_name in attachment_index:
                 atf = attachment_field_name.replace(" ", "_")
-                attachment_whitelist = ["IMAGE", "VIDEO", "RAW_TEXT", "HTML", "TEXT_URL"]
                 if attachment_index[attachment_field_name] not in attachment_whitelist:
                     print(f'Error: Invalid value for attachment_index key {attachment_field_name} : {attachment_index[attachment_field_name]}\n must be one of {attachment_whitelist}')
                     return None
                 if atf not in column_names:
                     print(f'Error: No column matching attachment_index key {attachment_field_name}')
                     return None
                 else:
@@ -255,18 +356,23 @@
                     index_value += 1                
         # Query your row_data, external_id, global_key and metadata_index key columns from 
         query = f"""SELECT {col_query} FROM {bq_table.project}.{bq_table.dataset_id}.{bq_table.table_id}"""
         query_job = self.bq_client.query(query)
         # Iterate over your query payload to construct a list of data row dictionaries in Labelbox format
         global_key_to_upload_dict = {}
         for row in query_job:
+            if len(row[query_lookup[row_data_col]]) <= 200:
+                global_key = row[query_lookup[row_data_col]]
+            else:
+                print("Global key too long (>200 characters). Replacing with randomly generated global key.")
+                global_key = str(uuid4())
             data_row_upload_dict = {
                 "row_data" : row[query_lookup[row_data_col]],
                 "metadata_fields" : [{"schema_id":metadata_name_key_to_schema['lb_integration_source'],"value":"BigQuery"}],
-                "global_key" : str(row[query_lookup[global_key_col]])
+                "global_key" : str(global_key)
             }
             if external_id_col:
                 data_row_upload_dict['external_id'] = row[query_lookup[external_id_col]]
             if metadata_index:
                 for metadata_field_name in metadata_index:
                     mdf = metadata_field_name.replace(" ", "_")
                     metadata_schema_id = metadata_name_key_to_schema[metadata_field_name]
@@ -279,15 +385,19 @@
                         "schema_id" : metadata_schema_id,
                         "value" : metadata_value
                     })
             if attachment_index:
                 data_row_upload_dict['attachments'] = [{"type" : attachment_index[attachment_field_name], "value" : row[query_lookup[attachment_field_name]]} for attachment_field_name in attachment_index]
             global_key_to_upload_dict[row[query_lookup[global_key_col]]] = data_row_upload_dict
         # Batch upload your list of data row dictionaries in Labelbox format
+        if type(lb_dataset) == str:
+            lb_dataset = self.lb_client.get_dataset(lb_dataset)
         upload_results = self.__batch_create_data_rows(client=self.lb_client, dataset=lb_dataset, global_key_to_upload_dict=global_key_to_upload_dict)
+
+
         print(f'Success')
         return upload_results
 
     def create_table_from_dataset(self, bq_dataset_id, bq_table_name, lb_dataset, metadata_index={}):
         """ Creates a BigQuery Table from a Labelbox dataset given a BigQuery Dataset ID, desired Table name, and optional metadata_index
         Args:
             bq_dataset_id   :   Required (str) - BigQuery Dataset ID structured in the following format: "google_project_name.dataset_name"
@@ -334,14 +444,15 @@
                         else:
                             field_to_value[data_row_metadata['name']] = data_row_metadata['value']
                 for metadata_field_name in metadata_index:
                     mdf = metadata_field_name.replace(" ", "_")
                     if metadata_field_name in field_to_value.keys():
                         row_dict[mdf] = field_to_value[metadata_field_name]
             rows_to_insert.append(row_dict)
+        print(len(rows_to_insert))
         errors = self.bq_client.insert_rows_json(bq_table, rows_to_insert)
         if not errors:
             print(f'Success\nCreated BigQuery Table with ID {bq_table.table_id}')
         else:
             print(errors)
         return errors
 
@@ -436,8 +547,8 @@
                 if field_name in list(metadata_index.keys()):
                     ### Get the table value given a global key for each column in 
                     table_value = query_dict[drid_to_global_key[drid]][field_name]
                     name_key = f"{field_name}///{table_value}"
                     field.value = metadata_name_key_to_schema[name_key] if name_key in metadata_name_key_to_schema.keys() else table_value
             upload_metadata.append(labelbox.schema.data_row_metadata.DataRowMetadata(data_row_id=drid, fields=new_metadata))
         results = lb_mdo.bulk_upsert(upload_metadata)
-        return results        
+        return results
```

### Comparing `labelboxbigquery-0.1.3/labelboxbigquery/connector.py` & `labelboxbigquery-0.1.5/labelboxbigquery/connector.py`

 * *Files identical despite different names*

### Comparing `labelboxbigquery-0.1.3/labelboxbigquery.egg-info/PKG-INFO` & `labelboxbigquery-0.1.5/labelboxbigquery.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: labelboxbigquery
-Version: 0.1.3
+Version: 0.1.5
 Summary: Labelbox Connector for BigQuery
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,bigquery,labelboxbigquery,labelbase
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: labelbox
+Requires-Dist: google-cloud-bigquery
+Requires-Dist: labelbase
 
 # Labelbox Connector for Google BigQuery
 
 Access the Labelbox Connector for Google BigQuery to easily perform the following functionalities:
 - `lbbq.client.create_data_rows_from_table` :   Creates Labelbox data rows (and metadata) given a BigQuery table
 - `lbbq.client.create_table_from_dataset`   :   Creates a BigQuery table given a Labelbox dataset
 - `lbbq.client.upsert_table_metadata`       :   Updates BigQuery table metadata columns given a Labelbox dataset
@@ -38,15 +41,15 @@
 * [Generate a Labelbox API key](https://labelbox.com/docs/api/getting-started#create_api_key)
 
 ## Configuration
 
 Install Labelbox-BigQuery to your Python environment. The installation will also add the Labelbox SDK and BigQuery SDK.
 
 ```
-pip install labelbox-bigquery
+pip install labelboxbigquery
 import labelboxbigquery
 ```
 
 ## Use
 
 The `client` class requires the following arguments:
 - `lb_api_key` = Labelbox API Key
```

### Comparing `labelboxbigquery-0.1.3/setup.py` & `labelboxbigquery-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="labelboxbigquery",
-    version="0.1.03",
+    version="0.1.05",
     author="Labelbox",
     author_email="raphael@labelbox.com",
     description="Labelbox Connector for BigQuery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://labelbox.com",
     packages=setuptools.find_packages(),
```

