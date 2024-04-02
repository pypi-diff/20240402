# Comparing `tmp/macapype-0.3.dev2.tar.gz` & `tmp/macapype-0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macapype/macapype/dist/tmpx5dq_wxx/macapype-0.3.dev2.tar", last modified: Wed Nov 10 15:29:04 2021, max compression
+gzip compressed data, was "/home/runner/work/macapype/macapype/dist/tmp8mj5qg1_/macapype-0.3.dev3.tar", last modified: Thu Nov 18 12:31:59 2021, max compression
```

## Comparing `macapype-0.3.dev2.tar` & `macapype-0.3.dev3.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (116)       86 2021-11-10 15:28:53.000000 macapype-0.3.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      194 2021-11-10 15:29:04.000000 macapype-0.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1171 2021-11-10 15:28:53.000000 macapype-0.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9957 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/plot_segment_baboon_ants_based.py
--rw-r--r--   0 runner    (1001) docker     (116)     7216 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/plot_segment_macaque_ants_based.py
--rw-r--r--   0 runner    (1001) docker     (116)     5989 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/plot_segment_macaque_spm_based.py
--rw-r--r--   0 runner    (1001) docker     (116)     8434 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/plot_segment_marmo_ants_based.py
--rw-r--r--   0 runner    (1001) docker     (116)     3043 2021-11-10 15:28:53.000000 macapype-0.3.dev2/examples/plot_segment_sphinx_macaque_ants_based.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype/
--rw-r--r--   0 runner    (1001) docker     (116)      254 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype/bash/
--rw-r--r--   0 runner    (1001) docker     (116)     5359 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/CropVolume.sh
--rw-r--r--   0 runner    (1001) docker     (116)     9777 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/IterREGBET.sh
--rw-r--r--   0 runner    (1001) docker     (116)    13742 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/NMT_subject_align
--rw-r--r--   0 runner    (1001) docker     (116)    10200 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/NMT_subject_align.csh
--rw-r--r--   0 runner    (1001) docker     (116)    10918 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/T1xT2BET.sh
--rw-r--r--   0 runner    (1001) docker     (116)     9223 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/T1xT2BiasFieldCorrection.sh
--rw-r--r--   0 runner    (1001) docker     (116)    50040 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/bash/atlasBREX.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype/nodes/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7722 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/correct_bias.py
--rw-r--r--   0 runner    (1001) docker     (116)    12691 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/extract_brain.py
--rw-r--r--   0 runner    (1001) docker     (116)     8902 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/prepare.py
--rw-r--r--   0 runner    (1001) docker     (116)    20481 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/register.py
--rw-r--r--   0 runner    (1001) docker     (116)    10618 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/segment.py
--rw-r--r--   0 runner    (1001) docker     (116)     4087 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/nodes/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype/pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16046 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/correct_bias.py
--rw-r--r--   0 runner    (1001) docker     (116)     6231 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/extract_brain.py
--rw-r--r--   0 runner    (1001) docker     (116)    55375 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/full_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (116)    40918 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/prepare.py
--rw-r--r--   0 runner    (1001) docker     (116)    19311 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/register.py
--rw-r--r--   0 runner    (1001) docker     (116)    22024 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/segment.py
--rw-r--r--   0 runner    (1001) docker     (116)    23208 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/pipelines/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1496 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/data_test_servers.json
--rw-r--r--   0 runner    (1001) docker     (116)     2193 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/regex_subs.json
--rw-r--r--   0 runner    (1001) docker     (116)      634 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/subs.json
--rw-r--r--   0 runner    (1001) docker     (116)     4601 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/templates.json
--rw-r--r--   0 runner    (1001) docker     (116)     3770 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/utils_bids.py
--rw-r--r--   0 runner    (1001) docker     (116)     5496 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/utils_nodes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1388 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/utils_spm.py
--rw-r--r--   0 runner    (1001) docker     (116)     3714 2021-11-10 15:28:53.000000 macapype-0.3.dev2/macapype/utils/utils_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      194 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2389 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       28 2021-11-10 15:29:04.000000 macapype-0.3.dev2/macapype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-11-10 15:29:04.000000 macapype-0.3.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2021-11-10 15:28:53.000000 macapype-0.3.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-10 15:29:04.000000 macapype-0.3.dev2/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3194 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_baboon_ants.json
--rw-r--r--   0 runner    (1001) docker     (116)     1715 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_baboon_ants_t1.json
--rw-r--r--   0 runner    (1001) docker     (116)     3233 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_baboon_ants_t1t2debias.json
--rw-r--r--   0 runner    (1001) docker     (116)     1612 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_chimp_ants_t1.json
--rw-r--r--   0 runner    (1001) docker     (116)     2034 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants.json
--rw-r--r--   0 runner    (1001) docker     (116)     1997 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants_segkmeans.json
--rw-r--r--   0 runner    (1001) docker     (116)     1330 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants_t1.json
--rw-r--r--   0 runner    (1001) docker     (116)     1389 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants_t1_template.json
--rw-r--r--   0 runner    (1001) docker     (116)     2104 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants_t1t2debias.json
--rw-r--r--   0 runner    (1001) docker     (116)     2287 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_ants_template.json
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_spm.json
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_spm_native.json
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_macaque_spm_t1_native.json
--rwxr-xr-x   0 runner    (1001) docker     (116)     2750 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_marmo_ants.json
--rwxr-xr-x   0 runner    (1001) docker     (116)     2212 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_marmo_ants_t1.json
--rw-r--r--   0 runner    (1001) docker     (116)     2530 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/params_segment_marmo_ants_t1t2debias.json
--rw-r--r--   0 runner    (1001) docker     (116)     6507 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/segment_from_mask_pnh_ants_based.py
--rw-r--r--   0 runner    (1001) docker     (116)    15197 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/segment_pnh.py
--rw-r--r--   0 runner    (1001) docker     (116)    10171 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/segment_pnh_regis.py
--rw-r--r--   0 runner    (1001) docker     (116)      106 2021-11-10 15:28:53.000000 macapype-0.3.dev2/workflows/which_spm.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2021-11-18 12:31:50.000000 macapype-0.3.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2021-11-18 12:31:59.000000 macapype-0.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1171 2021-11-18 12:31:50.000000 macapype-0.3.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9957 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/plot_segment_baboon_ants_based.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7216 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/plot_segment_macaque_ants_based.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5989 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/plot_segment_macaque_spm_based.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8434 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/plot_segment_marmo_ants_based.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3043 2021-11-18 12:31:50.000000 macapype-0.3.dev3/examples/plot_segment_sphinx_macaque_ants_based.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype/
+-rw-r--r--   0 runner    (1001) docker     (116)      254 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype/bash/
+-rw-r--r--   0 runner    (1001) docker     (116)     5359 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/CropVolume.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     9777 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/IterREGBET.sh
+-rw-r--r--   0 runner    (1001) docker     (116)    13742 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/NMT_subject_align
+-rw-r--r--   0 runner    (1001) docker     (116)    10200 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/NMT_subject_align.csh
+-rw-r--r--   0 runner    (1001) docker     (116)    10918 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/T1xT2BET.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     9223 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/T1xT2BiasFieldCorrection.sh
+-rw-r--r--   0 runner    (1001) docker     (116)    50040 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/bash/atlasBREX.sh
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype/nodes/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7722 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/correct_bias.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12691 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/extract_brain.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8902 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20481 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/register.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10618 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/segment.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4087 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/nodes/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16046 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/correct_bias.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6231 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/extract_brain.py
+-rw-r--r--   0 runner    (1001) docker     (116)    55442 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/full_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40742 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19320 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/register.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22024 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/segment.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23208 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/pipelines/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1496 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/data_test_servers.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2149 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/regex_subs.json
+-rw-r--r--   0 runner    (1001) docker     (116)      634 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/subs.json
+-rw-r--r--   0 runner    (1001) docker     (116)     4601 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/templates.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3770 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/utils_bids.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5496 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/utils_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1388 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/utils_spm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3714 2021-11-18 12:31:50.000000 macapype-0.3.dev3/macapype/utils/utils_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2177 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2021-11-18 12:31:59.000000 macapype-0.3.dev3/macapype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-11-18 12:31:59.000000 macapype-0.3.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1003 2021-11-18 12:31:50.000000 macapype-0.3.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:59.000000 macapype-0.3.dev3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2360 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_baboon_ants.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1749 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_baboon_ants_t1.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1647 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_chimp_ants_t1.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2035 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_ants.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1365 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_ants_t1.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_ants_t1_template.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2294 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_ants_template.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1097 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_spm.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_spm_native.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_macaque_spm_t1_native.json
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2751 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_marmo_ants.json
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2213 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/params_segment_marmo_ants_t1.json
+-rw-r--r--   0 runner    (1001) docker     (116)     6507 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/segment_from_mask_pnh_ants_based.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19897 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/segment_pnh.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10171 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/segment_pnh_regis.py
+-rw-r--r--   0 runner    (1001) docker     (116)      106 2021-11-18 12:31:50.000000 macapype-0.3.dev3/workflows/which_spm.py
```

### Comparing `macapype-0.3.dev2/README.md` & `macapype-0.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/examples/plot_segment_baboon_ants_based.py` & `macapype-0.3.dev3/examples/plot_segment_baboon_ants_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/examples/plot_segment_macaque_ants_based.py` & `macapype-0.3.dev3/examples/plot_segment_macaque_ants_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/examples/plot_segment_macaque_spm_based.py` & `macapype-0.3.dev3/examples/plot_segment_macaque_spm_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/examples/plot_segment_marmo_ants_based.py` & `macapype-0.3.dev3/examples/plot_segment_marmo_ants_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/examples/plot_segment_sphinx_macaque_ants_based.py` & `macapype-0.3.dev3/examples/plot_segment_sphinx_macaque_ants_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/CropVolume.sh` & `macapype-0.3.dev3/macapype/bash/CropVolume.sh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/IterREGBET.sh` & `macapype-0.3.dev3/macapype/bash/IterREGBET.sh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/NMT_subject_align` & `macapype-0.3.dev3/macapype/bash/NMT_subject_align`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/NMT_subject_align.csh` & `macapype-0.3.dev3/macapype/bash/NMT_subject_align.csh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/T1xT2BET.sh` & `macapype-0.3.dev3/macapype/bash/T1xT2BET.sh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/T1xT2BiasFieldCorrection.sh` & `macapype-0.3.dev3/macapype/bash/T1xT2BiasFieldCorrection.sh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/bash/atlasBREX.sh` & `macapype-0.3.dev3/macapype/bash/atlasBREX.sh`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/correct_bias.py` & `macapype-0.3.dev3/macapype/nodes/correct_bias.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/extract_brain.py` & `macapype-0.3.dev3/macapype/nodes/extract_brain.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/prepare.py` & `macapype-0.3.dev3/macapype/nodes/prepare.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/register.py` & `macapype-0.3.dev3/macapype/nodes/register.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/segment.py` & `macapype-0.3.dev3/macapype/nodes/segment.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/nodes/surface.py` & `macapype-0.3.dev3/macapype/nodes/surface.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/pipelines/correct_bias.py` & `macapype-0.3.dev3/macapype/pipelines/correct_bias.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/pipelines/extract_brain.py` & `macapype-0.3.dev3/macapype/pipelines/extract_brain.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/pipelines/full_pipelines.py` & `macapype-0.3.dev3/macapype/pipelines/full_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                        create_reg_seg_pipe)
 
 from .extract_brain import (create_extract_pipe,
                             create_extract_T1_pipe)
 
 from .surface import create_nii_to_mesh_pipe, create_nii_to_mesh_fs_pipe
 
