# Comparing `tmp/acb-0.5.8.tar.gz` & `tmp/acb-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.5.8.tar", last modified: Sat Mar  2 11:35:45 2024, max compression
+gzip compressed data, was "acb-0.5.9.tar", last modified: Sat Mar  9 15:07:54 2024, max compression
```

## Comparing `acb-0.5.8.tar` & `acb-0.5.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.5.8/LICENSE
--rw-r--r--   0        0        0      877 2024-02-25 15:01:48.403334 acb-0.5.8/README.md
--rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.5.8/acb/__init__.py
--rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.5.8/acb/actions/__init__.py
--rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.5.8/acb/actions/compress.py
--rw-r--r--   0        0        0     4765 2023-12-09 09:30:31.322361 acb-0.5.8/acb/actions/encode.py
--rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.5.8/acb/actions/hash.py
--rw-r--r--   0        0        0     5580 2024-02-09 17:39:47.412433 acb-0.5.8/acb/adapters/__init__.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.5.8/acb/adapters/app/__init__.py
--rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.5.8/acb/adapters/app/_base.py
--rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.5.8/acb/adapters/app/main.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.5.8/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.5.8/acb/adapters/cache/_base.py
--rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.5.8/acb/adapters/cache/memory.py
--rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.5.8/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.5.8/acb/adapters/dns/__init__.py
--rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.5.8/acb/adapters/dns/_base.py
--rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.5.8/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.5.8/acb/adapters/ftpd/__init__.py
--rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.5.8/acb/adapters/ftpd/_base.py
--rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.5.8/acb/adapters/ftpd/ftp.py
--rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.5.8/acb/adapters/ftpd/sftp.py
--rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.5.8/acb/adapters/logger/__init__.py
--rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.5.8/acb/adapters/logger/_base.py
--rw-r--r--   0        0        0     3333 2024-02-09 09:30:31.991719 acb-0.5.8/acb/adapters/logger/loguru.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.5.8/acb/adapters/logger/structlog.py
--rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.5.8/acb/adapters/monitoring/__init__.py
--rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.5.8/acb/adapters/monitoring/_base.py
--rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.5.8/acb/adapters/monitoring/sentry.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.5.8/acb/adapters/nosql/__init__.py
--rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.5.8/acb/adapters/nosql/_base.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.5.8/acb/adapters/nosql/firestore.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.5.8/acb/adapters/nosql/mongodb.py
--rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.5.8/acb/adapters/nosql/redis.py
--rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.5.8/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.5.8/acb/adapters/requests/_base.py
--rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.5.8/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.5.8/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.5.8/acb/adapters/secret/_base.py
--rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.5.8/acb/adapters/secret/infisical.py
--rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.5.8/acb/adapters/secret/secret_manager.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.5.8/acb/adapters/smtp/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.5.8/acb/adapters/smtp/_base.py
--rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.5.8/acb/adapters/smtp/gmail.py
--rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.5.8/acb/adapters/smtp/mailgun.py
--rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.5.8/acb/adapters/sql/__init__.py
--rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.5.8/acb/adapters/sql/_backup.py
--rw-r--r--   0        0        0     5287 2024-02-19 14:21:22.257011 acb-0.5.8/acb/adapters/sql/_base.py
--rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.5.8/acb/adapters/sql/_migrate.py
--rw-r--r--   0        0        0      702 2024-02-04 20:10:10.946072 acb-0.5.8/acb/adapters/sql/mysql.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.5.8/acb/adapters/sql/pgsql.py
--rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.5.8/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.5.8/acb/adapters/storage/_base.py
--rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.5.8/acb/adapters/storage/azure.py
--rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.5.8/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.5.8/acb/adapters/storage/file.py
--rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.5.8/acb/adapters/storage/memory.py
--rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.5.8/acb/adapters/storage/s3.py
--rw-r--r--   0        0        0    10433 2024-03-01 14:34:19.424984 acb-0.5.8/acb/config.py
--rw-r--r--   0        0        0     1955 2024-02-09 20:35:55.823253 acb-0.5.8/acb/debug.py
--rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.5.8/acb/depends.py
--rw-r--r--   0        0        0     3377 2024-03-02 11:35:45.906731 acb-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 acb-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.5.9/LICENSE
+-rw-r--r--   0        0        0      877 2024-02-25 15:01:48.403334 acb-0.5.9/README.md
+-rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.5.9/acb/__init__.py
+-rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.5.9/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.5.9/acb/actions/compress.py
+-rw-r--r--   0        0        0     4765 2023-12-09 09:30:31.322361 acb-0.5.9/acb/actions/encode.py
+-rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.5.9/acb/actions/hash.py
+-rw-r--r--   0        0        0     5580 2024-02-09 17:39:47.412433 acb-0.5.9/acb/adapters/__init__.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.5.9/acb/adapters/app/__init__.py
+-rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.5.9/acb/adapters/app/_base.py
+-rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.5.9/acb/adapters/app/main.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.5.9/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.5.9/acb/adapters/cache/_base.py
+-rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.5.9/acb/adapters/cache/memory.py
+-rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.5.9/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.5.9/acb/adapters/dns/__init__.py
+-rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.5.9/acb/adapters/dns/_base.py
+-rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.5.9/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.5.9/acb/adapters/ftpd/__init__.py
+-rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.5.9/acb/adapters/ftpd/_base.py
+-rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.5.9/acb/adapters/ftpd/ftp.py
+-rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.5.9/acb/adapters/ftpd/sftp.py
+-rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.5.9/acb/adapters/logger/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.5.9/acb/adapters/logger/_base.py
+-rw-r--r--   0        0        0     3333 2024-02-09 09:30:31.991719 acb-0.5.9/acb/adapters/logger/loguru.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.5.9/acb/adapters/logger/structlog.py
+-rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.5.9/acb/adapters/monitoring/__init__.py
+-rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.5.9/acb/adapters/monitoring/_base.py
+-rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.5.9/acb/adapters/monitoring/sentry.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.5.9/acb/adapters/nosql/__init__.py
+-rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.5.9/acb/adapters/nosql/_base.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.5.9/acb/adapters/nosql/firestore.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.5.9/acb/adapters/nosql/mongodb.py
+-rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.5.9/acb/adapters/nosql/redis.py
+-rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.5.9/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.5.9/acb/adapters/requests/_base.py
+-rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.5.9/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.5.9/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.5.9/acb/adapters/secret/_base.py
+-rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.5.9/acb/adapters/secret/infisical.py
+-rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.5.9/acb/adapters/secret/secret_manager.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.5.9/acb/adapters/smtp/__init__.py
+-rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.5.9/acb/adapters/smtp/_base.py
+-rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.5.9/acb/adapters/smtp/gmail.py
+-rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.5.9/acb/adapters/smtp/mailgun.py
+-rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.5.9/acb/adapters/sql/__init__.py
+-rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.5.9/acb/adapters/sql/_backup.py
+-rw-r--r--   0        0        0     5572 2024-03-09 15:03:14.357031 acb-0.5.9/acb/adapters/sql/_base.py
+-rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.5.9/acb/adapters/sql/_migrate.py
+-rw-r--r--   0        0        0      316 2024-03-09 14:44:51.517804 acb-0.5.9/acb/adapters/sql/mysql.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.5.9/acb/adapters/sql/pgsql.py
+-rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.5.9/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.5.9/acb/adapters/storage/_base.py
+-rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.5.9/acb/adapters/storage/azure.py
+-rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.5.9/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.5.9/acb/adapters/storage/file.py
+-rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.5.9/acb/adapters/storage/memory.py
+-rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.5.9/acb/adapters/storage/s3.py
+-rw-r--r--   0        0        0    10433 2024-03-01 14:34:19.424984 acb-0.5.9/acb/config.py
+-rw-r--r--   0        0        0     1955 2024-02-09 20:35:55.823253 acb-0.5.9/acb/debug.py
+-rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.5.9/acb/depends.py
+-rw-r--r--   0        0        0     3377 2024-03-09 15:07:54.600770 acb-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 acb-0.5.9/PKG-INFO
```

### Comparing `acb-0.5.8/LICENSE` & `acb-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/README.md` & `acb-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/__init__.py` & `acb-0.5.9/acb/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/actions/__init__.py` & `acb-0.5.9/acb/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/actions/compress.py` & `acb-0.5.9/acb/actions/compress.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/actions/encode.py` & `acb-0.5.9/acb/actions/encode.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/actions/hash.py` & `acb-0.5.9/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/__init__.py` & `acb-0.5.9/acb/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/app/main.py` & `acb-0.5.9/acb/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/cache/_base.py` & `acb-0.5.9/acb/adapters/cache/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/cache/memory.py` & `acb-0.5.9/acb/adapters/cache/memory.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/cache/redis.py` & `acb-0.5.9/acb/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/dns/_base.py` & `acb-0.5.9/acb/adapters/dns/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/dns/cloud_dns.py` & `acb-0.5.9/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/ftpd/ftp.py` & `acb-0.5.9/acb/adapters/ftpd/ftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/ftpd/sftp.py` & `acb-0.5.9/acb/adapters/ftpd/sftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/logger/loguru.py` & `acb-0.5.9/acb/adapters/logger/loguru.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/monitoring/sentry.py` & `acb-0.5.9/acb/adapters/monitoring/sentry.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/nosql/redis.py` & `acb-0.5.9/acb/adapters/nosql/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/requests/_base.py` & `acb-0.5.9/acb/adapters/requests/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/requests/httpx.py` & `acb-0.5.9/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/secret/_base.py` & `acb-0.5.9/acb/adapters/secret/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/secret/secret_manager.py` & `acb-0.5.9/acb/adapters/secret/secret_manager.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/smtp/_base.py` & `acb-0.5.9/acb/adapters/smtp/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/smtp/gmail.py` & `acb-0.5.9/acb/adapters/smtp/gmail.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/smtp/mailgun.py` & `acb-0.5.9/acb/adapters/smtp/mailgun.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/sql/_backup.py` & `acb-0.5.9/acb/adapters/sql/_backup.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/sql/_base.py` & `acb-0.5.9/acb/adapters/sql/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 from acb.config import gen_password
 from acb.config import Settings
 from acb.depends import depends
 from aioconsole import ainput
 from aioconsole import aprint
 from pydantic import SecretStr
 from sqlalchemy import inspect
