# Comparing `tmp/titanq-0.6.1.tar.gz` & `tmp/titanq-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.6.1.tar", last modified: Mon Apr  1 12:55:56 2024, max compression
+gzip compressed data, was "titanq-0.7.0.tar", last modified: Tue Apr  2 15:53:50 2024, max compression
```

## Comparing `titanq-0.6.1.tar` & `titanq-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-03-15 13:28:09.000000 titanq-0.6.1/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-01 12:55:56.798160 titanq-0.6.1/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-03-26 16:14:37.000000 titanq-0.6.1/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-01 12:53:14.000000 titanq-0.6.1/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-03-26 16:14:37.000000 titanq-0.6.1/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-01 12:55:56.798160 titanq-0.6.1/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6098 2024-03-15 13:45:14.000000 titanq-0.6.1/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    16855 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1492 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      736 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_optimize_response.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      117 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3380 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     8880 2024-03-28 20:55:17.000000 titanq-0.6.1/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      985 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    18311 2024-03-28 18:48:10.000000 titanq-0.6.1/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      993 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3942 2024-03-22 12:53:12.000000 titanq-0.6.1/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      871 2024-03-25 14:26:36.000000 titanq-0.6.1/titanq/_model/variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3813 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5682 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3746 2024-03-22 14:53:41.000000 titanq-0.6.1/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      740 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.661551 titanq-0.7.0/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.7.0/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-02 15:53:50.661551 titanq-0.7.0/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.7.0/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-02 15:31:47.000000 titanq-0.7.0/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.7.0/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-02 15:53:50.661551 titanq-0.7.0/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.653551 titanq-0.7.0/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.7.0/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    24022 2024-04-02 15:31:47.000000 titanq-0.7.0/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.7.0/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      736 2024-04-01 18:11:59.000000 titanq-0.7.0/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      427 2024-04-02 15:31:47.000000 titanq-0.7.0/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.653551 titanq-0.7.0/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.7.0/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.653551 titanq-0.7.0/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.7.0/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.657551 titanq-0.7.0/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.7.0/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5080 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      894 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    27041 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.7.0/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3942 2024-04-01 13:41:38.000000 titanq-0.7.0/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1541 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_model/variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.657551 titanq-0.7.0/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.7.0/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4287 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.7.0/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-02 15:53:50.657551 titanq-0.7.0/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-02 15:53:50.000000 titanq-0.7.0/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      789 2024-04-02 15:53:50.000000 titanq-0.7.0/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-02 15:53:50.000000 titanq-0.7.0/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-02 15:53:50.000000 titanq-0.7.0/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-02 15:53:50.000000 titanq-0.7.0/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.6.1/LICENSE.txt` & `titanq-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/PKG-INFO` & `titanq-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.6.1
+Version: 0.7.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.6.1/README.md` & `titanq-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/pyproject.toml` & `titanq-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.6.1"
+version = "0.7.0"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
```

### Comparing `titanq-0.6.1/tests/test_client.py` & `titanq-0.7.0/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,30 @@
 from titanq._client import Client, api_model
 from titanq import errors
 
 @pytest.fixture
 def solve_request():
     return api_model.SolveRequest(
         input=api_model.S3Input(
-            bias_file_name='test_bias_file_name.npy',
-            weights_file_name='test_weights_file_name.npy',
-            constraint_bounds_file_name=None,
-            constraint_weights_file_name=None,
             s3=api_model.AwsStorage(
                 bucket_name="test_input_bucket",
                 access_key_id="test_access_key",
                 secret_access_key="test_secret_access_key",
             ),
+            bias_file_name='test_bias_file_name.npy',
+            weights_file_name='test_weights_file_name.npy',
+            constraint_bounds_file_name=None,
+            constraint_weights_file_name=None,
+            variable_bounds_file_name=None,
+            manifest=api_model.Manifest(
+                has_set_partitioning_constraint= False,
+                has_cardinality_constraint= False,
+                has_equality_constraint=False,
+                has_inequality_constraint=False
+            ),
         ),
         output=api_model.S3Output(
                 result_archive_file_name="test.zip",
                 s3=api_model.AwsStorage(
                 bucket_name="test_output_bucket",
                 access_key_id="test_access_key",
                 secret_access_key="test_secret_access_key",
@@ -32,15 +39,15 @@
         ),
         parameters=api_model.Parameters(
             beta=[0.1],
             coupling_mult=0.5,
             num_chains=8,
             num_engines=2,
             timeout_in_secs=10,
-            variables_format='binary',
+            variable_types='binary',
             normalized=True,
         )
     )
 
 @pytest.fixture
 def baseurl():
     return "https://unittest.titanq.infinityq.io"
@@ -52,15 +59,16 @@
 @pytest.fixture
 def temp_storage_raw_response():
     return \
         '{"input": {' \
             '"weights.npy": { "upload": "http://weights-upload.com", "download": "http://weights-download.com" },' \
             '"bias.npy": { "upload": "http://bias-upload.com", "download": "http://bias-download.com" }, ' \
             '"constraint_weights.npy": { "upload": "http://constraint_weights-upload.com", "download": "http://constraint_weights-download.com" }, ' \
-            '"constraint_bounds.npy": { "upload": "http://constraint_bounds-upload.com", "download": "http://constraint_bounds-download.com" } }, ' \
+            '"constraint_bounds.npy": { "upload": "http://constraint_bounds-upload.com", "download": "http://constraint_bounds-download.com" }, ' \
+            '"variable_bounds.npy": { "upload": "http://variable_bounds-upload.com", "download": "http://variable_bounds-download.com" } }, ' \
         '"output": {' \
             '"result.zip": { "upload": "http://result-upload.com", "download": "http://result-download.com" } } }'
 
 def test_temp_storage(client, baseurl, temp_storage_raw_response):
     with requests_mock.Mocker() as m:
         adapter = m.get(f'{baseurl}/v1/temp_storage', content=temp_storage_raw_response.encode())
         temp_storage_response = client.temp_storage()
@@ -72,14 +80,16 @@
     assert temp_storage_response.input.weights_file.download == "http://weights-download.com"
     assert temp_storage_response.input.bias_file.upload == "http://bias-upload.com"
     assert temp_storage_response.input.bias_file.download == "http://bias-download.com"
     assert temp_storage_response.input.constraint_weights_file.upload == "http://constraint_weights-upload.com"
     assert temp_storage_response.input.constraint_weights_file.download == "http://constraint_weights-download.com"
     assert temp_storage_response.input.constraint_bounds_file.upload == "http://constraint_bounds-upload.com"
     assert temp_storage_response.input.constraint_bounds_file.download == "http://constraint_bounds-download.com"
+    assert temp_storage_response.input.variable_bounds_file.upload == "http://variable_bounds-upload.com"
+    assert temp_storage_response.input.variable_bounds_file.download == "http://variable_bounds-download.com"
     assert temp_storage_response.output.result_archive_file.upload == "http://result-upload.com"
     assert temp_storage_response.output.result_archive_file.download == "http://result-download.com"
 
 def test_credits(client, baseurl):
     raw_credit_response = '{"remaining_credits": 10,"expiration_date": "2023-12-13T16:44:00+00:00"}'
 
     with requests_mock.Mocker() as m:
```

### Comparing `titanq-0.6.1/tests/test_model.py` & `titanq-0.7.0/tests/test_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -260,30 +260,31 @@
         with pytest.raises(error):
             model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
     else:
         model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
 
 
 @pytest.mark.parametrize("vtype", [
-    Vtype.BINARY, Vtype.BIPOLAR,
+    (Vtype.BINARY),
+    (Vtype.BIPOLAR)
 ])
 def test_vtype_sent(model_s3_client, mock_titanq_client, vtype):
     model = model_s3_client
     mock_client = mock_titanq_client
 
     # optimize using sdk
     weights = np.random.rand(10, 10).astype(np.float32)
     bias = np.random.rand(10).astype(np.float32)
 
     model.add_variable_vector('x', 10, vtype)
     model.set_objective_matrices(weights, bias)
 
     model.optimize()
 
-    assert mock_client.request_sent.parameters.variables_format == str(vtype)
+    assert mock_client.request_sent.parameters.variable_types == str(vtype)
 
 
 @pytest.mark.parametrize("constraint_weights_dtype, constraint_bounds_dtype, error", [
     (np.float32, np.float32, None),
     (np.float64, np.float32, ValueError),
     (np.float32, np.float64, ValueError),
     (np.int32, np.int32, ValueError),
@@ -322,65 +323,65 @@
         model_s3_client.add_cardinality_constraint(np.array([1, 1]), 2)
 
 
 def test_add_set_partitioning_constraints_matrix(model_s3_client):
     model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
 
     model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1]]))
 
     model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 0, 0, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 0, 0, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1], [1, 1], [1, 1]]))
 
     with pytest.raises(errors.MaximumConstraintLimitError):
         model_s3_client.add_set_partitioning_constraints_matrix(np.array([[1, 1, 0, 0], [1, 1, 0, 0]]))
 
 
 def test_add_set_partitioning_constraint(model_s3_client):
     model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
 
     model_s3_client.add_set_partitioning_constraint(np.array([0, 1]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 1]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 1]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1]]))
 
     model_s3_client.add_set_partitioning_constraint(np.array([1, 0]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 1], [1, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 1], [1, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1]]))
 
     with pytest.raises(errors.MaximumConstraintLimitError):
         model_s3_client.add_set_partitioning_constraint(np.array([1, 0]))
 
 
 def test_add_cardinality_constraints_matrix(model_s3_client):
     model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
 
     model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 0, 1, 0], [0, 1, 1, 1]]), np.array([2, 3]))
