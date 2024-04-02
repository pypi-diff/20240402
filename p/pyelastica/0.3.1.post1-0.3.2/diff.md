# Comparing `tmp/pyelastica-0.3.1.post1.tar.gz` & `tmp/pyelastica-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelastica-0.3.1.post1.tar", max compression
+gzip compressed data, was "pyelastica-0.3.2.tar", max compression
```

## Comparing `pyelastica-0.3.1.post1.tar` & `pyelastica-0.3.2.tar`

### file list

```diff
@@ -1,57 +1,66 @@
--rw-r--r--   0        0        0     1072 2023-05-12 22:18:14.329239 pyelastica-0.3.1.post1/LICENSE
--rw-r--r--   0        0        0     9620 2023-05-12 23:22:02.521652 pyelastica-0.3.1.post1/README.md
--rw-r--r--   0        0        0     2272 2023-05-12 22:18:14.332679 pyelastica-0.3.1.post1/elastica/__init__.py
--rw-r--r--   0        0        0     9877 2023-05-12 22:18:14.332807 pyelastica-0.3.1.post1/elastica/_calculus.py
--rw-r--r--   0        0        0     9879 2023-05-12 22:18:14.332934 pyelastica-0.3.1.post1/elastica/_linalg.py
--rw-r--r--   0        0        0    11780 2023-05-12 22:18:14.333063 pyelastica-0.3.1.post1/elastica/_rotations.py
--rw-r--r--   0        0        0     3505 2023-05-12 22:18:14.333284 pyelastica-0.3.1.post1/elastica/_synchronize_periodic_boundary.py
--rw-r--r--   0        0        0    27380 2023-05-12 22:18:14.333604 pyelastica-0.3.1.post1/elastica/boundary_conditions.py
--rw-r--r--   0        0        0     8541 2023-05-12 22:18:14.333749 pyelastica-0.3.1.post1/elastica/callback_functions.py
--rw-r--r--   0        0        0    11358 2022-05-30 02:18:59.374910 pyelastica-0.3.1.post1/elastica/collision/AABBCollection.py
--rw-r--r--   0        0        0    12044 2023-05-12 22:18:14.333890 pyelastica-0.3.1.post1/elastica/dissipation.py
--rw-r--r--   0        0        0        0 2022-05-30 02:18:59.375000 pyelastica-0.3.1.post1/elastica/experimental/__init__.py
--rw-r--r--   0        0        0    15823 2023-05-12 22:18:14.334053 pyelastica-0.3.1.post1/elastica/experimental/connection_contact_joint/generic_system_type_connection.py
--rw-r--r--   0        0        0     9642 2023-05-12 19:16:52.744915 pyelastica-0.3.1.post1/elastica/experimental/connection_contact_joint/parallel_connection.py
--rw-r--r--   0        0        0     5850 2023-05-12 22:18:14.334171 pyelastica-0.3.1.post1/elastica/experimental/interaction.py
--rw-r--r--   0        0        0    18842 2023-05-12 22:18:14.334323 pyelastica-0.3.1.post1/elastica/external_forces.py
--rw-r--r--   0        0        0    35996 2023-05-12 22:18:14.334677 pyelastica-0.3.1.post1/elastica/interaction.py
--rw-r--r--   0        0        0    39414 2023-05-12 22:18:14.334909 pyelastica-0.3.1.post1/elastica/joint.py
--rw-r--r--   0        0        0      111 2023-05-12 22:18:14.335015 pyelastica-0.3.1.post1/elastica/memory_block/__init__.py
--rw-r--r--   0        0        0     7515 2023-05-12 22:18:14.335246 pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rigid_body.py
--rw-r--r--   0        0        0    27041 2023-05-12 22:18:14.335399 pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rod.py
--rw-r--r--   0        0        0     7761 2023-05-12 22:18:14.335506 pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rod_base.py
--rw-r--r--   0        0        0      390 2023-05-12 22:18:14.335613 pyelastica-0.3.1.post1/elastica/modules/__init__.py
--rw-r--r--   0        0        0     7657 2023-05-12 22:18:14.335859 pyelastica-0.3.1.post1/elastica/modules/base_system.py
--rw-r--r--   0        0        0     4726 2023-05-12 19:16:52.746366 pyelastica-0.3.1.post1/elastica/modules/callbacks.py
--rw-r--r--   0        0        0     9701 2023-05-12 19:16:52.746449 pyelastica-0.3.1.post1/elastica/modules/connections.py
--rw-r--r--   0        0        0     6627 2023-05-12 22:18:14.336039 pyelastica-0.3.1.post1/elastica/modules/constraints.py
--rw-r--r--   0        0        0     4170 2023-05-12 19:16:52.746631 pyelastica-0.3.1.post1/elastica/modules/damping.py
--rw-r--r--   0        0        0     5741 2023-05-12 19:16:52.746734 pyelastica-0.3.1.post1/elastica/modules/forcing.py
--rw-r--r--   0        0        0     2345 2023-05-12 22:18:14.336315 pyelastica-0.3.1.post1/elastica/modules/memory_block.py
--rw-r--r--   0        0        0      141 2023-05-12 22:18:14.336422 pyelastica-0.3.1.post1/elastica/reset_functions_for_block_structure/__init__.py
--rw-r--r--   0        0        0     1744 2023-05-12 22:18:14.336537 pyelastica-0.3.1.post1/elastica/reset_functions_for_block_structure/_reset_ghost_vector_or_scalar.py
--rw-r--r--   0        0        0     3002 2023-05-12 22:18:14.336771 pyelastica-0.3.1.post1/elastica/restart.py
--rw-r--r--   0        0        0       96 2023-05-12 22:18:14.336874 pyelastica-0.3.1.post1/elastica/rigidbody/__init__.py
--rw-r--r--   0        0        0     2944 2023-05-12 22:18:14.336989 pyelastica-0.3.1.post1/elastica/rigidbody/cylinder.py
--rw-r--r--   0        0        0    19346 2023-05-12 22:18:14.337174 pyelastica-0.3.1.post1/elastica/rigidbody/data_structures.py
--rw-r--r--   0        0        0     2945 2023-05-12 22:18:14.337381 pyelastica-0.3.1.post1/elastica/rigidbody/rigid_body.py
--rw-r--r--   0        0        0     2633 2023-05-12 22:18:14.337509 pyelastica-0.3.1.post1/elastica/rigidbody/sphere.py
--rw-r--r--   0        0        0      296 2023-05-12 22:18:14.337616 pyelastica-0.3.1.post1/elastica/rod/__init__.py
--rw-r--r--   0        0        0    34821 2023-05-12 22:18:14.337947 pyelastica-0.3.1.post1/elastica/rod/cosserat_rod.py
--rw-r--r--   0        0        0    19271 2023-05-12 22:18:14.338115 pyelastica-0.3.1.post1/elastica/rod/data_structures.py
--rw-r--r--   0        0        0    14848 2023-05-12 22:18:14.338430 pyelastica-0.3.1.post1/elastica/rod/factory_function.py
--rw-r--r--   0        0        0    28315 2023-05-12 22:18:14.338609 pyelastica-0.3.1.post1/elastica/rod/knot_theory.py
--rw-r--r--   0        0        0      595 2022-05-30 02:18:59.380183 pyelastica-0.3.1.post1/elastica/rod/rod_base.py
--rw-r--r--   0        0        0     3485 2023-05-12 19:16:52.747260 pyelastica-0.3.1.post1/elastica/systems/__init__.py
--rw-r--r--   0        0        0    16240 2023-05-12 22:18:14.338799 pyelastica-0.3.1.post1/elastica/systems/analytical.py
--rw-r--r--   0        0        0     3699 2023-05-12 22:18:14.338910 pyelastica-0.3.1.post1/elastica/timestepper/__init__.py
--rw-r--r--   0        0        0     2613 2023-05-12 22:18:14.339019 pyelastica-0.3.1.post1/elastica/timestepper/_stepper_interface.py
--rw-r--r--   0        0        0     8009 2022-05-30 02:18:59.381378 pyelastica-0.3.1.post1/elastica/timestepper/explicit_steppers.py
--rw-r--r--   0        0        0    10486 2023-05-12 22:18:14.339147 pyelastica-0.3.1.post1/elastica/timestepper/symplectic_steppers.py
--rw-r--r--   0        0        0     5802 2023-05-12 23:20:08.363151 pyelastica-0.3.1.post1/elastica/transformations.py
--rw-r--r--   0        0        0      184 2023-05-12 19:16:52.747449 pyelastica-0.3.1.post1/elastica/typing.py
--rw-r--r--   0        0        0     5322 2023-05-12 23:22:02.521725 pyelastica-0.3.1.post1/elastica/utils.py
--rw-r--r--   0        0        0       18 2023-05-12 22:18:14.339477 pyelastica-0.3.1.post1/elastica/version.py
--rw-r--r--   0        0        0      572 2023-05-12 22:18:14.339573 pyelastica-0.3.1.post1/elastica/wrappers.py
--rw-r--r--   0        0        0     3057 2023-05-12 23:28:10.139342 pyelastica-0.3.1.post1/pyproject.toml
--rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 pyelastica-0.3.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 19:50:46.420150 pyelastica-0.3.2/LICENSE
+-rw-r--r--   0        0        0    10311 2024-04-01 19:50:46.420336 pyelastica-0.3.2/README.md
+-rw-r--r--   0        0        0     2680 2024-04-01 19:50:46.421944 pyelastica-0.3.2/elastica/__init__.py
+-rw-r--r--   0        0        0     9877 2023-05-12 22:18:14.332807 pyelastica-0.3.2/elastica/_calculus.py
+-rw-r--r--   0        0        0    33572 2024-04-01 19:50:46.422103 pyelastica-0.3.2/elastica/_contact_functions.py
+-rw-r--r--   0        0        0     9879 2023-05-12 22:18:14.332934 pyelastica-0.3.2/elastica/_linalg.py
+-rw-r--r--   0        0        0    11780 2023-05-12 22:18:14.333063 pyelastica-0.3.2/elastica/_rotations.py
+-rw-r--r--   0        0        0     3505 2023-05-12 22:18:14.333284 pyelastica-0.3.2/elastica/_synchronize_periodic_boundary.py
+-rw-r--r--   0        0        0    27380 2023-05-12 22:18:14.333604 pyelastica-0.3.2/elastica/boundary_conditions.py
+-rw-r--r--   0        0        0     8541 2023-05-12 22:18:14.333749 pyelastica-0.3.2/elastica/callback_functions.py
+-rw-r--r--   0        0        0    11358 2022-05-30 02:18:59.374910 pyelastica-0.3.2/elastica/collision/AABBCollection.py
+-rw-r--r--   0        0        0    27628 2024-04-01 19:50:46.422224 pyelastica-0.3.2/elastica/contact_forces.py
+-rw-r--r--   0        0        0    14043 2024-04-01 19:50:46.422517 pyelastica-0.3.2/elastica/contact_utils.py
+-rw-r--r--   0        0        0    12044 2023-05-12 22:18:14.333890 pyelastica-0.3.2/elastica/dissipation.py
+-rw-r--r--   0        0        0        0 2022-05-30 02:18:59.375000 pyelastica-0.3.2/elastica/experimental/__init__.py
+-rw-r--r--   0        0        0    15823 2023-05-12 22:18:14.334053 pyelastica-0.3.2/elastica/experimental/connection_contact_joint/generic_system_type_connection.py
+-rw-r--r--   0        0        0     9642 2023-05-12 19:16:52.744915 pyelastica-0.3.2/elastica/experimental/connection_contact_joint/parallel_connection.py
+-rw-r--r--   0        0        0     5850 2023-05-12 22:18:14.334171 pyelastica-0.3.2/elastica/experimental/interaction.py
+-rw-r--r--   0        0        0    18265 2024-04-01 19:50:46.422705 pyelastica-0.3.2/elastica/external_forces.py
+-rw-r--r--   0        0        0    18196 2024-04-01 19:50:46.422963 pyelastica-0.3.2/elastica/interaction.py
+-rw-r--r--   0        0        0    25790 2024-04-01 19:50:46.423428 pyelastica-0.3.2/elastica/joint.py
+-rw-r--r--   0        0        0      111 2023-05-12 22:18:14.335015 pyelastica-0.3.2/elastica/memory_block/__init__.py
+-rw-r--r--   0        0        0     7989 2024-04-01 19:50:46.423885 pyelastica-0.3.2/elastica/memory_block/memory_block_rigid_body.py
+-rw-r--r--   0        0        0    23880 2024-04-01 19:50:46.424055 pyelastica-0.3.2/elastica/memory_block/memory_block_rod.py
+-rw-r--r--   0        0        0     7900 2024-04-01 19:50:46.424178 pyelastica-0.3.2/elastica/memory_block/memory_block_rod_base.py
+-rw-r--r--   0        0        0     9372 2024-04-01 19:50:46.424374 pyelastica-0.3.2/elastica/mesh/mesh_initializer.py
+-rw-r--r--   0        0        0      419 2024-04-01 19:50:46.424490 pyelastica-0.3.2/elastica/modules/__init__.py
+-rw-r--r--   0        0        0     8255 2024-04-01 19:50:46.424907 pyelastica-0.3.2/elastica/modules/base_system.py
+-rw-r--r--   0        0        0     4726 2023-05-12 19:16:52.746366 pyelastica-0.3.2/elastica/modules/callbacks.py
+-rw-r--r--   0        0        0     9701 2023-05-12 19:16:52.746449 pyelastica-0.3.2/elastica/modules/connections.py
+-rw-r--r--   0        0        0     6627 2023-05-12 22:18:14.336039 pyelastica-0.3.2/elastica/modules/constraints.py
+-rw-r--r--   0        0        0     4960 2023-10-03 14:14:11.716000 pyelastica-0.3.2/elastica/modules/contact (1).py
+-rw-r--r--   0        0        0     4857 2024-04-01 19:50:46.425069 pyelastica-0.3.2/elastica/modules/contact.py
+-rw-r--r--   0        0        0     4170 2023-05-12 19:16:52.746631 pyelastica-0.3.2/elastica/modules/damping.py
+-rw-r--r--   0        0        0     5741 2023-05-12 19:16:52.746734 pyelastica-0.3.2/elastica/modules/forcing.py
+-rw-r--r--   0        0        0     2524 2024-04-01 19:50:46.425192 pyelastica-0.3.2/elastica/modules/memory_block.py
+-rw-r--r--   0        0        0      141 2023-05-12 22:18:14.336422 pyelastica-0.3.2/elastica/reset_functions_for_block_structure/__init__.py
+-rw-r--r--   0        0        0     1744 2023-05-12 22:18:14.336537 pyelastica-0.3.2/elastica/reset_functions_for_block_structure/_reset_ghost_vector_or_scalar.py
+-rw-r--r--   0        0        0     3002 2023-05-12 22:18:14.336771 pyelastica-0.3.2/elastica/restart.py
+-rw-r--r--   0        0        0       96 2023-05-12 22:18:14.336874 pyelastica-0.3.2/elastica/rigidbody/__init__.py
+-rw-r--r--   0        0        0     2944 2023-05-12 22:18:14.336989 pyelastica-0.3.2/elastica/rigidbody/cylinder.py
+-rw-r--r--   0        0        0    19346 2023-05-12 22:18:14.337174 pyelastica-0.3.2/elastica/rigidbody/data_structures.py
+-rw-r--r--   0        0        0     2945 2023-05-12 22:18:14.337381 pyelastica-0.3.2/elastica/rigidbody/rigid_body.py
+-rw-r--r--   0        0        0     2633 2023-05-12 22:18:14.337509 pyelastica-0.3.2/elastica/rigidbody/sphere.py
+-rw-r--r--   0        0        0      296 2023-05-12 22:18:14.337616 pyelastica-0.3.2/elastica/rod/__init__.py
+-rw-r--r--   0        0        0    34821 2023-05-12 22:18:14.337947 pyelastica-0.3.2/elastica/rod/cosserat_rod.py
+-rw-r--r--   0        0        0    19271 2023-05-12 22:18:14.338115 pyelastica-0.3.2/elastica/rod/data_structures.py
+-rw-r--r--   0        0        0    14848 2023-05-12 22:18:14.338430 pyelastica-0.3.2/elastica/rod/factory_function.py
+-rw-r--r--   0        0        0    28315 2023-05-12 22:18:14.338609 pyelastica-0.3.2/elastica/rod/knot_theory.py
+-rw-r--r--   0        0        0      595 2022-05-30 02:18:59.380183 pyelastica-0.3.2/elastica/rod/rod_base.py
+-rw-r--r--   0        0        0      127 2024-04-01 19:50:46.425359 pyelastica-0.3.2/elastica/surface/__init__.py
+-rw-r--r--   0        0        0      917 2024-04-01 19:50:46.425436 pyelastica-0.3.2/elastica/surface/plane.py
+-rw-r--r--   0        0        0      316 2024-04-01 19:50:46.425504 pyelastica-0.3.2/elastica/surface/surface_base.py
+-rw-r--r--   0        0        0     3485 2023-05-12 19:16:52.747260 pyelastica-0.3.2/elastica/systems/__init__.py
+-rw-r--r--   0        0        0    16240 2023-05-12 22:18:14.338799 pyelastica-0.3.2/elastica/systems/analytical.py
+-rw-r--r--   0        0        0     3699 2023-05-12 22:18:14.338910 pyelastica-0.3.2/elastica/timestepper/__init__.py
+-rw-r--r--   0        0        0     2613 2023-05-12 22:18:14.339019 pyelastica-0.3.2/elastica/timestepper/_stepper_interface.py
+-rw-r--r--   0        0        0     8009 2022-05-30 02:18:59.381378 pyelastica-0.3.2/elastica/timestepper/explicit_steppers.py
+-rw-r--r--   0        0        0    10486 2023-05-12 22:18:14.339147 pyelastica-0.3.2/elastica/timestepper/symplectic_steppers.py
+-rw-r--r--   0        0        0     5802 2023-05-12 23:20:08.363151 pyelastica-0.3.2/elastica/transformations.py
+-rw-r--r--   0        0        0      283 2024-04-01 19:50:46.425599 pyelastica-0.3.2/elastica/typing.py
+-rw-r--r--   0        0        0     5322 2023-05-12 23:22:02.521725 pyelastica-0.3.2/elastica/utils.py
+-rw-r--r--   0        0        0       18 2024-04-01 19:50:46.425736 pyelastica-0.3.2/elastica/version.py
+-rw-r--r--   0        0        0      572 2023-05-12 22:18:14.339573 pyelastica-0.3.2/elastica/wrappers.py
+-rw-r--r--   0        0        0     3075 2024-04-01 19:50:46.431128 pyelastica-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12334 1970-01-01 00:00:00.000000 pyelastica-0.3.2/PKG-INFO
```

### Comparing `pyelastica-0.3.1.post1/LICENSE` & `pyelastica-0.3.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2023 GazzolaLab
+Copyright (c) 2019-2024 GazzolaLab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyelastica-0.3.1.post1/README.md` & `pyelastica-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [![Build_status][badge-travis]][link-travis] [![CI][badge-CI]][link-CI] [![Documentation Status][badge-docs-status]][link-docs-status] [![codecov][badge-codecov]][link-codecov] [![Downloads][badge-pepy-download-count]][link-pepy-download-count] [![DOI][badge-doi]][link-doi] [![Binder][badge-binder]][link-binder] [![Gitter][badge-gitter]][link-gitter]
  </div>
 
 PyElastica is the python implementation of **Elastica**: an *open-source* project for simulating assemblies of slender, one-dimensional structures using Cosserat Rod theory.
 
 [![gallery][link-readme-gallary]][link-project-website]
 
-Visit [cosseratrods.org][link-project-website] for more information and learn about Elastica and Cosserat rod theory.
+Visit [www.cosseratrods.org][link-project-website] for more information and learn about Elastica and Cosserat rod theory.
 
 ## How to Start
 [![PyPI version][badge-pypi]][link-pypi] [![Documentation Status][badge-docs-status]][link-docs-status]
 
-PyElastica is compatible with Python 3.8 - 3.10.
+PyElastica is compatible with Python 3.8 - 3.11.
 
 ~~~bash
 $ pip install pyelastica
 ~~~
 
 With this you get a minimal version with very little dependencies.
 
@@ -27,14 +27,19 @@
 - `docs`: packages to build documentation
 
 Options can be combined e.g.
 ```bash
 $ pip install "pyelastica[examples,docs]"
 ```
 
