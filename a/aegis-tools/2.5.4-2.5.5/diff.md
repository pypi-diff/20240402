# Comparing `tmp/aegis-tools-2.5.4.tar.gz` & `tmp/aegis-tools-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.5.4.tar", last modified: Fri Mar 22 00:51:44 2024, max compression
+gzip compressed data, was "aegis-tools-2.5.5.tar", last modified: Tue Apr  2 02:20:33 2024, max compression
```

## Comparing `aegis-tools-2.5.4.tar` & `aegis-tools-2.5.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-03-22 00:51:44.943233 aegis-tools-2.5.4/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-03-22 00:51:44.943233 aegis-tools-2.5.4/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-03-22 00:51:44.939233 aegis-tools-2.5.4/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20800 2024-03-21 19:10:22.000000 aegis-tools-2.5.4/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19045 2024-01-31 22:09:14.000000 aegis-tools-2.5.4/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.4/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24750 2024-03-21 19:10:22.000000 aegis-tools-2.5.4/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27038 2024-01-31 22:05:16.000000 aegis-tools-2.5.4/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.4/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    45872 2024-03-22 00:50:45.000000 aegis-tools-2.5.4/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-03-22 00:51:44.939233 aegis-tools-2.5.4/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.4/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.4/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.4/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.4/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.4/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    33163 2024-02-23 20:02:21.000000 aegis-tools-2.5.4/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-03-22 00:51:44.943233 aegis-tools-2.5.4/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.4/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.4/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.4/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.4/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.4/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.4/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.4/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.4/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.4/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.4/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.4/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.4/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.4/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.4/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78604 2024-02-21 22:36:17.000000 aegis-tools-2.5.4/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-03-22 00:51:44.943233 aegis-tools-2.5.4/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-03-22 00:51:44.000000 aegis-tools-2.5.4/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-03-22 00:51:44.943233 aegis-tools-2.5.4/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.4/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.379211 aegis-tools-2.5.5/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.359211 aegis-tools-2.5.5/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20800 2024-03-21 19:10:22.000000 aegis-tools-2.5.5/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19045 2024-01-31 22:09:14.000000 aegis-tools-2.5.5/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.5/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24750 2024-03-21 19:10:22.000000 aegis-tools-2.5.5/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27285 2024-03-25 22:46:01.000000 aegis-tools-2.5.5/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.5/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46086 2024-04-02 02:17:33.000000 aegis-tools-2.5.5/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.367211 aegis-tools-2.5.5/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.5/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.5/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.5/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.5/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.5/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    33163 2024-02-23 20:02:21.000000 aegis-tools-2.5.5/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.5/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.5/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.5/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.5/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.5/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.5/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.5/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.5/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.5/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.5/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.5/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.5/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.5/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78603 2024-04-02 02:17:33.000000 aegis-tools-2.5.5/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-02 02:20:33.379211 aegis-tools-2.5.5/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.5/setup.py
```

### Comparing `aegis-tools-2.5.4/LICENSE` & `aegis-tools-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/PKG-INFO` & `aegis-tools-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.4
+Version: 2.5.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.4/README.md` & `aegis-tools-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/aegis_.py` & `aegis-tools-2.5.5/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/build.py` & `aegis-tools-2.5.5/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/config.py` & `aegis-tools-2.5.5/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/database.py` & `aegis-tools-2.5.5/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/hydra.py` & `aegis-tools-2.5.5/aegis/hydra.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,21 +438,25 @@
                             #    logging.warning("%s queue purge deleted %s hydra_queue" % (self.thread_name, purged_completed))
                             # Log if there are expired queue items in the past...
                             past_items = aegis.model.HydraQueue.past_items(minutes=self.stuck_minutes, dbconn=dbconn)
                             if past_items and len(past_items):
                                 #logging.error("HydraQueue has %s stuck items", len(past_items))
                                 for past_item in past_items:
                                     past_item_type = aegis.model.HydraType.get_id(past_item['hydra_type_id'], dbconn=dbconn)
+                                    if past_item_type['status'] == 'paused':
+                                        continue
                                     logging.error("Running stuck hydra_queue_id: %s  hydra_type_name: %s", past_item['hydra_queue_id'], past_item_type['hydra_type_name'])
                                     past_item.run_now(dbconn=dbconn)
                             # Any hydra_type claimed since the next_run_dttm and over 5m old are stuck. Automatically unclaim them.
                             past_items = aegis.model.HydraType.past_items(minutes=self.stuck_minutes, dbconn=dbconn)
                             if past_items and len(past_items):
                                 #logging.error("HydraType has %s stuck items", len(past_items))
                                 for past_item in past_items:
