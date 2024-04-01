# Comparing `tmp/kafi-0.0.8.tar.gz` & `tmp/kafi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafi-0.0.8.tar", last modified: Sat Oct 14 12:09:26 2023, max compression
+gzip compressed data, was "kafi-0.0.9.tar", last modified: Tue Oct 17 20:59:26 2023, max compression
```

## Comparing `kafi-0.0.8.tar` & `kafi-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.709226 kafi-0.0.8/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    11357 2023-08-16 21:54:10.000000 kafi-0.0.8/LICENSE
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1172 2023-10-14 12:09:26.709226 kafi-0.0.8/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      599 2023-09-23 17:45:27.000000 kafi-0.0.8/README.md
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/kafi/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2411 2023-09-25 17:45:31.000000 kafi-0.0.8/kafi/addons.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4915 2023-09-18 16:27:40.000000 kafi-0.0.8/kafi/deserializer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2815 2023-09-25 17:12:03.000000 kafi-0.0.8/kafi/files.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/fs/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/kafi/fs/__init__.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/fs/azureblob/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:19.000000 kafi-0.0.8/kafi/fs/azureblob/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      765 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/fs/azureblob/azureblob.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3749 2023-09-18 16:27:40.000000 kafi-0.0.8/kafi/fs/azureblob/azureblob_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      261 2023-08-28 13:59:59.000000 kafi-0.0.8/kafi/fs/azureblob/azureblob_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      252 2023-08-28 14:00:09.000000 kafi-0.0.8/kafi/fs/azureblob/azureblob_producer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4866 2023-09-24 06:44:27.000000 kafi-0.0.8/kafi/fs/fs.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    17274 2023-09-25 17:20:26.000000 kafi-0.0.8/kafi/fs/fs_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     9171 2023-09-25 17:20:33.000000 kafi-0.0.8/kafi/fs/fs_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     5408 2023-09-25 17:20:39.000000 kafi-0.0.8/kafi/fs/fs_producer.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/fs/local/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:26.000000 kafi-0.0.8/kafi/fs/local/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      714 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/fs/local/local.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2478 2023-09-11 17:14:55.000000 kafi-0.0.8/kafi/fs/local/local_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      285 2023-08-28 13:58:36.000000 kafi-0.0.8/kafi/fs/local/local_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      243 2023-08-28 13:58:43.000000 kafi-0.0.8/kafi/fs/local/local_producer.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/fs/s3/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:24.000000 kafi-0.0.8/kafi/fs/s3/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      665 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/fs/s3/s3.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3145 2023-09-18 16:27:40.000000 kafi-0.0.8/kafi/fs/s3/s3_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      240 2023-08-28 14:01:40.000000 kafi-0.0.8/kafi/fs/s3/s3_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      231 2023-08-28 14:02:31.000000 kafi-0.0.8/kafi/fs/s3/s3_producer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    10827 2023-09-18 21:44:09.000000 kafi-0.0.8/kafi/functional.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     6252 2023-10-11 15:36:31.000000 kafi-0.0.8/kafi/helpers.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      218 2023-10-11 15:36:31.000000 kafi-0.0.8/kafi/kafi.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi/kafka/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/kafi/kafka/__init__.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.709226 kafi-0.0.8/kafi/kafka/cluster/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/kafi/kafka/cluster/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      816 2023-08-24 09:59:51.000000 kafi-0.0.8/kafi/kafka/cluster/cluster.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    33015 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/kafka/cluster/cluster_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4745 2023-09-21 09:45:44.000000 kafi-0.0.8/kafi/kafka/cluster/cluster_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2992 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/kafka/cluster/cluster_producer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     8529 2023-10-14 12:08:56.000000 kafi-0.0.8/kafi/kafka/kafka.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      168 2023-08-18 14:22:17.000000 kafi-0.0.8/kafi/kafka/kafka_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2382 2023-09-19 05:40:18.000000 kafi-0.0.8/kafi/kafka/kafka_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      285 2023-09-15 06:18:18.000000 kafi-0.0.8/kafi/kafka/kafka_producer.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.709226 kafi-0.0.8/kafi/kafka/restproxy/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/kafi/kafka/restproxy/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1868 2023-08-24 09:59:51.000000 kafi-0.0.8/kafi/kafka/restproxy/restproxy.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    23342 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/kafka/restproxy/restproxy_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     8810 2023-09-21 09:45:44.000000 kafi-0.0.8/kafi/kafka/restproxy/restproxy_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     6366 2023-09-24 06:15:46.000000 kafi-0.0.8/kafi/kafka/restproxy/restproxy_producer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1008 2023-09-24 06:22:04.000000 kafi-0.0.8/kafi/pandas.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     6108 2023-09-15 06:18:18.000000 kafi-0.0.8/kafi/schemaregistry.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     5334 2023-09-15 14:42:30.000000 kafi-0.0.8/kafi/serializer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4605 2023-09-15 06:32:20.000000 kafi-0.0.8/kafi/shell.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     9407 2023-09-24 07:57:51.000000 kafi-0.0.8/kafi/storage.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3609 2023-09-11 16:22:02.000000 kafi-0.0.8/kafi/storage_admin.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3692 2023-09-15 06:18:18.000000 kafi-0.0.8/kafi/storage_consumer.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     2371 2023-09-21 09:45:40.000000 kafi-0.0.8/kafi/storage_producer.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.705227 kafi-0.0.8/kafi.egg-info/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1172 2023-10-14 12:09:26.000000 kafi-0.0.8/kafi.egg-info/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1669 2023-10-14 12:09:26.000000 kafi-0.0.8/kafi.egg-info/SOURCES.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        1 2023-10-14 12:09:26.000000 kafi-0.0.8/kafi.egg-info/dependency_links.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      149 2023-10-14 12:09:26.000000 kafi-0.0.8/kafi.egg-info/requires.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       10 2023-10-14 12:09:26.000000 kafi-0.0.8/kafi.egg-info/top_level.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       38 2023-10-14 12:09:26.709226 kafi-0.0.8/setup.cfg
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1350 2023-10-14 12:07:05.000000 kafi-0.0.8/setup.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-14 12:09:26.709226 kafi-0.0.8/test/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.8/test/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    25123 2023-09-18 20:27:08.000000 kafi-0.0.8/test/test_cross_storage.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      718 2023-09-15 14:52:42.000000 kafi-0.0.8/test/test_fs_azureblob.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      723 2023-09-21 09:45:40.000000 kafi-0.0.8/test/test_fs_local.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      697 2023-09-15 14:55:53.000000 kafi-0.0.8/test/test_fs_s3.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      708 2023-09-25 17:42:46.000000 kafi-0.0.8/test/test_kafka_cluster.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1045 2023-09-15 14:42:30.000000 kafi-0.0.8/test/test_kafka_restproxy.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    44146 2023-09-25 17:43:34.000000 kafi-0.0.8/test/test_single_storage_base.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    11357 2023-08-16 21:54:10.000000 kafi-0.0.9/LICENSE
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1172 2023-10-17 20:59:26.229720 kafi-0.0.9/PKG-INFO
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      599 2023-09-23 17:45:27.000000 kafi-0.0.9/README.md
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.225720 kafi-0.0.9/kafi/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/kafi/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2411 2023-09-25 17:45:31.000000 kafi-0.0.9/kafi/addons.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     4915 2023-09-18 16:27:40.000000 kafi-0.0.9/kafi/deserializer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2815 2023-09-25 17:12:03.000000 kafi-0.0.9/kafi/files.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/fs/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/kafi/fs/__init__.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/fs/azureblob/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:19.000000 kafi-0.0.9/kafi/fs/azureblob/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      765 2023-09-21 09:45:40.000000 kafi-0.0.9/kafi/fs/azureblob/azureblob.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3749 2023-09-18 16:27:40.000000 kafi-0.0.9/kafi/fs/azureblob/azureblob_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      261 2023-08-28 13:59:59.000000 kafi-0.0.9/kafi/fs/azureblob/azureblob_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      252 2023-08-28 14:00:09.000000 kafi-0.0.9/kafi/fs/azureblob/azureblob_producer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2558 2023-10-16 19:51:58.000000 kafi-0.0.9/kafi/fs/fs.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    16826 2023-10-17 20:39:04.000000 kafi-0.0.9/kafi/fs/fs_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     9171 2023-09-25 17:20:33.000000 kafi-0.0.9/kafi/fs/fs_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     5408 2023-09-25 17:20:39.000000 kafi-0.0.9/kafi/fs/fs_producer.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/fs/local/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:26.000000 kafi-0.0.9/kafi/fs/local/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      714 2023-09-21 09:45:40.000000 kafi-0.0.9/kafi/fs/local/local.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2478 2023-09-11 17:14:55.000000 kafi-0.0.9/kafi/fs/local/local_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      285 2023-08-28 13:58:36.000000 kafi-0.0.9/kafi/fs/local/local_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      243 2023-08-28 13:58:43.000000 kafi-0.0.9/kafi/fs/local/local_producer.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/fs/s3/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-10-04 19:01:24.000000 kafi-0.0.9/kafi/fs/s3/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      665 2023-09-21 09:45:40.000000 kafi-0.0.9/kafi/fs/s3/s3.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3145 2023-09-18 16:27:40.000000 kafi-0.0.9/kafi/fs/s3/s3_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      240 2023-08-28 14:01:40.000000 kafi-0.0.9/kafi/fs/s3/s3_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      231 2023-08-28 14:02:31.000000 kafi-0.0.9/kafi/fs/s3/s3_producer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    10827 2023-09-18 21:44:09.000000 kafi-0.0.9/kafi/functional.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     6252 2023-10-11 15:36:31.000000 kafi-0.0.9/kafi/helpers.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      218 2023-10-11 15:36:31.000000 kafi-0.0.9/kafi/kafi.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/kafka/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/kafi/kafka/__init__.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/kafka/cluster/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/kafi/kafka/cluster/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      816 2023-08-24 09:59:51.000000 kafi-0.0.9/kafi/kafka/cluster/cluster.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    32343 2023-10-16 21:41:19.000000 kafi-0.0.9/kafi/kafka/cluster/cluster_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     4745 2023-09-21 09:45:44.000000 kafi-0.0.9/kafi/kafka/cluster/cluster_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2992 2023-09-21 09:45:40.000000 kafi-0.0.9/kafi/kafka/cluster/cluster_producer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     6027 2023-10-16 21:41:07.000000 kafi-0.0.9/kafi/kafka/kafka.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      168 2023-08-18 14:22:17.000000 kafi-0.0.9/kafi/kafka/kafka_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2382 2023-09-19 05:40:18.000000 kafi-0.0.9/kafi/kafka/kafka_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      285 2023-09-15 06:18:18.000000 kafi-0.0.9/kafi/kafka/kafka_producer.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/kafi/kafka/restproxy/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/kafi/kafka/restproxy/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1868 2023-08-24 09:59:51.000000 kafi-0.0.9/kafi/kafka/restproxy/restproxy.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    22801 2023-10-17 20:39:04.000000 kafi-0.0.9/kafi/kafka/restproxy/restproxy_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     8810 2023-09-21 09:45:44.000000 kafi-0.0.9/kafi/kafka/restproxy/restproxy_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     6366 2023-10-17 20:36:53.000000 kafi-0.0.9/kafi/kafka/restproxy/restproxy_producer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1008 2023-09-24 06:22:04.000000 kafi-0.0.9/kafi/pandas.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     6108 2023-09-15 06:18:18.000000 kafi-0.0.9/kafi/schemaregistry.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     5334 2023-09-15 14:42:30.000000 kafi-0.0.9/kafi/serializer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     4605 2023-09-15 06:32:20.000000 kafi-0.0.9/kafi/shell.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    11484 2023-10-17 20:39:04.000000 kafi-0.0.9/kafi/storage.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3609 2023-09-11 16:22:02.000000 kafi-0.0.9/kafi/storage_admin.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3692 2023-09-15 06:18:18.000000 kafi-0.0.9/kafi/storage_consumer.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     2371 2023-09-21 09:45:40.000000 kafi-0.0.9/kafi/storage_producer.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.225720 kafi-0.0.9/kafi.egg-info/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1172 2023-10-17 20:59:26.000000 kafi-0.0.9/kafi.egg-info/PKG-INFO
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1669 2023-10-17 20:59:26.000000 kafi-0.0.9/kafi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        1 2023-10-17 20:59:26.000000 kafi-0.0.9/kafi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      149 2023-10-17 20:59:26.000000 kafi-0.0.9/kafi.egg-info/requires.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       10 2023-10-17 20:59:26.000000 kafi-0.0.9/kafi.egg-info/top_level.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       38 2023-10-17 20:59:26.229720 kafi-0.0.9/setup.cfg
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1350 2023-10-17 20:39:10.000000 kafi-0.0.9/setup.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2023-10-17 20:59:26.229720 kafi-0.0.9/test/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2023-08-16 21:54:10.000000 kafi-0.0.9/test/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    25145 2023-10-17 20:57:37.000000 kafi-0.0.9/test/test_cross_storage.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      708 2023-10-17 20:39:04.000000 kafi-0.0.9/test/test_fs_azureblob.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      765 2023-10-17 20:39:04.000000 kafi-0.0.9/test/test_fs_local.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      687 2023-10-17 20:39:04.000000 kafi-0.0.9/test/test_fs_s3.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      708 2023-09-25 17:42:46.000000 kafi-0.0.9/test/test_kafka_cluster.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1087 2023-10-17 20:39:04.000000 kafi-0.0.9/test/test_kafka_restproxy.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    45155 2023-10-17 20:39:04.000000 kafi-0.0.9/test/test_single_storage_base.py
```

### Comparing `kafi-0.0.8/LICENSE` & `kafi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/PKG-INFO` & `kafi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kafka and Files
 Home-page: https://github.com/xdgrulez/kafi
 Author: Ralph M. Debusmann
 Author-email: matthias.debusmann@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kafi-0.0.8/README.md` & `kafi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/addons.py` & `kafi-0.0.9/kafi/addons.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/deserializer.py` & `kafi-0.0.9/kafi/deserializer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/files.py` & `kafi-0.0.9/kafi/files.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/azureblob/azureblob.py` & `kafi-0.0.9/kafi/fs/azureblob/azureblob.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/azureblob/azureblob_admin.py` & `kafi-0.0.9/kafi/fs/azureblob/azureblob_admin.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/fs_admin.py` & `kafi-0.0.9/kafi/fs/fs_admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,45 +33,35 @@
         #
         group_str_list = self.pattern_match(all_group_str_list, pattern)
         #
         return group_str_list
 
     #
 