+from sqlalchemy import log as sqlalchemy_log
+from sqlalchemy import pool
 from sqlalchemy.engine import URL
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.ext.asyncio import AsyncConnection
 from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy_utils import create_database
 from sqlalchemy_utils import database_exists
 from sqlalchemy_utils import drop_database
 from sqlmodel import SQLModel
 from sqlmodel.ext.asyncio.session import AsyncSession
-from sqlalchemy import log as sqlalchemy_log
 
 nest_asyncio.apply()
 
 
 class SqlBaseSettings(Settings):
     _driver: str
     _async_driver: str
@@ -34,33 +35,38 @@
     pool_pre_ping: t.Optional[bool] = False
     poolclass: t.Optional[t.Any] = None
     host: SecretStr = SecretStr("127.0.0.1")
     user: SecretStr = SecretStr("root")
     password: SecretStr = SecretStr(gen_password())
     _url: t.Optional[URL] = None
     _async_url: t.Optional[URL] = None
-    engine_kwargs: t.Optional[dict[str, t.Any]] = {}
+    engine_kwargs: t.Optional[dict[str, t.Any | None]] = {}
     backup_enabled: bool = False
     backup_bucket: str | None = None
 
     @depends.inject
     def __init__(self, config: Config = depends(), **values: t.Any) -> None:
         super().__init__(**values)
         url_kwargs = dict(
             drivername=self._driver,
             username=self.user.get_secret_value(),
             password=self.password.get_secret_value(),
             host=("127.0.0.1" if not config.deployed else self.host.get_secret_value()),
             port=self.port,
             database=config.app.name,
         )
