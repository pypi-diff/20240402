# Comparing `tmp/awslogs-0.7.0.tar.gz` & `tmp/awslogs-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awslogs-0.7.0.tar", last modified: Sat Sep 10 08:37:37 2016, max compression
+gzip compressed data, was "dist/awslogs-0.8.0.tar", last modified: Fri Jan 13 11:30:43 2017, max compression
```

## Comparing `awslogs-0.7.0.tar` & `awslogs-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2016-09-10 08:37:37.000000 awslogs-0.7.0/
--rw-r--r--   0 neo        (501) staff       (20)      525 2016-09-10 07:46:46.000000 awslogs-0.7.0/AUTHORS
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2016-09-10 08:37:37.000000 awslogs-0.7.0/awslogs/
--rw-r--r--   0 neo        (501) staff       (20)       76 2016-03-27 10:24:52.000000 awslogs-0.7.0/awslogs/__init__.py
--rw-r--r--   0 neo        (501) staff       (20)       94 2016-03-27 10:24:52.000000 awslogs-0.7.0/awslogs/_version.py
--rw-r--r--   0 neo        (501) staff       (20)     7716 2016-09-10 08:17:41.000000 awslogs-0.7.0/awslogs/bin.py
--rw-r--r--   0 neo        (501) staff       (20)     9949 2016-09-10 08:17:41.000000 awslogs-0.7.0/awslogs/core.py
--rw-r--r--   0 neo        (501) staff       (20)      846 2016-03-27 10:31:07.000000 awslogs-0.7.0/awslogs/exceptions.py
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2016-09-10 08:37:37.000000 awslogs-0.7.0/awslogs.egg-info/
--rw-r--r--   0 neo        (501) staff       (20)        1 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/dependency_links.txt
--rw-r--r--   0 neo        (501) staff       (20)       46 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/entry_points.txt
--rw-r--r--   0 neo        (501) staff       (20)        1 2015-10-29 21:32:15.000000 awslogs-0.7.0/awslogs.egg-info/not-zip-safe
--rw-r--r--   0 neo        (501) staff       (20)       47 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/pbr.json
--rw-r--r--   0 neo        (501) staff       (20)      726 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/PKG-INFO
--rw-r--r--   0 neo        (501) staff       (20)      130 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/requires.txt
--rw-r--r--   0 neo        (501) staff       (20)      404 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/SOURCES.txt
--rw-r--r--   0 neo        (501) staff       (20)        8 2016-09-10 08:37:36.000000 awslogs-0.7.0/awslogs.egg-info/top_level.txt
--rw-r--r--   0 neo        (501) staff       (20)     2542 2016-09-10 08:19:04.000000 awslogs-0.7.0/CHANGELOG
--rw-r--r--   0 neo        (501) staff       (20)     1529 2016-01-28 22:43:57.000000 awslogs-0.7.0/COPYING
--rw-r--r--   0 neo        (501) staff       (20)       67 2016-03-27 09:15:25.000000 awslogs-0.7.0/MANIFEST.in
--rw-r--r--   0 neo        (501) staff       (20)      726 2016-09-10 08:37:37.000000 awslogs-0.7.0/PKG-INFO
--rw-r--r--   0 neo        (501) staff       (20)     6174 2016-09-10 08:37:17.000000 awslogs-0.7.0/README.rst
--rw-r--r--   0 neo        (501) staff       (20)       88 2016-09-10 08:37:37.000000 awslogs-0.7.0/setup.cfg
--rw-r--r--   0 neo        (501) staff       (20)     1498 2016-09-10 08:17:41.000000 awslogs-0.7.0/setup.py
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2017-01-13 11:30:43.000000 awslogs-0.8.0/
+-rw-r--r--   0 neo        (501) staff       (20)      525 2016-09-10 07:46:46.000000 awslogs-0.8.0/AUTHORS
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs/
+-rw-r--r--   0 neo        (501) staff       (20)       76 2016-03-27 10:24:52.000000 awslogs-0.8.0/awslogs/__init__.py
+-rw-r--r--   0 neo        (501) staff       (20)       94 2016-03-27 10:24:52.000000 awslogs-0.8.0/awslogs/_version.py
+-rw-r--r--   0 neo        (501) staff       (20)     7986 2017-01-13 10:57:18.000000 awslogs-0.8.0/awslogs/bin.py
+-rw-r--r--   0 neo        (501) staff       (20)    10161 2017-01-13 10:57:18.000000 awslogs-0.8.0/awslogs/core.py
+-rw-r--r--   0 neo        (501) staff       (20)      846 2016-03-27 10:31:07.000000 awslogs-0.8.0/awslogs/exceptions.py
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/
+-rw-r--r--   0 neo        (501) staff       (20)        1 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/dependency_links.txt
+-rw-r--r--   0 neo        (501) staff       (20)       46 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/entry_points.txt
+-rw-r--r--   0 neo        (501) staff       (20)        1 2015-10-29 21:32:15.000000 awslogs-0.8.0/awslogs.egg-info/not-zip-safe
+-rw-r--r--   0 neo        (501) staff       (20)       46 2016-09-25 13:15:24.000000 awslogs-0.8.0/awslogs.egg-info/pbr.json
+-rw-r--r--   0 neo        (501) staff       (20)      726 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/PKG-INFO
+-rw-r--r--   0 neo        (501) staff       (20)      130 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/requires.txt
+-rw-r--r--   0 neo        (501) staff       (20)      404 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/SOURCES.txt
+-rw-r--r--   0 neo        (501) staff       (20)        8 2017-01-13 11:30:43.000000 awslogs-0.8.0/awslogs.egg-info/top_level.txt
+-rw-r--r--   0 neo        (501) staff       (20)     2663 2017-01-13 10:58:56.000000 awslogs-0.8.0/CHANGELOG
+-rw-r--r--   0 neo        (501) staff       (20)     1529 2016-01-28 22:43:57.000000 awslogs-0.8.0/COPYING
+-rw-r--r--   0 neo        (501) staff       (20)       67 2016-03-27 09:15:25.000000 awslogs-0.8.0/MANIFEST.in
+-rw-r--r--   0 neo        (501) staff       (20)      726 2017-01-13 11:30:43.000000 awslogs-0.8.0/PKG-INFO
+-rw-r--r--   0 neo        (501) staff       (20)     6174 2016-09-10 08:37:17.000000 awslogs-0.8.0/README.rst
+-rw-r--r--   0 neo        (501) staff       (20)       88 2017-01-13 11:30:43.000000 awslogs-0.8.0/setup.cfg
+-rw-r--r--   0 neo        (501) staff       (20)     1498 2017-01-13 10:57:38.000000 awslogs-0.8.0/setup.py
```

### Comparing `awslogs-0.7.0/AUTHORS` & `awslogs-0.8.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `awslogs-0.7.0/awslogs/bin.py` & `awslogs-0.8.0/awslogs/bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,20 @@
                             help="JMESPath query to use in filtering the response data")
 
     # groups
     groups_parser = subparsers.add_parser('groups', description='List groups')
     groups_parser.set_defaults(func="list_groups")
     add_common_arguments(groups_parser)
 
+    groups_parser.add_argument("-p",
+                               "--log-group-prefix",
+                               action="store",
+                               dest="log_group_prefix",
+                               help="List only groups matching the prefix")
+
     # streams
     streams_parser = subparsers.add_parser('streams', description='List streams')
     streams_parser.set_defaults(func="list_streams")
     add_common_arguments(streams_parser)
     add_date_range_arguments(streams_parser)
 
     streams_parser.add_argument("log_group_name",
```

