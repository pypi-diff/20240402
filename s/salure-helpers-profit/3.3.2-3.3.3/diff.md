# Comparing `tmp/salure_helpers_profit-3.3.2.tar.gz` & `tmp/salure_helpers_profit-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-3.3.2.tar", last modified: Wed Mar 20 12:14:27 2024, max compression
+gzip compressed data, was "dist/salure_helpers_profit-3.3.3.tar", last modified: Tue Apr  2 19:07:10 2024, max compression
```

## Comparing `salure_helpers_profit-3.3.2.tar` & `salure_helpers_profit-3.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/
--rw-r--r--   0 root         (0) root         (0)      262 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   164848 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      128 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 12:14:27.000000 salure_helpers_profit-3.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-20 12:14:05.000000 salure_helpers_profit-3.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   164848 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/setup.py
```

### Comparing `salure_helpers_profit-3.3.2/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.2/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -241,26 +241,31 @@
 
         # Checks if the column is in the metadata and if so adds it to the list of columns to convert
         columns_to_convert = [column for column in meta_data if column["id"] in data.columns]
 
         # Loops through the columns to convert and converts them to the correct datatype
         for column in columns_to_convert:
             new_type = mapping[column['dataType']]
+            col_data = data[column['id']]
+
 
             # Looks if the column is a datetime column and checks what the control type is to assign the correct type.
             # Control type are used in AFAS to determine the formatting 4 is a date, 7 is a time and 8 is a datetime.
             if new_type == "datetime64[ns]":
+                # Separated the datetime conversion from the other types to handle date objects with differening timezones
+                temp_datetime = pd.to_datetime(col_data, errors='coerce').dt.tz_localize(None)
                 if column["controlType"] == 4:
-                    data[column['id']] = data[column['id']].astype(new_type).dt.date
+                    data[column['id']] = temp_datetime.dt.date
                 elif column["controlType"] == 7:
-                    data[column['id']] = data[column['id']].astype(new_type).dt.time
+                    data[column['id']] = temp_datetime.dt.time
                 else:
-                    data[column['id']] = data[column['id']].astype(new_type)
+                    data[column['id']] = temp_datetime
             else:
-                data[column['id']] = data[column['id']].astype(new_type)
+                # Proceed with conversion for other types as normal
+                data[column['id']] = col_data.astype(new_type)
 
         # returns the dataframe with the correct datatypes
         return data
 
     # this method should be used to execute all requests so retry and raising are handled in one place
     @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_request_exception), reraise=True)
     def do_request(self, prepped_request: requests.PreparedRequest) -> requests.Response:
```

### Comparing `salure_helpers_profit-3.3.2/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.2/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_update.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.2/setup.py` & `salure_helpers_profit-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='3.3.2',
+    version='3.3.3',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

