# Comparing `tmp/scipion-em-cryosparc2-4.0.8.tar.gz` & `tmp/scipion-em-cryosparc2-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.0.8.tar", last modified: Wed Sep 13 08:38:20 2023, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.0.9.tar", last modified: Fri Nov 17 09:00:49 2023, max compression
```

## Comparing `scipion-em-cryosparc2-4.0.8.tar` & `scipion-em-cryosparc2-4.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.937466 scipion-em-cryosparc2-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.929465 scipion-em-cryosparc2-4.0.8/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    32591 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28291 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16128 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23486 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    24105 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    21348 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    24600 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23660 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    34464 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    38331 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    20773 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47395 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34624 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 08:38:20.933465 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-13 08:38:20.000000 scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 08:38:20.937466 scipion-em-cryosparc2-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2023-09-13 08:36:32.000000 scipion-em-cryosparc2-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.068780 scipion-em-cryosparc2-4.0.9/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32609 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.068780 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28554 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.072780 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16326 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24105 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23668 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34472 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38359 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.072780 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47395 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34894 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/setup.py
```

### Comparing `scipion-em-cryosparc2-4.0.8/LICENSE` & `scipion-em-cryosparc2-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/PKG-INFO` & `scipion-em-cryosparc2-4.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.8
+Version: 4.0.9
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,14 +34,19 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
+        **v4.0.9**
+        -----------
+        * **new**        Compatibility with cryoSPARC v4.4.0
+        * **fixed**      Handling aborted protocols/jobs
+        
         **v4.0.8**
         -----------
         * **new**        Compatibility with cryoSPARC v4.3.1
         * **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
         
         **v4.0.7**
         -----------
```

### Comparing `scipion-em-cryosparc2-4.0.8/README.rst` & `scipion-em-cryosparc2-4.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
 * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
 * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
 
 **Latest plugin version**
 ==========================
 