### Comparing `awslogs-0.7.0/awslogs/core.py` & `awslogs-0.8.0/awslogs/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.output_ingestion_time_enabled = kwargs.get(
             'output_ingestion_time_enabled')
         self.start = self.parse_datetime(kwargs.get('start'))
         self.end = self.parse_datetime(kwargs.get('end'))
         self.query = kwargs.get('query')
         if self.query is not None:
             self.query_expression = jmespath.compile(self.query)
-
+        self.log_group_prefix = kwargs.get('log_group_prefix')
         self.client = boto3.client(
             'logs',
             aws_access_key_id=self.aws_access_key_id,
             aws_secret_access_key=self.aws_secret_access_key,
             aws_session_token=self.aws_session_token,
             region_name=self.aws_region
         )
@@ -175,15 +175,15 @@
 
                 message = event['message']
                 if self.query is not None and message[0] == '{':
                     parsed = json.loads(event['message'])
                     message = self.query_expression.search(parsed)
                     if not isinstance(message, six.string_types):
                         message = json.dumps(message)
-                output.append(message)
+                output.append(message.rstrip())
 
                 print(' '.join(output))
                 sys.stdout.flush()
         try:
             consumer()
         except KeyboardInterrupt:
             print('Closing...\n')
@@ -197,16 +197,19 @@
     def list_streams(self):
         """Lists available CloudWatch logs streams in ``log_group_name``."""
         for stream in self.get_streams():
             print(stream)
 
     def get_groups(self):
         """Returns available CloudWatch logs groups"""
