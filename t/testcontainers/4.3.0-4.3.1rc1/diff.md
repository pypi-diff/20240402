# Comparing `tmp/testcontainers-4.3.0.tar.gz` & `tmp/testcontainers-4.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.3.0.tar", max compression
+gzip compressed data, was "testcontainers-4.3.1rc1.tar", max compression
```

## Comparing `testcontainers-4.3.0.tar` & `testcontainers-4.3.1rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11328 2024-04-01 11:51:45.518006 testcontainers-4.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-04-01 11:51:45.518006 testcontainers-4.3.0/README.md
--rw-r--r--   0        0        0      172 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0      605 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     7687 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     7262 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2418 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      498 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     2088 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4059 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3760 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3759 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     3313 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     4116 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3260 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     1808 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     3261 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2761 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4108 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2809 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3971 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5188 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2966 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     2722 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     5588 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8628 2024-04-01 11:51:45.526006 testcontainers-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 testcontainers-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-01-06 17:14:55.248304 testcontainers-4.3.1rc1/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/README.md
+-rw-r--r--   0        0        0      172 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13096 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-03-30 22:33:47.281295 testcontainers-4.3.1rc1/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     7687 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     7291 2024-04-02 13:13:45.170018 testcontainers-4.3.1rc1/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2418 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      498 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     2088 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4059 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3760 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-03-31 04:21:26.952617 testcontainers-4.3.1rc1/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3759 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2662 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     3313 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     4116 2024-03-31 04:19:23.524246 testcontainers-4.3.1rc1/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3016 2024-04-02 13:13:16.910367 testcontainers-4.3.1rc1/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     1808 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     3261 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2761 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4108 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2809 2024-03-31 06:55:02.770026 testcontainers-4.3.1rc1/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3971 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5188 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2966 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-03-31 05:46:55.463194 testcontainers-4.3.1rc1/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     2722 2024-03-31 04:19:23.528246 testcontainers-4.3.1rc1/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     5588 2024-03-31 04:21:26.956617 testcontainers-4.3.1rc1/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8631 2024-04-02 13:14:11.629684 testcontainers-4.3.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 testcontainers-4.3.1rc1/PKG-INFO
```

### Comparing `testcontainers-4.3.0/LICENSE.txt` & `testcontainers-4.3.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/README.md` & `testcontainers-4.3.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/compose/compose.py` & `testcontainers-4.3.1rc1/core/testcontainers/compose/compose.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/config.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/config.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/container.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/container.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/docker_client.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/docker_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     """
 
     def __init__(self, **kwargs) -> None:
         docker_host = get_docker_host()
 
         if docker_host:
             LOGGER.info(f"using host {docker_host}")
-            self.client = docker.DockerClient(base_url=docker_host)
+            kwargs["base_url"] = docker_host
+            self.client = docker.from_env(**kwargs)
         else:
             self.client = docker.from_env(**kwargs)
         self.client.api.headers["x-tc-sid"] = SESSION_ID
         self.client.api.headers["User-Agent"] = "tc-python/" + importlib.metadata.version("testcontainers")
 
     @ft.wraps(ContainerCollection.run)
     def run(
```

### Comparing `testcontainers-4.3.0/core/testcontainers/core/exceptions.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/generic.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/utils.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.3.1rc1/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.3.1rc1/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.3.1rc1/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.3.1rc1/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.3.1rc1/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.3.1rc1/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.3.1rc1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.3.1rc1/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.3.1rc1/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.3.1rc1/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.3.1rc1/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.3.1rc1/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.3.1rc1/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.3.1rc1/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.3.1rc1/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.3.1rc1/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.3.1rc1/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,49 +26,44 @@
 
     Example:
 
         .. doctest::
 
             >>> from testcontainers.mongodb import MongoDbContainer
 
-            >>> with MongoDbContainer("mongo:latest") as mongo:
+            >>> with MongoDbContainer("mongo:7.0.7") as mongo:
             ...    db = mongo.get_connection_client().test
             ...    # Insert a database entry
             ...    result = db.restaurants.insert_one(
             ...        {
-            ...            "address": {
-            ...                "street": "2 Avenue",
-            ...                "zipcode": "10075",
-            ...                "building": "1480",
-            ...                "coord": [-73.9557413, 40.7720266]
-            ...            },
-            ...            "borough": "Manhattan",
-            ...            "cuisine": "Italian",
             ...            "name": "Vella",
-            ...            "restaurant_id": "41704620"
+            ...            "cuisine": "Italian",
+            ...            "restaurant_id": "123456"
             ...        }
             ...    )
             ...    # Find the restaurant document
-            ...    cursor = db.restaurants.find({"borough": "Manhattan"})
+            ...    result = db.restaurants.find_one({"name": "Vella"})
+            ...    result["restaurant_id"]
+            '123456'
     """
 
     def __init__(
         self,
         image: str = "mongo:latest",
         port: int = 27017,
         username: Optional[str] = None,
         password: Optional[str] = None,
         dbname: Optional[str] = None,
         **kwargs
     ) -> None:
         raise_for_deprecated_parameter(kwargs, "port_to_expose", "port")
         super().__init__(image=image, **kwargs)
-        self.username = username or os.environ.get("MONGO_INITDB_ROOT_USERNAME", "test")
-        self.password = password or os.environ.get("MONGO_INITDB_ROOT_PASSWORD", "test")
-        self.dbname = dbname or os.environ.get("MONGO_DB", "test")
+        self.username = username if username else os.environ.get("MONGO_INITDB_ROOT_USERNAME", "test")
+        self.password = password if password else os.environ.get("MONGO_INITDB_ROOT_PASSWORD", "test")
+        self.dbname = dbname if dbname else os.environ.get("MONGO_DB", "test")
         self.port = port
         self.with_exposed_ports(self.port)
 
     def _configure(self) -> None:
         self.with_env("MONGO_INITDB_ROOT_USERNAME", self.username)
         self.with_env("MONGO_INITDB_ROOT_PASSWORD", self.password)
         self.with_env("MONGO_DB", self.dbname)
```

### Comparing `testcontainers-4.3.0/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.3.1rc1/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.3.1rc1/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.3.1rc1/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.3.1rc1/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.3.1rc1/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.3.1rc1/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.3.1rc1/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.3.1rc1/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.3.1rc1/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.3.1rc1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.3.1rc1/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.3.1rc1/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.3.1rc1/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.3.1rc1/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.0/pyproject.toml` & `testcontainers-4.3.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.3.0"  # auto-incremented by release-please
+version = "4.3.1rc1"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
```

### Comparing `testcontainers-4.3.0/PKG-INFO` & `testcontainers-4.3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.3.0
+Version: 4.3.1rc1
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

