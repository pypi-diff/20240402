# Comparing `tmp/grass_gis_helpers-0.6.0.tar.gz` & `tmp/grass_gis_helpers-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grass_gis_helpers-0.6.0.tar", last modified: Wed Mar  6 13:18:52 2024, max compression
+gzip compressed data, was "grass_gis_helpers-1.0.0.tar", last modified: Tue Apr  2 10:25:40 2024, max compression
```

## Comparing `grass_gis_helpers-0.6.0.tar` & `grass_gis_helpers-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-06 13:18:45.000000 grass_gis_helpers-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:52.253704 grass_gis_helpers-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/src/grass_gis_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/mapset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/src/grass_gis_helpers/open_geodata_germany/
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-06 13:18:08.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:18:52.257704 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-06 13:18:52.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-06 13:18:52.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 13:18:52.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-06 13:18:52.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-06 13:18:52.000000 grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.456539 grass_gis_helpers-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 10:25:35.000000 grass_gis_helpers-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:25:40.456539 grass_gis_helpers-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.448539 grass_gis_helpers-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/mapset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/top_level.txt
```

### Comparing `grass_gis_helpers-0.6.0/LICENSE` & `grass_gis_helpers-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/PKG-INFO` & `grass_gis_helpers-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 0.6.0
+Version: 1.0.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-0.6.0/README.md` & `grass_gis_helpers-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/pyproject.toml` & `grass_gis_helpers-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grass_gis_helpers"
-version = "0.6.0"
+version = "1.0.0"
 authors = [
   { name="Anika Weinmann", email="weinmann@mundialis.de" },
 ]
 maintainers = [{name="mundialis GmbH & Co. KG", email="info@mundialis.de"}]
 description = "This library provides functions which can be used for developing GRASS GIS addons."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/cleanup.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/cleanup.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/data_import.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/data_import.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/general.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/general.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     # ulimit -a
     cmd = grass.Popen("ulimit -a", shell=True, stdout=subprocess.PIPE)
     grass.message(
         _(f"\nulimit -a: \n{cmd.communicate()[0].decode('utf-8').rstrip()}")
     )
 
 
-def free_ram(unit, percent=100):
+def get_free_ram(unit, percent=100):
     """The function gives the amount of the percentages of the available
     RAM memory and free swap space.
     Args:
         unit(string): 'GB' or 'MB'
         percent(int): number of percent which should be used of the available
                       RAM memory and free swap space
                       default 100%
@@ -107,7 +107,29 @@
         memory_mb_percent = memory_mb * percent / 100.0
         return int(round(memory_mb_percent))
     elif unit == "GB":
         memory_gb_percent = memory_gb * percent / 100.0
         return int(round(memory_gb_percent))
     else:
         grass.fatal(f"Memory unit {unit} not supported")
+
+
+def test_memory(memory_string):
+    """Test if desired memory is available. In case RAM is smaller than
+    desired memory, use free RAM instead of desired memory value.
+    Args:
+        memory_string(string): string from standard memory input option
+    Returns:
+        free_ram(int): free RAM to use
+        memory(int): available memory to use
+    """
+    # check memory
+    memory = int(memory_string)
+    free_ram = get_free_ram("MB", 100)
+    if free_ram < memory:
+        grass.warning(
+            _(f"Using {memory} MB but only {free_ram} MB RAM available.")
+        )
+        grass.warning(_(f"Set used memory to {free_ram} MB."))
+        return free_ram
+    else:
+        return memory
```

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/location.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/location.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/mapset.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/mapset.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/open_geodata_germany/download_data.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/download_data.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/parallel.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/parallel.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/raster.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/raster.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/tiling.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/tiling.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/validation.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/validation.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers/vector.py` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers/vector.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/PKG-INFO` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 0.6.0
+Version: 1.0.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-0.6.0/src/grass_gis_helpers.egg-info/SOURCES.txt` & `grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

