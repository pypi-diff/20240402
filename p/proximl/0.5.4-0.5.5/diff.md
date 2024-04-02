# Comparing `tmp/proximl-0.5.4.tar.gz` & `tmp/proximl-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proximl-0.5.4.tar", last modified: Wed Feb 14 16:00:50 2024, max compression
+gzip compressed data, was "proximl-0.5.5.tar", last modified: Tue Apr  2 13:17:39 2024, max compression
```

## Comparing `proximl-0.5.4.tar` & `proximl-0.5.5.tar`

### file list

```diff
@@ -1,118 +1,123 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.183153 proximl-0.5.4/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-02-14 15:59:09.000000 proximl-0.5.4/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-02-14 16:00:50.183014 proximl-0.5.4/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-02-14 15:59:09.000000 proximl-0.5.4/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.167302 proximl-0.5.4/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-02-14 15:59:09.000000 proximl-0.5.4/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-02-14 15:59:09.000000 proximl-0.5.4/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-02-14 15:59:09.000000 proximl-0.5.4/examples/training_inference_pipeline.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.170199 proximl-0.5.4/proximl/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-02-14 15:59:43.000000 proximl-0.5.4/proximl/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.172220 proximl-0.5.4/proximl/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4338 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.173158 proximl-0.5.4/proximl/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      534 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/cloudbender/reservation.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.173415 proximl-0.5.4/proximl/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cli/project.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.174673 proximl-0.5.4/proximl/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      634 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/cloudbender/reservations.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17807 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    11045 2024-02-14 15:59:09.000000 proximl-0.5.4/proximl/proximl.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.170967 proximl-0.5.4/proximl.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3344 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-02-14 16:00:50.000000 proximl-0.5.4/proximl.egg-info/top_level.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)      975 2024-02-14 15:59:09.000000 proximl-0.5.4/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-02-14 16:00:50.183199 proximl-0.5.4/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-02-14 15:59:09.000000 proximl-0.5.4/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.165758 proximl-0.5.4/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.176093 proximl-0.5.4/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.176317 proximl-0.5.4/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3128 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3424 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    23341 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2848 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1492 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/integration/test_projects_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.179268 proximl-0.5.4/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.180426 proximl-0.5.4/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.181286 proximl-0.5.4/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cli/test_cli_project_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:50.182771 proximl-0.5.4/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/cloudbender/test_reservations_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    29059 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-02-14 15:59:09.000000 proximl-0.5.4/tests/unit/test_proximl.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.702524 proximl-0.5.5/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-02 13:14:52.000000 proximl-0.5.5/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-02 13:17:39.702373 proximl-0.5.5/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-02 13:14:52.000000 proximl-0.5.5/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.685341 proximl-0.5.5/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/training_inference_pipeline.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.688743 proximl-0.5.5/proximl/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.690963 proximl-0.5.5/proximl/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.691873 proximl-0.5.5/proximl/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      534 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/reservation.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.692142 proximl-0.5.5/proximl/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.693600 proximl-0.5.5/proximl/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      634 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/reservations.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.689502 proximl-0.5.5/proximl.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3502 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/top_level.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1000 2024-04-02 13:14:52.000000 proximl-0.5.5/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-02 13:17:39.702570 proximl-0.5.5/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-02 13:14:52.000000 proximl-0.5.5/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.683774 proximl-0.5.5/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.695319 proximl-0.5.5/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.695535 proximl-0.5.5/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.698396 proximl-0.5.5/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.699740 proximl-0.5.5/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.700585 proximl-0.5.5/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.702142 proximl-0.5.5/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_reservations_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31197 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_volumes_unit.py
```

### Comparing `proximl-0.5.4/LICENSE` & `proximl-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/PKG-INFO` & `proximl-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.4
+Version: 0.5.5
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.4 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.5 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.4/README.md` & `proximl-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/examples/create_dataset_and_training_job.py` & `proximl-0.5.5/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/examples/local_storage.py` & `proximl-0.5.5/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/examples/training_inference_pipeline.py` & `proximl-0.5.5/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/auth.py` & `proximl-0.5.5/proximl/auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/checkpoints.py` & `proximl-0.5.5/proximl/checkpoints.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/__init__.py` & `proximl-0.5.5/proximl/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,34 +138,31 @@
     projects = config.proximl.run(config.proximl.client.projects.list())
     project_names = [project.name for project in projects]
 
     active_project = [
         project for project in projects if project.id == active_project_id
     ]
 
-    active_project_name = (
-        active_project[0].name if len(active_project) else "UNSET"
-    )
+    active_project_name = active_project[0].name if len(active_project) else "UNSET"
 
     click.echo(f"Current Active Project: {active_project_name}")
 
     name = click.prompt(
         "Select Active Project:",
         type=click.Choice(project_names, case_sensitive=True),
         show_choices=True,
         default=active_project_name,
     )
