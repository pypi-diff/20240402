# Comparing `tmp/messagev-0.0.7.tar.gz` & `tmp/messagev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messagev-0.0.7.tar", last modified: Fri Mar 25 05:51:55 2022, max compression
+gzip compressed data, was "messagev-0.0.8.tar", last modified: Fri Apr  1 22:15:21 2022, max compression
```

## Comparing `messagev-0.0.7.tar` & `messagev-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 05:51:55.299386 messagev-0.0.7/
--rw-r--r--   0 root         (0) root         (0)      711 2022-03-25 05:51:55.299386 messagev-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-03-24 15:13:30.000000 messagev-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 05:51:55.299386 messagev-0.0.7/messagev/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-03-25 05:51:26.000000 messagev-0.0.7/messagev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2022-03-24 15:13:30.000000 messagev-0.0.7/messagev/auth_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     8596 2022-03-24 15:13:30.000000 messagev-0.0.7/messagev/base_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5881 2022-03-24 15:13:30.000000 messagev-0.0.7/messagev/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    41846 2022-03-25 05:49:28.000000 messagev-0.0.7/messagev/config_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 05:51:55.299386 messagev-0.0.7/messagev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      711 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      328 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-03-25 05:51:55.000000 messagev-0.0.7/messagev.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-03-25 05:51:55.299386 messagev-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-25 05:51:26.000000 messagev-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 22:15:21.460412 messagev-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      711 2022-04-01 22:15:21.460412 messagev-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       82 2022-04-01 21:59:04.000000 messagev-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 22:15:21.460412 messagev-0.0.8/messagev/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-04-01 22:14:10.000000 messagev-0.0.8/messagev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2022-04-01 22:15:18.000000 messagev-0.0.8/messagev/auth_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8596 2022-04-01 22:15:18.000000 messagev-0.0.8/messagev/base_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5881 2022-04-01 22:15:18.000000 messagev-0.0.8/messagev/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    47943 2022-04-01 22:15:18.000000 messagev-0.0.8/messagev/config_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 22:15:21.460412 messagev-0.0.8/messagev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      711 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      328 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-04-01 22:15:21.000000 messagev-0.0.8/messagev.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2022-04-01 22:15:21.460412 messagev-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2022-04-01 22:14:10.000000 messagev-0.0.8/setup.py
```

### Comparing `messagev-0.0.7/PKG-INFO` & `messagev-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: messagev
-Version: 0.0.7
+Version: 0.0.8
 Summary: MessageV: the python files generated for consuming the Orchest API
 Home-page: UNKNOWN
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Description: # MessageV
```

### Comparing `messagev-0.0.7/messagev/auth_pb2.py` & `messagev-0.0.8/messagev/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `messagev-0.0.7/messagev/base_pb2.py` & `messagev-0.0.8/messagev/base_pb2.py`

 * *Files identical despite different names*

### Comparing `messagev-0.0.7/messagev/command_pb2.py` & `messagev-0.0.8/messagev/command_pb2.py`

 * *Files identical despite different names*

