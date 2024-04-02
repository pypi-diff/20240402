# Comparing `tmp/pin_pink-2.0.0.tar.gz` & `tmp/pin_pink-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pin_pink-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pin_pink-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pin_pink-2.0.0.tar` & `pin_pink-2.1.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
--rw-r--r--   0        0        0      488 2024-02-07 11:27:28.651295 pin_pink-2.0.0/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     1269 2024-02-07 11:27:28.651295 pin_pink-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2843 2024-02-07 11:27:28.651295 pin_pink-2.0.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       77 2023-05-25 08:01:21.852593 pin_pink-2.0.0/.gitignore
--rw-r--r--   0        0        0     7386 2024-03-05 09:27:11.615650 pin_pink-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      570 2024-03-05 09:27:52.167241 pin_pink-2.0.0/CITATION.cff
--rw-r--r--   0        0        0     2172 2024-02-07 11:27:28.651295 pin_pink-2.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-25 08:01:21.852593 pin_pink-2.0.0/LICENSE
--rw-r--r--   0        0        0     8857 2024-03-05 09:28:02.639135 pin_pink-2.0.0/README.md
--rw-r--r--   0        0        0     9337 2024-03-01 14:31:11.751546 pin_pink-2.0.0/doc/conf.py
--rw-r--r--   0        0        0      968 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/css/custom.css
--rw-r--r--   0        0        0      372 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/developer-notes.rst
--rw-r--r--   0        0        0      279 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/environment.yml
--rw-r--r--   0        0        0    16030 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/images/apple-touch-icon-180x180.png
--rw-r--r--   0        0        0     1013 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/images/favicon-16x16.png
--rw-r--r--   0        0        0     1766 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/images/favicon-32x32.png
--rw-r--r--   0        0        0    18638 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/images/pink-round-corners-140x140.png
--rw-r--r--   0        0        0      981 2024-02-22 14:00:23.291147 pin_pink-2.0.0/doc/index.rst
--rw-r--r--   0        0        0      809 2024-02-22 13:55:14.742490 pin_pink-2.0.0/doc/installation.rst
--rw-r--r--   0        0        0     1930 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/introduction.rst
--rw-r--r--   0        0        0      844 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/inverse-kinematics.rst
--rw-r--r--   0        0        0      354 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/limits.rst
--rw-r--r--   0        0        0      632 2024-02-07 11:27:28.651295 pin_pink-2.0.0/doc/references.rst
--rw-r--r--   0        0        0      528 2024-02-22 13:58:38.292284 pin_pink-2.0.0/doc/tasks.rst
--rw-r--r--   0        0        0     1507 2024-02-07 11:27:28.651295 pin_pink-2.0.0/examples/README.md
--rw-r--r--   0        0        0     2690 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/arm_kinova_gen2.py
--rw-r--r--   0        0        0     2732 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/arm_ur3.py
--rw-r--r--   0        0        0     2748 2024-03-01 14:37:39.335282 pin_pink-2.0.0/examples/arm_ur5.py
--rw-r--r--   0        0        0     2548 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/double_pendulum.py
--rw-r--r--   0        0        0     1957 2024-03-01 14:37:39.347282 pin_pink-2.0.0/examples/end_effector_to_target.py
--rw-r--r--   0        0        0     6937 2024-03-01 14:37:39.335282 pin_pink-2.0.0/examples/flying_dual_arm_ur3.py
--rw-r--r--   0        0        0     4893 2024-03-01 14:37:39.335282 pin_pink-2.0.0/examples/humanoid_draco3.py
--rw-r--r--   0        0        0     4032 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/humanoid_jvrc.py
--rw-r--r--   0        0        0     3482 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/humanoid_sigmaban.py
--rw-r--r--   0        0        0      795 2024-03-01 14:33:19.518140 pin_pink-2.0.0/examples/load_custom_urdf.py
--rw-r--r--   0        0        0     2819 2024-03-01 14:33:21.390120 pin_pink-2.0.0/examples/meshcat_shapes.py
--rw-r--r--   0        0        0     2536 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/mobile_omni_wheeled_robot.py
--rw-r--r--   0        0        0     3417 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/mobile_stretch.py
--rw-r--r--   0        0        0     4719 2023-05-25 08:01:21.856593 pin_pink-2.0.0/examples/robots/double_pendulum.urdf
--rw-r--r--   0        0        0     2425 2023-05-25 08:01:21.856593 pin_pink-2.0.0/examples/robots/omnidirectional_wheeled_robot.urdf
--rw-r--r--   0        0        0     1480 2024-02-07 11:27:28.651295 pin_pink-2.0.0/examples/robots/simple_pendulum.urdf
--rw-r--r--   0        0        0     3268 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/simple_pendulum_configuration_limit.py
--rw-r--r--   0        0        0     3430 2024-03-01 14:37:39.323282 pin_pink-2.0.0/examples/visualize_in_meshcat.py
--rw-r--r--   0        0        0     3254 2024-03-01 14:37:39.327282 pin_pink-2.0.0/examples/visualize_in_yourdfpy.py
--rw-r--r--   0        0        0     3372 2024-03-01 14:37:39.327282 pin_pink-2.0.0/examples/wheeled_biped_upkie.py
--rw-r--r--   0        0        0      688 2024-03-05 09:27:23.879526 pin_pink-2.0.0/pink/__init__.py
--rw-r--r--   0        0        0     7097 2024-03-01 14:33:35.413965 pin_pink-2.0.0/pink/configuration.py
--rw-r--r--   0        0        0     2053 2024-03-01 14:33:37.557942 pin_pink-2.0.0/pink/exceptions.py
--rw-r--r--   0        0        0      338 2024-03-01 14:33:41.821895 pin_pink-2.0.0/pink/limits/__init__.py
--rw-r--r--   0        0        0     4016 2024-03-01 14:33:40.621908 pin_pink-2.0.0/pink/limits/configuration_limit.py
--rw-r--r--   0        0        0     1091 2024-03-01 14:33:43.117880 pin_pink-2.0.0/pink/limits/limit.py
--rw-r--r--   0        0        0     2877 2024-03-01 14:33:58.133715 pin_pink-2.0.0/pink/limits/velocity_limit.py
--rw-r--r--   0        0        0     5830 2024-03-01 14:34:01.197682 pin_pink-2.0.0/pink/solve_ik.py
--rw-r--r--   0        0        0      621 2024-03-01 14:34:06.909619 pin_pink-2.0.0/pink/tasks/__init__.py
--rw-r--r--   0        0        0     2453 2024-03-01 14:34:02.845663 pin_pink-2.0.0/pink/tasks/damping_task.py
--rw-r--r--   0        0        0      523 2024-03-01 14:34:04.621644 pin_pink-2.0.0/pink/tasks/exceptions.py
--rw-r--r--   0        0        0     9311 2024-03-01 14:34:06.037628 pin_pink-2.0.0/pink/tasks/frame_task.py
--rw-r--r--   0        0        0     2845 2024-03-01 14:34:08.469601 pin_pink-2.0.0/pink/tasks/joint_coupling_task.py
--rw-r--r--   0        0        0     7331 2024-03-01 14:34:09.829587 pin_pink-2.0.0/pink/tasks/linear_holonomic_task.py
--rw-r--r--   0        0        0     4171 2024-03-01 14:34:12.381559 pin_pink-2.0.0/pink/tasks/posture_task.py
--rw-r--r--   0        0        0     6778 2024-03-01 14:34:13.597545 pin_pink-2.0.0/pink/tasks/task.py
--rw-r--r--   0        0        0     3202 2024-03-01 14:34:15.437525 pin_pink-2.0.0/pink/utils.py
--rw-r--r--   0        0        0      620 2024-03-01 14:34:16.381515 pin_pink-2.0.0/pink/visualization.py
--rw-r--r--   0        0        0     1701 2024-02-07 11:27:28.655295 pin_pink-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      195 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0    14298 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_configuration.py
--rw-r--r--   0        0        0     3898 2024-03-01 14:34:18.669489 pin_pink-2.0.0/tests/test_configuration_limit.py
--rw-r--r--   0        0        0     1157 2024-03-01 14:34:21.589457 pin_pink-2.0.0/tests/test_damping_task.py
--rw-r--r--   0        0        0     9894 2024-03-01 14:34:23.181440 pin_pink-2.0.0/tests/test_frame_task.py
--rw-r--r--   0        0        0     3041 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_jacobians.py
--rw-r--r--   0        0        0     2426 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_joint_coupling_task.py
--rw-r--r--   0        0        0     3063 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_limits.py
--rw-r--r--   0        0        0     4581 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_linear_holonomic_task.py
--rw-r--r--   0        0        0     3741 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_posture_task.py
--rw-r--r--   0        0        0    11414 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_solve_ik.py
--rw-r--r--   0        0        0      574 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_task.py
--rw-r--r--   0        0        0     2034 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     1364 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tests/test_velocity_limit.py
--rw-r--r--   0        0        0     1371 2024-02-07 11:27:28.655295 pin_pink-2.0.0/tox.ini
--rw-r--r--   0        0        0    10173 1970-01-01 00:00:00.000000 pin_pink-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2024-02-07 11:27:28.651295 pin_pink-2.1.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     1269 2024-02-07 11:27:28.651295 pin_pink-2.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2843 2024-02-07 11:27:28.651295 pin_pink-2.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       77 2023-05-25 08:01:21.852593 pin_pink-2.1.0/.gitignore
+-rw-r--r--   0        0        0     7797 2024-04-02 09:54:04.920095 pin_pink-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2024-04-02 09:54:04.920095 pin_pink-2.1.0/CITATION.cff
+-rw-r--r--   0        0        0     2172 2024-02-07 11:27:28.651295 pin_pink-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-25 08:01:21.852593 pin_pink-2.1.0/LICENSE
+-rw-r--r--   0        0        0     8952 2024-04-02 09:54:04.920095 pin_pink-2.1.0/README.md
+-rw-r--r--   0        0        0     9337 2024-03-01 14:31:11.751546 pin_pink-2.1.0/doc/conf.py
+-rw-r--r--   0        0        0      968 2024-02-07 11:27:28.651295 pin_pink-2.1.0/doc/css/custom.css
+-rw-r--r--   0        0        0      368 2024-03-28 15:52:15.372598 pin_pink-2.1.0/doc/developer-notes.rst
+-rw-r--r--   0        0        0      279 2024-02-07 11:27:28.651295 pin_pink-2.1.0/doc/environment.yml
+-rw-r--r--   0        0        0    16030 2024-02-07 11:27:28.651295 pin_pink-2.1.0/doc/images/apple-touch-icon-180x180.png
+-rw-r--r--   0        0        0     1013 2024-02-07 11:27:28.651295 pin_pink-2.1.0/doc/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1766 2024-02-07 11:27:28.651295 pin_pink-2.1.0/doc/images/favicon-32x32.png
+-rw-r--r--   0        0        0     1006 2024-03-28 15:52:26.412474 pin_pink-2.1.0/doc/index.rst
+-rw-r--r--   0        0        0      805 2024-03-28 15:52:28.588450 pin_pink-2.1.0/doc/installation.rst
+-rw-r--r--   0        0        0     1836 2024-03-28 15:52:30.756426 pin_pink-2.1.0/doc/introduction.rst
+-rw-r--r--   0        0        0      840 2024-03-28 15:52:32.924401 pin_pink-2.1.0/doc/inverse-kinematics.rst
+-rw-r--r--   0        0        0      350 2024-03-28 15:52:35.164376 pin_pink-2.1.0/doc/limits.rst
+-rw-r--r--   0        0        0      628 2024-03-28 15:52:37.436351 pin_pink-2.1.0/doc/references.rst
+-rw-r--r--   0        0        0      524 2024-03-28 15:52:39.748325 pin_pink-2.1.0/doc/tasks.rst
+-rw-r--r--   0        0        0     1507 2024-02-07 11:27:28.651295 pin_pink-2.1.0/examples/README.md
+-rw-r--r--   0        0        0     2690 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/arm_kinova_gen2.py
+-rw-r--r--   0        0        0     2732 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/arm_ur3.py
+-rw-r--r--   0        0        0     2748 2024-03-01 14:37:39.335282 pin_pink-2.1.0/examples/arm_ur5.py
+-rw-r--r--   0        0        0     2548 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/double_pendulum.py
+-rw-r--r--   0        0        0     1935 2024-03-28 17:44:32.783862 pin_pink-2.1.0/examples/end_effector_to_target.py
+-rw-r--r--   0        0        0     6937 2024-03-01 14:37:39.335282 pin_pink-2.1.0/examples/flying_dual_arm_ur3.py
+-rw-r--r--   0        0        0     4893 2024-03-01 14:37:39.335282 pin_pink-2.1.0/examples/humanoid_draco3.py
+-rw-r--r--   0        0        0     4032 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/humanoid_jvrc.py
+-rw-r--r--   0        0        0     3482 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/humanoid_sigmaban.py
+-rw-r--r--   0        0        0      795 2024-03-01 14:33:19.518140 pin_pink-2.1.0/examples/load_custom_urdf.py
+-rw-r--r--   0        0        0     2819 2024-03-01 14:33:21.390120 pin_pink-2.1.0/examples/meshcat_shapes.py
+-rw-r--r--   0        0        0     2536 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/mobile_omni_wheeled_robot.py
+-rw-r--r--   0        0        0     3417 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/mobile_stretch.py
+-rw-r--r--   0        0        0     4719 2023-05-25 08:01:21.856593 pin_pink-2.1.0/examples/robots/double_pendulum.urdf
+-rw-r--r--   0        0        0     2425 2023-05-25 08:01:21.856593 pin_pink-2.1.0/examples/robots/omnidirectional_wheeled_robot.urdf
+-rw-r--r--   0        0        0     1480 2024-02-07 11:27:28.651295 pin_pink-2.1.0/examples/robots/simple_pendulum.urdf
+-rw-r--r--   0        0        0     3268 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/simple_pendulum_configuration_limit.py
+-rw-r--r--   0        0        0     3871 2024-04-02 09:41:44.483401 pin_pink-2.1.0/examples/stretch_relative_target.py
+-rw-r--r--   0        0        0     3571 2024-03-28 13:14:42.193565 pin_pink-2.1.0/examples/stretch_world_target.py
+-rw-r--r--   0        0        0     3430 2024-03-01 14:37:39.323282 pin_pink-2.1.0/examples/visualize_in_meshcat.py
+-rw-r--r--   0        0        0     3254 2024-03-01 14:37:39.327282 pin_pink-2.1.0/examples/visualize_in_yourdfpy.py
+-rw-r--r--   0        0        0     3372 2024-03-01 14:37:39.327282 pin_pink-2.1.0/examples/wheeled_biped_upkie.py
+-rw-r--r--   0        0        0      688 2024-04-02 09:54:04.920095 pin_pink-2.1.0/pink/__init__.py
+-rw-r--r--   0        0        0     8056 2024-04-02 09:41:44.483401 pin_pink-2.1.0/pink/configuration.py
+-rw-r--r--   0        0        0     2053 2024-03-01 14:33:37.557942 pin_pink-2.1.0/pink/exceptions.py
+-rw-r--r--   0        0        0      338 2024-03-01 14:33:41.821895 pin_pink-2.1.0/pink/limits/__init__.py
+-rw-r--r--   0        0        0     4016 2024-03-01 14:33:40.621908 pin_pink-2.1.0/pink/limits/configuration_limit.py
+-rw-r--r--   0        0        0     1091 2024-03-01 14:33:43.117880 pin_pink-2.1.0/pink/limits/limit.py
+-rw-r--r--   0        0        0     2877 2024-03-01 14:33:58.133715 pin_pink-2.1.0/pink/limits/velocity_limit.py
+-rw-r--r--   0        0        0     5830 2024-03-01 14:34:01.197682 pin_pink-2.1.0/pink/solve_ik.py
+-rw-r--r--   0        0        0      697 2024-03-28 13:14:42.193565 pin_pink-2.1.0/pink/tasks/__init__.py
+-rw-r--r--   0        0        0     2453 2024-03-01 14:34:02.845663 pin_pink-2.1.0/pink/tasks/damping_task.py
+-rw-r--r--   0        0        0      523 2024-03-01 14:34:04.621644 pin_pink-2.1.0/pink/tasks/exceptions.py
+-rw-r--r--   0        0        0     9314 2024-03-28 17:36:30.625325 pin_pink-2.1.0/pink/tasks/frame_task.py
+-rw-r--r--   0        0        0     2845 2024-03-01 14:34:08.469601 pin_pink-2.1.0/pink/tasks/joint_coupling_task.py
+-rw-r--r--   0        0        0     7331 2024-03-01 14:34:09.829587 pin_pink-2.1.0/pink/tasks/linear_holonomic_task.py
+-rw-r--r--   0        0        0     4171 2024-03-01 14:34:12.381559 pin_pink-2.1.0/pink/tasks/posture_task.py
+-rw-r--r--   0        0        0    10033 2024-04-02 09:41:44.483401 pin_pink-2.1.0/pink/tasks/relative_frame_task.py
+-rw-r--r--   0        0        0     6777 2024-03-28 16:22:25.623851 pin_pink-2.1.0/pink/tasks/task.py
+-rw-r--r--   0        0        0     3202 2024-03-01 14:34:15.437525 pin_pink-2.1.0/pink/utils.py
+-rw-r--r--   0        0        0      620 2024-03-01 14:34:16.381515 pin_pink-2.1.0/pink/visualization.py
+-rw-r--r--   0        0        0     1701 2024-03-11 12:47:53.724875 pin_pink-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    14374 2024-03-28 13:14:42.193565 pin_pink-2.1.0/tests/test_configuration.py
+-rw-r--r--   0        0        0     3845 2024-03-28 13:14:42.193565 pin_pink-2.1.0/tests/test_configuration_limit.py
+-rw-r--r--   0        0        0     1157 2024-03-01 14:34:21.589457 pin_pink-2.1.0/tests/test_damping_task.py
+-rw-r--r--   0        0        0     9894 2024-03-26 13:37:09.368565 pin_pink-2.1.0/tests/test_frame_task.py
+-rw-r--r--   0        0        0     3041 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_jacobians.py
+-rw-r--r--   0        0        0     2426 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_joint_coupling_task.py
+-rw-r--r--   0        0        0     3063 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_limits.py
+-rw-r--r--   0        0        0     4581 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_linear_holonomic_task.py
+-rw-r--r--   0        0        0     3741 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_posture_task.py
+-rw-r--r--   0        0        0     8613 2024-04-02 09:41:44.483401 pin_pink-2.1.0/tests/test_relative_frame_task.py
+-rw-r--r--   0        0        0    11414 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_solve_ik.py
+-rw-r--r--   0        0        0      574 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_task.py
+-rw-r--r--   0        0        0     2034 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1364 2024-02-07 11:27:28.655295 pin_pink-2.1.0/tests/test_velocity_limit.py
+-rw-r--r--   0        0        0     1371 2024-04-02 09:41:44.483401 pin_pink-2.1.0/tox.ini
+-rw-r--r--   0        0        0    10268 1970-01-01 00:00:00.000000 pin_pink-2.1.0/PKG-INFO
```

### Comparing `pin_pink-2.0.0/.github/workflows/docs.yml` & `pin_pink-2.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/.github/workflows/main.yml` & `pin_pink-2.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/CHANGELOG.md` & `pin_pink-2.1.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## Unreleased
+
+## [2.1.0] - 2024-04-02
+
+### Added
+
+- Function ``get_transform`` in the Configuration class
+- Task: relative frame task, where target is w.r.t another robot frame
+
+### Changed
+
+- Configuration: update function now accepts a configuration vector argument
+- Costs: setting cost in relative frame task now accepts plain float
+
 ## [2.0.0] - 2024-03-05
 
 ### Added
 
 - Add ``gain`` keyword argument to all task constructors where is makes sense
 - Damping task that minimizes joint velocities
 - Distribute package on conda-forge
