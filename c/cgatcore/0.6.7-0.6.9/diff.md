# Comparing `tmp/cgatcore-0.6.7.tar.gz` & `tmp/cgatcore-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cgatcore-0.6.7.tar", last modified: Wed Jul 29 06:02:55 2020, max compression
+gzip compressed data, was "dist/cgatcore-0.6.9.tar", last modified: Sun Oct 17 20:19:12 2021, max compression
```

## Comparing `cgatcore-0.6.7.tar` & `cgatcore-0.6.9.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/cgatcore/
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     4800 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/logfile.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    45642 2019-05-25 09:05:25.000000 cgatcore-0.6.7/cgatcore/experiment.pyc
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    42673 2019-05-25 09:05:25.000000 cgatcore-0.6.7/cgatcore/iotools.pyc
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    21187 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/tables.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    38484 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/iotools.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    11352 2020-06-14 09:42:24.000000 cgatcore-0.6.7/cgatcore/csv2db.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     9186 2020-07-27 11:17:04.000000 cgatcore-0.6.7/cgatcore/database.py
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/cgatcore/remote/
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     3801 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/ftp.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     4535 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/azure.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     4006 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/aws.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      597 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/__init__.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     2576 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/sftp.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     3917 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/remote/google_cloud.py
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/cgatcore/pipeline/
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    22163 2020-07-27 11:17:04.000000 cgatcore-0.6.7/cgatcore/pipeline/cluster.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      332 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/wrappers.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    47108 2020-07-27 11:17:04.000000 cgatcore-0.6.7/cgatcore/pipeline/execution.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    18613 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/parameters.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    19917 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/database.py
--rwxrwxr-x   0 adamc     (1399) usersfgu  (1000)    27075 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/farm.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     4254 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/run_function.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     4449 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/pipeline/files.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     2746 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/pipeline/utils.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    14137 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/pipeline/__init__.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    52339 2019-12-09 09:11:34.000000 cgatcore-0.6.7/cgatcore/pipeline/control.py
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/cgatcore/pipeline/logstash_formatter/
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     5921 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/pipeline/logstash_formatter/__init__.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    60597 2019-11-20 09:24:09.000000 cgatcore-0.6.7/cgatcore/experiment.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)       22 2020-07-29 06:02:47.000000 cgatcore-0.6.7/cgatcore/version.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)        0 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/__init__.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      150 2019-05-25 09:05:25.000000 cgatcore-0.6.7/cgatcore/__init__.pyc
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     9337 2018-12-10 17:09:09.000000 cgatcore-0.6.7/cgatcore/csvutils.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)    26586 2020-01-09 09:57:11.000000 cgatcore-0.6.7/cgatcore/table.py
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     3189 2019-04-25 08:14:13.000000 cgatcore-0.6.7/README.md
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     1072 2019-02-13 10:22:12.000000 cgatcore-0.6.7/LICENSE
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)       14 2018-12-10 17:09:09.000000 cgatcore-0.6.7/KNOWN_BUGS
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      176 2018-12-10 17:09:09.000000 cgatcore-0.6.7/INSTALL
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      273 2018-12-10 17:09:09.000000 cgatcore-0.6.7/THANKS.txt
-drwxrwxr-x   0 adamc     (1399) usersfgu  (1000)        0 2020-07-29 06:02:55.000000 cgatcore-0.6.7/cgatcore.egg-info/
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)        1 2019-01-30 09:19:06.000000 cgatcore-0.6.7/cgatcore.egg-info/not-zip-safe
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     1035 2020-07-29 06:02:54.000000 cgatcore-0.6.7/cgatcore.egg-info/SOURCES.txt
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)        9 2020-07-29 06:02:54.000000 cgatcore-0.6.7/cgatcore.egg-info/top_level.txt
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)        1 2020-07-29 06:02:54.000000 cgatcore-0.6.7/cgatcore.egg-info/dependency_links.txt
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      772 2020-07-29 06:02:54.000000 cgatcore-0.6.7/cgatcore.egg-info/PKG-INFO
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      358 2018-12-10 17:09:09.000000 cgatcore-0.6.7/MANIFEST.in
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)       77 2020-07-29 06:02:55.000000 cgatcore-0.6.7/setup.cfg
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)      772 2020-07-29 06:02:55.000000 cgatcore-0.6.7/PKG-INFO
--rw-rw-r--   0 adamc     (1399) usersfgu  (1000)     2292 2019-11-20 09:24:09.000000 cgatcore-0.6.7/setup.py
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.594062 cgatcore-0.6.9/
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)      176 2021-05-06 07:23:02.000000 cgatcore-0.6.9/INSTALL
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)       14 2021-05-06 07:23:02.000000 cgatcore-0.6.9/KNOWN_BUGS
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     1072 2021-05-06 07:23:02.000000 cgatcore-0.6.9/LICENSE
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)      358 2021-05-06 07:23:01.000000 cgatcore-0.6.9/MANIFEST.in
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)      772 2021-10-17 20:19:12.595063 cgatcore-0.6.9/PKG-INFO
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     3189 2021-05-06 07:23:02.000000 cgatcore-0.6.9/README.md
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)      273 2021-05-06 07:23:02.000000 cgatcore-0.6.9/THANKS.txt
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.551060 cgatcore-0.6.9/cgatcore/
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)        0 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/__init__.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    11352 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/csv2db.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     9337 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/csvutils.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     9186 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/database.py
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)    60618 2021-10-17 20:03:17.000000 cgatcore-0.6.9/cgatcore/experiment.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    38484 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/iotools.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     4800 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/logfile.py
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.583062 cgatcore-0.6.9/cgatcore/pipeline/
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    14137 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/__init__.py
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)    22172 2021-10-17 20:03:17.000000 cgatcore-0.6.9/cgatcore/pipeline/cluster.py
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)    52348 2021-10-17 20:03:17.000000 cgatcore-0.6.9/cgatcore/pipeline/control.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    19917 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/database.py
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)    48233 2021-10-17 20:03:17.000000 cgatcore-0.6.9/cgatcore/pipeline/execution.py
+-rwxr-x---   0 acribbs  (20008) acribbsgrp (20008)    27075 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/farm.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     4449 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/files.py
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.584062 cgatcore-0.6.9/cgatcore/pipeline/logstash_formatter/
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     5921 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/logstash_formatter/__init__.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    18613 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/parameters.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     4254 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/run_function.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     2746 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/utils.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)      332 2021-05-06 07:23:02.000000 cgatcore-0.6.9/cgatcore/pipeline/wrappers.py
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.593062 cgatcore-0.6.9/cgatcore/remote/
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)      597 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/__init__.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     4006 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/aws.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     4535 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/azure.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     3801 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/ftp.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     3917 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/google_cloud.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     2576 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/remote/sftp.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    26586 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/table.py
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)    21187 2021-05-06 07:23:01.000000 cgatcore-0.6.9/cgatcore/tables.py
+-rw-rw-r--   0 acribbs  (20008) acribbsgrp (20008)       22 2021-10-17 20:16:33.000000 cgatcore-0.6.9/cgatcore/version.py
+drwxrwxr-x   0 acribbs  (20008) acribbsgrp (20008)        0 2021-10-17 20:19:12.558060 cgatcore-0.6.9/cgatcore.egg-info/
+-rw-r--r--   0 acribbs  (20008) acribbsgrp (20008)      772 2021-10-17 20:19:12.000000 cgatcore-0.6.9/cgatcore.egg-info/PKG-INFO
+-rw-r--r--   0 acribbs  (20008) acribbsgrp (20008)      968 2021-10-17 20:19:12.000000 cgatcore-0.6.9/cgatcore.egg-info/SOURCES.txt
+-rw-r--r--   0 acribbs  (20008) acribbsgrp (20008)        1 2021-10-17 20:19:12.000000 cgatcore-0.6.9/cgatcore.egg-info/dependency_links.txt
+-rw-r--r--   0 acribbs  (20008) acribbsgrp (20008)        1 2021-05-06 07:49:46.000000 cgatcore-0.6.9/cgatcore.egg-info/not-zip-safe
+-rw-r--r--   0 acribbs  (20008) acribbsgrp (20008)        9 2021-10-17 20:19:12.000000 cgatcore-0.6.9/cgatcore.egg-info/top_level.txt
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)       77 2021-10-17 20:19:12.596063 cgatcore-0.6.9/setup.cfg
+-rw-r-----   0 acribbs  (20008) acribbsgrp (20008)     2292 2021-05-06 07:23:02.000000 cgatcore-0.6.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cgatcore-0.6.7/cgatcore/logfile.py` & `cgatcore-0.6.9/cgatcore/logfile.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/tables.py` & `cgatcore-0.6.9/cgatcore/tables.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/iotools.py` & `cgatcore-0.6.9/cgatcore/iotools.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/csv2db.py` & `cgatcore-0.6.9/cgatcore/csv2db.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/database.py` & `cgatcore-0.6.9/cgatcore/database.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/ftp.py` & `cgatcore-0.6.9/cgatcore/remote/ftp.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/azure.py` & `cgatcore-0.6.9/cgatcore/remote/azure.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/aws.py` & `cgatcore-0.6.9/cgatcore/remote/aws.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/__init__.py` & `cgatcore-0.6.9/cgatcore/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/sftp.py` & `cgatcore-0.6.9/cgatcore/remote/sftp.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/remote/google_cloud.py` & `cgatcore-0.6.9/cgatcore/remote/google_cloud.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/cluster.py` & `cgatcore-0.6.9/cgatcore/pipeline/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime
 import logging
 import gevent
 import cgatcore.experiment as E
 
 try:
     import drmaa
