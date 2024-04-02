# Comparing `tmp/pyCEPS-0.1.0.tar.gz` & `tmp/pyCEPS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCEPS-0.1.0.tar", last modified: Mon Mar 11 12:53:31 2024, max compression
+gzip compressed data, was "pyCEPS-0.1.1.tar", last modified: Tue Apr  2 08:03:33 2024, max compression
```

## Comparing `pyCEPS-0.1.0.tar` & `pyCEPS-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/pyCEPS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 12:53:31.000000 pyCEPS-0.1.0/pyCEPS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.164528 pyCEPS-0.1.0/pyceps/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18782 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.164528 pyCEPS-0.1.0/pyceps/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/cartotypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/lesions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/precisiontypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    41572 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/datatypes/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/pyceps/fileio/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99208 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/cartoio.py
--rw-r--r--   0 runner    (1001) docker     (127)    25097 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/cartoutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/igb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/pathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/precisionio.py
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/precisionutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/fileio/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/pyceps/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/colormaps.json
--rw-r--r--   0 runner    (1001) docker     (127)    30881 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/dashapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/dashelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/dashlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/pyceps/visualize/dashutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-11 12:53:23.000000 pyCEPS-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 12:53:31.168528 pyCEPS-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-11 12:53:28.000000 pyCEPS-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyCEPS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.885007 pyCEPS-0.1.1/pyceps/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18779 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.885007 pyCEPS-0.1.1/pyceps/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/cartotypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/lesions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/precisiontypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41578 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyceps/fileio/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99276 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/cartoio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25097 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/cartoutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/igb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/pathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/precisionio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/precisionutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyceps/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/colormaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30881 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-02 08:03:31.000000 pyCEPS-0.1.1/setup.py
```

### Comparing `pyCEPS-0.1.0/LICENSE.txt` & `pyCEPS-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/PKG-INFO` & `pyCEPS-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
```

### Comparing `pyCEPS-0.1.0/README.md` & `pyCEPS-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyCEPS.egg-info/PKG-INFO` & `pyCEPS-0.1.1/pyCEPS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
```

### Comparing `pyCEPS-0.1.0/pyCEPS.egg-info/SOURCES.txt` & `pyCEPS-0.1.1/pyCEPS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/__init__.py` & `pyCEPS-0.1.1/pyceps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/cli.py` & `pyCEPS-0.1.1/pyceps/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
     # now we can import maps from EAM repo
     if import_maps:
         logger.info('need to import map(s): {}'.format(import_maps))
 
         if args.pkl_file and not study.is_root_valid():
             logger.warning('a valid study root is necessary to import maps!')
         else:
