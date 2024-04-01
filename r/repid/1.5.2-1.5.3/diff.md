# Comparing `tmp/repid-1.5.2.tar.gz` & `tmp/repid-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.5.2.tar", last modified: Wed Mar  6 20:45:55 2024, max compression
+gzip compressed data, was "repid-1.5.3.tar", last modified: Mon Apr  1 23:29:47 2024, max compression
```

## Comparing `repid-1.5.2.tar` & `repid-1.5.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1089 2024-03-06 20:45:38.557012 repid-1.5.2/LICENSE
--rw-r--r--   0        0        0     2604 2024-03-06 20:45:38.557012 repid-1.5.2/README.md
--rw-r--r--   0        0        0     4379 2024-03-06 20:45:55.021151 repid-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1397 2024-03-06 20:45:38.561012 repid-1.5.2/repid/__init__.py
--rw-r--r--   0        0        0     1544 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_asyncify.py
--rw-r--r--   0        0        0     7835 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_processor.py
--rw-r--r--   0        0        0     4656 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_runner.py
--rw-r--r--   0        0        0      551 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/__init__.py
--rw-r--r--   0        0        0      501 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/args_bucket_in_message_id.py
--rw-r--r--   0        0        0      272 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/dataclass_hacks.py
--rw-r--r--   0        0        0      834 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/get_dependency.py
--rw-r--r--   0        0        0      432 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/internal_exceptions.py
--rw-r--r--   0        0        0     1268 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/is_installed.py
--rw-r--r--   0        0        0     1012 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/json_encoder.py
--rw-r--r--   0        0        0      135 2024-03-06 20:45:38.561012 repid-1.5.2/repid/_utils/regex_validators.py
--rw-r--r--   0        0        0      536 2024-03-06 20:45:38.561012 repid-1.5.2/repid/actor.py
--rw-r--r--   0        0        0     2499 2024-03-06 20:45:38.561012 repid-1.5.2/repid/config.py
--rw-r--r--   0        0        0     4493 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connection.py
--rw-r--r--   0        0        0      736 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/__init__.py
--rw-r--r--   0        0        0     6765 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     3856 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      859 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     8826 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7289 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      803 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0     1809 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1544 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0    11878 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     8025 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     4107 2024-03-06 20:45:38.561012 repid-1.5.2/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     8405 2024-03-06 20:45:38.561012 repid-1.5.2/repid/converter.py
--rw-r--r--   0        0        0      355 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/__init__.py
--rw-r--r--   0        0        0     2268 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/_buckets.py
--rw-r--r--   0        0        0      820 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/_key.py
--rw-r--r--   0        0        0     5504 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/priorities.py
--rw-r--r--   0        0        0     3733 2024-03-06 20:45:38.561012 repid-1.5.2/repid/data/protocols.py
--rw-r--r--   0        0        0      282 2024-03-06 20:45:38.561012 repid-1.5.2/repid/dependencies/__init__.py
--rw-r--r--   0        0        0     3171 2024-03-06 20:45:38.561012 repid-1.5.2/repid/dependencies/depends.py
--rw-r--r--   0        0        0     7327 2024-03-06 20:45:38.561012 repid-1.5.2/repid/dependencies/message_dependency.py
--rw-r--r--   0        0        0      866 2024-03-06 20:45:38.561012 repid-1.5.2/repid/dependencies/protocols.py
--rw-r--r--   0        0        0      587 2024-03-06 20:45:38.561012 repid-1.5.2/repid/dependencies/resolver_context.py
--rw-r--r--   0        0        0     3421 2024-03-06 20:45:38.561012 repid-1.5.2/repid/health_check_server.py
--rw-r--r--   0        0        0     7478 2024-03-06 20:45:38.561012 repid-1.5.2/repid/job.py
--rw-r--r--   0        0        0      546 2024-03-06 20:45:38.561012 repid-1.5.2/repid/logger.py
--rw-r--r--   0        0        0     1887 2024-03-06 20:45:38.561012 repid-1.5.2/repid/main.py
--rw-r--r--   0        0        0     3791 2024-03-06 20:45:38.565012 repid-1.5.2/repid/message.py
--rw-r--r--   0        0        0      257 2024-03-06 20:45:38.565012 repid-1.5.2/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2024-03-06 20:45:38.565012 repid-1.5.2/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3685 2024-03-06 20:45:38.565012 repid-1.5.2/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3639 2024-03-06 20:45:38.565012 repid-1.5.2/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2024-03-06 20:45:38.565012 repid-1.5.2/repid/py.typed
--rw-r--r--   0        0        0     1930 2024-03-06 20:45:38.565012 repid-1.5.2/repid/queue.py
--rw-r--r--   0        0        0     1319 2024-03-06 20:45:38.565012 repid-1.5.2/repid/retry_policy.py
--rw-r--r--   0        0        0     5006 2024-03-06 20:45:38.565012 repid-1.5.2/repid/router.py
--rw-r--r--   0        0        0      512 2024-03-06 20:45:38.565012 repid-1.5.2/repid/serializer.py
--rw-r--r--   0        0        0      781 2024-03-06 20:45:38.565012 repid-1.5.2/repid/testing/__init__.py
--rw-r--r--   0        0        0     3147 2024-03-06 20:45:38.565012 repid-1.5.2/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6163 2024-03-06 20:45:38.565012 repid-1.5.2/repid/testing/plugin.py
--rw-r--r--   0        0        0     4720 2024-03-06 20:45:38.565012 repid-1.5.2/repid/worker.py
--rw-r--r--   0        0        0        0 2024-03-06 20:45:38.565012 repid-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0     1145 2024-03-06 20:45:38.565012 repid-1.5.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4678 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_consumer_different_categories.py
--rw-r--r--   0        0        0     4005 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0     1402 2024-03-06 20:45:38.565012 repid-1.5.2/tests/integration/test_rabbitmq_specific.py
--rw-r--r--   0        0        0      431 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_actor.py
--rw-r--r--   0        0        0     4608 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_config.py
--rw-r--r--   0        0        0     2986 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_connection.py
--rw-r--r--   0        0        0     3834 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10230 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_default_data_models.py
--rw-r--r--   0        0        0    13979 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_dependencies.py
--rw-r--r--   0        0        0     2110 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_health_check_server.py
--rw-r--r--   0        0        0     3004 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_job.py
--rw-r--r--   0        0        0     2298 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_json.py
--rw-r--r--   0        0        0     1366 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_main.py
--rw-r--r--   0        0        0     5627 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_message.py
--rw-r--r--   0        0        0     7842 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     7360 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_queue.py
--rw-r--r--   0        0        0     3180 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_router.py
--rw-r--r--   0        0        0     3673 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_runner.py
--rw-r--r--   0        0        0      762 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_serializer.py
--rw-r--r--   0        0        0     1893 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_utils.py
--rw-r--r--   0        0        0     8346 2024-03-06 20:45:38.565012 repid-1.5.2/tests/test_worker.py
--rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 repid-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-01 23:29:30.139399 repid-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2604 2024-04-01 23:29:30.139399 repid-1.5.3/README.md
+-rw-r--r--   0        0        0     4379 2024-04-01 23:29:47.795714 repid-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1397 2024-04-01 23:29:30.143399 repid-1.5.3/repid/__init__.py
+-rw-r--r--   0        0        0     1544 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_asyncify.py
+-rw-r--r--   0        0        0     8009 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_processor.py
+-rw-r--r--   0        0        0     5664 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_runner.py
+-rw-r--r--   0        0        0      551 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0      834 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/get_dependency.py
+-rw-r--r--   0        0        0      432 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/internal_exceptions.py
+-rw-r--r--   0        0        0     1268 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0     1012 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2024-04-01 23:29:30.143399 repid-1.5.3/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      536 2024-04-01 23:29:30.143399 repid-1.5.3/repid/actor.py
+-rw-r--r--   0        0        0     2499 2024-04-01 23:29:30.143399 repid-1.5.3/repid/config.py
+-rw-r--r--   0        0        0     4493 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connection.py
+-rw-r--r--   0        0        0      736 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6765 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     3856 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      859 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     8826 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7289 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      803 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0     1809 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1544 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0    11878 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     8025 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     4107 2024-04-01 23:29:30.143399 repid-1.5.3/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     8405 2024-04-01 23:29:30.143399 repid-1.5.3/repid/converter.py
+-rw-r--r--   0        0        0      355 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/__init__.py
+-rw-r--r--   0        0        0     2268 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_key.py
+-rw-r--r--   0        0        0     5504 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/priorities.py
+-rw-r--r--   0        0        0     3733 2024-04-01 23:29:30.143399 repid-1.5.3/repid/data/protocols.py
+-rw-r--r--   0        0        0      282 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/__init__.py
+-rw-r--r--   0        0        0     3171 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/depends.py
+-rw-r--r--   0        0        0     7327 2024-04-01 23:29:30.143399 repid-1.5.3/repid/dependencies/message_dependency.py
+-rw-r--r--   0        0        0      866 2024-04-01 23:29:30.147399 repid-1.5.3/repid/dependencies/protocols.py
+-rw-r--r--   0        0        0      587 2024-04-01 23:29:30.147399 repid-1.5.3/repid/dependencies/resolver_context.py
+-rw-r--r--   0        0        0     3421 2024-04-01 23:29:30.147399 repid-1.5.3/repid/health_check_server.py
+-rw-r--r--   0        0        0     7478 2024-04-01 23:29:30.147399 repid-1.5.3/repid/job.py
+-rw-r--r--   0        0        0      548 2024-04-01 23:29:30.147399 repid-1.5.3/repid/logger.py
+-rw-r--r--   0        0        0     1887 2024-04-01 23:29:30.147399 repid-1.5.3/repid/main.py
+-rw-r--r--   0        0        0     3791 2024-04-01 23:29:30.147399 repid-1.5.3/repid/message.py
+-rw-r--r--   0        0        0      257 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3685 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3639 2024-04-01 23:29:30.147399 repid-1.5.3/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/repid/py.typed
+-rw-r--r--   0        0        0     1930 2024-04-01 23:29:30.147399 repid-1.5.3/repid/queue.py
+-rw-r--r--   0        0        0     1319 2024-04-01 23:29:30.147399 repid-1.5.3/repid/retry_policy.py
+-rw-r--r--   0        0        0     5006 2024-04-01 23:29:30.147399 repid-1.5.3/repid/router.py
+-rw-r--r--   0        0        0      512 2024-04-01 23:29:30.147399 repid-1.5.3/repid/serializer.py
+-rw-r--r--   0        0        0      781 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6163 2024-04-01 23:29:30.147399 repid-1.5.3/repid/testing/plugin.py
+-rw-r--r--   0        0        0     4920 2024-04-01 23:29:30.147399 repid-1.5.3/repid/worker.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     1145 2024-04-01 23:29:30.147399 repid-1.5.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4678 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_consumer_different_categories.py
+-rw-r--r--   0        0        0     4005 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0     1402 2024-04-01 23:29:30.147399 repid-1.5.3/tests/integration/test_rabbitmq_specific.py
+-rw-r--r--   0        0        0      431 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_actor.py
+-rw-r--r--   0        0        0     4608 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10230 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_default_data_models.py
+-rw-r--r--   0        0        0    13979 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2110 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_health_check_server.py
+-rw-r--r--   0        0        0     3004 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_job.py
+-rw-r--r--   0        0        0     2298 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_json.py
+-rw-r--r--   0        0        0     1366 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_main.py
+-rw-r--r--   0        0        0     5627 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_message.py
+-rw-r--r--   0        0        0     7842 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7360 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_router.py
+-rw-r--r--   0        0        0     3673 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_runner.py
+-rw-r--r--   0        0        0      762 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_serializer.py
+-rw-r--r--   0        0        0     1893 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_utils.py
+-rw-r--r--   0        0        0     9065 2024-04-01 23:29:30.147399 repid-1.5.3/tests/test_worker.py
+-rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 repid-1.5.3/PKG-INFO
```

### Comparing `repid-1.5.2/LICENSE` & `repid-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/README.md` & `repid-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/pyproject.toml` & `repid-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.5.2"
+version = "1.5.3"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
```

### Comparing `repid-1.5.2/repid/__init__.py` & `repid-1.5.3/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/_asyncify.py` & `repid-1.5.3/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/_processor.py` & `repid-1.5.3/repid/_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,18 @@
             "time_limit": time_limit,
         }
 
         result: str | None = None
         success: bool
         exception = None
 