-except (ImportError, RuntimeError):
+except (ImportError, RuntimeError, OSError):
     pass
 
 
 def get_logger():
     return logging.getLogger("cgatcore.pipeline")
```

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/execution.py` & `cgatcore-0.6.9/cgatcore/pipeline/execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from cgatcore.pipeline.parameters import substitute_parameters, get_params
 from cgatcore.pipeline.cluster import get_queue_manager, JobInfo
 
 # talking to a cluster
 try:
     import drmaa
     HAS_DRMAA = True
-except (ImportError, RuntimeError):
+except (ImportError, RuntimeError, OSError):
     HAS_DRMAA = False
 
 # global drmaa session
 GLOBAL_SESSION = None
 
 # Timeouts for event loop
 GEVENT_TIMEOUT_STARTUP = 5
@@ -189,16 +189,24 @@
             continue
         parts = re.split(" +", line)
         if len(parts) == 2:
             env_map[parts[0]] = parts[1]
         elif len(parts) == 3:
             env_map[parts[0]] = parts[2]
     if env_name not in env_map:
+
+        # IMS: conda envs can be located at abitrary locations, and not be
+        # registered with conda. NB this can't tellif the directory contains a
+        # valid env.
+        if os.path.exists(env_name) and os.path.isdir(env_name):
+            return(env_name)
+
         raise IOError("conda environment {} does not exist, found {}".format(
             env_name, sorted(env_map.keys())))
+
     return env_map[env_name]
 
 
 def execute(statement, **kwargs):
     '''execute a statement locally.
 
     This method implements the same parameter interpolation
@@ -439,14 +447,23 @@
 
         self.shellfile = kwargs.get("shell_logfile", None)
         if self.shellfile:
             if not self.shellfile.startswith(os.sep):
                 self.shellfile = os.path.join(
                     self.work_dir, os.path.basename(self.shellfile))
 
+        self.monitor_interval_queued = kwargs.get('monitor_interval_queued', None)
+        if self.monitor_interval_queued is None:
+            self.monitor_interval_queued = get_params()["cluster"].get(
+                'monitor_interval_queued_default', GEVENT_TIMEOUT_WAIT)
+        self.monitor_interval_running = kwargs.get('monitor_interval_running', None)
+        if self.monitor_interval_running is None:
+            self.monitor_interval_running = get_params()["cluster"].get(
+                'monitor_interval_running_default', GEVENT_TIMEOUT_WAIT)
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
 
     def expand_statement(self, statement):
@@ -830,16 +847,20 @@
         self.logger.info("waiting for %i jobs to finish " % len(job_ids))
         running_job_ids = set(job_ids)
         while running_job_ids:
             for job_id in list(running_job_ids):
                 status = self.session.jobStatus(job_id)
                 if status in (drmaa.JobState.DONE, drmaa.JobState.FAILED):
                     running_job_ids.remove(job_id)
+                if status in (drmaa.JobState.RUNNING):
+                    # The drmaa documentation is unclear as to what gets returned
+                    # for a job array when tasks can be in different states
+                    gevent.sleep(self.monitor_interval_running)
                 else:
-                    gevent.sleep(GEVENT_TIMEOUT_WAIT)
+                    gevent.sleep(self.monitor_interval_queued)
                     break
 
 
 class GridArrayExecutor(GridExecutor):
 
     def run(self, statement_list):
```

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/parameters.py` & `cgatcore-0.6.9/cgatcore/pipeline/parameters.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/database.py` & `cgatcore-0.6.9/cgatcore/pipeline/database.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/farm.py` & `cgatcore-0.6.9/cgatcore/pipeline/farm.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/run_function.py` & `cgatcore-0.6.9/cgatcore/pipeline/run_function.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/files.py` & `cgatcore-0.6.9/cgatcore/pipeline/files.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/utils.py` & `cgatcore-0.6.9/cgatcore/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/__init__.py` & `cgatcore-0.6.9/cgatcore/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/control.py` & `cgatcore-0.6.9/cgatcore/pipeline/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 import ruffus
 
 # talking to a cluster
 try:
     import drmaa
     HAS_DRMAA = True