-from macapype.utils.misc import parse_key, list_input_files
+from macapype.utils.misc import parse_key, list_input_files, show_files
 
 
 ###############################################################################
 # SPM based segmentation (from: Régis Trapeau)
 # -soft SPM or SPM_T1
 ###############################################################################
 def create_full_spm_subpipes(
@@ -198,33 +198,33 @@
                          native_iter_reg_pipe, 'inputnode.t1_debiased_file')
 
         seg_pipe.connect(inputnode, 'indiv_params',
                          native_iter_reg_pipe, 'inputnode.indiv_params')
 
         # Compute brain mask using old_segment of SPM and postprocessing on
         # tissues' masks
-        if "old_segment_pipe" in params.keys():
+        if "native_old_segment_pipe" in params.keys():
 
             old_segment_pipe = create_native_old_segment_pipe(
                 params_template,
-                params=parse_key(params, "old_segment_pipe"))
+                params=parse_key(params, "native_old_segment_pipe"))
 
             seg_pipe.connect(debias, 't1_debiased_file',
                              old_segment_pipe, 'inputnode.T1')
 
             seg_pipe.connect(native_iter_reg_pipe,
-                             'register_csf_to_nat.out_file',
+                             ('register_csf_to_nat.out_file', show_files),
                              old_segment_pipe, 'inputnode.native_csf')
 
             seg_pipe.connect(native_iter_reg_pipe,
-                             'register_wm_to_nat.out_file',
+                             ('register_wm_to_nat.out_file', show_files),
                              old_segment_pipe, 'inputnode.native_wm')
 
             seg_pipe.connect(native_iter_reg_pipe,
-                             'register_gm_to_nat.out_file',
+                             ('register_gm_to_nat.out_file',show_files),
                              old_segment_pipe, 'inputnode.native_gm')
 
             seg_pipe.connect(inputnode, 'indiv_params',
                              old_segment_pipe, 'inputnode.indiv_params')
 
         else:
             return seg_pipe