-        logger.info("Running actor '{actor_name}' on message {message_id}.", extra=logger_extra)
-        logger.debug("Time limit is set to {time_limit}.", extra=logger_extra)
+        logger.debug(
+            "Running actor '{actor_name}' on message {message_id} with time limit {time_limit}.",
+            extra=logger_extra,
+        )
 
         started_when = time.time_ns()
 
         resolver_context = ResolverContext(
             message_key=key,
             message_raw_payload=payload,
             message_parameters=parameters,
@@ -100,31 +102,36 @@
             args, kwargs = actor.converter.convert_inputs(payload)
             _result = await asyncio.wait_for(
                 actor.fn(*args, **kwargs, **dependency_kwargs),
                 timeout=time_limit,
             )
             result = actor.converter.convert_outputs(_result)
         except _NoAction as exc:
+            logger.debug(
+                "Actor '{actor_name}' finished explicitly on message {message_id}.",
+                extra=logger_extra,
+            )
             return ActorResult(
                 data=exc.data,
                 success=exc.success,
                 exception=exc.exception,
                 started_when=started_when,
                 finished_when=time.time_ns(),
                 reporting_done=True,
             )
         except Exception as exc:  # noqa: BLE001
             exception = exc
             success = False
-            logger.exception(
+            logger.debug(
                 "Error inside of an actor '{actor_name}' on message {message_id}.",
                 extra=logger_extra,
+                exc_info=exc,
             )
         else:
-            logger.info(
+            logger.debug(
                 "Actor '{actor_name}' finished successfully on message {message_id}.",
                 extra=logger_extra,
             )
             success = True
 
         return ActorResult(
             data=result,
```

### Comparing `repid-1.5.2/repid/_runner.py` & `repid-1.5.3/repid/_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,34 +22,35 @@
         max_tasks: int = float("inf"),  # type: ignore[assignment]
         tasks_concurrency_limit: int = 1000,
         health_check_server: HealthCheckServer | None = None,
         _connection: Connection | None = None,
     ):
         self._conn = _connection or Repid.get_magic_connection()
 
-        self.tasks: set[asyncio.Task] = set()
+        self._tasks: set[asyncio.Task] = set()
+        self._wait_for_cancel_task: asyncio.Task | None = None
 
         self.stop_consume_event = asyncio.Event()
         self.cancel_event = asyncio.Event()
 
         self.max_tasks = max_tasks
-        self.tasks_concurrency_limit = tasks_concurrency_limit
-        self.limiter = asyncio.Semaphore(tasks_concurrency_limit)
+        self._tasks_concurrency_limit = tasks_concurrency_limit
+        self._limiter = asyncio.Semaphore(tasks_concurrency_limit)
         self._tasks_processed = 0
 
-        self.health_check_server = health_check_server
+        self._health_check_server = health_check_server
 
         super().__init__(self._conn)
 
     @property
     def max_tasks_hit(self) -> bool:
         return (
             self.max_tasks
             - self._tasks_processed
-            - (self.tasks_concurrency_limit - self.limiter._value)
+            - (self._tasks_concurrency_limit - self._limiter._value)
             <= 0
         )
 
     @property
     def cancel_event_task(self) -> asyncio.Task:
         if not hasattr(self, "_cancel_event_task"):
             self._cancel_event_task = asyncio.create_task(self.cancel_event.wait())
@@ -58,16 +59,16 @@
     @property
     def stop_consume_event_task(self) -> asyncio.Task:
         if not hasattr(self, "_stop_consume_event_task"):
             self._stop_consume_event_task = asyncio.create_task(self.stop_consume_event.wait())
         return self._stop_consume_event_task
 
     def _task_callback(self, task: asyncio.Task) -> None:
-        self.tasks.discard(task)
-        self.limiter.release()
+        self._tasks.discard(task)
+        self._limiter.release()
         self._tasks_processed += 1
         if self.max_tasks_hit:
             self.stop_consume_event.set()
 
     async def _process_with_event(
         self,
         actor: ActorData,
@@ -89,34 +90,34 @@
     async def _run_consumer(
         self,
         consumer: ConsumerT,
         actors: dict[str, ActorData],
     ) -> None:
         async for key, payload, params in consumer:
             actor = actors[key.topic]
-            if self.limiter.locked():
+            if self._limiter.locked():
                 await consumer.pause()
-                await self.limiter.acquire()
+                await self._limiter.acquire()
                 await consumer.unpause()
             else:
-                await self.limiter.acquire()
+                await self._limiter.acquire()
             t = asyncio.create_task(self._process_with_event(actor, key, payload, params))
-            self.tasks.add(t)
+            self._tasks.add(t)
             t.add_done_callback(self._task_callback)
 
     async def run_one_queue(
         self,
         queue_name: str,
         topics: Iterable[str],
         actors: dict[str, ActorData],
     ) -> ConsumerT:
         consumer = self._conn.message_broker.get_consumer(
             queue_name,
             topics,
-            self.tasks_concurrency_limit,
+            self._tasks_concurrency_limit,
         )
         await consumer.start()
         consume_task = asyncio.create_task(self._run_consumer(consumer, actors))
         await asyncio.wait(
             {self.stop_consume_event_task, consume_task},
             return_when=asyncio.FIRST_COMPLETED,
         )
@@ -126,13 +127,36 @@
             and (exc := consume_task.exception()) is not None
         ):
             logger.critical(
                 "Error while running consumer on queue '{queue_name}'.",
                 extra={"queue_name": queue_name},
                 exc_info=exc,
             )
-            if self.health_check_server is not None:
-                self.health_check_server.health_status = HealthCheckStatus.UNHEALTHY
+            if self._health_check_server is not None:
+                self._health_check_server.health_status = HealthCheckStatus.UNHEALTHY
         if self.stop_consume_event.is_set():
             consume_task.cancel()
         await consumer.pause()
         return consumer
+
+    async def stop_wait_and_cancel(self, wait_for: float) -> None:
+        self.stop_consume_event.set()
+        await asyncio.sleep(wait_for)
+        self.cancel_event.set()
+
+    def sync_stop_wait_and_cancel(self, wait_for: float) -> None:
+        self._wait_for_cancel_task = asyncio.create_task(self.stop_wait_and_cancel(wait_for))
+
+    async def finish_gracefully(self, timeout: float) -> None:
+        logger.debug("Gracefully finishing runner.")
+        self.stop_consume_event.set()
+        if self._tasks:
+            _, pending = await asyncio.wait(
+                self._tasks,
+                return_when=asyncio.ALL_COMPLETED,
+                timeout=timeout,
+            )
+            if pending:
+                logger.error("Some tasks timeouted when gracefully finishing runner.")
+        if self._wait_for_cancel_task is not None:
+            self._wait_for_cancel_task.cancel()
+        self.cancel_event.set()
```

### Comparing `repid-1.5.2/repid/_utils/__init__.py` & `repid-1.5.3/repid/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/_utils/get_dependency.py` & `repid-1.5.3/repid/_utils/get_dependency.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/_utils/is_installed.py` & `repid-1.5.3/repid/_utils/is_installed.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/_utils/json_encoder.py` & `repid-1.5.3/repid/_utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/actor.py` & `repid-1.5.3/repid/actor.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/config.py` & `repid-1.5.3/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connection.py` & `repid-1.5.3/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/__init__.py` & `repid-1.5.3/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/abc.py` & `repid-1.5.3/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/in_memory/bucket_broker.py` & `repid-1.5.3/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/in_memory/consumer.py` & `repid-1.5.3/repid/connections/in_memory/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/in_memory/message_broker.py` & `repid-1.5.3/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/in_memory/utils.py` & `repid-1.5.3/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/rabbitmq/consumer.py` & `repid-1.5.3/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/rabbitmq/message_broker.py` & `repid-1.5.3/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/rabbitmq/protocols.py` & `repid-1.5.3/repid/connections/rabbitmq/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/rabbitmq/utils.py` & `repid-1.5.3/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/redis/bucket_broker.py` & `repid-1.5.3/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/redis/consumer.py` & `repid-1.5.3/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/redis/message_broker.py` & `repid-1.5.3/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/connections/redis/utils.py` & `repid-1.5.3/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/converter.py` & `repid-1.5.3/repid/converter.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/data/_buckets.py` & `repid-1.5.3/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/data/_key.py` & `repid-1.5.3/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/data/_parameters.py` & `repid-1.5.3/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/data/protocols.py` & `repid-1.5.3/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/dependencies/depends.py` & `repid-1.5.3/repid/dependencies/depends.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/dependencies/message_dependency.py` & `repid-1.5.3/repid/dependencies/message_dependency.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/dependencies/protocols.py` & `repid-1.5.3/repid/dependencies/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/dependencies/resolver_context.py` & `repid-1.5.3/repid/dependencies/resolver_context.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/health_check_server.py` & `repid-1.5.3/repid/health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/job.py` & `repid-1.5.3/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/logger.py` & `repid-1.5.3/repid/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, MutableMapping
 
 
-class FormatWithExtraAdapter(logging.LoggerAdapter):
+class _FormatWithExtraAdapter(logging.LoggerAdapter):
     def process(
         self,
         msg: str,
         kwargs: MutableMapping[str, Any],
     ) -> tuple[str, MutableMapping[str, Any]]:
         if extra := kwargs.get("extra", None):
             msg = msg.format(**extra)
         return msg, kwargs
 
 
 logger = logging.getLogger("repid")
 logger.addHandler(logging.NullHandler())
-logger = FormatWithExtraAdapter(logger, {})  # type: ignore[assignment]
+logger = _FormatWithExtraAdapter(logger, {})  # type: ignore[assignment]
```

### Comparing `repid-1.5.2/repid/main.py` & `repid-1.5.3/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/message.py` & `repid-1.5.3/repid/message.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/middlewares/middleware.py` & `repid-1.5.3/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/middlewares/wrapper.py` & `repid-1.5.3/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/queue.py` & `repid-1.5.3/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/retry_policy.py` & `repid-1.5.3/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/router.py` & `repid-1.5.3/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/serializer.py` & `repid-1.5.3/repid/serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/testing/__init__.py` & `repid-1.5.3/repid/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/testing/modifiers.py` & `repid-1.5.3/repid/testing/modifiers.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/testing/plugin.py` & `repid-1.5.3/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/repid/worker.py` & `repid-1.5.3/repid/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 import asyncio
 import signal
-from typing import TYPE_CHECKING, Callable
+import sys
+from collections.abc import Iterable
+from typing import TYPE_CHECKING
 
 from repid._runner import _Runner
 from repid.health_check_server import HealthCheckServer
+from repid.logger import logger
 from repid.main import Repid
 from repid.queue import Queue
 from repid.router import Router, RouterDefaults
 
 if TYPE_CHECKING:
     from repid.connection import Connection
-    from repid.connections.abc import ConsumerT
     from repid.health_check_server import HealthCheckServerSettings
 
 
 class Worker(Router):
     def __init__(
         self,
-        routers: list[Router] | None = None,
+        routers: Iterable[Router] | None = None,
         *,
         graceful_shutdown_time: float = 25.0,
         messages_limit: int = float("inf"),  # type: ignore[assignment]
         tasks_limit: int = 1000,
-        handle_signals: list[signal.Signals] | None = None,
+        handle_signals: Iterable[signal.Signals] | None = None,
         router_defaults: RouterDefaults | None = None,
         auto_declare: bool = True,
         run_health_check_server: bool = False,
         health_check_server_settings: HealthCheckServerSettings | None = None,
         _connection: Connection | None = None,
     ):
         super().__init__(defaults=router_defaults)
@@ -37,105 +39,102 @@
 
         if routers is not None:
             for router in routers:
                 self.include_router(router)
 
         self.tasks_limit = tasks_limit
         self.graceful_shutdown_time = graceful_shutdown_time
+        self.graceful_consumer_finish_time = 5.0
+        self.graceful_health_check_server_finish_time = 1.0
         self.messages_limit = messages_limit
         self.handle_signals = (
-            [signal.SIGINT, signal.SIGTERM] if handle_signals is None else handle_signals
+            frozenset([signal.SIGINT, signal.SIGTERM] if handle_signals is None else handle_signals)
+            if sys.platform != "emscripten"
+            else frozenset()
         )
         self.auto_declare = auto_declare
         self.health_check_server = None
         if run_health_check_server:
             self.health_check_server = HealthCheckServer(health_check_server_settings)
 
     async def declare_all_queues(self) -> None:
         await asyncio.gather(
             *(
                 Queue(queue_name, _connection=self._conn).declare()
                 for queue_name in self.topics_by_queue
             ),
         )
 
-    async def run(self) -> _Runner:  # noqa: C901
+    async def run(self) -> _Runner:
         if self.health_check_server is not None:
             await self.health_check_server.start()
 
         runner = _Runner(
             max_tasks=self.messages_limit,
             tasks_concurrency_limit=self.tasks_limit,
             health_check_server=self.health_check_server,
             _connection=self._conn,
         )
 
-        if not self.actors:
+        if not self.actors or not self.topics_by_queue:
+            logger.info("Exiting worker, as there are no actors to run.")
             if self.health_check_server is not None:  # pragma: no cover
                 await self.health_check_server.stop()
             return runner
 
         if self.auto_declare:
             await self.declare_all_queues()
 
         loop = asyncio.get_running_loop()
-        signal_handler = self._signal_handler_constructor(runner)
-        for sig in self.handle_signals:
-            loop.add_signal_handler(sig, signal_handler)
+        self._register_signals(loop, runner)
 
-        consumer_tasks: set[asyncio.Task] = set()
-
-        for queue_name in self.topics_by_queue:
-            t = asyncio.create_task(
-                runner.run_one_queue(
-                    queue_name,
-                    self.topics_by_queue[queue_name],
-                    self.actors,
+        logger.debug("Starting consumers.")
+        try:
+            consumers = await asyncio.gather(
+                *(
+                    runner.run_one_queue(
+                        queue_name,
+                        self.topics_by_queue[queue_name],
+                        self.actors,
+                    )
+                    for queue_name in self.topics_by_queue
                 ),
             )
-            consumer_tasks.add(t)
-
-        consumers: set[ConsumerT] = set()
-        if consumer_tasks:
-            consumer_futures, _ = await asyncio.wait(
-                consumer_tasks,
-                return_when=asyncio.ALL_COMPLETED,
-            )
-            for ft in consumer_futures:
-                if ft.exception() is None:
-                    consumers.add(ft.result())
-
-        runner.stop_consume_event.set()
+        except asyncio.CancelledError as exc:
+            logger.critical("Worker was cancelled.", exc_info=exc)
+            raise
 
-        if runner.tasks:
-            await asyncio.wait(runner.tasks, return_when=asyncio.ALL_COMPLETED)
+        await runner.finish_gracefully(timeout=self.graceful_shutdown_time)
 
         if consumers:
-            await asyncio.wait(
-                {asyncio.create_task(c.finish()) for c in consumers},
-                return_when=asyncio.ALL_COMPLETED,
+            logger.debug("Gracefully finishing consumers.")
+            await asyncio.wait_for(
+                asyncio.gather(*(c.finish() for c in consumers)),
+                timeout=self.graceful_consumer_finish_time,
             )
 
-        runner.cancel_event.set()
-
         if self.health_check_server is not None:
-            await self.health_check_server.stop()
+            await asyncio.wait_for(
+                self.health_check_server.stop(),
+                timeout=self.graceful_health_check_server_finish_time,
+            )
+
+        self._unregister_signals(loop)
 
         return runner
 
-    def _signal_handler_constructor(self, runner: _Runner) -> Callable[[], None]:
+    def _register_signals(self, loop: asyncio.AbstractEventLoop, runner: _Runner) -> None:
         def signal_handler() -> None:
-            runner.stop_consume_event.set()
-
-            async def wait_before_cancel() -> None:
-                await asyncio.sleep(self.graceful_shutdown_time)
-                runner.cancel_event.set()
+            runner.sync_stop_wait_and_cancel(self.graceful_shutdown_time)
+            self._unregister_signals(loop)
 
-            t = asyncio.create_task(wait_before_cancel())
-            runner.tasks.add(t)
-            t.add_done_callback(runner.tasks.discard)
-
-            loop = asyncio.get_running_loop()
-            for sig in self.handle_signals:
-                loop.remove_signal_handler(sig)
+        if self.handle_signals:
+            logger.debug(
+                "Registering signal ({signals}) handlers.",
+                extra={"signals": self.handle_signals},
+            )
+        for sig in self.handle_signals:
+            loop.add_signal_handler(sig, signal_handler)
 
-        return signal_handler
+    def _unregister_signals(self, loop: asyncio.AbstractEventLoop) -> None:
+        for sig in self.handle_signals:
+            loop.remove_signal_handler(sig)
```

### Comparing `repid-1.5.2/tests/conftest.py` & `repid-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/conftest.py` & `repid-1.5.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_buckets.py` & `repid-1.5.3/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_consumer.py` & `repid-1.5.3/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_consumer_different_categories.py` & `repid-1.5.3/tests/integration/test_consumer_different_categories.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_default_flow.py` & `repid-1.5.3/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_no_messages_lost.py` & `repid-1.5.3/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/integration/test_rabbitmq_specific.py` & `repid-1.5.3/tests/integration/test_rabbitmq_specific.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_config.py` & `repid-1.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_connection.py` & `repid-1.5.3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_consumer.py` & `repid-1.5.3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_consumer_abc.py` & `repid-1.5.3/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_default_data_models.py` & `repid-1.5.3/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_dependencies.py` & `repid-1.5.3/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_health_check_server.py` & `repid-1.5.3/tests/test_health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_hypothesis.py` & `repid-1.5.3/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_job.py` & `repid-1.5.3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_json.py` & `repid-1.5.3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_main.py` & `repid-1.5.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_message.py` & `repid-1.5.3/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_middleware.py` & `repid-1.5.3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_multiprocessing.py` & `repid-1.5.3/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_pydantic.py` & `repid-1.5.3/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_pytest_plugin.py` & `repid-1.5.3/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_router.py` & `repid-1.5.3/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_runner.py` & `repid-1.5.3/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_serializer.py` & `repid-1.5.3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_utils.py` & `repid-1.5.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.5.2/tests/test_worker.py` & `repid-1.5.3/tests/test_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,44 @@
     await asyncio.sleep(0.3)
     assert not task.done()
     pid = os.getpid()
     os.kill(pid, SIGINT)
     await task
 
 
+async def test_worker_cancel(caplog: pytest.LogCaptureFixture) -> None:
+    r = Router()
+
+    @r.actor
+    async def awesome_job() -> None:
+        await asyncio.sleep(0.01)
+
+    myworker = Worker(routers=[r], graceful_shutdown_time=1)
+
+    task = asyncio.Task(myworker.run())
+    j = Job("awesome_job")
+    await j.queue.declare()
+    await j.enqueue()
+    assert not task.done()
+    assert task.cancel()
+    with pytest.raises(asyncio.CancelledError):
+        await task
+    assert any(
+        (
+            all(
+                (
+                    "CRITICAL" in x,
+                    "Worker was cancelled." in x,
+                ),
+            )
+            for x in caplog.text.splitlines()
+        ),
+    )
+
+
 async def test_worker_long_task_reject() -> None:
     r = Router()
     j = Job("awesome_job")
     await j.queue.declare()
     await j.enqueue()
     hit = False
     never_hit = False
```

### Comparing `repid-1.5.2/PKG-INFO` & `repid-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.5.2
+Version: 1.5.3
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repid Version: 1.5.2 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.5.3 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

