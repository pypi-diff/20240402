# Comparing `tmp/AppWrapper-0.2.4a0.tar.gz` & `tmp/AppWrapper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.4a0.tar", last modified: Tue Apr  2 02:50:04 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.5.tar", last modified: Tue Apr  2 03:24:00 2024, max compression
```

## Comparing `AppWrapper-0.2.4a0.tar` & `AppWrapper-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.228889 AppWrapper-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.228889 AppWrapper-0.2.5/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 03:24:00.000000 AppWrapper-0.2.5/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 03:24:00.000000 AppWrapper-0.2.5/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:24:00.000000 AppWrapper-0.2.5/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 03:24:00.000000 AppWrapper-0.2.5/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 03:24:00.000000 AppWrapper-0.2.5/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 03:24:00.228889 AppWrapper-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 03:23:49.000000 AppWrapper-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.228889 AppWrapper-0.2.5/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 03:23:49.000000 AppWrapper-0.2.5/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-02 03:23:49.000000 AppWrapper-0.2.5/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:24:00.228889 AppWrapper-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 03:23:49.000000 AppWrapper-0.2.5/setup.py
```

### Comparing `AppWrapper-0.2.4a0/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.5/app_wrapper/app_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,24 +189,25 @@
             logger.info(f"Starting download for '{file_key}'")
 
             file_path = os.path.join(self.file_folder, file_key)
             pathlib.Path(file_path).parents[0].mkdir(
                 parents=True, exist_ok=True
             )
 
-            total_size = int(res.headers.get("content-length", 0))
-            chunk_size = int(total_size / 10)
-            bytes_so_far = 0
+            # total_size = int(res.headers.get("content-length", 0))
+            # chunk_size = int(total_size / 10)
+            # bytes_so_far = 0
 
             with open(file_path, "wb") as f:
-                for data in res.iter_content(chunk_size=chunk_size):
-                    f.write(data)
-                    bytes_so_far += len(data)
-                    progress = (bytes_so_far / total_size) * 100
-                    logger.info(f"Download progress: {progress:.2f}%")
+                f.write(res.content)
+                # for data in res.iter_content(chunk_size=chunk_size):
+                #     f.write(data)
+                #     bytes_so_far += len(data)
+                #     progress = (bytes_so_far / total_size) * 100
+                #     logger.info(f"Download progress: {progress:.2f}%")
             logger.info(f"Finished download for '{file_key}'")
 
     def upload_file_to_s3(self, result):
         file_path = result["file_path"]
         file_name = file_path.split("/")[-1]
 
         presigned_put_url = requests.get(
```