-    assert (model_s3_client._constraints.weights() == np.array([[1, 0, 1, 0], [0, 1, 1, 1]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [3, 3]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1, 0, 1, 0], [0, 1, 1, 1]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [3, 3]]))
 
     model_s3_client.add_cardinality_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]), np.array([1, 1]))
-    assert (model_s3_client._constraints.weights() == np.array([[1, 0, 1, 0], [0, 1, 1, 1], [0, 1, 0, 0], [1, 0, 0, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [3, 3], [1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1, 0, 1, 0], [0, 1, 1, 1], [0, 1, 0, 0], [1, 0, 0, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [3, 3], [1, 1], [1, 1]]))
 
     with pytest.raises(errors.MaximumConstraintLimitError):
         model_s3_client.add_cardinality_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]), np.array([1, 1]))
 
 
 def test_add_cardinality_constraint(model_s3_client):
     model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
 
     model_s3_client.add_cardinality_constraint(np.array([1, 1]), 2)
-    assert (model_s3_client._constraints.weights() == np.array([[1, 1]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[2, 2]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1, 1]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2]]))
 
     model_s3_client.add_cardinality_constraint(np.array([0, 1]), 1)
-    assert (model_s3_client._constraints.weights() == np.array([[1, 1], [0, 1]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1, 1], [0, 1]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [1, 1]]))
 
     with pytest.raises(errors.MaximumConstraintLimitError):
         model_s3_client.add_cardinality_constraint(np.array([0, 1]), 1)
 
 @pytest.mark.parametrize("constraint_mask, cardinality, error", [
     (np.array([1, 1]), 1, None),
     (np.array([1, 1]), 2, None),
@@ -391,24 +392,140 @@
 
     if error:
         with pytest.raises(ValueError):
             model_s3_client.add_cardinality_constraint(constraint_mask, cardinality)
     else:
         model_s3_client.add_cardinality_constraint(constraint_mask, cardinality)
 
+def test_cardinality_or_set_partitioning_constraint_variable_types(model_s3_client, mock_titanq_client):
+    weights = np.random.rand(2, 2).astype(np.float32)
+    bias = np.random.rand(2).astype(np.float32)
+
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+    model_s3_client.set_objective_matrices(weights, bias)
+    model_s3_client.add_cardinality_constraint(np.array([1, 1]), 2)
+
+    model_s3_client.optimize()
+
+    assert mock_titanq_client.request_sent.parameters.variable_types == "binary"
+    assert mock_titanq_client.request_sent.input.variable_bounds_file_name == 'test-variable_bounds.npy'
+
+def test_add_equality_constraint(model_s3_client):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    model_s3_client.add_equality_constraint(np.array([1.05, -1.1], dtype=np.float32), -3.45)
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[-3.45, -3.45]], dtype=np.float32))
+
+    model_s3_client.add_equality_constraint(np.array([14, 0], dtype=np.float32), 0)
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1], [14, 0]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[-3.45, -3.45], [0, 0]], dtype=np.float32))
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_equality_constraint(np.array([99, 99], dtype=np.float32), 99)
+
+def test_add_equality_constraint_matrix(model_s3_client):
+    model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
+
+    model_s3_client.add_equality_constraints_matrix(np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32), np.array([2, 10], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [10, 10]], dtype=np.float32))
+
+    model_s3_client.add_equality_constraints_matrix(np.array([[0, 5, 0, 0], [0, 0, -5, 0]], dtype=np.float32), np.array([-1, 1], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0], [0, 5, 0, 0], [0, 0, -5, 0]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [10, 10], [-1, -1], [1, 1]], dtype=np.float32))
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_equality_constraints_matrix(np.array([[99, 99, 99, 99], [99, 99, 99, 99]], dtype=np.float32), np.array([-99, 99], dtype=np.float32))
+
+
+def test_equality_constraint_override_variable_types(model_s3_client, mock_titanq_client):
+    weights = np.random.rand(2, 2).astype(np.float32)
+    bias = np.random.rand(2).astype(np.float32)
+
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+    model_s3_client.set_objective_matrices(weights, bias)
+    model_s3_client.add_equality_constraint(np.array([1.05, -1.1], dtype=np.float32), -3.45)
+    model_s3_client.optimize()
+
+    assert mock_titanq_client.request_sent.parameters.variable_types == "bb"
+    assert mock_titanq_client.request_sent.input.variable_bounds_file_name == "test-variable_bounds.npy"
+
+
+def test_add_inequality_constraint(model_s3_client):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    model_s3_client.add_inequality_constraint(np.array([1.05, -1.1], dtype=np.float32), np.array([np.nan, -3.45], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[np.nan, -3.45]], dtype=np.float32))
+
+    model_s3_client.add_inequality_constraint(np.array([14, 0], dtype=np.float32), np.array([-0.09, 0], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1], [14, 0]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[np.nan, -3.45], [-0.09, 0]], dtype=np.float32))
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_inequality_constraint(np.array([99, 99], dtype=np.float32), np.array([99, np.nan], dtype=np.float32))
+
+def test_add_inequality_constraint_matrix(model_s3_client):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+    model_s3_client.add_inequality_constraints_matrix(np.array([[-3.51, 0], [10, 0]], dtype=np.float32), np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32))
+
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0], [10, 0]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32))
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_inequality_constraints_matrix(np.array([[99, 99], [99, 99]], dtype=np.float32), np.array([[-99, 99], [-99, np.nan]], dtype=np.float32))
+
+
+def test_inequality_constraint_override_variable_types(model_s3_client, mock_titanq_client):
+    weights = np.random.rand(2, 2).astype(np.float32)
+    bias = np.random.rand(2).astype(np.float32)
+
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+    model_s3_client.set_objective_matrices(weights, bias)
+    model_s3_client.add_inequality_constraint(np.array([1.05, -1.1], dtype=np.float32), np.array([1.0, np.nan], dtype=np.float32))
+    model_s3_client.optimize()
+
+    assert mock_titanq_client.request_sent.parameters.variable_types == "bb"
+    assert mock_titanq_client.request_sent.input.variable_bounds_file_name == "test-variable_bounds.npy"
+
+
 def test_combination_constraint(model_s3_client):
     model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
 
     model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1]]))
 
     model_s3_client.add_set_partitioning_constraint(np.array([0, 1, 0, 0]))
