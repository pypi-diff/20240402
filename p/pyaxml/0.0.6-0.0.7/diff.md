# Comparing `tmp/pyaxml-0.0.6.tar.gz` & `tmp/pyaxml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaxml-0.0.6.tar", last modified: Wed Mar 20 23:30:53 2024, max compression
+gzip compressed data, was "pyaxml-0.0.7.tar", last modified: Tue Apr  2 21:34:10 2024, max compression
```

## Comparing `pyaxml-0.0.6.tar` & `pyaxml-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 23:30:53.277874 pyaxml-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-03-20 23:30:14.000000 pyaxml-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22742 2024-03-20 23:30:53.276876 pyaxml-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-03-20 23:30:14.000000 pyaxml-0.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1174 2024-03-20 23:30:14.000000 pyaxml-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 23:30:53.277874 pyaxml-0.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 23:30:53.273880 pyaxml-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 23:30:53.274879 pyaxml-0.0.6/src/pyaxml/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-03-20 23:30:14.000000 pyaxml-0.0.6/src/pyaxml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30177 2024-03-20 23:30:14.000000 pyaxml-0.0.6/src/pyaxml/axml.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-20 23:30:14.000000 pyaxml-0.0.6/src/pyaxml/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 23:30:53.276876 pyaxml-0.0.6/src/pyaxml/proto/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-20 23:30:14.000000 pyaxml-0.0.6/src/pyaxml/proto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2024-03-20 23:30:14.000000 pyaxml-0.0.6/src/pyaxml/proto/axml.proto
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 23:30:53.276876 pyaxml-0.0.6/src/pyaxml.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22742 2024-03-20 23:30:53.000000 pyaxml-0.0.6/src/pyaxml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-20 23:30:53.000000 pyaxml-0.0.6/src/pyaxml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 23:30:53.000000 pyaxml-0.0.6/src/pyaxml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-20 23:30:53.000000 pyaxml-0.0.6/src/pyaxml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-20 23:30:53.000000 pyaxml-0.0.6/src/pyaxml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.871738 pyaxml-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-04-02 21:33:29.000000 pyaxml-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22742 2024-04-02 21:34:10.871738 pyaxml-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-02 21:33:29.000000 pyaxml-0.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2024-04-02 21:33:29.000000 pyaxml-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 21:34:10.871738 pyaxml-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.866738 pyaxml-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.868738 pyaxml-0.0.7/src/pyaxml/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30159 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/axml.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.870738 pyaxml-0.0.7/src/pyaxml/proto/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/proto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/proto/axml.proto
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.870738 pyaxml-0.0.7/src/pyaxml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22742 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/top_level.txt
```

### Comparing `pyaxml-0.0.6/LICENSE` & `pyaxml-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.6/PKG-INFO` & `pyaxml-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.6
+Version: 0.0.7
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

### Comparing `pyaxml-0.0.6/README.md` & `pyaxml-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.6/pyproject.toml` & `pyaxml-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.6/src/pyaxml/axml.py` & `pyaxml-0.0.7/src/pyaxml/axml.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             self.proto = axml_pb2.StringBlocks()
     
     def compute(self):
         """Compute all fields to have all StringBlocks elements
         """
 
         idx = 0
+        del self.proto.stringoffsets[:]
         for s in self.proto.stringblocks:
             self.proto.stringoffsets.append(idx)
             idx += len(StringBlock(proto=s, utf8=self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG).pack())
 
         self.proto.hnd.stringoffset = AXML_STRING_POOL_HEADER_SIZE + \
             len(b"".join(pack('<I', x) for x in self.proto.stringoffsets)) + \
             len(b"".join(pack('<I', x) for x in self.proto.styleoffsets))
@@ -626,15 +627,14 @@
     @property
     def get_proto(self):
         """_summary_
 
         Returns:
             _type_: _description_
         """
-        self.proto.stringblocks = self.stringblocks.proto
         return self.proto
 
     ###########################################
     #                                         #
     #           ENOCDE from XML               #
     #                                         #
     ###########################################
@@ -804,15 +804,15 @@
                         if not val in res:
                             self.stringblocks.get(name)
                             res.append(val)
         self.proto.resourcemap.CopyFrom(ResourceMap(res=res).proto)
 
     ###########################################
     #                                         #
-    #           ENOCDE from XML               #
+    #           ENCODE from XML               #
     #                                         #
     ###########################################
     
     def compute(self):
         """Compute all fields to have all AXML elements
         """
         self.stringblocks.compute()
```

### Comparing `pyaxml-0.0.6/src/pyaxml/proto/axml.proto` & `pyaxml-0.0.7/src/pyaxml/proto/axml.proto`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.6/src/pyaxml.egg-info/PKG-INFO` & `pyaxml-0.0.7/src/pyaxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.6
+Version: 0.0.7
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

