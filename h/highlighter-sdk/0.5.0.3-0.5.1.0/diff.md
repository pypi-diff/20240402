# Comparing `tmp/highlighter_sdk-0.5.0.3.tar.gz` & `tmp/highlighter_sdk-0.5.1.0.tar.gz`

## Comparing `highlighter_sdk-0.5.0.3.tar` & `highlighter_sdk-0.5.1.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/_colors.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/assessments.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/aws_s3.py
--rw-r--r--   0        0        0    10903 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/base_models.py
--rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/capabilities.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/const.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cropping.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/data_files.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/entity_avro_schema.py
--rw-r--r--   0        0        0    16291 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/gql_base.py
--rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/gql_client.py
--rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/io.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/itertools.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/labeled_uuid.py
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/logging.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/object_classes.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/pagination.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/presigned_url.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/tasks.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/training_config.py
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/training_runs.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/__init__.py
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/assessment.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/common.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/config.py
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/data_files.py
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/dataset.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/experiment.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/highlighter.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/object_class.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/step.py
--rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/task.py
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/cli/training_run.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/__init__.py
--rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/base_models.py
--rw-r--r--   0        0        0    38549 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/dataset.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/interfaces.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/aws_s3/__init__.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/aws_s3/writer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/__init__.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/common.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/reader.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/writer.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/highlighter/__init__.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/highlighter/reader.py
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/highlighter/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/torch_image_folder/__init__.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/torch_image_folder/reader.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/datasets/formats/torch_image_folder/writer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/splits/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/highlighter/splits/random_split.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/LICENSE
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/README.md
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/pyproject.toml
--rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.0.3/PKG-INFO
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/_colors.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/assessments.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/aws_s3.py
+-rw-r--r--   0        0        0    10903 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/base_models.py
+-rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/capabilities.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/const.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cropping.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/data_files.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/entity_avro_schema.py
+-rw-r--r--   0        0        0    16291 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/gql_base.py
+-rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/gql_client.py
+-rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/io.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/itertools.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/labeled_uuid.py
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/logging.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/object_classes.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/pagination.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/presigned_url.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/shape_utils.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/tasks.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/training_config.py
+-rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/training_runs.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/__init__.py
+-rw-r--r--   0        0        0    11612 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/assessment.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/common.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/config.py
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/data_files.py
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/dataset.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/experiment.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/highlighter.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/object_class.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/step.py
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/task.py
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/training_run.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/__init__.py
+-rw-r--r--   0        0        0    10743 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/base_models.py
+-rw-r--r--   0        0        0    38549 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/dataset.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/interfaces.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/__init__.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/writer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/__init__.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/common.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/reader.py
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/writer.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/__init__.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/reader.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/__init__.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/reader.py
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/writer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/splits/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/splits/random_split.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/LICENSE
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/README.md
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/PKG-INFO
```

### Comparing `highlighter_sdk-0.5.0.3/highlighter/__init__.py` & `highlighter_sdk-0.5.1.0/highlighter/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/_colors.py` & `highlighter_sdk-0.5.1.0/highlighter/_colors.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/assessments.py` & `highlighter_sdk-0.5.1.0/highlighter/assessments.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/aws_s3.py` & `highlighter_sdk-0.5.1.0/highlighter/aws_s3.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/base_models.py` & `highlighter_sdk-0.5.1.0/highlighter/base_models.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/capabilities.py` & `highlighter_sdk-0.5.1.0/highlighter/capabilities.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/const.py` & `highlighter_sdk-0.5.1.0/highlighter/const.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cropping.py` & `highlighter_sdk-0.5.1.0/highlighter/cropping.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/data_files.py` & `highlighter_sdk-0.5.1.0/highlighter/data_files.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/entity_avro_schema.py` & `highlighter_sdk-0.5.1.0/highlighter/entity_avro_schema.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/gql_base.py` & `highlighter_sdk-0.5.1.0/highlighter/gql_base.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/gql_client.py` & `highlighter_sdk-0.5.1.0/highlighter/gql_client.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/io.py` & `highlighter_sdk-0.5.1.0/highlighter/io.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/labeled_uuid.py` & `highlighter_sdk-0.5.1.0/highlighter/labeled_uuid.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/object_classes.py` & `highlighter_sdk-0.5.1.0/highlighter/object_classes.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/pagination.py` & `highlighter_sdk-0.5.1.0/highlighter/pagination.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/presigned_url.py` & `highlighter_sdk-0.5.1.0/highlighter/presigned_url.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/tasks.py` & `highlighter_sdk-0.5.1.0/highlighter/tasks.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/training_config.py` & `highlighter_sdk-0.5.1.0/highlighter/training_config.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/training_runs.py` & `highlighter_sdk-0.5.1.0/highlighter/training_runs.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/workflow.py` & `highlighter_sdk-0.5.1.0/highlighter/workflow.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/assessment.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/assessment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import json
 from typing import Dict, List
 
 import click
 import fastavro as avro
 import yaml
 from pydantic import BaseModel