+**v4.0.9**
+-----------
+* **new**        Compatibility with cryoSPARC v4.4.0
+* **fixed**      Handling aborted protocols/jobs
+
 **v4.0.8**
 -----------
 * **new**        Compatibility with cryoSPARC v4.3.1
 * **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
 
 **v4.0.7**
 -----------
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.0.8'
+__version__ = '4.0.9'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
     _pathVars = [CRYOSPARC_HOME]
     _supportedVersions = [V3_0_0, V3_0_1, V3_1_0, V3_2_0, V3_3_0, V3_3_1,
                           V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
 
     @classmethod
     def _defineVariables(cls):
         cls._defineVar(CRYOSPARC_HOME, os.environ.get(CRYOSPARC_DIR, ""))
         cls._defineVar(CRYO_PROJECTS_DIR, "scipion_projects")
 
     @classmethod
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 V4_0_3 = 'V4.0.3'
 V4_1_0 = 'V4.1.0'
 V4_1_1 = 'V4.1.1'
 V4_1_2 = 'V4.1.2'
 V4_2_0 = 'V4.2.0'
 V4_2_1 = 'V4.2.1'
 V4_3_1 = 'V4.3.1'
+V4_4_0 = 'V4.4.0'
 
 # Symmetry dict
 CS_SYM_NAME = dict()
 CS_SYM_NAME[SYM_CYCLIC] = 'Cn'
 CS_SYM_NAME[SYM_DIHEDRAL_Y] = 'Dn'
 CS_SYM_NAME[SYM_TETRAHEDRAL] = 'T'
 CS_SYM_NAME[SYM_OCTAHEDRAL] = 'O'
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from collections import OrderedDict
+import  subprocess
 
 import emtable
 import numpy as np
 import os
 import argparse
 import sys
 import logging
@@ -48,17 +48,24 @@
 
 
 def convertCs2Star(argsList):
     input = os.path.abspath(argsList[0])
     output = os.path.abspath(argsList[1])
     cryosparcScriptPath = os.path.join(os.path.dirname(__file__),
                                        CRYOSPARC_CS2STAR_SCRIPT)
-    cmd = Plugin.getCondaActivationCmd() + Plugin.getPyemEnvActivation() + ' && python3 ' + cryosparcScriptPath + ' %s %s' % (
-    input, output)
-    os.system(cmd)
+    cmd = (Plugin.getCondaActivationCmd() + Plugin.getPyemEnvActivation() + ' && python3 ' +
+           cryosparcScriptPath + ' %s %s' % (input, output))
+
+    logger.info("convertCs2Star: %s" % cmd)
+
+    process = subprocess.Popen(cmd, shell=True, cwd=os.getcwd(), stdout=subprocess.PIPE,
+                               stderr=subprocess.PIPE)
+    out, error = process.communicate()
+    logger.info(out.decode())
+    logger.error(error.decode())
 
 
 def defineArgs():
     parser = argparse.ArgumentParser()
     parser.add_argument("input",
                         help="Cryosparc metadata .csv (v0.6.5) or .cs (v2+) files",
                         nargs="*")
@@ -154,15 +161,15 @@
 def particleToRow(part, partRow, **kwargs):
     """ Set labels values from Particle to md row. """
     coord = part.getCoordinate()
     if coord is not None:
         coordinateToRow(coord, partRow, copyId=False)
     if part.hasMicId():
         partRow.setValue(md.RLN_MICROGRAPH_ID, int(part.getMicId()))
-        # If the row does not contains the micrograph name
+        # If the row does not contain the micrograph name
         # use a fake micrograph name using id to relion
         # could at least group for CTF using that
         if not partRow.hasLabel(md.RLN_MICROGRAPH_NAME):
             partRow.setValue(md.RLN_MICROGRAPH_NAME,
                              'fake_micrograph_%06d.mrc' % part.getMicId())
     if part.hasAttribute('_rlnParticleId'):
         partRow.setValue(md.RLN_PARTICLE_ID, int(part._rlnParticleId.get()))
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/cs2Start.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 def cs2Star(args):
     from glob import glob
     import pandas as pd
     import numpy as np
     import logging
     from pyem import metadata
     from pyem import star
+    # see https://numpy.org/doc/stable/reference/generated/numpy.load.html
+    # for an explanation of MAX_HEADER_SIZE
+    MAX_HEADER_SIZE = 50000
 
     log = logging.getLogger('root')
     hdlr = logging.StreamHandler(sys.stdout)
     log.addHandler(hdlr)
-    log.setLevel(logging.getLevelName(args.loglevel.upper()))
+    log.setLevel(logging.getLevelName(logging.INFO))
 
     if args.swapxy:
         log.warning(
             "Axis swapping is now the default and --swapxy has no effect. "
             "Use --noswapxy if unswapping is needed (unlikely).")
 
     if args.input[0].endswith(".cs"):
         log.debug("Detected CryoSPARC 2+ .cs file")
-        cs = np.load(args.input[0])
+        cs = np.load(args.input[0], max_header_size=MAX_HEADER_SIZE)
         if args.first10k:
             cs = cs[:10000]
 
         if args.movies:
             if not os.path.isdir(args.output):
                 log.error("%s is not a directory" % args.output)
                 return 1
@@ -62,21 +65,22 @@
             if len(args.input) > 1 and args.input[-1].endswith(".star"):
                 mic_star = args.input[-1]
                 star.write_star(mic_star, data_general[
                     [f for f in fields if f in data_general]])
             return 0
 
         try:
+            log.info("Parsing .cs file...")
             df = metadata.parse_cryosparc_2_cs(cs, passthroughs=args.input[1:],
                                                minphic=args.minphic,
                                                boxsize=args.boxsize,
                                                swapxy=args.noswapxy,
                                                invertx=args.invertx,
                                                inverty=args.inverty)
-        except (KeyError, ValueError) as e:
+        except Exception as e:
             log.error(e, exc_info=True)
             log.error("Required fields could not be mapped. Are you using the "
                       "right input file(s)?")
             return 1
     else:
         log.debug("Detected CryoSPARC 0.6.5 .csv file")
         if len(args.input) > 1:
@@ -209,12 +213,13 @@
                         help="Only read first 10,000 particles for rapid testing.",
                         action="store_true",
                         dest="first10k")
     parser.add_argument("--loglevel", "-l", type=str, default="WARNING",
                         help="Logging level and debug output")
     return parser
 