@@ -254,15 +268,16 @@
 - Documentation reads versions from the main module
 - Remove unused mock imports
 
 ## [0.0.1] - 2022-02-06
 
 Python package infrastructure.
 
-[unreleased]: https://github.com/qpsolvers/qpsolvers/compare/v2.0.0...HEAD
+[unreleased]: https://github.com/qpsolvers/qpsolvers/compare/v2.1.0...HEAD
+[2.1.0]: https://github.com/qpsolvers/qpsolvers/compare/v2.0.0...v2.1.0
 [2.0.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.1.0...v2.0.0
 [1.1.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.0.0...v1.1.0
 [1.0.0]: https://github.com/qpsolvers/qpsolvers/compare/v0.11.0...v1.0.0
 [0.11.0]: https://github.com/qpsolvers/qpsolvers/compare/v0.10.0...v0.11.0
 [0.10.0]: https://github.com/qpsolvers/qpsolvers/compare/v0.9.0....v0.10.0
 [0.9.0]: https://github.com/qpsolvers/qpsolvers/compare/v0.8.0...v0.9.0
 [0.8.0]: https://github.com/qpsolvers/qpsolvers/compare/v0.7.0...v0.8.0
```

### Comparing `pin_pink-2.0.0/CITATION.cff` & `pin_pink-2.1.0/CITATION.cff`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cff-version: 1.2.0
 message: "If you find this code helpful, please cite it as below."
 title: "Pink: Python inverse kinematics based on Pinocchio"
-version: 2.0.0
-date-released: 2024-03-05
+version: 2.1.0
+date-released: 2024-04-02
 url: "https://github.com/stephane-caron/pink"
 license: "Apache-2.0"
 authors:
 - family-names: "Caron"
   given-names: "Stéphane"
   orcid: "https://orcid.org/0000-0003-2906-692X"
 - family-names: "De Mont-Marin"
```

### Comparing `pin_pink-2.0.0/CONTRIBUTING.md` & `pin_pink-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/LICENSE` & `pin_pink-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/README.md` & `pin_pink-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Pink
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/pink/main.yml?branch=main)](https://github.com/stephane-caron/pink/actions)
+[![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/pink/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/pink/)
 [![Coverage](https://coveralls.io/repos/github/stephane-caron/pink/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/pink?branch=main)
-[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://stephane-caron.github.io/pink/)
 [![Conda version](https://anaconda.org/conda-forge/pink/badges/version.svg)](https://anaconda.org/conda-forge/pink)
 [![PyPI version](https://img.shields.io/pypi/v/pin-pink)](https://pypi.org/project/pin-pink/)
 
 **P**ython **in**verse **k**inematics for articulated robot models, based on [Pinocchio](https://github.com/stack-of-tasks/pinocchio).
 
 ![Banner for Pink v0.5.0](https://user-images.githubusercontent.com/1189580/192318997-ed7574c3-8238-451d-9548-a769d46ec03b.png)
 
@@ -152,25 +152,25 @@
 If you use Pink in your scientific works, please cite it *e.g.* as follows:
 
 ```bibtex
 @software{pink2024,
   title = {{Pink: Python inverse kinematics based on Pinocchio}},
   author = {Caron, Stéphane and De Mont-Marin, Yann and Budhiraja, Rohan and Bang, Seung Hyeon},
   license = {Apache-2.0},
-  month = mar,
   url = {https://github.com/stephane-caron/pink},
-  version = {2.0.0},
+  version = {2.1.0},
   year = {2024}
 }
 ```
 
 ## See also
 
 Software:
 
 - [Jink.jl](https://github.com/adubredu/Jink.jl): Julia package for differential multi-task inverse kinematics.
+- [PlaCo](https://github.com/rhoban/placo): C++ inverse kinematics based on Pinocchio.
 - [pymanoid](https://github.com/stephane-caron/pymanoid): precursor to Pink based on OpenRAVE.
 
 Technical notes:
 
 - [Inverse kinematics](https://scaron.info/robotics/inverse-kinematics.html): a general introduction to differential inverse kinematics.
 - [Jacobian of a kinematic task and derivatives on manifolds](https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html).
```

### Comparing `pin_pink-2.0.0/doc/conf.py` & `pin_pink-2.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/doc/css/custom.css` & `pin_pink-2.1.0/doc/css/custom.css`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/doc/images/apple-touch-icon-180x180.png` & `pin_pink-2.1.0/doc/images/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/doc/images/favicon-16x16.png` & `pin_pink-2.1.0/doc/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/doc/images/favicon-32x32.png` & `pin_pink-2.1.0/doc/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/doc/index.rst` & `pin_pink-2.1.0/doc/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/index.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/index.rst
 
 .. title:: Table of Contents
 
 ####
 Pink
 ####
 
-.. image:: images/pink-round-corners-140x140.png
-   :height: 140px
-   :alt: alternate text
-   :align: right
-
 **P**\ ython **in**\ verse **k**\ inematics for articulated robot models, based on `Pinocchio <https://github.com/stack-of-tasks/pinocchio>`_.
 
+.. image:: https://user-images.githubusercontent.com/1189580/192318997-ed7574c3-8238-451d-9548-a769d46ec03b.png
+   :alt: Banner for Pink
+
 Inverse kinematics in Pink is defined by weighted :ref:`tasks <Tasks>` and :ref:`limits <Limits>`. The library adds a :ref:`configuration <Configuration>` type to Pinocchio, a configuration being a robot model and data to which forward kinematics have been applied. Given a configuration, tasks and a time step, :func:`pink.solve_ik.solve_ik` computes joint velocities that steer the model towards fulfilling all tasks at best.
 
 .. toctree::
     :maxdepth: 1
 
     installation.rst
     introduction.rst
```

### Comparing `pin_pink-2.0.0/doc/installation.rst` & `pin_pink-2.1.0/doc/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/installation.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/installation.rst
 
 ************
 Installation
 ************
 
 From Conda
 ==========
```

### Comparing `pin_pink-2.0.0/doc/introduction.rst` & `pin_pink-2.1.0/doc/introduction.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/introduction.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/introduction.rst
 
 ************
 Introduction
 ************
 
 Inverse kinematics (IK) is the problem of computing *motions* (in Pink: velocities) that achieve a given set of *tasks*, such as putting a foot on a surface, moving the center of mass to a target location, etc.
 
-This documentation assumes you are already familiar with task-based inverse kinematics. You can check out for instance this `note on inverse kinematics <https://scaron.info/robot-locomotion/inverse-kinematics.html>`__ for a general introduction.
+This documentation assumes you are already familiar with task-based inverse kinematics. You can check out for instance this `post on inverse kinematics <https://scaron.info/robot-locomotion/inverse-kinematics.html>`__ for a general introduction.
 
 Notations
 =========
 
 In Pink, we adopt the subscript right-to-left convention for transforms, and superscript notation to indicate the frame of a motion or force vector:
 
 .. list-table::
@@ -19,31 +19,29 @@
 
     * - Quantity
       - Notation
     * - Affine transform from frame :math:`A` to frame :math:`B`
       - :math:`T_{BA}`
     * - Body angular velocity of frame :math:`A` in frame :math:`B`
       - :math:`{}^A \omega_{BA}`
-    * - Plücker transform from frame :math:`A` to frame :math:`B`
-      - :math:`X_{BA}`
     * - Position of frame :math:`B` in frame :math:`A`
       - :math:`{}^A p_B`
     * - Rotation matrix from frame :math:`A` to frame :math:`B`
       - :math:`R_{BA}`
     * - Spatial angular velocity of frame :math:`A` in frame :math:`B`
       - :math:`{}^B \omega_{BA}`
     * - World frame (inertial)
       - :math:`W`
 
 With these notations frame transforms can be read left to right, for example:
 
 .. raw:: latex html
 
     \begin{align}
-    X_{CA} & = X_{CB} X_{BA} &
+    T_{CA} & = T_{CB} T_{BA} &
     {}^{B} \omega & = R_{BA} {}^{A} \omega &
     {}^B p_C & = R_{BA} {}^A p_C + {}^B p_A
     \end{align}
 
 See also this `spatial algebra cheat sheet
 <https://scaron.info/robot-locomotion/spatial-vector-algebra-cheat-sheet.html>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pin_pink-2.0.0/doc/inverse-kinematics.rst` & `pin_pink-2.1.0/doc/inverse-kinematics.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/inverse-kinematics.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/inverse-kinematics.rst
 
 ******************
 Inverse kinematics
 ******************
 
 The main function solve inverse kinematics is :func:`.solve_ik`. Here is for
 instance how it appears in a closed-loop inverse kinematics:
```

### Comparing `pin_pink-2.0.0/doc/references.rst` & `pin_pink-2.1.0/doc/references.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/references.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/references.rst
 
 **********
 References
 **********
 
 .. [FrameTaskJacobian] `Jacobian of a kinematic task and derivatives on manifolds <https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html>`_. S. Caron. 2023.
```

### Comparing `pin_pink-2.0.0/doc/tasks.rst` & `pin_pink-2.1.0/doc/tasks.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:github_url: https://github.com/stephane-caron/pink/tree/main/doc/src/tasks.rst
+:github_url: https://github.com/stephane-caron/pink/tree/main/doc/tasks.rst
 
 .. _Tasks:
 
 *****
 Tasks
 *****
```

### Comparing `pin_pink-2.0.0/examples/README.md` & `pin_pink-2.1.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/arm_kinova_gen2.py` & `pin_pink-2.1.0/examples/arm_kinova_gen2.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/arm_ur3.py` & `pin_pink-2.1.0/examples/arm_ur3.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/arm_ur5.py` & `pin_pink-2.1.0/examples/arm_ur5.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/double_pendulum.py` & `pin_pink-2.1.0/examples/double_pendulum.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/end_effector_to_target.py` & `pin_pink-2.1.0/examples/end_effector_to_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,46 +29,46 @@
         pinocchio.FrameType.OP_FRAME,
     )
 )
 robot.data = pinocchio.Data(robot.model)
 low = robot.model.lowerPositionLimit
 high = robot.model.upperPositionLimit
 robot.q0 = pinocchio.neutral(robot.model)
-# Task Details:
-np.random.seed(0)
 
+# Task details
+np.random.seed(0)
 q_final = np.array(
     [
         np.random.uniform(low=low[i], high=high[i], size=(1,))[0]
         for i in range(6)
     ]
 )
 pinocchio.forwardKinematics(robot.model, robot.data, q_final)
 
 target_pose = robot.data.oMi[parent_joint]
 ee_task = pink.tasks.FrameTask(FRAME_NAME, [1.0, 1.0, 1.0], [1.0, 1.0, 1.0])
 ee_task.set_target(target_pose)
 tasks = [ee_task]
 
-# IK:
+# Inverse kinematics parameters
 dt = 1e-2
 damping = 1e-8
-niter = 10000
+n_iter = 10000
 solver = "quadprog"
 
-pink_configuration = pink.Configuration(robot.model, robot.data, robot.q0)
+configuration = pink.Configuration(robot.model, robot.data, robot.q0)
 
-for i in range(niter):
+for i in range(n_iter):
     dv = pink.solve_ik(
-        pink_configuration,
-        [ee_task],  # , config_task],
+        configuration,
+        [ee_task],
         dt=dt,
         damping=damping,
         solver=solver,
     )
-    q_out = pinocchio.integrate(robot.model, pink_configuration.q, dv * dt)
-    pink_configuration = pink.Configuration(robot.model, robot.data, q_out)
+    q_out = pinocchio.integrate(robot.model, configuration.q, dv * dt)
+    configuration = pink.Configuration(robot.model, robot.data, q_out)
     pinocchio.updateFramePlacements(robot.model, robot.data)
-    err = ee_task.compute_error(pink_configuration)
+    err = ee_task.compute_error(configuration)
     print(i, err)
-    if np.linalg.norm(ee_task.compute_error(pink_configuration)) < 1e-8:
+    if np.linalg.norm(ee_task.compute_error(configuration)) < 1e-8:
         break
```

### Comparing `pin_pink-2.0.0/examples/flying_dual_arm_ur3.py` & `pin_pink-2.1.0/examples/flying_dual_arm_ur3.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/humanoid_draco3.py` & `pin_pink-2.1.0/examples/humanoid_draco3.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/humanoid_jvrc.py` & `pin_pink-2.1.0/examples/humanoid_jvrc.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/humanoid_sigmaban.py` & `pin_pink-2.1.0/examples/humanoid_sigmaban.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/load_custom_urdf.py` & `pin_pink-2.1.0/examples/load_custom_urdf.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/meshcat_shapes.py` & `pin_pink-2.1.0/examples/meshcat_shapes.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/mobile_omni_wheeled_robot.py` & `pin_pink-2.1.0/examples/mobile_omni_wheeled_robot.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/mobile_stretch.py` & `pin_pink-2.1.0/examples/mobile_stretch.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/robots/double_pendulum.urdf` & `pin_pink-2.1.0/examples/robots/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/robots/omnidirectional_wheeled_robot.urdf` & `pin_pink-2.1.0/examples/robots/omnidirectional_wheeled_robot.urdf`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/robots/simple_pendulum.urdf` & `pin_pink-2.1.0/examples/robots/simple_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/simple_pendulum_configuration_limit.py` & `pin_pink-2.1.0/examples/simple_pendulum_configuration_limit.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/visualize_in_meshcat.py` & `pin_pink-2.1.0/examples/visualize_in_meshcat.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/visualize_in_yourdfpy.py` & `pin_pink-2.1.0/examples/visualize_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/examples/wheeled_biped_upkie.py` & `pin_pink-2.1.0/examples/wheeled_biped_upkie.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/__init__.py` & `pin_pink-2.1.0/pink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     JointCouplingTask,
     LinearHolonomicTask,
     PostureTask,
     Task,
 )
 from .utils import custom_configuration_vector
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 __all__ = [
     "Configuration",
     "FrameTask",
     "JointCouplingTask",
     "LinearHolonomicTask",
     "PostureTask",
```

### Comparing `pin_pink-2.0.0/pink/configuration.py` & `pin_pink-2.1.0/pink/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 Pink uses `Pinocchio <https://github.com/stack-of-tasks/pinocchio>`__ for
 forward kinematics. A :class:`Configuration` is a pair of Pinocchio model and
 data where forward kinematics have been run, indicating that frame transforms
 and frame Jacobians used for IK can be queried.
 """
 
+from typing import Optional
+
 import numpy as np
 import pinocchio as pin
 
 from .exceptions import FrameNotFound, NotWithinConfigurationLimits
 from .limits import ConfigurationLimit, VelocityLimit
 from .utils import VectorSpace, get_root_joint_dim
 
@@ -85,18 +87,26 @@
         q_readonly.setflags(write=False)
         self.data = data.copy() if copy_data else data
         self.model = model
         self.q = q_readonly
         self.tangent = model.tangent
         #
         if forward_kinematics:
-            self.update()
+            self.update(None)
+
+    def update(self, q: Optional[np.ndarray] = None) -> None:
+        """Update configuration to a new vector and run forward kinematics.
 
-    def update(self) -> None:
-        """Run forward kinematics from the configuration."""
+        Args:
+            q: New configuration vector.
+        """
+        if q is not None:
+            q_readonly = q.copy()
+            q_readonly.setflags(write=False)
+            self.q = q_readonly
         pin.computeJointJacobians(self.model, self.data, self.q)
         pin.updateFramePlacements(self.model, self.data)
 
     def check_limits(self, tol: float = 1e-6) -> None:
         """Check that the current configuration is within limits.
 
         Args:
@@ -169,14 +179,31 @@
         """
         frame_id = self.model.getFrameId(frame)
         try:
             return self.data.oMf[frame_id].copy()
         except IndexError as index_error:
             raise FrameNotFound(frame, self.model.frames) from index_error
 
+    def get_transform(self, source: str, dest: str) -> pin.SE3:
+        """Get the pose of a frame with respect to another frame.
+
+        Args:
+            source: Name of the frame to get the pose of.
+            dest: Name of the frame to get the pose in.
+
+        Returns:
+            Current transform from the source frame to the dest frame.
+
+        Raises:
+            KeyError: if any of the frame names is not found in the model.
+        """
+        transform_source_to_world = self.get_transform_frame_to_world(source)
+        transform_dest_to_world = self.get_transform_frame_to_world(dest)
+        return transform_dest_to_world.actInv(transform_source_to_world)
+
     def integrate(self, velocity, dt) -> np.ndarray:
         """Integrate a velocity starting from the current configuration.
 
         Args:
             velocity: Velocity in tangent space.
             dt: Integration duration in [s].
 
@@ -188,9 +215,9 @@
     def integrate_inplace(self, velocity, dt) -> None:
         """Integrate a velocity starting from the current configuration.
 
         Args:
             velocity: Velocity in tangent space.
             dt: Integration duration in [s].
         """
-        self.q = pin.integrate(self.model, self.q, velocity * dt)
-        self.update()
+        q = pin.integrate(self.model, self.q, velocity * dt)
+        self.update(q)
```

### Comparing `pin_pink-2.0.0/pink/exceptions.py` & `pin_pink-2.1.0/pink/exceptions.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/limits/configuration_limit.py` & `pin_pink-2.1.0/pink/limits/configuration_limit.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/limits/limit.py` & `pin_pink-2.1.0/pink/limits/limit.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/limits/velocity_limit.py` & `pin_pink-2.1.0/pink/limits/velocity_limit.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/solve_ik.py` & `pin_pink-2.1.0/pink/solve_ik.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/__init__.py` & `pin_pink-2.1.0/pink/tasks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 from .damping_task import DampingTask
 from .exceptions import TargetNotSet, TaskJacobianNotSet
 from .frame_task import FrameTask
 from .joint_coupling_task import JointCouplingTask
 from .linear_holonomic_task import LinearHolonomicTask
 from .posture_task import PostureTask
+from .relative_frame_task import RelativeFrameTask
 from .task import Task
 
 __all__ = [
     "DampingTask",
     "FrameTask",
+    "RelativeFrameTask",
     "TargetNotSet",
     "TaskJacobianNotSet",
     "JointCouplingTask",
     "LinearHolonomicTask",
     "PostureTask",
     "Task",
 ]
```

### Comparing `pin_pink-2.0.0/pink/tasks/damping_task.py` & `pin_pink-2.1.0/pink/tasks/damping_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/exceptions.py` & `pin_pink-2.1.0/pink/tasks/exceptions.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/frame_task.py` & `pin_pink-2.1.0/pink/tasks/frame_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,18 @@
             configuration: Robot configuration.
         """
         self.set_target(configuration.get_transform_frame_to_world(self.frame))
 
     def compute_error(self, configuration: Configuration) -> np.ndarray:
         r"""Compute frame task error.
 
-        Mathematically this error is a twist :math:`e(q) \in se(3)` expressed
-        in the local frame (i.e., it is a *body* twist). We map it to
-        :math:`\mathbb{R}^6` using Pinocchio's convention where linear
-        coordinates are followed by angular coordinates.
+        This error is a twist :math:`e(q) \in se(3)` expressed in the local
+        frame (i.e. it is a *body* twist). We map it to :math:`\mathbb{R}^6`
+        using Pinocchio's convention where linear coordinates are followed by
+        angular coordinates.
 
         The error is the right-minus difference between the target pose
         :math:`T_{0t}` and current frame pose :math:`T_{0b}`:
 
         .. math::
 
             e(q) := {}_b \xi_{0b} = -(T_{t0} \boxminus T_{b0})
@@ -195,14 +195,16 @@
     def compute_jacobian(self, configuration: Configuration) -> np.ndarray:
         r"""Compute the frame task Jacobian.
 
         The task Jacobian :math:`J(q) \in \mathbb{R}^{6 \times n_v}` is the
         derivative of the task error :math:`e(q) \in \mathbb{R}^6` with respect
         to the configuration :math:`q`. The formula for the frame task is:
 
+        .. math::
+
             J(q) = -\text{Jlog}_6(T_{tb}) {}_b J_{0b}(q)
 
         The derivation of the formula for this Jacobian is detailed in
         [FrameTaskJacobian]_. See also :func:`Task.compute_jacobian` for more
         context on task Jacobians.
 
         Args:
```

### Comparing `pin_pink-2.0.0/pink/tasks/joint_coupling_task.py` & `pin_pink-2.1.0/pink/tasks/joint_coupling_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/linear_holonomic_task.py` & `pin_pink-2.1.0/pink/tasks/linear_holonomic_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/posture_task.py` & `pin_pink-2.1.0/pink/tasks/posture_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/tasks/task.py` & `pin_pink-2.1.0/pink/tasks/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             J(q) \Delta q = -\alpha e(q)
 
         The Jacobian matrix :math:`J(q) \in \mathbb{R}^{k \times n_v}`, with
         :math:`n_v` the dimension of the robot's tangent space, is the
         derivative of the task error :math:`e(q)` with respect to the
         configuration :math:`q \in \mathbb{R}^{n_q}`. This Jacobian is
         implemented in :func:`Task.compute_jacobian`. Finally, the
-        configuration displacement :math:`\\Delta q` is the output of inverse
+        configuration displacement :math:`\Delta q` is the output of inverse
         kinematics.
 
         In the first-order task dynamics, the error :math:`e(q)` is multiplied
         by the task gain :math:`\alpha \in [0, 1]`. This gain can be one for
         dead-beat control (*i.e.* converge as fast as possible, but might be
         unstable as it neglects our first-order approximation), but it can also
         be lower a slower task (similar to low-pass filtering).
```

### Comparing `pin_pink-2.0.0/pink/utils.py` & `pin_pink-2.1.0/pink/utils.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pink/visualization.py` & `pin_pink-2.1.0/pink/visualization.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/pyproject.toml` & `pin_pink-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "loop-rate-limiters >=0.1.0",
     "numpy >=1.19.0",
     "pin >=2.6.3",
-    "qpsolvers >=2.5.0",
+    "qpsolvers >=4.3.1",
     "quadprog >=0.1.11",
 ]
 keywords = ["inverse", "kinematics", "pinocchio"]
 
 [project.urls]
 Documentation = "https://stephane-caron.github.io/pink/"
 Source = "https://github.com/stephane-caron/pink"
```

### Comparing `pin_pink-2.0.0/tests/test_configuration.py` & `pin_pink-2.1.0/tests/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 class TestConfiguration(unittest.TestCase):
     """Test configuration type."""
 
     def test_constructor(self):
         """Constructing a configuration computes Jacobians."""
         robot = load_robot_description(
-            "jvrc_description", root_joint=pin.JointModelFreeFlyer()
+            "jvrc_description",
+            root_joint=pin.JointModelFreeFlyer(),
+            commit="9ff8efbc7043459a8f0892662bd030d8020fb682",
         )
         robot.data.J.fill(42.0)
         configuration = Configuration(robot.model, robot.data, robot.q0)
         J_check = np.array(
             [
                 [
                     1.0,
@@ -105,34 +107,34 @@
                     0.0,
                     0.522,
                     0.0,
                     0.0,
                     -0.0,
                     -0.022,
                     -0.0,
-                    -0.124,
-                    -0.169,
-                    -0.124,
-                    -0.169,
+                    -0.106,
+                    -0.151,
+                    -0.106,
+                    -0.151,
                     -0.106,
                     -0.151,
                     0.003,
                     0.645,
                     0.0,
                     0.0,
                     0.522,
                     0.0,
                     0.0,
                     -0.0,
                     -0.022,
                     -0.0,
-                    -0.124,
-                    -0.169,
-                    -0.124,
-                    -0.169,
+                    -0.106,
+                    -0.151,
+                    -0.106,
+                    -0.151,
                     -0.106,
                     -0.151,
                 ],
                 [
                     0.0,
                     0.0,
                     1.0,
@@ -157,36 +159,36 @@
                     0.0,
                     -0.24,
                     0.0,
                     0.004,
                     0.0,
                     -0.24,
                     0.0,
-                    -0.246,
-                    -0.246,
-                    -0.246,
-                    -0.246,
-                    -0.217,
-                    -0.217,
+                    -0.256,
+                    -0.256,
+                    -0.256,
+                    -0.256,
+                    -0.207,
+                    -0.207,
                     -0.0,
                     -0.0,
                     -0.003,
                     0.0,
                     0.24,
                     0.0,
                     0.004,
                     0.0,
                     0.24,
                     0.0,
-                    0.246,
-                    0.246,
-                    0.246,
-                    0.246,
-                    0.217,
-                    0.217,
+                    0.256,
+                    0.256,
+                    0.256,
+                    0.256,
+                    0.207,
+                    0.207,
                 ],
                 [
                     0.0,
                     0.0,
                     0.0,
                     1.0,
                     0.0,
```

### Comparing `pin_pink-2.0.0/tests/test_configuration_limit.py` & `pin_pink-2.1.0/tests/test_configuration_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,23 +59,23 @@
             This test works with a commit-pinned description of Upkie. It will
             not work for any description, as a robot may have e.g. some
             velocity-unbounded joints.
         """
         robot = load_robot_description(
             "upkie_description",
             root_joint=pin.JointModelFreeFlyer(),
-            # https://github.com/robot-descriptions/robot_descriptions.py/issues/31
-            # commit="62f3ba24c2045b44faedb7c6c6167e74e157b49e",
+            commit="62f3ba24c2045b44faedb7c6c6167e74e157b49e",
         )
+        dt = 1e-3  # [s]
         configuration = Configuration(robot.model, robot.data, robot.q0)
         limit = ConfigurationLimit(robot.model)
-        G, h = limit.compute_qp_inequalities(robot.q0, dt=1e-3)
+        G, h = limit.compute_qp_inequalities(robot.q0, dt=dt)
         v_lim = configuration.model.velocityLimit
-        self.assertLess(np.max(+G @ v_lim - h), -tol)
-        self.assertLess(np.max(-G @ v_lim - h), -tol)
+        self.assertLess(np.max(+G @ v_lim * dt - h), -tol)
+        self.assertLess(np.max(-G @ v_lim * dt - h), -tol)
 
     def test_configuration_limit_repulsion(self, tol=1e-10):
         """Velocities are scaled down when close to a configuration limit.
 
         Args:
             tol: Numerical tolerance.
         """
```

### Comparing `pin_pink-2.0.0/tests/test_damping_task.py` & `pin_pink-2.1.0/tests/test_damping_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_frame_task.py` & `pin_pink-2.1.0/tests/test_frame_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_jacobians.py` & `pin_pink-2.1.0/tests/test_jacobians.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_joint_coupling_task.py` & `pin_pink-2.1.0/tests/test_joint_coupling_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_limits.py` & `pin_pink-2.1.0/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_linear_holonomic_task.py` & `pin_pink-2.1.0/tests/test_linear_holonomic_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_posture_task.py` & `pin_pink-2.1.0/tests/test_posture_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_solve_ik.py` & `pin_pink-2.1.0/tests/test_solve_ik.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_task.py` & `pin_pink-2.1.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_utils.py` & `pin_pink-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tests/test_velocity_limit.py` & `pin_pink-2.1.0/tests/test_velocity_limit.py`

 * *Files identical despite different names*

### Comparing `pin_pink-2.0.0/tox.ini` & `pin_pink-2.1.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 
 [testenv]
 deps =
     numpy
     pin >=2.6.4
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=1.4.1
+    robot_descriptions >=1.9.0
 commands =
     python -m unittest discover --failfast
 
 [testenv:coverage]
 deps =
     coverage
     numpy
     pin >=2.6.4
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=1.4.1
+    robot_descriptions >=1.9.0
 commands =
     coverage erase
     coverage run -m unittest discover --failfast
     coverage report --include="pink/*"
 
 [testenv:lint]
 deps =
     black >=22.10.0
     ruff >=0.0.220
     mypy >=0.812
     pin >=2.6.4
     pylint >=2.8.2
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=1.4.1
+    robot_descriptions >=1.9.0
 commands =
     black --check --diff pink
     ruff pink
     pylint pink --exit-zero --rcfile={toxinidir}/tox.ini
     mypy pink --ignore-missing-imports
 
 [pylint]
```

### Comparing `pin_pink-2.0.0/PKG-INFO` & `pin_pink-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pin-pink
-Version: 2.0.0
+Version: 2.1.0
 Summary: Inverse kinematics for articulated robot models, based on Pinocchio.
 Keywords: inverse,kinematics,pinocchio
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,26 +16,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: loop-rate-limiters >=0.1.0
 Requires-Dist: numpy >=1.19.0
 Requires-Dist: pin >=2.6.3
-Requires-Dist: qpsolvers >=2.5.0
+Requires-Dist: qpsolvers >=4.3.1
 Requires-Dist: quadprog >=0.1.11
 Project-URL: Changelog, https://github.com/stephane-caron/pink/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://stephane-caron.github.io/pink/
 Project-URL: Source, https://github.com/stephane-caron/pink
 Project-URL: Tracker, https://github.com/stephane-caron/pink/issues
 
 # Pink
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/pink/main.yml?branch=main)](https://github.com/stephane-caron/pink/actions)
+[![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/pink/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/pink/)
 [![Coverage](https://coveralls.io/repos/github/stephane-caron/pink/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/pink?branch=main)
-[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://stephane-caron.github.io/pink/)
 [![Conda version](https://anaconda.org/conda-forge/pink/badges/version.svg)](https://anaconda.org/conda-forge/pink)
 [![PyPI version](https://img.shields.io/pypi/v/pin-pink)](https://pypi.org/project/pin-pink/)
 
 **P**ython **in**verse **k**inematics for articulated robot models, based on [Pinocchio](https://github.com/stack-of-tasks/pinocchio).
 
 ![Banner for Pink v0.5.0](https://user-images.githubusercontent.com/1189580/192318997-ed7574c3-8238-451d-9548-a769d46ec03b.png)
 
@@ -181,26 +181,26 @@
 If you use Pink in your scientific works, please cite it *e.g.* as follows:
 
 ```bibtex
 @software{pink2024,
   title = {{Pink: Python inverse kinematics based on Pinocchio}},
   author = {Caron, Stéphane and De Mont-Marin, Yann and Budhiraja, Rohan and Bang, Seung Hyeon},
   license = {Apache-2.0},
-  month = mar,
   url = {https://github.com/stephane-caron/pink},
-  version = {2.0.0},
+  version = {2.1.0},
   year = {2024}
 }
 ```
 
 ## See also
 
 Software:
 
 - [Jink.jl](https://github.com/adubredu/Jink.jl): Julia package for differential multi-task inverse kinematics.
+- [PlaCo](https://github.com/rhoban/placo): C++ inverse kinematics based on Pinocchio.
 - [pymanoid](https://github.com/stephane-caron/pymanoid): precursor to Pink based on OpenRAVE.
 
 Technical notes:
 
 - [Inverse kinematics](https://scaron.info/robotics/inverse-kinematics.html): a general introduction to differential inverse kinematics.
 - [Jacobian of a kinematic task and derivatives on manifolds](https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html).
```