```

### Comparing `macapype-0.3.dev2/macapype/pipelines/prepare.py` & `macapype-0.3.dev3/macapype/pipelines/prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,23 +485,18 @@
         data_preparation_pipe.connect(align_T2_on_T1, "out_file",
                                       crop_T2, 'in_file')
     else:
 
         # Brain extraction (unused) + Automated Cropping
         # default, if crop_T1 is undefined
 
-        if "bet_crop" not in params.keys():
+        if "bet_crop" in params.keys():
 
-            params["bet_crop"] = {"m": True, "aT2": True, "c": 10, "n": 2}
-
-            print("Using default bet_crop parameters: {}".format(
-                params["bet_crop"]))
-
-        bet_crop = NodeParams(T1xT2BET(), params=params["bet_crop"],
-                              name='bet_crop')
+            bet_crop = NodeParams(T1xT2BET(), params=params["bet_crop"],
+                                  name='bet_crop')
 
         if "reorient" in params.keys():
 
             data_preparation_pipe.connect(reorient_T1_pipe,
                                           'reorient.out_file',
                                           bet_crop, 't1_file')
             data_preparation_pipe.connect(reorient_T2_pipe,
```

### Comparing `macapype-0.3.dev2/macapype/pipelines/register.py` & `macapype-0.3.dev3/macapype/pipelines/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,35 +209,35 @@
         inputnode, ('indiv_params', parse_key, "reg"),
         reg, 'indiv_params')
 
     # apply inv_transfo over the 3 tissues:
     # gm
     register_gm_to_nat = pe.Node(fsl.ApplyXFM(), name="register_gm_to_nat")
     register_gm_to_nat.inputs.in_file = params_template["template_gm"]
-    register_gm_to_nat.inputs.output_type = "NIFTI"  # for SPM segment
+    register_gm_to_nat.inputs.output_type = "NIFTI_GZ"  # for SPM segment
 
     native_iter_reg_pipe.connect(inputnode, 't1_debiased_file',
                                  register_gm_to_nat, 'reference')
     native_iter_reg_pipe.connect(reg, 'inv_transfo_file',
                                  register_gm_to_nat, "in_matrix_file")
 
     # wm
     register_wm_to_nat = pe.Node(fsl.ApplyXFM(), name="register_wm_to_nat")
     register_wm_to_nat.inputs.in_file = params_template["template_wm"]
