# Comparing `tmp/msscrawler-1.3.1.tar.gz` & `tmp/msscrawler-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msscrawler-1.3.1.tar", last modified: Sat Mar 23 15:36:05 2024, max compression
+gzip compressed data, was "msscrawler-1.3.2.tar", last modified: Tue Apr  2 08:21:07 2024, max compression
```

## Comparing `msscrawler-1.3.1.tar` & `msscrawler-1.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.987167 msscrawler-1.3.1/
--rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-03-23 15:36:05.987079 msscrawler-1.3.1/PKG-INFO
--rw-r--r--   0 hoonie     (501) staff       (20)     4347 2023-10-27 15:07:06.000000 msscrawler-1.3.1/README.md
--rw-r--r--   0 hoonie     (501) staff       (20)       86 2023-10-24 15:03:13.000000 msscrawler-1.3.1/pyproject.toml
--rw-r--r--   0 hoonie     (501) staff       (20)      719 2024-03-23 15:36:05.987678 msscrawler-1.3.1/setup.cfg
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.973307 msscrawler-1.3.1/src/
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.975949 msscrawler-1.3.1/src/msscrawler/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      488 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/base_crawler.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.976934 msscrawler-1.3.1/src/msscrawler/connectors/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.977703 msscrawler-1.3.1/src/msscrawler/connectors/databases/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/databases/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      548 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/databases/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)      984 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/databases/mongodb_connector.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.978476 msscrawler-1.3.1/src/msscrawler/connectors/message_brokers/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/message_brokers/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      344 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/connectors/message_brokers/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)     2550 2023-12-07 04:59:45.000000 msscrawler-1.3.1/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py
--rw-r--r--   0 hoonie     (501) staff       (20)     8396 2024-03-17 06:30:45.000000 msscrawler-1.3.1/src/msscrawler/generic_crawler.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.980193 msscrawler-1.3.1/src/msscrawler/items/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/items/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      224 2024-03-08 08:12:57.000000 msscrawler-1.3.1/src/msscrawler/items/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)       74 2024-03-19 08:01:55.000000 msscrawler-1.3.1/src/msscrawler/items/brand_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      394 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/items/category_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      841 2024-03-23 15:35:05.000000 msscrawler-1.3.1/src/msscrawler/items/product_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      244 2024-01-19 08:49:20.000000 msscrawler-1.3.1/src/msscrawler/items/website_item.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.980761 msscrawler-1.3.1/src/msscrawler/log/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/log/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      655 2023-12-14 08:19:28.000000 msscrawler-1.3.1/src/msscrawler/log/default.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.981255 msscrawler-1.3.1/src/msscrawler/middlewares/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/middlewares/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.982354 msscrawler-1.3.1/src/msscrawler/mixins/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/mixins/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1069 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/mixins/database_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)       70 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/mixins/env_loader_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)      819 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/mixins/message_connector_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1804 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/mixins/spider_cache_mixin.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.982800 msscrawler-1.3.1/src/msscrawler/pipelines/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/pipelines/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      480 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/pipelines/base.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.982998 msscrawler-1.3.1/src/msscrawler/sites/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/sites/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.983938 msscrawler-1.3.1/src/msscrawler/sites/shopping/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.984375 msscrawler-1.3.1/src/msscrawler/sites/shopping/spiders/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/spiders/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1316 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py
--rw-r--r--   0 hoonie     (501) staff       (20)     9636 2024-02-05 03:03:42.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/website_crawler.py
--rw-r--r--   0 hoonie     (501) staff       (20)      215 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/website_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)     5416 2024-02-05 03:08:25.000000 msscrawler-1.3.1/src/msscrawler/sites/shopping/website_pipeline.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.986266 msscrawler-1.3.1/src/msscrawler/spiders/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.1/src/msscrawler/spiders/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     9969 2024-03-17 06:31:14.000000 msscrawler-1.3.1/src/msscrawler/spiders/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)      429 2024-03-19 08:04:31.000000 msscrawler-1.3.1/src/msscrawler/spiders/brand.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1171 2024-01-20 16:39:13.000000 msscrawler-1.3.1/src/msscrawler/spiders/category.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1598 2024-03-23 15:35:20.000000 msscrawler-1.3.1/src/msscrawler/spiders/product.py
--rw-r--r--   0 hoonie     (501) staff       (20)      734 2024-02-29 02:01:52.000000 msscrawler-1.3.1/src/msscrawler/spiders/website.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-03-23 15:36:05.986719 msscrawler-1.3.1/src/msscrawler.egg-info/
--rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-03-23 15:36:05.000000 msscrawler-1.3.1/src/msscrawler.egg-info/PKG-INFO
--rw-r--r--   0 hoonie     (501) staff       (20)     1757 2024-03-23 15:36:05.000000 msscrawler-1.3.1/src/msscrawler.egg-info/SOURCES.txt
--rw-r--r--   0 hoonie     (501) staff       (20)        1 2024-03-23 15:36:05.000000 msscrawler-1.3.1/src/msscrawler.egg-info/dependency_links.txt
--rw-r--r--   0 hoonie     (501) staff       (20)       11 2024-03-23 15:36:05.000000 msscrawler-1.3.1/src/msscrawler.egg-info/top_level.txt
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.673157 msscrawler-1.3.2/
+-rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-02 08:21:07.673071 msscrawler-1.3.2/PKG-INFO
+-rw-r--r--   0 hoonie     (501) staff       (20)     4347 2023-10-27 15:07:06.000000 msscrawler-1.3.2/README.md
+-rw-r--r--   0 hoonie     (501) staff       (20)       86 2023-10-24 15:03:13.000000 msscrawler-1.3.2/pyproject.toml
+-rw-r--r--   0 hoonie     (501) staff       (20)      719 2024-04-02 08:21:07.673432 msscrawler-1.3.2/setup.cfg
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.660218 msscrawler-1.3.2/src/
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.662662 msscrawler-1.3.2/src/msscrawler/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      488 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/base_crawler.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.663943 msscrawler-1.3.2/src/msscrawler/connectors/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.664820 msscrawler-1.3.2/src/msscrawler/connectors/databases/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/databases/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      548 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/databases/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      984 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/databases/mongodb_connector.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.665650 msscrawler-1.3.2/src/msscrawler/connectors/message_brokers/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/message_brokers/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      344 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/connectors/message_brokers/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     2550 2023-12-07 04:59:45.000000 msscrawler-1.3.2/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     8396 2024-03-17 06:30:45.000000 msscrawler-1.3.2/src/msscrawler/generic_crawler.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.667268 msscrawler-1.3.2/src/msscrawler/items/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/items/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      224 2024-03-08 08:12:57.000000 msscrawler-1.3.2/src/msscrawler/items/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)       74 2024-03-19 08:01:55.000000 msscrawler-1.3.2/src/msscrawler/items/brand_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      394 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/items/category_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      841 2024-03-23 15:35:05.000000 msscrawler-1.3.2/src/msscrawler/items/product_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      244 2024-01-19 08:49:20.000000 msscrawler-1.3.2/src/msscrawler/items/website_item.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.667694 msscrawler-1.3.2/src/msscrawler/log/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/log/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      655 2023-12-14 08:19:28.000000 msscrawler-1.3.2/src/msscrawler/log/default.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.668022 msscrawler-1.3.2/src/msscrawler/middlewares/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/middlewares/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.669013 msscrawler-1.3.2/src/msscrawler/mixins/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/mixins/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1069 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/mixins/database_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)       70 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/mixins/env_loader_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      819 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/mixins/message_connector_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1804 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/mixins/spider_cache_mixin.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.669312 msscrawler-1.3.2/src/msscrawler/pipelines/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/pipelines/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      480 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/pipelines/base.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.669479 msscrawler-1.3.2/src/msscrawler/sites/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/sites/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.670371 msscrawler-1.3.2/src/msscrawler/sites/shopping/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.670881 msscrawler-1.3.2/src/msscrawler/sites/shopping/spiders/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/spiders/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1316 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     9636 2024-02-05 03:03:42.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/website_crawler.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      215 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/website_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     5416 2024-02-05 03:08:25.000000 msscrawler-1.3.2/src/msscrawler/sites/shopping/website_pipeline.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.672446 msscrawler-1.3.2/src/msscrawler/spiders/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.2/src/msscrawler/spiders/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     9969 2024-03-17 06:31:14.000000 msscrawler-1.3.2/src/msscrawler/spiders/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      429 2024-03-19 08:04:31.000000 msscrawler-1.3.2/src/msscrawler/spiders/brand.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1171 2024-01-20 16:39:13.000000 msscrawler-1.3.2/src/msscrawler/spiders/category.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1594 2024-04-02 08:18:05.000000 msscrawler-1.3.2/src/msscrawler/spiders/product.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      734 2024-02-29 02:01:52.000000 msscrawler-1.3.2/src/msscrawler/spiders/website.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-02 08:21:07.672783 msscrawler-1.3.2/src/msscrawler.egg-info/
+-rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-02 08:21:07.000000 msscrawler-1.3.2/src/msscrawler.egg-info/PKG-INFO
+-rw-r--r--   0 hoonie     (501) staff       (20)     1757 2024-04-02 08:21:07.000000 msscrawler-1.3.2/src/msscrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 hoonie     (501) staff       (20)        1 2024-04-02 08:21:07.000000 msscrawler-1.3.2/src/msscrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 hoonie     (501) staff       (20)       11 2024-04-02 08:21:07.000000 msscrawler-1.3.2/src/msscrawler.egg-info/top_level.txt
```

### Comparing `msscrawler-1.3.1/PKG-INFO` & `msscrawler-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msscrawler
-Version: 1.3.1
+Version: 1.3.2
 Summary: A common package for crawling
 Home-page: https://bitbucket.org/dosiin/common/src/package/
 Author: no name
 Author-email: msscrawler@gmail.com
 Project-URL: Bug Tracker, https://bitbucket.org/dosiin/common/src/package/issues
 Project-URL: repository, https://bitbucket.org/dosiin/common/src/package/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `msscrawler-1.3.1/README.md` & `msscrawler-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/setup.cfg` & `msscrawler-1.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = msscrawler
