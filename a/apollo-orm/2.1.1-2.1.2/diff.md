# Comparing `tmp/apollo-orm-2.1.1.tar.gz` & `tmp/apollo-orm-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.1.tar", last modified: Mon Apr  1 20:58:37 2024, max compression
+gzip compressed data, was "apollo-orm-2.1.2.tar", last modified: Tue Apr  2 17:47:50 2024, max compression
```

## Comparing `apollo-orm-2.1.1.tar` & `apollo-orm-2.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.786523 apollo-orm-2.1.1/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-01 20:58:37.785087 apollo-orm-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.750048 apollo-orm-2.1.1/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.1/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.755054 apollo-orm-2.1.1/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.1/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.756049 apollo-orm-2.1.1/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.1/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.757049 apollo-orm-2.1.1/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.759106 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.759106 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.761105 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.763145 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.764145 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.766146 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.767150 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.769524 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.770797 apollo-orm-2.1.1/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.1/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.774352 apollo-orm-2.1.1/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    20501 2024-04-01 20:58:02.000000 apollo-orm-2.1.1/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.777684 apollo-orm-2.1.1/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.779685 apollo-orm-2.1.1/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.1/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.780683 apollo-orm-2.1.1/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.1/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.1/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.782686 apollo-orm-2.1.1/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.1/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.1/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.784079 apollo-orm-2.1.1/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-01 20:58:19.000000 apollo-orm-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 20:58:37.786523 apollo-orm-2.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.782686 apollo-orm-2.1.1/tests/
--rw-rw-rw-   0        0        0    13745 2024-03-27 21:46:59.000000 apollo-orm-2.1.1/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.462821 apollo-orm-2.1.2/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-02 17:47:50.462821 apollo-orm-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.432821 apollo-orm-2.1.2/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.2/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.436820 apollo-orm-2.1.2/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.2/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.437822 apollo-orm-2.1.2/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.2/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.437822 apollo-orm-2.1.2/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.439822 apollo-orm-2.1.2/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.439822 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.441820 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.442820 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.444820 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.445822 apollo-orm-2.1.2/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.447821 apollo-orm-2.1.2/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.448820 apollo-orm-2.1.2/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.2/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.450820 apollo-orm-2.1.2/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.2/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.452820 apollo-orm-2.1.2/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.2/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.2/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.2/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    21081 2024-04-02 17:42:32.000000 apollo-orm-2.1.2/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.455820 apollo-orm-2.1.2/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.2/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.2/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.2/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.2/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.456820 apollo-orm-2.1.2/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.2/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.458820 apollo-orm-2.1.2/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.2/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.2/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.459821 apollo-orm-2.1.2/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.2/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.2/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.461821 apollo-orm-2.1.2/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-02 17:47:50.000000 apollo-orm-2.1.2/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-02 17:47:50.000000 apollo-orm-2.1.2/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 17:47:50.000000 apollo-orm-2.1.2/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 17:47:50.000000 apollo-orm-2.1.2/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-02 17:05:09.000000 apollo-orm-2.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 17:47:50.462821 apollo-orm-2.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 17:47:50.460819 apollo-orm-2.1.2/tests/
+-rw-rw-rw-   0        0        0    13745 2024-03-27 21:46:59.000000 apollo-orm-2.1.2/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.1/LICENSE` & `apollo-orm-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/PKG-INFO` & `apollo-orm-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.1
+Version: 2.1.2
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.1/README.md` & `apollo-orm-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo-orm-2.1.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo-orm-2.1.2/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo-orm-2.1.2/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/orm/abstracts/idatabase.py` & `apollo-orm-2.1.2/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/orm/core.py` & `apollo-orm-2.1.2/apollo_orm/orm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 import uuid
 from asyncio import Semaphore
 from datetime import datetime, date
 
 from typing import Dict, Optional, List, Any
 
 from cassandra.auth import PlainTextAuthProvider
-from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture
+from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture, \
+    EXEC_PROFILE_DEFAULT
 from cassandra.concurrent import execute_concurrent_with_args
 from cassandra.connection import ConnectionException
