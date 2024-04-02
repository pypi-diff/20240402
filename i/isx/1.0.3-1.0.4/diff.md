# Comparing `tmp/isx-1.0.3.tar.gz` & `tmp/isx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isx-1.0.3.tar", last modified: Thu Jan 18 21:10:41 2024, max compression
+gzip compressed data, was "isx-1.0.4.tar", last modified: Tue Apr  2 20:35:14 2024, max compression
```

## Comparing `isx-1.0.3.tar` & `isx-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:10:41.959991 isx-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-01-18 21:10:38.000000 isx-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-18 21:10:41.959991 isx-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-18 21:10:38.000000 isx-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:10:41.959991 isx-1.0.3/isx/
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-01-18 21:10:38.000000 isx-1.0.3/isx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:10:41.959991 isx-1.0.3/isx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-18 21:10:41.000000 isx-1.0.3/isx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-18 21:10:41.000000 isx-1.0.3/isx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 21:10:41.000000 isx-1.0.3/isx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-18 21:10:41.000000 isx-1.0.3/isx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 21:10:41.000000 isx-1.0.3/isx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-01-18 21:10:38.000000 isx-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 21:10:41.959991 isx-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-18 21:10:40.000000 isx-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:14.639136 isx-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-04-02 20:35:11.000000 isx-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 20:35:14.639136 isx-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 20:35:11.000000 isx-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:14.639136 isx-1.0.4/isx/
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-02 20:35:11.000000 isx-1.0.4/isx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:14.639136 isx-1.0.4/isx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 20:35:14.000000 isx-1.0.4/isx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 20:35:14.000000 isx-1.0.4/isx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:35:14.000000 isx-1.0.4/isx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 20:35:14.000000 isx-1.0.4/isx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:35:14.000000 isx-1.0.4/isx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-02 20:35:11.000000 isx-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:35:14.639136 isx-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-02 20:35:13.000000 isx-1.0.4/setup.py
```

### Comparing `isx-1.0.3/LICENSE.txt` & `isx-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isx-1.0.3/PKG-INFO` & `isx-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: isx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-based ISXD file reader
 Home-page: https://github.com/inscopix/py_isx
-Author: Srinivas Gorur-Shandilya
-Author-email: s.gorur_shandilya@bruker.com
-Maintainer: Zachary Ip
-Maintainer-email: Zachary.Ip@bruker.com
+Author: Inscopix, Inc.
+Author-email: support@inscopix.com
+Maintainer: Inscopix, Inc.
+Maintainer-email: support@inscopix.com
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `isx-1.0.3/README.md` & `isx-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `isx-1.0.3/isx/__init__.py` & `isx-1.0.4/isx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 
     """
 
     file_path: str = None
     footer: dict = None
     timing: Timing = Timing()
-    spacing: Timing = Spacing()
+    spacing: Spacing = Spacing()
 
     def __init__(self):
         pass
 
     @property
     def data_type(self):
         if self.footer["dataType"] == 0:
@@ -176,21 +176,18 @@
 
         Returns:
             The retrieved frame data.
         """
 
         if self.footer["dataType"] == 0:
             bytes_per_pixel = 2
-            format_string = "H"
         elif self.footer["dataType"] == 1:
             bytes_per_pixel = 4
-            format_string = "f"
         elif self.footer["dataType"] == 2:
             bytes_per_pixel = 1
