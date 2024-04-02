# Comparing `tmp/kscale-onshape-library-0.0.7.tar.gz` & `tmp/kscale-onshape-library-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscale-onshape-library-0.0.7.tar", last modified: Mon Apr  1 00:05:25 2024, max compression
+gzip compressed data, was "kscale-onshape-library-0.0.8.tar", last modified: Tue Apr  2 21:09:12 2024, max compression
```

## Comparing `kscale-onshape-library-0.0.7.tar` & `kscale-onshape-library-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.170166 kscale-onshape-library-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-01 00:05:25.170166 kscale-onshape-library-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.162166 kscale-onshape-library-0.0.7/kol/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.166166 kscale-onshape-library-0.0.7/kol/onshape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34926 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.166166 kscale-onshape-library-0.0.7/kol/onshape/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/onshape/schema/part.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.166166 kscale-onshape-library-0.0.7/kol/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.166166 kscale-onshape-library-0.0.7/kol/scripts/bullet/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/bullet/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/bullet/plane.obj
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/bullet/plane.urdf
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/get_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/pybullet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/scripts/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/kol/urdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.170166 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 00:05:25.000000 kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-01 00:05:25.170166 kscale-onshape-library-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:05:25.170166 kscale-onshape-library-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/tests/test_onshape_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-01 00:05:16.000000 kscale-onshape-library-0.0.7/tests/test_urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/onshape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35127 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/onshape/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/part.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kol/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kol/scripts/bullet/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.obj
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/get_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/pybullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/tests/test_onshape_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/tests/test_urdf.py
```

### Comparing `kscale-onshape-library-0.0.7/LICENSE` & `kscale-onshape-library-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/PKG-INFO` & `kscale-onshape-library-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscale-onshape-library
-Version: 0.0.7
+Version: 0.0.8
 Summary: K-Scale's library for programmatically interacting with OnShape
 Home-page: https://github.com/kscalelabs/onshape
 Author: Benjamin Bolte
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
```

### Comparing `kscale-onshape-library-0.0.7/README.md` & `kscale-onshape-library-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/geometry.py` & `kscale-onshape-library-0.0.8/kol/geometry.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/logging.py` & `kscale-onshape-library-0.0.8/kol/logging.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/api.py` & `kscale-onshape-library-0.0.8/kol/onshape/api.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/client.py` & `kscale-onshape-library-0.0.8/kol/onshape/client.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/converter.py` & `kscale-onshape-library-0.0.8/kol/onshape/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,25 +91,27 @@
         default_revolute_joint_limits: The default limits for revolute joints.
         suffix_to_joint_effort: The mapping from joint suffix to effort. This
             is used to override the default joint effort limits by matching
             the suffix of the joint name.
         suffix_to_joint_velocity: The mapping from joint suffix to velocity.
             This is used to override the default joint velocity limits by
             matching the suffix of the joint name.
+        disable_mimics: Whether to disable mimic joints.
     """
 
     def __init__(
         self,
         document_url: str,
         output_dir: str | Path | None = None,
         api: OnshapeApi | None = None,
         default_prismatic_joint_limits: urdf.JointLimits = urdf.JointLimits(80.0, 5.0, -1.0, 1.0),
         default_revolute_joint_limits: urdf.JointLimits = urdf.JointLimits(80.0, 5.0, -np.pi, np.pi),
         suffix_to_joint_effort: list[tuple[str, float]] = [],
         suffix_to_joint_velocity: list[tuple[str, float]] = [],
+        disable_mimics: bool = False,
     ) -> None:
         super().__init__()
 
         # Gets a default output directory.
         self.output_dir = Path.cwd() / "robot" if output_dir is None else Path(output_dir)
 
         # Creates a new directory for cached artifacts.
@@ -122,14 +124,15 @@
 
         self.api = OnshapeApi(OnshapeClient()) if api is None else api
         self.document = self.api.parse_url(document_url)
         self.default_prismatic_joint_limits = default_prismatic_joint_limits
         self.default_revolute_joint_limits = default_revolute_joint_limits
         self.suffix_to_joint_effort = [(k.lower().strip(), v) for k, v in suffix_to_joint_effort]
         self.suffix_to_joint_velocity = [(k.lower().strip(), v) for k, v in suffix_to_joint_velocity]
+        self.disable_mimics = disable_mimics
 
         # Map containing all cached items.
         self.cache_map: dict[str, Any] = {}
 
         # Map containing the transformations from the STL origin to the part frame.
         self.stl_origin_to_part_tf: dict[Key, np.matrix] = {}
 
@@ -433,14 +436,16 @@
         central_node = self.central_node
         logger.debug("Central node: %s", self.key_name(central_node, "link"))
         return nx.bfs_tree(self.graph, central_node)
 
     @functools.cached_property
     def relations(self) -> dict[Key, MimicRelation]:
         relations: dict[Key, MimicRelation] = {}
+        if self.disable_mimics:
+            return relations
         for path, mate_relation_feature in self.key_to_mate_relation_feature.items():
             if mate_relation_feature.suppressed:
                 continue
 
             relation_type = mate_relation_feature.featureData.relationType
             match relation_type:
                 case RelationType.GEAR:
```

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/schema/assembly.py` & `kscale-onshape-library-0.0.8/kol/onshape/schema/assembly.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/schema/common.py` & `kscale-onshape-library-0.0.8/kol/onshape/schema/common.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/schema/features.py` & `kscale-onshape-library-0.0.8/kol/onshape/schema/features.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/onshape/schema/part.py` & `kscale-onshape-library-0.0.8/kol/onshape/schema/part.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/resolvers.py` & `kscale-onshape-library-0.0.8/kol/resolvers.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/scripts/bullet/plane.urdf` & `kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.urdf`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/scripts/cli.py` & `kscale-onshape-library-0.0.8/kol/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/scripts/get_urdf.py` & `kscale-onshape-library-0.0.8/kol/scripts/get_urdf.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/scripts/pybullet.py` & `kscale-onshape-library-0.0.8/kol/scripts/pybullet.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/scripts/stl.py` & `kscale-onshape-library-0.0.8/kol/scripts/stl.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kol/urdf.py` & `kscale-onshape-library-0.0.8/kol/urdf.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/PKG-INFO` & `kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscale-onshape-library
-Version: 0.0.7
+Version: 0.0.8
 Summary: K-Scale's library for programmatically interacting with OnShape
 Home-page: https://github.com/kscalelabs/onshape
 Author: Benjamin Bolte
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
```

### Comparing `kscale-onshape-library-0.0.7/kscale_onshape_library.egg-info/SOURCES.txt` & `kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/pyproject.toml` & `kscale-onshape-library-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/setup.py` & `kscale-onshape-library-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/tests/test_onshape_schema.py` & `kscale-onshape-library-0.0.8/tests/test_onshape_schema.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.7/tests/test_urdf.py` & `kscale-onshape-library-0.0.8/tests/test_urdf.py`

 * *Files identical despite different names*