-    register_wm_to_nat.inputs.output_type = "NIFTI"  # for SPM segment
+    register_wm_to_nat.inputs.output_type = "NIFTI_GZ"  # for SPM segment
 
     native_iter_reg_pipe.connect(inputnode, 't1_debiased_file',
                                  register_wm_to_nat, 'reference')
     native_iter_reg_pipe.connect(reg, 'inv_transfo_file',
                                  register_wm_to_nat, "in_matrix_file")
 
     # csf
     register_csf_to_nat = pe.Node(fsl.ApplyXFM(), name="register_csf_to_nat")
     register_csf_to_nat.inputs.in_file = params_template["template_csf"]
-    register_csf_to_nat.inputs.output_type = "NIFTI"  # for SPM segment
+    register_csf_to_nat.inputs.output_type = "NIFTI_GZ"  # for SPM segment
 
     native_iter_reg_pipe.connect(inputnode, 't1_debiased_file',
                                  register_csf_to_nat, 'reference')
     native_iter_reg_pipe.connect(reg, 'inv_transfo_file',
                                  register_csf_to_nat, "in_matrix_file")
 
     return native_iter_reg_pipe
```

### Comparing `macapype-0.3.dev2/macapype/pipelines/segment.py` & `macapype-0.3.dev3/macapype/pipelines/segment.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/pipelines/surface.py` & `macapype-0.3.dev3/macapype/pipelines/surface.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/data_test_servers.json` & `macapype-0.3.dev3/macapype/utils/data_test_servers.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/misc.py` & `macapype-0.3.dev3/macapype/utils/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,16 +57,14 @@
     shutil.copy(zipped_file, dest)
 
     if zipped_file[-3:] == ".gz":
         subprocess.check_output("gunzip " + dest, shell=True)
     else:
         ValueError("Non GZip file given")
 
-    print(os.listdir(os.path.abspath("")))
-
     unzipped_file = dest[:-3]
     return unzipped_file
 
 
 def merge_3_elem_to_list(elem1, elem2, elem3):
     return [elem1, elem2, elem3]
```

### Comparing `macapype-0.3.dev2/macapype/utils/subs.json` & `macapype-0.3.dev3/macapype/utils/subs.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/templates.json` & `macapype-0.3.dev3/macapype/utils/templates.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/utils_bids.py` & `macapype-0.3.dev3/macapype/utils/utils_bids.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/utils_nodes.py` & `macapype-0.3.dev3/macapype/utils/utils_nodes.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/utils_spm.py` & `macapype-0.3.dev3/macapype/utils/utils_spm.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype/utils/utils_tests.py` & `macapype-0.3.dev3/macapype/utils/utils_tests.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/macapype.egg-info/SOURCES.txt` & `macapype-0.3.dev3/macapype.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -46,25 +46,21 @@
 macapype/utils/utils_bids.py
 macapype/utils/utils_nodes.py
 macapype/utils/utils_spm.py
 macapype/utils/utils_tests.py
 workflows/__init__.py
 workflows/params_segment_baboon_ants.json
 workflows/params_segment_baboon_ants_t1.json
-workflows/params_segment_baboon_ants_t1t2debias.json
 workflows/params_segment_chimp_ants_t1.json
 workflows/params_segment_macaque_ants.json
-workflows/params_segment_macaque_ants_segkmeans.json
 workflows/params_segment_macaque_ants_t1.json
 workflows/params_segment_macaque_ants_t1_template.json
-workflows/params_segment_macaque_ants_t1t2debias.json
 workflows/params_segment_macaque_ants_template.json
 workflows/params_segment_macaque_spm.json
 workflows/params_segment_macaque_spm_native.json
 workflows/params_segment_macaque_spm_t1_native.json
 workflows/params_segment_marmo_ants.json
 workflows/params_segment_marmo_ants_t1.json
-workflows/params_segment_marmo_ants_t1t2debias.json
 workflows/segment_from_mask_pnh_ants_based.py
 workflows/segment_pnh.py
 workflows/segment_pnh_regis.py
 workflows/which_spm.py