-            study.import_maps(study.mapNames,
+            study.import_maps(import_maps,
                               egm_names_from_pos=args.egm_from_pos)
             # import lesion data for all loaded maps
             for map_name in study.maps.keys():
                 study.maps[map_name].import_lesions(directory=None)
             data_changed = True
 
     # work out which map(s) to process
```

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/__init__.py` & `pyCEPS-0.1.1/pyceps/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/cartotypes.py` & `pyCEPS-0.1.1/pyceps/datatypes/cartotypes.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/lesions.py` & `pyCEPS-0.1.1/pyceps/datatypes/lesions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/precisiontypes.py` & `pyCEPS-0.1.1/pyceps/datatypes/precisiontypes.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/signals.py` & `pyCEPS-0.1.1/pyceps/datatypes/signals.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/study.py` & `pyCEPS-0.1.1/pyceps/datatypes/study.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
     def export_additional_meshes(self, *args, **kwargs):
         raise NotImplementedError
 
     def is_root_valid(self, root_dir=None):
         raise NotImplementedError
 
-    def set_root(self, root_dir):
+    def set_repository(self, root_dir):
         raise NotImplementedError
 
     @classmethod
     def load(cls, filename, root=None):
         raise NotImplemented
 
     def list_maps(self, minimal=False):
```

### Comparing `pyCEPS-0.1.0/pyceps/datatypes/surface.py` & `pyCEPS-0.1.1/pyceps/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/exceptions.py` & `pyCEPS-0.1.1/pyceps/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/__init__.py` & `pyCEPS-0.1.1/pyceps/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/cartoio.py` & `pyCEPS-0.1.1/pyceps/fileio/cartoio.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,31 +652,32 @@
         else:
             f = open(filename, 'rb')
         obj = pickle.load(f)
         f.close()
 
         # try to set root if explicitly given
         if root:
-            if obj.set_root(os.path.abspath(root)):
+            if obj.set_repository(os.path.abspath(root)):
                 log.info('setting study root to {}'.format(root))
                 return obj
             else:
                 log.info('cannot set study root to {}\n'
                          'Trying to use root information from PKL'
                          .format(root))
 
         # try to re-set previous study root
-        if obj.set_root(obj.repository.base):
+        if obj.set_repository(obj.repository.base):
             log.info('previous study root is still valid ({})'
                      .format(obj.repository.root))
             return obj
 
         # no valid root found so far, set to pkl directory
         log.warning('no valid study root found. Using .pkl location!'.upper())
-        obj.repository.update_root(os.path.dirname(os.path.abspath(filename)))
+        obj.repository.base = os.path.abspath(filename)
+        obj.repository.root = os.path.dirname(os.path.abspath(filename))
         return obj
 
     def export_additional_meshes(self, filename=''):
         """
         Export additional meshes and registration matrix in study to VTK.
         Overrides BaseClass method.
 
@@ -828,15 +829,15 @@
             if not tmp_root.root:
                 # dummy repo was not initialized properly, so root is invalid
                 return False
             return self._locate_study_xml(tmp_root, pwd=pwd) is not None
 
         return False
 
-    def set_root(self, root_dir):
+    def set_repository(self, root_dir):
         """
         Change path to root directory. Overrides BaseClass method.
         If new root directory is invalid, it is not changed.
 
         Parameters:
             root_dir : string
                 new root directory
```

### Comparing `pyCEPS-0.1.0/pyceps/fileio/cartoutils.py` & `pyCEPS-0.1.1/pyceps/fileio/cartoutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/igb.py` & `pyCEPS-0.1.1/pyceps/fileio/igb.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/pathtools.py` & `pyCEPS-0.1.1/pyceps/fileio/pathtools.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/precisionio.py` & `pyCEPS-0.1.1/pyceps/fileio/precisionio.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if not all(n in folder_list for n in self.mapNames):
             # root saved in study is invalid
             return False
 
         # specified root directory is valid
         return True
 
-    def set_root(self, root_dir):
+    def set_repository(self, root_dir):
         """
         Change path to root directory.
 
         If new root directory is invalid, it is not changed.
 
         Parameters:
             root_dir : string
@@ -175,27 +175,27 @@
         else:
             f = open(filename, 'rb')
         obj = pickle.load(f)
         f.close()
 
         # try to set root if explicitly given
         if root:
-            if obj.set_root(os.path.abspath(root)):
+            if obj.set_repository(os.path.abspath(root)):
                 log.info('setting study root to {}'.format(root))
                 return obj
             else:
                 log.info('cannot set study root to {}\n'
                          'Trying to use root information from PKL'
                          .format(root))
 
         # check if repository is valid and accessible
         if obj.is_root_valid():
             log.info('previous study root is still valid ({})'
                      .format(obj.studyRoot))
-            obj.set_root(os.path.abspath(obj.studyRoot))
+            obj.set_repository(os.path.abspath(obj.studyRoot))
             return obj
 
         # no valid root found so far, set to pkl directory
         log.warning('no valid study root found. Using .pkl location!'.upper())
         obj.studyRoot = os.path.abspath(filename)
 
         return obj
```

### Comparing `pyCEPS-0.1.0/pyceps/fileio/precisionutils.py` & `pyCEPS-0.1.1/pyceps/fileio/precisionutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/fileio/writer.py` & `pyCEPS-0.1.1/pyceps/fileio/writer.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/interpolation.py` & `pyCEPS-0.1.1/pyceps/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/utils.py` & `pyCEPS-0.1.1/pyceps/utils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/__init__.py` & `pyCEPS-0.1.1/pyceps/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/colormaps.json` & `pyCEPS-0.1.1/pyceps/visualize/colormaps.json`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/dashapp.py` & `pyCEPS-0.1.1/pyceps/visualize/dashapp.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/dashelements.py` & `pyCEPS-0.1.1/pyceps/visualize/dashelements.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/dashlayout.py` & `pyCEPS-0.1.1/pyceps/visualize/dashlayout.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/pyceps/visualize/dashutils.py` & `pyCEPS-0.1.1/pyceps/visualize/dashutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.0/setup.py` & `pyCEPS-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                'openCARP compatible data formats.'
                )
 LICENSE = 'GPLv3+'
 URL = 'https://github.com/medunigraz/pyCEPS'
 EMAIL = 'robert.arnold@medunigraz.at'
 AUTHOR = 'Robert Arnold'
 REQUIRES_PYTHON = '>=3.8'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 CLASSIFIERS = [
     # Trove classifiers
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