-    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1], [1, 1]]))
 
     model_s3_client.add_cardinality_constraint(np.array([1, 1, 1, 1]), 2)
-    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 1, 1, 1]])).all()
-    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1], [2, 2]])).all()
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 1, 1, 1]]))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[1, 1], [1, 1], [1, 1], [2, 2]]))
 
     with pytest.raises(errors.MaximumConstraintLimitError):
-        model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 1, 0, 0], [1, 1, 0, 0]]), [2, 2])
+        model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 1, 0, 0], [1, 1, 0, 0]]), np.array([2, 2]))
+
+
+def test_manifest(model_s3_client, mock_titanq_client):
+    weights = np.random.rand(4, 4).astype(np.float32)
+    bias = np.random.rand(4).astype(np.float32)
+
+    # Construct the request
+    model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
+    model_s3_client.set_objective_matrices(weights, bias)
+
+    model_s3_client.add_set_partitioning_constraint(np.array([0, 0, 1, 0]))
+    model_s3_client.add_cardinality_constraint(np.array([1, 0, 1, 0]), 2)
+    model_s3_client.add_equality_constraint(np.array([44.01, 0, 10, -1], dtype=np.float32), -50.01)
+    model_s3_client.add_inequality_constraint(np.array([44.01, 0, 10, -1], dtype=np.float32), np.array([np.nan, 10], dtype=np.float32))
+
+    # Send the request
+    model_s3_client.optimize()
+
+    # Make sure the appropriate manifest flag have been sent
+    assert mock_titanq_client.request_sent.input.manifest.has_set_partitioning_constraint == True
+    assert mock_titanq_client.request_sent.input.manifest.has_cardinality_constraint == True
+    assert mock_titanq_client.request_sent.input.manifest.has_equality_constraint == True
+    assert mock_titanq_client.request_sent.input.manifest.has_inequality_constraint == True
```

### Comparing `titanq-0.6.1/tests/test_numpy_util.py` & `titanq-0.7.0/tests/test_numpy_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import pytest
 import numpy as np