-    selected_project = [
-        project for project in projects if project.name == name
-    ]
+    selected_project = [project for project in projects if project.name == name]
     config.proximl.client.set_active_project(selected_project[0].id)
 
 
 from proximl.cli.connection import connection
 from proximl.cli.dataset import dataset
 from proximl.cli.model import model
 from proximl.cli.checkpoint import checkpoint
+from proximl.cli.volume import volume
 from proximl.cli.environment import environment
 from proximl.cli.gpu import gpu
 from proximl.cli.job import job
 from proximl.cli.project import project
 from proximl.cli.cloudbender import cloudbender
```

### Comparing `proximl-0.5.4/proximl/cli/checkpoint.py` & `proximl-0.5.5/proximl/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/__init__.py` & `proximl-0.5.5/proximl/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/datastore.py` & `proximl-0.5.5/proximl/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/device.py` & `proximl-0.5.5/proximl/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/node.py` & `proximl-0.5.5/proximl/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/provider.py` & `proximl-0.5.5/proximl/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/region.py` & `proximl-0.5.5/proximl/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/cloudbender/reservation.py` & `proximl-0.5.5/proximl/cli/cloudbender/reservation.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/connection.py` & `proximl-0.5.5/proximl/cli/connection.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/dataset.py` & `proximl-0.5.5/proximl/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/environment.py` & `proximl-0.5.5/proximl/cli/environment.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/gpu.py` & `proximl-0.5.5/proximl/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/job/__init__.py` & `proximl-0.5.5/proximl/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/job/create.py` & `proximl-0.5.5/proximl/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/model.py` & `proximl-0.5.5/proximl/cli/model.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cli/project.py` & `proximl-0.5.5/proximl/cli/project.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/cloudbender.py` & `proximl-0.5.5/proximl/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/datastores.py` & `proximl-0.5.5/proximl/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/device_configs.py` & `proximl-0.5.5/proximl/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/devices.py` & `proximl-0.5.5/proximl/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/nodes.py` & `proximl-0.5.5/proximl/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/providers.py` & `proximl-0.5.5/proximl/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/regions.py` & `proximl-0.5.5/proximl/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/cloudbender/reservations.py` & `proximl-0.5.5/proximl/cloudbender/reservations.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/connections.py` & `proximl-0.5.5/proximl/connections.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/datasets.py` & `proximl-0.5.5/proximl/datasets.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/environments.py` & `proximl-0.5.5/proximl/environments.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/exceptions.py` & `proximl-0.5.5/proximl/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,35 @@
         self._message = data
 
     @property
     def status(self) -> str:
         return self._status
 
     def __repr__(self):
-        return "CheckpointError({self.status}, {self.message})".format(
-            self=self
-        )
+        return "CheckpointError({self.status}, {self.message})".format(self=self)
 
     def __str__(self):
-        return "CheckpointError({self.status}, {self.message})".format(
-            self=self
-        )
+        return "CheckpointError({self.status}, {self.message})".format(self=self)
+
+
+class VolumeError(ProxiMLException):
+    def __init__(self, status, data, *args):
+        super().__init__(data, *args)
+        self._status = status
+        self._message = data
+
+    @property
+    def status(self) -> str:
+        return self._status
+
+    def __repr__(self):
+        return "VolumeError({self.status}, {self.message})".format(self=self)
+
+    def __str__(self):
+        return "VolumeError({self.status}, {self.message})".format(self=self)
 
 
 class ConnectionError(ProxiMLException):
     def __init__(self, message, *args):
         super().__init__(message, *args)
         self._message = message
 
@@ -126,15 +139,11 @@
         self._message = message
 
     @property
     def attribute(self) -> str:
         return self._attribute
 
     def __repr__(self):
-        return "SpecificationError({self.attribute}, {self.message})".format(
-            self=self
-        )
+        return "SpecificationError({self.attribute}, {self.message})".format(self=self)
 
     def __str__(self):
-        return "SpecificationError({self.attribute}, {self.message})".format(
-            self=self
-        )
+        return "SpecificationError({self.attribute}, {self.message})".format(self=self)
```

### Comparing `proximl-0.5.4/proximl/gpu_types.py` & `proximl-0.5.5/proximl/gpu_types.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/jobs.py` & `proximl-0.5.5/proximl/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,15 @@
             worker_commands=worker_commands,
             workers=kwargs.get("workers"),
             environment=environment,
             data=data,
             model=model,
             endpoint=endpoint,
             source_job_uuid=kwargs.get("source_job_uuid"),