+
 if __name__ == "__main__":
     parser = defineArgs()
     argsList = [sys.argv[1], sys.argv[2]]
     args = parser.parse_args(argsList)
-    sys.exit(cs2Star(args))
+    sys.exit(cs2Star(args))
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.0.9/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import os
 import ast
 import requests
+import logging
+logger = logging.getLogger(__name__)
+
 from pkg_resources import parse_version
 
 import pwem.protocols as pw
 import pyworkflow.object as pwobj
 import pyworkflow.utils as pwutils
 from pwem.objects import FSC
 
@@ -247,18 +250,23 @@
         self.particles = pwobj.String(str(importedParticlesJob.get()) +
                                       '.imported_particles')
 
     def setAborted(self):
         """ Set the status to aborted and updated the endTime. """
         pw.EMProtocol.setAborted(self)
         if hasattr(self, 'projectName') and hasattr(self, 'currenJob') and self.currenJob.get() is not None:
-            status = getJobStatus(self.projectName.get(), self.currenJob.get())
+            job = str(self.currenJob.get())
+            project = str(self.projectName.get())
+            status = getJobStatus(project, job)
             if status not in STOP_STATUSES:
-                killJob(str(self.projectName.get()), str(self.currenJob.get()))
-                clearJob(str(self.projectName.get()), str(self.currenJob.get()))
+                try:
+                    killJob(project, job)
+                    clearJob(project, job)
+                except Exception as e:
+                    logger.error("Can't kill job %s from project %s" % (job, project), exc_info=e)
 
     def createFSC(self, idd, imgSet, vol):
         # Need to get the cryosparc master address
         system_info = getSystemInfo()
         status_errors = system_info[0]
 
         if not status_errors:
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     """
     Prepares particles for use in 3DFlex training and reconstruction. At the same
     way,  Takes in a consensus (rigid) refinement density map, plus optionally
      a segmentation and generates a tetrahedral mesh for 3DFlex.
     """
     _label = '3D flex data/mesh prepare'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1,