-from titanq._model.numpy_util import convert_to_float32, reshape_to_2d, is_ndarray_binary
+from titanq._model.numpy_util import (
+    convert_to_float32,
+    is_upperbound_bigger_equal_lowerbound,
+    is_ndarray_binary,
+    ndarray_contains_nan_inf,
+    reshape_to_2d,
+    validate_cardinalities,
+)
 
 @pytest.mark.parametrize("array, expected_dtype", [
     (np.array([[1, 2], [3, 4]]), np.float32),
     (np.array([[1.5, 2.5], [3.5, 4.5]]), np.float32),
     (np.empty((0, 0)), np.float32),
     (np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]]), np.float32)
 ])
@@ -40,8 +47,45 @@
     (np.array([0, 1.01]), False),
     (np.array([[0, 0], [0, 2]]), False),
     (np.array([0]), True),
     (np.array([0, 1]), True),
     (np.array([[1, 1], [0, 0]]), True),
 ])
 def test_is_ndarray_binary(array, expected_result):
-    assert is_ndarray_binary(array) == expected_result
+    assert is_ndarray_binary(array) == expected_result
+
+
+@pytest.mark.parametrize("array, expected_value", [
+    (np.array([0]), False),
+    (np.array([1]), False),
+    (np.array([1.01]), False),
+    (np.array([-1.01]), False),
+    (np.array([np.nan]), True),
+    (np.array([-np.nan]), True),
+    (np.array([np.NaN]), True),
+    (np.array([np.NAN]), True),
+    (np.array([np.inf]), True),
+    (np.array([-np.inf]), True),
+])
+def test_ndarray_contains_nan_inf(array, expected_value):
+    assert ndarray_contains_nan_inf(array) == expected_value
+
+@pytest.mark.parametrize("array, expected_value", [
+    (np.array([[0, 1], [-1, 4000]]), False),
+    (np.array([[1, 1], [0, 1]]), True),
+    (np.array([[1.01, 1], [5.4, 1]]), True),
+])
+def test_is_upperbound_bigger_equal_lowerbound(array, expected_value):
+    assert is_upperbound_bigger_equal_lowerbound(array) == expected_value
+
+
+@pytest.mark.parametrize("cardinalities, expected_error", [
+    (2, None),
+    (3, None),
+    (4, ValueError),
+])
+def test_validate_cardinalities(cardinalities, expected_error):
+    if expected_error:
+        with pytest.raises(expected_error):
+            validate_cardinalities(np.array([[1,1,1]]), np.array([cardinalities]))
+    else:
+        validate_cardinalities(np.array([[1,1,1]]), np.array([cardinalities]))
```

### Comparing `titanq-0.6.1/tests/test_optimize_response.py` & `titanq-0.7.0/tests/test_optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/titanq/__init__.py` & `titanq-0.7.0/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/titanq/_client/client.py` & `titanq-0.7.0/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/titanq/_client/model.py` & `titanq-0.7.0/titanq/_client/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,36 +14,48 @@
     access_key_id: SecretStr
     secret_access_key: SecretStr
 
     @field_serializer('access_key_id', 'secret_access_key', when_used='json')
     def dump_secret(self, v):
         return v.get_secret_value()
 