-            project_uuid=kwargs.get("project_uuid")
-            or self.proximl.active_project,
+            project_uuid=kwargs.get("project_uuid") or self.proximl.active_project,
         )
         payload = {
             k: v
             for k, v in config.items()
             if v or (k in ["model"] and not kwargs.get("source_job_uuid"))
         }
         if (
@@ -99,17 +98,15 @@
     async def create_json(self, payload):
         logging.debug(f"Job payload: {payload}")
         resp = await self.proximl._query("/job", "POST", None, payload)
         job = Job(self.proximl, **resp)
         return job
 
     async def remove(self, id, **kwargs):
-        await self.proximl._query(
-            f"/job/{id}", "DELETE", dict(**kwargs, force=True)
-        )
+        await self.proximl._query(f"/job/{id}", "DELETE", dict(**kwargs, force=True))
 
 
 class Job:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
         self._job = kwargs
         self._id = self._job.get("id", self._job.get("job_uuid"))
@@ -304,26 +301,34 @@
         return resp
 
     def get_connection_details(self):
         details = dict(
             entity_type="job",
             project_uuid=self._job.get("project_uuid"),
             cidr=self.dict.get("vpn").get("cidr"),
-            ssh_port=self._job.get("vpn").get("client").get("ssh_port")
-            if self._job.get("vpn").get("client")
-            else None,
-            model_path=self._job.get("model").get("source_uri")
-            if self._job.get("model").get("source_type") == "local"
-            else None,
-            input_path=self._job.get("data").get("input_uri")
-            if self._job.get("data").get("input_type") == "local"
-            else None,
-            output_path=self._job.get("data").get("output_uri")
-            if self._job.get("data").get("output_type") == "local"
-            else None,
+            ssh_port=(
+                self._job.get("vpn").get("client").get("ssh_port")
+                if self._job.get("vpn").get("client")
+                else None
+            ),
+            model_path=(
+                self._job.get("model").get("source_uri")
+                if self._job.get("model").get("source_type") == "local"
+                else None
+            ),
+            input_path=(
+                self._job.get("data").get("input_uri")
+                if self._job.get("data").get("input_type") == "local"
+                else None
+            ),
+            output_path=(
+                self._job.get("data").get("output_uri")
+                if self._job.get("data").get("output_type") == "local"
+                else None
+            ),
         )
         return details
 
     async def open(self):
         if self.type != "notebook":
             raise SpecificationError(
                 "type",
@@ -392,44 +397,38 @@
             f"/job/{self.id}", "GET", dict(project_uuid=self._project_uuid)
         )
         self.__init__(self.proximl, **resp)
         return self
 
     def _get_msg_handler(self, msg_handler):
         worker_numbers = {
-            w.get("job_worker_uuid"): ind + 1
-            for ind, w in enumerate(self._workers)
+            w.get("job_worker_uuid"): ind + 1 for ind, w in enumerate(self._workers)
         }
         worker_numbers["data_worker"] = 0
 
         def handler(data):
             if data.get("type") == "subscription":
                 data["worker_number"] = worker_numbers.get(data.get("stream"))
                 if msg_handler:
                     msg_handler(data)
                 else:
-                    timestamp = datetime.fromtimestamp(
-                        int(data.get("time")) / 1000
-                    )
+                    timestamp = datetime.fromtimestamp(int(data.get("time")) / 1000)
                     if len(self._workers) > 1:
                         print(
                             f"{timestamp.strftime('%m/%d/%Y, %H:%M:%S')}: Worker {data.get('worker_number')} - {data.get('msg').rstrip()}"
                         )
                     else:
                         print(
                             f"{timestamp.strftime('%m/%d/%Y, %H:%M:%S')}: {data.get('msg').rstrip()}"
                         )
 
         return handler
 
     async def attach(self, msg_handler=None):
-        if (
-            self.type == "notebook"
-            and self.status != "waiting for data/model download"
-        ):
+        if self.type == "notebook" and self.status != "waiting for data/model download":
             raise SpecificationError(
                 "type",
                 "Notebooks cannot be attached to after model download is complete.  Use open() instead.",
             )
         await self.refresh()
         if self.status not in ["finished", "failed"]:
             await self.proximl._ws_subscribe(
@@ -438,17 +437,15 @@
                 self.id,
                 self._get_msg_handler(msg_handler),
             )
 
     async def copy(self, name, **kwargs):
         logging.debug(f"copy request - name: {name} ; kwargs: {kwargs}")
         if self.type != "notebook":
-            raise SpecificationError(
-                "job", "Only notebook job types can be copied"
-            )
+            raise SpecificationError("job", "Only notebook job types can be copied")
 
         job = await self.proximl.jobs.create(
             name,
             type=kwargs.get("type") or self.type,
             gpu_type=kwargs.get("gpu_type"),
             gpu_types=kwargs.get("gpu_types")
             or self._job.get("resources").get("gpu_types"),
@@ -500,46 +497,46 @@
             and status == "finished"
             and self.status == "stopped"
         ):
             return
 
         POLL_INTERVAL_MIN = 5
         POLL_INTERVAL_MAX = 60
-        POLL_INTERVAL = max(
-            min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN
-        )
+        POLL_INTERVAL = max(min(timeout / 60, POLL_INTERVAL_MAX), POLL_INTERVAL_MIN)
         retry_count = math.ceil(timeout / POLL_INTERVAL)
         count = 0
         while count < retry_count:
             await asyncio.sleep(POLL_INTERVAL)
             try:
                 await self.refresh()
             except ApiError as e:
                 if status == "archived" and e.status == 404:
                     return
                 raise e
             if (
                 self.status == status
                 or (
-                    self.type == "training"
-                    and status == "finished"
-                    and self.status == "stopped"
-                )
-                or (
                     status
                     in [
                         "waiting for GPUs",
                         "waiting for resources",
                     ]  ## this status could be very short and the polling could miss it
-                    and self.status in ["starting", "provisioning", "running"]
+                    and self.status
+                    not in ["new", "waiting for GPUs", "waiting for resources"]
                 )
                 or (
                     status
                     == "waiting for data/model download"  ## this status could be very short and the polling could miss it
-                    and self.status in ["starting", "provisioning", "running"]
+                    and self.status
+                    not in [
+                        "new",
+                        "waiting for GPUs",
+                        "waiting for resources",
+                        "waiting for data/model download",
+                    ]
                 )
             ):
                 return self
             elif self.status == "failed":
                 raise JobError(self.status, self)
             else:
                 count += 1
```

### Comparing `proximl-0.5.4/proximl/models.py` & `proximl-0.5.5/proximl/models.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/projects.py` & `proximl-0.5.5/proximl/projects.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/proximl/proximl.py` & `proximl-0.5.5/proximl/proximl.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import traceback
 from importlib.metadata import version
 
 from proximl.auth import Auth
 from proximl.datasets import Datasets
 from proximl.models import Models
 from proximl.checkpoints import Checkpoints
+from proximl.volumes import Volumes
 from proximl.jobs import Jobs
 from proximl.gpu_types import GpuTypes
 from proximl.environments import Environments
 from proximl.exceptions import ApiError, ProxiMLException
 from proximl.connections import Connections
 from proximl.projects import Projects
 from proximl.cloudbender import Cloudbender
@@ -62,14 +63,15 @@
             kwargs.get("project")
             or os.environ.get("PROXIML_PROJECT")
             or config.get("project")
         )
         self.datasets = Datasets(self)
         self.models = Models(self)
         self.checkpoints = Checkpoints(self)