+For plotting videos, ffmpeg has to be installed:
+```bash
+$ conda install -c conda-forge ffmpeg
+```
+
 Documentation of PyElastica is available [here][link-docs-website].
 
 If you want to simulate magnetic Cosserat rods interacting with external magnetic environments you can install the derived package using
 
 ```bash
 $ pip install magneto_pyelastica
 ```
@@ -42,71 +47,76 @@
 Details can be found [here](https://github.com/armantekinalp/MagnetoPyElastica).
 
 ## Citation
 
 We ask that any publications which use Elastica cite as following:
 
 ```
-@software{arman_tekinalp_2023_7931429,
+@software{arman_tekinalp_2024_10883271,
   author       = {Arman Tekinalp and
                   Seung Hyun Kim and
                   Yashraj Bhosale and
                   Tejaswin Parthasarathy and
                   Noel Naughton and
-                  Ilia Nasiriziba and
+                  Ali Albazroun and
+                  Rahul Joon and
                   Songyuan Cui and
+                  Ilia Nasiriziba and
                   Maximilian Stölzle and
                   Chia-Hsien (Cathy) Shih and
-                  Mattia Gazzola
-                  },
-  title        = {GazzolaLab/PyElastica: v0.3.1},
-  month        = may,
-  year         = 2023,
+                  Mattia Gazzola},
+  title        = {GazzolaLab/PyElastica: v0.3.2},
+  month        = mar,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.3.1},
-  doi          = {10.5281/zenodo.7931429},
-  url          = {https://doi.org/10.5281/zenodo.7931429}
+  version      = {v0.3.2},
+  doi          = {10.5281/zenodo.10883271},
+  url          = {https://doi.org/10.5281/zenodo.10883271}
 }
 ```
 
 <details>
   <summary><h4>References</h4></summary>
 
 - Gazzola, Dudte, McCormick, Mahadevan, <strong>Forward and inverse problems in the mechanics of soft filaments</strong>, Royal Society Open Science, 2018. doi: [10.1098/rsos.171628](https://doi.org/10.1098/rsos.171628)
 - Zhang, Chan, Parthasarathy, Gazzola, <strong>Modeling and simulation of complex dynamic musculoskeletal architectures</strong>, Nature Communications, 2019. doi: [10.1038/s41467-019-12759-5](https://doi.org/10.1038/s41467-019-12759-5)
 
 </details>
 
 ## List of publications and submissions
+- [Soft, slender and active structures in fluids: embedding Cosserat rods in vortex methods](https://doi.org/10.48550/arXiv.2401.09506) (UIUC 2024)
+- [Neural models and algorithms for sensorimotor control of an octopus arm](https://doi.org/10.48550/arXiv.2402.01074)(UIUC 2024)
+- [On the mechanical origins of waving, coiling and skewing in Arabidopsis thaliana roots](https://www.pnas.org/doi/10.1073/pnas.2312761121) (Tel Aviv University, UIUC 2024) (PNAS)
 - [Topology, dynamics, and control of an octopus-analog muscular hydrostat](https://arxiv.org/abs/2304.08413) (UIUC, 2023)
-- [Hierarchical control and learning of a foraging CyberOctopus](https://arxiv.org/abs/2302.05811) (UIUC, 2023)
+- [Hierarchical control and learning of a foraging CyberOctopus](https://onlinelibrary.wiley.com/doi/full/10.1002/aisy.202300088) (UIUC, 2023) (Advanced Intelligent Systems)
 - [Energy-shaping control of a muscular octopus arm moving in three dimensions](https://royalsocietypublishing.org/doi/full/10.1098/rspa.2022.0593) (UIUC, 2023) (Proceedings of the Royal Society A 2023)
 - [A sensory feedback control law for octopus arm movements](https://ieeexplore.ieee.org/abstract/document/9993021/) (UIUC, 2022) (IEEE CDC 2022)
 - [Control-oriented modeling of bend propagation in an octopus arm](https://ieeexplore.ieee.org/abstract/document/9867689/) (UIUC, 2021) (IEEE ACC 2022)
 - [A physics-informed, vision-based method to reconstruct all deformation modes in slender bodies](https://arxiv.org/abs/2109.08372) (UIUC, 2021) (IEEE ICRA 2022) [code](https://github.com/GazzolaLab/BR2-vision-based-smoothing)
 - [Optimal control of a soft CyberOctopus arm](https://ieeexplore.ieee.org/document/9483284) (UIUC, 2021) (IEEE ACC 2021)
 - [Elastica: A compliant mechanics environment for soft robotic control](https://ieeexplore.ieee.org/document/9369003) (UIUC, 2021) (IEEE RA-L 2021)
 - [Controlling a CyberOctopus soft arm with muscle-like actuation](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9683318) (UIUC, 2020) (IEEE CDC 2021)
 - [Energy shaping control of a CyberOctopus soft arm](https://ieeexplore.ieee.org/document/9304408) (UIUC, 2020) (IEEE CDC 2020)
 
 ## Tutorials
 [![Binder][badge-binder-tutorial]][link-binder]
 
 We have created several Jupyter notebooks and Python scripts to help users get started with PyElastica. The Jupyter notebooks are available on Binder, allowing you to try out some of the tutorials without having to install PyElastica.
 
-We have also included an example script for visualizing PyElastica simulations using POVray. This script is located in the examples folder ([`examples/visualization`](examples/visualization)).
+We have also included an example script for visualizing PyElastica simulations using POVray. This script is located in the examples folder ([`examples/Visualization`](examples/Visualization)).
 
 ## Contribution
 
 If you would like to participate, please read our [contribution guideline](CONTRIBUTING.md)
 
-PyElastica is developed by the [Gazzola Lab][link-lab-website] at the University of Illinois at Urbana-Champaign.
+PyElastica is developed by the [Gazzola Lab][link-lab-website] at the University of Illinois Urbana-Champaign.
 
 ## Senior Developers ✨
 _Names arranged alphabetically_
+- Ali Albazroun
 - Arman Tekinalp
 - Chia-Hsien Shih (Cathy)
 - Fan Kiat Chan
 - Ilia Nasiriziba
 - Noel Naughton
 - [Seung Hyun Kim](https://github.com/skim0119)
 - Songyuan Cui
```

### Comparing `pyelastica-0.3.1.post1/elastica/__init__.py` & `pyelastica-0.3.2/elastica/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from collections import defaultdict
-from elastica.rod.knot_theory import KnotTheory, KnotTheoryCompatibleProtocol
+from elastica.rod.knot_theory import (
+    KnotTheory,
+    KnotTheoryCompatibleProtocol,
+    compute_link,
+    compute_twist,
+    compute_writhe,
+)
 from elastica.rod.rod_base import RodBase
 from elastica.rod.cosserat_rod import CosseratRod
 from elastica.rigidbody.rigid_body import RigidBodyBase
 from elastica.rigidbody.cylinder import Cylinder
 from elastica.rigidbody.sphere import Sphere
+from elastica.surface.plane import Plane
 from elastica.boundary_conditions import (
     ConstraintBase,
     FreeBC,
     OneEndFixedBC,
     GeneralConstraint,
     FixedConstraint,
     HelicalBucklingBC,
@@ -32,39 +39,51 @@
 from elastica.joint import (
     FreeJoint,
     ExternalContact,
     FixedJoint,
     HingeJoint,
     SelfContact,
 )
+from elastica.contact_forces import (
+    NoContact,
+    RodRodContact,
+    RodCylinderContact,
+    RodSelfContact,
+    RodSphereContact,
+    RodPlaneContact,
+    RodPlaneContactWithAnisotropicFriction,
+    CylinderPlaneContact,
+)
 from elastica.callback_functions import CallBackBaseClass, ExportCallBack, MyCallBack
 from elastica.dissipation import (
     DamperBase,
     AnalyticalLinearDamper,
     LaplaceDissipationFilter,
 )
 from elastica.modules.base_system import BaseSystemCollection
 from elastica.modules.callbacks import CallBacks
 from elastica.modules.connections import Connections
 from elastica.modules.constraints import Constraints
 from elastica.modules.forcing import Forcing
 from elastica.modules.damping import Damping
+from elastica.modules.contact import Contact
+
 from elastica.transformations import inv_skew_symmetrize
 from elastica.transformations import rotate
 from elastica._calculus import (
     position_difference_kernel,
     position_average,
     quadrature_kernel,
     difference_kernel,
     quadrature_kernel_for_block_structure,
     difference_kernel_for_block_structure,
 )
 from elastica._linalg import levi_civita_tensor
 from elastica.utils import isqrt
-from elastica.typing import RodType, SystemType
+from elastica.typing import RodType, SystemType, AllowedContactType
 from elastica.timestepper import (
     integrate,
     PositionVerlet,
     PEFRL,
     RungeKutta4,
     EulerForward,
     extend_stepper_interface,
```

### Comparing `pyelastica-0.3.1.post1/elastica/_calculus.py` & `pyelastica-0.3.2/elastica/_calculus.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/_linalg.py` & `pyelastica-0.3.2/elastica/_linalg.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/_rotations.py` & `pyelastica-0.3.2/elastica/_rotations.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/_synchronize_periodic_boundary.py` & `pyelastica-0.3.2/elastica/_synchronize_periodic_boundary.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/boundary_conditions.py` & `pyelastica-0.3.2/elastica/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/callback_functions.py` & `pyelastica-0.3.2/elastica/callback_functions.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/collision/AABBCollection.py` & `pyelastica-0.3.2/elastica/collision/AABBCollection.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/dissipation.py` & `pyelastica-0.3.2/elastica/dissipation.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/experimental/connection_contact_joint/generic_system_type_connection.py` & `pyelastica-0.3.2/elastica/experimental/connection_contact_joint/generic_system_type_connection.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/experimental/connection_contact_joint/parallel_connection.py` & `pyelastica-0.3.2/elastica/experimental/connection_contact_joint/parallel_connection.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/experimental/interaction.py` & `pyelastica-0.3.2/elastica/experimental/interaction.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/external_forces.py` & `pyelastica-0.3.2/elastica/external_forces.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,14 @@
         Parameters
         ----------
         system : SystemType
             Rod or rigid-body object
         time : float
             The time of simulation.
 
-        Returns
-        -------
-
         """
         pass
 
     def apply_torques(self, system: SystemType, time: np.float64 = 0.0):
         """Apply torques to a rod-like object.
 
         In NoForces class, this routine simply passes.
@@ -54,17 +51,14 @@
         Parameters
         ----------
         system : SystemType
             Rod or rigid-body object
         time : float
             The time of simulation.
 
-        Returns
-        -------
-
         """
         pass
 
 
 class GravityForces(NoForces):
     """
     This class applies a constant gravitational force to the entire rod.
@@ -105,17 +99,14 @@
         acc_gravity: numpy.ndarray
             1D (dim) array containing data with 'float' type. Gravitational acceleration vector.
         mass: numpy.ndarray
             1D (blocksize) array containing data with 'float' type. Mass on the nodes.
         external_forces: numpy.ndarray
             2D (dim, blocksize) array containing data with 'float' type. External force vector.
 
-        Returns
-        -------
-
         """
         inplace_addition(external_forces, _batch_product_i_k_to_ik(acc_gravity, mass))
 
 
 class EndpointForces(NoForces):
     """
     This class applies constant forces on the endpoint nodes.
@@ -178,17 +169,14 @@
         end_force: numpy.ndarray
             1D (dim) array containing data with 'float' type.
             Force applied to last node of the system.
         time: float
         ramp_up_time: float
             Applied forces are ramped up until ramp up time.
 
-        Returns
-        -------
-
         """
         factor = min(1.0, time / ramp_up_time)
         external_forces[..., 0] += start_force * factor
         external_forces[..., -1] += end_force * factor
 
 
 class UniformTorques(NoForces):
@@ -341,31 +329,15 @@
 
         if with_spline:
             assert b_coeff.size != 0, "Beta spline coefficient array (t_coeff) is empty"
             my_spline, ctr_pts, ctr_coeffs = _bspline(b_coeff)
             self.my_spline = my_spline(self.s)
 
         else:
-
-            def constant_function(input):
-                """
-                Return array of ones same as the size of the input array. This
-                function is called when Beta spline function is not used.
-
-                Parameters
-                ----------
-                input
-
-                Returns
-                -------
-
-                """
-                return np.ones(input.shape)
-
-            self.my_spline = constant_function(self.s)
+            self.my_spline = np.full_like(self.s, fill_value=1.0)
 
     def apply_torques(self, rod: RodType, time: np.float64 = 0.0):
         self.compute_muscle_torques(
             time,
             self.my_spline,
             self.s,
             self.angular_frequency,
@@ -426,16 +398,14 @@
     Parameters
     ----------
     external_force_or_torque: numpy.ndarray
         2D (dim, blocksize) array containing data with 'float' type.
     force_or_torque: numpy.ndarray
         2D (dim, blocksize) array containing data with 'float' type.
 
-    Returns
-    -------
 
     """
     blocksize = force_or_torque.shape[1]
     for i in range(3):
         for k in range(blocksize):
             external_force_or_torque[i, k] += force_or_torque[i, k]
 
@@ -450,16 +420,14 @@
     Parameters
     ----------
     external_force_or_torque: numpy.ndarray
         2D (dim, blocksize) array containing data with 'float' type.
     force_or_torque: numpy.ndarray
         2D (dim, blocksize) array containing data with 'float' type.
 
-    Returns
-    -------
 
     """
     blocksize = force_or_torque.shape[1]
     for i in range(3):
         for k in range(blocksize):
             external_force_or_torque[i, k] -= force_or_torque[i, k]
```

### Comparing `pyelastica-0.3.1.post1/elastica/interaction.py` & `pyelastica-0.3.2/elastica/_contact_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,222 +1,495 @@
-__doc__ = """ Numba implementation module containing interactions between a rod and its environment."""
+__doc__ = """ Numba implementation module containing contact force calculation functions between rods and rigid bodies and other rods, rigid bodies or surfaces."""
 
-
-import numpy as np
-from elastica.external_forces import NoForces
-
-
-from numba import njit
+from elastica.contact_utils import (
+    _dot_product,
+    _norm,
+    _find_min_dist,
+    _find_slipping_elements,
+    _node_to_element_mass_or_force,
+    _elements_to_nodes_inplace,
+    _node_to_element_position,
+    _node_to_element_velocity,
+)
 from elastica._linalg import (
     _batch_matvec,
     _batch_cross,
     _batch_norm,
     _batch_dot,
     _batch_product_i_k_to_ik,
     _batch_product_i_ik_to_k,
     _batch_product_k_ik_to_ik,
     _batch_vector_sum,
     _batch_matrix_transpose,
     _batch_vec_oneD_vec_cross,
 )
+import numba
+import numpy as np
 
 
-@njit(cache=True)
-def find_slipping_elements(velocity_slip, velocity_threshold):
-    """
-    This function takes the velocity of elements and checks if they are larger than the threshold velocity.
-    If the velocity of elements is larger than threshold velocity, that means those elements are slipping.
-    In other words, kinetic friction will be acting on those elements, not static friction.
-    This function outputs an array called slip function, this array has a size of the number of elements.
-    If the velocity of the element is smaller than the threshold velocity slip function value for that element is 1,
-    which means static friction is acting on that element. If the velocity of the element is larger than
-    the threshold velocity slip function value for that element is between 0 and 1, which means kinetic friction is acting
-    on that element.
-
-    Parameters
-    ----------
-    velocity_slip : numpy.ndarray
-        2D (dim, blocksize) array containing data with 'float' type.
-        Rod-like object element velocity.
-    velocity_threshold : float
-        Threshold velocity to determine slip.
-
-    Returns
-    -------
-    slip_function : numpy.ndarray
-        2D (dim, blocksize) array containing data with 'float' type.
-    """
-    """
-    Developer Notes
-    -----
-    Benchmark results, for a blocksize of 100 using timeit
-    python version: 18.9 µs ± 2.98 µs per loop
-    this version: 1.96 µs ± 58.3 ns per loop
-    """
-    abs_velocity_slip = _batch_norm(velocity_slip)
-    slip_points = np.where(np.fabs(abs_velocity_slip) > velocity_threshold)
-    slip_function = np.ones((velocity_slip.shape[1]))
-    slip_function[slip_points] = np.fabs(
-        1.0 - np.minimum(1.0, abs_velocity_slip[slip_points] / velocity_threshold - 1.0)
-    )
-    return slip_function
-
-
-@njit(cache=True)
-def node_to_element_mass_or_force(input):
-    """
-    This function converts the mass/forces on rod nodes to
-    elements, where special treatment is necessary at the ends.
-
-    Parameters
-    ----------
-    input: numpy.ndarray
-        2D (dim, blocksize) array containing nodal mass/forces
-        with 'float' type.
-
-    Returns
-    -------
-    output: numpy.ndarray
-        2D (dim, blocksize) array containing elemental mass/forces
-        with 'float' type.
-    """
-    """
-    Developer Notes
-    -----
-    Benchmark results, for a blocksize of 100 using timeit
-    Python version: 18.1 µs ± 1.03 µs per loop
-    This version: 1.55 µs ± 13.4 ns per loop
-    """
-    blocksize = input.shape[1] - 1  # nelem
-    output = np.zeros((3, blocksize))
-    for i in range(3):
-        for k in range(0, blocksize):
-            output[i, k] += 0.5 * (input[i, k] + input[i, k + 1])
-
-            # Put extra care for the first and last element
-    output[..., 0] += 0.5 * input[..., 0]
-    output[..., -1] += 0.5 * input[..., -1]
-
-    return output
-
-
-def nodes_to_elements(input):
-    # Remove the function beyond v0.4.0
-    raise NotImplementedError(
-        "This function is removed in v0.3.1. Please use\n"
-        "elastica.interaction.node_to_element_mass_or_force()\n"
-        "instead for node-to-element interpolation of mass/forces."
+@numba.njit(cache=True)
+def _calculate_contact_forces_rod_cylinder(
+    x_collection_rod,
+    edge_collection_rod,
+    x_cylinder_center,
+    x_cylinder_tip,
+    edge_cylinder,
+    radii_sum,
+    length_sum,
+    internal_forces_rod,
+    external_forces_rod,
+    external_forces_cylinder,
+    external_torques_cylinder,
+    cylinder_director_collection,
+    velocity_rod,
+    velocity_cylinder,
+    contact_k,
+    contact_nu,
+    velocity_damping_coefficient,
+    friction_coefficient,
+) -> None:
+    # We already pass in only the first n_elem x
+    n_points = x_collection_rod.shape[1]
+    cylinder_total_contact_forces = np.zeros((3))
+    cylinder_total_contact_torques = np.zeros((3))
+    for i in range(n_points):
+        # Element-wise bounding box
+        x_selected = x_collection_rod[..., i]
+        # x_cylinder is already a (,) array from outised
+        del_x = x_selected - x_cylinder_tip
+        norm_del_x = _norm(del_x)
+
+        # If outside then don't process
+        if norm_del_x >= (radii_sum[i] + length_sum[i]):
+            continue
+
+        # find the shortest line segment between the two centerline
+        # segments : differs from normal cylinder-cylinder intersection
+        distance_vector, x_cylinder_contact_point, _ = _find_min_dist(
+            x_selected, edge_collection_rod[..., i], x_cylinder_tip, edge_cylinder
+        )
+        distance_vector_length = _norm(distance_vector)
+        distance_vector /= distance_vector_length
+
+        gamma = radii_sum[i] - distance_vector_length
+
+        # If distance is large, don't worry about it
+        if gamma < -1e-5:
+            continue
+
+        # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
+        # As a quick fix, use this instead
+        mask = (gamma > 0.0) * 1.0
+
+        # Compute contact spring force
+        contact_force = contact_k * gamma * distance_vector
+        interpenetration_velocity = velocity_cylinder[..., 0] - 0.5 * (
+            velocity_rod[..., i] + velocity_rod[..., i + 1]
+        )
+        # Compute contact damping
+        normal_interpenetration_velocity = (
+            _dot_product(interpenetration_velocity, distance_vector) * distance_vector
+        )
+        contact_damping_force = -contact_nu * normal_interpenetration_velocity
+
+        # magnitude* direction
+        net_contact_force = 0.5 * mask * (contact_damping_force + contact_force)
+
+        # Compute friction
+        slip_interpenetration_velocity = (
+            interpenetration_velocity - normal_interpenetration_velocity
+        )
+        slip_interpenetration_velocity_mag = np.linalg.norm(
+            slip_interpenetration_velocity
+        )
+        slip_interpenetration_velocity_unitized = slip_interpenetration_velocity / (
+            slip_interpenetration_velocity_mag + 1e-14
+        )
+        # Compute friction force in the slip direction.
+        damping_force_in_slip_direction = (
+            velocity_damping_coefficient * slip_interpenetration_velocity_mag
+        )
+        # Compute Coulombic friction
+        coulombic_friction_force = friction_coefficient * np.linalg.norm(
+            net_contact_force
+        )
+        # Compare damping force in slip direction and kinetic friction and minimum is the friction force.
+        friction_force = (
+            -min(damping_force_in_slip_direction, coulombic_friction_force)
+            * slip_interpenetration_velocity_unitized
+        )
+        # Update contact force
+        net_contact_force += friction_force
+
+        # Torques acting on the cylinder
+        moment_arm = x_cylinder_contact_point - x_cylinder_center
+
+        # Add it to the rods at the end of the day
+        if i == 0:
+            external_forces_rod[..., i] -= 2 / 3 * net_contact_force
+            external_forces_rod[..., i + 1] -= 4 / 3 * net_contact_force
+            cylinder_total_contact_forces += 2.0 * net_contact_force
+            cylinder_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+        elif i == n_points - 1:
+            external_forces_rod[..., i] -= 4 / 3 * net_contact_force
+            external_forces_rod[..., i + 1] -= 2 / 3 * net_contact_force
+            cylinder_total_contact_forces += 2.0 * net_contact_force
+            cylinder_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+        else:
+            external_forces_rod[..., i] -= net_contact_force
+            external_forces_rod[..., i + 1] -= net_contact_force
+            cylinder_total_contact_forces += 2.0 * net_contact_force
+            cylinder_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+
+    # Update the cylinder external forces and torques
+    external_forces_cylinder[..., 0] += cylinder_total_contact_forces
+    external_torques_cylinder[..., 0] += (
+        cylinder_director_collection @ cylinder_total_contact_torques
+    )
+
+
+@numba.njit(cache=True)
+def _calculate_contact_forces_rod_rod(
+    x_collection_rod_one,
+    radius_rod_one,
+    length_rod_one,
+    tangent_rod_one,
+    velocity_rod_one,
+    internal_forces_rod_one,
+    external_forces_rod_one,
+    x_collection_rod_two,
+    radius_rod_two,
+    length_rod_two,
+    tangent_rod_two,
+    velocity_rod_two,
+    internal_forces_rod_two,
+    external_forces_rod_two,
+    contact_k,
+    contact_nu,
+) -> None:
+    # We already pass in only the first n_elem x
+    n_points_rod_one = x_collection_rod_one.shape[1]
+    n_points_rod_two = x_collection_rod_two.shape[1]
+    edge_collection_rod_one = _batch_product_k_ik_to_ik(length_rod_one, tangent_rod_one)
+    edge_collection_rod_two = _batch_product_k_ik_to_ik(length_rod_two, tangent_rod_two)
+
+    for i in range(n_points_rod_one):
+        for j in range(n_points_rod_two):
+            radii_sum = radius_rod_one[i] + radius_rod_two[j]
+            length_sum = length_rod_one[i] + length_rod_two[j]
+            # Element-wise bounding box
+            x_selected_rod_one = x_collection_rod_one[..., i]
+            x_selected_rod_two = x_collection_rod_two[..., j]
+
+            del_x = x_selected_rod_one - x_selected_rod_two
+            norm_del_x = _norm(del_x)
+
+            # If outside then don't process
+            if norm_del_x >= (radii_sum + length_sum):
+                continue
+
+            # find the shortest line segment between the two centerline
+            # segments : differs from normal cylinder-cylinder intersection
+            distance_vector, _, _ = _find_min_dist(
+                x_selected_rod_one,
+                edge_collection_rod_one[..., i],
+                x_selected_rod_two,
+                edge_collection_rod_two[..., j],
+            )
+            distance_vector_length = _norm(distance_vector)
+            distance_vector /= distance_vector_length
+            gamma = radii_sum - distance_vector_length
+
+            # If distance is large, don't worry about it
+            if gamma < -1e-5:
+                continue
+
+            rod_one_elemental_forces = 0.5 * (
+                external_forces_rod_one[..., i]
+                + external_forces_rod_one[..., i + 1]
+                + internal_forces_rod_one[..., i]
+                + internal_forces_rod_one[..., i + 1]
+            )
+
+            rod_two_elemental_forces = 0.5 * (
+                external_forces_rod_two[..., j]
+                + external_forces_rod_two[..., j + 1]
+                + internal_forces_rod_two[..., j]
+                + internal_forces_rod_two[..., j + 1]
+            )
+
+            equilibrium_forces = -rod_one_elemental_forces + rod_two_elemental_forces
+
+            """FIX ME: Remove normal force and tune rod-rod contact example"""
+            normal_force = _dot_product(equilibrium_forces, distance_vector)
+            # Following line same as np.where(normal_force < 0.0, -normal_force, 0.0)
+            normal_force = abs(min(normal_force, 0.0))
+
+            # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
+            # As a quick fix, use this instead
+            mask = (gamma > 0.0) * 1.0
+
+            contact_force = contact_k * gamma
+            interpenetration_velocity = 0.5 * (
+                (velocity_rod_one[..., i] + velocity_rod_one[..., i + 1])
+                - (velocity_rod_two[..., j] + velocity_rod_two[..., j + 1])
+            )
+            contact_damping_force = contact_nu * _dot_product(
+                interpenetration_velocity, distance_vector
+            )
+
+            # magnitude* direction
+            net_contact_force = (
+                normal_force + 0.5 * mask * (contact_damping_force + contact_force)
+            ) * distance_vector
+
+            # Add it to the rods at the end of the day
+            if i == 0:
+                external_forces_rod_one[..., i] -= net_contact_force * 2 / 3
+                external_forces_rod_one[..., i + 1] -= net_contact_force * 4 / 3
+            elif i == n_points_rod_one - 1:
+                external_forces_rod_one[..., i] -= net_contact_force * 4 / 3
+                external_forces_rod_one[..., i + 1] -= net_contact_force * 2 / 3
+            else:
+                external_forces_rod_one[..., i] -= net_contact_force
+                external_forces_rod_one[..., i + 1] -= net_contact_force
+
+            if j == 0:
+                external_forces_rod_two[..., j] += net_contact_force * 2 / 3
+                external_forces_rod_two[..., j + 1] += net_contact_force * 4 / 3
+            elif j == n_points_rod_two - 1:
+                external_forces_rod_two[..., j] += net_contact_force * 4 / 3
+                external_forces_rod_two[..., j + 1] += net_contact_force * 2 / 3
+            else:
+                external_forces_rod_two[..., j] += net_contact_force
+                external_forces_rod_two[..., j + 1] += net_contact_force
+
+
+@numba.njit(cache=True)
+def _calculate_contact_forces_self_rod(
+    x_collection_rod,
+    radius_rod,
+    length_rod,
+    tangent_rod,
+    velocity_rod,
+    external_forces_rod,
+    contact_k,
+    contact_nu,
+) -> None:
+    # We already pass in only the first n_elem x
+    n_points_rod = x_collection_rod.shape[1]
+    edge_collection_rod_one = _batch_product_k_ik_to_ik(length_rod, tangent_rod)
+
+    for i in range(n_points_rod):
+        skip = int(1 + np.ceil(0.8 * np.pi * radius_rod[i] / length_rod[i]))
+        for j in range(i - skip, -1, -1):
+            radii_sum = radius_rod[i] + radius_rod[j]
+            length_sum = length_rod[i] + length_rod[j]
+            # Element-wise bounding box
+            x_selected_rod_index_i = x_collection_rod[..., i]
+            x_selected_rod_index_j = x_collection_rod[..., j]
+
+            del_x = x_selected_rod_index_i - x_selected_rod_index_j
+            norm_del_x = _norm(del_x)
+
+            # If outside then don't process
+            if norm_del_x >= (radii_sum + length_sum):
+                continue
+
+            # find the shortest line segment between the two centerline
+            # segments : differs from normal cylinder-cylinder intersection
+            distance_vector, _, _ = _find_min_dist(
+                x_selected_rod_index_i,
+                edge_collection_rod_one[..., i],
+                x_selected_rod_index_j,
+                edge_collection_rod_one[..., j],
+            )
+            distance_vector_length = _norm(distance_vector)
+            distance_vector /= distance_vector_length
+
+            gamma = radii_sum - distance_vector_length
+
+            # If distance is large, don't worry about it
+            if gamma < -1e-5:
+                continue
+
+            # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
+            # As a quick fix, use this instead
+            mask = (gamma > 0.0) * 1.0
+
+            contact_force = contact_k * gamma
+            interpenetration_velocity = 0.5 * (
+                (velocity_rod[..., i] + velocity_rod[..., i + 1])
+                - (velocity_rod[..., j] + velocity_rod[..., j + 1])
+            )
+            contact_damping_force = contact_nu * _dot_product(
+                interpenetration_velocity, distance_vector
+            )
+
+            # magnitude* direction
+            net_contact_force = (
+                0.5 * mask * (contact_damping_force + contact_force)
+            ) * distance_vector
+
+            # Add it to the rods at the end of the day
+            # if i == 0:
+            #     external_forces_rod[...,i] -= net_contact_force *2/3
+            #     external_forces_rod[...,i+1] -= net_contact_force * 4/3
+            if i == n_points_rod - 1:
+                external_forces_rod[..., i] -= net_contact_force * 4 / 3
+                external_forces_rod[..., i + 1] -= net_contact_force * 2 / 3
+            else:
+                external_forces_rod[..., i] -= net_contact_force
+                external_forces_rod[..., i + 1] -= net_contact_force
+
+            if j == 0:
+                external_forces_rod[..., j] += net_contact_force * 2 / 3
+                external_forces_rod[..., j + 1] += net_contact_force * 4 / 3
+            # elif j == n_points_rod:
+            #     external_forces_rod[..., j] += net_contact_force * 4/3
+            #     external_forces_rod[..., j+1] += net_contact_force * 2/3
+            else:
+                external_forces_rod[..., j] += net_contact_force
+                external_forces_rod[..., j + 1] += net_contact_force
+
+
+@numba.njit(cache=True)
+def _calculate_contact_forces_rod_sphere(
+    x_collection_rod,
+    edge_collection_rod,
+    x_sphere_center,
+    x_sphere_tip,
+    edge_sphere,
+    radii_sum,
+    length_sum,
+    internal_forces_rod,
+    external_forces_rod,
+    external_forces_sphere,
+    external_torques_sphere,
+    sphere_director_collection,
+    velocity_rod,
+    velocity_sphere,
+    contact_k,
+    contact_nu,
+    velocity_damping_coefficient,
+    friction_coefficient,
+) -> None:
+    # We already pass in only the first n_elem x
+    n_points = x_collection_rod.shape[1]
+    sphere_total_contact_forces = np.zeros((3))
+    sphere_total_contact_torques = np.zeros((3))
+    for i in range(n_points):
+        # Element-wise bounding box
+        x_selected = x_collection_rod[..., i]
+        # x_sphere is already a (,) array from outside
+        del_x = x_selected - x_sphere_tip
+        norm_del_x = _norm(del_x)
+
+        # If outside then don't process
+        if norm_del_x >= (radii_sum[i] + length_sum[i]):
+            continue
+
+        # find the shortest line segment between the two centerline
+        distance_vector, x_sphere_contact_point, _ = _find_min_dist(
+            x_selected, edge_collection_rod[..., i], x_sphere_tip, edge_sphere
+        )
+        distance_vector_length = _norm(distance_vector)
+        distance_vector /= distance_vector_length
+
+        gamma = radii_sum[i] - distance_vector_length
+
+        # If distance is large, don't worry about it
+        if gamma < -1e-5:
+            continue
+
+        # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
+        # As a quick fix, use this instead
+        mask = (gamma > 0.0) * 1.0
+
+        # Compute contact spring force
+        contact_force = contact_k * gamma * distance_vector
+        interpenetration_velocity = velocity_sphere[..., 0] - 0.5 * (
+            velocity_rod[..., i] + velocity_rod[..., i + 1]
+        )
+        # Compute contact damping
+        normal_interpenetration_velocity = (
+            _dot_product(interpenetration_velocity, distance_vector) * distance_vector
+        )
+        contact_damping_force = -contact_nu * normal_interpenetration_velocity
+
+        # magnitude* direction
+        net_contact_force = 0.5 * mask * (contact_damping_force + contact_force)
+
+        # Compute friction
+        slip_interpenetration_velocity = (
+            interpenetration_velocity - normal_interpenetration_velocity
+        )
+        slip_interpenetration_velocity_mag = np.linalg.norm(
+            slip_interpenetration_velocity
+        )
+        slip_interpenetration_velocity_unitized = slip_interpenetration_velocity / (
+            slip_interpenetration_velocity_mag + 1e-14
+        )
+        # Compute friction force in the slip direction.
+        damping_force_in_slip_direction = (
+            velocity_damping_coefficient * slip_interpenetration_velocity_mag
+        )
+        # Compute Coulombic friction
+        coulombic_friction_force = friction_coefficient * np.linalg.norm(
+            net_contact_force
+        )
+        # Compare damping force in slip direction and kinetic friction and minimum is the friction force.
+        friction_force = (
+            -min(damping_force_in_slip_direction, coulombic_friction_force)
+            * slip_interpenetration_velocity_unitized
+        )
+        # Update contact force
+        net_contact_force += friction_force
+
+        # Torques acting on the cylinder
+        moment_arm = x_sphere_contact_point - x_sphere_center
+
+        # Add it to the rods at the end of the day
+        if i == 0:
+            external_forces_rod[..., i] -= 2 / 3 * net_contact_force
+            external_forces_rod[..., i + 1] -= 4 / 3 * net_contact_force
+            sphere_total_contact_forces += 2.0 * net_contact_force
+            sphere_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+        elif i == n_points - 1:
+            external_forces_rod[..., i] -= 4 / 3 * net_contact_force
+            external_forces_rod[..., i + 1] -= 2 / 3 * net_contact_force
+            sphere_total_contact_forces += 2.0 * net_contact_force
+            sphere_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+        else:
+            external_forces_rod[..., i] -= net_contact_force
+            external_forces_rod[..., i + 1] -= net_contact_force
+            sphere_total_contact_forces += 2.0 * net_contact_force
+            sphere_total_contact_torques += np.cross(
+                moment_arm, 2.0 * net_contact_force
+            )
+
+    # Update the cylinder external forces and torques
+    external_forces_sphere[..., 0] += sphere_total_contact_forces
+    external_torques_sphere[..., 0] += (
+        sphere_director_collection @ sphere_total_contact_torques
     )
 
 
-@njit(cache=True)
-def elements_to_nodes_inplace(vector_in_element_frame, vector_in_node_frame):
-    """
-    Updating nodal forces using the forces computed on elements
-    Parameters
-    ----------
-    vector_in_element_frame
-    vector_in_node_frame
-
-    Returns
-    -------
-    Notes
-    -----
-    Benchmark results, for a blocksize of 100 using timeit
-    Python version: 23.1 µs ± 7.57 µs per loop
-    This version: 696 ns ± 10.2 ns per loop
-    """
-    for i in range(3):
-        for k in range(vector_in_element_frame.shape[1]):
-            vector_in_node_frame[i, k] += 0.5 * vector_in_element_frame[i, k]
-            vector_in_node_frame[i, k + 1] += 0.5 * vector_in_element_frame[i, k]
-
-
-# base class for interaction
-# only applies normal force no friction
-class InteractionPlane:
-    """
-    The interaction plane class computes the plane reaction
-    force on a rod-like object.  For more details regarding the contact module refer to
-    Eqn 4.8 of Gazzola et al. RSoS (2018).
-
-        Attributes
-        ----------
-        k: float
-            Stiffness coefficient between the plane and the rod-like object.
-        nu: float
-            Dissipation coefficient between the plane and the rod-like object.
-        plane_origin: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            Origin of the plane.
-        plane_normal: numpy.ndarray
-           2D (dim, 1) array containing data with 'float' type.
-           The normal vector of the plane.
-        surface_tol: float
-            Penetration tolerance between the plane and the rod-like object.
-
-    """
-
-    def __init__(self, k, nu, plane_origin, plane_normal):
-        """
-
-        Parameters
-        ----------
-        k: float
-            Stiffness coefficient between the plane and the rod-like object.
-        nu: float
-            Dissipation coefficient between the plane and the rod-like object.
-        plane_origin: numpy.ndarray
-           2D (dim, 1) array containing data with 'float' type.
-           Origin of the plane.
-        plane_normal: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            The normal vector of the plane.
-        """
-        self.k = k
-        self.nu = nu
-        self.plane_origin = plane_origin.reshape(3, 1)
-        self.plane_normal = plane_normal.reshape(3)
-        self.surface_tol = 1e-4
-
-    def apply_normal_force(self, system):
-        """
-        In the case of contact with the plane, this function computes the plane reaction force on the element.
-
-        Parameters
-        ----------
-        system: object
-            Rod-like object.
-
-        Returns
-        -------
-        plane_response_force_mag : numpy.ndarray
-            1D (blocksize) array containing data with 'float' type.
-            Magnitude of plane response force acting on rod-like object.
-        no_contact_point_idx : numpy.ndarray
-            1D (blocksize) array containing data with 'int' type.
-            Index of rod-like object elements that are not in contact with the plane.
-        """
-        return apply_normal_force_numba(
-            self.plane_origin,
-            self.plane_normal,
-            self.surface_tol,
-            self.k,
-            self.nu,
-            system.radius,
-            system.mass,
-            system.position_collection,
-            system.velocity_collection,
-            system.internal_forces,
-            system.external_forces,
-        )
-
-
-@njit(cache=True)
-def apply_normal_force_numba(
+@numba.njit(cache=True)
+def _calculate_contact_forces_rod_plane(
     plane_origin,
     plane_normal,
     surface_tol,
     k,
     nu,
     radius,
     mass,
@@ -237,15 +510,15 @@
     Returns
     -------
     magnitude of the plane response
     """
 
     # Compute plane response force
     nodal_total_forces = _batch_vector_sum(internal_forces, external_forces)
-    element_total_forces = node_to_element_mass_or_force(nodal_total_forces)
+    element_total_forces = _node_to_element_mass_or_force(nodal_total_forces)
 
     force_component_along_normal_direction = _batch_product_i_ik_to_k(
         plane_normal, element_total_forces
     )
     forces_along_normal_direction = _batch_product_i_k_to_ik(
         plane_normal, force_component_along_normal_direction
     )
@@ -258,23 +531,23 @@
     ] = 0.0
     # Compute response force on the element. Plane response force
     # has to be away from the surface and towards the element. Thus
     # multiply forces along normal direction with negative sign.
     plane_response_force = -forces_along_normal_direction
 
     # Elastic force response due to penetration
-    element_position = node_to_element_position(position_collection)
+    element_position = _node_to_element_position(position_collection)
     distance_from_plane = _batch_product_i_ik_to_k(
         plane_normal, (element_position - plane_origin)
     )
     plane_penetration = np.minimum(distance_from_plane - radius, 0.0)
     elastic_force = -k * _batch_product_i_k_to_ik(plane_normal, plane_penetration)
 
     # Damping force response due to velocity towards the plane
-    element_velocity = node_to_element_velocity(
+    element_velocity = _node_to_element_velocity(
         mass=mass, node_velocity_collection=velocity_collection
     )
     normal_component_of_element_velocity = _batch_product_i_ik_to_k(
         plane_normal, element_velocity
     )
     damping_force = -nu * _batch_product_i_k_to_ik(
         plane_normal, normal_component_of_element_velocity
@@ -287,143 +560,21 @@
     no_contact_point_idx = np.where((distance_from_plane - radius) > surface_tol)[0]
     # If rod element does not have any contact with plane, plane cannot apply response
     # force on the element. Thus lets set plane response force to 0.0 for the no contact points.
     plane_response_force[..., no_contact_point_idx] = 0.0
     plane_response_force_total[..., no_contact_point_idx] = 0.0
 
     # Update the external forces
-    elements_to_nodes_inplace(plane_response_force_total, external_forces)
+    _elements_to_nodes_inplace(plane_response_force_total, external_forces)
 
     return (_batch_norm(plane_response_force), no_contact_point_idx)
 
 
-# class for anisotropic frictional plane
-# NOTE: friction coefficients are passed as arrays in the order
-# mu_forward : mu_backward : mu_sideways
-# head is at x[0] and forward means head to tail
-# same convention for kinetic and static
-# mu named as to which direction it opposes
-class AnisotropicFrictionalPlane(NoForces, InteractionPlane):
-    """
-    This anisotropic friction plane class is for computing
-    anisotropic friction forces on rods.
-    A detailed explanation of the implemented equations
-    can be found in Gazzola et al. RSoS. (2018).
-
-        Attributes
-        ----------
-        k: float
-            Stiffness coefficient between the plane and the rod-like object.
-        nu: float
-            Dissipation coefficient between the plane and the rod-like object.
-        plane_origin: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            Origin of the plane.
-        plane_normal: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            The normal vector of the plane.
-        slip_velocity_tol: float
-            Velocity tolerance to determine if the element is slipping or not.
-        static_mu_array: numpy.ndarray
-            1D (3,) array containing data with 'float' type.
-            [forward, backward, sideways] static friction coefficients.
-        kinetic_mu_array: numpy.ndarray
-            1D (3,) array containing data with 'float' type.
-            [forward, backward, sideways] kinetic friction coefficients.
-    """
-
-    def __init__(
-        self,
-        k,
-        nu,
-        plane_origin,
-        plane_normal,
-        slip_velocity_tol,
-        static_mu_array,
-        kinetic_mu_array,
-    ):
-        """
-
-        Parameters
-        ----------
-        k: float
-            Stiffness coefficient between the plane and the rod-like object.
-        nu: float
-            Dissipation coefficient between the plane and the rod-like object.
-        plane_origin: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            Origin of the plane.
-        plane_normal: numpy.ndarray
-            2D (dim, 1) array containing data with 'float' type.
-            The normal vector of the plane.
-        slip_velocity_tol: float
-            Velocity tolerance to determine if the element is slipping or not.
-        static_mu_array: numpy.ndarray
-            1D (3,) array containing data with 'float' type.
-            [forward, backward, sideways] static friction coefficients.
-        kinetic_mu_array: numpy.ndarray
-            1D (3,) array containing data with 'float' type.
-            [forward, backward, sideways] kinetic friction coefficients.
-        """
-        InteractionPlane.__init__(self, k, nu, plane_origin, plane_normal)
-        self.slip_velocity_tol = slip_velocity_tol
-        (
-            self.static_mu_forward,
-            self.static_mu_backward,
-            self.static_mu_sideways,
-        ) = static_mu_array
-        (
-            self.kinetic_mu_forward,
-            self.kinetic_mu_backward,
-            self.kinetic_mu_sideways,
-        ) = kinetic_mu_array
-
-    # kinetic and static friction should separate functions
-    # for now putting them together to figure out common variables
-    def apply_forces(self, system, time=0.0):
-        """
-        Call numba implementation to apply friction forces
-        Parameters
-        ----------
-        system
-        time
-
-        Returns
-        -------
-
-        """
-        anisotropic_friction(
-            self.plane_origin,
-            self.plane_normal,
-            self.surface_tol,
-            self.slip_velocity_tol,
-            self.k,
-            self.nu,
-            self.kinetic_mu_forward,
-            self.kinetic_mu_backward,
-            self.kinetic_mu_sideways,
-            self.static_mu_forward,
-            self.static_mu_backward,
-            self.static_mu_sideways,
-            system.radius,
-            system.mass,
-            system.tangents,
-            system.position_collection,
-            system.director_collection,
-            system.velocity_collection,
-            system.omega_collection,
-            system.internal_forces,
-            system.external_forces,
-            system.internal_torques,
-            system.external_torques,
-        )
-
-
-@njit(cache=True)
-def anisotropic_friction(
+@numba.njit(cache=True)
+def _calculate_contact_forces_rod_plane_with_anisotropic_friction(
     plane_origin,
     plane_normal,
     surface_tol,
     slip_velocity_tol,
     k,
     nu,
     kinetic_mu_forward,
@@ -440,15 +591,18 @@
     velocity_collection,
     omega_collection,
     internal_forces,
     external_forces,
     internal_torques,
     external_torques,
 ):
-    plane_response_force_mag, no_contact_point_idx = apply_normal_force_numba(
+    (
+        plane_response_force_mag,
+        no_contact_point_idx,
+    ) = _calculate_contact_forces_rod_plane(
         plane_origin,
         plane_normal,
         surface_tol,
         k,
         nu,
         radius,
         mass,
@@ -470,15 +624,15 @@
     )
     # Normalize tangent_perpendicular_to_normal_direction. This is axial direction for plane. Here we are adding
     # small tolerance (1e-10) for normalization, in order to prevent division by 0.
     axial_direction = _batch_product_k_ik_to_ik(
         1 / (tangent_perpendicular_to_normal_direction_mag + 1e-14),
         tangent_perpendicular_to_normal_direction,
     )
-    element_velocity = node_to_element_velocity(
+    element_velocity = _node_to_element_velocity(
         mass=mass, node_velocity_collection=velocity_collection
     )
     # first apply axial kinetic friction
     velocity_mag_along_axial_direction = _batch_dot(element_velocity, axial_direction)
     velocity_along_axial_direction = _batch_product_k_ik_to_ik(
         velocity_mag_along_axial_direction, axial_direction
     )
@@ -488,18 +642,17 @@
     velocity_sign_along_axial_direction = np.sign(velocity_mag_along_axial_direction)
     # Check top for sign convention
     kinetic_mu = 0.5 * (
         kinetic_mu_forward * (1 + velocity_sign_along_axial_direction)
         + kinetic_mu_backward * (1 - velocity_sign_along_axial_direction)
     )
     # Call slip function to check if elements slipping or not
-    slip_function_along_axial_direction = find_slipping_elements(
+    slip_function_along_axial_direction = _find_slipping_elements(
         velocity_along_axial_direction, slip_velocity_tol
     )
-
     # Now rolling kinetic friction
     rolling_direction = _batch_vec_oneD_vec_cross(axial_direction, plane_normal)
     torque_arm = _batch_product_i_k_to_ik(-plane_normal, radius)
     velocity_along_rolling_direction = _batch_dot(element_velocity, rolling_direction)
     directors_transpose = _batch_matrix_transpose(director_collection)
     # w_rot = Q.T @ omega @ Q @ r
     rotation_velocity = _batch_matvec(
@@ -511,15 +664,15 @@
     )
     slip_velocity_mag_along_rolling_direction = (
         velocity_along_rolling_direction + rotation_velocity_along_rolling_direction
     )
     slip_velocity_along_rolling_direction = _batch_product_k_ik_to_ik(
         slip_velocity_mag_along_rolling_direction, rolling_direction
     )
-    slip_function_along_rolling_direction = find_slipping_elements(
+    slip_function_along_rolling_direction = _find_slipping_elements(
         slip_velocity_along_rolling_direction, slip_velocity_tol
     )
     # Compute unitized total slip velocity vector. We will use this to distribute the weight of the rod in axial
     # and rolling directions.
     unitized_total_velocity = (
         slip_velocity_along_rolling_direction + velocity_along_axial_direction
     )
@@ -531,40 +684,40 @@
         * plane_response_force_mag
         * _batch_dot(unitized_total_velocity, axial_direction)
         * axial_direction
     )
     # If rod element does not have any contact with plane, plane cannot apply friction
     # force on the element. Thus lets set kinetic friction force to 0.0 for the no contact points.
     kinetic_friction_force_along_axial_direction[..., no_contact_point_idx] = 0.0
-    elements_to_nodes_inplace(
+    _elements_to_nodes_inplace(
         kinetic_friction_force_along_axial_direction, external_forces
     )
     # Apply kinetic friction in rolling direction.
     kinetic_friction_force_along_rolling_direction = -(
         (1.0 - slip_function_along_rolling_direction)
         * kinetic_mu_sideways
         * plane_response_force_mag
         * _batch_dot(unitized_total_velocity, rolling_direction)
         * rolling_direction
     )
     # If rod element does not have any contact with plane, plane cannot apply friction
     # force on the element. Thus lets set kinetic friction force to 0.0 for the no contact points.
     kinetic_friction_force_along_rolling_direction[..., no_contact_point_idx] = 0.0
-    elements_to_nodes_inplace(
+    _elements_to_nodes_inplace(
         kinetic_friction_force_along_rolling_direction, external_forces
     )
     # torque = Q @ r @ Fr
     external_torques += _batch_matvec(
         director_collection,
         _batch_cross(torque_arm, kinetic_friction_force_along_rolling_direction),
     )
 
     # now axial static friction
     nodal_total_forces = _batch_vector_sum(internal_forces, external_forces)
-    element_total_forces = node_to_element_mass_or_force(nodal_total_forces)
+    element_total_forces = _node_to_element_mass_or_force(nodal_total_forces)
     force_component_along_axial_direction = _batch_dot(
         element_total_forces, axial_direction
     )
     force_component_sign_along_axial_direction = np.sign(
         force_component_along_axial_direction
     )
     # check top for sign convention
@@ -580,15 +733,15 @@
         np.minimum(np.fabs(force_component_along_axial_direction), max_friction_force)
         * force_component_sign_along_axial_direction
         * axial_direction
     )
     # If rod element does not have any contact with plane, plane cannot apply friction
     # force on the element. Thus lets set static friction force to 0.0 for the no contact points.
     static_friction_force_along_axial_direction[..., no_contact_point_idx] = 0.0
-    elements_to_nodes_inplace(
+    _elements_to_nodes_inplace(
         static_friction_force_along_axial_direction, external_forces
     )
 
     # now rolling static friction
     # there is some normal, tangent and rolling directions inconsitency from Elastica
     total_torques = _batch_matvec(
         directors_transpose, (internal_torques + external_torques)
@@ -616,351 +769,25 @@
         np.minimum(np.fabs(noslip_force), max_friction_force)
         * noslip_force_sign
         * rolling_direction
     )
     # If rod element does not have any contact with plane, plane cannot apply friction
     # force on the element. Thus lets set plane static friction force to 0.0 for the no contact points.
     static_friction_force_along_rolling_direction[..., no_contact_point_idx] = 0.0
-    elements_to_nodes_inplace(
+    _elements_to_nodes_inplace(
         static_friction_force_along_rolling_direction, external_forces
     )
     external_torques += _batch_matvec(
         director_collection,
         _batch_cross(torque_arm, static_friction_force_along_rolling_direction),
     )
 
 
-# Slender body module
-@njit(cache=True)
-def sum_over_elements(input):
-    """
-    This function sums all elements of the input array.
-    Using a Numba njit decorator shows better performance
-    compared to python sum(), .sum() and np.sum()
-
-    Parameters
-    ----------
-    input: numpy.ndarray
-        1D (blocksize) array containing data with 'float' type.
-
-    Returns
-    -------
-    float
-
-    """
-    """
-    Developer Note
-    -----
-    Faster than sum(), .sum() and np.sum()
-
-    For blocksize = 200
-
-    sum(): 36.9 µs ± 3.99 µs per loop (mean ± std. dev. of 7 runs, 10000 loops each)
-
-    .sum(): 3.17 µs ± 90.1 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
-
-    np.sum(): 5.17 µs ± 364 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
-
-    This version: 513 ns ± 24.6 ns per loop (mean ± std. dev. of 7 runs, 1000000 loops each)
-    """
-
-    output = 0.0
-    for i in range(input.shape[0]):
-        output += input[i]
-
-    return output
-
-
-@njit(cache=True)
-def node_to_element_position(node_position_collection):
-    """
-    This function computes the position of the elements
-    from the nodal values.
-    Here we define a separate function because benchmark results
-    showed that using Numba, we get more than 3 times faster calculation.
-
-    Parameters
-    ----------
-    node_position_collection: numpy.ndarray
-        2D (dim, blocksize) array containing nodal positions with
-        'float' type.
-
-    Returns
-    -------
-    element_position_collection: numpy.ndarray
-        2D (dim, blocksize) array containing elemental positions with
-        'float' type.
-    """
-    """
-    Developer Notes
-    -----
-    Benchmark results, for a blocksize of 100,
-
-    Python version: 3.5 µs ± 149 ns per loop
-
-    This version: 729 ns ± 14.3 ns per loop
-
-    """
-    n_elem = node_position_collection.shape[1] - 1
-    element_position_collection = np.empty((3, n_elem))
-    for k in range(n_elem):
-        element_position_collection[0, k] = 0.5 * (
-            node_position_collection[0, k + 1] + node_position_collection[0, k]
-        )
-        element_position_collection[1, k] = 0.5 * (
-            node_position_collection[1, k + 1] + node_position_collection[1, k]
-        )
-        element_position_collection[2, k] = 0.5 * (
-            node_position_collection[2, k + 1] + node_position_collection[2, k]
-        )
-
-    return element_position_collection
-
-
-@njit(cache=True)
-def node_to_element_velocity(mass, node_velocity_collection):
-    """
-    This function computes the velocity of the elements
-    from the nodal values. Uses the velocity of center of mass
-    in order to conserve momentum during computation.
-
-    Parameters
-    ----------
-    mass: numpy.ndarray
-        2D (dim, blocksize) array containing nodal masses with
-        'float' type.
-    node_velocity_collection: numpy.ndarray
-        2D (dim, blocksize) array containing nodal velocities with
-        'float' type.
-
-    Returns
-    -------
-    element_velocity_collection: numpy.ndarray
-        2D (dim, blocksize) array containing elemental velocities with
-        'float' type.
-    """
-    n_elem = node_velocity_collection.shape[1] - 1
-    element_velocity_collection = np.empty((3, n_elem))
-    for k in range(n_elem):
-        element_velocity_collection[0, k] = (
-            mass[k + 1] * node_velocity_collection[0, k + 1]
-            + mass[k] * node_velocity_collection[0, k]
-        )
-        element_velocity_collection[1, k] = (
-            mass[k + 1] * node_velocity_collection[1, k + 1]
-            + mass[k] * node_velocity_collection[1, k]
-        )
-        element_velocity_collection[2, k] = (
-            mass[k + 1] * node_velocity_collection[2, k + 1]
-            + mass[k] * node_velocity_collection[2, k]
-        )
-        element_velocity_collection[:, k] /= mass[k + 1] + mass[k]
-
-    return element_velocity_collection
-
-
-def node_to_element_pos_or_vel(vector_in_node_frame):
-    # Remove the function beyond v0.4.0
-    raise NotImplementedError(
-        "This function is removed in v0.3.0. For node-to-element interpolation please use: \n"
-        "elastica.interaction.node_to_element_position() for rod position \n"
-        "elastica.interaction.node_to_element_velocity() for rod velocity. \n"
-        "For detail, refer to issue #80."
-    )
-
-
-@njit(cache=True)
-def slender_body_forces(
-    tangents, velocity_collection, dynamic_viscosity, lengths, radius, mass
-):
-    r"""
-    This function computes hydrodynamic forces on a body using slender body theory.
-    The below implementation is from Eq. 4.13 in Gazzola et al. RSoS. (2018).
-
-    .. math::
-        F_{h}=\frac{-4\pi\mu}{\ln{(L/r)}}\left(\mathbf{I}-\frac{1}{2}\mathbf{t}^{\textrm{T}}\mathbf{t}\right)\mathbf{v}
-
-
-
-    Parameters
-    ----------
-    tangents: numpy.ndarray
-        2D (dim, blocksize) array containing data with 'float' type.
-        Rod-like element tangent directions.
-    velocity_collection: numpy.ndarray
-        2D (dim, blocksize) array containing data with 'float' type.
-        Rod-like object velocity collection.
-    dynamic_viscosity: float
-        Dynamic viscosity of the fluid.
-    length: numpy.ndarray
-        1D (blocksize) array containing data with 'float' type.
-        Rod-like object element lengths.
-    radius: numpy.ndarray
-        1D (blocksize) array containing data with 'float' type.
-        Rod-like object element radius.
-    mass: numpy.ndarray
-        1D (blocksize) array containing data with 'float' type.
-        Rod-like object node mass.
-
-    Returns
-    -------
-    stokes_force: numpy.ndarray
-       2D (dim, blocksize) array containing data with 'float' type.
-    """
-
-    """
-    Developer Note
-    ----
-    Faster than numpy einsum implementation for blocksize 100
-
-    numpy: 39.5 µs ± 6.78 µs per loop (mean ± std. dev. of 7 runs, 10000 loops each)
-
-    this version: 3.91 µs ± 310 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
-    """
-
-    f = np.empty((tangents.shape[0], tangents.shape[1]))
-    total_length = sum_over_elements(lengths)
-    element_velocity = node_to_element_velocity(
-        mass=mass, node_velocity_collection=velocity_collection
-    )
-
-    for k in range(tangents.shape[1]):
-        # compute the entries of t`t. a[#][#] are the the
-        # entries of t`t matrix
-        a11 = tangents[0, k] * tangents[0, k]
-        a12 = tangents[0, k] * tangents[1, k]
-        a13 = tangents[0, k] * tangents[2, k]
-
-        a21 = tangents[1, k] * tangents[0, k]
-        a22 = tangents[1, k] * tangents[1, k]
-        a23 = tangents[1, k] * tangents[2, k]
-
-        a31 = tangents[2, k] * tangents[0, k]
-        a32 = tangents[2, k] * tangents[1, k]
-        a33 = tangents[2, k] * tangents[2, k]
-
-        # factor = - 4*pi*mu/ln(L/r)
-        factor = (
-            -4.0
-            * np.pi
-            * dynamic_viscosity
-            / np.log(total_length / radius[k])
-            * lengths[k]
-        )
-
-        # Fh = factor * ((I - 0.5 * a) * v)
-        f[0, k] = factor * (
-            (1.0 - 0.5 * a11) * element_velocity[0, k]
-            + (0.0 - 0.5 * a12) * element_velocity[1, k]
-            + (0.0 - 0.5 * a13) * element_velocity[2, k]
-        )
-        f[1, k] = factor * (
-            (0.0 - 0.5 * a21) * element_velocity[0, k]
-            + (1.0 - 0.5 * a22) * element_velocity[1, k]
-            + (0.0 - 0.5 * a23) * element_velocity[2, k]
-        )
-        f[2, k] = factor * (
-            (0.0 - 0.5 * a31) * element_velocity[0, k]
-            + (0.0 - 0.5 * a32) * element_velocity[1, k]
-            + (1.0 - 0.5 * a33) * element_velocity[2, k]
-        )
-
-    return f
-
-
-# slender body theory
-class SlenderBodyTheory(NoForces):
-    """
-    This slender body theory class is for flow-structure
-    interaction problems. This class applies hydrodynamic
-    forces on the body using the slender body theory given in
-    Eq. 4.13 of Gazzola et al. RSoS (2018).
-
-        Attributes
-        ----------
-        dynamic_viscosity: float
-            Dynamic viscosity of the fluid.
-
-    """
-
-    def __init__(self, dynamic_viscosity):
-        """
-
-        Parameters
-        ----------
-        dynamic_viscosity : float
-            Dynamic viscosity of the fluid.
-        """
-        super(SlenderBodyTheory, self).__init__()
-        self.dynamic_viscosity = dynamic_viscosity
-
-    def apply_forces(self, system, time=0.0):
-        """
-        This function applies hydrodynamic forces on body
-        using the slender body theory given in
-        Eq. 4.13 Gazzola et. al. RSoS 2018 paper
-
-        Parameters
-        ----------
-        system
-
-        Returns
-        -------
-
-        """
-
-        stokes_force = slender_body_forces(
-            system.tangents,
-            system.velocity_collection,
-            self.dynamic_viscosity,
-            system.lengths,
-            system.radius,
-            system.mass,
-        )
-        elements_to_nodes_inplace(stokes_force, system.external_forces)
-
-
-# base class for interaction
-# only applies normal force no friction
-class InteractionPlaneRigidBody:
-    def __init__(self, k, nu, plane_origin, plane_normal):
-        self.k = k
-        self.nu = nu
-        self.plane_origin = plane_origin.reshape(3, 1)
-        self.plane_normal = plane_normal.reshape(3)
-        self.surface_tol = 1e-4
-
-    def apply_normal_force(self, system):
-        """
-        This function computes the plane force response on the rigid body, in the
-        case of contact. Contact model given in Eqn 4.8 Gazzola et. al. RSoS 2018 paper
-        is used.
-        Parameters
-        ----------
-        system
-
-        Returns
-        -------
-        magnitude of the plane response
-        """
-        return apply_normal_force_numba_rigid_body(
-            self.plane_origin,
-            self.plane_normal,
-            self.surface_tol,
-            self.k,
-            self.nu,
-            system.length,
-            system.position_collection,
-            system.velocity_collection,
-            system.external_forces,
-        )
-
-
-@njit(cache=True)
-def apply_normal_force_numba_rigid_body(
+@numba.njit(cache=True)
+def _calculate_contact_forces_cylinder_plane(
     plane_origin,
     plane_normal,
     surface_tol,
     k,
     nu,
     length,
     position_collection,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyelastica-0.3.1.post1/elastica/joint.py` & `pyelastica-0.3.2/elastica/joint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 __doc__ = """ Module containing joint classes to connect multiple rods together. """
-
-from elastica._linalg import _batch_product_k_ik_to_ik
 from elastica._rotations import _inv_rotate
 from elastica.typing import SystemType, RodType
-from math import sqrt
-import numba
 import numpy as np
+import logging
 
 
 class FreeJoint:
     """
     This free joint class is the base class for all joints. Free or spherical
     joints constrains the relative movement between two nodes (chosen by the user)
     by applying restoring forces. For implementation details, refer to Zhang et al. Nature Communications (2019).
@@ -360,105 +357,55 @@
     """
     return (
         system_one.director_collection[..., index_one]
         @ system_two.director_collection[..., index_two].T
     )
 
 
-@numba.njit(cache=True)
+# everything below this comment should be removed beyond v0.4.0
 def _dot_product(a, b):
-    sum = 0.0
-    for i in range(3):
-        sum += a[i] * b[i]
-    return sum
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._dot_product()\n"
+        "instead for find the dot product between a and b."
+    )
 
 
-@numba.njit(cache=True)
 def _norm(a):
-    return sqrt(_dot_product(a, a))
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._norm()\n"
+        "instead for finding the norm of a."
+    )
 
 
-@numba.njit(cache=True)
 def _clip(x, low, high):
-    return max(low, min(x, high))
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._clip()\n"
+        "instead for clipping x."
+    )
 
 
-# Can this be made more efficient than 2 comp, 1 or?
-@numba.njit(cache=True)
 def _out_of_bounds(x, low, high):
-    return (x < low) or (x > high)
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._out_of_bounds()\n"
+        "instead for checking if x is out of bounds."
+    )
 
 
-@numba.njit(cache=True)
 def _find_min_dist(x1, e1, x2, e2):
-    e1e1 = _dot_product(e1, e1)
-    e1e2 = _dot_product(e1, e2)
-    e2e2 = _dot_product(e2, e2)
-
-    x1e1 = _dot_product(x1, e1)
-    x1e2 = _dot_product(x1, e2)
-    x2e1 = _dot_product(e1, x2)
-    x2e2 = _dot_product(x2, e2)
-
-    s = 0.0
-    t = 0.0
-
-    parallel = abs(1.0 - e1e2 ** 2 / (e1e1 * e2e2)) < 1e-6
-    if parallel:
-        # Some are parallel, so do processing
-        t = (x2e1 - x1e1) / e1e1  # Comes from taking dot of e1 with a normal
-        t = _clip(t, 0.0, 1.0)
-        s = (x1e2 + t * e1e2 - x2e2) / e2e2  # Same as before
-        s = _clip(s, 0.0, 1.0)
-    else:
-        # Using the Cauchy-Binet formula on eq(7) in docstring referenc
-        s = (e1e1 * (x1e2 - x2e2) + e1e2 * (x2e1 - x1e1)) / (e1e1 * e2e2 - (e1e2) ** 2)
-        t = (e1e2 * s + x2e1 - x1e1) / e1e1
-
-        if _out_of_bounds(s, 0.0, 1.0) or _out_of_bounds(t, 0.0, 1.0):
-            # potential_s = -100.0
-            # potential_t = -100.0
-            # potential_d = -100.0
-            # overall_minimum_distance = 1e20
-
-            # Fill in the possibilities
-            potential_t = (x2e1 - x1e1) / e1e1
-            s = 0.0
-            t = _clip(potential_t, 0.0, 1.0)
-            potential_d = _norm(x1 + e1 * t - x2)
-            overall_minimum_distance = potential_d
-
-            potential_t = (x2e1 + e1e2 - x1e1) / e1e1
-            potential_t = _clip(potential_t, 0.0, 1.0)
-            potential_d = _norm(x1 + e1 * potential_t - x2 - e2)
-            if potential_d < overall_minimum_distance:
-                s = 1.0
-                t = potential_t
-                overall_minimum_distance = potential_d
-
-            potential_s = (x1e2 - x2e2) / e2e2
-            potential_s = _clip(potential_s, 0.0, 1.0)
-            potential_d = _norm(x2 + potential_s * e2 - x1)
-            if potential_d < overall_minimum_distance:
-                s = potential_s
-                t = 0.0
-                overall_minimum_distance = potential_d
-
-            potential_s = (x1e2 + e1e2 - x2e2) / e2e2
-            potential_s = _clip(potential_s, 0.0, 1.0)
-            potential_d = _norm(x2 + potential_s * e2 - x1 - e1)
-            if potential_d < overall_minimum_distance:
-                s = potential_s
-                t = 1.0
-
-    # Return distance, contact point of system 2, contact point of system 1
-    return x2 + s * e2 - x1 - t * e1, x2 + s * e2, x1 - t * e1
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._find_min_dist()\n"
+        "instead for finding minimum distance between contact points."
+    )
 
 
-@numba.njit(cache=True)
 def _calculate_contact_forces_rod_rigid_body(
     x_collection_rod,
     edge_collection_rod,
     x_cylinder_center,
     x_cylinder_tip,
     edge_cylinder,
     radii_sum,
@@ -471,133 +418,21 @@
     velocity_rod,
     velocity_cylinder,
     contact_k,
     contact_nu,
     velocity_damping_coefficient,
     friction_coefficient,
 ):
-    # We already pass in only the first n_elem x
-    n_points = x_collection_rod.shape[1]
-    cylinder_total_contact_forces = np.zeros((3))
-    cylinder_total_contact_torques = np.zeros((3))
-    for i in range(n_points):
-        # Element-wise bounding box
-        x_selected = x_collection_rod[..., i]
-        # x_cylinder is already a (,) array from outised
-        del_x = x_selected - x_cylinder_tip
-        norm_del_x = _norm(del_x)
-
-        # If outside then don't process
-        if norm_del_x >= (radii_sum[i] + length_sum[i]):
-            continue
-
-        # find the shortest line segment between the two centerline
-        # segments : differs from normal cylinder-cylinder intersection
-        distance_vector, x_cylinder_contact_point, _ = _find_min_dist(
-            x_selected, edge_collection_rod[..., i], x_cylinder_tip, edge_cylinder
-        )
-        distance_vector_length = _norm(distance_vector)
-        distance_vector /= distance_vector_length
-
-        gamma = radii_sum[i] - distance_vector_length
-
-        # If distance is large, don't worry about it
-        if gamma < -1e-5:
-            continue
-
-        rod_elemental_forces = 0.5 * (
-            external_forces_rod[..., i]
-            + external_forces_rod[..., i + 1]
-            + internal_forces_rod[..., i]
-            + internal_forces_rod[..., i + 1]
-        )
-        equilibrium_forces = -rod_elemental_forces + external_forces_cylinder[..., 0]
-
-        normal_force = _dot_product(equilibrium_forces, distance_vector)
-        # Following line same as np.where(normal_force < 0.0, -normal_force, 0.0)
-        normal_force = abs(min(normal_force, 0.0))
-
-        # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
-        # As a quick fix, use this instead
-        mask = (gamma > 0.0) * 1.0
-
-        # Compute contact spring force
-        contact_force = contact_k * gamma * distance_vector
-        interpenetration_velocity = velocity_cylinder[..., 0] - 0.5 * (
-            velocity_rod[..., i] + velocity_rod[..., i + 1]
-        )
-        # Compute contact damping
-        normal_interpenetration_velocity = (
-            _dot_product(interpenetration_velocity, distance_vector) * distance_vector
-        )
-        contact_damping_force = -contact_nu * normal_interpenetration_velocity
-
-        # magnitude* direction
-        net_contact_force = 0.5 * mask * (contact_damping_force + contact_force)
-
-        # Compute friction
-        slip_interpenetration_velocity = (
-            interpenetration_velocity - normal_interpenetration_velocity
-        )
-        slip_interpenetration_velocity_mag = np.linalg.norm(
-            slip_interpenetration_velocity
-        )
-        slip_interpenetration_velocity_unitized = slip_interpenetration_velocity / (
-            slip_interpenetration_velocity_mag + 1e-14
-        )
-        # Compute friction force in the slip direction.
-        damping_force_in_slip_direction = (
-            velocity_damping_coefficient * slip_interpenetration_velocity_mag
-        )
-        # Compute Coulombic friction
-        coulombic_friction_force = friction_coefficient * np.linalg.norm(
-            net_contact_force
-        )
-        # Compare damping force in slip direction and kinetic friction and minimum is the friction force.
-        friction_force = (
-            -min(damping_force_in_slip_direction, coulombic_friction_force)
-            * slip_interpenetration_velocity_unitized
-        )
-        # Update contact force
-        net_contact_force += friction_force
-
-        # Torques acting on the cylinder
-        moment_arm = x_cylinder_contact_point - x_cylinder_center
-
-        # Add it to the rods at the end of the day
-        if i == 0:
-            external_forces_rod[..., i] -= 2 / 3 * net_contact_force
-            external_forces_rod[..., i + 1] -= 4 / 3 * net_contact_force
-            cylinder_total_contact_forces += 2.0 * net_contact_force
-            cylinder_total_contact_torques += np.cross(
-                moment_arm, 2.0 * net_contact_force
-            )
-        elif i == n_points:
-            external_forces_rod[..., i] -= 4 / 3 * net_contact_force
-            external_forces_rod[..., i + 1] -= 2 / 3 * net_contact_force
-            cylinder_total_contact_forces += 2.0 * net_contact_force
-            cylinder_total_contact_torques += np.cross(
-                moment_arm, 2.0 * net_contact_force
-            )
-        else:
-            external_forces_rod[..., i] -= net_contact_force
-            external_forces_rod[..., i + 1] -= net_contact_force
-            cylinder_total_contact_forces += 2.0 * net_contact_force
-            cylinder_total_contact_torques += np.cross(
-                moment_arm, 2.0 * net_contact_force
-            )
-
-    # Update the cylinder external forces and torques
-    external_forces_cylinder[..., 0] += cylinder_total_contact_forces
-    external_torques_cylinder[..., 0] += (
-        cylinder_director_collection @ cylinder_total_contact_torques
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica._contact_functions._calculate_contact_forces_rod_cylinder()\n"
+        "instead for calculating rod cylinder contact forces."
     )
 
 
-@numba.njit(cache=True)
 def _calculate_contact_forces_rod_rod(
     x_collection_rod_one,
     radius_rod_one,
     length_rod_one,
     tangent_rod_one,
     velocity_rod_one,
     internal_forces_rod_one,
@@ -608,291 +443,75 @@
     tangent_rod_two,
     velocity_rod_two,
     internal_forces_rod_two,
     external_forces_rod_two,
     contact_k,
     contact_nu,
 ):
-    # We already pass in only the first n_elem x
-    n_points_rod_one = x_collection_rod_one.shape[1]
-    n_points_rod_two = x_collection_rod_two.shape[1]
-    edge_collection_rod_one = _batch_product_k_ik_to_ik(length_rod_one, tangent_rod_one)
-    edge_collection_rod_two = _batch_product_k_ik_to_ik(length_rod_two, tangent_rod_two)
-
-    for i in range(n_points_rod_one):
-        for j in range(n_points_rod_two):
-            radii_sum = radius_rod_one[i] + radius_rod_two[j]
-            length_sum = length_rod_one[i] + length_rod_two[j]
-            # Element-wise bounding box
-            x_selected_rod_one = x_collection_rod_one[..., i]
-            x_selected_rod_two = x_collection_rod_two[..., j]
-
-            del_x = x_selected_rod_one - x_selected_rod_two
-            norm_del_x = _norm(del_x)
-
-            # If outside then don't process
-            if norm_del_x >= (radii_sum + length_sum):
-                continue
-
-            # find the shortest line segment between the two centerline
-            # segments : differs from normal cylinder-cylinder intersection
-            distance_vector, _, _ = _find_min_dist(
-                x_selected_rod_one,
-                edge_collection_rod_one[..., i],
-                x_selected_rod_two,
-                edge_collection_rod_two[..., j],
-            )
-            distance_vector_length = _norm(distance_vector)
-            distance_vector /= distance_vector_length
-
-            gamma = radii_sum - distance_vector_length
-
-            # If distance is large, don't worry about it
-            if gamma < -1e-5:
-                continue
-
-            rod_one_elemental_forces = 0.5 * (
-                external_forces_rod_one[..., i]
-                + external_forces_rod_one[..., i + 1]
-                + internal_forces_rod_one[..., i]
-                + internal_forces_rod_one[..., i + 1]
-            )
-
-            rod_two_elemental_forces = 0.5 * (
-                external_forces_rod_two[..., j]
-                + external_forces_rod_two[..., j + 1]
-                + internal_forces_rod_two[..., j]
-                + internal_forces_rod_two[..., j + 1]
-            )
-
-            equilibrium_forces = -rod_one_elemental_forces + rod_two_elemental_forces
-
-            normal_force = _dot_product(equilibrium_forces, distance_vector)
-            # Following line same as np.where(normal_force < 0.0, -normal_force, 0.0)
-            normal_force = abs(min(normal_force, 0.0))
-
-            # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
-            # As a quick fix, use this instead
-            mask = (gamma > 0.0) * 1.0
-
-            contact_force = contact_k * gamma
-            interpenetration_velocity = 0.5 * (
-                (velocity_rod_one[..., i] + velocity_rod_one[..., i + 1])
-                - (velocity_rod_two[..., j] + velocity_rod_two[..., j + 1])
-            )
-            contact_damping_force = contact_nu * _dot_product(
-                interpenetration_velocity, distance_vector
-            )
-
-            # magnitude* direction
-            net_contact_force = (
-                normal_force + 0.5 * mask * (contact_damping_force + contact_force)
-            ) * distance_vector
-
-            # Add it to the rods at the end of the day
-            if i == 0:
-                external_forces_rod_one[..., i] -= net_contact_force * 2 / 3
-                external_forces_rod_one[..., i + 1] -= net_contact_force * 4 / 3
-            elif i == n_points_rod_one:
-                external_forces_rod_one[..., i] -= net_contact_force * 4 / 3
-                external_forces_rod_one[..., i + 1] -= net_contact_force * 2 / 3
-            else:
-                external_forces_rod_one[..., i] -= net_contact_force
-                external_forces_rod_one[..., i + 1] -= net_contact_force
-
-            if j == 0:
-                external_forces_rod_two[..., j] += net_contact_force * 2 / 3
-                external_forces_rod_two[..., j + 1] += net_contact_force * 4 / 3
-            elif j == n_points_rod_two:
-                external_forces_rod_two[..., j] += net_contact_force * 4 / 3
-                external_forces_rod_two[..., j + 1] += net_contact_force * 2 / 3
-            else:
-                external_forces_rod_two[..., j] += net_contact_force
-                external_forces_rod_two[..., j + 1] += net_contact_force
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica._contact_functions._calculate_contact_forces_rod_rod()\n"
+        "instead for calculating rod rod contact forces."
+    )
 
 
-@numba.njit(cache=True)
 def _calculate_contact_forces_self_rod(
     x_collection_rod,
     radius_rod,
     length_rod,
     tangent_rod,
     velocity_rod,
     external_forces_rod,
     contact_k,
     contact_nu,
 ):
-    # We already pass in only the first n_elem x
-    n_points_rod = x_collection_rod.shape[1]
-    edge_collection_rod_one = _batch_product_k_ik_to_ik(length_rod, tangent_rod)
-
-    for i in range(n_points_rod):
-        skip = 1 + np.ceil(0.8 * np.pi * radius_rod[i] / length_rod[i])
-        for j in range(i - skip, -1, -1):
-            radii_sum = radius_rod[i] + radius_rod[j]
-            length_sum = length_rod[i] + length_rod[j]
-            # Element-wise bounding box
-            x_selected_rod_index_i = x_collection_rod[..., i]
-            x_selected_rod_index_j = x_collection_rod[..., j]
-
-            del_x = x_selected_rod_index_i - x_selected_rod_index_j
-            norm_del_x = _norm(del_x)
-
-            # If outside then don't process
-            if norm_del_x >= (radii_sum + length_sum):
-                continue
-
-            # find the shortest line segment between the two centerline
-            # segments : differs from normal cylinder-cylinder intersection
-            distance_vector, _, _ = _find_min_dist(
-                x_selected_rod_index_i,
-                edge_collection_rod_one[..., i],
-                x_selected_rod_index_j,
-                edge_collection_rod_one[..., j],
-            )
-            distance_vector_length = _norm(distance_vector)
-            distance_vector /= distance_vector_length
-
-            gamma = radii_sum - distance_vector_length
-
-            # If distance is large, don't worry about it
-            if gamma < -1e-5:
-                continue
-
-            # CHECK FOR GAMMA > 0.0, heaviside but we need to overload it in numba
-            # As a quick fix, use this instead
-            mask = (gamma > 0.0) * 1.0
-
-            contact_force = contact_k * gamma
-            interpenetration_velocity = 0.5 * (
-                (velocity_rod[..., i] + velocity_rod[..., i + 1])
-                - (velocity_rod[..., j] + velocity_rod[..., j + 1])
-            )
-            contact_damping_force = contact_nu * _dot_product(
-                interpenetration_velocity, distance_vector
-            )
-
-            # magnitude* direction
-            net_contact_force = (
-                0.5 * mask * (contact_damping_force + contact_force)
-            ) * distance_vector
-
-            # Add it to the rods at the end of the day
-            # if i == 0:
-            #     external_forces_rod[...,i] -= net_contact_force *2/3
-            #     external_forces_rod[...,i+1] -= net_contact_force * 4/3
-            if i == n_points_rod:
-                external_forces_rod[..., i] -= net_contact_force * 4 / 3
-                external_forces_rod[..., i + 1] -= net_contact_force * 2 / 3
-            else:
-                external_forces_rod[..., i] -= net_contact_force
-                external_forces_rod[..., i + 1] -= net_contact_force
-
-            if j == 0:
-                external_forces_rod[..., j] += net_contact_force * 2 / 3
-                external_forces_rod[..., j + 1] += net_contact_force * 4 / 3
-            # elif j == n_points_rod:
-            #     external_forces_rod[..., j] += net_contact_force * 4/3
-            #     external_forces_rod[..., j+1] += net_contact_force * 2/3
-            else:
-                external_forces_rod[..., j] += net_contact_force
-                external_forces_rod[..., j + 1] += net_contact_force
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica._contact_functions._calculate_contact_forces_self_rod()\n"
+        "instead for calculating rod self-contact forces."
+    )
 
 
-@numba.njit(cache=True)
 def _aabbs_not_intersecting(aabb_one, aabb_two):
-    """Returns true if not intersecting else false"""
-    if (aabb_one[0, 1] < aabb_two[0, 0]) | (aabb_one[0, 0] > aabb_two[0, 1]):
-        return 1
-    if (aabb_one[1, 1] < aabb_two[1, 0]) | (aabb_one[1, 0] > aabb_two[1, 1]):
-        return 1
-    if (aabb_one[2, 1] < aabb_two[2, 0]) | (aabb_one[2, 0] > aabb_two[2, 1]):
-        return 1
-
-    return 0
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._aabbs_not_intersecting()\n"
+        "instead for checking aabbs intersection."
+    )
 
 
-@numba.njit(cache=True)
 def _prune_using_aabbs_rod_rigid_body(
     rod_one_position_collection,
     rod_one_radius_collection,
     rod_one_length_collection,
     cylinder_position,
     cylinder_director,
     cylinder_radius,
     cylinder_length,
 ):
-    max_possible_dimension = np.zeros((3,))
-    aabb_rod = np.empty((3, 2))
-    aabb_cylinder = np.empty((3, 2))
-    max_possible_dimension[...] = np.max(rod_one_radius_collection) + np.max(
-        rod_one_length_collection
-    )
-    for i in range(3):
-        aabb_rod[i, 0] = (
-            np.min(rod_one_position_collection[i]) - max_possible_dimension[i]
-        )
-        aabb_rod[i, 1] = (
-            np.max(rod_one_position_collection[i]) + max_possible_dimension[i]
-        )
-
-    # Is actually Q^T * d but numba complains about performance so we do
-    # d^T @ Q
-    cylinder_dimensions_in_local_FOR = np.array(
-        [cylinder_radius, cylinder_radius, 0.5 * cylinder_length]
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._prune_using_aabbs_rod_cylinder()\n"
+        "instead for checking rod cylinder intersection."
     )
-    cylinder_dimensions_in_world_FOR = np.zeros_like(cylinder_dimensions_in_local_FOR)
-    for i in range(3):
-        for j in range(3):
-            cylinder_dimensions_in_world_FOR[i] += (
-                cylinder_director[j, i, 0] * cylinder_dimensions_in_local_FOR[j]
-            )
-
-    max_possible_dimension = np.abs(cylinder_dimensions_in_world_FOR)
-    aabb_cylinder[..., 0] = cylinder_position[..., 0] - max_possible_dimension
-    aabb_cylinder[..., 1] = cylinder_position[..., 0] + max_possible_dimension
-    return _aabbs_not_intersecting(aabb_cylinder, aabb_rod)
 
 
-@numba.njit(cache=True)
 def _prune_using_aabbs_rod_rod(
     rod_one_position_collection,
     rod_one_radius_collection,
     rod_one_length_collection,
     rod_two_position_collection,
     rod_two_radius_collection,
     rod_two_length_collection,
 ):
-    max_possible_dimension = np.zeros((3,))
-    aabb_rod_one = np.empty((3, 2))
-    aabb_rod_two = np.empty((3, 2))
-    max_possible_dimension[...] = np.max(rod_one_radius_collection) + np.max(
-        rod_one_length_collection
+    raise NotImplementedError(
+        "This function is removed in v0.3.2. Please use\n"
+        "elastica.contact_utils._prune_using_aabbs_rod_rod()\n"
+        "instead for checking rod rod intersection."
     )
-    for i in range(3):
-        aabb_rod_one[i, 0] = (
-            np.min(rod_one_position_collection[i]) - max_possible_dimension[i]
-        )
-        aabb_rod_one[i, 1] = (
-            np.max(rod_one_position_collection[i]) + max_possible_dimension[i]
-        )
-
-    max_possible_dimension[...] = np.max(rod_two_radius_collection) + np.max(
-        rod_two_length_collection
-    )
-
-    for i in range(3):
-        aabb_rod_two[i, 0] = (
-            np.min(rod_two_position_collection[i]) - max_possible_dimension[i]
-        )
-        aabb_rod_two[i, 1] = (
-            np.max(rod_two_position_collection[i]) + max_possible_dimension[i]
-        )
-
-    return _aabbs_not_intersecting(aabb_rod_two, aabb_rod_one)
 
 
 class ExternalContact(FreeJoint):
     """
     This class is for applying contact forces between rod-cylinder and rod-rod.
     If you are want to apply contact forces between rod and cylinder, first system is always rod and second system
     is always cylinder.
@@ -950,32 +569,50 @@
             slip direction.
         friction_coefficient : float
             For Coulombic friction coefficient for rigid-body and rod contact.
         """
         super().__init__(k, nu)
         self.velocity_damping_coefficient = velocity_damping_coefficient
         self.friction_coefficient = friction_coefficient
+        log = logging.getLogger(self.__class__.__name__)
+        log.warning(
+            # Remove warning and add error if ExternalContact is used in v0.3.3
+            # Remove the option to use ExternalContact, beyond v0.3.3
+            "The option to use the ExternalContact joint for the rod-rod and rod-cylinder contact is now deprecated.\n"
+            "Instead, for rod-rod contact or rod-cylinder contact,use RodRodContact or RodCylinderContact from the add-on Contact mixin class.\n"
+            "For reference see the classes elastica.contact_forces.RodRodContact() and elastica.contact_forces.RodCylinderContact().\n"
+            "For usage check examples/RigidbodyCases/RodRigidBodyContact/rod_cylinder_contact.py and examples/RodContactCase/RodRodContact/rod_rod_contact_parallel_validation.py.\n"
+            " The option to use the ExternalContact joint for the rod-rod and rod-cylinder will be removed in the future (v0.3.3).\n"
+        )
 
     def apply_forces(
         self,
         rod_one: RodType,
         index_one,
         rod_two: SystemType,
         index_two,
     ):
         # del index_one, index_two
+        from elastica.contact_utils import (
+            _prune_using_aabbs_rod_cylinder,
+            _prune_using_aabbs_rod_rod,
+        )
+        from elastica._contact_functions import (
+            _calculate_contact_forces_rod_cylinder,
+            _calculate_contact_forces_rod_rod,
+        )
 
         # TODO: raise error during the initialization if rod one is rigid body.
 
         # If rod two has one element, then it is rigid body.
         if rod_two.n_elems == 1:
             cylinder_two = rod_two
             # First, check for a global AABB bounding box, and see whether that
             # intersects
-            if _prune_using_aabbs_rod_rigid_body(
+            if _prune_using_aabbs_rod_cylinder(
                 rod_one.position_collection,
                 rod_one.radius,
                 rod_one.lengths,
                 cylinder_two.position_collection,
                 cylinder_two.director_collection,
                 cylinder_two.radius[0],
                 cylinder_two.length[0],
@@ -987,15 +624,15 @@
                 - 0.5 * cylinder_two.length * cylinder_two.director_collection[2, :, 0]
             )
 
             rod_element_position = 0.5 * (
                 rod_one.position_collection[..., 1:]
                 + rod_one.position_collection[..., :-1]
             )
-            _calculate_contact_forces_rod_rigid_body(
+            _calculate_contact_forces_rod_cylinder(
                 rod_element_position,
                 rod_one.lengths * rod_one.tangents,
                 cylinder_two.position_collection[..., 0],
                 x_cyl,
                 cylinder_two.length * cylinder_two.director_collection[2, :, 0],
                 rod_one.radius + cylinder_two.radius,
                 rod_one.lengths + cylinder_two.length,
@@ -1054,17 +691,29 @@
     """
     This class is modeling self contact of rod.
 
     """
 
     def __init__(self, k, nu):
         super().__init__(k, nu)
+        log = logging.getLogger(self.__class__.__name__)
+        log.warning(
+            # Remove warning and add error if SelfContact is used in v0.3.3
+            # Remove the option to use SelfContact, beyond v0.3.3
+            "The option to use the SelfContact joint for the rod self contact is now deprecated.\n"
+            "Instead, for rod self contact use RodSelfContact from the add-on Contact mixin class.\n"
+            "For reference see the class elastica.contact_forces.RodSelfContact(), and for usage check examples/RodContactCase/RodSelfContact/solenoids.py.\n"
+            "The option to use the SelfContact joint for the rod self contact will be removed in the future (v0.3.3).\n"
+        )
 
     def apply_forces(self, rod_one: RodType, index_one, rod_two: SystemType, index_two):
         # del index_one, index_two
+        from elastica._contact_functions import (
+            _calculate_contact_forces_self_rod,
+        )
 
         _calculate_contact_forces_self_rod(
             rod_one.position_collection[
                 ..., :-1
             ],  # Discount last node, we want element start position
             rod_one.radius,
             rod_one.lengths,
```

### Comparing `pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rigid_body.py` & `pyelastica-0.3.2/elastica/memory_block/memory_block_rigid_body.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 __doc__ = """Create block-structure class for collection of rigid body systems."""
 import numpy as np
-from typing import Sequence, List
+from typing import Sequence, Literal
 
 from elastica.rigidbody import RigidBodyBase
 from elastica.rigidbody.data_structures import _RigidRodSymplecticStepperMixin
 
 
 class MemoryBlockRigidBody(RigidBodyBase, _RigidRodSymplecticStepperMixin):
-    def __init__(self, systems: Sequence, system_idx_list: List[int]):
+    def __init__(self, systems: Sequence, system_idx_list: Sequence[np.int64]):
 
         self.n_bodies = len(systems)
         self.n_elems = self.n_bodies
         self.n_nodes = self.n_elems
         self.system_idx_list = np.array(system_idx_list, dtype=np.int64)
 
         # Allocate block structure using system collection.
-        self.allocate_block_variables_scalars(systems)
-        self.allocate_block_variables_vectors(systems)
-        self.allocate_block_variables_matrix(systems)
-        self.allocate_block_variables_for_symplectic_stepper(systems)
+        self._allocate_block_variables_scalars(systems)
+        self._allocate_block_variables_vectors(systems)
+        self._allocate_block_variables_matrix(systems)
+        self._allocate_block_variables_for_symplectic_stepper(systems)
 
         # Initialize the mixin class for symplectic time-stepper.
         _RigidRodSymplecticStepperMixin.__init__(self)
 
-    def allocate_block_variables_scalars(self, systems: Sequence):
+    def _allocate_block_variables_scalars(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables for
         block-structure and references allocated variables back to the systems.
 
         Parameters
         ----------
         systems
@@ -51,27 +51,22 @@
             "volume": 3,
             "mass": 4,
         }
         self.scalar_dofs_in_rigid_bodies = np.zeros(
             (len(map_scalar_dofs_in_rigid_bodies), self.n_elems)
         )
 
-        for k, v in map_scalar_dofs_in_rigid_bodies.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.scalar_dofs_in_rigid_bodies[v], (self.n_elems,)
-            )
-
-        for k, v in map_scalar_dofs_in_rigid_bodies.items():
-            for system_idx, system in enumerate(systems):
-                self.__dict__[k][..., system_idx : system_idx + 1] = system.__dict__[k]
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., system_idx : system_idx + 1]
-                )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_scalar_dofs_in_rigid_bodies,
+            systems=systems,
+            block_memory=self.scalar_dofs_in_rigid_bodies,
+            value_type="scalar",
+        )
 
-    def allocate_block_variables_vectors(self, systems: Sequence):
+    def _allocate_block_variables_vectors(self, systems: Sequence):
         """
         This function takes system collection and allocates the vector variables for
         block-structure and references allocated vector variables back to the systems.
 
         Parameters
         ----------
         systems
@@ -92,36 +87,29 @@
             "external_torques": 2,
         }
 
         self.vector_dofs_in_rigid_bodies = np.zeros(
             (len(map_vector_dofs_in_rigid_bodies), 3 * self.n_elems)
         )
 
-        for k, v in map_vector_dofs_in_rigid_bodies.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.vector_dofs_in_rigid_bodies[v], (3, self.n_elems)
-            )
-
-        for k, v in map_vector_dofs_in_rigid_bodies.items():
-            for system_idx, system in enumerate(systems):
-                self.__dict__[k][..., system_idx : system_idx + 1] = system.__dict__[
-                    k
-                ].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., system_idx : system_idx + 1]
-                )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_vector_dofs_in_rigid_bodies,
+            systems=systems,
+            block_memory=self.vector_dofs_in_rigid_bodies,
+            value_type="vector",
+        )
 
-    def allocate_block_variables_matrix(self, systems: Sequence):
+    def _allocate_block_variables_matrix(self, systems: Sequence):
         """
         This function takes system collection and allocates the matrix variables for
         block-structure and references allocated matrix variables back to the systems.
 
         Parameters
         ----------
-        system
+        systems
 
         Returns
         -------
 
         """
 
         # Things in rigid bodies that are matrix
@@ -135,29 +123,22 @@
             "inv_mass_second_moment_of_inertia": 2,
         }
 
         self.matrix_dofs_in_rigid_bodies = np.zeros(
             (len(map_matrix_dofs_in_rigid_bodies), 9 * self.n_elems)
         )
 
-        for k, v in map_matrix_dofs_in_rigid_bodies.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.matrix_dofs_in_rigid_bodies[v], (3, 3, self.n_elems)
-            )
-
-        for k, v in map_matrix_dofs_in_rigid_bodies.items():
-            for system_idx, system in enumerate(systems):
-                self.__dict__[k][..., system_idx : system_idx + 1] = system.__dict__[
-                    k
-                ].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., system_idx : system_idx + 1]
-                )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_matrix_dofs_in_rigid_bodies,
+            systems=systems,
+            block_memory=self.matrix_dofs_in_rigid_bodies,
+            value_type="tensor",
+        )
 
-    def allocate_block_variables_for_symplectic_stepper(self, systems: Sequence):
+    def _allocate_block_variables_for_symplectic_stepper(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables used by symplectic
         stepper for block-structure and references allocated variables back to the systems.
 
         Parameters
         ----------
         systems
@@ -177,29 +158,74 @@
         map_rate_collection = {
             "velocity_collection": 0,
             "omega_collection": 1,
             "acceleration_collection": 2,
             "alpha_collection": 3,
         }
         self.rate_collection = np.zeros((len(map_rate_collection), 3 * self.n_elems))
-        for k, v in map_rate_collection.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.rate_collection[v], (3, self.n_elems)
-            )
-
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_rate_collection,
+            systems=systems,
+            block_memory=self.rate_collection,
+            value_type="vector",
+        )
         # For Dynamic state update of position Verlet create references
         self.v_w_collection = np.lib.stride_tricks.as_strided(
             self.rate_collection[0:2], (2, 3 * self.n_elems)
         )
 
         self.dvdt_dwdt_collection = np.lib.stride_tricks.as_strided(
             self.rate_collection[2:-1], (2, 3 * self.n_elems)
         )
 
-        for k, v in map_rate_collection.items():
+    def _map_system_properties_to_block_memory(
+        self,
+        mapping_dict: dict,
+        systems: Sequence,
+        block_memory: np.ndarray,
+        value_type: Literal["scalar", "vector", "tensor"],
+    ) -> None:
+        """Map system (rigid bodies) properties to memory blocks.
+
+        Parameters
+        ----------
+        mapping_dict: dict
+            Dictionary with attribute names as keys and block row index as values.
+        systems: Sequence
+            A sequence containing Cosserat rod objects to map from.
+        block_memory: ndarray
+            Memory block that, at the end of the method execution, contains all designated
+            attributes of all systems.
+        value_type: str
+            A string that indicates the shape of the attribute.
+            Options among "scalar", "vector", and "tensor".
+
+        """
+        if value_type == "scalar":
+            view_shape = (self.n_elems,)
+
+        elif value_type == "vector":
+            view_shape = (3, self.n_elems)
+
+        elif value_type == "tensor":
+            view_shape = (3, 3, self.n_elems)
+
+        else:
+            raise ValueError(
+                "Incorrect value type. Must be one of scalar, vector, and tensor."
+            )
+
+        for k, v in mapping_dict.items():
+            self.__dict__[k] = np.lib.stride_tricks.as_strided(
+                block_memory[v],
+                shape=view_shape,
+            )
+
             for system_idx, system in enumerate(systems):
-                self.__dict__[k][..., system_idx : system_idx + 1] = system.__dict__[
-                    k
-                ].copy()
+                self.__dict__[k][..., system_idx : system_idx + 1] = (
+                    system.__dict__[k]
+                    if value_type == "scalar"
+                    else system.__dict__[k].copy()
+                )
                 system.__dict__[k] = np.ndarray.view(
                     self.__dict__[k][..., system_idx : system_idx + 1]
                 )
```

### Comparing `pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rod.py` & `pyelastica-0.3.2/elastica/memory_block/memory_block_rod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __doc__ = """Create block-structure class for collection of Cosserat rod systems."""
 import numpy as np
-from typing import Sequence
+from typing import Sequence, Literal, Callable
 from elastica.memory_block.memory_block_rod_base import (
     MemoryBlockRodBase,
     make_block_memory_metadata,
     make_block_memory_periodic_boundary_metadata,
 )
 from elastica.rod.data_structures import _RodSymplecticStepperMixin
 from elastica.reset_functions_for_block_structure import _reset_scalar_ghost
@@ -138,53 +138,38 @@
                 self.periodic_boundary_elems_idx += (
                     self.ghost_elems_idx[1::2][n_straight_rods - 1] + 1
                 )
                 self.periodic_boundary_voronoi_idx += (
                     self.ghost_voronoi_idx[2::3][n_straight_rods - 1] + 1
                 )
 
-                # Compute the start and end of the rod nodes again. This time, boundary cells are added.
-                self.start_idx_in_rod_nodes[n_straight_rods:] = (
-                    self.periodic_boundary_nodes_idx[0, 0::3] + 1
-                )
-                self.end_idx_in_rod_nodes[
-                    n_straight_rods:
-                ] = self.periodic_boundary_nodes_idx[0, 1::3]
+            # Compute the start and end of the rod nodes again. This time, boundary cells are added.
+            self.start_idx_in_rod_nodes[n_straight_rods:] = (
+                self.periodic_boundary_nodes_idx[0, 0::3] + 1
+            )
+            self.end_idx_in_rod_nodes[
+                n_straight_rods:
+            ] = self.periodic_boundary_nodes_idx[0, 1::3]
+
+            self.start_idx_in_rod_elems[n_straight_rods:] = (
+                self.periodic_boundary_elems_idx[0, 0::2] + 1
+            )
+            self.end_idx_in_rod_elems[
+                n_straight_rods:
+            ] = self.periodic_boundary_elems_idx[0, 1::2]
 
-                self.start_idx_in_rod_elems[n_straight_rods:] = (
-                    self.periodic_boundary_elems_idx[0, 0::2] + 1
-                )
-                self.end_idx_in_rod_elems[
-                    n_straight_rods:
-                ] = self.periodic_boundary_elems_idx[0, 1::2]
-
-                self.start_idx_in_rod_voronoi[n_straight_rods:] = (
-                    self.periodic_boundary_voronoi_idx[0, :] + 1
-                )
-            else:
-                # Compute the start and end of the rod nodes again. This time, boundary cells are added.
-                self.start_idx_in_rod_nodes[:] = (
-                    self.periodic_boundary_nodes_idx[0, 0::3] + 1
-                )
-                self.end_idx_in_rod_nodes[:] = self.periodic_boundary_nodes_idx[0, 1::3]
-
-                self.start_idx_in_rod_elems[:] = (
-                    self.periodic_boundary_elems_idx[0, 0::2] + 1
-                )
-                self.end_idx_in_rod_elems[:] = self.periodic_boundary_elems_idx[0, 1::2]
-
-                self.start_idx_in_rod_voronoi[:] = (
-                    self.periodic_boundary_voronoi_idx[0, :] + 1
-                )
+            self.start_idx_in_rod_voronoi[n_straight_rods:] = (
+                self.periodic_boundary_voronoi_idx[0, :] + 1
+            )
 
         # Allocate block structure using system collection.
-        self.allocate_block_variables_in_nodes(systems)
-        self.allocate_block_variables_in_elements(systems)
-        self.allocate_blocks_variables_in_voronoi(systems)
-        self.allocate_blocks_variables_for_symplectic_stepper(systems)
+        self._allocate_block_variables_in_nodes(systems)
+        self._allocate_block_variables_in_elements(systems)
+        self._allocate_blocks_variables_in_voronoi(systems)
+        self._allocate_blocks_variables_for_symplectic_stepper(systems)
 
         # Reset ghosts of mass, rest length and rest voronoi length to 1. Otherwise
         # since ghosts are not modified, this causes a division by zero error.
         _reset_scalar_ghost(self.mass, self.ghost_nodes_idx, 1.0)
         _reset_scalar_ghost(self.rest_lengths, self.ghost_elems_idx, 1.0)
         _reset_scalar_ghost(self.rest_voronoi_lengths, self.ghost_voronoi_idx, 1.0)
 
@@ -211,15 +196,15 @@
             _synchronize_periodic_boundary_of_vector_collection(
                 self.rest_kappa, self.periodic_boundary_voronoi_idx
             )
 
         # Initialize the mixin class for symplectic time-stepper.
         _RodSymplecticStepperMixin.__init__(self)
 
-    def allocate_block_variables_in_nodes(self, systems: Sequence):
+    def _allocate_block_variables_in_nodes(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables on
         node for block-structure and references allocated variables back to the
         systems.
 
         Parameters
         ----------
@@ -232,67 +217,44 @@
 
         # Things in nodes that are scalars
         #             0 ("mass", float64[:]),
         map_scalar_dofs_in_rod_nodes = {"mass": 0}
         self.scalar_dofs_in_rod_nodes = np.zeros(
             (len(map_scalar_dofs_in_rod_nodes), self.n_nodes)
         )
-        for k, v in map_scalar_dofs_in_rod_nodes.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.scalar_dofs_in_rod_nodes[v], (self.n_nodes,)
-            )
-
-        for k, v in map_scalar_dofs_in_rod_nodes.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_nodes[system_idx]
-                end_idx = self.end_idx_in_rod_nodes[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic node boundaries
-            _synchronize_periodic_boundary_of_scalar_collection(
-                self.__dict__[k], self.periodic_boundary_nodes_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_scalar_dofs_in_rod_nodes,
+            systems=systems,
+            block_memory=self.scalar_dofs_in_rod_nodes,
+            domain_type="node",
+            value_type="scalar",
+        )
 
         # Things in nodes that are vectors
         #             0 ("position_collection", float64[:, :]),
         #             1 ("internal_forces", float64[:, :]),
         #             2 ("external_forces", float64[:, :]),
         # 6 in total
         map_vector_dofs_in_rod_nodes = {
             "position_collection": 0,
             "internal_forces": 1,
             "external_forces": 2,
         }
         self.vector_dofs_in_rod_nodes = np.zeros(
             (len(map_vector_dofs_in_rod_nodes), 3 * self.n_nodes)
         )
-        for k, v in map_vector_dofs_in_rod_nodes.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.vector_dofs_in_rod_nodes[v], (3, self.n_nodes)
-            )
-
-        for k, v in map_vector_dofs_in_rod_nodes.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_nodes[system_idx]
-                end_idx = self.end_idx_in_rod_nodes[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic node boundaries
-            _synchronize_periodic_boundary_of_vector_collection(
-                self.__dict__[k], self.periodic_boundary_nodes_idx
-            )
-
-        # Things in nodes that are matrices
-        # Null set
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_vector_dofs_in_rod_nodes,
+            systems=systems,
+            block_memory=self.vector_dofs_in_rod_nodes,
+            domain_type="node",
+            value_type="vector",
+        )
 
-    def allocate_block_variables_in_elements(self, systems: Sequence):
+    def _allocate_block_variables_in_elements(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables on
         elements for block-structure and references allocated variables back to the
         systems.
 
         Parameters
         ----------
@@ -319,31 +281,21 @@
             "rest_lengths": 4,
             "dilatation": 5,
             "dilatation_rate": 6,
         }
         self.scalar_dofs_in_rod_elems = np.zeros(
             (len(map_scalar_dofs_in_rod_elems), self.n_elems)
         )
-        for k, v in map_scalar_dofs_in_rod_elems.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.scalar_dofs_in_rod_elems[v], (self.n_elems,)
-            )
-
-        for k, v in map_scalar_dofs_in_rod_elems.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_elems[system_idx]
-                end_idx = self.end_idx_in_rod_elems[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic element boundaries
-            _synchronize_periodic_boundary_of_scalar_collection(
-                self.__dict__[k], self.periodic_boundary_elems_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_scalar_dofs_in_rod_elems,
+            systems=systems,
+            block_memory=self.scalar_dofs_in_rod_elems,
+            domain_type="element",
+            value_type="scalar",
+        )
 
         # Things in elements that are vectors
         #             0 ("tangents", float64[:, :]),
         #             1 ("sigma", float64[:, :]),
         #             2 ("rest_sigma", float64[:, :]),
         #             3 ("internal_torques", float64[:, :]),
         #             4 ("external_torques", float64[:, :]),
@@ -355,31 +307,21 @@
             "internal_torques": 3,
             "external_torques": 4,
             "internal_stress": 5,
         }
         self.vector_dofs_in_rod_elems = np.zeros(
             (len(map_vector_dofs_in_rod_elems), 3 * self.n_elems)
         )
-        for k, v in map_vector_dofs_in_rod_elems.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.vector_dofs_in_rod_elems[v], (3, self.n_elems)
-            )
-
-        for k, v in map_vector_dofs_in_rod_elems.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_elems[system_idx]
-                end_idx = self.end_idx_in_rod_elems[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic element boundaries
-            _synchronize_periodic_boundary_of_vector_collection(
-                self.__dict__[k], self.periodic_boundary_elems_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_vector_dofs_in_rod_elems,
+            systems=systems,
+            block_memory=self.vector_dofs_in_rod_elems,
+            domain_type="element",
+            value_type="vector",
+        )
 
         # Things in elements that are matrices
         #             0 ("director_collection", float64[:, :, :]),
         #             1 ("mass_second_moment_of_inertia", float64[:, :, :]),
         #             2 ("inv_mass_second_moment_of_inertia", float64[:, :, :]),
         #             3 ("shear_matrix", float64[:, :, :]),
         map_matrix_dofs_in_rod_elems = {
@@ -387,33 +329,23 @@
             "mass_second_moment_of_inertia": 1,
             "inv_mass_second_moment_of_inertia": 2,
             "shear_matrix": 3,
         }
         self.matrix_dofs_in_rod_elems = np.zeros(
             (len(map_matrix_dofs_in_rod_elems), 9 * self.n_elems)
         )
-        for k, v in map_matrix_dofs_in_rod_elems.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.matrix_dofs_in_rod_elems[v], (3, 3, self.n_elems)
-            )
-
-        for k, v in map_matrix_dofs_in_rod_elems.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_elems[system_idx]
-                end_idx = self.end_idx_in_rod_elems[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic element boundaries
-            _synchronize_periodic_boundary_of_matrix_collection(
-                self.__dict__[k], self.periodic_boundary_elems_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_matrix_dofs_in_rod_elems,
+            systems=systems,
+            block_memory=self.matrix_dofs_in_rod_elems,
+            domain_type="element",
+            value_type="tensor",
+        )
 
-    def allocate_blocks_variables_in_voronoi(self, systems: Sequence):
+    def _allocate_blocks_variables_in_voronoi(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables on
         voronoi for block-structure and references allocated variables back to the
         systems.
 
         Parameters
         ----------
@@ -430,88 +362,57 @@
         map_scalar_dofs_in_rod_voronois = {
             "voronoi_dilatation": 0,
             "rest_voronoi_lengths": 1,
         }
         self.scalar_dofs_in_rod_voronois = np.zeros(
             (len(map_scalar_dofs_in_rod_voronois), self.n_voronoi)
         )
-        for k, v in map_scalar_dofs_in_rod_voronois.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.scalar_dofs_in_rod_voronois[v], (self.n_voronoi,)
-            )
-
-        for k, v in map_scalar_dofs_in_rod_voronois.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_voronoi[system_idx]
-                end_idx = self.end_idx_in_rod_voronoi[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic voronoi boundaries
-            _synchronize_periodic_boundary_of_scalar_collection(
-                self.__dict__[k], self.periodic_boundary_voronoi_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_scalar_dofs_in_rod_voronois,
+            systems=systems,
+            block_memory=self.scalar_dofs_in_rod_voronois,
+            domain_type="voronoi",
+            value_type="scalar",
+        )
 
         # Things in voronoi that are vectors
         #             0 ("kappa", float64[:, :]),
         #             1 ("rest_kappa", float64[:, :]),
         #             2 ("internal_couple", float64[:, :]),
         map_vector_dofs_in_rod_voronois = {
             "kappa": 0,
             "rest_kappa": 1,
             "internal_couple": 2,
         }
         self.vector_dofs_in_rod_voronois = np.zeros(
             (len(map_vector_dofs_in_rod_voronois), 3 * self.n_voronoi)
         )
-        for k, v in map_vector_dofs_in_rod_voronois.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.vector_dofs_in_rod_voronois[v], (3, self.n_voronoi)
-            )
-
-        for k, v in map_vector_dofs_in_rod_voronois.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_voronoi[system_idx]
-                end_idx = self.end_idx_in_rod_voronoi[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic voronoi boundaries
-            _synchronize_periodic_boundary_of_vector_collection(
-                self.__dict__[k], self.periodic_boundary_voronoi_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_vector_dofs_in_rod_voronois,
+            systems=systems,
+            block_memory=self.vector_dofs_in_rod_voronois,
+            domain_type="voronoi",
+            value_type="vector",
+        )
 
         # Things in voronoi that are matrices
         #             0 ("bend_matrix", float64[:, :, :]),
         map_matrix_dofs_in_rod_voronois = {"bend_matrix": 0}
         self.matrix_dofs_in_rod_voronois = np.zeros(
             (len(map_matrix_dofs_in_rod_voronois), 9 * self.n_voronoi)
         )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_matrix_dofs_in_rod_voronois,
+            systems=systems,
+            block_memory=self.matrix_dofs_in_rod_voronois,
+            domain_type="voronoi",
+            value_type="tensor",
+        )
 
-        for k, v in map_matrix_dofs_in_rod_voronois.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.matrix_dofs_in_rod_voronois[v], (3, 3, self.n_voronoi)
-            )
-
-        for k, v in map_matrix_dofs_in_rod_voronois.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_voronoi[system_idx]
-                end_idx = self.end_idx_in_rod_voronoi[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic voronoi boundaries
-            _synchronize_periodic_boundary_of_matrix_collection(
-                self.__dict__[k], self.periodic_boundary_voronoi_idx
-            )
-
-    def allocate_blocks_variables_for_symplectic_stepper(self, systems: Sequence):
+    def _allocate_blocks_variables_for_symplectic_stepper(self, systems: Sequence):
         """
         This function takes system collection and allocates the variables used by symplectic
         stepper for block-structure and references allocated variables back to the systems.
 
         Parameters
         ----------
         systems
@@ -531,75 +432,148 @@
         map_rate_collection = {
             "velocity_collection": 0,
             "omega_collection": 1,
             "acceleration_collection": 2,
             "alpha_collection": 3,
         }
         self.rate_collection = np.zeros((len(map_rate_collection), 3 * self.n_nodes))
-        for k, v in map_rate_collection.items():
-            self.__dict__[k] = np.lib.stride_tricks.as_strided(
-                self.rate_collection[v], (3, self.n_nodes)
-            )
-
-        self.__dict__["velocity_collection"] = np.lib.stride_tricks.as_strided(
-            self.rate_collection[0], (3, self.n_nodes)
-        )
-
-        self.__dict__["omega_collection"] = np.lib.stride_tricks.as_strided(
-            self.rate_collection[1],
-            (3, self.n_elems),
-        )
-
-        self.__dict__["acceleration_collection"] = np.lib.stride_tricks.as_strided(
-            self.rate_collection[2],
-            (3, self.n_nodes),
-        )
-
-        self.__dict__["alpha_collection"] = np.lib.stride_tricks.as_strided(
-            self.rate_collection[3],
-            (3, self.n_elems),
-        )
 
         # For Dynamic state update of position Verlet create references
         self.v_w_collection = np.lib.stride_tricks.as_strided(
             self.rate_collection[0:2], (2, 3 * self.n_nodes)
         )
 
         self.dvdt_dwdt_collection = np.lib.stride_tricks.as_strided(
-            self.rate_collection[2:-1], (2, 3 * self.n_nodes)
+            self.rate_collection[2:], (2, 3 * self.n_nodes)
         )
 
         # Copy systems variables on nodes to block structure
         map_rate_collection_dofs_in_rod_nodes = {
             "velocity_collection": 0,
-            "acceleration_collection": 1,
+            "acceleration_collection": 2,
         }
-        for k, v in map_rate_collection_dofs_in_rod_nodes.items():
-            for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_nodes[system_idx]
-                end_idx = self.end_idx_in_rod_nodes[system_idx]
-                self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
-                system.__dict__[k] = np.ndarray.view(
-                    self.__dict__[k][..., start_idx:end_idx]
-                )
-            # synchronize the periodic node boundaries
-            _synchronize_periodic_boundary_of_vector_collection(
-                self.__dict__[k], self.periodic_boundary_nodes_idx
-            )
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_rate_collection_dofs_in_rod_nodes,
+            systems=systems,
+            block_memory=self.rate_collection,
+            domain_type="node",
+            value_type="vector",
+        )
 
-        # Copy systems variables on nodes to block structure
+        # Copy systems variables on elements to block structure
         map_rate_collection_dofs_in_rod_elems = {
-            "omega_collection": 0,
-            "alpha_collection": 1,
+            "omega_collection": 1,
+            "alpha_collection": 3,
         }
-        for k, v in map_rate_collection_dofs_in_rod_elems.items():
+        self._map_system_properties_to_block_memory(
+            mapping_dict=map_rate_collection_dofs_in_rod_elems,
+            systems=systems,
+            block_memory=self.rate_collection,
+            domain_type="element",
+            value_type="vector",
+        )
+
+    def _map_system_properties_to_block_memory(
+        self,
+        mapping_dict: dict,
+        systems: Sequence,
+        block_memory: np.ndarray,
+        domain_type: Literal["node", "element", "voronoi"],
+        value_type: Literal["scalar", "vector", "tensor"],
+    ) -> None:
+        """Map system (Cosserat rods) properties to memory blocks.
+
+        This method take domain types (node, element, voronoi) and value
+        types (scalar, vector, tensor) as inputs and compute internally how to
+        construct the mapping properly.
+
+        Parameters
+        ----------
+        mapping_dict: dict
+            Dictionary with attribute names as keys and block row index as values.
+        systems: Sequence
+            A sequence containing Cosserat rod objects to map from.
+        block_memory: ndarray
+            Memory block that, at the end of the method execution, contains all designated
+            attributes of all systems.
+        domain_type: str
+            A string that indicates the discretized domain where the attributes reside.
+            Options among "node", "element", and "voronoi".
+        value_type: str
+            A string that indicates the shape of the attribute.
+            Options among "scalar", "vector", and "tensor".
+
+        """
+
+        # typedef
+        start_idx_list: np.ndarray
+        end_idx_list: np.ndarray
+        periodic_boundary_idx: np.ndarray
+        synchronize_periodic_boundary: Callable
+        domain_num: np.int64
+        view_shape: tuple
+
+        if domain_type == "node":
+            start_idx_list = self.start_idx_in_rod_nodes.view()
+            end_idx_list = self.end_idx_in_rod_nodes.view()
+            domain_num = self.n_nodes
+            periodic_boundary_idx = self.periodic_boundary_nodes_idx.view()
+
+        elif domain_type == "element":
+            start_idx_list = self.start_idx_in_rod_elems.view()
+            end_idx_list = self.end_idx_in_rod_elems.view()
+            domain_num = self.n_elems
+            periodic_boundary_idx = self.periodic_boundary_elems_idx.view()
+
+        elif domain_type == "voronoi":
+            start_idx_list = self.start_idx_in_rod_voronoi.view()
+            end_idx_list = self.end_idx_in_rod_voronoi.view()
+            domain_num = self.n_voronoi
+            periodic_boundary_idx = self.periodic_boundary_voronoi_idx.view()
+
+        else:
+            raise ValueError(
+                "Incorrect domain type. Must be one of node, element, and voronoi"
+            )
+
+        if value_type == "scalar":
+            view_shape = (domain_num,)
+            synchronize_periodic_boundary = (
+                _synchronize_periodic_boundary_of_scalar_collection
+            )
+
+        elif value_type == "vector":
+            view_shape = (3, domain_num)
+            synchronize_periodic_boundary = (
+                _synchronize_periodic_boundary_of_vector_collection
+            )
+
+        elif value_type == "tensor":
+            view_shape = (3, 3, domain_num)
+            synchronize_periodic_boundary = (
+                _synchronize_periodic_boundary_of_matrix_collection
+            )
+
+        else:
+            raise ValueError(
+                "Incorrect value type. Must be one of scalar, vector, and tensor."
+            )
+
+        for k, v in mapping_dict.items():
+            # Map class attributes to block memory
+            self.__dict__[k] = np.lib.stride_tricks.as_strided(
+                block_memory[v],
+                shape=view_shape,
+            )
+
+            # Copy system attributes into block memory, then make system attributes
+            # views into the block memory
             for system_idx, system in enumerate(systems):
-                start_idx = self.start_idx_in_rod_elems[system_idx]
-                end_idx = self.end_idx_in_rod_elems[system_idx]
+                start_idx = start_idx_list[system_idx]
+                end_idx = end_idx_list[system_idx]
                 self.__dict__[k][..., start_idx:end_idx] = system.__dict__[k].copy()
                 system.__dict__[k] = np.ndarray.view(
                     self.__dict__[k][..., start_idx:end_idx]
                 )
-            # synchronize the periodic node boundaries
-            _synchronize_periodic_boundary_of_vector_collection(
-                self.__dict__[k], self.periodic_boundary_elems_idx
-            )
+
+            # Synchronize periodic boundaries
+            synchronize_periodic_boundary(self.__dict__[k], periodic_boundary_idx)
```

### Comparing `pyelastica-0.3.1.post1/elastica/memory_block/memory_block_rod_base.py` & `pyelastica-0.3.2/elastica/memory_block/memory_block_rod_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 __doc__ = """Create block-structure class for collection of Cosserat rod systems."""
 import numpy as np
+from typing import Iterable
 
 
-def make_block_memory_metadata(n_elems_in_rods):
+def make_block_memory_metadata(n_elems_in_rods: np.ndarray) -> Iterable:
     """
-    This function, takes number of elements of each rod as an numpy array and computes,
+    This function, takes number of elements of each rod as a numpy array and computes,
     ghost nodes, elements and voronoi element indexes and numbers and returns it.
 
     Parameters
     ----------
-    n_elems_in_rods
+    n_elems_in_rods: ndarray
+        An integer array containing the number of elements in each of the n rod.
 
     Returns
     -------
-
+    n_elems_with_ghosts: int64
+        Total number of elements with ghost elements included. There are two ghost elements
+        between each pair of two rods adjacent in memory block.
+    ghost_nodes_idx: ndarray
+        An integer array of length n - 1 containing the indices of ghost nodes in memory block.
+    ghost_elements_idx: ndarray
+        An integer array of length 2 * (n - 1) containing the indices of ghost elements in memory block.
+    ghost_voronoi_idx: ndarray
+        An integer array of length 2 * (n - 1) containing the indices of ghost Voronoi nodes in memory block.
     """
-    n_nodes_in_rods = n_elems_in_rods + 1
-    n_voronois_in_rods = n_elems_in_rods - 1
 
+    n_nodes_in_rods = n_elems_in_rods + 1
     n_rods = n_elems_in_rods.shape[0]
 
     # Gap between two rods have one ghost node
     # n_nodes_with_ghosts = np.sum(n_nodes_in_rods) + (n_rods - 1)
     # Gap between two rods have two ghost elements : comes out to n_nodes_with_ghosts - 1
     n_elems_with_ghosts = np.sum(n_elems_in_rods) + 2 * (n_rods - 1)
     # Gap between two rods have three ghost voronois : comes out to n_nodes_with_ghosts - 2
     # n_voronoi_with_ghosts = np.sum(n_voronois_in_rods) + 3 * (n_rods - 1)
 
-    # To be nulled
-    ghost_nodes_idx = np.zeros(((n_rods - 1),), dtype=np.int64)
-    ghost_nodes_idx[:] = n_nodes_in_rods[:-1]
-    ghost_nodes_idx = np.cumsum(ghost_nodes_idx)
+    ghost_nodes_idx = np.cumsum(n_nodes_in_rods[:-1], dtype=np.int64)
     # Add [0, 1, 2, ... n_rods-2] to the ghost_nodes idx to accommodate miscounting
     ghost_nodes_idx += np.arange(0, n_rods - 1, dtype=np.int64)
 
     ghost_elems_idx = np.zeros((2 * (n_rods - 1),), dtype=np.int64)
-    ghost_elems_idx[::2] = n_elems_in_rods[:-1]
-    ghost_elems_idx[1::2] = 1
-    ghost_elems_idx = np.cumsum(ghost_elems_idx)
-    # Add [0, 0, 1, 1, 2, 2, ... n_rods-2, n_rods-2] to the ghost_elems idx to accommodate miscounting
-    ghost_elems_idx += np.repeat(np.arange(0, n_rods - 1, dtype=np.int64), 2)
+    ghost_elems_idx[::2] = ghost_nodes_idx - 1
+    ghost_elems_idx[1::2] = ghost_nodes_idx.copy()
 
     ghost_voronoi_idx = np.zeros((3 * (n_rods - 1),), dtype=np.int64)
-    ghost_voronoi_idx[::3] = n_voronois_in_rods[:-1]
-    ghost_voronoi_idx[1::3] = 1
-    ghost_voronoi_idx[2::3] = 1
-    ghost_voronoi_idx = np.cumsum(ghost_voronoi_idx)
-    # Add [0, 0, 0, 1, 1, 1, 2, 2, 2, ... n_rods-2, n_rods-2, n_rods-2] to the ghost_voronoi idx
-    # to accommodate miscounting
-    ghost_voronoi_idx += np.repeat(np.arange(0, n_rods - 1, dtype=np.int64), 3)
+    ghost_voronoi_idx[::3] = ghost_nodes_idx - 2
+    ghost_voronoi_idx[1::3] = ghost_nodes_idx - 1
+    ghost_voronoi_idx[2::3] = ghost_nodes_idx.copy()
 
     return n_elems_with_ghosts, ghost_nodes_idx, ghost_elems_idx, ghost_voronoi_idx
 
 
 def make_block_memory_periodic_boundary_metadata(n_elems_in_rods):
     """
     This function, takes the number of elements of ring rods and computes the periodic boundary node,
```

### Comparing `pyelastica-0.3.1.post1/elastica/modules/base_system.py` & `pyelastica-0.3.2/elastica/modules/base_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 from typing import Iterable, Callable, AnyStr
 
 from collections.abc import MutableSequence
 
 from elastica.rod import RodBase
 from elastica.rigidbody import RigidBodyBase
+from elastica.surface import SurfaceBase
 from elastica.modules.memory_block import construct_memory_block_structures
 from elastica._synchronize_periodic_boundary import _ConstrainPeriodicBoundaries
 
 
 class BaseSystemCollection(MutableSequence):
     """
     Base System for simulator classes. Every simulation class written by the user
@@ -50,15 +51,15 @@
         self._feature_group_callback: Iterable[
             Callable[[float, int, AnyStr], None]
         ] = []
         self._feature_group_finalize: Iterable[Callable] = []
         # We need to initialize our mixin classes
         super(BaseSystemCollection, self).__init__()
         # List of system types/bases that are allowed
-        self.allowed_sys_types = (RodBase, RigidBodyBase)
+        self.allowed_sys_types = (RodBase, RigidBodyBase, SurfaceBase)
         # List of systems to be integrated
         self._systems = []
         # Flag Finalize: Finalizing twice will cause an error,
         # but the error message is very misleading
         self._finalize_flag = False
 
     def _check_type(self, sys_to_be_added: AnyStr):
@@ -164,17 +165,28 @@
 
         # Clear the finalize feature group, just for the safety.
         self._feature_group_finalize.clear()
         self._feature_group_finalize = None
 
         # Toggle the finalize_flag
         self._finalize_flag = True
+        # sort _feature_group_synchronize so that _call_contacts is at the end
+        _call_contacts_index = []
+        for idx, feature in enumerate(self._feature_group_synchronize):
+            if feature.__name__ == "_call_contacts":
+                _call_contacts_index.append(idx)
+
+        # Move to the _call_contacts to the end of the _feature_group_synchronize list.
+        for index in _call_contacts_index:
+            self._feature_group_synchronize.append(
+                self._feature_group_synchronize.pop(index)
+            )
 
     def synchronize(self, time: float):
-        # Collection call _featuer_group_synchronize
+        # Collection call _feature_group_synchronize
         for feature in self._feature_group_synchronize:
             feature(time)
 
     def constrain_values(self, time: float):
         # Collection call _feature_group_constrain_values
         for feature in self._feature_group_constrain_values:
             feature(time)
```

### Comparing `pyelastica-0.3.1.post1/elastica/modules/callbacks.py` & `pyelastica-0.3.2/elastica/modules/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/modules/connections.py` & `pyelastica-0.3.2/elastica/modules/connections.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/modules/constraints.py` & `pyelastica-0.3.2/elastica/modules/constraints.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/modules/damping.py` & `pyelastica-0.3.2/elastica/modules/damping.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/modules/forcing.py` & `pyelastica-0.3.2/elastica/modules/forcing.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/modules/memory_block.py` & `pyelastica-0.3.2/elastica/modules/memory_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __doc__ = """
 This function is a module to construct memory blocks for different types of systems, such as
 Cosserat Rods, Rigid Body etc.
 """
 
 from elastica.rod import RodBase
 from elastica.rigidbody import RigidBodyBase
+from elastica.surface import SurfaceBase
 from elastica.memory_block import MemoryBlockCosseratRod, MemoryBlockRigidBody
 
 
 def construct_memory_block_structures(systems):
     """
     This function takes the systems (rod or rigid body) appended to the simulator class and
     separates them into lists depending on if system is Cosserat rod or rigid body. Then using
@@ -30,24 +31,29 @@
             temp_list_for_cosserat_rod_systems.append(sys_to_be_added)
             temp_list_for_cosserat_rod_systems_idx.append(system_idx)
 
         elif issubclass(sys_to_be_added.__class__, RigidBodyBase):
             temp_list_for_rigid_body_systems.append(sys_to_be_added)
             temp_list_for_rigid_body_systems_idx.append(system_idx)
 
+        elif issubclass(sys_to_be_added.__class__, SurfaceBase):
+            pass
+
         else:
             raise TypeError(
                 "{0}\n"
                 "is not a system passing validity\n"
                 "checks for constructing block structure. If you are sure that\n"
                 "{0}\n"
                 "satisfies all criteria for being a system, please add\n"
                 "it here with correct memory block implementation.\n"
                 "The allowed types are\n"
-                "{1} {2}".format(sys_to_be_added.__class__, RodBase, RigidBodyBase)
+                "{1} {2} {3}".format(
+                    sys_to_be_added.__class__, RodBase, RigidBodyBase, SurfaceBase
+                )
             )
 
     if temp_list_for_cosserat_rod_systems:
         _memory_blocks.append(
             MemoryBlockCosseratRod(
                 temp_list_for_cosserat_rod_systems,
                 temp_list_for_cosserat_rod_systems_idx,
```

### Comparing `pyelastica-0.3.1.post1/elastica/reset_functions_for_block_structure/_reset_ghost_vector_or_scalar.py` & `pyelastica-0.3.2/elastica/reset_functions_for_block_structure/_reset_ghost_vector_or_scalar.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/restart.py` & `pyelastica-0.3.2/elastica/restart.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rigidbody/cylinder.py` & `pyelastica-0.3.2/elastica/rigidbody/cylinder.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rigidbody/data_structures.py` & `pyelastica-0.3.2/elastica/rigidbody/data_structures.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rigidbody/rigid_body.py` & `pyelastica-0.3.2/elastica/rigidbody/rigid_body.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rigidbody/sphere.py` & `pyelastica-0.3.2/elastica/rigidbody/sphere.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rod/cosserat_rod.py` & `pyelastica-0.3.2/elastica/rod/cosserat_rod.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rod/data_structures.py` & `pyelastica-0.3.2/elastica/rod/data_structures.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rod/factory_function.py` & `pyelastica-0.3.2/elastica/rod/factory_function.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rod/knot_theory.py` & `pyelastica-0.3.2/elastica/rod/knot_theory.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/rod/rod_base.py` & `pyelastica-0.3.2/elastica/rod/rod_base.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/systems/__init__.py` & `pyelastica-0.3.2/elastica/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/systems/analytical.py` & `pyelastica-0.3.2/elastica/systems/analytical.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/timestepper/__init__.py` & `pyelastica-0.3.2/elastica/timestepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/timestepper/_stepper_interface.py` & `pyelastica-0.3.2/elastica/timestepper/_stepper_interface.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/timestepper/explicit_steppers.py` & `pyelastica-0.3.2/elastica/timestepper/explicit_steppers.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/timestepper/symplectic_steppers.py` & `pyelastica-0.3.2/elastica/timestepper/symplectic_steppers.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/transformations.py` & `pyelastica-0.3.2/elastica/transformations.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/utils.py` & `pyelastica-0.3.2/elastica/utils.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/elastica/wrappers.py` & `pyelastica-0.3.2/elastica/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyelastica-0.3.1.post1/pyproject.toml` & `pyelastica-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyelastica"
-version = "0.3.1.post1"
+version = "0.3.2"
 description = "Elastica is a software to simulate the dynamics of filaments that, at every cross-section, can undergo all six possible modes of deformation, allowing the filament to bend, twist, stretch and shear, while interacting with complex environments via muscular activity, surface contact, friction and hydrodynamics."
 readme = "README.md"
 authors = ["GazzolaLab <armant2@illinois.edu>"]
 license = "MIT"
 repository = "https://github.com/GazzolaLab/PyElastica"
 homepage = "https://www.cosseratrods.org/"
 documentation = "https://docs.cosseratrods.org/en/latest/"
 keywords = []
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
 # Trove classifiers
 # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
 "License :: OSI Approved :: MIT License",
-"Development Status :: 3 - Alpha",
+"Development Status :: 4 - Beta",
 "Programming Language :: Python",
 "Programming Language :: Python :: 3.8",
 "Programming Language :: Python :: 3.9",
 "Programming Language :: Python :: 3.10",
+"Programming Language :: Python :: 3.11",
 "Programming Language :: Python :: Implementation :: CPython",
 "Intended Audience :: Science/Research",
 "Intended Audience :: Education",
 ]
 
 # ...
 packages = [
     { include = "elastica" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-numba = "^0.55.0"
+python = ">=3.8,<3.12"
+numba = "^0.57.0"
 numpy = "^1.19.2"
 scipy = "^1.5.2"
 tqdm = "^4.61.1"
+matplotlib = "^3.3.2"
+pyvista = "^0.39.1"
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 Sphinx = {version = "^6.1", optional = true}
 sphinx-book-theme = {version = "^1.0", optional = true}
-readthedocs-sphinx-search = {version = "^0.1.1", optional = true}
+readthedocs-sphinx-search = {version = ">=0.1.1,<0.4.0", optional = true}
 sphinx-autodoc-typehints = {version = "^1.21", optional = true}
 myst-parser = {version = "^1.0", optional = true}
 numpydoc = {version = "^1.3.1", optional = true}
 docutils = {version = "^0.18", optional = true}
 cma = {version = "^3.2.2", optional = true}
-matplotlib = {version = "^3.3.2", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "21.12b0"
 pytest = "^7.1.1"
 coverage = "^6.3.3"
 pre-commit = "^2.19.0"
 pytest-html = "^3.1.1"
@@ -73,15 +75,14 @@
   "sphinx-autodoc-typehints",
   "myst-parser",
   "numpydoc",
   "docutils",
 ]
 examples = [
   "cma",
-  "matplotlib",
 ]
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `pyelastica-0.3.1.post1/PKG-INFO` & `pyelastica-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: pyelastica
-Version: 0.3.1.post1
+Version: 0.3.2
 Summary: Elastica is a software to simulate the dynamics of filaments that, at every cross-section, can undergo all six possible modes of deformation, allowing the filament to bend, twist, stretch and shear, while interacting with complex environments via muscular activity, surface contact, friction and hydrodynamics.
 Home-page: https://www.cosseratrods.org/
 License: MIT
 Author: GazzolaLab
 Author-email: armant2@illinois.edu
-Requires-Python: >=3.8,<3.11
-Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: docs
 Provides-Extra: examples
 Requires-Dist: Sphinx (>=6.1,<7.0) ; extra == "docs"
 Requires-Dist: cma (>=3.2.2,<4.0.0) ; extra == "examples"
 Requires-Dist: docutils (>=0.18,<0.19) ; extra == "docs"
-Requires-Dist: matplotlib (>=3.3.2,<4.0.0) ; extra == "examples"
+Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
 Requires-Dist: myst-parser (>=1.0,<2.0) ; extra == "docs"
-Requires-Dist: numba (>=0.55.0,<0.56.0)
+Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numpy (>=1.19.2,<2.0.0)
 Requires-Dist: numpydoc (>=1.3.1,<2.0.0) ; extra == "docs"
-Requires-Dist: readthedocs-sphinx-search (>=0.1.1,<0.2.0) ; extra == "docs"
+Requires-Dist: pyvista (>=0.39.1,<0.40.0)
+Requires-Dist: readthedocs-sphinx-search (>=0.1.1,<0.4.0) ; extra == "docs"
 Requires-Dist: scipy (>=1.5.2,<2.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.21,<2.0) ; extra == "docs"
 Requires-Dist: sphinx-book-theme (>=1.0,<2.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.61.1,<5.0.0)
 Project-URL: Documentation, https://docs.cosseratrods.org/en/latest/
 Project-URL: Repository, https://github.com/GazzolaLab/PyElastica
 Description-Content-Type: text/markdown
@@ -45,20 +44,20 @@
 [![Build_status][badge-travis]][link-travis] [![CI][badge-CI]][link-CI] [![Documentation Status][badge-docs-status]][link-docs-status] [![codecov][badge-codecov]][link-codecov] [![Downloads][badge-pepy-download-count]][link-pepy-download-count] [![DOI][badge-doi]][link-doi] [![Binder][badge-binder]][link-binder] [![Gitter][badge-gitter]][link-gitter]
  </div>
 
 PyElastica is the python implementation of **Elastica**: an *open-source* project for simulating assemblies of slender, one-dimensional structures using Cosserat Rod theory.
 
 [![gallery][link-readme-gallary]][link-project-website]
 
-Visit [cosseratrods.org][link-project-website] for more information and learn about Elastica and Cosserat rod theory.
+Visit [www.cosseratrods.org][link-project-website] for more information and learn about Elastica and Cosserat rod theory.
 
 ## How to Start
 [![PyPI version][badge-pypi]][link-pypi] [![Documentation Status][badge-docs-status]][link-docs-status]
 
-PyElastica is compatible with Python 3.8 - 3.10.
+PyElastica is compatible with Python 3.8 - 3.11.
 
 ~~~bash
 $ pip install pyelastica
 ~~~
 
 With this you get a minimal version with very little dependencies.
 
@@ -68,14 +67,19 @@
 - `docs`: packages to build documentation
 
 Options can be combined e.g.
 ```bash
 $ pip install "pyelastica[examples,docs]"
 ```
 
+For plotting videos, ffmpeg has to be installed:
+```bash
+$ conda install -c conda-forge ffmpeg
+```
+
 Documentation of PyElastica is available [here][link-docs-website].
 
 If you want to simulate magnetic Cosserat rods interacting with external magnetic environments you can install the derived package using
 
 ```bash
 $ pip install magneto_pyelastica
 ```
@@ -83,71 +87,76 @@
 Details can be found [here](https://github.com/armantekinalp/MagnetoPyElastica).
 
 ## Citation
 
 We ask that any publications which use Elastica cite as following:
 
 ```
-@software{arman_tekinalp_2023_7931429,
+@software{arman_tekinalp_2024_10883271,
   author       = {Arman Tekinalp and
                   Seung Hyun Kim and
                   Yashraj Bhosale and
                   Tejaswin Parthasarathy and
                   Noel Naughton and
-                  Ilia Nasiriziba and
+                  Ali Albazroun and
+                  Rahul Joon and
                   Songyuan Cui and
+                  Ilia Nasiriziba and
                   Maximilian Stölzle and
                   Chia-Hsien (Cathy) Shih and
-                  Mattia Gazzola
-                  },
-  title        = {GazzolaLab/PyElastica: v0.3.1},
-  month        = may,
-  year         = 2023,
+                  Mattia Gazzola},
+  title        = {GazzolaLab/PyElastica: v0.3.2},
+  month        = mar,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.3.1},
-  doi          = {10.5281/zenodo.7931429},
-  url          = {https://doi.org/10.5281/zenodo.7931429}
+  version      = {v0.3.2},
+  doi          = {10.5281/zenodo.10883271},
+  url          = {https://doi.org/10.5281/zenodo.10883271}
 }
 ```
 
 <details>
   <summary><h4>References</h4></summary>
 
 - Gazzola, Dudte, McCormick, Mahadevan, <strong>Forward and inverse problems in the mechanics of soft filaments</strong>, Royal Society Open Science, 2018. doi: [10.1098/rsos.171628](https://doi.org/10.1098/rsos.171628)
 - Zhang, Chan, Parthasarathy, Gazzola, <strong>Modeling and simulation of complex dynamic musculoskeletal architectures</strong>, Nature Communications, 2019. doi: [10.1038/s41467-019-12759-5](https://doi.org/10.1038/s41467-019-12759-5)
 
 </details>
 
 ## List of publications and submissions
+- [Soft, slender and active structures in fluids: embedding Cosserat rods in vortex methods](https://doi.org/10.48550/arXiv.2401.09506) (UIUC 2024)
+- [Neural models and algorithms for sensorimotor control of an octopus arm](https://doi.org/10.48550/arXiv.2402.01074)(UIUC 2024)
+- [On the mechanical origins of waving, coiling and skewing in Arabidopsis thaliana roots](https://www.pnas.org/doi/10.1073/pnas.2312761121) (Tel Aviv University, UIUC 2024) (PNAS)
 - [Topology, dynamics, and control of an octopus-analog muscular hydrostat](https://arxiv.org/abs/2304.08413) (UIUC, 2023)
-- [Hierarchical control and learning of a foraging CyberOctopus](https://arxiv.org/abs/2302.05811) (UIUC, 2023)
+- [Hierarchical control and learning of a foraging CyberOctopus](https://onlinelibrary.wiley.com/doi/full/10.1002/aisy.202300088) (UIUC, 2023) (Advanced Intelligent Systems)
 - [Energy-shaping control of a muscular octopus arm moving in three dimensions](https://royalsocietypublishing.org/doi/full/10.1098/rspa.2022.0593) (UIUC, 2023) (Proceedings of the Royal Society A 2023)
 - [A sensory feedback control law for octopus arm movements](https://ieeexplore.ieee.org/abstract/document/9993021/) (UIUC, 2022) (IEEE CDC 2022)
 - [Control-oriented modeling of bend propagation in an octopus arm](https://ieeexplore.ieee.org/abstract/document/9867689/) (UIUC, 2021) (IEEE ACC 2022)
 - [A physics-informed, vision-based method to reconstruct all deformation modes in slender bodies](https://arxiv.org/abs/2109.08372) (UIUC, 2021) (IEEE ICRA 2022) [code](https://github.com/GazzolaLab/BR2-vision-based-smoothing)
 - [Optimal control of a soft CyberOctopus arm](https://ieeexplore.ieee.org/document/9483284) (UIUC, 2021) (IEEE ACC 2021)
 - [Elastica: A compliant mechanics environment for soft robotic control](https://ieeexplore.ieee.org/document/9369003) (UIUC, 2021) (IEEE RA-L 2021)
 - [Controlling a CyberOctopus soft arm with muscle-like actuation](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9683318) (UIUC, 2020) (IEEE CDC 2021)
 - [Energy shaping control of a CyberOctopus soft arm](https://ieeexplore.ieee.org/document/9304408) (UIUC, 2020) (IEEE CDC 2020)
 
 ## Tutorials
 [![Binder][badge-binder-tutorial]][link-binder]
 
 We have created several Jupyter notebooks and Python scripts to help users get started with PyElastica. The Jupyter notebooks are available on Binder, allowing you to try out some of the tutorials without having to install PyElastica.
 
-We have also included an example script for visualizing PyElastica simulations using POVray. This script is located in the examples folder ([`examples/visualization`](examples/visualization)).
+We have also included an example script for visualizing PyElastica simulations using POVray. This script is located in the examples folder ([`examples/Visualization`](examples/Visualization)).
 
 ## Contribution
 
 If you would like to participate, please read our [contribution guideline](CONTRIBUTING.md)
 
-PyElastica is developed by the [Gazzola Lab][link-lab-website] at the University of Illinois at Urbana-Champaign.
+PyElastica is developed by the [Gazzola Lab][link-lab-website] at the University of Illinois Urbana-Champaign.
 
 ## Senior Developers ✨
 _Names arranged alphabetically_
+- Ali Albazroun
 - Arman Tekinalp
 - Chia-Hsien Shih (Cathy)
 - Fan Kiat Chan
 - Ilia Nasiriziba
 - Noel Naughton
 - [Seung Hyun Kim](https://github.com/skim0119)
 - Songyuan Cui
```

