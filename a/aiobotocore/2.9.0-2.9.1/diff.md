# Comparing `tmp/aiobotocore-2.9.0.tar.gz` & `tmp/aiobotocore-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobotocore-2.9.0.tar", last modified: Wed Dec 13 07:26:05 2023, max compression
+gzip compressed data, was "aiobotocore-2.9.1.tar", last modified: Wed Jan 17 22:35:10 2024, max compression
```

## Comparing `aiobotocore-2.9.0.tar` & `aiobotocore-2.9.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 07:26:05.380291 aiobotocore-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20779 2023-12-13 07:26:05.380291 aiobotocore-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 07:26:05.376291 aiobotocore-2.9.0/aiobotocore/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/_endpoint_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24006 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    39258 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/httpsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 07:26:05.376291 aiobotocore-2.9.0/aiobotocore/retries/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/retries/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/retries/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/retries/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/retries/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14592 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/aiobotocore/waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 07:26:05.380291 aiobotocore-2.9.0/aiobotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20779 2023-12-13 07:26:05.000000 aiobotocore-2.9.0/aiobotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-12-13 07:26:05.000000 aiobotocore-2.9.0/aiobotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 07:26:05.000000 aiobotocore-2.9.0/aiobotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-13 07:26:05.000000 aiobotocore-2.9.0/aiobotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 07:26:05.000000 aiobotocore-2.9.0/aiobotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-13 07:26:05.380291 aiobotocore-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 07:26:05.380291 aiobotocore-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21758 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_basic_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_eventstreams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (127)    26737 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_sns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_stubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-13 07:26:01.000000 aiobotocore-2.9.0/tests/test_waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 22:35:10.513674 aiobotocore-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-01-17 22:35:10.513674 aiobotocore-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 22:35:10.509674 aiobotocore-2.9.1/aiobotocore/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/_endpoint_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24006 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39258 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/httpsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 22:35:10.509674 aiobotocore-2.9.1/aiobotocore/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/retries/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/retries/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/retries/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/retries/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14592 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27333 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/aiobotocore/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 22:35:10.513674 aiobotocore-2.9.1/aiobotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-01-17 22:35:10.000000 aiobotocore-2.9.1/aiobotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-01-17 22:35:10.000000 aiobotocore-2.9.1/aiobotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 22:35:10.000000 aiobotocore-2.9.1/aiobotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-17 22:35:10.000000 aiobotocore-2.9.1/aiobotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-17 22:35:10.000000 aiobotocore-2.9.1/aiobotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-17 22:35:10.517674 aiobotocore-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 22:35:10.513674 aiobotocore-2.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21758 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_basic_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_eventstreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26737 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_stubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-17 22:35:06.000000 aiobotocore-2.9.1/tests/test_waiter.py
```

### Comparing `aiobotocore-2.9.0/CHANGES.rst` & `aiobotocore-2.9.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 -------
 
+2.9.1 (2024-01-17)
+^^^^^^^^^^^^^^^^^^
+* fix race condition in S3 Express identity cache #1072
+
 2.9.0 (2023-12-12)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore dependency specification
 
 2.8.0 (2023-11-28)
 ^^^^^^^^^^^^^^^^^^
 * add AioStubber that returns AioAWSResponse()
```

### Comparing `aiobotocore-2.9.0/LICENSE` & `aiobotocore-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/PKG-INFO` & `aiobotocore-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobotocore
-Version: 2.9.0
+Version: 2.9.1
 Summary: Async client for aws services using botocore and aiohttp
 Home-page: https://github.com/aio-libs/aiobotocore
 Download-URL: https://pypi.python.org/pypi/aiobotocore
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
@@ -285,14 +285,18 @@
 
 If you only need awscli and not boto3 (or vice versa) you can just install one extra or
 the other.
 
 Changes
 -------
 
+2.9.1 (2024-01-17)
+^^^^^^^^^^^^^^^^^^
+* fix race condition in S3 Express identity cache #1072
+
 2.9.0 (2023-12-12)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore dependency specification
 
 2.8.0 (2023-11-28)
 ^^^^^^^^^^^^^^^^^^
 * add AioStubber that returns AioAWSResponse()