```

### Comparing `macapype-0.3.dev2/setup.py` & `macapype-0.3.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/workflows/params_segment_baboon_ants.json` & `macapype-0.3.dev3/workflows/params_segment_marmo_ants.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4499421296296296%*

 * *Differences: {"'brain_extraction_pipe'": "{'extract_pipe': {'atlas_brex': {'f': 0.6, 'reg': 1, 'wrp': "*

 * *                            "'10,10,10', 'dil': 4, 'args': '-vox 1'}}}",*

 * * "'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}",*

 * * "'general'": "{'template_name': 'MBM_v3.0.1'}",*

 * * "'mask_from_seg_pipe'": "OrderedDict([('dilate_mask', OrderedDict([('kernel_shape', 'sphere'), "*

 * *                         "('kernel_size', 2)])), ('erode_mask', OrderedDict([('kernel_shape', "*

 * *                         "'sph […]*

```diff
@@ -11,18 +11,20 @@
                 40,
                 30
             ],
             "shrink_factor": 2
         },
         "extract_pipe": {
             "atlas_brex": {
-                "f": 0.5,
+                "args": "-vox 1",
+                "dil": 4,
+                "f": 0.6,
                 "msk": "a,0,0",
-                "reg": 2,
-                "wrp": "1"
+                "reg": 1,
+                "wrp": "10,10,10"
             }
         }
     },
     "brain_segment_pipe": {
         "masked_correct_bias_pipe": {
             "norm_smooth": {
                 "op_string": "-s 2 -div %s"
@@ -34,15 +36,15 @@
                 "sigma": 2
             }
         },
         "register_NMT_pipe": {
             "NMT_subject_align": {
                 "afni_ext": "orig"
             },
-            "NMT_version": "1.3",
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
@@ -67,58 +69,41 @@
             "threshold_wm": {
                 "thresh": 0.5
             },
             "use_priors": 0.0
         }
     },
     "general": {
-        "template_name": "haiko89_template"
+        "template_name": "MBM_v3.0.1"
     },
-    "long_single_preparation_pipe": {
-        "align_T2_on_T1": {
-            "cost": "normmi",
-            "dof": 6
-        },
-        "prep_T1": {
-            "crop_T1": {
-                "args": "should be defined in indiv"
-            },
-            "denoise": {
-                "shrink_factor": 1
-            },
-            "norm_intensity": {
-                "args": "-r 0 --verbose 1",
-                "bspline_fitting_distance": 200,
-                "convergence_threshold": 1e-08,
-                "dimension": 3,
-                "n_iterations": [
-                    50,
-                    50,
-                    40,
-                    30
-                ],
-                "shrink_factor": 2
-            }
+    "mask_from_seg_pipe": {
+        "dilate_mask": {
+            "kernel_shape": "sphere",
+            "kernel_size": 2
         },
-        "prep_T2": {
-            "crop_T2": {
-                "args": "should be defined in indiv"
-            },
-            "denoise": {
-                "shrink_factor": 1
-            },
-            "norm_intensity": {
-                "args": "-r 0 --verbose 1",
-                "bspline_fitting_distance": 200,
-                "convergence_threshold": 1e-08,
-                "dimension": 3,
-                "n_iterations": [
-                    50,
-                    50,
-                    40,
-                    30
-                ],
-                "shrink_factor": 2
-            }
+        "erode_mask": {
+            "kernel_shape": "sphere",
+            "kernel_size": 2
+        }
+    },
+    "short_preparation_pipe": {
+        "crop_T1": {
+            "args": "should be defined in indiv"
+        },
+        "denoise": {
+            "shrink_factor": 1
+        },
+        "norm_intensity": {
+            "args": "-r 0 --verbose 1",
+            "bspline_fitting_distance": 200,
+            "convergence_threshold": 1e-08,
+            "dimension": 3,
+            "n_iterations": [
+                50,
+                50,
+                40,
+                30
+            ],
+            "shrink_factor": 2
         }
     }
 }
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_baboon_ants_t1.json` & `macapype-0.3.dev3/workflows/params_segment_baboon_ants_t1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}"}*

```diff
@@ -10,14 +10,15 @@
         }
     },
     "brain_segment_pipe": {
         "register_NMT_pipe": {
             "NMT_subject_align": {
                 "afni_ext": "orig"
             },
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_baboon_ants_t1t2debias.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_ants_template.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.39236111111111116%*

 * *Differences: {"'brain_extraction_pipe'": "{'extract_pipe': {'atlas_brex': {'reg': 1, 'wrp': '10,10,10', 'dil': "*

 * *                            "2, 'nrm': 1}}, 'N4debias': OrderedDict([('dimension', 3), "*

 * *                            "('bspline_fitting_distance', 200), ('n_iterations', [50, 50, 40, "*

 * *                            "30]), ('convergence_threshold', 1e-08), ('shrink_factor', 2), "*

 * *                            "('args', '-r 0 --verbose 1')]), delete: ['correct_bias_pipe']}",*

 * * "'brain_segment_pipe'": "{'register_NMT […]*

```diff
@@ -1,26 +1,30 @@
 {
     "brain_extraction_pipe": {
-        "correct_bias_pipe": {
-            "norm_smooth": {
-                "op_string": "-s 2 -div %s"
-            },
-            "smooth": {
-                "args": "-bin -s 2"
-            },
-            "smooth_bias": {
-                "sigma": 2
-            }
+        "N4debias": {
+            "args": "-r 0 --verbose 1",
+            "bspline_fitting_distance": 200,
+            "convergence_threshold": 1e-08,
+            "dimension": 3,
+            "n_iterations": [
+                50,
+                50,
+                40,
+                30
+            ],
+            "shrink_factor": 2
         },
         "extract_pipe": {
             "atlas_brex": {
+                "dil": 2,
                 "f": 0.5,
                 "msk": "a,0,0",
-                "reg": 2,
-                "wrp": "1"
+                "nrm": 1,
+                "reg": 1,
+                "wrp": "10,10,10"
             }
         }
     },
     "brain_segment_pipe": {
         "masked_correct_bias_pipe": {
             "norm_smooth": {
                 "op_string": "-s 2 -div %s"
@@ -29,18 +33,15 @@
                 "args": "-bin -s 2"
             },
             "smooth_bias": {
                 "sigma": 2
             }
         },
         "register_NMT_pipe": {
-            "NMT_subject_align": {
-                "afni_ext": "orig"
-            },
-            "NMT_version": "1.3",
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
@@ -65,58 +66,25 @@
             "threshold_wm": {
                 "thresh": 0.5
             },
             "use_priors": 0.0
         }
     },
     "general": {
-        "template_name": "haiko89_template"
+        "template_name": "NMT_v1.3better"
     },
-    "long_single_preparation_pipe": {
-        "align_T2_on_T1": {
-            "cost": "normmi",
-            "dof": 6
+    "mask_from_seg_pipe": {
+        "dilate_mask": {
+            "kernel_shape": "sphere",
+            "kernel_size": 2
         },
-        "prep_T1": {
-            "crop_T1": {
-                "args": "should be defined in indiv"
-            },
-            "denoise": {
-                "shrink_factor": 1
-            },
-            "norm_intensity": {
-                "args": "-r 0 --verbose 1",
-                "bspline_fitting_distance": 200,
-                "convergence_threshold": 1e-08,
-                "dimension": 3,
-                "n_iterations": [
-                    50,
-                    50,
-                    40,
-                    30
-                ],
-                "shrink_factor": 2
-            }
-        },
-        "prep_T2": {
-            "crop_T2": {
-                "args": "should be defined in indiv"
-            },
-            "denoise": {
-                "shrink_factor": 1
-            },
-            "norm_intensity": {
-                "args": "-r 0 --verbose 1",
-                "bspline_fitting_distance": 200,
-                "convergence_threshold": 1e-08,
-                "dimension": 3,
-                "n_iterations": [
-                    50,
-                    50,
-                    40,
-                    30
-                ],
-                "shrink_factor": 2
-            }
+        "erode_mask": {
+            "kernel_shape": "sphere",
+            "kernel_size": 2
+        }
+    },
+    "short_preparation_pipe": {
+        "crop_T1": {
+            "args": "should be defined in indiv"
         }
     }
 }
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_chimp_ants_t1.json` & `macapype-0.3.dev3/workflows/params_segment_chimp_ants_t1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}"}*

```diff
@@ -7,14 +7,15 @@
                 "reg": 2,
                 "wrp": "1"
             }
         }
     },
     "brain_segment_pipe": {
         "register_NMT_pipe": {
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_ants.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_ants.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666667%*

 * *Differences: {"'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}"}*

```diff
@@ -33,15 +33,15 @@
                 "args": "-bin -s 2"
             },
             "smooth_bias": {
                 "sigma": 2
             }
         },
         "register_NMT_pipe": {
-            "NMT_version": "1.3",
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_ants_segkmeans.json` & `macapype-0.3.dev3/workflows/params_segment_marmo_ants_t1.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7703869047619047%*

 * *Differences: {"'brain_extraction_pipe'": "{'extract_pipe': {'atlas_brex': {'f': 0.6, 'dil': 4, 'args': '-vox "*

 * *                            "1', delete: ['nrm']}}, delete: ['N4debias']}",*

 * * "'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3', 'NMT_subject_align': "*

 * *                         "OrderedDict([('afni_ext', 'orig')])}, 'segment_atropos_pipe': "*

 * *                         "{'use_priors': 0.0}}",*

 * * "'general'": "{'template_name': 'MBM_v3.0.1'}",*

 * * "'short_preparation_pipe'": "{'norm_intensity': Ordere […]*

```diff
@@ -1,28 +1,15 @@
 {
     "brain_extraction_pipe": {
-        "N4debias": {
-            "args": "-r 0 --verbose 1",
-            "bspline_fitting_distance": 200,
-            "convergence_threshold": 1e-08,
-            "dimension": 3,
-            "n_iterations": [
-                50,
-                50,
-                40,
-                30
-            ],
-            "shrink_factor": 2
-        },
         "extract_pipe": {
             "atlas_brex": {
-                "dil": 2,
-                "f": 0.5,
+                "args": "-vox 1",
+                "dil": 4,
+                "f": 0.6,
                 "msk": "a,0,0",
-                "nrm": 1,
                 "reg": 1,
                 "wrp": "10,10,10"
             }
         }
     },
     "brain_segment_pipe": {
         "masked_correct_bias_pipe": {
@@ -33,15 +20,18 @@
                 "args": "-bin -s 2"
             },
             "smooth_bias": {
                 "sigma": 2
             }
         },
         "register_NMT_pipe": {
-            "NMT_version": "1.3",
+            "NMT_subject_align": {
+                "afni_ext": "orig"
+            },
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
@@ -61,19 +51,36 @@
                 "thresh": 0.5
             },
             "threshold_gm": {
                 "thresh": 0.5
             },
             "threshold_wm": {
                 "thresh": 0.5
-            }
+            },
+            "use_priors": 0.0
         }
     },
     "general": {
-        "template_name": "NMT_v1.3"
+        "template_name": "MBM_v3.0.1"
     },
     "short_preparation_pipe": {
         "crop_T1": {
             "args": "should be defined in indiv"
+        },
+        "denoise": {
+            "shrink_factor": 1
+        },
+        "norm_intensity": {
+            "args": "-r 0 --verbose 1",
+            "bspline_fitting_distance": 200,
+            "convergence_threshold": 1e-08,
+            "dimension": 3,
+            "n_iterations": [
+                50,
+                50,
+                40,
+                30
+            ],
+            "shrink_factor": 2
         }
     }
 }
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_ants_t1.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_ants_t1.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}"}*