+                          V4_4_0]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     particles and performs high-resolution refinement using L-BFGS under
     the 3DFlex model. This is the stage at which improvements to density
     in high-res regions are computed. Outputs two half-maps that can be used
     for FSC validation, sharpening, and other downstream tasks.
     """
     _label = '3D flex reconstruction'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Uses a mesh and prepared particles (at a downsampled resolution) to train
     a 3DFlex model. Parameters control the number of latent dimensions,
     size of the model, and training hyperparameters. This job outputs
     checkpoints during training.
     """
     _label = '3D flex training'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Wrapper protocol for the Cryosparc's per-particle Global CTF refinement.
     Performs per-exposure-group CTF parameter refinement of higher-order
     aberrations, against a given 3D reference
     """
     _label = 'global ctf refinement'
     _className = "ctf_refine_global"
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
     newParamsName = []
 
     def _initialize(self):
         self._createFilenameTemplates()
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     alignment algorithm, and optional Non-Uniform regularization as used in
     other cryoSPARC refinement jobs.
     """
     _label = '3D helical refinement'
     _devStatus = BETA
     _fscColumns = 4
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
     _className = "helix_refine"
 
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputParticles', PointerParam,
                       pointerClass='SetOfParticles',
                       label="Input particles", important=True,
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     _label = 'homogeneous reconstruction'
     _className = "homo_reconstruct"
     _devStatus = NEW
     _fscColumns = 6
     _protCompatibility = [V3_3_0, V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2,
                           V4_0_3, V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1,
-                          V4_3_1]
+                          V4_3_1, V4_4_0]
     ewsParamsName = []
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         the fly.
     """
     _label = '3D homogeneous refinement'
     _fscColumns = 6
     _className = "homo_refine_new"
     ewsParamsName = []
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     classification routine that can complement the existing Heterogeneous
     Refinement job in finding new discrete classes of data.
     """
     _label = '3D Classification'
     _className = "class_3D"
     _devStatus = BETA
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
         myDict = {
@@ -323,19 +323,18 @@
         """
         self._initializeUtilsVariables()
         self.info(pwutils.yellowStr("Creating the output..."))
 
         csOutputFolder = os.path.join(self.projectDir.get(),
                                       self.run3dClassification.get())
         itera = self.findLastIteration(self.run3dClassification.get())
-
-        csParticlesName = "%s%s_00%s_particles.cs" % (
+        csParticlesName = "%s%s_%s_particles.cs" % (
                                                  getOutputPreffix(self.projectName.get()),
                                                  self.run3dClassification.get(),
-                                                 itera)
+                                                 itera.zfill(5))
         csPassParticles = "%s_passthrough_particles_all_classes.cs" % self.run3dClassification.get()
 
         # Copy the CS output particles to extra folder
         copyFiles(csOutputFolder, self._getExtraPath(), files=[csParticlesName,
                                                                csPassParticles])
 
         csFile = os.path.join(self._getExtraPath(), csParticlesName)
@@ -435,24 +434,24 @@
             output_file.write('\n\n')
             output_file.write('loop_')
             output_file.write('\n')
             output_file.write('_rlnReferenceImage')
             output_file.write('\n')
             numOfClass = self.class3D_N_K.get()
             for i in range(numOfClass):
-                csVolName = ("%s%s_class_%02d_00%s_volume.mrc" %
+                csVolName = ("%s%s_class_%02d_%s_volume.mrc" %
                              (getOutputPreffix(self.projectName.get()),
-                              self.run3dClassification.get(), i, itera))
+                              self.run3dClassification.get(), i, itera.zfill(5)))
 
                 copyFiles(csOutputFolder, self._getExtraPath(),
                           files=[csVolName])
 
-                row = ("%s/%s%s_class_%02d_00%s_volume.mrc\n" %
+                row = ("%s/%s%s_class_%02d_%s_volume.mrc\n" %
                        (self._getExtraPath(), getOutputPreffix(self.projectName.get()),
-                        self.run3dClassification.get(), i, itera))
+                        self.run3dClassification.get(), i, itera.zfill(5)))
                 output_file.write(row)
 
     def findLastIteration(self, jobName):
         import ast
         get_job_streamlog(self.projectName.get(),
                           jobName,
                           self._getFileName('stream_log'))
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class ProtCryoSparcLocalRefine(ProtCryosparcBase, ProtOperateParticles):
     """ Signal subtraction protocol of cryoSPARC.
         Subtract projections of a masked volume from particles.
         """
     _label = 'local refinement'
     _devStatus = NEW
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0,  V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
     _className = "new_local_refine"
     _fscColumns = 6
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,19 +591,24 @@
     :parameter jobId: cryosparc job id
     :parameter failureMessage: Message for the exception thrown in case job fails
     :returns job Status
     :raises Exception when parsing cryosparc's output looks wrong"""
 
     # While is needed here, cause waitJob has a timeout of 5 secs.
     while True:
-        status = getJobStatus(projectName, jobId)
-        if status not in STOP_STATUSES:
-            waitJob(projectName, jobId)
-        else:
-            break
+        try:
+            status = getJobStatus(projectName, jobId)
+            if status not in STOP_STATUSES:
+                waitJob(projectName, jobId)
+            else:
+                break
+        except Exception as e:
+            logger.error("Can't query cryoSPARC about the job %s. Maybe it needs a restart ? We'll wait 5 minutes" % jobId, exc_info=e)
+            import time
+            time.sleep(300)  # wait 5 minutes
 
     if status != STATUS_COMPLETED:
         raise Exception(failureMessage)
 
     return status
```

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.0.9/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.8
+Version: 4.0.9
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,14 +34,19 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
+        **v4.0.9**
+        -----------
+        * **new**        Compatibility with cryoSPARC v4.4.0
+        * **fixed**      Handling aborted protocols/jobs
+        
         **v4.0.8**
         -----------
         * **new**        Compatibility with cryoSPARC v4.3.1
         * **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
         
         **v4.0.7**
         -----------
```

### Comparing `scipion-em-cryosparc2-4.0.8/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.8/setup.py` & `scipion-em-cryosparc2-4.0.9/setup.py`

 * *Files identical despite different names*