+from shapely.wkt import loads as wkt_loads
 
 from highlighter import ENTITY_AVRO_SCHEMA, SubmissionType
 from highlighter.aws_s3 import upload_file_to_s3
 from highlighter.base_models import PageInfo
+from highlighter.const import PIXEL_LOCATION_ATTRIBUTE_UUID
 from highlighter.datasets import Dataset
 from highlighter.datasets.formats.coco.reader import CocoReader
 from highlighter.datasets.formats.highlighter.writer import (
-    CreateAssessmentPayload, HighlighterAssessmentsWriter)
+    CreateSubmissionPayload, HighlighterAssessmentsWriter)
 from highlighter.pagination import paginate
 from highlighter.assessments import (
     create_assessment_with_avro_file, get_latest_assessments_gen)
+from highlighter.shape_utils import polygon_to_multipolygon_if_self_intersecting
+
 
 ASSESSMENT_FIELDS = list(SubmissionType.__annotations__.keys())
 
 
 class AnnotationsAttributesParamType(click.ParamType):
     name = "dict"
 
@@ -59,15 +63,15 @@
     "--user-id",
     type=int,
     required=False,
     help="User ID to load submission against",
 )
 @click.option(
     "-i",
-    "--data_file-id",
+    "--data-file-id",
     type=int,
     required=True,
     help="Image ID",
 )
 @click.option(
     "-s",
     "--status",
@@ -178,21 +182,21 @@
     annotations_attributes,
     eavt_attributes,
     task_id,
     output,
 ):
     client = ctx.obj["client"]
 
