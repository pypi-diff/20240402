# Comparing `tmp/AppWrapper-0.2.3.tar.gz` & `tmp/AppWrapper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.3.tar", last modified: Mon Mar 25 07:31:36 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.4.tar", last modified: Tue Apr  2 02:22:29 2024, max compression
```

## Comparing `AppWrapper-0.2.3.tar` & `AppWrapper-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:31:36.322881 AppWrapper-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:31:36.322881 AppWrapper-0.2.3/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 07:31:36.000000 AppWrapper-0.2.3/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 07:31:36.000000 AppWrapper-0.2.3/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 07:31:36.000000 AppWrapper-0.2.3/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 07:31:36.000000 AppWrapper-0.2.3/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 07:31:36.000000 AppWrapper-0.2.3/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 07:31:36.322881 AppWrapper-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 07:31:25.000000 AppWrapper-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:31:36.322881 AppWrapper-0.2.3/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 07:31:25.000000 AppWrapper-0.2.3/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-25 07:31:25.000000 AppWrapper-0.2.3/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 07:31:36.322881 AppWrapper-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-25 07:31:25.000000 AppWrapper-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/setup.py
```

### Comparing `AppWrapper-0.2.3/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.4/app_wrapper/app_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,20 +182,32 @@
 
             if res.status_code != 200:
                 error_log = f"Failed: File download. \
                                     status code: {res.status_code} detail: {res.reason} \
                                     file_key: {file_key} presigned url: {presigned_get_url}"
                 self.update_status(Status.Failed.value, error_log)
 
+            logging.info(f"Starting download for '{file_key}'")
+
             file_path = os.path.join(self.file_folder, file_key)
             pathlib.Path(file_path).parents[0].mkdir(
                 parents=True, exist_ok=True
             )
+
+            total_size = int(res.headers.get("content-length", 0))
+            chunk_size = int(total_size / 10)
+            bytes_so_far = 0
+
             with open(file_path, "wb") as f:
-                f.write(res.content)
+                for data in res.iter_content(chunk_size=chunk_size):
+                    f.write(data)
+                    bytes_so_far += len(data)
+                    progress = (bytes_so_far / total_size) * 100
+                    logging.info(f"Download progress: {progress:.2f}%")
+            logging.info(f"Finished download for '{file_key}'")
 
     def upload_file_to_s3(self, result):
         file_path = result["file_path"]
         file_name = file_path.split("/")[-1]
 
         presigned_put_url = requests.get(
             f"{self.TOAD_HOST}/utils/presigned-upload-url/?app_id={self.main_app_id}&task_id={self.task_id}&file_name={file_name}"
```