-    def config(self, pattern):
-        topic_str_list = self.list_topics(pattern)
-        #
-        topic_str_config_dict_dict = {topic_str: self.get_config(topic_str) for topic_str in topic_str_list}
-        #
-        return topic_str_config_dict_dict
-
-    def set_config(self, pattern, config, **kwargs):
+    def config(self, pattern, config=None, **kwargs):
         config_dict = config
         #
         topic_str_list = self.list_topics(pattern)
         #
-        for topic_str in topic_str_list:
-            metadata_dict = self.get_metadata(topic_str)
-            metadata_dict["config"] = config_dict
-            self.set_metadata(topic_str, metadata_dict)
+        if config_dict is not None:
+            for topic_str in topic_str_list:
+                metadata_dict = self.get_metadata(topic_str)
+                metadata_dict["config"] = config_dict
+                self.set_metadata(topic_str, metadata_dict)
+        #
+        topic_str_config_dict_dict = {topic_str: self.get_config(topic_str) for topic_str in topic_str_list}
         #
-        topic_str_config_dict_dict = {topic_str: config_dict for topic_str in topic_str_list}
         return topic_str_config_dict_dict
 
     #
 
-    def exists(self, topic_or_file_str):
-        return self.list_topics(topic_or_file_str) != []
-
-    #
-
     def create(self, topic, partitions=1, config={}, **kwargs):
         topic_str = topic
         #
