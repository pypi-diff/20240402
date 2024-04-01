# Comparing `tmp/OperationBattleshipCommonUtilities-0.2.0.tar.gz` & `tmp/OperationBattleshipCommonUtilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OperationBattleshipCommonUtilities-0.2.0.tar", last modified: Sun Mar 24 01:48:48 2024, max compression
+gzip compressed data, was "OperationBattleshipCommonUtilities-0.3.0.tar", last modified: Mon Apr  1 21:57:51 2024, max compression
```

## Comparing `OperationBattleshipCommonUtilities-0.2.0.tar` & `OperationBattleshipCommonUtilities-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 01:48:48.967401 OperationBattleshipCommonUtilities-0.2.0/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 OperationBattleshipCommonUtilities-0.2.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-03-24 01:48:48.950806 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-03-24 01:48:48.000000 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-03-24 01:48:48.000000 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 01:48:48.000000 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-24 01:48:48.000000 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-03-24 01:48:48.000000 OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-03-24 01:48:48.950806 OperationBattleshipCommonUtilities-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 OperationBattleshipCommonUtilities-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 01:48:48.950806 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2993 2024-03-08 05:55:33.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6670 2024-03-08 05:59:13.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3164 2024-03-08 06:00:01.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0      773 2024-02-21 14:18:57.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2242 2024-03-08 06:03:38.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     2547 2024-03-08 06:04:21.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0    21398 2024-03-22 04:01:25.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     2100 2024-01-07 18:57:00.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2021 2024-01-09 06:04:28.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     2758 2024-03-19 02:54:10.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-03-24 01:48:48.967401 OperationBattleshipCommonUtilities-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-03-24 01:46:51.000000 OperationBattleshipCommonUtilities-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:57:51.685660 OperationBattleshipCommonUtilities-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 OperationBattleshipCommonUtilities-0.3.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-01 21:57:51.685660 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/
+-rw-rw-rw-   0        0        0     3177 2024-04-01 21:57:51.000000 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-01 21:57:51.000000 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 21:57:51.000000 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-01 21:57:51.000000 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-01 21:57:51.000000 OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3177 2024-04-01 21:57:51.685660 OperationBattleshipCommonUtilities-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 OperationBattleshipCommonUtilities-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 21:57:51.685660 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/
+-rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 21:51:05.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/CompanyDao.py
+-rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/FailureLogger.py
+-rw-rw-rw-   0        0        0      832 2024-04-01 21:48:28.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/GeographyHelper.py
+-rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-rw-rw-   0        0        0    17614 2024-04-01 21:47:24.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobPostingDao.py
+-rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/NomicAICaller.py
+-rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/OpenAICaller.py
+-rw-rw-rw-   0        0        0     2758 2024-03-19 02:54:10.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 21:57:51.685660 OperationBattleshipCommonUtilities-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-01 21:55:45.000000 OperationBattleshipCommonUtilities-0.3.0/setup.py
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/LICENSE` & `OperationBattleshipCommonUtilities-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `OperationBattleshipCommonUtilities-0.3.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/PKG-INFO` & `OperationBattleshipCommonUtilities-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/README.md` & `OperationBattleshipCommonUtilities-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/ApifyJobsCaller.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 import psycopg2
 
 load_dotenv('.env')
 
-# Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 class CandidateRequirementsDao:
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
@@ -35,37 +34,30 @@
         host=os.getenv("host"),
         database=os.getenv("database"),
         user=os.getenv("digitalOcean"),
         password=os.getenv("password"),
         port=os.getenv("port")
         )
         try:
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Prepare the SQL insert statement
             sql_insert_query = "INSERT INTO Candidate_Requirements (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
 
-            # Loop through each row in the DataFrame and insert it into the database
             for index, row in candidateRequirementsDataFrame.iterrows():
 
                 # Convert UUID to string before insertion
                 job_posting_id_str = str(row['job_posting_id'])
                 unique_id_str = str(row['unique_id'])
                 data = (job_posting_id_str, unique_id_str, row['item'])
                 cur.execute(sql_insert_query, data)
 
-            # Commit the transaction
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return success or some form of acknowledgment
             return "Update successful!"
 
         except Exception as e:
-            print("Database connection error:", e)
-            # Ensure connection is closed even if error occurs
+            logging.error("Database connection error:", e)
             conn.close()
             return None
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/CompanyDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/CompanyDao.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,127 +36,148 @@
         return companyDataFrame
     
     """
     When given a URL for the Company's LinkedIn Page, we want to get the UUID from the Companies Table. 
     """
     def getCompanyUuidByLinkedInUrl(self, companyLinkedinUrl):
         try:
-            # Establish a connection to the database
+            
             conn = psycopg2.connect(
                 host=os.getenv("host"),
                 database=os.getenv("database"),
-                user=os.getenv("digitalOcean"),  # Ensure correct environment variable name
+                user=os.getenv("digitalOcean"),  
                 password=os.getenv("password"),
                 port=os.getenv("port")
             )
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query with parameterized input
             cur.execute("SELECT company_id FROM Companies WHERE linkedin_url = %s", (companyLinkedinUrl,))
             
-            # Fetch all the rows
             rows = cur.fetchall()
             
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Check the number of rows returned and return the company_id
             if rows:
-                return rows[0][0]  # Assuming there's always one unique ID per LinkedIn URL
+                return rows[0][0]  
             else:
-                logging.info(f"Error in getting Company ID. We always expect an ID in this function. Failed for: {companyLinkedinUrl} ")
-                return None  # Or appropriate error handling/message
+                logging.error(f"Error in getting Company ID. We always expect an ID in this function. Failed for: {companyLinkedinUrl} ")
+                return None  
 
         except Exception as e:
-            # Log or print the error for debugging
-            print("Database connection error:", e)
-            logging.info(f"Database error in CompanyDao.getCompanyUuidByLinkedInUrl for Company at: {companyLinkedinUrl} ")
-            # Close the connection in case of error
+            
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.getCompanyUuidByLinkedInUrl for Company at: {companyLinkedinUrl} ")
             if 'conn' in locals():
                 conn.close()
             return None
     
     """
     This function will check the company table and determine if this table contains any records with this company URL. 
 
     """
     def doesCompanyExist(self, linkedInCompanyUrl):
         
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
+
             cur = conn.cursor()
             
-            # Execute the SQL query with parameterized input
             cur.execute("SELECT * FROM companies WHERE linkedin_url = %s", (linkedInCompanyUrl, ))    
             
-            # Fetch all the rows
             rows = cur.fetchall()
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Check the number of rows returned and return True or False
             return len(rows) > 0
 
         except Exception as e:
-            # Log or print the error for debugging
-            print("Database connection error:", e)
-            logging.info(f"Database error in CompanyDao.doesCompanyExist for Company at: {linkedInCompanyUrl} ")           
-            # Close the connection in case of error
+            
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.doesCompanyExist for Company at: {linkedInCompanyUrl} ")           
+            
             if 'conn' in locals():
                 conn.close()
-            return False  # You might want to return False or re-raise the exception depending on your use case
+            return False  
     
 
     def insertCompany(self, companyDataFrame):
         conn = None
         try:
-            # Establish a connection to the database
             conn = psycopg2.connect(
                 host=os.getenv("host"),
                 database=os.getenv("database"),
                 user=os.getenv("digitalOcean"),
                 password=os.getenv("password"),
                 port=os.getenv("port")
             )
-            # Create a new cursor
             cur = conn.cursor()
 
-            # SQL statement for inserting data
             insert_sql = """
             INSERT INTO Companies (
                 company_id, company_name, company_website, linkedin_url, industry, 
                 num_employees, ownership_type, about_webpage, careers_page, 
                 home_page_summary, about_page_summary, linkedin_company_summary, 
                 has_datascience, has_product_operations
             ) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
             """
 
-            # Assuming there's only one row in the DataFrame, access the first row directly
             row = companyDataFrame.iloc[0].apply(lambda x: str(x) if isinstance(x, uuid.UUID) else x)
             cur.execute(insert_sql, tuple(row))
 
-            # Commit the changes
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
+            return
+
         except Exception as e:
-            # Log or print the error for debugging
-            print("Database connection error:", e)
-            logging.info(f"Database error in CompanyDao.insertCompany for Company at: {companyDataFrame["company_name"]} ")  
-            # Close the connection in case of error
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.insertCompany for Company at: {companyDataFrame["company_name"]} ")  
             if conn:
                 conn.close()
+            return
+        
+    def getCompanyNameByCompanyId(self, company_id):
+
+        try:
+
+            conn = psycopg2.connect(
+                host=os.getenv("host"),
+                database=os.getenv("database"),
+                user=os.getenv("digitalOcean"),  
+                password=os.getenv("password"),
+                port=os.getenv("port")
+            )
+            
+            cur = conn.cursor()
+            
+            cur.execute("SELECT company_name FROM Companies WHERE company_id = %s", (company_id,))
+            
+            rows = cur.fetchall()
+            
+            cur.close()
+            conn.close()
+
+            if rows:
+                return rows[0][0]  
+            else:
+                logging.info(f"Error in getting Company Name. We always expect an name in this function. Failed for company id: {company_id} ")
+                return None  
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.getCompanyNameByCompanyId for Company at: {company_id} ")
+            
+            if 'conn' in locals():
+                conn.close()
+            return None
+
+
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/FailureLogger.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/FailureLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import json
 import logging
 import random
 from dotenv import load_dotenv
 import csv
 
-# Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 load_dotenv('.env')
 
 class FailureLogger:
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
 
+TODO: Implement this class and update other scripts to call this instead. 
+
 """
 
 import os
 from datetime import datetime
 import uuid
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 import psycopg2
 
 load_dotenv('.env')
 
-# Configure logging
+
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class GenaricDatabaseDao:
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
     def execute_select_command(sql_statement):
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/GeographyHelper.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 """
 import logging
 import re
 import pandas as pd
 
 
-# Configure logging
+
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class GeographyHelper :
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
 
     def getCityState(self, cityStateString):
 
-            # Regular expression to match the patterns "City, State" or "State, Country"
+        # Regular expression to match the patterns "City, State" or "State, Country"
         pattern = re.compile(r"([A-Za-z\s\-]+)(?:, )?([A-Z]{2})?")
 
         # Apply the pattern to the string
         match = pattern.match(cityStateString)
 
         # Initialize city and state as None
         city, state = None, None
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobKeyWordsDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 import psycopg2
 
 load_dotenv('.env')
 
-# Configure logging
+
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class JobKeyWordsDao :
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
 
@@ -28,38 +28,72 @@
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
         )
         try:
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Prepare the SQL insert statement
             sql_insert_query = "INSERT INTO Job_Keywords (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
 
-            # Loop through each row in the DataFrame and insert it into the database
             for index, row in jobKeyWordsDataFrame.iterrows():
 
                 # Convert UUID to string before insertion
                 job_posting_id_str = str(row['job_posting_id'])
                 unique_id_str = str(row['unique_id'])
                 data = (job_posting_id_str, unique_id_str, row['item'])
                 cur.execute(sql_insert_query, data)
                 
-            # Commit the transaction
-
+            
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return success or some form of acknowledgment
             return "Update successful!"
 
         except Exception as e:
-            print("Database connection error:", e)
-            # Ensure connection is closed even if error occurs
+            logging.error("Database connection error:", e)
             conn.close()
             return None
+        
+
+
+    def getKeywordsForJobID(self, job_posting_id):
+
+        """
+        This function calls the Job Keywords Table to find all the records that have the given job_posting_id 
+        
+        Returns the list as a Pandas DataFrame
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+
+            cur = conn.cursor()
+            
+            sql_select_query = "SELECT * FROM job_keywords WHERE job_posting_id = %s"
+            cur.execute(sql_select_query, (job_posting_id,))  
+
+            rows = cur.fetchall()
+
+            if rows:
+                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
+            else:
+                df = pd.DataFrame()
+
+            cur.close()
+            conn.close()
+
+            return df
+
+        except Exception as e:
+            logging.error(f"Database connection error in getSkillsForJobID: {e}")
+            conn.close()
+            return pd.DataFrame()
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobPostingDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobPostingDao.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 import psycopg2
 
 load_dotenv('.env')
 
-# Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 class JobPostingDao:
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
@@ -31,78 +30,61 @@
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings WHERE job_category IN ('Product_Management', 'Data_Science')")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getAllDataScienceOrProductCategorizedJobs(). ")  
             conn.close()
         return
 
-
-        return 
-    
     def getAllProductManagerJobs(self):
         """
         This fuction calls the Job Posting Table to find all the records that contain either AI or Product Manager in the title.  
     
         """
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
-            
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%')")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getAllProductManagerJobs. ")  
             conn.close()
         return
     
     """
     This method will update the given LinkedIn Job Posting with today's date for most recent updated date. 
     """
     def updateLinkedInJobRecordUpdatedDate(self, jobUrl):
@@ -111,43 +93,37 @@
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
         )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
             # Code to construct a SQL query from the job_posting dataframe
             # Assuming job_posting is a single record from your DataFrame
             sql_update_query = """
             UPDATE job_postings
             SET job_last_collected_date = %s
             WHERE posting_url = %s;
             """
-            # Prepare data tuple to be updated
             todaysDate = datetime.now().replace(hour=0, minute=0, second=0, microsecond=0).strftime('%Y-%m-%d %H:%M:%S'), 
             data = (todaysDate, jobUrl)
             
-            # Execute the SQL query
             cur.execute(sql_update_query, data)
             
-            # Commit the transaction
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return success or some form of acknowledgment
             return "Update successful!"
 
         except Exception as e:
-            print("Database connection error:", e)
+            logging.error("Database connection error:", e)
             conn.close()
             return None
     
     def update_job_posting(self, job_posting):
  
         # Dynamically build the SET part of the SQL statement
         set_sql = ', '.join([f"{col} = %s" for col in job_posting.index if col != 'job_posting_id'])
@@ -189,155 +165,131 @@
             try:
                 formatted_sql = cur.mogrify(sql_update_query, data).decode("utf-8")
                 logging.error("Formatted SQL sent to DB: %s", formatted_sql)
             except Exception as mogrify_error:
                 logging.error("Error formatting SQL: %s", mogrify_error)
 
         finally:
-            # Close the connection if it's open
+            
             if conn is not None:
                 conn.close()
 
     
     def fetchPmJobsRequiringEnrichment(sef):
         """
         This fuction calls the Job Posting Table to find all the PM records that need further enrichment. 
         This process adds salary details, AI Details and basic job description info. 
         """
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%') AND is_ai IS NULL order by job_posting_date desc;")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
             conn.close()
             return None
 
 
     def fetchJobsRequiringEnrichment(self):
         """
         This fuction calls the Job Posting Table to find all the records that need further enrichment. 
         This process adds salary details, AI Details and basic job description info. 
         """
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings WHERE is_ai IS NULL")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
-
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.fetchJobsRequiringEnrichment(). ")  
             conn.close()
             return None
     
     def checkIfJobExists(self, cleanedLinkedInJobURL):
         try:
-            # Establish a connection to the database
             conn = psycopg2.connect(
                 host=os.getenv("host"),
                 database=os.getenv("database"),
-                user=os.getenv("digitalOcean"),  # Assuming this is the correct env variable name
+                user=os.getenv("digitalOcean"),  
                 password=os.getenv("password"),
                 port=os.getenv("port")
             )
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Prepare the SQL command
             sql_command = "SELECT * FROM job_postings WHERE posting_url = %s"
             
-            
-
-            # Execute the SQL command
             cur.execute(sql_command, (cleanedLinkedInJobURL, ))
             
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Check the number of rows returned and return True or False
             return len(rows) > 0
 
         except Exception as e:
-            # Log or print the error for debugging
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.checkIfJobExists for Job at: {cleanedLinkedInJobURL} ")  
+            
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.checkIfJobExists for Job at: {cleanedLinkedInJobURL} ")  
             
             mogrified_query = cur.mogrify(sql_command, (cleanedLinkedInJobURL, )).decode('utf-8')
-            logging.info(f"Executing SQL command: {mogrified_query}")
-            # Close the connection in case of error
+            logging.error(f"Error occurred while Executing SQL command: {mogrified_query}")
+           
             if 'conn' in locals():
                 conn.close()
-            return False  # You might want to return False or re-raise the exception depending on your use case
+            return False  
         
 
     def insertNewJobRecord(self, jobpostingDataFrame):
 
         conn = None
         try:
-            # Establish a connection to the database
+           
             conn = psycopg2.connect(
                 host=os.getenv("host"),
                 database=os.getenv("database"),
                 user=os.getenv("digitalOcean"),
                 password=os.getenv("password"),
                 port=os.getenv("port")
             )
-            # Create a new cursor
+           
             cur = conn.cursor()
 
             # SQL statement for inserting data
             insert_sql = """INSERT INTO job_postings (
                 job_posting_id, company_id, posting_url, posting_source, posting_source_id, job_title,
                  full_posting_description, job_description, is_ai, job_salary, job_posting_company_information, 
                  job_posting_date, job_insertion_date, job_last_collected_date, job_active, city, state
@@ -358,162 +310,139 @@
             cur.close()
             conn.close()
             return 1
 
         except Exception as e:
             # Log or print the error for debugging
 
-            logging.info(f"Database error: {e}")
-            logging.info(f"Database error in JobPosting.insertNewJobRecord for Job at: {jobpostingDataFrame["posting_url"]} ")
-            logging.info(f"Executing SQL: {insert_sql} with data: {tuple(row)}")  
-            # Close the connection in case of error
+            logging.error(f"Database error: {e}")
+            logging.error(f"Database error in JobPosting.insertNewJobRecord for Job at: {jobpostingDataFrame["posting_url"]} ")
+            logging.error(f"Executing SQL: {insert_sql} with data: {tuple(row)}")  
+            
             if conn:
                 conn.close() 
             
             return -1
         
     def getAllJobs(self):
         """
         This fuction calls the Job Posting Table to find all the records and returns them to the user as a pandas pd 
         """
-        # Establish a connection to the database
+        
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
             conn.close()
             return None
         
     def getCurrentJobsIdsAsDataFrame(self):
         """
         This fuction calls the Job Posting Table to find all the records and returns them to the user as a pandas pd 
         """
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT posting_url FROM job_postings")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getCurrentJobsIdsAsDataFrame. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getCurrentJobsIdsAsDataFrame. ")  
             conn.close()
             return None
     
     def getProductManagerJobs(self):
 
         return
     
     def getUncategorizedJobs(self):
         
         """
         This fuction calls the Job Posting Table to find all the PM records that need further enrichment. 
         This process adds salary details, AI Details and basic job description info. 
         """
-        # Establish a connection to the database
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
             
-            # Execute the SQL query. We know that the is_ai column will be null when the data is raw. 
             cur.execute("SELECT * FROM job_postings WHERE job_category is null;")
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return the DataFrame
+
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
-            logging.info(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in JobPosting.getUnprocessedAiClassificationJobs. ")  
             conn.close()
             return None
 
-
-        return
     
     def getjobsFromListOfJobsIds(self, dataframeOfJobIds):
         """
         Purpose: When given a list of Job_Ids, this function will call the job_postings table and return the list of jobs that match the given IDs. 
 
         Args:
             dataframeOfJobIds: Pandas Dataframe where one column contains 'id' and this corresponds to job_posting_id in the Postgres DB
 
         Return Value:
             Pandas Dataframe of each job record, company name and aother associated metadata.  
         """
         job_ids = dataframeOfJobIds['job_posting_id'].tolist()
 
-        # Convert list of job_ids to tuple for SQL query
         job_ids_tuple = tuple(job_ids)
 
-        # SQL query
         sql_query = f"""
         SELECT
             c.company_name,
             jp.job_title,
             jp.posting_url,
             jp.full_posting_description,
             jp.job_description,
@@ -541,41 +470,36 @@
         FROM
             job_postings jp
         JOIN
             companies c ON jp.company_id = c.company_id
         WHERE
             jp.job_posting_id IN %s;
         """
-        # Establish a connection to the database
+        
         conn = psycopg2.connect(
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
             )
         try:
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Execute the SQL query with parameterized input for safety
             cur.execute(sql_query, (job_ids_tuple,))
 
-            # Fetch all the rows
             rows = cur.fetchall()
 
-            # Convert the results into a pandas DataFrame
             if rows:
                 df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
             else:
                 df = pd.DataFrame()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
             return df
 
         except Exception as e:
-            print("Database connection error:", e)
+            logging.error("Database connection error:", e)
             conn.close()
             return pd.DataFrame()
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 import psycopg2
 
 load_dotenv('.env')
 
-# Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-
 class JobResponsibilitiesDao :
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
 
     def insertJobResponsibilitiesForJobPosting(self, jobResponsibilitiesDataFrame):
         """
@@ -26,37 +24,30 @@
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
         )
         try:
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Prepare the SQL insert statement
             sql_insert_query = "INSERT INTO Job_Responsibilities (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
 
-            # Loop through each row in the DataFrame and insert it into the database
             for index, row in jobResponsibilitiesDataFrame.iterrows():
 
                 # Convert UUID to string before insertion
                 job_posting_id_str = str(row['job_posting_id'])
                 unique_id_str = str(row['unique_id'])
                 data = (job_posting_id_str, unique_id_str, row['item'])
                 cur.execute(sql_insert_query, data)
                 
-            # Commit the transaction
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return success or some form of acknowledgment
             return "Update successful!"
 
         except Exception as e:
-            print("Database connection error:", e)
-            # Ensure connection is closed even if error occurs
+            logging.error("Database connection error:", e)
             conn.close()
             return None
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobSkillsDao.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,38 +24,72 @@
             host=os.getenv("host"),
             database=os.getenv("database"),
             user=os.getenv("digitalOcean"),
             password=os.getenv("password"),
             port=os.getenv("port")
         )
         try:
-            # Create a new cursor
             cur = conn.cursor()
 
-            # Prepare the SQL insert statement
             sql_insert_query = "INSERT INTO Job_Skills (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
 
-            # Loop through each row in the DataFrame and insert it into the database
             for index, row in jobSkillsDataFrame.iterrows():
 
                 # Convert UUID to string before insertion
                 job_posting_id_str = str(row['job_posting_id'])
                 unique_id_str = str(row['unique_id'])
                 data = (job_posting_id_str, unique_id_str, row['item'])
                 cur.execute(sql_insert_query, data)
                 
                 
-            # Commit the transaction
             conn.commit()
 
-            # Close the cursor and connection
             cur.close()
             conn.close()
 
-            # Return success or some form of acknowledgment
             return "Update successful!"
 
         except Exception as e:
-            print("Database connection error:", e)
-            # Ensure connection is closed even if error occurs
+            logging.error("Database connection error:", e)
             conn.close()
             return None
+        
+
+    def getSkillsForJobID(self, job_posting_id):
+
+        """
+        This function calls the Job Skills Table to find all the records that have the given job_posting_id 
+        
+        Returns the list as a Pandas DataFrame
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+
+            cur = conn.cursor()
+            
+            sql_select_query = "SELECT * FROM job_skills WHERE job_posting_id = %s"
+            cur.execute(sql_select_query, (job_posting_id,))  
+
+            rows = cur.fetchall()
+
+            if rows:
+                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
+            else:
+                df = pd.DataFrame()
+
+            cur.close()
+            conn.close()
+
+            return df
+
+        except Exception as e:
+            logging.error(f"Database connection error in getSkillsForJobID: {e}")
+            conn.close()
+            return pd.DataFrame()  
+
```

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/NomicAICaller.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/OpenAICaller.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `OperationBattleshipCommonUtilities-0.3.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.2.0/setup.py` & `OperationBattleshipCommonUtilities-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.2.0',
+    version='0.3.0',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