-            format_string = "b"
         else:
             raise NotImplementedError(
                 "Unknown number of bytes per pixel. Cannot decode this frame."
             )
 
         if self.footer["hasFrameHeaderFooter"]:
             raise NotImplementedError(
@@ -209,18 +206,16 @@
 
         n_pixels = self.spacing.num_pixels[0] * self.spacing.num_pixels[1]
 
         n_bytes_per_frame = n_pixels * bytes_per_pixel
 
         with open(self.file_path, mode="rb") as file:
             file.seek(index * n_bytes_per_frame)
-
             data = file.read(bytes_per_pixel * n_pixels)
-
-            frame = struct.unpack(format_string * n_pixels, data)
+            frame = np.frombuffer(data, dtype=self.data_type)
             frame = np.reshape(frame, self.spacing.num_pixels)
 
         return frame
 
     def get_frame_timestamp(self, index):
         raise NotImplementedError(NOT_IMPLEMENTED_MESSAGE)
 
@@ -247,15 +242,14 @@
     !!! info "How to use the CellSet class"
         To see how to use this class to read data from
         ISXD Cellsets, click [here](../how-to/read-cellset.md).
         This reference page describes each member of this
         class and what each function does."""
 
     num_cells: int = 0
-    timing = None
     file_path = None
     footer = None
     spacing: Spacing = Spacing()
     timing: Timing = Timing()
 
     def __init__(self):
         pass
@@ -371,19 +365,19 @@
     """
 
     metadata = _extract_footer(file_path)
 
     isx_datatype_mapping = {
         0: "miniscope_movie",
         1: "cell_set",
-        2: "isxd_behavioral_movie",  # not currently supported on IDEAS
+        2: "isxd_behavioral_movie",
         3: "gpio_data",
         4: "miniscope_image",
         5: "neural_events",
-        6: "isxd_metrics",  # not currently supported on IDEAS
+        6: "isxd_metrics",
         7: "imu_data",
         8: "vessel_set",
     }
     return isx_datatype_mapping[metadata["type"]]
 
 
 @beartype
```

### Comparing `isx-1.0.3/isx.egg-info/PKG-INFO` & `isx-1.0.4/isx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: isx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-based ISXD file reader
 Home-page: https://github.com/inscopix/py_isx
-Author: Srinivas Gorur-Shandilya
-Author-email: s.gorur_shandilya@bruker.com
-Maintainer: Zachary Ip
-Maintainer-email: Zachary.Ip@bruker.com
+Author: Inscopix, Inc.
+Author-email: support@inscopix.com
+Maintainer: Inscopix, Inc.
+Maintainer-email: support@inscopix.com
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `isx-1.0.3/pyproject.toml` & `isx-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 [tool.poetry]
 name = "isx"
 version = "0.0.0.dev"
 description = "Python-based ISXD file reader"
-authors = ["Srinivas Gorur-Shandilya <s.gorur_shandilya@bruker.com>", "Zachary Ip <Zachary.Ip@bruker.com>"]
-maintainers = ["Zachary Ip <Zachary.Ip@bruker.com>"]
+authors = ["Inscopix, Inc. <support@inscopix.com>"]
+maintainers = ["Inscopix, Inc. <support@inscopix.com>"]
 readme = "README.md"
 license = "CC-BY-NC-4.0"
 homepage = "https://github.com/inscopix/py_isx"
 repository = "https://github.com/inscopix/py_isx"
 documentation = "https://inscopix.github.io/py_isx/"
```

### Comparing `isx-1.0.3/setup.py` & `isx-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,21 +24,21 @@
           'mkdocs-git-committers-plugin-2>=2.2.3,<3.0.0'],
  'test': ['pytest>=7.2.0',
           'poetry2setup>=1.1.0,<2.0.0',
           'requests>=2.31.0,<3.0.0']}
 
 setup_kwargs = {
     'name': 'isx','long_description_content_type':'text/markdown',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Python-based ISXD file reader',
     'long_description': '# isx: pure-python API to read Inscopix data\n\n![](https://github.com/inscopix/py_isx/actions/workflows/main.yml/badge.svg) \n![](https://img.shields.io/pypi/v/isx)\n\nThis is a pure-python API to read Inscopix ISXD files. \n\n\n## Documentation\n\n[Read the documentation](https://inscopix.github.io/py_isx/)\n\n## Support\n\n|  File type | Support |\n|  --------- | ------- |\n| ISXD CellSet   | ✅ |\n| ISXD Movie   | ✅ |\n| ISXD Movie (multi-plane)   | ❌ |\n| ISXD Movie (dual-color)   | ❌ |\n| GPIO data   | ❌ |\n| ISXD Events   | ❌ |\n| ISXD VesselSet   | ❌ |\n\n\n## Install\n\n### Poetry\n\n```bash\npoetry add isx\n```\n\n### pip\n\n\n```bash\npip install isx\n```\n\n## Caution\n\nThis is a work in progress, and all reading functions in the IDPS Python API are not supported yet. \n\n\n## Testing\n\nThis code is tested using GitHub Actions on the following python\nversions:\n\n- 3.9\n- 3.10\n- 3.11\n- 3.12\n',
-    'author': 'Srinivas Gorur-Shandilya',
-    'author_email': 's.gorur_shandilya@bruker.com',
-    'maintainer': 'Zachary Ip',
-    'maintainer_email': 'Zachary.Ip@bruker.com',
+    'author': 'Inscopix, Inc.',
+    'author_email': 'support@inscopix.com',
+    'maintainer': 'Inscopix, Inc.',
+    'maintainer_email': 'support@inscopix.com',
     'url': 'https://github.com/inscopix/py_isx',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.9,<4.0',
 }
```