-    result = client.createAssessment(
-        return_type=CreateAssessmentPayload,
+    result = client.createSubmission(
+        return_type=CreateSubmissionPayload,
         projectId=workflow_id,
         userId=user_id,
-        imageId=image_id,
+        imageId=data_file_id,
         status=status,
-        modelId=model_id,
+        modelId=capability_id,
         matchedImageId=matched_image_id,
         trainingRunId=training_run_id,
         imageQueueId=step_id,
         dataSourceId=data_source_id,
         startedAt=started_at,
         flagReason=flag_reason,
         backgroundInfoLayerFileData=background_info_layer_file_data,
@@ -243,19 +247,28 @@
     "--data-source-ids",
     type=int,
     required=False,
     help="Where the existing data_files are in Highlighter",
     default=None,
     multiple=True,
 )
+@click.option(
+    "--fix-invalid-polygons/--no-fix-invalid-polygons",
+    type=bool,
+    required=False,
+    help="Try to convert self-intersecting Polygons to MultiPolygon",
+    default=False,
+)
 
 @click.pass_context
 def create_from_dataset(
     ctx, dataset_format, data_path, workflow_id, user_id, data_source_ids,
-):
+    fix_invalid_polygons,
+    ):
+
     """Create assessments from an on disk dataset.
 
     It is expected that data_files have been uploaded already to one of the provided
     --data-source-ids. If you use `hl data_file create` with a coco dataset it will
     produce a directory containing an augmented coco dataset with symlinks mapping
     the Highlighter data_file_id to the original file path. We recommend this workflow
     in most cases.
@@ -296,14 +309,32 @@
             old_id: original_source_url_to_id[filename] for old_id, filename in old_id_filename
         }
         ds.data_files_df.loc[:, "data_file_id"] = ds.data_files_df.data_file_id.map(old_id_to_new_id)
         ds.annotations_df.loc[:, "data_file_id"] = ds.annotations_df.data_file_id.map(
             old_id_to_new_id
         )
 
+
+
+    def validate_polygons(wkt_str, fix_invalid_polygons=fix_invalid_polygons):
+        result = wkt_loads(wkt_str)
+        if (result.geom_type == "Polygon") and fix_invalid_polygons:
+            result = polygon_to_multipolygon_if_self_intersecting(result)
+
+        if not result.is_valid:
+            raise ValueError(f"Invalid pixel location shape: {result}. "
+                             "Possibly self-intersecting or un-closed Polygon. "
+                             "Try using --fix-invalid-polygons flag")
+        return result.wkt
+
+    adf = ds.annotations_df
+    validated_polys = adf[adf.attribute_id == PIXEL_LOCATION_ATTRIBUTE_UUID].value.apply(validate_polygons)
+    adf.loc[validated_polys.index, "value"] = validated_polys
+    ds.annotations_df = adf
+
     writer = HighlighterAssessmentsWriter(client, workflow_id, user_id=user_id)
     writer.write(ds)
 
 @assessment_group.command("create-from-avro")
 @click.option(
     "--avro-file",
     type=click.Path(dir_okay=False, exists=True),
```

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/common.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/common.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/config.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/config.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/data_files.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/data_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import yaml
 
 from highlighter.io import (create_data_files,
                             multithread_graphql_file_download)
 from highlighter.cli.common import _to_pathlib
 
 
-@click.group("data_file")
+@click.group("data-file")
 @click.pass_context
 def data_file_group(ctx):
     pass
 
 
 @data_file_group.command("read")
 @click.option(
@@ -34,15 +34,15 @@
     required=False,
     multiple=True,
     default=[],
     show_default=True,
 )
 @click.option(
     "-o",
-    "--data_file-dir",
+    "--data-file-dir",
     type=click.Path(exists=True, file_okay=False),
     required=True,
     help="Where to save the data_files to",
 )
 @click.pass_context
 def read(ctx, ids, paths, data_file_dir):
     client = ctx.obj["client"]
@@ -65,15 +65,15 @@
     "-i",
     "--data-source-id",
     type=int,
     required=True,
 )
 @click.option(
     "-d",
-    "--data_file-dir",
+    "--data-file-dir",
     type=click.Path(exists=True, file_okay=False),
     required=False,
     default="",
     help="Directory of data_files to upload",
     callback=_to_pathlib,
 )
 @click.option(
```

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/dataset.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/experiment.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/highlighter.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/highlighter.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/object_class.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/object_class.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/step.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/step.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/task.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/task.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/cli/training_run.py` & `highlighter_sdk-0.5.1.0/highlighter/cli/training_run.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/__init__.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/base_models.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/base_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from highlighter.labeled_uuid import LabeledUUID
 from highlighter.const import (
         OBJECT_CLASS_ATTRIBUTE_UUID,
         PIXEL_LOCATION_ATTRIBUTE_UUID,
         EMBEDDING_ATTRIBUTE_UUID,
         DATA_FILE_ATTRIBUTE_UUID,
         )
+from highlighter.shape_utils import polygon_to_multipolygon_if_self_intersecting
 
 __all__ = [
         "AttributeRecord",
         "ImageRecord",
         "S3Files",
         ]
 
@@ -146,15 +147,16 @@
         """Create a LocationAttributeValue for a polygon
 
         Args:
             coords: A sequence of (x, y [,z]) numeric coordinate pairs or triples, or
             an array-like with shape (N, 2) or (N, 3).
             Also can be a sequence of Point objects.
         """
-        value = geom.Polygon(coords).wkt
+        polygon = geom.Polygon(coords)
+        value = polygon_to_multipolygon_if_self_intersecting(polygon).wkt
         return cls(attribute_id=attribute_id, value=value, confidence=confidence)
 
     @classmethod
     def from_multpolygon_coords(cls,
                                 coords: Sequence[Sequence[Tuple[float, float]]],
                                 attribute_id: Union[LabeledUUID, UUID] = PIXEL_LOCATION_ATTRIBUTE_UUID,
                                 confidence: float = 1.0,
```

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/dataset.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/__init__.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/aws_s3/writer.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/writer.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/common.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/common.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/reader.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/reader.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/coco/writer.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/writer.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/highlighter/reader.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/reader.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/highlighter/writer.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         return True
     try:
         UUID(attr_id)
         return True
     except (ValueError, TypeError):
         return False
 
-class CreateAssessmentPayload(BaseModel):
+class CreateSubmissionPayload(BaseModel):
     submission: Optional[SubmissionType]
     errors: List[str]
 
 
 class DatumSourceInputType(BaseModel):
     pipelineId: Optional[int]
     pipelineElementId: Optional[str]
@@ -138,26 +138,26 @@
                 else:
                     warnings.warn((f"Skipping invallid attribute_id, got: '{attr_id}'"))
 
             kwargs = {"userId": self.user_id}
             kwargs = {k:v for k,v in kwargs.items() if v is not None}
 
             response = self.client.create_submission(
-                return_type=CreateAssessmentPayload,
+                return_type=CreateSubmissionPayload,
                 projectId=self.workflow_id,
                 imageId=data_file_id,
                 status="completed",
                 startedAt=datetime.now().isoformat(),
                 eavtAttributes=eavt_attrs,
                 **kwargs,
             )
 
             if (response.submission is None) or (response.errors):
                 warnings.warn(
-                    "Failed to create assessment: {} ".format(response.errors)
+                        f"Failed to create assessment: {response.errors}\n{eavt_attrs}\ndata_file: {data_file_id}\nworkflow: {self.workflow_id} "
                 )
 
             # We check if data_files_df is populated before adding these fields
             # because when we're just performing inference we may not have this
             # DataFrame populated.
             elif dataset.data_files_df.shape[0] > 0:
```

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/torch_image_folder/reader.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/reader.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/datasets/formats/torch_image_folder/writer.py` & `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/writer.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/highlighter/splits/random_split.py` & `highlighter_sdk-0.5.1.0/highlighter/splits/random_split.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/LICENSE` & `highlighter_sdk-0.5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/README.md` & `highlighter_sdk-0.5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.0.3/pyproject.toml` & `highlighter_sdk-0.5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "highlighter-sdk"
-version =  "0.5.0.3"
+version =  "0.5.1.0"
 readme = "README.md"
 description = "Package to interact with the Highlighter Perception System"
 requires-python = ">=3.7,<4.0"
 
 # From pep 0639:
 # https://peps.python.org/pep-0639/#i-have-a-private-package-that-won-t-be-distributed
 license-files = { paths = ["LICENSE"] }
```

### Comparing `highlighter_sdk-0.5.0.3/PKG-INFO` & `highlighter_sdk-0.5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: highlighter-sdk
-Version: 0.5.0.3
+Version: 0.5.1.0
 Summary: Package to interact with the Highlighter Perception System
 Project-URL: Documentation, https://highlighter-docs.netlify.app/
 Author-email: Joshua Patterson <joshua.patterson@silverpond.com.au>, Jono Chang <jonathan.chang@silverpond.com.au>, Simon Hudson <simon.hudson@silverpond.com.au>
 License-File: LICENSE
 Keywords: enterprise perception system
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

