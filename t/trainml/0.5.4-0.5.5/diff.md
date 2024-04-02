# Comparing `tmp/trainml-0.5.4.tar.gz` & `tmp/trainml-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainml-0.5.4.tar", last modified: Wed Feb 14 16:00:53 2024, max compression
+gzip compressed data, was "trainml-0.5.5.tar", last modified: Tue Apr  2 13:15:54 2024, max compression
```

## Comparing `trainml-0.5.4.tar` & `trainml-0.5.5.tar`

### file list

```diff
@@ -1,118 +1,123 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.081632 trainml-0.5.4/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.4/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-02-14 16:00:53.081483 trainml-0.5.4/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.4/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.058548 trainml-0.5.4/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.4/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.4/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.4/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.4/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      975 2023-06-23 16:08:41.000000 trainml-0.5.4/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-02-14 16:00:53.081681 trainml-0.5.4/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.4/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.056366 trainml-0.5.4/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.061066 trainml-0.5.4/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.4/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.061418 trainml-0.5.4/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.4/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.4/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.4/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3128 2023-03-20 21:28:50.000000 trainml-0.5.4/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3424 2023-03-20 21:28:58.000000 trainml-0.5.4/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.4/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.4/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    23341 2024-02-13 19:56:57.000000 trainml-0.5.4/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2848 2023-03-20 21:29:23.000000 trainml-0.5.4/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1492 2023-03-20 21:29:29.000000 trainml-0.5.4/tests/integration/test_projects_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.065125 trainml-0.5.4/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.4/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.067463 trainml-0.5.4/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.4/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.068858 trainml-0.5.4/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.4/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-06-22 02:20:03.000000 trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.4/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.4/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.4/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.4/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.4/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.4/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.4/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2023-06-22 01:48:21.000000 trainml-0.5.4/tests/unit/cli/test_cli_project_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.070636 trainml-0.5.4/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.4/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.4/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.4/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.4/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.4/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.4/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.4/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2023-06-23 16:54:00.000000 trainml-0.5.4/tests/unit/cloudbender/test_reservations_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    29059 2023-06-23 19:46:53.000000 trainml-0.5.4/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.4/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.4/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.4/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.4/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.4/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.4/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.4/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.4/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.4/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2023-06-22 01:37:38.000000 trainml-0.5.4/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.4/tests/unit/test_trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.073979 trainml-0.5.4/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-02-14 15:59:51.000000 trainml-0.5.4/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.4/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.4/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2023-09-08 19:04:34.000000 trainml-0.5.4/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.076591 trainml-0.5.4/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4338 2023-06-19 19:39:43.000000 trainml-0.5.4/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.4/trainml/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.078230 trainml-0.5.4/trainml/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      534 2023-06-23 19:38:26.000000 trainml-0.5.4/trainml/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.4/trainml/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.4/trainml/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.4/trainml/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.4/trainml/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.4/trainml/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2023-06-22 02:14:39.000000 trainml-0.5.4/trainml/cli/cloudbender/reservation.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.4/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.4/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.4/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.4/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.078703 trainml-0.5.4/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.4/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.4/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.4/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2023-06-21 21:09:43.000000 trainml-0.5.4/trainml/cli/project.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.081116 trainml-0.5.4/trainml/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.4/trainml/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      634 2023-06-23 15:52:00.000000 trainml-0.5.4/trainml/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.4/trainml/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.4/trainml/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.4/trainml/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.4/trainml/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.4/trainml/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.4/trainml/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2023-06-23 16:23:17.000000 trainml-0.5.4/trainml/cloudbender/reservations.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.4/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-01-23 15:13:39.000000 trainml-0.5.4/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.4/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2023-01-05 20:17:59.000000 trainml-0.5.4/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.4/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17807 2023-06-19 18:48:46.000000 trainml-0.5.4/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2023-09-08 19:05:25.000000 trainml-0.5.4/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2023-06-21 21:05:20.000000 trainml-0.5.4/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    11045 2023-09-08 15:42:05.000000 trainml-0.5.4/trainml/trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-02-14 16:00:53.074764 trainml-0.5.4/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3344 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-02-14 16:00:53.000000 trainml-0.5.4/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.186591 trainml-0.5.5/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.5/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-02 13:15:54.186436 trainml-0.5.5/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.5/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.164142 trainml-0.5.5/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.5/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.5/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.5/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.5/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1000 2024-02-29 19:07:44.000000 trainml-0.5.5/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-02 13:15:54.186637 trainml-0.5.5/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.5/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.162157 trainml-0.5.5/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.166468 trainml-0.5.5/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.5/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.166835 trainml-0.5.5/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.5/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.5/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.5/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.5/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.5/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.5/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.5/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-03-19 18:51:28.000000 trainml-0.5.5/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.5/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.5/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.5/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.170410 trainml-0.5.5/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.5/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.172501 trainml-0.5.5/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.5/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.173898 trainml-0.5.5/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.5/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-06-22 02:20:03.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.5/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.5/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.5/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.5/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.5/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.5/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2023-06-22 01:48:21.000000 trainml-0.5.5/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.5/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.175686 trainml-0.5.5/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.5/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.5/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.5/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.5/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.5/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.5/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2023-06-23 16:54:00.000000 trainml-0.5.5/tests/unit/cloudbender/test_reservations_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31197 2024-03-12 15:29:40.000000 trainml-0.5.5/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.5/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.5/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.5/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.5/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.5/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.5/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.5/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.5/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.5/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2023-06-22 01:37:38.000000 trainml-0.5.5/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.5/tests/unit/test_trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.5/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.179251 trainml-0.5.5/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-02 13:13:59.000000 trainml-0.5.5/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.5/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.5/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2023-09-08 19:04:34.000000 trainml-0.5.5/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.181962 trainml-0.5.5/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.5/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.5/trainml/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.183442 trainml-0.5.5/trainml/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      534 2023-06-23 19:38:26.000000 trainml-0.5.5/trainml/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.5/trainml/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.5/trainml/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.5/trainml/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.5/trainml/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.5/trainml/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2023-06-22 02:14:39.000000 trainml-0.5.5/trainml/cli/cloudbender/reservation.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.5/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.5/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.5/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.5/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.183921 trainml-0.5.5/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.5/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.5/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.5/trainml/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2023-06-21 21:09:43.000000 trainml-0.5.5/trainml/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.5/trainml/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.186145 trainml-0.5.5/trainml/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.5/trainml/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      634 2023-06-23 15:52:00.000000 trainml-0.5.5/trainml/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.5/trainml/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.5/trainml/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.5/trainml/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.5/trainml/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.5/trainml/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.5/trainml/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2023-06-23 16:23:17.000000 trainml-0.5.5/trainml/cloudbender/reservations.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.5/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-01-23 15:13:39.000000 trainml-0.5.5/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.5/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.5/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.5/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-03-11 15:18:02.000000 trainml-0.5.5/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2023-09-08 19:05:25.000000 trainml-0.5.5/trainml/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2023-06-21 21:05:20.000000 trainml-0.5.5/trainml/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.5/trainml/trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-03-12 13:04:15.000000 trainml-0.5.5/trainml/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.180047 trainml-0.5.5/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3502 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.5.4/LICENSE` & `trainml-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/PKG-INFO` & `trainml-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.4
+Version: 0.5.5
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.4 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.5 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.4/README.md` & `trainml-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/examples/create_dataset_and_training_job.py` & `trainml-0.5.5/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/examples/local_storage.py` & `trainml-0.5.5/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/examples/training_inference_pipeline.py` & `trainml-0.5.5/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/pyproject.toml` & `trainml-0.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

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
     "create: Tests that create resources on the trainml platform",
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
     "unit: All unit tests (no trainML environment required)",
     "integration: All integration tests (trainML environment required)",
     "sdk: All tests of the SDK",