### Comparing `messagev-0.0.7/messagev/config_pb2.py` & `messagev-0.0.8/messagev/config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,79 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='config.proto',
   package='messagev.deployv',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0c\x63onfig.proto\x12\x10messagev.deployv\"\x97\x03\n\x06\x43onfig\x12(\n\x06\x63ommon\x18\x01 \x01(\x0b\x32\x18.messagev.deployv.Common\x12:\n\tcustomers\x18\x02 \x03(\x0b\x32\'.messagev.deployv.Config.CustomersEntry\x12,\n\nserver_cfg\x18\x03 \x01(\x0b\x32\x18.messagev.deployv.Server\x12&\n\x05\x62trfs\x18\x04 \x01(\x0b\x32\x17.messagev.deployv.Btrfs\x12\"\n\x03zfs\x18\x05 \x01(\x0b\x32\x15.messagev.deployv.Zfs\x12,\n\x08\x64\x61tabase\x18\x06 \x01(\x0b\x32\x1a.messagev.deployv.Database\x12(\n\x06\x61lerts\x18\x07 \x01(\x0b\x32\x18.messagev.deployv.Alerts\x1aU\n\x0e\x43ustomersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.messagev.deployv.CustomerInstances:\x02\x38\x01\"\xdf\x01\n\x06\x43ommon\x12\x10\n\x08work_dir\x18\x01 \x01(\t\x12\x12\n\nbackup_src\x18\x02 \x01(\t\x12\x13\n\x0b\x63onfig_file\x18\x03 \x01(\t\x12\x0c\n\x04jobs\x18\x04 \x01(\x05\x12\x10\n\x08password\x18\x05 \x01(\t\x12\x36\n\rs3_credential\x18\x06 \x01(\x0b\x32\x1f.messagev.deployv.S3Credentials\x12\r\n\x05no_fs\x18\x07 \x01(\x08\x12\x0e\n\x06no_cpt\x18\x08 \x01(\x08\x12\x10\n\x08log_file\x18\t \x01(\t\x12\x11\n\tlog_level\x18\n \x01(\t\"h\n\rS3Credentials\x12\x10\n\x08\x45ndPoint\x18\x01 \x01(\t\x12\x10\n\x08\x43lientID\x18\x02 \x01(\t\x12\x11\n\tSecretKey\x18\x03 \x01(\t\x12\x10\n\x08Insecure\x18\x04 \x01(\x08\x12\x0e\n\x06Region\x18\x05 \x01(\t\"t\n\x11\x43ustomerInstances\x12\x35\n\tinstances\x18\x01 \x03(\x0b\x32\".messagev.deployv.CustomerInstance\x12(\n\x06restic\x18\x02 \x01(\x0b\x32\x18.messagev.deployv.Restic\"z\n\x10\x43ustomerInstance\x12\x13\n\x0b\x63ustomer_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nconfigFile\x18\x03 \x01(\t\x12\x0c\n\x04jobs\x18\x04 \x01(\x05\x12\r\n\x05no_fs\x18\x05 \x01(\x08\x12\x0e\n\x06no_cpt\x18\x06 \x01(\x08\"\x18\n\x06Server\x12\x0e\n\x06listen\x18\x01 \x01(\t\"y\n\x05\x42trfs\x12\x11\n\tbase_path\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x62_storage_path\x18\x02 \x01(\t\x12\x17\n\x0f\x66s_storage_path\x18\x03 \x01(\t\x12\x12\n\ndb_version\x18\x04 \x01(\t\x12\x17\n\x0f\x64\x62_version_read\x18\x05 \x01(\x08\"z\n\x03Zfs\x12\x14\n\x0c\x62\x61se_dataset\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x62_storage_path\x18\x02 \x01(\t\x12\x17\n\x0f\x66s_storage_path\x18\x03 \x01(\t\x12\x12\n\ndb_version\x18\x04 \x01(\t\x12\x17\n\x0f\x64\x62_version_read\x18\x05 \x01(\x08\"C\n\x08\x44\x61tabase\x12\x11\n\tpsql_repo\x18\x01 \x01(\t\x12\x10\n\x08psql_tag\x18\x02 \x01(\t\x12\x12\n\nadmin_pass\x18\x03 \x01(\t\"B\n\x0eGitlabIncident\x12\x10\n\x08repo_url\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x0f\n\x07node_id\x18\x03 \x01(\t\"C\n\x06\x41lerts\x12\x39\n\x0fgitlab_incident\x18\x01 \x01(\x0b\x32 .messagev.deployv.GitlabIncident\"\x94\x02\n\x06Restic\x12\x12\n\nrepository\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0e\n\x06htpass\x18\x03 \x01(\t\x12:\n\tvariables\x18\x04 \x03(\x0b\x32\'.messagev.deployv.Restic.VariablesEntry\x12\x36\n\x07options\x18\x05 \x03(\x0b\x32%.messagev.deployv.Restic.OptionsEntry\x1a\x30\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3'