+class Manifest(BaseModel):
+    """
+    The manifest object of the solver request
+    """
+    has_set_partitioning_constraint: bool
+    has_cardinality_constraint: bool
+    has_equality_constraint: bool
+    has_inequality_constraint: bool
 
 class S3Input(BaseModel):
     """
     Input object of the solve request with s3
     """
+    s3: AwsStorage
     bias_file_name: str
     weights_file_name: str
     constraint_bounds_file_name: Optional[str]
     constraint_weights_file_name: Optional[str]
-    s3: AwsStorage
+    variable_bounds_file_name: Optional[str]
+    manifest: Optional[Manifest]
 
 
 class UrlInput(BaseModel):
     """
     Input object of the solve request with url
     """
     # always true, the user does not have to set this value
     file_name_is_url: bool = Field(default=True, frozen=True)
     bias_file_name: str
     weights_file_name: str
     constraint_bounds_file_name: Optional[str]
     constraint_weights_file_name: Optional[str]
+    variable_bounds_file_name: Optional[str]
+    manifest: Optional[Manifest]
 
 
 class S3Output(BaseModel):
     """
     Output object of the solve request with s3
     """
     result_archive_file_name: str
@@ -63,15 +75,15 @@
     Tuning parameters used by the solver
     """
     beta: List[float]
     coupling_mult: float
     timeout_in_secs: float
     num_chains: int
     num_engines: int
-    variables_format: str
+    variable_types: str
     normalized: bool
 
 
 class SolveRequest(BaseModel):
     """
     The actual solve request object send to the backend
     """
@@ -116,14 +128,15 @@
     """
     Object containing input files for temporary storage object
     """
     weights_file: FileUrls = Field(alias="weights.npy")
     bias_file: FileUrls = Field(alias="bias.npy")
     constraint_weights_file: FileUrls = Field(alias="constraint_weights.npy")
     constraint_bounds_file: FileUrls = Field(alias="constraint_bounds.npy")
+    variable_bounds_file: FileUrls = Field(alias="variable_bounds.npy")
 
 
 class TempStorageOutput(BaseModel):
     """"
     Object containing output files for temporary storage object
     """
     result_archive_file: FileUrls = Field(alias="result.zip")
```

### Comparing `titanq-0.6.1/titanq/_model/errors.py` & `titanq-0.7.0/titanq/_model/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 
 class ConstraintSizeError(TitanQError):
     """The constraint size does not match"""
 
 class ObjectiveAlreadySetError(TitanQError):
     """An objective has already been set"""
 
-class ConstraintsAlreadySetError(TitanQError):
-    """Constraints has already been set"""
-
 class OptimizeError(TitanQError):
     """Error occur during optimization"""
 
 class ServerError(TitanQError):
     """Error returned by the server"""
 
 class ConnectionError(TitanQError):
```

### Comparing `titanq-0.6.1/titanq/_model/objective.py` & `titanq-0.7.0/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/titanq/_model/optimize_response.py` & `titanq-0.7.0/titanq/_model/optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.6.1/titanq/_model/variable.py` & `titanq-0.7.0/titanq/_model/variable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import numpy as np
 
 class Vtype(str, enum.Enum):
     BINARY = 'binary'
     BIPOLAR = 'bipolar'
 
     def __str__(self) -> str:
         return str(self.value)
@@ -32,8 +33,26 @@
         """
         return self._vtype
 
     def name(self) -> str:
         """
         :return: Name of this variable vector.
         """