-except (ImportError, RuntimeError):
+except (ImportError, RuntimeError, OSError):
     HAS_DRMAA = False
 
 import cgatcore.experiment as E
 import cgatcore.iotools as iotools
 from cgatcore.pipeline.parameters import input_validation, get_params, get_parameters
 from cgatcore.pipeline.utils import get_caller, get_caller_locals, is_test
 from cgatcore.pipeline.execution import execute, start_session,\
```

### Comparing `cgatcore-0.6.7/cgatcore/pipeline/logstash_formatter/__init__.py` & `cgatcore-0.6.9/cgatcore/pipeline/logstash_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/experiment.py` & `cgatcore-0.6.9/cgatcore/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 import textwrap
 import random
 import uuid
 import yaml
 # import convenience functions from logging
 import logging
 import logging.config
-from logging import warning, info, log, debug, error, critical
+from logging import warning, info, log, debug, error, critical, exception
 from logging import warning as warn
 
 
 class DefaultOptions:
     stdlog = sys.stdout
     stdout = sys.stdout
     stderr = sys.stderr
@@ -1006,15 +1006,15 @@
                 global_options.log_config_filename):
             global_options.log_config_filename = None
 
         if global_options.log_config_filename:
             if os.path.exists(global_options.log_config_filename):
                 # configure logging from filename
                 with open(global_options.log_config_filename) as inf:
