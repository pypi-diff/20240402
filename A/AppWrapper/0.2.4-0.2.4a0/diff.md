# Comparing `tmp/AppWrapper-0.2.4.tar.gz` & `tmp/AppWrapper-0.2.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.4.tar", last modified: Tue Apr  2 02:22:29 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.4a0.tar", last modified: Tue Apr  2 02:50:04 2024, max compression
```

## Comparing `AppWrapper-0.2.4.tar` & `AppWrapper-0.2.4a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 02:22:29.000000 AppWrapper-0.2.4/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:22:29.984781 AppWrapper-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 02:22:19.000000 AppWrapper-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 02:50:04.000000 AppWrapper-0.2.4a0/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:50:04.825492 AppWrapper-0.2.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 02:49:54.000000 AppWrapper-0.2.4a0/setup.py
```

### Comparing `AppWrapper-0.2.4/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.4a0/app_wrapper/app_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._seen_so_far += bytes_amount
         percentage = round((self._seen_so_far / self._size) * 100)
         if (
             percentage in self._seen_percentages.keys()
             and not self._seen_percentages[percentage]
         ):
             self._seen_percentages[percentage] = True
-            logging.info(
+            logger.info(
                 f"Download progress for '{self._filename}': {percentage}%"
             )
 
 
 class Status(str, Enum):
     Complete = "Complete"
     Processing = "Processing"
@@ -75,15 +75,15 @@
         self.LOCAL_MODE = LOCAL_MODE
         AppWrapper.LOCAL_MODE = LOCAL_MODE
         AppWrapper.AWS_ACCESS_KEY_ID = AWS_ACCESS_KEY_ID
         AppWrapper.AWS_SECRET_ACCESS_KEY = AWS_SECRET_ACCESS_KEY
         AppWrapper.AWS_DEFAULT_REGION = AWS_DEFAULT_REGION
 
         if self.LOCAL_MODE:
-            logging.warning("This app is running in a local environment.")
+            logger.warning("This app is running in a local environment.")
         else:
             try:
                 self.TOAD_HOST = os.getenv("TOAD_HOST", None)
                 self.tenant_id = os.getenv("TENANT_ID")
                 self.task_id = os.environ["TASK_ID"]
                 AppWrapper.TOAD_HOST = self.TOAD_HOST
                 AppWrapper.task_id = self.task_id
@@ -124,27 +124,27 @@
                 "s3",
                 aws_access_key_id=AppWrapper.AWS_ACCESS_KEY_ID,
                 aws_secret_access_key=AppWrapper.AWS_SECRET_ACCESS_KEY,
                 region_name=AppWrapper.AWS_DEFAULT_REGION,
             )
 
             remote_file = s3.Bucket(bucket).Object(key)
-            logging.info(f"Starting download for '{remote_file.key}'")
+            logger.info(f"Starting download for '{remote_file.key}'")
             download_logger = S3DownloadLogger(
                 remote_file.content_length, remote_file.key
             )
 
             remote_file.download_file(download_path, Callback=download_logger)
-            logging.info(f"Finished download for '{remote_file.key}'")
+            logger.info(f"Finished download for '{remote_file.key}'")
         else:
             presigned_get_url = requests.get(
                 f"{AppWrapper.TOAD_HOST}/utils/presigned-download-url-s3/?bucket={bucket}&key={key}"
             ).json()["url"]
 
-            logging.info(f"Starting download for '{key}'")
+            logger.info(f"Starting download for '{key}'")
 
             res = requests.get(presigned_get_url, stream=True)
 
             if res.status_code != 200:
                 error_log = f"Failed: File download. \
                                     status code: {res.status_code} detail: {res.reason} \
                                     key: {key} presigned url: {presigned_get_url}"
@@ -159,16 +159,16 @@
                 parents=True, exist_ok=True
             )
             with open(download_path, "wb") as f:
                 for data in res.iter_content(chunk_size=chunk_size):
                     f.write(data)
                     bytes_so_far += len(data)
                     progress = (bytes_so_far / total_size) * 100
-                    logging.info(f"Download progress: {progress:.2f}%")
-            logging.info(f"Finished download for '{key}'")
+                    logger.info(f"Download progress: {progress:.2f}%")
+            logger.info(f"Finished download for '{key}'")
 
     def download_file_from_s3(self):
         """
         DO NOT USE THIS METHOD IN APP.
         This method is only for apps backend(toad).
         """
         for _, s3_path in enumerate(self.app_input_files):
@@ -182,15 +182,15 @@
 
             if res.status_code != 200:
                 error_log = f"Failed: File download. \
                                     status code: {res.status_code} detail: {res.reason} \
                                     file_key: {file_key} presigned url: {presigned_get_url}"
                 self.update_status(Status.Failed.value, error_log)
 
-            logging.info(f"Starting download for '{file_key}'")
+            logger.info(f"Starting download for '{file_key}'")
 
             file_path = os.path.join(self.file_folder, file_key)
             pathlib.Path(file_path).parents[0].mkdir(
                 parents=True, exist_ok=True
             )
 
             total_size = int(res.headers.get("content-length", 0))
@@ -198,16 +198,16 @@
             bytes_so_far = 0
 
             with open(file_path, "wb") as f:
                 for data in res.iter_content(chunk_size=chunk_size):
                     f.write(data)
                     bytes_so_far += len(data)
                     progress = (bytes_so_far / total_size) * 100
-                    logging.info(f"Download progress: {progress:.2f}%")
-            logging.info(f"Finished download for '{file_key}'")
+                    logger.info(f"Download progress: {progress:.2f}%")
+            logger.info(f"Finished download for '{file_key}'")
 
     def upload_file_to_s3(self, result):
         file_path = result["file_path"]
         file_name = file_path.split("/")[-1]
 
         presigned_put_url = requests.get(
             f"{self.TOAD_HOST}/utils/presigned-upload-url/?app_id={self.main_app_id}&task_id={self.task_id}&file_name={file_name}"
@@ -254,15 +254,15 @@
 
     def __call__(self, func):
         def inner(*args, **kwargs):
             if self.LOCAL_MODE:
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
-                    logging.error(e)
+                    logger.error(e)
             else:
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
                     logger.error(e)
                     logger.error(traceback.format_exc())
                     self.send_pod_log_to_s3()
```