+  serialized_pb=b'\n\x0c\x63onfig.proto\x12\x10messagev.deployv\"\x97\x03\n\x06\x43onfig\x12(\n\x06\x63ommon\x18\x01 \x01(\x0b\x32\x18.messagev.deployv.Common\x12:\n\tcustomers\x18\x02 \x03(\x0b\x32\'.messagev.deployv.Config.CustomersEntry\x12,\n\nserver_cfg\x18\x03 \x01(\x0b\x32\x18.messagev.deployv.Server\x12&\n\x05\x62trfs\x18\x04 \x01(\x0b\x32\x17.messagev.deployv.Btrfs\x12\"\n\x03zfs\x18\x05 \x01(\x0b\x32\x15.messagev.deployv.Zfs\x12,\n\x08\x64\x61tabase\x18\x06 \x01(\x0b\x32\x1a.messagev.deployv.Database\x12(\n\x06\x61lerts\x18\x07 \x01(\x0b\x32\x18.messagev.deployv.Alerts\x1aU\n\x0e\x43ustomersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.messagev.deployv.CustomerInstances:\x02\x38\x01\"\xf0\x01\n\x06\x43ommon\x12\x10\n\x08work_dir\x18\x01 \x01(\t\x12\x12\n\nbackup_src\x18\x02 \x01(\t\x12\x13\n\x0b\x63onfig_file\x18\x03 \x01(\t\x12\x0c\n\x04jobs\x18\x04 \x01(\x05\x12\x10\n\x08password\x18\x05 \x01(\t\x12\x36\n\rs3_credential\x18\x06 \x01(\x0b\x32\x1f.messagev.deployv.S3Credentials\x12\r\n\x05no_fs\x18\x07 \x01(\x08\x12\x0e\n\x06no_cpt\x18\x08 \x01(\x08\x12\x10\n\x08log_file\x18\t \x01(\t\x12\x11\n\tlog_level\x18\n \x01(\t\x12\x0f\n\x07node_id\x18\x0b \x01(\t\"h\n\rS3Credentials\x12\x10\n\x08\x45ndPoint\x18\x01 \x01(\t\x12\x10\n\x08\x43lientID\x18\x02 \x01(\t\x12\x11\n\tSecretKey\x18\x03 \x01(\t\x12\x10\n\x08Insecure\x18\x04 \x01(\x08\x12\x0e\n\x06Region\x18\x05 \x01(\t\"t\n\x11\x43ustomerInstances\x12\x35\n\tinstances\x18\x01 \x03(\x0b\x32\".messagev.deployv.CustomerInstance\x12(\n\x06restic\x18\x02 \x01(\x0b\x32\x18.messagev.deployv.Restic\"z\n\x10\x43ustomerInstance\x12\x13\n\x0b\x63ustomer_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nconfigFile\x18\x03 \x01(\t\x12\x0c\n\x04jobs\x18\x04 \x01(\x05\x12\r\n\x05no_fs\x18\x05 \x01(\x08\x12\x0e\n\x06no_cpt\x18\x06 \x01(\x08\"\x18\n\x06Server\x12\x0e\n\x06listen\x18\x01 \x01(\t\"y\n\x05\x42trfs\x12\x11\n\tbase_path\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x62_storage_path\x18\x02 \x01(\t\x12\x17\n\x0f\x66s_storage_path\x18\x03 \x01(\t\x12\x12\n\ndb_version\x18\x04 \x01(\t\x12\x17\n\x0f\x64\x62_version_read\x18\x05 \x01(\x08\"z\n\x03Zfs\x12\x14\n\x0c\x62\x61se_dataset\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x62_storage_path\x18\x02 \x01(\t\x12\x17\n\x0f\x66s_storage_path\x18\x03 \x01(\t\x12\x12\n\ndb_version\x18\x04 \x01(\t\x12\x17\n\x0f\x64\x62_version_read\x18\x05 \x01(\x08\"C\n\x08\x44\x61tabase\x12\x11\n\tpsql_repo\x18\x01 \x01(\t\x12\x10\n\x08psql_tag\x18\x02 \x01(\t\x12\x12\n\nadmin_pass\x18\x03 \x01(\t\"1\n\x0eGitlabIncident\x12\x10\n\x08repo_url\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\x9c\x02\n\x0bGitlabIssue\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nproject_id\x18\x02 \x01(\x03\x12\r\n\x05token\x18\x03 \x01(\t\x12;\n\ntoken_type\x18\x04 \x01(\x0e\x32\'.messagev.deployv.GitlabIssue.TokenType\x12;\n\nissue_type\x18\x05 \x01(\x0e\x32\'.messagev.deployv.GitlabIssue.IssueType\".\n\tTokenType\x12\t\n\x05OAUTH\x10\x00\x12\x0b\n\x07PRIVATE\x10\x01\x12\t\n\x05\x42\x41SIC\x10\x02\"3\n\tIssueType\x12\t\n\x05ISSUE\x10\x00\x12\x0c\n\x08INCIDENT\x10\x01\x12\r\n\tTEST_CASE\x10\x02\"x\n\x06\x41lerts\x12\x39\n\x0fgitlab_incident\x18\x01 \x01(\x0b\x32 .messagev.deployv.GitlabIncident\x12\x33\n\x0cgitlab_issue\x18\x02 \x01(\x0b\x32\x1d.messagev.deployv.GitlabIssue\"\x94\x02\n\x06Restic\x12\x12\n\nrepository\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0e\n\x06htpass\x18\x03 \x01(\t\x12:\n\tvariables\x18\x04 \x03(\x0b\x32\'.messagev.deployv.Restic.VariablesEntry\x12\x36\n\x07options\x18\x05 \x03(\x0b\x32%.messagev.deployv.Restic.OptionsEntry\x1a\x30\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3'
 )
 
 
 