-        if self.exists(topic_str):
+        if self.list_topics(topic_str) != []:
             raise Exception(f"Topic \"{topic_str}\" already exists.")
         #
         config_dict = config
         partitions_int = partitions
         #
         metadata_dict = {"topic": topic_str, "partitions": partitions_int, "config": config_dict}
         self.set_metadata(topic_str, metadata_dict)
@@ -127,35 +117,31 @@
                         topic_str_partition_int_offsets_int_dict_dict[topic_str][partition_int] = message_dict["offset"]
                         break
         #
         return topic_str_partition_int_offsets_int_dict_dict
 
     #
 
-    def partitions(self, pattern=None, verbose=False):
-        topic_str_list = self.list_topics(pattern)
-        #
-        topic_str_partitions_int_dict = {topic_str: self.get_partitions(topic_str) for topic_str in topic_str_list}
-        #
-        return topic_str_partitions_int_dict
-
-    def set_partitions(self, pattern, num_partitions, **kwargs):
-        partitions_int = num_partitions
+    def partitions(self, pattern=None, partitions=None, verbose=False, **kwargs):
+        partitions_int = partitions
         #
         topic_str_list = self.list_topics(pattern)
         #
-        topic_str_partitions_int_dict = {}
-        for topic_str in topic_str_list:
-            metadata_dict = self.get_metadata(topic_str)
-            #
-            metadata_dict["partitions"] = partitions_int
-            #
-            self.set_metadata(topic_str, metadata_dict)
-            #
-            topic_str_partitions_int_dict[topic_str] = partitions_int
+        if partitions_int is not None:
+            topic_str_partitions_int_dict = {}
+            for topic_str in topic_str_list:
+                metadata_dict = self.get_metadata(topic_str)
+                #
+                metadata_dict["partitions"] = partitions_int
+                #
+                self.set_metadata(topic_str, metadata_dict)
+                #
+                topic_str_partitions_int_dict[topic_str] = partitions_int
+        #
+        topic_str_partitions_int_dict = {topic_str: self.get_partitions(topic_str) for topic_str in topic_str_list}
         #
         return topic_str_partitions_int_dict
 
     #
 
     def watermarks(self, pattern, **kwargs):
         topic_str_list = self.list_topics(pattern)
@@ -296,27 +282,25 @@
         if state_bool:
             group_str_state_str_dict = {group_str: state_str for group_str, state_str in group_str_state_str_tuple_list}
             return group_str_state_str_dict
         else:
             group_str_list = [group_str for group_str, _ in group_str_state_str_tuple_list]
             return group_str_list
 
-    def group_offsets(self, pattern, state_pattern="*"):
-        group_str_list = self.groups(pattern, state_pattern)
+    def group_offsets(self, pattern, group_offsets=None, state_pattern="*"):
+        topic_str_offsets_dict_dict = group_offsets
         #
-        group_str_topic_str_offsets_dict_dict_dict = {group_str: self.get_group_dict(group_str)["offsets"] for group_str in group_str_list}
+        group_str_list = self.groups(pattern, state_pattern)
         #
-        return group_str_topic_str_offsets_dict_dict_dict
-
-    def set_group_offsets(self, group_offsets):
-        group_str_topic_str_offsets_dict_dict_dict = group_offsets
+        if topic_str_offsets_dict_dict is not None:
+            for group_str in group_str_list:
+                new_group_dict = {"offsets": topic_str_offsets_dict_dict}
+                self.set_group_dict(group_str, new_group_dict)
         #
-        for group_str, topic_str_offsets_dict_dict in group_str_topic_str_offsets_dict_dict_dict.items():
-            new_group_dict = {"offsets": topic_str_offsets_dict_dict}
-            self.set_group_dict(group_str, new_group_dict)
+        group_str_topic_str_offsets_dict_dict_dict = {group_str: self.get_group_dict(group_str)["offsets"] for group_str in group_str_list}
         #
         return group_str_topic_str_offsets_dict_dict_dict
 
     # Metadata/Groups
 
     def read_dict_from_file(self, abs_path_file_str):
         if self.exists_file(abs_path_file_str):
