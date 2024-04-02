# Comparing `tmp/dreifus-0.1.8.tar.gz` & `tmp/dreifus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-_ex26wnu/dreifus-0.1.8.tar", last modified: Thu Nov 23 15:31:06 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-m2ao667d/dreifus-0.1.9.tar", last modified: Tue Jan 16 12:25:48 2024, max compression
```

## Comparing `dreifus-0.1.8.tar` & `dreifus-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:06.258185 dreifus-0.1.8/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2694 2023-11-23 15:31:06.250002 dreifus-0.1.8/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2134 2023-07-20 15:21:23.000000 dreifus-0.1.8/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1083 2023-11-23 15:29:55.000000 dreifus-0.1.8/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-11-23 15:31:06.259186 dreifus-0.1.8/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.1.8/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:05.151788 dreifus-0.1.8/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:05.462407 dreifus-0.1.8/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.1.8/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.1.8/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6338 2023-06-16 11:08:44.000000 dreifus-0.1.8/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2835 2023-11-10 11:06:10.000000 dreifus-0.1.8/src/dreifus/graphics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6882 2023-08-28 12:07:25.000000 dreifus-0.1.8/src/dreifus/image.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:05.810768 dreifus-0.1.8/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.1.8/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6455 2023-08-28 20:24:05.000000 dreifus-0.1.8/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.1.8/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1313 2023-11-10 11:06:10.000000 dreifus-0.1.8/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    18177 2023-10-30 10:36:09.000000 dreifus-0.1.8/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.1.8/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.1.8/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13699 2023-08-31 11:11:56.000000 dreifus-0.1.8/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3155 2023-10-06 13:44:30.000000 dreifus-0.1.8/src/dreifus/render.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.1.8/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:05.900430 dreifus-0.1.8/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.1.8/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4082 2023-07-23 22:13:56.000000 dreifus-0.1.8/src/dreifus/util/colormap.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.1.8/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:06.042843 dreifus-0.1.8/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.1.8/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.1.8/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5925 2023-09-12 09:24:51.000000 dreifus-0.1.8/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.1.8/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:06.237475 dreifus-0.1.8/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2694 2023-11-23 15:31:04.000000 dreifus-0.1.8/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1013 2023-11-23 15:31:05.000000 dreifus-0.1.8/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-11-23 15:31:04.000000 dreifus-0.1.8/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       52 2023-11-23 15:31:04.000000 dreifus-0.1.8/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-11-23 15:31:04.000000 dreifus-0.1.8/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-11-23 15:31:06.213822 dreifus-0.1.8/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.1.8/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.1.8/test/test_camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1530 2023-11-10 11:15:53.000000 dreifus-0.1.8/test/test_graphics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7927 2023-08-28 12:09:11.000000 dreifus-0.1.8/test/test_image.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.1.8/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.1.8/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4475 2023-09-12 09:27:51.000000 dreifus-0.1.8/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.634065 dreifus-0.1.9/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2694 2024-01-16 12:25:48.626978 dreifus-0.1.9/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2134 2023-07-20 15:21:23.000000 dreifus-0.1.9/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1083 2024-01-16 12:17:21.000000 dreifus-0.1.9/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2024-01-16 12:25:48.635072 dreifus-0.1.9/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.1.9/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:47.860144 dreifus-0.1.9/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.064901 dreifus-0.1.9/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.1.9/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.1.9/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6513 2024-01-16 12:16:45.000000 dreifus-0.1.9/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2835 2023-11-10 11:06:10.000000 dreifus-0.1.9/src/dreifus/graphics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6882 2023-08-28 12:07:25.000000 dreifus-0.1.9/src/dreifus/image.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.361745 dreifus-0.1.9/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.1.9/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6455 2023-08-28 20:24:05.000000 dreifus-0.1.9/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.1.9/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1313 2023-11-10 11:06:10.000000 dreifus-0.1.9/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    18177 2023-10-30 10:36:09.000000 dreifus-0.1.9/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.1.9/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.1.9/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13699 2023-08-31 11:11:56.000000 dreifus-0.1.9/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3155 2023-10-06 13:44:30.000000 dreifus-0.1.9/src/dreifus/render.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.1.9/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.429637 dreifus-0.1.9/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.1.9/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4082 2023-07-23 22:13:56.000000 dreifus-0.1.9/src/dreifus/util/colormap.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.1.9/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.503193 dreifus-0.1.9/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.1.9/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.1.9/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6519 2024-01-16 12:16:05.000000 dreifus-0.1.9/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.1.9/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.617957 dreifus-0.1.9/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2694 2024-01-16 12:25:47.000000 dreifus-0.1.9/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1013 2024-01-16 12:25:47.000000 dreifus-0.1.9/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2024-01-16 12:25:47.000000 dreifus-0.1.9/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       52 2024-01-16 12:25:47.000000 dreifus-0.1.9/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2024-01-16 12:25:47.000000 dreifus-0.1.9/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2024-01-16 12:25:48.595811 dreifus-0.1.9/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.1.9/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.1.9/test/test_camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1530 2023-11-10 11:15:53.000000 dreifus-0.1.9/test/test_graphics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7927 2023-08-28 12:09:11.000000 dreifus-0.1.9/test/test_image.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.1.9/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.1.9/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4475 2023-09-12 09:27:51.000000 dreifus-0.1.9/test/test_vector.py
```

### Comparing `dreifus-0.1.8/PKG-INFO` & `dreifus-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreifus
-Version: 0.1.8
+Version: 0.1.9
 Summary: dreifus lifts your 3D camera experience and facilitates computer vision applications
 Author-email: Tobias Kirschstein <tobias.kirschstein@gmail.com>
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
```

### Comparing `dreifus-0.1.8/README.md` & `dreifus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/pyproject.toml` & `dreifus-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.1.8"
+version = "0.1.9"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.7.0"
```

### Comparing `dreifus-0.1.8/src/dreifus/camera.py` & `dreifus-0.1.9/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/camera_bundle.py` & `dreifus-0.1.9/src/dreifus/camera_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 from dreifus.camera import PoseType
 
 from dreifus.matrix import Pose
 from dreifus.vector import Vec3, rotation_matrix_between_vectors, offset_vector_between_line_and_point, \
     angle_between_vectors