+_GITLABISSUE_TOKENTYPE = _descriptor.EnumDescriptor(
+  name='TokenType',
+  full_name='messagev.deployv.GitlabIssue.TokenType',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='OAUTH', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='PRIVATE', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='BASIC', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=1614,
+  serialized_end=1660,
+)
+_sym_db.RegisterEnumDescriptor(_GITLABISSUE_TOKENTYPE)
+
+_GITLABISSUE_ISSUETYPE = _descriptor.EnumDescriptor(
+  name='IssueType',
+  full_name='messagev.deployv.GitlabIssue.IssueType',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='ISSUE', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='INCIDENT', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='TEST_CASE', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=1662,
+  serialized_end=1713,
+)
+_sym_db.RegisterEnumDescriptor(_GITLABISSUE_ISSUETYPE)
+
 
 _CONFIG_CUSTOMERSENTRY = _descriptor.Descriptor(
   name='CustomersEntry',
   full_name='messagev.deployv.Config.CustomersEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
@@ -211,28 +271,35 @@
     _descriptor.FieldDescriptor(
       name='log_level', full_name='messagev.deployv.Common.log_level', index=9,
       number=10, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_id', full_name='messagev.deployv.Common.node_id', index=10,
+      number=11, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=445,
-  serialized_end=668,
+  serialized_end=685,
 )
 
 
 _S3CREDENTIALS = _descriptor.Descriptor(
   name='S3Credentials',
   full_name='messagev.deployv.S3Credentials',
   filename=None,
@@ -283,16 +350,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=670,
-  serialized_end=774,
+  serialized_start=687,
+  serialized_end=791,
 )
 
 
 _CUSTOMERINSTANCES = _descriptor.Descriptor(
   name='CustomerInstances',
   full_name='messagev.deployv.CustomerInstances',
   filename=None,
@@ -322,16 +389,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=776,
-  serialized_end=892,
+  serialized_start=793,
+  serialized_end=909,
 )
 
 
 _CUSTOMERINSTANCE = _descriptor.Descriptor(
   name='CustomerInstance',
   full_name='messagev.deployv.CustomerInstance',
   filename=None,
@@ -389,16 +456,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=894,
-  serialized_end=1016,
+  serialized_start=911,
+  serialized_end=1033,
 )
 
 
 _SERVER = _descriptor.Descriptor(
   name='Server',
   full_name='messagev.deployv.Server',
   filename=None,
@@ -421,16 +488,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1018,
-  serialized_end=1042,
+  serialized_start=1035,
+  serialized_end=1059,
 )
 
 
 _BTRFS = _descriptor.Descriptor(
   name='Btrfs',
   full_name='messagev.deployv.Btrfs',
   filename=None,
@@ -481,16 +548,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1044,
-  serialized_end=1165,
+  serialized_start=1061,
+  serialized_end=1182,
 )
 
 
 _ZFS = _descriptor.Descriptor(
   name='Zfs',
   full_name='messagev.deployv.Zfs',
   filename=None,
@@ -541,16 +608,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1167,
-  serialized_end=1289,
+  serialized_start=1184,
+  serialized_end=1306,
 )
 
 
 _DATABASE = _descriptor.Descriptor(
   name='Database',
   full_name='messagev.deployv.Database',
   filename=None,
@@ -587,16 +654,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1291,
-  serialized_end=1358,
+  serialized_start=1308,
+  serialized_end=1375,
 )
 
 
 _GITLABINCIDENT = _descriptor.Descriptor(
   name='GitlabIncident',
   full_name='messagev.deployv.GitlabIncident',
   filename=None,
@@ -614,35 +681,90 @@
     _descriptor.FieldDescriptor(
       name='token', full_name='messagev.deployv.GitlabIncident.token', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1377,
+  serialized_end=1426,
+)
+
+
+_GITLABISSUE = _descriptor.Descriptor(
+  name='GitlabIssue',
+  full_name='messagev.deployv.GitlabIssue',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='url', full_name='messagev.deployv.GitlabIssue.url', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='node_id', full_name='messagev.deployv.GitlabIncident.node_id', index=2,
+      name='project_id', full_name='messagev.deployv.GitlabIssue.project_id', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='token', full_name='messagev.deployv.GitlabIssue.token', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='token_type', full_name='messagev.deployv.GitlabIssue.token_type', index=3,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issue_type', full_name='messagev.deployv.GitlabIssue.issue_type', index=4,
+      number=5, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _GITLABISSUE_TOKENTYPE,
+    _GITLABISSUE_ISSUETYPE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1360,
-  serialized_end=1426,
+  serialized_start=1429,
+  serialized_end=1713,
 )
 
 
 _ALERTS = _descriptor.Descriptor(
   name='Alerts',
   full_name='messagev.deployv.Alerts',
   filename=None,
@@ -653,28 +775,35 @@
     _descriptor.FieldDescriptor(
       name='gitlab_incident', full_name='messagev.deployv.Alerts.gitlab_incident', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='gitlab_issue', full_name='messagev.deployv.Alerts.gitlab_issue', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1428,
-  serialized_end=1495,
+  serialized_start=1715,
+  serialized_end=1835,
 )
 
 
 _RESTIC_VARIABLESENTRY = _descriptor.Descriptor(
   name='VariablesEntry',
   full_name='messagev.deployv.Restic.VariablesEntry',
   filename=None,
@@ -704,16 +833,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1678,
-  serialized_end=1726,
+  serialized_start=2018,
+  serialized_end=2066,
 )
 
 _RESTIC_OPTIONSENTRY = _descriptor.Descriptor(
   name='OptionsEntry',
   full_name='messagev.deployv.Restic.OptionsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -742,16 +871,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1728,
-  serialized_end=1774,
+  serialized_start=2068,
+  serialized_end=2114,
 )
 
 _RESTIC = _descriptor.Descriptor(
   name='Restic',
   full_name='messagev.deployv.Restic',
   filename=None,
   file=DESCRIPTOR,
@@ -801,45 +930,51 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1498,
-  serialized_end=1774,
+  serialized_start=1838,
+  serialized_end=2114,
 )
 
 _CONFIG_CUSTOMERSENTRY.fields_by_name['value'].message_type = _CUSTOMERINSTANCES
 _CONFIG_CUSTOMERSENTRY.containing_type = _CONFIG
 _CONFIG.fields_by_name['common'].message_type = _COMMON
 _CONFIG.fields_by_name['customers'].message_type = _CONFIG_CUSTOMERSENTRY
 _CONFIG.fields_by_name['server_cfg'].message_type = _SERVER
 _CONFIG.fields_by_name['btrfs'].message_type = _BTRFS
 _CONFIG.fields_by_name['zfs'].message_type = _ZFS
 _CONFIG.fields_by_name['database'].message_type = _DATABASE
 _CONFIG.fields_by_name['alerts'].message_type = _ALERTS
 _COMMON.fields_by_name['s3_credential'].message_type = _S3CREDENTIALS
 _CUSTOMERINSTANCES.fields_by_name['instances'].message_type = _CUSTOMERINSTANCE
 _CUSTOMERINSTANCES.fields_by_name['restic'].message_type = _RESTIC
+_GITLABISSUE.fields_by_name['token_type'].enum_type = _GITLABISSUE_TOKENTYPE
+_GITLABISSUE.fields_by_name['issue_type'].enum_type = _GITLABISSUE_ISSUETYPE
+_GITLABISSUE_TOKENTYPE.containing_type = _GITLABISSUE
+_GITLABISSUE_ISSUETYPE.containing_type = _GITLABISSUE
 _ALERTS.fields_by_name['gitlab_incident'].message_type = _GITLABINCIDENT
+_ALERTS.fields_by_name['gitlab_issue'].message_type = _GITLABISSUE
 _RESTIC_VARIABLESENTRY.containing_type = _RESTIC
 _RESTIC_OPTIONSENTRY.containing_type = _RESTIC
 _RESTIC.fields_by_name['variables'].message_type = _RESTIC_VARIABLESENTRY
 _RESTIC.fields_by_name['options'].message_type = _RESTIC_OPTIONSENTRY
 DESCRIPTOR.message_types_by_name['Config'] = _CONFIG
 DESCRIPTOR.message_types_by_name['Common'] = _COMMON
 DESCRIPTOR.message_types_by_name['S3Credentials'] = _S3CREDENTIALS
 DESCRIPTOR.message_types_by_name['CustomerInstances'] = _CUSTOMERINSTANCES
 DESCRIPTOR.message_types_by_name['CustomerInstance'] = _CUSTOMERINSTANCE
 DESCRIPTOR.message_types_by_name['Server'] = _SERVER
 DESCRIPTOR.message_types_by_name['Btrfs'] = _BTRFS
 DESCRIPTOR.message_types_by_name['Zfs'] = _ZFS
 DESCRIPTOR.message_types_by_name['Database'] = _DATABASE
 DESCRIPTOR.message_types_by_name['GitlabIncident'] = _GITLABINCIDENT
+DESCRIPTOR.message_types_by_name['GitlabIssue'] = _GITLABISSUE
 DESCRIPTOR.message_types_by_name['Alerts'] = _ALERTS
 DESCRIPTOR.message_types_by_name['Restic'] = _RESTIC
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Config = _reflection.GeneratedProtocolMessageType('Config', (_message.Message,), {
 
   'CustomersEntry' : _reflection.GeneratedProtocolMessageType('CustomersEntry', (_message.Message,), {
@@ -914,14 +1049,21 @@
 GitlabIncident = _reflection.GeneratedProtocolMessageType('GitlabIncident', (_message.Message,), {
   'DESCRIPTOR' : _GITLABINCIDENT,
   '__module__' : 'config_pb2'
   # @@protoc_insertion_point(class_scope:messagev.deployv.GitlabIncident)
   })
 _sym_db.RegisterMessage(GitlabIncident)
 
+GitlabIssue = _reflection.GeneratedProtocolMessageType('GitlabIssue', (_message.Message,), {
+  'DESCRIPTOR' : _GITLABISSUE,
+  '__module__' : 'config_pb2'
+  # @@protoc_insertion_point(class_scope:messagev.deployv.GitlabIssue)
+  })
+_sym_db.RegisterMessage(GitlabIssue)
+
 Alerts = _reflection.GeneratedProtocolMessageType('Alerts', (_message.Message,), {
   'DESCRIPTOR' : _ALERTS,
   '__module__' : 'config_pb2'
   # @@protoc_insertion_point(class_scope:messagev.deployv.Alerts)
   })
 _sym_db.RegisterMessage(Alerts)
```

### Comparing `messagev-0.0.7/messagev.egg-info/PKG-INFO` & `messagev-0.0.8/messagev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: messagev
-Version: 0.0.7
+Version: 0.0.8
 Summary: MessageV: the python files generated for consuming the Orchest API
 Home-page: UNKNOWN
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Description: # MessageV
```

### Comparing `messagev-0.0.7/setup.py` & `messagev-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open('HISTORY.rst') as history_file:
     history = history_file.read().replace('.. :changelog:', '')
 
 requirements = open('requirements.txt').readlines()
 
 setup(
     name='messagev',
-    version='0.0.7',
+    version='0.0.8',
     description="MessageV: the python files generated for consuming the Orchest API",
     long_description=readme + '\n\n' + history,
     author="Vauxoo",
     author_email='info@vauxoo.com',
     url='',
     packages=[
         'messagev',
```