+        self.volumes = Volumes(self)
         self.jobs = Jobs(self)
         self.gpu_types = GpuTypes(self)
         self.environments = Environments(self)
         self.connections = Connections(self)
         self.projects = Projects(self)
         self.cloudbender = Cloudbender(self)
         self.api_url = (
@@ -113,17 +115,15 @@
             else {
                 "Authorization": tokens.get("id_token"),
                 "User-Agent": f"proxiML-sdk/{self._version}",
             }
         )
         if params:
             if not isinstance(params, dict):
-                raise ProxiMLException(
-                    "Query parameters must be a valid dictionary"
-                )
+                raise ProxiMLException("Query parameters must be a valid dictionary")
             params = {
                 k: (str(v).lower() if isinstance(v, bool) else v)
                 for k, v in params.items()
             }  ## aiohttp doesn't support boolean
         if (
             method != "POST"
             and self.active_project
@@ -151,21 +151,17 @@
                 params=params,
             ) as resp:
                 if (resp.status // 100) in [4, 5]:
                     what = await resp.read()
                     content_type = resp.headers.get("content-type", "")
                     resp.close()
                     if content_type == "application/json":
-                        raise ApiError(
-                            resp.status, json.loads(what.decode("utf8"))
-                        )
+                        raise ApiError(resp.status, json.loads(what.decode("utf8")))
                     else:
-                        raise ApiError(
-                            resp.status, {"message": what.decode("utf8")}
-                        )
+                        raise ApiError(resp.status, {"message": what.decode("utf8")})
                 results = await resp.json()
                 return results
 
     async def _ws_subscribe(self, entity, project_uuid, id, msg_handler):
         headers = {
             "User-Agent": f"proxiML-sdk/{self._version}",
             "Content-Type": "application/json",
@@ -269,23 +265,19 @@
                                 asyncio.create_task(delayed_close(ws))
                             else:
                                 msg_handler(data)
                     connection_tries = 0
                     logging.debug(f"Websocket Disconnected.  Done? {done}")
                 except Exception as e:
                     connection_tries += 1
-                    logging.debug(
-                        f"Connection error: {traceback.format_exc()}"
-                    )
+                    logging.debug(f"Connection error: {traceback.format_exc()}")
                     if connection_tries == 5:
                         raise ApiError(
                             500,
-                            {
-                                "message": f"Connection error: {traceback.format_exc()}"
-                            },
+                            {"message": f"Connection error: {traceback.format_exc()}"},
                         )
 
     def set_active_project(self, project_uuid):
         CONFIG_DIR = os.path.expanduser(
             os.environ.get("PROXIML_CONFIG_DIR") or "~/.proximl"
         )
         with open(f"{CONFIG_DIR}/config.json", "w") as file:
```

### Comparing `proximl-0.5.4/proximl.egg-info/PKG-INFO` & `proximl-0.5.5/proximl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.4
+Version: 0.5.5
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.4 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.5 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.4/proximl.egg-info/SOURCES.txt` & `proximl-0.5.5/proximl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 proximl/environments.py
 proximl/exceptions.py
 proximl/gpu_types.py
 proximl/jobs.py
 proximl/models.py
 proximl/projects.py
 proximl/proximl.py
+proximl/volumes.py
 proximl.egg-info/PKG-INFO
 proximl.egg-info/SOURCES.txt
 proximl.egg-info/dependency_links.txt
 proximl.egg-info/entry_points.txt
 proximl.egg-info/requires.txt
 proximl.egg-info/top_level.txt
 proximl/cli/__init__.py
 proximl/cli/checkpoint.py
 proximl/cli/connection.py
 proximl/cli/dataset.py
 proximl/cli/environment.py
 proximl/cli/gpu.py
 proximl/cli/model.py
 proximl/cli/project.py
+proximl/cli/volume.py
 proximl/cli/cloudbender/__init__.py
 proximl/cli/cloudbender/datastore.py
 proximl/cli/cloudbender/device.py
 proximl/cli/cloudbender/node.py
 proximl/cli/cloudbender/provider.py
 proximl/cli/cloudbender/region.py
 proximl/cli/cloudbender/reservation.py
@@ -56,14 +58,15 @@
 tests/integration/test_checkpoints_integration.py
 tests/integration/test_datasets_integration.py
 tests/integration/test_environments_integration.py
 tests/integration/test_gpu_types_integration.py
 tests/integration/test_jobs_integration.py
 tests/integration/test_models_integration.py
 tests/integration/test_projects_integration.py
+tests/integration/test_volumes_integration.py
 tests/integration/cloudbender/__init__.py
 tests/integration/cloudbender/test_providers_integration.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_auth.py
 tests/unit/test_checkpoints_unit.py
 tests/unit/test_connections_unit.py
@@ -71,23 +74,25 @@
 tests/unit/test_environments_unit.py
 tests/unit/test_exceptions.py
 tests/unit/test_gpu_types_unit.py
 tests/unit/test_jobs_unit.py
 tests/unit/test_models_unit.py
 tests/unit/test_projects_unit.py
 tests/unit/test_proximl.py
+tests/unit/test_volumes_unit.py
 tests/unit/cli/__init__.py
 tests/unit/cli/conftest.py
 tests/unit/cli/test_cli_checkpoint_unit.py
 tests/unit/cli/test_cli_datasets_unit.py
 tests/unit/cli/test_cli_environment_unit.py
 tests/unit/cli/test_cli_gpu_unit.py
 tests/unit/cli/test_cli_job_unit.py
 tests/unit/cli/test_cli_model_unit.py
 tests/unit/cli/test_cli_project_unit.py
+tests/unit/cli/test_cli_volume_unit.py
 tests/unit/cli/cloudbender/__init__.py
 tests/unit/cli/cloudbender/test_cli_datastore_unit.py
 tests/unit/cli/cloudbender/test_cli_device_unit.py
 tests/unit/cli/cloudbender/test_cli_node_unit.py
 tests/unit/cli/cloudbender/test_cli_provider_unit.py
 tests/unit/cli/cloudbender/test_cli_region_unit.py
 tests/unit/cli/cloudbender/test_cli_reservation_unit.py
```

### Comparing `proximl-0.5.4/pyproject.toml` & `proximl-0.5.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.pytest.ini_options]
 python_files = "test_*"
 python_classes = "*Tests"
 python_functions = "test_*"
 asyncio_mode = "auto"
-testpaths = [
-    "tests",
-]
+testpaths = ["tests"]
 markers = [
     "create: Tests that create resources on the proximl platform",
     "gpu_types: Gpu Type tests",
     "environments: Environment tests",
     "datasets: Datasets tests",
     "models: Models tests",
     "checkpoints: Checkpoints tests",
+    "volumes: Volumes tests",
     "jobs: Jobs tests",
     "connections: Connections tests",
     "projects: Projects tests",
     "cloudbender: CloudBender tests",
     "providers: Providers tests",
     "regions: Regions tests",
     "nodes: Nodes tests",
     "devices: Devices tests",
     "datastores: Datastores tests",
     "reservations: Reservations tests",
     "device_configs: DeviceConfigs tests",
     "unit: All unit tests (no proxiML environment required)",
     "integration: All integration tests (proxiML environment required)",
     "sdk: All tests of the SDK",
-    "cli: All test of the cli"
-]
+    "cli: All test of the cli",
+]
```

### Comparing `proximl-0.5.4/setup.py` & `proximl-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/integration/cloudbender/test_providers_integration.py` & `proximl-0.5.5/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/integration/conftest.py` & `proximl-0.5.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/integration/test_checkpoints_integration.py` & `proximl-0.5.5/tests/integration/test_checkpoints_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,26 +50,28 @@
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
 
 @mark.create
 @mark.asyncio