-from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, HostDistance
+from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, HostDistance, RetryPolicy, \
+    ExponentialReconnectionPolicy, SpeculativeExecutionPolicy
 from cassandra.query import PreparedStatement
 from apollo_orm.domains.models.entities.column.entity import Column
 from apollo_orm.domains.models.entities.concurrent.pre_processed_insert.entity import PreProcessedInsertData
 from apollo_orm.domains.models.entities.concurrent.result_list.entity import ResultList
 from apollo_orm.domains.models.entities.concurrent.result_process.entity import ResultProcess
 from apollo_orm.domains.models.entities.connection_config.entity import ConnectionConfig
 from apollo_orm.domains.models.entities.table_config.entity import TableConfig
@@ -116,15 +118,17 @@
                  ):
         self._in_process = []
         self._semaphore: Optional[Semaphore] = None
         self._policy = DCAwareRoundRobinPolicy(
             connection_config.credential.datacenter) if connection_config.credential.datacenter else RoundRobinPolicy()
         self._load_balancing_policy = TokenAwarePolicy(self._policy)
         self._execution_profile: ExecutionProfile = ExecutionProfile(load_balancing_policy=self._load_balancing_policy,
-                                                                     request_timeout=client_timeout)
+                                                                     request_timeout=client_timeout,
+                                                                     retry_policy=RetryPolicy(),
+                                                                     speculative_execution_policy=SpeculativeExecutionPolicy())
         self._connection_config = connection_config
         self._attempts = attempts
         self._table_config: Optional[List[TableConfig]] = None
         self._prepared_statements: Dict[str, PreparedStatement] = {}
         self.cluster: Optional[Cluster] = None
         self.session: Optional[Session] = None
         self.connect()
@@ -141,15 +145,17 @@
                     password=self._connection_config.credential.password
                 )
                 self.cluster = Cluster(
                     contact_points=self._connection_config.credential.hosts,
                     port=self._connection_config.credential.port,
                     auth_provider=auth_provider,
                     protocol_version=protocol_version,
-                    execution_profiles={'EXECUTION_PROFILE': self._execution_profile}
+                    execution_profiles={EXEC_PROFILE_DEFAULT: self._execution_profile},
+                    reconnection_policy=ExponentialReconnectionPolicy(base_delay=1.0, max_delay=60.0,
+                                                                      max_attempts=self._attempts)
                 )
                 self.session = self.cluster.connect()
                 self._semaphore = threading.Semaphore(self._get_number_of_requests())
                 self._scan_tables()
                 self.log.info(f"Connected to {self._connection_config.credential.hosts}")
                 return
             except ConnectionException as e:
@@ -316,14 +322,15 @@
         self._execute_query(prepared_statement, values)
 
     def release_semaphore(self):
         self._semaphore.release()
 
     def _execute_async_query(self, statement: PreparedStatement, values: List[Any]) -> ResponseFuture:
         self._semaphore.acquire()
+        statement.is_idempotent = True
         self.log.info(f"Executing query: {statement.query_string} with values: {values}")
         try:
             return self.session.execute_async(statement.bind(values))
         except (NoHostAvailable, ConnectionException) as e:
             self.log.error(f"Connection error: {e}. Reconnecting...")
             self.reconnect()
             return self.session.execute_async(statement.bind(values))
```

### Comparing `apollo-orm-2.1.1/apollo_orm/orm/credentials/credential_service.py` & `apollo-orm-2.1.2/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/orm/credentials/json_credential_service.py` & `apollo-orm-2.1.2/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo-orm-2.1.2/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo-orm-2.1.2/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm/utils/logger/logger.py` & `apollo-orm-2.1.2/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/apollo_orm.egg-info/PKG-INFO` & `apollo-orm-2.1.2/apollo_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.1
+Version: 2.1.2
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.1/apollo_orm.egg-info/SOURCES.txt` & `apollo-orm-2.1.2/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.1/pyproject.toml` & `apollo-orm-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.1/tests/test_full_process.py` & `apollo-orm-2.1.2/tests/test_full_process.py`

 * *Files identical despite different names*