-    "cli: All test of the cli"
-]
+    "cli: All test of the cli",
+]
```

### Comparing `trainml-0.5.4/setup.py` & `trainml-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/integration/cloudbender/test_providers_integration.py` & `trainml-0.5.5/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/integration/conftest.py` & `trainml-0.5.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/integration/test_checkpoints_integration.py` & `trainml-0.5.5/tests/integration/test_checkpoints_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,28 @@
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
 
 @mark.create
 @mark.asyncio
-async def test_checkpoint_aws(trainml, capsys):
+async def test_checkpoint_wasabi(trainml, capsys):
     checkpoint = await trainml.checkpoints.create(
-        name="CLI Automated AWS",
-        source_type="aws",
-        source_uri="s3://trainml-examples/models/mxnet-model.zip",
+        name="CLI Automated Wasabi",
+        source_type="wasabi",
+        source_uri="s3://trainml-example/models/trainml-examples",
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
 async def test_checkpoint_local(trainml, capsys):
     checkpoint = await trainml.checkpoints.create(
         name="CLI Automated Local",
```

### Comparing `trainml-0.5.4/tests/integration/test_datasets_integration.py` & `trainml-0.5.5/tests/integration/test_datasets_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 @mark.create
 @mark.asyncio
 class GetDatasetTests:
     @fixture(scope="class")
     async def dataset(self, trainml):
         dataset = await trainml.datasets.create(
             name="CLI Automated",
-            source_type="aws",
-            source_uri="s3://trainml-examples/data/cifar10",
+            source_type="wasabi",
+            source_uri="s3://trainml-example/input/cifar-10/cifar-10-batches-bin",
+            source_options=dict(endpoint_url="https://s3.wasabisys.com"),
         )
         dataset = await dataset.wait_for("ready", 300)
         yield dataset
         await dataset.remove()
         dataset = await dataset.wait_for("archived", 60)
 
     async def test_get_public_datasets(self, trainml):
@@ -44,17 +45,15 @@
         regex = r"^{.*\"dataset_uuid\": \"" + dataset.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_dataset_repr(self, dataset):
         string = repr(dataset)
         regex = (
-            r"^Dataset\( trainml , \*\*{.*'dataset_uuid': '"
-            + dataset.id
-            + r"'.*}\)$"
+            r"^Dataset\( trainml , \*\*{.*'dataset_uuid': '" + dataset.id + r"'.*}\)$"
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_get_dataset_log_url(self, dataset, request):
         env = request.config.getoption("--env")
         regex = (
```

### Comparing `trainml-0.5.4/tests/integration/test_environments_integration.py` & `trainml-0.5.5/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/integration/test_gpu_types_integration.py` & `trainml-0.5.5/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/integration/test_jobs_integration.py` & `trainml-0.5.5/tests/integration/test_jobs_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
                 disk_size=10,
                 data=dict(
                     output_uri="s3://trainml-examples/output/resnet_cifar10",
                     output_type="aws",
                 ),
             )
         assert (
-            "Invalid Request - Only regional datastore are allowed for Notebook and Endpoint output locations"
+            "Invalid Request - output_type invalid for Notebook and Endpoint jobs"
             in error.value.message
         )
 
     async def test_invalid_output_type_for_endpoint(self, trainml):
         with raises(ApiError) as error:
             await trainml.jobs.create(
                 name="Invalid Output Type for Endpoint",
@@ -294,15 +294,53 @@
                 ),
                 data=dict(
                     output_uri="s3://trainml-examples/output/resnet_cifar10",
                     output_type="aws",
                 ),
             )
         assert (
-            "Invalid Request - Only regional datastore are allowed for Notebook and Endpoint output locations"
+            "Invalid Request - output_type invalid for Notebook and Endpoint jobs"
+            in error.value.message
+        )
+
+    async def test_invalid_volumes_for_training(self, trainml):
+        with raises(ApiError) as error:
+            await trainml.jobs.create(
+                name="Invalid Volumes for Training",
+                type="training",
+                gpu_types=["rtx3090"],
+                disk_size=10,
+                data=dict(
+                    output_uri="s3://trainml-examples/output/resnet_cifar10",
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
+    async def test_invalid_volumes_for_inference(self, trainml):
+        with raises(ApiError) as error:
+            await trainml.jobs.create(
+                name="Invalid Volumes for Inference",
+                type="inference",
+                gpu_types=["rtx3090"],
+                disk_size=10,
+                data=dict(
+                    output_uri="s3://trainml-examples/output/resnet_cifar10",
+                    output_type="aws",
+                    volumes=["volume-id"],
+                ),
+                workers=["python predict.py"],
+            )
+        assert (
+            "Invalid Request - Only Notebook and Endpoint job types can use writable volumes"
             in error.value.message
         )
 
     async def test_invalid_datasets_for_inference(self, trainml):
         with raises(ApiError) as error:
             await trainml.jobs.create(
                 name="Datasets for Inference Job",
```

### Comparing `trainml-0.5.4/tests/integration/test_models_integration.py` & `trainml-0.5.5/tests/integration/test_models_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,37 +39,35 @@
         string = str(model)
         regex = r"^{.*\"model_uuid\": \"" + model.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_model_repr(self, model):
         string = repr(model)
-        regex = (
-            r"^Model\( trainml , \*\*{.*'model_uuid': '"
-            + model.id
-            + r"'.*}\)$"
-        )
+        regex = r"^Model\( trainml , \*\*{.*'model_uuid': '" + model.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
 
 @mark.create
 @mark.asyncio
-async def test_model_aws(trainml, capsys):
+async def test_model_wasabi(trainml, capsys):
     model = await trainml.models.create(
-        name="CLI Automated AWS",
-        source_type="aws",
-        source_uri="s3://trainml-examples/models/mxnet-model.zip",
+        name="CLI Automated Wasabi",
+        source_type="wasabi",
+        source_uri="s3://trainml-example/models/trainml-examples",
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
 async def test_model_local(trainml, capsys):
     model = await trainml.models.create(
         name="CLI Automated Local",
```

### Comparing `trainml-0.5.4/tests/integration/test_projects_integration.py` & `trainml-0.5.5/tests/integration/test_projects_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 
 @mark.create
 @mark.asyncio
 class GetProjectsTests:
     @fixture(scope="class")
     async def project(self, trainml):
-        project = await trainml.projects.create(
-            name="New Project", copy_keys=False
-        )
+        project = await trainml.projects.create(name="New Project", copy_keys=False)
         yield project
         await project.remove()
 
     async def test_get_projects(self, trainml):
         projects = await trainml.projects.list()
         assert len(projects) > 0
 
@@ -37,12 +35,10 @@
         string = str(project)
         regex = r"^{.*\"id\": \"" + project.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_project_repr(self, project):
         string = repr(project)
-        regex = (
-            r"^Project\( trainml , \*\*{.*'id': '" + project.id + r"'.*}\)$"
-        )
+        regex = r"^Project\( trainml , \*\*{.*'id': '" + project.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
```

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/cloudbender/test_cli_reservation_unit.py` & `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_checkpoint_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_datasets_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_gpu_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_job_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_model_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cli/test_cli_project_unit.py` & `trainml-0.5.5/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_datastores_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_device_configs_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_devices_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_nodes_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_providers_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_regions_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/cloudbender/test_reservations_unit.py` & `trainml-0.5.5/tests/unit/cloudbender/test_reservations_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/conftest.py` & `trainml-0.5.5/tests/unit/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pytest import fixture, mark
 from unittest.mock import Mock, AsyncMock, patch, create_autospec
 
 from trainml.trainml import TrainML
 from trainml.auth import Auth
 from trainml.datasets import Dataset, Datasets
 from trainml.checkpoints import Checkpoint, Checkpoints
+from trainml.volumes import Volume, Volumes
 from trainml.models import Model, Models
 from trainml.gpu_types import GpuType, GpuTypes
 from trainml.environments import Environment, Environments
 from trainml.jobs import Job, Jobs
 from trainml.connections import Connections
 from trainml.projects import (
     Projects,
@@ -255,14 +256,87 @@
             size=10000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
     ]
 
 
 @fixture(scope="session")
+def mock_my_volumes():
+    trainml = Mock()
+    yield [
+        Volume(
+            trainml,
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
+            trainml,
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
+            trainml,
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
+            trainml,
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
+            trainml,
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
+            trainml,
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
     trainml = Mock()
     yield [
         GpuType(
             trainml,
             **{
                 "name": "A100",
@@ -899,14 +973,17 @@
     ]
 
 
 @fixture(scope="function")
 def mock_trainml(
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
     trainml = create_autospec(TrainML)
     trainml.active_project = "proj-id-1"
     trainml.project = "proj-id-1"
     trainml.datasets = create_autospec(Datasets)
     trainml.checkpoints = create_autospec(Checkpoints)
+    trainml.volumes = create_autospec(Volumes)
     trainml.models = create_autospec(Models)
     trainml.gpu_types = create_autospec(GpuTypes)
     trainml.environments = create_autospec(Environments)
     trainml.jobs = create_autospec(Jobs)
     trainml.connections = create_autospec(Connections)
     trainml.projects = create_autospec(Projects)
     trainml.datasets.list = AsyncMock(return_value=mock_my_datasets)
     trainml.datasets.list_public = AsyncMock(return_value=mock_public_datasets)
     trainml.checkpoints.list = AsyncMock(return_value=mock_my_checkpoints)
-    trainml.checkpoints.list_public = AsyncMock(
-        return_value=mock_public_checkpoints
-    )
+    trainml.checkpoints.list_public = AsyncMock(return_value=mock_public_checkpoints)
     trainml.models.list = AsyncMock(return_value=mock_models)
+    trainml.volumes.list = AsyncMock(return_value=mock_my_volumes)
     trainml.gpu_types.list = AsyncMock(return_value=mock_gpu_types)
     trainml.environments.list = AsyncMock(return_value=mock_environments)
     trainml.jobs.list = AsyncMock(return_value=mock_jobs)
     trainml.projects.list = AsyncMock(return_value=mock_projects)
 
     trainml.cloudbender = create_autospec(Cloudbender)
 
@@ -946,19 +1023,15 @@
     trainml.cloudbender.regions = create_autospec(Regions)
     trainml.cloudbender.regions.list = AsyncMock(return_value=mock_regions)
     trainml.cloudbender.nodes = create_autospec(Nodes)
     trainml.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     trainml.cloudbender.devices = create_autospec(Nodes)
     trainml.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     trainml.cloudbender.datastores = create_autospec(Datastores)
-    trainml.cloudbender.datastores.list = AsyncMock(
-        return_value=mock_datastores
-    )
+    trainml.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
     trainml.cloudbender.reservations = create_autospec(Reservations)
-    trainml.cloudbender.reservations.list = AsyncMock(
-        return_value=mock_reservations
-    )
+    trainml.cloudbender.reservations.list = AsyncMock(return_value=mock_reservations)
     trainml.cloudbender.device_configs = create_autospec(DeviceConfigs)
     trainml.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield trainml
```

### Comparing `trainml-0.5.4/tests/unit/test_auth.py` & `trainml-0.5.5/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_checkpoints_unit.py` & `trainml-0.5.5/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_connections_unit.py` & `trainml-0.5.5/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_datasets_unit.py` & `trainml-0.5.5/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_environments_unit.py` & `trainml-0.5.5/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_exceptions.py` & `trainml-0.5.5/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_gpu_types_unit.py` & `trainml-0.5.5/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_jobs_unit.py` & `trainml-0.5.5/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_models_unit.py` & `trainml-0.5.5/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_projects_unit.py` & `trainml-0.5.5/tests/unit/test_projects_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/tests/unit/test_trainml.py` & `trainml-0.5.5/tests/unit/test_trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/auth.py` & `trainml-0.5.5/trainml/auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/checkpoints.py` & `trainml-0.5.5/trainml/checkpoints.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/__init__.py` & `trainml-0.5.5/trainml/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,34 +138,31 @@
     projects = config.trainml.run(config.trainml.client.projects.list())
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
     config.trainml.client.set_active_project(selected_project[0].id)
 
 
 from trainml.cli.connection import connection
 from trainml.cli.dataset import dataset
 from trainml.cli.model import model
 from trainml.cli.checkpoint import checkpoint
+from trainml.cli.volume import volume
 from trainml.cli.environment import environment
 from trainml.cli.gpu import gpu
 from trainml.cli.job import job
 from trainml.cli.project import project
 from trainml.cli.cloudbender import cloudbender
```

### Comparing `trainml-0.5.4/trainml/cli/checkpoint.py` & `trainml-0.5.5/trainml/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/__init__.py` & `trainml-0.5.5/trainml/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/datastore.py` & `trainml-0.5.5/trainml/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/device.py` & `trainml-0.5.5/trainml/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/node.py` & `trainml-0.5.5/trainml/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/provider.py` & `trainml-0.5.5/trainml/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/region.py` & `trainml-0.5.5/trainml/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/cloudbender/reservation.py` & `trainml-0.5.5/trainml/cli/cloudbender/reservation.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/connection.py` & `trainml-0.5.5/trainml/cli/connection.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/dataset.py` & `trainml-0.5.5/trainml/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/environment.py` & `trainml-0.5.5/trainml/cli/environment.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/gpu.py` & `trainml-0.5.5/trainml/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/job/__init__.py` & `trainml-0.5.5/trainml/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/job/create.py` & `trainml-0.5.5/trainml/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/model.py` & `trainml-0.5.5/trainml/cli/model.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cli/project.py` & `trainml-0.5.5/trainml/cli/project.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/cloudbender.py` & `trainml-0.5.5/trainml/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/datastores.py` & `trainml-0.5.5/trainml/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/device_configs.py` & `trainml-0.5.5/trainml/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/devices.py` & `trainml-0.5.5/trainml/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/nodes.py` & `trainml-0.5.5/trainml/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/providers.py` & `trainml-0.5.5/trainml/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/regions.py` & `trainml-0.5.5/trainml/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/cloudbender/reservations.py` & `trainml-0.5.5/trainml/cloudbender/reservations.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/connections.py` & `trainml-0.5.5/trainml/connections.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/datasets.py` & `trainml-0.5.5/trainml/datasets.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/environments.py` & `trainml-0.5.5/trainml/environments.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/exceptions.py` & `trainml-0.5.5/trainml/exceptions.py`

 * *Files 6% similar despite different names*

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
+class VolumeError(TrainMLException):
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
 
 
 class ConnectionError(TrainMLException):
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

### Comparing `trainml-0.5.4/trainml/gpu_types.py` & `trainml-0.5.5/trainml/gpu_types.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/jobs.py` & `trainml-0.5.5/trainml/jobs.py`

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
-            or self.trainml.active_project,
+            project_uuid=kwargs.get("project_uuid") or self.trainml.active_project,
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
         resp = await self.trainml._query("/job", "POST", None, payload)
         job = Job(self.trainml, **resp)
         return job
 
     async def remove(self, id, **kwargs):
-        await self.trainml._query(
-            f"/job/{id}", "DELETE", dict(**kwargs, force=True)
-        )
+        await self.trainml._query(f"/job/{id}", "DELETE", dict(**kwargs, force=True))
 
 
 class Job:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
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
         self.__init__(self.trainml, **resp)
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
             await self.trainml._ws_subscribe(
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
 
         job = await self.trainml.jobs.create(
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

### Comparing `trainml-0.5.4/trainml/models.py` & `trainml-0.5.5/trainml/models.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/projects.py` & `trainml-0.5.5/trainml/projects.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.4/trainml/trainml.py` & `trainml-0.5.5/trainml/trainml.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import traceback
 from importlib.metadata import version
 
 from trainml.auth import Auth
 from trainml.datasets import Datasets
 from trainml.models import Models
 from trainml.checkpoints import Checkpoints
+from trainml.volumes import Volumes
 from trainml.jobs import Jobs
 from trainml.gpu_types import GpuTypes
 from trainml.environments import Environments
 from trainml.exceptions import ApiError, TrainMLException
 from trainml.connections import Connections
 from trainml.projects import Projects
 from trainml.cloudbender import Cloudbender
@@ -62,14 +63,15 @@
             kwargs.get("project")
             or os.environ.get("TRAINML_PROJECT")
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
                 "User-Agent": f"trainML-sdk/{self._version}",
             }
         )
         if params:
             if not isinstance(params, dict):
-                raise TrainMLException(
-                    "Query parameters must be a valid dictionary"
-                )
+                raise TrainMLException("Query parameters must be a valid dictionary")
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
             "User-Agent": f"trainML-sdk/{self._version}",
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
             os.environ.get("TRAINML_CONFIG_DIR") or "~/.trainml"
         )
         with open(f"{CONFIG_DIR}/config.json", "w") as file:
```

### Comparing `trainml-0.5.4/trainml.egg-info/PKG-INFO` & `trainml-0.5.5/trainml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.4
+Version: 0.5.5
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.4 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.5 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.4/trainml.egg-info/SOURCES.txt` & `trainml-0.5.5/trainml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
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
@@ -26,23 +27,25 @@
 tests/unit/test_environments_unit.py
 tests/unit/test_exceptions.py
 tests/unit/test_gpu_types_unit.py
 tests/unit/test_jobs_unit.py
 tests/unit/test_models_unit.py
 tests/unit/test_projects_unit.py
 tests/unit/test_trainml.py
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
@@ -63,28 +66,30 @@
 trainml/environments.py
 trainml/exceptions.py
 trainml/gpu_types.py
 trainml/jobs.py
 trainml/models.py
 trainml/projects.py
 trainml/trainml.py
+trainml/volumes.py
 trainml.egg-info/PKG-INFO
 trainml.egg-info/SOURCES.txt
 trainml.egg-info/dependency_links.txt
 trainml.egg-info/entry_points.txt
 trainml.egg-info/requires.txt
 trainml.egg-info/top_level.txt
 trainml/cli/__init__.py
 trainml/cli/checkpoint.py
 trainml/cli/connection.py
 trainml/cli/dataset.py
 trainml/cli/environment.py
 trainml/cli/gpu.py
 trainml/cli/model.py
 trainml/cli/project.py
+trainml/cli/volume.py
 trainml/cli/cloudbender/__init__.py
 trainml/cli/cloudbender/datastore.py
 trainml/cli/cloudbender/device.py
 trainml/cli/cloudbender/node.py
 trainml/cli/cloudbender/provider.py
 trainml/cli/cloudbender/region.py
 trainml/cli/cloudbender/reservation.py
```