+        kwargs = {}
+        if self.log_group_prefix is not None:
+            kwargs = {'logGroupNamePrefix': self.log_group_prefix}
         paginator = self.client.get_paginator('describe_log_groups')
-        for page in paginator.paginate():
+        for page in paginator.paginate(**kwargs):
             for group in page.get('logGroups', []):
                 yield group['logGroupName']
 
     def get_streams(self, log_group_name=None):
         """Returns available CloudWatch logs streams in ``log_group_name``."""
         kwargs = {'logGroupName': log_group_name or self.log_group_name}
         window_start = self.start or 0
```

### Comparing `awslogs-0.7.0/awslogs/exceptions.py` & `awslogs-0.8.0/awslogs/exceptions.py`

 * *Files identical despite different names*

### Comparing `awslogs-0.7.0/awslogs.egg-info/PKG-INFO` & `awslogs-0.8.0/awslogs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awslogs
-Version: 0.7.0
+Version: 0.8.0
 Summary: awslogs is a simple command line tool to read aws cloudwatch logs.
 Home-page: https://github.com/jorgebastida/awslogs
 Author: Jorge Bastida
 Author-email: me@jorgebastida.com
 License: BSD
 Description: awslogs is a simple command line tool to read aws cloudwatch logs.
 Keywords: aws logs cloudwatch
```

### Comparing `awslogs-0.7.0/CHANGELOG` & `awslogs-0.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.8.0
+=====
+- New: ``--log-group-prefix``, ``-p`` option to filter groups.
+- Fix: Remove extra newline after each line.
+
 0.7.0
 =====
 - Improve documentation (Thanks Pietro Di Bello)
 - Make it possible to use timezoned timestamps as input for ``-start`` and ``-end`` (Thanks Samuel Cochran)
 - New: ``--query`` will now accept a JMESPath query which will filter the response data (Thanks Samuel Cochran)
 
 0.6.0
```

### Comparing `awslogs-0.7.0/COPYING` & `awslogs-0.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `awslogs-0.7.0/PKG-INFO` & `awslogs-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awslogs
-Version: 0.7.0
+Version: 0.8.0
 Summary: awslogs is a simple command line tool to read aws cloudwatch logs.
 Home-page: https://github.com/jorgebastida/awslogs
 Author: Jorge Bastida
 Author-email: me@jorgebastida.com
 License: BSD
 Description: awslogs is a simple command line tool to read aws cloudwatch logs.
 Keywords: aws logs cloudwatch
```

### Comparing `awslogs-0.7.0/README.rst` & `awslogs-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `awslogs-0.7.0/setup.py` & `awslogs-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 if 'bdist_wheel' not in sys.argv and sys.version_info < (2, 7):
     install_requires.append('argparse>1.1.0')
 
 
 setup(
     name='awslogs',
-    version='0.7.0',
+    version='0.8.0',
     url='https://github.com/jorgebastida/awslogs',
     license='BSD',
     author='Jorge Bastida',
     author_email='me@jorgebastida.com',
     description='awslogs is a simple command line tool to read aws cloudwatch logs.',
     long_description='awslogs is a simple command line tool to read aws cloudwatch logs.',
     keywords="aws logs cloudwatch",
```