```

### Comparing `aiobotocore-2.9.0/README.rst` & `aiobotocore-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/_endpoint_helpers.py` & `aiobotocore-2.9.1/aiobotocore/_endpoint_helpers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/args.py` & `aiobotocore-2.9.1/aiobotocore/args.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/awsrequest.py` & `aiobotocore-2.9.1/aiobotocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/client.py` & `aiobotocore-2.9.1/aiobotocore/client.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/config.py` & `aiobotocore-2.9.1/aiobotocore/config.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/configprovider.py` & `aiobotocore-2.9.1/aiobotocore/configprovider.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/credentials.py` & `aiobotocore-2.9.1/aiobotocore/credentials.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/discovery.py` & `aiobotocore-2.9.1/aiobotocore/discovery.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/endpoint.py` & `aiobotocore-2.9.1/aiobotocore/endpoint.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/eventstream.py` & `aiobotocore-2.9.1/aiobotocore/eventstream.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/handlers.py` & `aiobotocore-2.9.1/aiobotocore/handlers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/hooks.py` & `aiobotocore-2.9.1/aiobotocore/hooks.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/httpchecksum.py` & `aiobotocore-2.9.1/aiobotocore/httpchecksum.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/httpsession.py` & `aiobotocore-2.9.1/aiobotocore/httpsession.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/paginate.py` & `aiobotocore-2.9.1/aiobotocore/paginate.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/parsers.py` & `aiobotocore-2.9.1/aiobotocore/parsers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/regions.py` & `aiobotocore-2.9.1/aiobotocore/regions.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/response.py` & `aiobotocore-2.9.1/aiobotocore/response.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/retries/adaptive.py` & `aiobotocore-2.9.1/aiobotocore/retries/adaptive.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/retries/bucket.py` & `aiobotocore-2.9.1/aiobotocore/retries/bucket.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/retries/special.py` & `aiobotocore-2.9.1/aiobotocore/retries/special.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/retries/standard.py` & `aiobotocore-2.9.1/aiobotocore/retries/standard.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/retryhandler.py` & `aiobotocore-2.9.1/aiobotocore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/session.py` & `aiobotocore-2.9.1/aiobotocore/session.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/signers.py` & `aiobotocore-2.9.1/aiobotocore/signers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/stub.py` & `aiobotocore-2.9.1/aiobotocore/stub.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/tokens.py` & `aiobotocore-2.9.1/aiobotocore/tokens.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore/utils.py` & `aiobotocore-2.9.1/aiobotocore/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -363,38 +363,24 @@
             advisory_timeout=45,
             mandatory_timeout=10,
         )
         return credential_entry
 
 
 class AioS3ExpressIdentityCache(AioIdentityCache, S3ExpressIdentityCache):
-    @functools.cached_property
-    def _aio_credential_cache(self):
-        """Substitutes upstream credential cache."""
-        return {}
+    @functools.lru_cache(maxsize=100)
+    def _get_credentials(self, bucket):
+        return asyncio.create_task(super().get_credentials(bucket=bucket))
 
     async def get_credentials(self, bucket):
         # upstream uses `@functools.lru_cache(maxsize=100)` to cache credentials.
         # This is incompatible with async code.
         # We need to implement custom caching logic.
 
-        if (credentials := self._aio_credential_cache.get(bucket)) is None:
-            # cache miss -> get credentials asynchronously
-            credentials = await super().get_credentials(bucket=bucket)
-
-            # upstream cache is bounded at 100 entries
-            if len(self._aio_credential_cache) >= 100:
-                # drop oldest entry from cache (deviates from lru_cache logic)
-                self._aio_credential_cache.pop(
-                    next(iter(self._aio_credential_cache)),
-                )
-
-            self._aio_credential_cache[bucket] = credentials
-
-        return credentials
+        return await self._get_credentials(bucket=bucket)
 
     def build_refresh_callback(self, bucket):
         async def refresher():
             response = await self._client.create_session(Bucket=bucket)
             creds = response['Credentials']
             expiration = self._serialize_if_needed(
                 creds['Expiration'], iso=True
```

### Comparing `aiobotocore-2.9.0/aiobotocore/waiter.py` & `aiobotocore-2.9.1/aiobotocore/waiter.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/aiobotocore.egg-info/PKG-INFO` & `aiobotocore-2.9.1/aiobotocore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobotocore
-Version: 2.9.0
+Version: 2.9.1
 Summary: Async client for aws services using botocore and aiohttp
 Home-page: https://github.com/aio-libs/aiobotocore
 Download-URL: https://pypi.python.org/pypi/aiobotocore
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
@@ -285,14 +285,18 @@
 
 If you only need awscli and not boto3 (or vice versa) you can just install one extra or
 the other.
 
 Changes
 -------
 
+2.9.1 (2024-01-17)
+^^^^^^^^^^^^^^^^^^
+* fix race condition in S3 Express identity cache #1072
+
 2.9.0 (2023-12-12)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore dependency specification
 
 2.8.0 (2023-11-28)
 ^^^^^^^^^^^^^^^^^^
 * add AioStubber that returns AioAWSResponse()
```

### Comparing `aiobotocore-2.9.0/aiobotocore.egg-info/SOURCES.txt` & `aiobotocore-2.9.1/aiobotocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/setup.py` & `aiobotocore-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_adaptive.py` & `aiobotocore-2.9.1/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_basic_s3.py` & `aiobotocore-2.9.1/tests/test_basic_s3.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_config.py` & `aiobotocore-2.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_dynamodb.py` & `aiobotocore-2.9.1/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_ec2.py` & `aiobotocore-2.9.1/tests/test_ec2.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_eventstreams.py` & `aiobotocore-2.9.1/tests/test_eventstreams.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_lambda.py` & `aiobotocore-2.9.1/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_monitor.py` & `aiobotocore-2.9.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_mturk.py` & `aiobotocore-2.9.1/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_patches.py` & `aiobotocore-2.9.1/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_response.py` & `aiobotocore-2.9.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_session.py` & `aiobotocore-2.9.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_sns.py` & `aiobotocore-2.9.1/tests/test_sns.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_sqs.py` & `aiobotocore-2.9.1/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_stubber.py` & `aiobotocore-2.9.1/tests/test_stubber.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_version.py` & `aiobotocore-2.9.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.9.0/tests/test_waiter.py` & `aiobotocore-2.9.1/tests/test_waiter.py`

 * *Files identical despite different names*