-                    dict_yaml = yaml.load(inf)
+                    dict_yaml = yaml.safe_load(inf)
                 logging.config.dictConfig(dict_yaml)
             else:
                 raise OSError("file {} with logging configuration does not exist".format(
                     global_options.log_config_filename))
         else:
             # configure logging from command line options
             # map from 0-10 to logging scale
@@ -1238,15 +1238,15 @@
                 global_args.log_config_filename):
             global_args.log_config_filename = None
 
         if global_args.log_config_filename:
             if os.path.exists(global_args.log_config_filename):
                 # configure logging from filename
                 with open(global_args.log_config_filename) as inf:
-                    dict_yaml = yaml.load(inf)
+                    dict_yaml = yaml.safe_load(inf)
                 logging.config.dictConfig(dict_yaml)
             else:
                 raise OSError("file {} with logging configuration does not exist".format(
                     global_args.log_config_filename))
         else:
             # configure logging from command line options
             # map from 0-10 to logging scale
```

### Comparing `cgatcore-0.6.7/cgatcore/csvutils.py` & `cgatcore-0.6.9/cgatcore/csvutils.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore/table.py` & `cgatcore-0.6.9/cgatcore/table.py`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/README.md` & `cgatcore-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/LICENSE` & `cgatcore-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cgatcore-0.6.7/cgatcore.egg-info/SOURCES.txt` & `cgatcore-0.6.9/cgatcore.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 LICENSE
 MANIFEST.in
 README.md
 THANKS.txt
 setup.cfg
 setup.py
 cgatcore/__init__.py
-cgatcore/__init__.pyc
 cgatcore/csv2db.py
 cgatcore/csvutils.py
 cgatcore/database.py
 cgatcore/experiment.py
-cgatcore/experiment.pyc
 cgatcore/iotools.py
-cgatcore/iotools.pyc
 cgatcore/logfile.py
 cgatcore/table.py
 cgatcore/tables.py
 cgatcore/version.py
 cgatcore.egg-info/PKG-INFO
 cgatcore.egg-info/SOURCES.txt
 cgatcore.egg-info/dependency_links.txt
```

### Comparing `cgatcore-0.6.7/cgatcore.egg-info/PKG-INFO` & `cgatcore-0.6.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cgatcore
-Version: 0.6.7
+Version: 0.6.9
 Summary: cgatcore : the Computational Genomics Analysis Toolkit
 Home-page: https://github.com/cgat-developers/cgat-core
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Description: CGAT : the Computational Genomics Analysis Toolkit
 Keywords: computational genomics
```

### Comparing `cgatcore-0.6.7/PKG-INFO` & `cgatcore-0.6.9/cgatcore.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cgatcore
-Version: 0.6.7
+Version: 0.6.9
 Summary: cgatcore : the Computational Genomics Analysis Toolkit
 Home-page: https://github.com/cgat-developers/cgat-core
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Description: CGAT : the Computational Genomics Analysis Toolkit
 Keywords: computational genomics
```

### Comparing `cgatcore-0.6.7/setup.py` & `cgatcore-0.6.9/setup.py`

 * *Files identical despite different names*