-        return self._name
+        return self._name
+
+    def variable_types_as_list(self) -> str:
+        """
+        :return: Generate a string of 'b' depending on the variable size
+        """
+        if self._vtype == Vtype.BIPOLAR:
+            raise ValueError("Cannot set variable types as a list for 'bipolar' type")
+
+        return "".join(['b' for _ in range(self._size)])
+
+    def create_variable_bounds(self):
+        """
+        :return: Generate a string of 'b' depending on the variable size
+        """
+        if self._vtype == Vtype.BIPOLAR:
+            raise ValueError("Cannot set variable types as a list for 'bipolar' type")
+
+        return np.tile(np.array([0,1]), (self._size, 1))
```

### Comparing `titanq-0.6.1/titanq/_storage/managed_storage.py` & `titanq-0.7.0/titanq/_storage/managed_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,40 +20,54 @@
 
         :titanq_client: titanq_client to be used to fetch temporary URL's
         """
         self._titanq_client = titanq_client
         self._urls = titanq_client.temp_storage()
         self._constraint_bounds_uploaded = False
         self._constraint_weights_uploaded = False
+        self._variable_bounds_uploaded = False
 
-    def _upload_arrays(self, bias: bytes, weights: bytes, constraint_bounds: Optional[bytes], constraint_weights: Optional[bytes]):
+    def _upload_arrays(
+        self,
+        bias: bytes,
+        weights: bytes,
+        constraint_bounds: Optional[bytes],
+        constraint_weights: Optional[bytes],
+        variable_bounds: Optional[bytes]
+        ):
         upload_tuple = [
             (self._urls.input.bias_file.upload, bias),
             (self._urls.input.weights_file.upload, weights),
         ]
 
         if constraint_bounds:
             self._constraint_bounds_uploaded = True
             upload_tuple.append((self._urls.input.constraint_bounds_file.upload, constraint_bounds))
 
         if constraint_weights:
             self._constraint_weights_uploaded = True
             upload_tuple.append((self._urls.input.constraint_weights_file.upload, constraint_weights))
 
+        if variable_bounds:
+            self._variable_bounds_uploaded = True
+            upload_tuple.append((self._urls.input.variable_bounds_file.upload, constraint_weights))
+
         log.debug(f"Uploading files on our temporary storage")
         for url, data in upload_tuple:
             requests.put(url, data=data)
 
 
     def _input(self) -> UrlInput:
         return UrlInput(
             weights_file_name=self._urls.input.weights_file.download,
             bias_file_name=self._urls.input.bias_file.download,
             constraint_bounds_file_name=self._urls.input.constraint_bounds_file.download if self._constraint_bounds_uploaded else None,
             constraint_weights_file_name=self._urls.input.constraint_weights_file.download if self._constraint_weights_uploaded else None,
+            variable_bounds_file_name=self._urls.input.variable_bounds_file.download if self._variable_bounds_uploaded else None,
+            manifest=None
         )
 
     def _output(self) -> UrlOutput:
         return UrlOutput(result_archive_file_name=self._urls.output.result_archive_file.upload)
 
     def _wait_for_result_to_be_uploaded_and_download(self) -> bytes:
         self._wait_for_file_to_be_uploaded(self._urls.output.result_archive_file.download)
```

### Comparing `titanq-0.6.1/titanq/_storage/s3_storage.py` & `titanq-0.7.0/titanq/_storage/s3_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 log = logging.getLogger("TitanQ")
 
 _BIAS_FILE = "bias.npy"
 _WEIGHTS_FILE = "weights.npy"
 _CONSTRAINT_BOUNDS_FILE = "constraint_bounds.npy"
 _CONSTRAINT_WEIGHTS_FILE = "constraints_weights.npy"
+_VARIABLE_BOUNDS_FILE = "variable_bounds.npy"
 _RESULT_FILE = "result.zip"
 
 
 
 class S3Storage(StorageClient):
     def __init__(self, access_key, secret_key, bucket_name):
         """