+                                    if past_item['status'] == 'paused':
+                                        continue
                                     logging.error("Unclaiming stuck hydra_type_id: %s  hydra_type_name: %s", past_item['hydra_type_name'], past_item['hydra_type_name'])
                                     past_item.unclaim(dbconn=dbconn)
                         elif hydra_type['status'] != 'paused' and hydra_type['next_run_dttm'] and hydra_type['next_run_dttm'] < (utcnow - datetime.timedelta(seconds=30)):
                             if hydra_type['run_env'] == aegis.config.get('env'):
                                 self.logw(hydra_type, "HYDRA TYPE BEHIND ON RUNNING")
 
                 # Better handling of AdminShutdown, OperationalError, to capture structured and complete data to logs and alerts.
```

### Comparing `aegis-tools-2.5.4/aegis/mailer.py` & `aegis-tools-2.5.5/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/model.py` & `aegis-tools-2.5.5/aegis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -990,14 +990,20 @@
             cache_obj = cls.get_key(cache_key)
         else:
             cls.insert(cache_key, cache_json, cache_expiry)
             cache_obj = cls.get_key(cache_key)
         return cache_obj
 
     @staticmethod
+    def del_star(cache_key):
+        cache_key = cache_key.replace('*', '%%')
+        sql = "DELETE FROM cache WHERE cache_key LIKE '" + cache_key + "'"
+        return db().execute_rowcount(sql)
+
+    @staticmethod
     def del_key(cache_key):
         sql = "DELETE FROM cache WHERE cache_key=%s"
         return db().execute(sql, cache_key)
 
     @staticmethod
     def purge_expired():
         sql = "DELETE FROM cache WHERE cache_expiry < NOW()"
```

### Comparing `aegis-tools-2.5.4/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.5.5/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.5.5/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/build-mysql.sql` & `aegis-tools-2.5.5/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/build-pgsql.sql` & `aegis-tools-2.5.5/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.5.5/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/google_signin.sql` & `aegis-tools-2.5.5/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.5.5/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.5.5/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/member_auth.sql` & `aegis-tools-2.5.5/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.5.5/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/sql/reports.sql` & `aegis-tools-2.5.5/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/stdlib.py` & `aegis-tools-2.5.5/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/build.html` & `aegis-tools-2.5.5/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/build_confirm.html` & `aegis-tools-2.5.5/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/build_form.html` & `aegis-tools-2.5.5/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/build_view.html` & `aegis-tools-2.5.5/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/frame.html` & `aegis-tools-2.5.5/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/hydra.html` & `aegis-tools-2.5.5/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/hydra_form.html` & `aegis-tools-2.5.5/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/hydra_queue.html` & `aegis-tools-2.5.5/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/report.html` & `aegis-tools-2.5.5/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/report_form.html` & `aegis-tools-2.5.5/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/reports.html` & `aegis-tools-2.5.5/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/templates/w3.css` & `aegis-tools-2.5.5/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/threadpool.py` & `aegis-tools-2.5.5/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/aegis/webapp.py` & `aegis-tools-2.5.5/aegis/webapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         if self.tmpl.get('session_ck', {}).get('audit_session_id'):
             audit_session_id = self.tmpl['session_ck']['audit_session_id']
             audit_session_row = aegis.model.AuditSession.get_id(audit_session_id, dbconn=self.dbconn)
         if audit_session_row:
             self.audit_session['last_request_name'] = self.tmpl['request_name']
             self.audit_session['last_request_dttm'] = aegis.database.Literal('NOW()')
             if aegis.database.mysql_available:
-                self.audit_session['session_time'] = aegis.database.Literal('UNIX_TIMESTAMP(NOW()) - UNIX_TIMESTAMP(created_dttm)')
+                self.audit_session['session_time'] = aegis.database.Literal('UNIX_TIMESTAMP(NOW()) - UNIX_TIMESTAMP(create_dttm)')
             elif aegis.database.pgsql_available:
                 self.audit_session['session_time'] = aegis.database.Literal('EXTRACT(EPOCH FROM NOW()) - EXTRACT(EPOCH FROM create_dttm)')
             self.audit_session['request_cnt'] = aegis.database.Literal('request_cnt+1')
             self.audit_request['request_nbr'] = audit_session_row['request_cnt'] + 1
             self.audit_session['marketing_id'] = audit_session_row['marketing_id']
         else:
             self.audit_session['marketing_id'] = aegis.stdlib.validate_int(self.get_marketing_id())
```

### Comparing `aegis-tools-2.5.4/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.5.5/aegis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.4
+Version: 2.5.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.4/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.5.5/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.4/setup.py` & `aegis-tools-2.5.5/setup.py`

 * *Files identical despite different names*

