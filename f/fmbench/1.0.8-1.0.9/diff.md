# Comparing `tmp/fmbench-1.0.8.tar.gz` & `tmp/fmbench-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmbench-1.0.8.tar", max compression
+gzip compressed data, was "fmbench-1.0.9.tar", max compression
```

## Comparing `fmbench-1.0.8.tar` & `fmbench-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      962 2024-02-12 14:06:15.239728 fmbench-1.0.8/LICENSE
--rw-r--r--   0        0        0      779 2024-02-14 03:04:40.179528 fmbench-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    17847 2024-02-13 22:11:50.775285 fmbench-1.0.8/README.md
--rw-r--r--   0        0        0    26418 2024-02-13 18:58:11.244466 fmbench-1.0.8/src/fmbench/1_generate_data.ipynb
--rw-r--r--   0        0        0    28554 2024-02-13 18:58:11.296586 fmbench-1.0.8/src/fmbench/2_deploy_model.ipynb
--rw-r--r--   0        0        0    47105 2024-02-13 04:48:31.182285 fmbench-1.0.8/src/fmbench/3_run_inference.ipynb
--rw-r--r--   0        0        0    48485 2024-02-14 03:01:00.798450 fmbench-1.0.8/src/fmbench/4_model_metric_analysis.ipynb
--rw-r--r--   0        0        0    17642 2024-02-13 04:48:31.190184 fmbench-1.0.8/src/fmbench/5_cleanup.ipynb
--rw-r--r--   0        0        0        0 2024-02-13 04:48:31.191177 fmbench-1.0.8/src/fmbench/__init__.py
--rw-r--r--   0        0        0       57 2024-02-13 04:48:31.192177 fmbench-1.0.8/src/fmbench/config_filepath.txt
--rw-r--r--   0        0        0     9430 2024-02-13 04:48:31.194170 fmbench-1.0.8/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-quick.yml
--rw-r--r--   0        0        0     9387 2024-02-13 04:48:31.196170 fmbench-1.0.8/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-v1.yml
--rw-r--r--   0        0        0     5248 2024-02-13 04:48:31.197160 fmbench-1.0.8/src/fmbench/configs/config-llama2-70b-g5-p4d-tgi.yml
--rw-r--r--   0        0        0     5585 2024-02-13 04:48:31.199153 fmbench-1.0.8/src/fmbench/configs/config-llama2-70b-g5-p4d-trt.yml
--rw-r--r--   0        0        0     5124 2024-02-14 02:59:37.677398 fmbench-1.0.8/src/fmbench/configs/config-llama2-7b-g5-quick.yml
--rw-r--r--   0        0        0     4182 2024-02-13 04:53:09.680756 fmbench-1.0.8/src/fmbench/configs/config-mistral-7b-tgi-g5.yml
--rw-r--r--   0        0        0     7356 2024-02-14 03:01:13.524941 fmbench-1.0.8/src/fmbench/globals.py
--rw-r--r--   0        0        0     5268 2024-02-13 14:14:33.449850 fmbench-1.0.8/src/fmbench/main.py
--rw-r--r--   0        0        0      371 2024-02-13 04:48:31.205239 fmbench-1.0.8/src/fmbench/prompt_template/prompt_template.txt
--rw-r--r--   0        0        0      126 2024-02-13 04:48:31.205736 fmbench-1.0.8/src/fmbench/requirements.txt
--rw-r--r--   0        0        0     1262 2024-02-13 04:48:31.207235 fmbench-1.0.8/src/fmbench/scripts/jumpstart.py
--rw-r--r--   0        0        0     7085 2024-02-13 04:48:31.208232 fmbench-1.0.8/src/fmbench/scripts/p4d_djl.py
--rw-r--r--   0        0        0     4781 2024-02-13 04:48:31.209229 fmbench-1.0.8/src/fmbench/scripts/p4d_hf_tgi.py
--rw-r--r--   0        0        0      259 2024-02-13 04:48:31.210225 fmbench-1.0.8/src/fmbench/scripts/p4d_serving.properties
--rw-r--r--   0        0        0     9941 2024-02-14 03:01:12.728539 fmbench-1.0.8/src/fmbench/utils.py
--rw-r--r--   0        0        0    18476 1970-01-01 00:00:00.000000 fmbench-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      962 2024-02-12 14:06:15.239728 fmbench-1.0.9/LICENSE
+-rw-r--r--   0        0        0      779 2024-02-14 03:10:27.241471 fmbench-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    17847 2024-02-13 22:11:50.775285 fmbench-1.0.9/README.md
+-rw-r--r--   0        0        0    26418 2024-02-13 18:58:11.244466 fmbench-1.0.9/src/fmbench/1_generate_data.ipynb
+-rw-r--r--   0        0        0    28554 2024-02-13 18:58:11.296586 fmbench-1.0.9/src/fmbench/2_deploy_model.ipynb
+-rw-r--r--   0        0        0    47105 2024-02-13 04:48:31.182285 fmbench-1.0.9/src/fmbench/3_run_inference.ipynb
+-rw-r--r--   0        0        0    48454 2024-02-14 03:09:59.846561 fmbench-1.0.9/src/fmbench/4_model_metric_analysis.ipynb
+-rw-r--r--   0        0        0    17642 2024-02-13 04:48:31.190184 fmbench-1.0.9/src/fmbench/5_cleanup.ipynb
+-rw-r--r--   0        0        0        0 2024-02-13 04:48:31.191177 fmbench-1.0.9/src/fmbench/__init__.py
+-rw-r--r--   0        0        0       57 2024-02-13 04:48:31.192177 fmbench-1.0.9/src/fmbench/config_filepath.txt
+-rw-r--r--   0        0        0     9430 2024-02-13 04:48:31.194170 fmbench-1.0.9/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-quick.yml
+-rw-r--r--   0        0        0     9387 2024-02-13 04:48:31.196170 fmbench-1.0.9/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-v1.yml
+-rw-r--r--   0        0        0     5248 2024-02-13 04:48:31.197160 fmbench-1.0.9/src/fmbench/configs/config-llama2-70b-g5-p4d-tgi.yml
+-rw-r--r--   0        0        0     5585 2024-02-13 04:48:31.199153 fmbench-1.0.9/src/fmbench/configs/config-llama2-70b-g5-p4d-trt.yml
+-rw-r--r--   0        0        0     5124 2024-02-14 02:59:37.677398 fmbench-1.0.9/src/fmbench/configs/config-llama2-7b-g5-quick.yml
+-rw-r--r--   0        0        0     4182 2024-02-13 04:53:09.680756 fmbench-1.0.9/src/fmbench/configs/config-mistral-7b-tgi-g5.yml
+-rw-r--r--   0        0        0     7356 2024-02-14 03:01:13.524941 fmbench-1.0.9/src/fmbench/globals.py
+-rw-r--r--   0        0        0     5268 2024-02-13 14:14:33.449850 fmbench-1.0.9/src/fmbench/main.py
+-rw-r--r--   0        0        0      371 2024-02-13 04:48:31.205239 fmbench-1.0.9/src/fmbench/prompt_template/prompt_template.txt
+-rw-r--r--   0        0        0      126 2024-02-13 04:48:31.205736 fmbench-1.0.9/src/fmbench/requirements.txt
+-rw-r--r--   0        0        0     1262 2024-02-13 04:48:31.207235 fmbench-1.0.9/src/fmbench/scripts/jumpstart.py
+-rw-r--r--   0        0        0     7085 2024-02-13 04:48:31.208232 fmbench-1.0.9/src/fmbench/scripts/p4d_djl.py
+-rw-r--r--   0        0        0     4781 2024-02-13 04:48:31.209229 fmbench-1.0.9/src/fmbench/scripts/p4d_hf_tgi.py
+-rw-r--r--   0        0        0      259 2024-02-13 04:48:31.210225 fmbench-1.0.9/src/fmbench/scripts/p4d_serving.properties
+-rw-r--r--   0        0        0     9941 2024-02-14 03:01:12.728539 fmbench-1.0.9/src/fmbench/utils.py
+-rw-r--r--   0        0        0    18476 1970-01-01 00:00:00.000000 fmbench-1.0.9/PKG-INFO
```

### Comparing `fmbench-1.0.8/LICENSE` & `fmbench-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/pyproject.toml` & `fmbench-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fmbench"
-version = "1.0.8"
+version = "1.0.9"
 description ="Benchmark performance of **any model** on **any supported instance type** on Amazon SageMaker."
 authors = ["Amit Arora <aroraai@amazon.com>", "Madhur prashant <Madhurpt@amazon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
```

### Comparing `fmbench-1.0.8/README.md` & `fmbench-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/1_generate_data.ipynb` & `fmbench-1.0.9/src/fmbench/1_generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/2_deploy_model.ipynb` & `fmbench-1.0.9/src/fmbench/2_deploy_model.ipynb`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/3_run_inference.ipynb` & `fmbench-1.0.9/src/fmbench/3_run_inference.ipynb`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/4_model_metric_analysis.ipynb` & `fmbench-1.0.9/src/fmbench/4_model_metric_analysis.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'Python 3', 'name': 'python3'}}"}*