@@ -36,41 +37,56 @@
 
         timestamp = datetime.datetime.now().isoformat()
         self._remote_folder = f"titanq_sdk/{timestamp}"
 
         # keep track of which file were uploaded
         self._file_uploaded = set()
 
-    def _upload_arrays(self, bias: bytes, weights: bytes, constraint_bounds: Optional[bytes], constraint_weights: Optional[bytes]):
+    def _upload_arrays(
+        self,
+        bias: bytes,
+        weights: bytes,
+        constraint_bounds: Optional[bytes],
+        constraint_weights: Optional[bytes],
+        variable_bounds: Optional[bytes]
+        ) -> None:
+
         upload_tuple = [
             (self._get_full_filename(_BIAS_FILE), bias),
             (self._get_full_filename(_WEIGHTS_FILE), weights)
         ]
 
         if constraint_bounds:
             upload_tuple.append((self._get_full_filename(_CONSTRAINT_BOUNDS_FILE), constraint_bounds))
 
         if constraint_weights:
             upload_tuple.append((self._get_full_filename(_CONSTRAINT_WEIGHTS_FILE), constraint_weights))
 
+        if variable_bounds:
+            upload_tuple.append((self._get_full_filename(_VARIABLE_BOUNDS_FILE), variable_bounds))
+
         for filename, body in upload_tuple:
             log.debug(f"Uploading object on AWS s3: {filename}")
             self._s3.put_object(Body=body, Bucket=self._bucket_name, Key=filename)
             self._file_uploaded.add(filename)
 
     def _input(self) -> S3Input:
         constraint_bounds = self._get_full_filename(_CONSTRAINT_BOUNDS_FILE)
         constraint_weights = self._get_full_filename(_CONSTRAINT_WEIGHTS_FILE)
+        variable_bounds = self._get_full_filename(_VARIABLE_BOUNDS_FILE)
 
         return S3Input(
+            s3=self._get_api_model_location(),
             weights_file_name=self._get_full_filename(_WEIGHTS_FILE),
             bias_file_name=self._get_full_filename(_BIAS_FILE),
             constraint_weights_file_name=constraint_weights if constraint_weights in self._file_uploaded else None,
             constraint_bounds_file_name=constraint_bounds if constraint_bounds in self._file_uploaded else None,
-            s3=self._get_api_model_location())
+            variable_bounds_file_name=variable_bounds if variable_bounds in self._file_uploaded else None,
+            manifest=None
+        )
 
     def _output(self) -> S3Output:
         return S3Output(
             result_archive_file_name=self._get_full_filename(_RESULT_FILE),
             s3=self._get_api_model_location())
 
     def _get_api_model_location(self) -> AwsStorage:
