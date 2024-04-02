# Comparing `tmp/windmill_train-1.0.0.8-py3-none-any.whl.zip` & `tmp/windmill_train-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8333 bytes, number of entries: 11
--rw-r--r--  2.0 unx      236 b- defN 24-Mar-18 09:39 windmilltrainingv1/__init__.py
--rw-r--r--  2.0 unx      236 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/__init__.py
--rw-r--r--  2.0 unx      916 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/training_api_dataset.py
--rw-r--r--  2.0 unx      633 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/training_api_job.py
--rw-r--r--  2.0 unx     1044 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/training_api_pipeline.py
--rw-r--r--  2.0 unx      736 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/training_api_project.py
--rw-r--r--  2.0 unx    25394 b- defN 24-Mar-18 09:39 windmilltrainingv1/client/training_client.py
--rw-r--r--  2.0 unx      681 b- defN 24-Mar-18 09:39 windmill_train-1.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 09:39 windmill_train-1.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Mar-18 09:39 windmill_train-1.0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1032 b- defN 24-Mar-18 09:39 windmill_train-1.0.0.8.dist-info/RECORD
-11 files, 31019 bytes uncompressed, 6539 bytes compressed:  78.9%
+Zip file size: 8325 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      236 b- defN 24-Mar-18 15:18 windmilltrainingv1/__init__.py
+-rw-r--r--  2.0 unx      236 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/__init__.py
+-rw-r--r--  2.0 unx      916 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/training_api_dataset.py
+-rw-r--r--  2.0 unx      633 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/training_api_job.py
+-rw-r--r--  2.0 unx     1044 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/training_api_pipeline.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/training_api_project.py
+-rw-r--r--  2.0 unx    25345 b- defN 24-Mar-18 15:18 windmilltrainingv1/client/training_client.py
+-rw-r--r--  2.0 unx      681 b- defN 24-Mar-18 15:18 windmill_train-1.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 15:18 windmill_train-1.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Mar-18 15:18 windmill_train-1.0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1032 b- defN 24-Mar-18 15:18 windmill_train-1.0.0.9.dist-info/RECORD
+11 files, 30970 bytes uncompressed, 6531 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: windmilltrainingv1/client/training_api_project.py
 Comment: 
 
 Filename: windmilltrainingv1/client/training_client.py
 Comment: 
 
-Filename: windmill_train-1.0.0.8.dist-info/METADATA
+Filename: windmill_train-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: windmill_train-1.0.0.8.dist-info/WHEEL
+Filename: windmill_train-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: windmill_train-1.0.0.8.dist-info/top_level.txt
+Filename: windmill_train-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: windmill_train-1.0.0.8.dist-info/RECORD
+Filename: windmill_train-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## windmilltrainingv1/client/training_client.py

```diff
@@ -30,19 +30,19 @@
             config (Optional[BceClientConfiguration]): The client configuration to use.
             ak (Optional[str]): Access key for authentication.
             sk (Optional[str]): Secret key for authentication.
             endpoint (Optional[str]): The service endpoint URL.
     """
 
     def __init__(self, config: Optional[BceClientConfiguration] = None, ak: Optional[str] = "",
-                 sk: Optional[str] = "", endpoint: Optional[str] = "", context: Optional[dict] = None):
+                 sk: Optional[str] = "", endpoint: Optional[str] = ""):
         """
         Initialize the TrainingClient with the provided configuration.
         """
-        super(TrainingClient, self).__init__(config=config, ak=ak, sk=sk, endpoint=endpoint, context=context)
+        super(TrainingClient, self).__init__(config=config, ak=ak, sk=sk, endpoint=endpoint)
 
     """
     job api
     """
 
     def create_job(self, workspace_id: str,
                    project_name: str,
```

## Comparing `windmill_train-1.0.0.8.dist-info/METADATA` & `windmill_train-1.0.0.9.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-train
-Version: 1.0.0.8
+Version: 1.0.0.9
 Summary: sdk in python for windmill artifact
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-train/blob/master/sdk/python/training_client.py
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `windmill_train-1.0.0.8.dist-info/RECORD` & `windmill_train-1.0.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 windmilltrainingv1/__init__.py,sha256=-40HavO7yr8NLlSFfBgNmfscw7UhsKjE83dguUuejbY,236
 windmilltrainingv1/client/__init__.py,sha256=-40HavO7yr8NLlSFfBgNmfscw7UhsKjE83dguUuejbY,236
 windmilltrainingv1/client/training_api_dataset.py,sha256=SQYCaVLXHNOhBieVWhT-BCgkc9m1FpOtkQREhXSjEd8,916
 windmilltrainingv1/client/training_api_job.py,sha256=NwCrAFY7lQqb4qlmNVWRl4a1nO0h0X405qlHmlEW4hs,633
 windmilltrainingv1/client/training_api_pipeline.py,sha256=afUX2D1BSZXNECspjNd0eCqc3owvUYiz1Fg2v7iXInc,1044
 windmilltrainingv1/client/training_api_project.py,sha256=VHSdPaTZhYMvfj7iY0UWKDxDLn5WfntSXccfJhQDlO0,736
-windmilltrainingv1/client/training_client.py,sha256=c3nqJiQx1nDZyg72QjukGonGl2xLWhlxa8tJQIEi4Wg,25394
-windmill_train-1.0.0.8.dist-info/METADATA,sha256=HiXksOBsfX0AGD8K7-nqRS88HmM4hBn12hyzIy6kVb8,681
-windmill_train-1.0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-windmill_train-1.0.0.8.dist-info/top_level.txt,sha256=X5extS0ERqY2Xoyd5tZ2C6CYkrkcDSpTxmjsIERA24o,19
-windmill_train-1.0.0.8.dist-info/RECORD,,
+windmilltrainingv1/client/training_client.py,sha256=lg_FIXcFWwbgBO7uaFh1JT4Cz1a5p7VL5nLp3TAQsJg,25345
+windmill_train-1.0.0.9.dist-info/METADATA,sha256=LcWtQHgF-HCnNBUjgvyQIGFR6tCRxx8vmfb9kTDvQXo,681
+windmill_train-1.0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+windmill_train-1.0.0.9.dist-info/top_level.txt,sha256=X5extS0ERqY2Xoyd5tZ2C6CYkrkcDSpTxmjsIERA24o,19
+windmill_train-1.0.0.9.dist-info/RECORD,,
```