```

### Comparing `kafi-0.0.8/kafi/fs/fs_consumer.py` & `kafi-0.0.9/kafi/fs/fs_consumer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/fs_producer.py` & `kafi-0.0.9/kafi/fs/fs_producer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/local/local.py` & `kafi-0.0.9/kafi/fs/local/local.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/local/local_admin.py` & `kafi-0.0.9/kafi/fs/local/local_admin.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/s3/s3.py` & `kafi-0.0.9/kafi/fs/s3/s3.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/fs/s3/s3_admin.py` & `kafi-0.0.9/kafi/fs/s3/s3_admin.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/functional.py` & `kafi-0.0.9/kafi/functional.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/helpers.py` & `kafi-0.0.9/kafi/helpers.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/cluster/cluster.py` & `kafi-0.0.9/kafi/kafka/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/cluster/cluster_admin.py` & `kafi-0.0.9/kafi/kafka/cluster/cluster_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,33 +66,27 @@
         else:
             pattern_str_list = [str(pattern_int_or_str) for pattern_int_or_str in pattern_int_or_str_list]
         #
         broker_dict = {broker_int: brokerMetadata.host + ":" + str(brokerMetadata.port) for broker_int, brokerMetadata in self.adminClient.list_topics().brokers.items() if any(fnmatch(str(broker_int), pattern_str) for pattern_str in pattern_str_list)}
         #
         return broker_dict
 
-    def broker_config(self, pattern=None):
-        broker_dict = self.brokers(pattern)
-        #
-        broker_int_broker_config_dict = {broker_int: self.get_resource_config_dict(ResourceType.BROKER, str(broker_int)) for broker_int in broker_dict}
-        #
-        return broker_int_broker_config_dict
-
-    def set_broker_config(self, config, pattern=None, **kwargs):
+    def broker_config(self, pattern=None, config=None, **kwargs):
         config_dict = config
         test_bool = kwargs["test"] if "test" in kwargs else False
         #
         broker_dict = self.brokers(pattern)
         #
-        for broker_int in broker_dict:
-            self.set_resource_config_dict(ResourceType.BROKER, str(broker_int), config_dict, test=test_bool)
+        if config is not None:
+            for broker_int in broker_dict:
+                self.set_resource_config_dict(ResourceType.BROKER, str(broker_int), config_dict, test=test_bool)
         #
-        broker_int_broker_config_dict_dict = {broker_int: config_dict for broker_int in broker_dict}
+        broker_int_broker_config_dict = {broker_int: self.get_resource_config_dict(ResourceType.BROKER, str(broker_int)) for broker_int in broker_dict}
         #
-        return broker_int_broker_config_dict_dict
+        return broker_int_broker_config_dict
 
     # Broker/Topic Configuration
 
     def get_resource_config_dict(self, resourceType, resource_str):
         configResource = ConfigResource(resourceType, resource_str)
         # configEntry_dict: ConfigResource -> ConfigEntry
         configEntry_dict = self.adminClient.describe_configs([configResource])[configResource].result()
@@ -162,33 +156,33 @@
         listConsumerGroupsResult = self.adminClient.list_consumer_groups(states=consumerGroupState_set).result()
         consumerGroupListing_list = listConsumerGroupsResult.valid
         #
         group_str_state_str_dict = {consumerGroupListing.group_id: consumerGroupState_to_str(consumerGroupListing.state) for consumerGroupListing in consumerGroupListing_list if any(fnmatch(consumerGroupListing.group_id, pattern_str) for pattern_str in pattern_str_or_str_list)}
         #
         return group_str_state_str_dict if state else list(group_str_state_str_dict.keys())
 
-    def group_offsets(self, pattern, state_pattern="*"):
-        pattern_str_or_str_list = pattern
-        #
-        group_str_list = self.groups(pattern_str_or_str_list, state_pattern)
-        if not group_str_list:
-            return {}
-        #
-        consumerGroupTopicPartitions_list = [_ConsumerGroupTopicPartitions(group_str) for group_str in group_str_list]
-        group_str_consumerGroupTopicPartitions_future_dict = self.adminClient.list_consumer_group_offsets(consumerGroupTopicPartitions_list)
-        #
-        group_offsets = group_str_consumerGroupTopicPartitions_future_dict_to_group_offsets(group_str_consumerGroupTopicPartitions_future_dict)
-        #
-        return group_offsets
-
-    def set_group_offsets(self, group_offsets):
-        consumerGroupTopicPartitions_list = group_offsets_to_consumerGroupTopicPartitions_list(group_offsets)
-        group_str_consumerGroupTopicPartitions_future_dict = self.adminClient.alter_consumer_group_offsets(consumerGroupTopicPartitions_list)
+    def group_offsets(self, pattern, group_offsets=None, state_pattern="*"):
+        group_offsets_dict = group_offsets
         #
-        group_offsets = group_str_consumerGroupTopicPartitions_future_dict_to_group_offsets(group_str_consumerGroupTopicPartitions_future_dict)
+        if group_offsets_dict is not None:
+            group_str = pattern
+            #
+            consumerGroupTopicPartitions = group_str_group_offsets_to_consumerGroupTopicPartitions(group_str, group_offsets)
+            group_str_consumerGroupTopicPartitions_future_dict = self.adminClient.alter_consumer_group_offsets([consumerGroupTopicPartitions])
+            #
+            group_offsets = group_str_consumerGroupTopicPartitions_future_dict_to_group_offsets(group_str_consumerGroupTopicPartitions_future_dict)
+        else:
+            group_str_list = self.groups(pattern, state_pattern)
+            if not group_str_list:
+                return {}
+            #
+            consumerGroupTopicPartitions_list = [_ConsumerGroupTopicPartitions(group_str) for group_str in group_str_list]
+            group_str_consumerGroupTopicPartitions_future_dict = self.adminClient.list_consumer_group_offsets(consumerGroupTopicPartitions_list)
+            #
+            group_offsets = group_str_consumerGroupTopicPartitions_future_dict_to_group_offsets(group_str_consumerGroupTopicPartitions_future_dict)
         #
         return group_offsets
 
     # Topics
 
     def block_topic(self, topic, exists=True):
         topic_str = topic
@@ -210,47 +204,40 @@
             if num_retries_int >= self.storage_obj.block_num_retries():
                 break
             time.sleep(self.storage_obj.block_interval())
         return False
 
     #
 
-    def config(self, pattern):
-        pattern_str_or_str_list = pattern
-        #
-        topic_str_list = self.list_topics(pattern_str_or_str_list)
-        #
-        topic_str_config_dict_dict = {topic_str: self.get_resource_config_dict(ResourceType.TOPIC, topic_str) for topic_str in topic_str_list}
-        #
-        return topic_str_config_dict_dict
-
-    def set_config(self, pattern, config, **kwargs):
-        pattern_str_or_str_list = pattern
+    def config(self, pattern, config=None, **kwargs):
         config_dict = config
         test_bool = kwargs["test"] if "test" in kwargs else False
         #
-        topic_str_list = self.list_topics(pattern_str_or_str_list)
+        topic_str_list = self.list_topics(pattern)
         #
-        for topic_str in topic_str_list:
-            self.set_resource_config_dict(ResourceType.TOPIC, topic_str, config_dict, test=test_bool)
+        if config is not None:
+            for topic_str in topic_str_list:
+                self.set_resource_config_dict(ResourceType.TOPIC, topic_str, config_dict, test=test_bool)
+        #
+        topic_str_config_dict_dict = {topic_str: self.get_resource_config_dict(ResourceType.TOPIC, topic_str) for topic_str in topic_str_list}
         #