```

### Comparing `titanq-0.6.1/titanq/_storage/storage_client.py` & `titanq-0.7.0/titanq/_storage/storage_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,23 @@
         pass
 
     def temp_files_manager(self,
         bias: np.ndarray,
         weights: np.ndarray,
         constraint_bounds: Optional[np.ndarray],
         constraint_weights: Optional[np.ndarray],
+        variable_bounds: Optional[np.ndarray]
     ) -> Type["TempFileManager"]:
         """'
         Creates and returns a context manager that will be handling the temporary file management
 
         :param bias: bias numpy array
         :param weights: weights numpy array
         """
-        return TempFileManager(self, bias, weights, constraint_bounds, constraint_weights)
+        return TempFileManager(self, bias, weights, constraint_bounds, constraint_weights, variable_bounds)
 
     @abstractmethod
     def _input(self) -> Union[S3Input, UrlInput]:
         """
         Returns the api model for the input of the solve request
 
         :return: either the s3 or the url input
@@ -39,21 +40,23 @@
         """
         Returns the api model for the output of the solve request
 
         :return: either the s3 or the url output
         """
 
     @abstractmethod
-    def _upload_arrays(self, bias: bytes, weights: bytes, constraint_bounds: Optional[bytes], constraint_weights: Optional[bytes]):
-        """
-        Uploads .npy arrays (bias and weights) to the storage client
-
-        :param bias: bias array in bytes
-        :param weights: weights array in bytes
-        """
+    def _upload_arrays(
+        self,
+        bias: bytes,
+        weights: bytes,
+        constraint_bounds: Optional[bytes],
+        constraint_weights: Optional[bytes],
+        variable_bounds: Optional[bytes]
+        ):
+        """Uploads .npy arrays to the storage client"""
 
     @abstractmethod
     def _wait_for_result_to_be_uploaded_and_download(self) -> bytes:
         """
         Wait until a file is uploaded on the storage client and download it
 
         :return: content of the result file in bytes
@@ -72,33 +75,36 @@
     def __init__(
         self,
         storage_client: StorageClient,
         bias: np.ndarray,
         weights: np.ndarray,
         constraint_bounds: Optional[np.ndarray],
         constraint_weights: Optional[np.ndarray],
+        variable_bounds: Optional[np.ndarray]
     ) -> None:
         """
         :param storage_client: storage client that will handle uploads, downloads and generating api models
         :param bias: bias numpy array
         :param weights: weights numpy array
         """
         super().__init__()
         self._storage_client = storage_client
         self._bias = bias
         self._weights = weights
         self._constraint_bounds = constraint_bounds
         self._constraint_weights = constraint_weights
+        self._variable_bounds = variable_bounds
 
     def __enter__(self) -> Type["TempFileManager"]:
         self._storage_client._upload_arrays(
             self._to_bytes(self._bias),
             self._to_bytes(self._weights),
             self._to_bytes(self._constraint_bounds),
             self._to_bytes(self._constraint_weights),
+            self._to_bytes(self._variable_bounds)
         )
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self._storage_client._delete_remote_object()
 
     def input(self) -> Union[S3Input, UrlInput]:
```

### Comparing `titanq-0.6.1/titanq.egg-info/PKG-INFO` & `titanq-0.7.0/titanq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.6.1
+Version: 0.7.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.6.1/titanq.egg-info/SOURCES.txt` & `titanq-0.7.0/titanq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 README.md
 pyproject.toml
 requirements.txt
 tests/test_client.py
 tests/test_model.py
 tests/test_numpy_util.py
 tests/test_optimize_response.py
+tests/test_variable.py
 titanq/__init__.py
 titanq.egg-info/PKG-INFO
 titanq.egg-info/SOURCES.txt
 titanq.egg-info/dependency_links.txt
 titanq.egg-info/requires.txt
 titanq.egg-info/top_level.txt
 titanq/_client/__init__.py
 titanq/_client/client.py
 titanq/_client/model.py
 titanq/_model/__init__.py
 titanq/_model/constraints.py
 titanq/_model/errors.py
+titanq/_model/manifest.py
 titanq/_model/model.py
 titanq/_model/numpy_util.py
 titanq/_model/objective.py
 titanq/_model/optimize_response.py
 titanq/_model/variable.py
 titanq/_storage/__init__.py
 titanq/_storage/managed_storage.py
```