-version = 1.3.1
+version = 1.3.2
 author = no name
 author_email = msscrawler@gmail.com
 description = A common package for crawling
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://bitbucket.org/dosiin/common/src/package/
 project_urls =
```

### Comparing `msscrawler-1.3.1/src/msscrawler/connectors/databases/base.py` & `msscrawler-1.3.2/src/msscrawler/connectors/databases/base.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/connectors/databases/mongodb_connector.py` & `msscrawler-1.3.2/src/msscrawler/connectors/databases/mongodb_connector.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py` & `msscrawler-1.3.2/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/generic_crawler.py` & `msscrawler-1.3.2/src/msscrawler/generic_crawler.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/items/product_item.py` & `msscrawler-1.3.2/src/msscrawler/items/product_item.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/log/default.py` & `msscrawler-1.3.2/src/msscrawler/log/default.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/mixins/database_mixin.py` & `msscrawler-1.3.2/src/msscrawler/mixins/database_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/mixins/message_connector_mixin.py` & `msscrawler-1.3.2/src/msscrawler/mixins/message_connector_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/mixins/spider_cache_mixin.py` & `msscrawler-1.3.2/src/msscrawler/mixins/spider_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py` & `msscrawler-1.3.2/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/sites/shopping/website_crawler.py` & `msscrawler-1.3.2/src/msscrawler/sites/shopping/website_crawler.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/sites/shopping/website_pipeline.py` & `msscrawler-1.3.2/src/msscrawler/sites/shopping/website_pipeline.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/spiders/base.py` & `msscrawler-1.3.2/src/msscrawler/spiders/base.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/spiders/category.py` & `msscrawler-1.3.2/src/msscrawler/spiders/category.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler/spiders/product.py` & `msscrawler-1.3.2/src/msscrawler/spiders/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         items["shipping_type"] = 1  # update when error
         items["shipping_condition"] = 0  # update when error
         items["options"] = []  # update when error
         items["total_options"] = 0  # update when error
         items["currency"] = "KRW"  # update when error
         items["category_id"] = self.category_id
         items["image_urls"] = []
-        items["wish_count"] = "Null"
-        items["review_count"] = "Null"
+        items["wish_count"] = None
+        items["review_count"] = None
         items["outdate"] = False
         items["platform_category_name"] = ""
         items["platform_category_url"] = ""
         items["platform_category_breadcrumb"] = ""
         items["platform_category_id"] = None
         return items
```

### Comparing `msscrawler-1.3.1/src/msscrawler/spiders/website.py` & `msscrawler-1.3.2/src/msscrawler/spiders/website.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.1/src/msscrawler.egg-info/PKG-INFO` & `msscrawler-1.3.2/src/msscrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msscrawler
-Version: 1.3.1
+Version: 1.3.2
 Summary: A common package for crawling
 Home-page: https://bitbucket.org/dosiin/common/src/package/
 Author: no name
 Author-email: msscrawler@gmail.com
 Project-URL: Bug Tracker, https://bitbucket.org/dosiin/common/src/package/issues
 Project-URL: repository, https://bitbucket.org/dosiin/common/src/package/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `msscrawler-1.3.1/src/msscrawler.egg-info/SOURCES.txt` & `msscrawler-1.3.2/src/msscrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