+        self.poolclass = getattr(pool, self.poolclass) if self.poolclass else None
         self._url = URL.create(**url_kwargs)  # type: ignore
         async_url_kwargs = dict(drivername=self._async_driver)
         self._async_url = URL.create(**(url_kwargs | async_url_kwargs))  # type: ignore
         self.engine_kwargs["echo"] = config.debug.sql  # type: ignore
+        self.engine_kwargs = (  # type: ignore
+            dict(poolclass=self.poolclass, pool_pre_ping=self.pool_pre_ping)
+            | self.engine_kwargs
+        )
 
 
 class SqlBase(AdapterBase):
     exists: bool = False
 
     @cached_property
     def engine(self) -> AsyncEngine:
```

### Comparing `acb-0.5.8/acb/adapters/storage/_base.py` & `acb-0.5.9/acb/adapters/storage/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/storage/cloud_storage.py` & `acb-0.5.9/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/adapters/storage/file.py` & `acb-0.5.9/acb/adapters/storage/file.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/config.py` & `acb-0.5.9/acb/config.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/debug.py` & `acb-0.5.9/acb/debug.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/acb/depends.py` & `acb-0.5.9/acb/depends.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.8/pyproject.toml` & `acb-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,38 +32,38 @@
 
 [tool.creosote]
 paths = [
     "acb",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pdm",
-    "pytest",
-    "pdm-bump",
-    "pyyaml",
     "phonenumbers",
-    "ulid-py",
+    "pyyaml",
     "autotyping",
-    "alive-progress",
-    "pyfiglet",
     "pre-commit",
+    "ulid-py",
+    "pdm",
+    "pdm-bump",
+    "pyfiglet",
+    "pytest",
+    "alive-progress",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "acb",
 ]
 skips = [
-    "B404",
-    "B113",
-    "B403",
     "B603",
+    "B403",
+    "B113",
+    "B404",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "acb",
 ]
@@ -84,15 +84,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "acb"
-version = "0.5.8"
+version = "0.5.9"
 description = "Asynchronous Component Base"
 dependencies = [
     "itsdangerous>=2.1.2",
     "arrow>=1.3.0",
     "dill>=0.3.8",
     "blake3>=0.4.1",
     "loguru>=0.7.2",
```

### Comparing `acb-0.5.8/PKG-INFO` & `acb-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.5.8
+Version: 0.5.9
 Summary: Asynchronous Component Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Pydantic
```