+from dreifus.vector.vector_numpy import rotation_matrix_around_axis
 
 
 def calculate_look_center(cam_to_world_poses: List[Pose]) -> Vec3:
     a = []  # point on look-direction line (i.e., position of camera)
     d = []  # look direction
 
     for cam_to_world_pose in cam_to_world_poses:
@@ -113,15 +114,16 @@
     if up is not None:
         # Aligning the look direction might mess up the up direction again
         up_directions = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction = np.mean(up_directions, axis=0)
         angle = angle_between_vectors(average_up_direction, up)
 
         # TODO: Here we assume that look direction should be z axis. Correct would be to rotate around look direction
-        rotator = Pose.from_euler(Vec3(0, 0, angle), pose_type=PoseType.CAM_2_CAM)
+        rotator = Pose(rotation_matrix_around_axis(look, angle), Vec3(), pose_type=PoseType.CAM_2_CAM)
+        # rotator = Pose.from_euler(Vec3(0, 0, angle), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator @ cam_pose for cam_pose in cam_to_world_poses]
         transformation = rotator @ transformation
 
         up_directions_after_alignment = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction_after_alignment = np.mean(up_directions_after_alignment, axis=0)
         assert average_up_direction_after_alignment.dot(up) > 0.9, \
             "Up directions could not be properly aligned. This can happen if the desired look direction is something else than the z-axis"
```

### Comparing `dreifus-0.1.8/src/dreifus/graphics.py` & `dreifus-0.1.9/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/image.py` & `dreifus-0.1.9/src/dreifus/image.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.1.9/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.1.9/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/pose_base.py` & `dreifus-0.1.9/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.1.9/src/dreifus/matrix/pose_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/pose_torch.py` & `dreifus-0.1.9/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.1.9/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/pyvista.py` & `dreifus-0.1.9/src/dreifus/pyvista.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/render.py` & `dreifus-0.1.9/src/dreifus/render.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/trajectory.py` & `dreifus-0.1.9/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/util/colormap.py` & `dreifus-0.1.9/src/dreifus/util/colormap.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/vector/vector_base.py` & `dreifus-0.1.9/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus/vector/vector_numpy.py` & `dreifus-0.1.9/src/dreifus/vector/vector_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import Optional, Tuple, Union, List
 
 import numpy as np
 
 # ==========================================================
 # 3D utilities
 # ==========================================================
+from scipy.linalg import expm, norm
+
 from dreifus.vector.vector_base import Vec3TypeX, unpack_3d_params, unpack_nd_params
 
 
 def rotation_matrix_between_vectors(vec1: Vec3TypeX, vec2: Vec3TypeX) -> np.ndarray:
     """ Find the rotation matrix that aligns vec1 to vec2
     :param vec1: A 3d "source" vector
     :param vec2: A 3d "destination" vector
@@ -26,14 +28,31 @@
         kmat = np.array([[0, -v[2], v[1]], [v[2], 0, -v[0]], [-v[1], v[0], 0]])
         return np.eye(3) + kmat + kmat.dot(kmat) * ((1 - c) / (s ** 2))
 
     else:
         return np.eye(3)  # cross of all zeros only occurs on identical directions
 
 
+def rotation_matrix_around_axis(axis: Vec3TypeX, theta: float) -> np.ndarray:
+    """
+    Computes a 3x3 rotation matrix that moves 3D points in space around the specified axis by theta radians.
+
+    Parameters
+    ----------
+        axis: Which axis to rotate around (always goes through origin)
+        theta: How much to rotate in radians. Rotation is applied in clockwise fashion (right-hand rotation)
+
+    Returns
+    -------
+        The 3x3 rotation matrix
+    """
+
+    return expm(np.cross(np.eye(3), axis / norm(axis) * theta))
+
+
 def angle_between_vectors(vec1: Vec3TypeX, vec2: Vec3TypeX) -> float:
     vec1 = Vec3(vec1)
     vec2 = Vec3(vec2)
     return math.acos(vec1.dot(vec2) / (vec1.length() * vec2.length()))
 
 
 def offset_vector_between_line_and_point(offset: Vec3TypeX, direction: Vec3TypeX, point: Vec3TypeX):
```

### Comparing `dreifus-0.1.8/src/dreifus/vector/vector_torch.py` & `dreifus-0.1.9/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/src/dreifus.egg-info/PKG-INFO` & `dreifus-0.1.9/src/dreifus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreifus
-Version: 0.1.8
+Version: 0.1.9
 Summary: dreifus lifts your 3D camera experience and facilitates computer vision applications
 Author-email: Tobias Kirschstein <tobias.kirschstein@gmail.com>
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
```

### Comparing `dreifus-0.1.8/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.1.9/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_camera.py` & `dreifus-0.1.9/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_camera_bundle.py` & `dreifus-0.1.9/test/test_camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_graphics.py` & `dreifus-0.1.9/test/test_graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_image.py` & `dreifus-0.1.9/test/test_image.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_intrinsics.py` & `dreifus-0.1.9/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_pose.py` & `dreifus-0.1.9/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.1.8/test/test_vector.py` & `dreifus-0.1.9/test/test_vector.py`

 * *Files identical despite different names*