```diff
@@ -7,14 +7,15 @@
                 "reg": 2,
                 "wrp": "1"
             }
         }
     },
     "brain_segment_pipe": {
         "register_NMT_pipe": {
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_ants_t1_template.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_ants_t1_template.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3'}}"}*

```diff
@@ -9,14 +9,15 @@
                 "reg": 1,
                 "wrp": "10,10,10"
             }
         }
     },
     "brain_segment_pipe": {
         "register_NMT_pipe": {
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_ants_template.json` & `macapype-0.3.dev3/workflows/params_segment_baboon_ants.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6854166666666666%*

 * *Differences: {"'brain_extraction_pipe'": "{'extract_pipe': {'atlas_brex': {'reg': 2, 'wrp': '1', delete: "*

 * *                            "['dil', 'nrm']}}}",*

 * * "'brain_segment_pipe'": "{'register_NMT_pipe': {'NMT_version': 'v1.3', 'NMT_subject_align': "*

 * *                         "OrderedDict([('afni_ext', 'orig')])}}",*

 * * "'general'": "{'template_name': 'haiko89_template'}",*

 * * "'short_preparation_pipe'": "{'norm_intensity': OrderedDict([('dimension', 3), "*

 * *                             "('bspline_fitting_distance', 200), ('n_it […]*

```diff
@@ -11,20 +11,18 @@
                 40,
                 30
             ],
             "shrink_factor": 2
         },
         "extract_pipe": {
             "atlas_brex": {
-                "dil": 2,
                 "f": 0.5,
                 "msk": "a,0,0",
-                "nrm": 1,
-                "reg": 1,
-                "wrp": "10,10,10"
+                "reg": 2,
+                "wrp": "1"
             }
         }
     },
     "brain_segment_pipe": {
         "masked_correct_bias_pipe": {
             "norm_smooth": {
                 "op_string": "-s 2 -div %s"
@@ -33,15 +31,18 @@
                 "args": "-bin -s 2"
             },
             "smooth_bias": {
                 "sigma": 2
             }
         },
         "register_NMT_pipe": {
-            "NMT_version": "1.3",
+            "NMT_subject_align": {
+                "afni_ext": "orig"
+            },
+            "NMT_version": "v1.3",
             "norm_intensity": {
                 "args": "-r 0 --verbose 1",
                 "bspline_fitting_distance": 200,
                 "convergence_threshold": 1e-08,
                 "dimension": 3,
                 "n_iterations": [
                     50,
@@ -66,25 +67,28 @@
             "threshold_wm": {
                 "thresh": 0.5
             },
             "use_priors": 0.0
         }
     },
     "general": {
-        "template_name": "NMT_v1.3"
-    },
-    "mask_from_seg_pipe": {
-        "dilate_mask": {
-            "kernel_shape": "sphere",
-            "kernel_size": 2
-        },
-        "erode_mask": {
-            "kernel_shape": "sphere",
-            "kernel_size": 2
-        }
+        "template_name": "haiko89_template"
     },
     "short_preparation_pipe": {
         "crop_T1": {
             "args": "should be defined in indiv"
+        },
+        "norm_intensity": {
+            "args": "-r 0 --verbose 1",
+            "bspline_fitting_distance": 200,
+            "convergence_threshold": 1e-08,
+            "dimension": 3,
+            "n_iterations": [
+                50,
+                50,
+                40,
+                30
+            ],
+            "shrink_factor": 2
         }
     }
 }
```

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_spm.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_spm.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_spm_native.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_spm_native.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/workflows/params_segment_macaque_spm_t1_native.json` & `macapype-0.3.dev3/workflows/params_segment_macaque_spm_t1_native.json`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/workflows/segment_from_mask_pnh_ants_based.py` & `macapype-0.3.dev3/workflows/segment_from_mask_pnh_ants_based.py`

 * *Files identical despite different names*

### Comparing `macapype-0.3.dev2/workflows/segment_pnh.py` & `macapype-0.3.dev3/workflows/segment_pnh.py`

 * *Files 26% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 from macapype.utils.misc import show_files, get_first_elem
 
 ###############################################################################
 
 def create_main_workflow(data_dir, process_dir, soft, species, subjects, sessions,
                          acquisitions, reconstructions, params_file,
                          indiv_params_file, mask_file, nprocs,
-                         wf_name="test_pipeline_single",
+                         wf_name="macapype",
                          deriv=False, pad=False):
 
     # macapype_pipeline
     """ Set up the segmentatiopn pipeline based on ANTS
 
     Arguments
     ---------
@@ -121,14 +121,19 @@
     workflow: nipype.pipeline.engine.Workflow
 
 
     """
 
     soft = soft.lower()
 
+    ssoft = soft.split("_")
+
+    if 'test' in ssoft:
+        soft = "_".join(ssoft[:-1])
+
     # formating args
     data_dir = op.abspath(data_dir)
 
 
     try:
         os.makedirs(process_dir)
     except OSError:
@@ -172,27 +177,154 @@
 
     params = json.load(open(params_file))
 
     pprint.pprint(params)
 
     # indiv_params
     indiv_params = {}
-    if indiv_params_file is not None:
+
+    if indiv_params_file is None:
+
+        print("No indiv params where found, modifing pipepline to default")
+
+        if "short_preparation_pipe" in params.keys():
+            if "crop_T1" in params["short_preparation_pipe"].keys():
+                print("Deleting crop_T1")
+                del params["short_preparation_pipe"]["crop_T1"]
+
+                print("Adding automated bet_crop")
+
+                params["short_preparation_pipe"]["bet_crop"] = {"m": True, "aT2": True, "c": 10, "n": 2}
+
+                print("Using default bet_crop parameters: {}".format(
+                    params["short_preparation_pipe"]["bet_crop"]))
+
+                print("New params after modification")
+                pprint.pprint(params)
+
+                wf_name+="_bet_crop"
+
+    else:
+
+        assert "short_preparation_pipe" in params.keys(),\
+            "Error, short_preparation_pipe not found in params"
+
+        prep_pipe = "short_preparation_pipe"
+        count_all_sessions=0
+        count_T1_crops=0
+        count_long_crops=0
+        count_multi_long_crops=0
 
         print("Indiv Params:", indiv_params_file)
 
         assert os.path.exists(indiv_params_file), "Error with file {}".format(
             indiv_params_file)
 
         indiv_params = json.load(open(indiv_params_file))
 
         wf_name+="_indiv_params"
 
+        pprint.pprint(indiv_params)
+
+        if subjects is None or sessions is None:
+            print("For whole BIDS dir, unable to assess if the indiv_params is correct")
+            print("Running with params as it is")
+            
+        else:
+                
+            print("Will modify params if necessary, given specified subjects and sessions;\n")
+            
+            for sub in indiv_params.keys():
+
+                if sub.split('-')[1] not in subjects:
+                    continue
+
+                for ses in indiv_params[sub].keys():
+
+                    if ses.split('-')[1] not in sessions:
+                        continue
+
+                    count_all_sessions+=1
+
+                    print (indiv_params[sub][ses].keys())
+
+                    if "crop_T1" in indiv_params[sub][ses].keys():
+                        count_T1_crops+=1
+
+                        if "crop_T2" in indiv_params[sub][ses].keys() \
+                            and 't1' not in ssoft:
+
+                            count_long_crops+=1
 
-    pprint.pprint(indiv_params)
+                            if isinstance(
+                                indiv_params[sub][ses]["crop_T1"]["args"],
+                                list) and isinstance(
+                                    indiv_params[sub][ses]["crop_T2"]["args"],
+                                    list):
+
+                                count_multi_long_crops+=1
+
+            print("count_all_sessions {}".format(count_all_sessions))
+
+            print("count_T1_crops {}".format(count_T1_crops))
+            print("count_long_crops {}".format(count_long_crops))
+            print("count_multi_long_crops {}".format(count_multi_long_crops))
+
+            if count_multi_long_crops==count_all_sessions:
+                print("**** Found list of crops for T1 and T2 for all sub/ses \
+                    in indiv -> long_multi_preparation_pipe")
+
+                wf_name+="_multi_crop_T1_T2"
+
+                prep_pipe = "long_multi_preparation_pipe"
+
+            elif count_long_crops==count_all_sessions:
+
+                print("**** Found crop for T1 and crop for T2 for all sub/ses \
+                    in indiv -> long_single_preparation_pipe")
+
+                wf_name+="_crop_T1_T2"
+
+                prep_pipe = "long_single_preparation_pipe"
+
+            elif count_T1_crops==count_all_sessions:
+
+                print("**** Found crop for T1 for all sub/ses in indiv \
+                    -> keeping short_preparation_pipe")
+
+                wf_name+="_crop_T1"
+
+            else:
+                print("**** not all sub/ses have T1 and T2 crops ")
+                print("Error")
+                exit(0)
+
+            if prep_pipe != "short_preparation_pipe":
+
+                params[prep_pipe]={
+                    "prep_T1": {"crop_T1": {"args": "should be defined in indiv"}},
+                    "prep_T2": {"crop_T2": {"args": "should be defined in indiv"}},
+                    "align_T2_on_T1": {"dof": 6, "cost": "normmi"}}
+
+                if "norm_intensity" in params["short_preparation_pipe"].keys():
+                    norm_intensity= params["short_preparation_pipe"]["norm_intensity"]
+
+                    params[prep_pipe]["prep_T1"]["norm_intensity"]=norm_intensity
+                    params[prep_pipe]["prep_T2"]["norm_intensity"]=norm_intensity
+
+
+                if "denoise" in params["short_preparation_pipe"].keys():
+                    denoise= params["short_preparation_pipe"]["denoise"]
+
+                    params[prep_pipe]["prep_T1"]["denoise"]=denoise
+                    params[prep_pipe]["prep_T2"]["denoise"]=denoise
+
+                del params["short_preparation_pipe"]
+
+            pprint.pprint(params)
 
     # params_template
     assert ("general" in params.keys() and \
         "template_name" in params["general"].keys()), \
             "Error, the params.json should contains a general/template_name"
 
     template_name = params["general"]["template_name"]
@@ -208,16 +340,14 @@
 
     # soft
     wf_name += "_{}".format(soft)
 
     if mask_file is not None:
          wf_name += "_mask"
 
-    ssoft = soft.lower().split("_")
-
     assert "spm" in ssoft or "spm12" in ssoft or "ants" in ssoft, \
         "error with {}, should be among [spm12, spm, ants]".format(ssoft)
 
     # main_workflow
     main_workflow = pe.Workflow(name= wf_name)
 
     main_workflow.base_dir = process_dir
@@ -347,15 +477,15 @@
                             transfo_MD_pipe, 'inputnode.lin_transfo_file')
 
         main_workflow.connect(segment_pnh_pipe, "reg.inv_transfo_file",
                             transfo_MD_pipe, 'inputnode.inv_lin_transfo_file')
 
     if deriv:
 
-        datasink_name = os.path.join("derivatives", "macapype_{}".format(soft))
+        datasink_name = os.path.join("derivatives", "macapype_" + soft)
 
         if "regex_subs" in params.keys():
             params_regex_subs = params["regex_subs"]
         else:
             params_regex_subs={}
 
         if "subs" in params.keys():
```

### Comparing `macapype-0.3.dev2/workflows/segment_pnh_regis.py` & `macapype-0.3.dev3/workflows/segment_pnh_regis.py`

 * *Files identical despite different names*