-        topic_str_key_str_value_str_tuple_dict = {topic_str: config_dict for topic_str in topic_str_list}
-        return topic_str_key_str_value_str_tuple_dict
+        return topic_str_config_dict_dict
 
     #
 
-    def create(self, topic, partitions=1, config={}, **kwargs):
+    def create(self, topic, partitions=1, replication=-1, config={}, **kwargs):
         topic_str = topic
         partitions_int = partitions
+        replication_int = replication
         config_dict = config
         block_bool = kwargs["block"] if "block" in kwargs else True
         #
         config_dict["retention.ms"] = config_dict["retention.ms"] if "retention.ms" in config_dict else self.storage_obj.retention_ms()
         #
-        newTopic = NewTopic(topic_str, partitions_int, config=config_dict)
+        newTopic = NewTopic(topic_str, partitions_int, replication_factor=replication_int, config=config_dict)
         self.adminClient.create_topics([newTopic])
         #
         if block_bool:
             self.block_topic(topic_str, exists=True)
         #
         return topic_str
 
@@ -298,55 +285,50 @@
                 for topicPartition in topicPartition_list1:
                     offsets_dict[topicPartition.partition] = topicPartition.offset
                 #
                 topic_str_partition_int_offsets_int_dict_dict[topic_str] = offsets_dict
         #
         return topic_str_partition_int_offsets_int_dict_dict
 
-    def partitions(self, pattern=None, verbose=False):
+    def partitions(self, pattern=None, partitions=None, verbose=False, **kwargs):
         pattern_str_or_str_list = pattern
+        partitions_int = partitions
+        verbose_bool = verbose
+        test_bool = kwargs["test"] if "test" in kwargs else False
+        #
+        if partitions_int is not None:
+            topic_str_list = self.list_topics(pattern_str_or_str_list)
+            #
+            newPartitions_list = [NewPartitions(topic_str, partitions_int) for topic_str in topic_str_list]
+            topic_str_future_dict = self.adminClient.create_partitions(newPartitions_list, validate_only=test_bool)
+            #
+            for future in topic_str_future_dict.values():
+                future.result()
         #
         if pattern_str_or_str_list is None:
             pattern_str_or_str_list = ["*"]
         elif isinstance(pattern_str_or_str_list, str):
             pattern_str_or_str_list = [pattern_str_or_str_list]
         #
-        verbose_bool = verbose
-        #
         topic_str_topicMetadata_dict = self.adminClient.list_topics().topics
         #
         if verbose_bool:
             topic_str_topic_dict_dict = {topic_str: topicMetadata_to_topic_dict(topic_str_topicMetadata_dict[topic_str]) for topic_str in topic_str_topicMetadata_dict if any(fnmatch(topic_str, pattern_str) for pattern_str in pattern_str_or_str_list)}
             #
             topic_str_partition_int_partition_dict_dict_dict = {}
             for topic_str, topic_dict in topic_str_topic_dict_dict.items():
                 partitions_dict = topic_dict["partitions"]
                 topic_str_partition_int_partition_dict_dict_dict[topic_str] = partitions_dict
             #
             return topic_str_partition_int_partition_dict_dict_dict
         else:
             topic_str_partitions_int_dict = {topic_str: len(topic_str_topicMetadata_dict[topic_str].partitions) for topic_str in topic_str_topicMetadata_dict if any(fnmatch(topic_str, pattern_str) for pattern_str in pattern_str_or_str_list)}
+            #
             return topic_str_partitions_int_dict
 
-    def set_partitions(self, pattern, num_partitions, **kwargs):
-        pattern_str_or_str_list = pattern
-        partitions_int = num_partitions
-        test_bool = kwargs["test"] if "test" in kwargs else False
-        #
-        topic_str_list = self.list_topics(pattern_str_or_str_list)
-        #
-        newPartitions_list = [NewPartitions(topic_str, partitions_int) for topic_str in topic_str_list]
-        topic_str_future_dict = self.adminClient.create_partitions(newPartitions_list, validate_only=test_bool)
-        #
-        for future in topic_str_future_dict.values():
-            future.result()
-        #
-        topic_str_partitions_int_dict = {topic_str: partitions_int for topic_str in topic_str_list}
-        return topic_str_partitions_int_dict
-
     def watermarks(self, pattern, **kwargs):
         timeout_float = kwargs["timeout"] if "timeout" in kwargs else -1.0
         #
         config_dict = self.storage_obj.kafka_config_dict.copy()
         config_dict["group.id"] = "dummy_group_id"
         consumer = Consumer(config_dict)
         #
@@ -397,24 +379,23 @@
 def group_str_consumerGroupTopicPartitions_future_dict_to_group_offsets(group_str_consumerGroupTopicPartitions_future_dict):
     consumerGroupTopicPartitions_list = group_str_consumerGroupTopicPartitions_future_dict_to_consumerGroupTopicPartitions_list(group_str_consumerGroupTopicPartitions_future_dict)
     #
     group_offsets = consumerGroupTopicPartitions_list_to_group_offsets(consumerGroupTopicPartitions_list)
     #
     return group_offsets
 