-async def test_checkpoint_aws(proximl, capsys):
+async def test_checkpoint_wasabi(proximl, capsys):
     checkpoint = await proximl.checkpoints.create(
-        name="CLI Automated AWS",
-        source_type="aws",
-        source_uri="s3://proximl-examples/models/mxnet-model.zip",
+        name="CLI Automated Wasabi",
+        source_type="wasabi",
+        source_uri="s3://proximl-example/models/proximl-examples",
+        capacity="10G",
+        source_options=dict(endpoint_url="https://s3.wasabisys.com"),
     )
     checkpoint = await checkpoint.wait_for("ready", 300)
     status = checkpoint.status
     size = checkpoint.size
     await checkpoint.remove()
     assert status == "ready"
-    assert size >= 1000000
+    assert size >= 500000
 
 
 @mark.create
 @mark.asyncio
 async def test_checkpoint_local(proximl, capsys):
     checkpoint = await proximl.checkpoints.create(
         name="CLI Automated Local",
```

### Comparing `proximl-0.5.4/tests/integration/test_datasets_integration.py` & `proximl-0.5.5/tests/integration/test_datasets_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 @mark.create
 @mark.asyncio
 class GetDatasetTests:
     @fixture(scope="class")
     async def dataset(self, proximl):
         dataset = await proximl.datasets.create(
             name="CLI Automated",
-            source_type="aws",
-            source_uri="s3://proximl-examples/data/cifar10",
+            source_type="wasabi",
+            source_uri="s3://proximl-example/input/cifar-10/cifar-10-batches-bin",
+            source_options=dict(endpoint_url="https://s3.wasabisys.com"),
         )
         dataset = await dataset.wait_for("ready", 300)
         yield dataset
         await dataset.remove()
         dataset = await dataset.wait_for("archived", 60)
 
     async def test_get_public_datasets(self, proximl):
@@ -44,17 +45,15 @@
         regex = r"^{.*\"dataset_uuid\": \"" + dataset.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_dataset_repr(self, dataset):
         string = repr(dataset)
         regex = (
-            r"^Dataset\( proximl , \*\*{.*'dataset_uuid': '"
-            + dataset.id
-            + r"'.*}\)$"
+            r"^Dataset\( proximl , \*\*{.*'dataset_uuid': '" + dataset.id + r"'.*}\)$"
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_get_dataset_log_url(self, dataset, request):
         env = request.config.getoption("--env")
         regex = (
```

### Comparing `proximl-0.5.4/tests/integration/test_environments_integration.py` & `proximl-0.5.5/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/integration/test_gpu_types_integration.py` & `proximl-0.5.5/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/integration/test_jobs_integration.py` & `proximl-0.5.5/tests/integration/test_jobs_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
                 disk_size=10,
                 data=dict(
                     output_uri="s3://proximl-examples/output/resnet_cifar10",
                     output_type="aws",
                 ),
             )
         assert (
-            "Invalid Request - Only regional datastore are allowed for Notebook and Endpoint output locations"
+            "Invalid Request - output_type invalid for Notebook and Endpoint jobs"
             in error.value.message
         )
 
     async def test_invalid_output_type_for_endpoint(self, proximl):
         with raises(ApiError) as error:
             await proximl.jobs.create(
                 name="Invalid Output Type for Endpoint",
@@ -294,15 +294,53 @@
                 ),
                 data=dict(
                     output_uri="s3://proximl-examples/output/resnet_cifar10",
                     output_type="aws",
                 ),
             )
         assert (
-            "Invalid Request - Only regional datastore are allowed for Notebook and Endpoint output locations"
+            "Invalid Request - output_type invalid for Notebook and Endpoint jobs"
+            in error.value.message
+        )
+
+    async def test_invalid_volumes_for_training(self, proximl):
+        with raises(ApiError) as error:
+            await proximl.jobs.create(
+                name="Invalid Volumes for Training",
+                type="training",
+                gpu_types=["rtx3090"],
+                disk_size=10,
+                data=dict(
+                    output_uri="s3://proximl-examples/output/resnet_cifar10",
+                    output_type="aws",
+                    volumes=["volume-id"],
+                ),
+                workers=["python train.py"],
+            )
+        assert (
+            "Invalid Request - Only Notebook and Endpoint job types can use writable volumes"
+            in error.value.message
+        )
+
+    async def test_invalid_volumes_for_inference(self, proximl):
+        with raises(ApiError) as error:
+            await proximl.jobs.create(
+                name="Invalid Volumes for Inference",
+                type="inference",
+                gpu_types=["rtx3090"],
+                disk_size=10,
+                data=dict(
+                    output_uri="s3://proximl-examples/output/resnet_cifar10",
+                    output_type="aws",
+                    volumes=["volume-id"],
+                ),
+                workers=["python predict.py"],
+            )
+        assert (
+            "Invalid Request - Only Notebook and Endpoint job types can use writable volumes"
             in error.value.message
         )
 
     async def test_invalid_datasets_for_inference(self, proximl):
         with raises(ApiError) as error:
             await proximl.jobs.create(
                 name="Datasets for Inference Job",
```

### Comparing `proximl-0.5.4/tests/integration/test_models_integration.py` & `proximl-0.5.5/tests/integration/test_models_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,37 +39,35 @@
         string = str(model)
         regex = r"^{.*\"model_uuid\": \"" + model.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_model_repr(self, model):
         string = repr(model)
-        regex = (
-            r"^Model\( proximl , \*\*{.*'model_uuid': '"
-            + model.id
-            + r"'.*}\)$"
-        )
+        regex = r"^Model\( proximl , \*\*{.*'model_uuid': '" + model.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
 
 @mark.create
 @mark.asyncio
-async def test_model_aws(proximl, capsys):
+async def test_model_wasabi(proximl, capsys):
     model = await proximl.models.create(
-        name="CLI Automated AWS",
-        source_type="aws",
-        source_uri="s3://proximl-examples/models/mxnet-model.zip",
+        name="CLI Automated Wasabi",
+        source_type="wasabi",
+        source_uri="s3://proximl-example/models/proximl-examples",
+        capacity="10G",
+        source_options=dict(endpoint_url="https://s3.wasabisys.com"),
     )
     model = await model.wait_for("ready", 300)
     status = model.status
     size = model.size
     await model.remove()
     assert status == "ready"
-    assert size >= 1000000
+    assert size >= 500000
 
 
 @mark.create
 @mark.asyncio
 async def test_model_local(proximl, capsys):
     model = await proximl.models.create(
         name="CLI Automated Local",
```

### Comparing `proximl-0.5.4/tests/integration/test_projects_integration.py` & `proximl-0.5.5/tests/integration/test_projects_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 
 @mark.create
 @mark.asyncio
 class GetProjectsTests:
     @fixture(scope="class")
     async def project(self, proximl):
-        project = await proximl.projects.create(
-            name="New Project", copy_keys=False
-        )
+        project = await proximl.projects.create(name="New Project", copy_keys=False)
         yield project
         await project.remove()
 
     async def test_get_projects(self, proximl):
         projects = await proximl.projects.list()
         assert len(projects) > 0
 
@@ -37,12 +35,10 @@
         string = str(project)
         regex = r"^{.*\"id\": \"" + project.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_project_repr(self, project):
         string = repr(project)
-        regex = (
-            r"^Project\( proximl , \*\*{.*'id': '" + project.id + r"'.*}\)$"
-        )
+        regex = r"^Project\( proximl , \*\*{.*'id': '" + project.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
```

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/cloudbender/test_cli_reservation_unit.py` & `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_checkpoint_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_datasets_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_environment_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_gpu_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_job_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_model_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cli/test_cli_project_unit.py` & `proximl-0.5.5/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_datastores_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_device_configs_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_devices_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_nodes_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_providers_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_regions_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/cloudbender/test_reservations_unit.py` & `proximl-0.5.5/tests/unit/cloudbender/test_reservations_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/conftest.py` & `proximl-0.5.5/tests/unit/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pytest import fixture, mark
 from unittest.mock import Mock, AsyncMock, patch, create_autospec
 
 from proximl.proximl import ProxiML
 from proximl.auth import Auth
 from proximl.datasets import Dataset, Datasets
 from proximl.checkpoints import Checkpoint, Checkpoints
+from proximl.volumes import Volume, Volumes
 from proximl.models import Model, Models
 from proximl.gpu_types import GpuType, GpuTypes
 from proximl.environments import Environment, Environments
 from proximl.jobs import Job, Jobs
 from proximl.connections import Connections
 from proximl.projects import (
     Projects,
@@ -255,14 +256,87 @@
             size=10000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
     ]
 
 
 @fixture(scope="session")
+def mock_my_volumes():
+    proximl = Mock()
+    yield [
+        Volume(
+            proximl,
+            id="1",
+            project_uuid="proj-id-1",
+            name="first one",
+            status="ready",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2020-12-31T23:59:59.000Z",
+        ),
+        Volume(
+            proximl,
+            id="2",
+            project_uuid="proj-id-1",
+            name="second one",
+            status="ready",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Volume(
+            proximl,
+            id="3",
+            project_uuid="proj-id-1",
+            name="first one",
+            status="ready",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Volume(
+            proximl,
+            id="4",
+            project_uuid="proj-id-1",
+            name="other one",
+            status="ready",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2020-12-31T23:59:59.000Z",
+        ),
+        Volume(
+            proximl,
+            id="5",
+            project_uuid="proj-id-1",
+            name="not ready",
+            status="new",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Volume(
+            proximl,
+            id="6",
+            project_uuid="proj-id-1",
+            name="failed",
+            status="failed",
+            capacity="10G",
+            used_size=100000000,
+            billed_size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+    ]
+
+
+@fixture(scope="session")
 def mock_gpu_types():
     proximl = Mock()
     yield [
         GpuType(
             proximl,
             **{
                 "name": "A100",
@@ -899,14 +973,17 @@
     ]
 
 
 @fixture(scope="function")
 def mock_proximl(
     mock_my_datasets,
     mock_public_datasets,
+    mock_my_checkpoints,
+    mock_public_checkpoints,
+    mock_my_volumes,
     mock_models,
     mock_gpu_types,
     mock_environments,
     mock_jobs,
     mock_projects,
     mock_providers,
     mock_regions,
@@ -917,27 +994,27 @@
     mock_device_configs,
 ):
     proximl = create_autospec(ProxiML)
     proximl.active_project = "proj-id-1"
     proximl.project = "proj-id-1"
     proximl.datasets = create_autospec(Datasets)
     proximl.checkpoints = create_autospec(Checkpoints)
+    proximl.volumes = create_autospec(Volumes)
     proximl.models = create_autospec(Models)
     proximl.gpu_types = create_autospec(GpuTypes)
     proximl.environments = create_autospec(Environments)
     proximl.jobs = create_autospec(Jobs)
     proximl.connections = create_autospec(Connections)
     proximl.projects = create_autospec(Projects)
     proximl.datasets.list = AsyncMock(return_value=mock_my_datasets)
     proximl.datasets.list_public = AsyncMock(return_value=mock_public_datasets)
     proximl.checkpoints.list = AsyncMock(return_value=mock_my_checkpoints)
-    proximl.checkpoints.list_public = AsyncMock(
-        return_value=mock_public_checkpoints
-    )
+    proximl.checkpoints.list_public = AsyncMock(return_value=mock_public_checkpoints)
     proximl.models.list = AsyncMock(return_value=mock_models)
+    proximl.volumes.list = AsyncMock(return_value=mock_my_volumes)
     proximl.gpu_types.list = AsyncMock(return_value=mock_gpu_types)
     proximl.environments.list = AsyncMock(return_value=mock_environments)
     proximl.jobs.list = AsyncMock(return_value=mock_jobs)
     proximl.projects.list = AsyncMock(return_value=mock_projects)
 
     proximl.cloudbender = create_autospec(Cloudbender)
 
@@ -946,19 +1023,15 @@
     proximl.cloudbender.regions = create_autospec(Regions)
     proximl.cloudbender.regions.list = AsyncMock(return_value=mock_regions)
     proximl.cloudbender.nodes = create_autospec(Nodes)
     proximl.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     proximl.cloudbender.devices = create_autospec(Nodes)
     proximl.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     proximl.cloudbender.datastores = create_autospec(Datastores)
-    proximl.cloudbender.datastores.list = AsyncMock(
-        return_value=mock_datastores
-    )
+    proximl.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
     proximl.cloudbender.reservations = create_autospec(Reservations)
-    proximl.cloudbender.reservations.list = AsyncMock(
-        return_value=mock_reservations
-    )
+    proximl.cloudbender.reservations.list = AsyncMock(return_value=mock_reservations)
     proximl.cloudbender.device_configs = create_autospec(DeviceConfigs)
     proximl.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield proximl
```

### Comparing `proximl-0.5.4/tests/unit/test_auth.py` & `proximl-0.5.5/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_checkpoints_unit.py` & `proximl-0.5.5/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_connections_unit.py` & `proximl-0.5.5/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_datasets_unit.py` & `proximl-0.5.5/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_environments_unit.py` & `proximl-0.5.5/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_exceptions.py` & `proximl-0.5.5/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_gpu_types_unit.py` & `proximl-0.5.5/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_jobs_unit.py` & `proximl-0.5.5/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_models_unit.py` & `proximl-0.5.5/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_projects_unit.py` & `proximl-0.5.5/tests/unit/test_projects_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.4/tests/unit/test_proximl.py` & `proximl-0.5.5/tests/unit/test_proximl.py`

 * *Files identical despite different names*