```diff
@@ -1428,17 +1428,17 @@
                 "memoryGiB": 512,
                 "name": "ml.trn1n.32xlarge",
                 "vcpuNum": 128
             }
         ],
         "instance_type": "ml.c5.large",
         "kernelspec": {
-            "display_name": "conda_fmbench_python311",
+            "display_name": "Python 3",
             "language": "python",
-            "name": "conda_fmbench_python311"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `fmbench-1.0.8/src/fmbench/5_cleanup.ipynb` & `fmbench-1.0.9/src/fmbench/5_cleanup.ipynb`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-quick.yml` & `fmbench-1.0.9/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-quick.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-v1.yml` & `fmbench-1.0.9/src/fmbench/configs/config-llama2-13b-inf2-g5-p4d-v1.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-llama2-70b-g5-p4d-tgi.yml` & `fmbench-1.0.9/src/fmbench/configs/config-llama2-70b-g5-p4d-tgi.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-llama2-70b-g5-p4d-trt.yml` & `fmbench-1.0.9/src/fmbench/configs/config-llama2-70b-g5-p4d-trt.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-llama2-7b-g5-quick.yml` & `fmbench-1.0.9/src/fmbench/configs/config-llama2-7b-g5-quick.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/configs/config-mistral-7b-tgi-g5.yml` & `fmbench-1.0.9/src/fmbench/configs/config-mistral-7b-tgi-g5.yml`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/globals.py` & `fmbench-1.0.9/src/fmbench/globals.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/main.py` & `fmbench-1.0.9/src/fmbench/main.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/scripts/jumpstart.py` & `fmbench-1.0.9/src/fmbench/scripts/jumpstart.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/scripts/p4d_djl.py` & `fmbench-1.0.9/src/fmbench/scripts/p4d_djl.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/scripts/p4d_hf_tgi.py` & `fmbench-1.0.9/src/fmbench/scripts/p4d_hf_tgi.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/src/fmbench/utils.py` & `fmbench-1.0.9/src/fmbench/utils.py`

 * *Files identical despite different names*

### Comparing `fmbench-1.0.8/PKG-INFO` & `fmbench-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmbench
-Version: 1.0.8
+Version: 1.0.9
 Summary: Benchmark performance of **any model** on **any supported instance type** on Amazon SageMaker.
 Author: Amit Arora
 Author-email: aroraai@amazon.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