-
-def group_offsets_to_consumerGroupTopicPartitions_list(group_offsets):
-    consumerGroupTopicPartitions_list = []
-    for group_str, topic_offsets in group_offsets.items():
-        topicPartition_list = []
-        for topic_str, partition_offsets in topic_offsets.items():
-            for partition_int, offset_int in partition_offsets.items():
-                topicPartition_list.append(TopicPartition(topic_str, partition_int, offset_int))
-        consumerGroupTopicPartitions_list.append(_ConsumerGroupTopicPartitions(group_str, topicPartition_list))
-    return consumerGroupTopicPartitions_list
+def group_str_group_offsets_to_consumerGroupTopicPartitions(group_str, group_offsets):
+    topicPartition_list = []
+    for topic_str, partition_offsets in group_offsets.items():
+        for partition_int, offset_int in partition_offsets.items():
+            topicPartition_list.append(TopicPartition(topic_str, partition_int, offset_int))
+    #
+    consumerGroupTopicPartitions = _ConsumerGroupTopicPartitions(group_str, topicPartition_list)
+    #
+    return consumerGroupTopicPartitions
 
 
 def consumerGroupDescription_to_group_description_dict(consumerGroupDescription):
     group_description_dict = {"group_id": consumerGroupDescription.group_id,
                               "is_simple_consumer_group": consumerGroupDescription.is_simple_consumer_group,
                               "members": [memberDescription_to_dict(memberDescription) for memberDescription in consumerGroupDescription.members],
                               "partition_assignor": consumerGroupDescription.partition_assignor,
```

### Comparing `kafi-0.0.8/kafi/kafka/cluster/cluster_consumer.py` & `kafi-0.0.9/kafi/kafka/cluster/cluster_consumer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/cluster/cluster_producer.py` & `kafi-0.0.9/kafi/kafka/cluster/cluster_producer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/kafka_consumer.py` & `kafi-0.0.9/kafi/kafka/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/restproxy/restproxy.py` & `kafi-0.0.9/kafi/kafka/restproxy/restproxy.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/restproxy/restproxy_admin.py` & `kafi-0.0.9/kafi/kafka/restproxy/restproxy_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,29 @@
         response_dict = get(url_str, headers_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
         kafkaBroker_dict_list = response_dict["data"]
         #
         broker_dict = {kafkaBroker_dict["broker_id"]: kafkaBroker_dict["host"] + ":" + str(kafkaBroker_dict["port"]) for kafkaBroker_dict in kafkaBroker_dict_list if any(fnmatch(str(kafkaBroker_dict["broker_id"]), pattern_str) for pattern_str in pattern_str_list)}
         #
         return broker_dict
 
-    def broker_config(self, pattern=None):
+    def broker_config(self, pattern=None, config=None, **kwargs):
+        config_dict = config
+        #
         broker_dict = self.brokers(pattern)
         #
         (rest_proxy_url_str, auth_str_tuple) = self.restproxy_obj.get_url_str_auth_str_tuple_tuple()
         #
+        if config_dict is not None:
+            url_str = f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/broker-configs:alter"
+            headers_dict = {"Content-Type": "application/json"}
+            #
+            dict_list = [{"name": key_str, "value": value_str} for key_str, value_str in config_dict.items()]
+            payload_dict = {"data": dict_list}
+            post(url_str, headers_dict, payload_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
+        #        
         url_str = f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/broker-configs"
         headers_dict = {"Content-Type": "application/json"}
         response_dict = get(url_str, headers_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
         kafkaClusterConfig_dict_list = response_dict["data"]
         #
         cluster_config_dict = {}
         for kafkaClusterConfig_dict in kafkaClusterConfig_dict_list:
@@ -107,31 +117,14 @@
             #
             cluster_config_dict[key_str] = value_str
         #
         broker_int_broker_config_dict = {broker_int: cluster_config_dict for broker_int in broker_dict}
         #
         return broker_int_broker_config_dict
 
-    def set_broker_config(self, config, pattern=None, **kwargs):
-        config_dict = config
-        broker_dict = self.brokers(pattern)
-        #
-        (rest_proxy_url_str, auth_str_tuple) = self.restproxy_obj.get_url_str_auth_str_tuple_tuple()
-        #
-        url_str = f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/broker-configs:alter"
-        headers_dict = {"Content-Type": "application/json"}
-        #
-        dict_list = [{"name": key_str, "value": value_str} for key_str, value_str in config_dict.items()]
-        payload_dict = {"data": dict_list}
-        post(url_str, headers_dict, payload_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
-        #
-        broker_int_broker_config_dict_dict = {broker_int: config_dict for broker_int in broker_dict}
-        #
-        return broker_int_broker_config_dict_dict
-
     # Groups
 
     def describe_groups(self, pattern="*", state_pattern="*"):
         pattern_str_list = [pattern] if isinstance(pattern, str) else pattern
         state_pattern_str_list = [state_pattern] if isinstance(pattern, str) else state_pattern
         #
         kafkaConsumerGroup_dict_list = self.get_kafkaConsumerGroup_dict_list(pattern_str_list)
@@ -167,15 +160,15 @@
         #
         kafkaConsumerGroup_dict_list = self.get_kafkaConsumerGroup_dict_list(pattern_str_list)
         #
         group_str_state_str_dict = {kafkaConsumerGroup_dict["consumer_group_id"]: kafkaConsumerGroup_dict["state"].lower() for kafkaConsumerGroup_dict in kafkaConsumerGroup_dict_list if any(fnmatch(kafkaConsumerGroup_dict["consumer_group_id"], pattern_str) for pattern_str in pattern_str_list) and any(fnmatch(kafkaConsumerGroup_dict["state"].lower(), state_pattern_str) for state_pattern_str in state_pattern_str_list)}
         #
         return group_str_state_str_dict if state_bool else list(group_str_state_str_dict.keys())
 
-    def group_offsets(self, pattern, state_pattern="*"):
+    def group_offsets(self, pattern, group_offsets=None, state_pattern="*"):
         pattern_str_list = [pattern] if isinstance(pattern, str) else pattern
         state_pattern_str_list = [state_pattern] if isinstance(pattern, str) else state_pattern
         #
         kafkaConsumerGroup_dict_list = self.get_kafkaConsumerGroup_dict_list(pattern_str_list)
         #
         group_str_list = [kafkaConsumerGroup_dict["consumer_group_id"] for kafkaConsumerGroup_dict in kafkaConsumerGroup_dict_list if any(fnmatch(kafkaConsumerGroup_dict["consumer_group_id"], pattern_str) for pattern_str in pattern_str_list) and any(fnmatch(kafkaConsumerGroup_dict["state"], state_pattern_str.upper()) for state_pattern_str in state_pattern_str_list)]
         #
@@ -207,18 +200,30 @@
             #
             group_offsets[group_str] = topic_str_offsets_dict_dict
         #
         return group_offsets
 
     # Topics
 
-    def config(self, pattern_str_or_str_list):
+    def config(self, pattern, config=None, **kwargs):
+        config_dict = config
+        #
         (rest_proxy_url_str, auth_str_tuple) = self.restproxy_obj.get_url_str_auth_str_tuple_tuple()
         #
-        topic_str_list = self.list_topics(pattern_str_or_str_list)
+        topic_str_list = self.list_topics(pattern)
+        #
+        if config_dict is not None:
+            for topic_str in topic_str_list:
+                url_str = f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/topics/{topic_str}/configs:alter"
+                headers_dict = {"Content-Type": "application/json"}
+                #
+                key_str_value_str_dict_list = [{"name": config_key_str, "value": config_value_str} for config_key_str, config_value_str in config_dict.items()]
+                payload_dict = {"data": key_str_value_str_dict_list}
+                #
+                post(url_str, headers_dict, payload_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
         #
         def kafkaTopicConfigList_dict_to_config_dict(kafkaTopicConfigList_dict):
             config_dict = {}
             #
             kafkaTopicConfig_dict_list = kafkaTopicConfigList_dict["data"]
             for kafkaTopicConfig_dict in kafkaTopicConfig_dict_list:
                 config_key_str = kafkaTopicConfig_dict["name"]
@@ -229,31 +234,14 @@
             return config_dict
 
         #
         topic_str_config_dict_dict = {topic_str: kafkaTopicConfigList_dict_to_config_dict(get(f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/topics/{topic_str}/configs", None, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())) for topic_str in topic_str_list}
         #
         return topic_str_config_dict_dict
     
-    def set_config(self, pattern_str_or_str_list, config_dict, **kwargs):
-        (rest_proxy_url_str, auth_str_tuple) = self.restproxy_obj.get_url_str_auth_str_tuple_tuple()
-        #
-        topic_str_list = self.list_topics(pattern_str_or_str_list)
-        #
-        topic_str_config_dict_dict = {}
-        for topic_str in topic_str_list:
-            url_str = f"{rest_proxy_url_str}/v3/clusters/{self.cluster_id_str}/topics/{topic_str}/configs:alter"
-            headers_dict = {"Content-Type": "application/json"}
-            key_str_value_str_dict_list = [{"name": config_key_str, "value": config_value_str} for config_key_str, config_value_str in config_dict.items()]
-            payload_dict = {"data": key_str_value_str_dict_list}
-            post(url_str, headers_dict, payload_dict, auth_str_tuple=auth_str_tuple, retries=self.restproxy_obj.requests_num_retries())
-            #
-            topic_str_config_dict_dict[topic_str] = config_dict
-        #
-        return topic_str_config_dict_dict
-
     #
 
     def create(self, topic_str, partitions=1, config={}, **kwargs):
         (rest_proxy_url_str, auth_str_tuple) = self.restproxy_obj.get_url_str_auth_str_tuple_tuple()
         #
         partitions_int = partitions
         config_dict = config
@@ -292,15 +280,15 @@
         kafkaTopic_dict_list = response_dict["data"]
         topic_str_list = [kafkaTopic_dict["topic_name"] for kafkaTopic_dict in kafkaTopic_dict_list]
         #
         filtered_topic_str_list = self.pattern_match(topic_str_list, pattern)
         #
         return filtered_topic_str_list
 
-    def partitions(self, pattern=None, verbose=False):
+    def partitions(self, pattern=None, partitions=None, verbose=False, **kwargs):
         pattern_str_or_str_list = pattern
         if pattern_str_or_str_list is None:
             pattern_str_or_str_list = ["*"]
         elif isinstance(pattern_str_or_str_list, str):
             pattern_str_or_str_list = [pattern_str_or_str_list]
         #
         verbose_bool = verbose
```

### Comparing `kafi-0.0.8/kafi/kafka/restproxy/restproxy_consumer.py` & `kafi-0.0.9/kafi/kafka/restproxy/restproxy_consumer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/kafka/restproxy/restproxy_producer.py` & `kafi-0.0.9/kafi/kafka/restproxy/restproxy_producer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/pandas.py` & `kafi-0.0.9/kafi/pandas.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/schemaregistry.py` & `kafi-0.0.9/kafi/schemaregistry.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/serializer.py` & `kafi-0.0.9/kafi/serializer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/shell.py` & `kafi-0.0.9/kafi/shell.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/storage_admin.py` & `kafi-0.0.9/kafi/storage_admin.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/storage_consumer.py` & `kafi-0.0.9/kafi/storage_consumer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi/storage_producer.py` & `kafi-0.0.9/kafi/storage_producer.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/kafi.egg-info/PKG-INFO` & `kafi-0.0.9/kafi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kafka and Files
 Home-page: https://github.com/xdgrulez/kafi
 Author: Ralph M. Debusmann
 Author-email: matthias.debusmann@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kafi-0.0.8/kafi.egg-info/SOURCES.txt` & `kafi-0.0.9/kafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/setup.py` & `kafi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='kafi',
-    version='0.0.8',
+    version='0.0.9',
     description='Kafka and Files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/xdgrulez/kafi',
     author='Ralph M. Debusmann',
     author_email='matthias.debusmann@gmail.com',
     license='Apache License 2.0',
```

### Comparing `kafi-0.0.8/test/test_cross_storage.py` & `kafi-0.0.9/test/test_cross_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
     w2.produce(test_obj.snack_ish_dict_list)
     w2.close()
     #
     group_str1 = test_obj.create_test_group_name(storage1)
     time.sleep(0.1)
     group_str2 = test_obj.create_test_group_name(storage2)
     #
-    (message_dict_message_dict_tuple_list, message_counter_int1, message_counter_int2) = storage1.diff(topic_str1, storage2, topic_str2, group1=group_str1, group2=group_str2, type1="json", type2="json", n=3)
+    (message_dict_message_dict_tuple_list, message_counter_int1, message_counter_int2) = storage1.diff(topic_str1, storage2, topic_str2, group1=group_str1, group2=group_str2, type1="json", type2="json", n=3, consume_batch_size=3)
     test_obj.assertEqual(3, len(message_dict_message_dict_tuple_list))
     test_obj.assertEqual(3, message_counter_int1)
     test_obj.assertEqual(3, message_counter_int2)
 
 # Files
 
 def test_from_to_file(test_obj, storage1, storage2):
```

### Comparing `kafi-0.0.8/test/test_fs_azureblob.py` & `kafi-0.0.9/test/test_fs_local.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 
 if os.path.basename(os.getcwd()) == "test":
     sys.path.insert(1, "..")
 else:
     sys.path.insert(1, ".")
 
 from test.test_single_storage_base import TestSingleStorageBase
-from kafi.fs.azureblob.azureblob import AzureBlob
+from kafi.fs.local.local import Local
 
 #
 
 class Test(TestSingleStorageBase):
     def setUp(self):
         super().setUp()
-        self.path_str = "test"
+        self.path_str = "/tmp/kafi/test/local"
+        os.makedirs(self.path_str, exist_ok=True)
 
     def tearDown(self):
         super().tearDown()
 
     #
 
     def get_storage(self):
-        a = AzureBlob("local")
-        a.root_dir(self.path_str)
+        l = Local("local")
+        l.root_dir(self.path_str)
         #
-        return a
+        return l
 
     def is_ccloud(self):
         return False
 
+    #
+
     def test_acls(self):
         pass
 
     def test_brokers(self):
         pass
 
-    def test_offsets_for_times(self):
+    def test_compact(self):
         pass
```

### Comparing `kafi-0.0.8/test/test_fs_local.py` & `kafi-0.0.9/test/test_fs_s3.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 
 if os.path.basename(os.getcwd()) == "test":
     sys.path.insert(1, "..")
 else:
     sys.path.insert(1, ".")
 
 from test.test_single_storage_base import TestSingleStorageBase
-from kafi.fs.local.local import Local
+from kafi.fs.s3.s3 import S3
 
 #
 
 class Test(TestSingleStorageBase):
     def setUp(self):
         super().setUp()
-        self.path_str = "/tmp/kafi/test/local"
-        os.makedirs(self.path_str, exist_ok=True)
+        self.path_str = "test"
 
     def tearDown(self):
         super().tearDown()
 
     #
 
     def get_storage(self):
-        l = Local("local")
-        l.root_dir(self.path_str)
+        s = S3("local")
+        s.root_dir(self.path_str)
         #
-        return l
+        return s
 
     def is_ccloud(self):
         return False
 
     #
 
     def test_acls(self):
         pass
 
     def test_brokers(self):
         pass
+
+    def test_compact(self):
+        pass
```

### Comparing `kafi-0.0.8/test/test_fs_s3.py` & `kafi-0.0.9/test/test_kafka_restproxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,53 @@
 
 if os.path.basename(os.getcwd()) == "test":
     sys.path.insert(1, "..")
 else:
     sys.path.insert(1, ".")
 
 from test.test_single_storage_base import TestSingleStorageBase
-from kafi.fs.s3.s3 import S3
-
-#
+from kafi.kafka.restproxy.restproxy import RestProxy
+from kafi.kafka.cluster.cluster import Cluster
 
 class Test(TestSingleStorageBase):
     def setUp(self):
         super().setUp()
-        self.path_str = "test"
+        self.principal_str = None
+
 
     def tearDown(self):
         super().tearDown()
 
     #
 
     def get_storage(self):
-        s = S3("local")
-        s.root_dir(self.path_str)
+        r = RestProxy("local")
+        #
+        return r
+
+    def get_cluster(self):
+        c = Cluster("local")
         #
-        return s
+        return c
 
     def is_ccloud(self):
-        return False
+        r = self.get_storage()
+        #
+        return "confluent.cloud" in r.rest_proxy_config_dict["rest.proxy.url"]
+    
+    def test_delete_groups(self):
+        pass
 
-    #
+    def test_set_group_offsets(self):
+        pass
+
+    def test_offsets_for_times(self):
+        pass
 
-    def test_acls(self):
+    def test_consume_from_offsets(self):
         pass
 
-    def test_brokers(self):
+    def test_error_handling(self):
         pass
 
-    def test_offsets_for_times(self):
+    def test_compact(self):
         pass
```

### Comparing `kafi-0.0.8/test/test_kafka_cluster.py` & `kafi-0.0.9/test/test_kafka_cluster.py`

 * *Files identical despite different names*

### Comparing `kafi-0.0.8/test/test_single_storage_base.py` & `kafi-0.0.9/test/test_single_storage_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,19 +120,19 @@
             broker_dict2 = s.brokers([broker_int])
             self.assertEqual(broker_dict1, broker_dict2)
             old_broker_config_dict = s.broker_config(broker_int)[broker_int]
             if "background.threads" in old_broker_config_dict:
                 old_background_threads_str = old_broker_config_dict["background.threads"]
             else:
                 old_background_threads_str = 10
-            s.set_broker_config({"background.threads": 5}, broker_int)
+            s.broker_config(broker_int, {"background.threads": 5})
             time.sleep(0.5)
             new_background_threads_str = s.broker_config(broker_int)[broker_int]["background.threads"]
             self.assertEqual(new_background_threads_str, "5")
-            s.set_broker_config({"background.threads": old_background_threads_str}, broker_int)
+            s.broker_config(broker_int, {"background.threads": old_background_threads_str})
 
     # Groups
 
     def test_groups(self):
         if self.__class__.__name__ == "TestSingleStorageBase":
             return
         #
@@ -281,15 +281,15 @@
         producer.produce("message 1")
         producer.produce("message 2")
         producer.produce("message 3")
         producer.close()
         #
         group_str = self.create_test_group_name()
         consumer = s.consumer(topic_str, group=group_str, type="str")
-        group_str_topic_str_offsets_dict_dict_dict = s.set_group_offsets({group_str: {topic_str: {0: 2}}})
+        group_str_topic_str_offsets_dict_dict_dict = s.group_offsets(group_str, {topic_str: {0: 2}})
         self.assertEqual(group_str_topic_str_offsets_dict_dict_dict, {group_str: {topic_str: {0: 2}}})
         [message_dict] = consumer.consume(n=1)
         consumer.commit()
         self.assertEqual(message_dict["value"], "message 3")
         #
         consumer.close()
 
@@ -300,15 +300,15 @@
             return
         #
         s = self.get_storage()
         #
         topic_str = self.create_test_topic_name()
         s.touch(topic_str)
         #
-        s.set_config(topic_str, {"retention.ms": "4711"})
+        s.config(topic_str, {"retention.ms": "4711"})
         new_retention_ms_str = s.config(topic_str)[topic_str]["retention.ms"]
         self.assertEqual(new_retention_ms_str, "4711")
 
     def test_create_delete(self):
         if self.__class__.__name__ == "TestSingleStorageBase":
             return
         #
@@ -391,15 +391,15 @@
         #
         if s.__class__.__name__ == "RestProxy":
             s.create(topic_str, partitions=2)
         else:
             s.create(topic_str)
             partitions_int_1 = s.partitions(topic_str)[topic_str]
             self.assertEqual(partitions_int_1, 1)
-            s.set_partitions(topic_str, 2)
+            s.partitions(topic_str, 2)
         #
         partitions_int_2 = s.partitions(topic_str)[topic_str]
         self.assertEqual(partitions_int_2, 2)
         if s.__class__.__name__ in ["Cluster", "RestProxy"]:
             topic_str_partition_int_partition_dict_dict_dict = s.partitions(topic_str, verbose=True)[topic_str]
             self.assertEqual(list(topic_str_partition_int_partition_dict_dict_dict.keys()), [0, 1])
             self.assertEqual(topic_str_partition_int_partition_dict_dict_dict[0]["leader"], 1)
@@ -647,14 +647,42 @@
         group_str2 = self.create_test_group_name()
         (message_dict_list, n_int1) = s.cat(topic_str1, group=group_str2, value_type="str", n=3)
         self.assertEqual(3, len(message_dict_list))
         self.assertEqual(3, n_int1)
         value_str_list = [message_dict["value"] for message_dict in message_dict_list]
         self.assertEqual(value_str_list, self.snack_str_list)
 
+    def test_compact(self):
+        if self.__class__.__name__ == "TestSingleStorageBase":
+            return
+        #
+        if not self.is_ccloud():
+            s = self.get_storage()
+            #
+            topic_str = self.create_test_topic_name()
+            s.create(topic_str, config={"cleanup.policy": "compact", "max.compaction.lag.ms": 100, "min.cleanable.dirty.ratio": 0.0000000001, "segment.ms": 100, "delete.retention.ms": 100})
+            #
+            pr = s.producer(topic_str)
+            for i in range(0, 100):
+                if i % 2 == 0:
+                    pr.produce(i, key="even")
+                else:
+                    pr.produce(i, key="odd")
+            pr.flush()
+            #
+            (n_int1, _, _) = s.wc(topic_str)
+            self.assertEqual(n_int1, 100)
+            pr.produce(100, key="even")
+            time.sleep(6)
+            pr.produce(101, key="odd")
+            pr.close()
+            #
+            (n_int2, _, _) = s.wc(topic_str)
+            self.assertEqual(n_int2, 4)
+
     def test_cluster_settings(self):
         if self.__class__.__name__ == "TestSingleStorageBase":
             return
         #
         s = self.get_storage()
         #
         s.verbose(0)
```

