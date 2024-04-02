# Comparing `tmp/biomero-1.6.0.tar.gz` & `tmp/biomero-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-kj4_z6jj/biomero-1.6.0.tar", last modified: Thu Feb 29 12:17:35 2024, max compression
+gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-sn_9sy7g/biomero-1.7.0.tar", last modified: Tue Apr  2 12:55:51 2024, max compression
```

## Comparing `biomero-1.6.0.tar` & `biomero-1.7.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 12:17:21.000000 biomero-1.6.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-29 12:17:21.000000 biomero-1.6.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-29 12:17:21.000000 biomero-1.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-29 12:17:21.000000 biomero-1.6.0/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-02-29 12:17:21.000000 biomero-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-29 12:17:21.000000 biomero-1.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 12:17:21.000000 biomero-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-29 12:17:21.000000 biomero-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    52792 2024-02-29 12:17:35.000000 biomero-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38777 2024-02-29 12:17:21.000000 biomero-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-29 12:17:21.000000 biomero-1.6.0/biomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-29 12:17:21.000000 biomero-1.6.0/biomero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    76368 2024-02-29 12:17:21.000000 biomero-1.6.0/biomero/slurm_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    52792 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 12:17:35.000000 biomero-1.6.0/biomero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/omero_slurm_client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-29 12:17:21.000000 biomero-1.6.0/docs/tutorial_link.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-29 12:17:21.000000 biomero-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/convert_job_array.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/convert_zarr_to_tiff.def
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/convert_zarr_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/example.config
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/job_template.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/pull_images.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/slurm-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/resources/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/resources/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/Cells.tif
--rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/cellexpansion.png
--rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/gc_allow_ssh.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/nuclei_labels.png
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/webclient_init_env.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/webclient_init_env_done.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/webclient_run_cellpose.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/images/webclient_run_workflow.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/tutorial_cellexpansion.md
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/tutorial_cellprofiler.md
--rw-r--r--   0 runner    (1001) docker     (127)    26882 2024-02-29 12:17:21.000000 biomero-1.6.0/resources/tutorials/tutorial_local_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 12:17:35.000000 biomero-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:21.000000 biomero-1.6.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:35.000000 biomero-1.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:17:21.000000 biomero-1.6.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45067 2024-02-29 12:17:21.000000 biomero-1.6.0/tests/unit/test_slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 12:55:35.000000 biomero-1.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-02 12:55:35.000000 biomero-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-02 12:55:35.000000 biomero-1.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:55:35.000000 biomero-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 12:55:35.000000 biomero-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-02 12:55:51.000000 biomero-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-02 12:55:35.000000 biomero-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78069 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/omero_slurm_client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/tutorial_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-02 12:55:35.000000 biomero-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_job_array.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_zarr_to_tiff.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_zarr_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/job_template.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/pull_images.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/slurm-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/Cells.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/cellexpansion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/gc_allow_ssh.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/nuclei_labels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_init_env.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_init_env_done.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_run_cellpose.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_run_workflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_Azure_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_cellexpansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_cellprofiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_local_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:55:51.000000 biomero-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45067 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/unit/test_slurm_client.py
```

### Comparing `biomero-1.6.0/.github/workflows/python-package.yml` & `biomero-1.7.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/.github/workflows/python-publish.yml` & `biomero-1.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/.github/workflows/sphinx.yml` & `biomero-1.7.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/.gitignore` & `biomero-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/CITATION.cff` & `biomero-1.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/LICENSE` & `biomero-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/PKG-INFO` & `biomero-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -276,25 +276,26 @@
 
 Your Slurm cluster/login node needs to have:
 1. SSH access w/ public key (headless)
 2. SCP access (generally comes with SSH)
 3. 7zip installed
 4. Singularity/Apptainer installed
 5. (Optional) Git installed, if you want your own job scripts
+6. Slurm accounting enabled
 
 ## OMERO Requirements
 
 Your OMERO _processing_ node needs to have:
 1. SSH client and access to the Slurm cluster (w/ private key / headless)
 2. SCP access to the Slurm cluster
 3. Python3.7+
 4. This library installed 
     - Latest release on PyPI `python3 -m pip install biomero`
     - or latest Github version `python3 -m pip install 'git+https://github.com/NL-BioImaging/biomero'`
-5. uration setup at `/etc/slurm-.ini`
+5. Configuration setup at `/etc/slurm-.ini`
 6. Requirements for some scripts: `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` and the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr).
 
 Your OMERO _server_ node needs to have:
 1. Some OMERO example scripts installed to interact with this library:
     - My examples on github: `https://github.com/NL-BioImaging/biomero-scripts`
     - Install those at `/opt/omero/server/OMERO.server/lib/scripts/slurm/`, e.g. `git clone https://github.com/NL-BioImaging/biomero-scripts.git <path>/slurm`
```

### Comparing `biomero-1.6.0/README.md` & `biomero-1.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,25 +53,26 @@
 
 Your Slurm cluster/login node needs to have:
 1. SSH access w/ public key (headless)
 2. SCP access (generally comes with SSH)
 3. 7zip installed
 4. Singularity/Apptainer installed
 5. (Optional) Git installed, if you want your own job scripts
+6. Slurm accounting enabled
 
 ## OMERO Requirements
 
 Your OMERO _processing_ node needs to have:
 1. SSH client and access to the Slurm cluster (w/ private key / headless)
 2. SCP access to the Slurm cluster
 3. Python3.7+
 4. This library installed 
     - Latest release on PyPI `python3 -m pip install biomero`
     - or latest Github version `python3 -m pip install 'git+https://github.com/NL-BioImaging/biomero'`
-5. uration setup at `/etc/slurm-.ini`
+5. Configuration setup at `/etc/slurm-.ini`
 6. Requirements for some scripts: `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` and the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr).
 
 Your OMERO _server_ node needs to have:
 1. Some OMERO example scripts installed to interact with this library:
     - My examples on github: `https://github.com/NL-BioImaging/biomero-scripts`
     - Install those at `/opt/omero/server/OMERO.server/lib/scripts/slurm/`, e.g. `git clone https://github.com/NL-BioImaging/biomero-scripts.git <path>/slurm`
```

### Comparing `biomero-1.6.0/biomero/constants.py` & `biomero-1.7.0/biomero/constants.py`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/biomero/slurm_client.py` & `biomero-1.7.0/biomero/slurm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,4641 +133,4748 @@
 00000840: 2020 2020 2020 2020 2020 2020 6966 206e              if n
 00000850: 6f74 2070 6f6c 6c5f 7265 7375 6c74 2e6f  ot poll_result.o
 00000860: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
 00000870: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
 00000880: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
 00000890: 2020 2020 2020 2066 2245 7272 6f72 2063         f"Error c
 000008a0: 6865 636b 696e 6720 6a6f 6220 7374 6174  hecking job stat
-000008b0: 7573 3a7b 2070 6f6c 6c5f 7265 7375 6c74  us:{ poll_result
-000008c0: 2e73 7464 6572 7220 7d22 290a 2020 2020  .stderr }").    
-000008d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000008e0: 2e6a 6f62 5f73 7461 7465 203d 2022 4641  .job_state = "FA
-000008f0: 494c 4544 220a 2020 2020 2020 2020 2020  ILED".          
-00000900: 2020 7365 6c66 2e6a 6f62 5f73 7461 7465    self.job_state
-00000910: 203d 206a 6f62 5f73 7461 7475 735f 6469   = job_status_di
-00000920: 6374 5b73 656c 662e 6a6f 625f 6964 5d0a  ct[self.job_id].
-00000930: 2020 2020 2020 2020 2020 2020 2320 7761              # wa
-00000940: 6974 2066 6f72 2031 3020 7365 636f 6e64  it for 10 second
-00000950: 7320 6265 666f 7265 2063 6865 636b 696e  s before checkin
-00000960: 6720 6167 6169 6e0a 2020 2020 2020 2020  g again.        
-00000970: 2020 2020 6f6d 6572 6f43 6f6e 6e2e 6b65      omeroConn.ke
-00000980: 6570 416c 6976 6528 2920 2023 206b 6565  epAlive()  # kee
-00000990: 7020 7468 6520 4f4d 4552 4f20 636f 6e6e  p the OMERO conn
-000009a0: 6563 7469 6f6e 2061 6c69 7665 0a20 2020  ection alive.   
-000009b0: 2020 2020 2020 2020 2074 696d 6573 6c65           timesle
-000009c0: 6570 2e73 6c65 6570 2831 3029 0a20 2020  ep.sleep(10).   
-000009d0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-000009e0: 2866 224a 6f62 207b 7365 6c66 2e6a 6f62  (f"Job {self.job
-000009f0: 5f69 647d 2066 696e 6973 6865 643a 207b  _id} finished: {
-00000a00: 7365 6c66 2e6a 6f62 5f73 7461 7465 7d22  self.job_state}"
-00000a10: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-00000a20: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-00000a30: 2020 2066 2259 6f75 2063 616e 2067 6574     f"You can get
-00000a40: 2074 6865 206c 6f67 6669 6c65 2075 7369   the logfile usi
-00000a50: 6e67 2060 536c 7572 6d20 4765 7420 5570  ng `Slurm Get Up
-00000a60: 6461 7465 6020 6f6e 206a 6f62 207b 7365  date` on job {se
-00000a70: 6c66 2e6a 6f62 5f69 647d 2229 0a20 2020  lf.job_id}").   
-00000a80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000a90: 2e6a 6f62 5f73 7461 7465 0a0a 2020 2020  .job_state..    
-00000aa0: 6465 6620 636f 6d70 6c65 7465 6428 7365  def completed(se
-00000ab0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00000ac0: 0a20 2020 2020 2020 2043 6865 636b 2069  .        Check i
-00000ad0: 6620 7468 6520 536c 7572 6d20 6a6f 6220  f the Slurm job 
-00000ae0: 6861 7320 636f 6d70 6c65 7465 6420 7375  has completed su
-00000af0: 6363 6573 7366 756c 6c79 2e0a 0a20 2020  ccessfully...   
-00000b00: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00000b10: 2020 2020 2020 2020 2020 626f 6f6c 3a20            bool: 
-00000b20: 5472 7565 2069 6620 7468 6520 6a6f 6220  True if the job 
-00000b30: 6861 7320 636f 6d70 6c65 7465 643b 2046  has completed; F
-00000b40: 616c 7365 206f 7468 6572 7769 7365 2e0a  alse otherwise..
-00000b50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00000b60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000b70: 6a6f 625f 7374 6174 6520 3d3d 2022 434f  job_state == "CO
-00000b80: 4d50 4c45 5445 4422 0a0a 2020 2020 6465  MPLETED"..    de
-00000b90: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
-00000ba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00000bb0: 2020 2020 2052 6574 7572 6e20 6120 7374       Return a st
-00000bc0: 7269 6e67 2072 6570 7265 7365 6e74 6174  ring representat
-00000bd0: 696f 6e20 6f66 2074 6865 2053 6c75 726d  ion of the Slurm
-00000be0: 4a6f 6220 696e 7374 616e 6365 2e0a 0a20  Job instance... 
-00000bf0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00000c00: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00000c10: 2053 7472 696e 6720 7265 7072 6573 656e   String represen
-00000c20: 7461 7469 6f6e 2e0a 2020 2020 2020 2020  tation..        
-00000c30: 2222 220a 2020 2020 2020 2020 7072 6f70  """.        prop
-00000c40: 6572 7469 6573 203d 2027 2c20 272e 6a6f  erties = ', '.jo
-00000c50: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00000c60: 6622 7b6b 6579 7d3d 7b76 616c 7565 7d22  f"{key}={value}"
-00000c70: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
-00000c80: 696e 2073 656c 662e 5f5f 6469 6374 5f5f  in self.__dict__
-00000c90: 2e69 7465 6d73 2829 290a 2020 2020 2020  .items()).      
-00000ca0: 2020 7265 7475 726e 2066 2253 6c75 726d    return f"Slurm
-00000cb0: 4a6f 6228 7b70 726f 7065 7274 6965 737d  Job({properties}
-00000cc0: 2922 0a0a 0a63 6c61 7373 2053 6c75 726d  )"...class Slurm
-00000cd0: 436c 6965 6e74 2843 6f6e 6e65 6374 696f  Client(Connectio
-00000ce0: 6e29 3a0a 2020 2020 2222 2241 2063 6c69  n):.    """A cli
-00000cf0: 656e 7420 666f 7220 636f 6e6e 6563 7469  ent for connecti
-00000d00: 6e67 2074 6f20 616e 6420 696e 7465 7261  ng to and intera
-00000d10: 6374 696e 6720 7769 7468 2061 2053 6c75  cting with a Slu
-00000d20: 726d 2063 6c75 7374 6572 206f 7665 720a  rm cluster over.
-00000d30: 2020 2020 5353 482e 0a0a 2020 2020 5468      SSH...    Th
-00000d40: 6973 2063 6c61 7373 2065 7874 656e 6473  is class extends
-00000d50: 2074 6865 2043 6f6e 6e65 6374 696f 6e20   the Connection 
-00000d60: 636c 6173 732c 2061 6464 696e 6720 6d65  class, adding me
-00000d70: 7468 6f64 7320 616e 640a 2020 2020 6174  thods and.    at
-00000d80: 7472 6962 7574 6573 2073 7065 6369 6669  tributes specifi
-00000d90: 6320 746f 2077 6f72 6b69 6e67 2077 6974  c to working wit
-00000da0: 6820 536c 7572 6d2e 0a0a 2020 2020 536c  h Slurm...    Sl
-00000db0: 7572 6d43 6c69 656e 7420 6163 6365 7074  urmClient accept
-00000dc0: 7320 7468 6520 7361 6d65 2061 7267 756d  s the same argum
-00000dd0: 656e 7473 2061 7320 436f 6e6e 6563 7469  ents as Connecti
-00000de0: 6f6e 2e20 4265 6c6f 7720 6f6e 6c79 0a20  on. Below only. 
-00000df0: 2020 206d 656e 7469 6f6e 7320 7468 6520     mentions the 
-00000e00: 6164 6465 6420 6f6e 6573 3a0a 0a20 2020  added ones:..   
-00000e10: 2054 6865 2065 6173 6965 7374 2077 6179   The easiest way
-00000e20: 2074 6f20 7365 7420 7468 6973 2063 6c69   to set this cli
-00000e30: 656e 7420 7570 2069 7320 6279 2075 7369  ent up is by usi
-00000e40: 6e67 2061 2073 6c75 726d 2d63 6f6e 6669  ng a slurm-confi
-00000e50: 672e 696e 690a 2020 2020 616e 6420 7468  g.ini.    and th
-00000e60: 6520 6672 6f6d 2d63 6f6e 6669 6728 2920  e from-config() 
-00000e70: 6d65 7468 6f64 2e0a 0a20 2020 2041 7474  method...    Att
-00000e80: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
-00000e90: 2073 6c75 726d 5f64 6174 615f 7061 7468   slurm_data_path
-00000ea0: 2028 7374 7229 3a20 5468 6520 7061 7468   (str): The path
-00000eb0: 2074 6f20 7468 6520 6469 7265 6374 6f72   to the director
-00000ec0: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00000ed0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00000ee0: 6120 6669 6c65 7320 666f 7220 536c 7572  a files for Slur
-00000ef0: 6d20 6a6f 6273 2e0a 2020 2020 2020 2020  m jobs..        
-00000f00: 736c 7572 6d5f 696d 6167 6573 5f70 6174  slurm_images_pat
-00000f10: 6820 2873 7472 293a 2054 6865 2070 6174  h (str): The pat
-00000f20: 6820 746f 2074 6865 2064 6972 6563 746f  h to the directo
-00000f30: 7279 2063 6f6e 7461 696e 696e 670a 2020  ry containing.  
-00000f40: 2020 2020 2020 2020 2020 7468 6520 5369            the Si
-00000f50: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
-00000f60: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
-00000f70: 0a20 2020 2020 2020 2073 6c75 726d 5f63  .        slurm_c
-00000f80: 6f6e 7665 7274 6572 735f 7061 7468 2028  onverters_path (
-00000f90: 7374 7229 3a20 5468 6520 7061 7468 2074  str): The path t
-00000fa0: 6f20 7468 6520 6469 7265 6374 6f72 7920  o the directory 
-00000fb0: 636f 6e74 6169 6e69 6e67 0a20 2020 2020  containing.     
-00000fc0: 2020 2020 2020 2074 6865 2053 696e 6775         the Singu
-00000fd0: 6c61 7269 7479 2069 6d61 6765 7320 666f  larity images fo
-00000fe0: 7220 6669 6c65 2063 6f6e 7665 7274 6572  r file converter
-00000ff0: 732e 0a20 2020 2020 2020 2073 6c75 726d  s..        slurm
-00001000: 5f6d 6f64 656c 5f70 6174 6873 2028 6469  _model_paths (di
-00001010: 6374 293a 2041 2064 6963 7469 6f6e 6172  ct): A dictionar
-00001020: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00001030: 2070 6174 6873 2074 6f0a 2020 2020 2020   paths to.      
-00001040: 2020 2020 2020 7468 6520 5369 6e67 756c        the Singul
-00001050: 6172 6974 7920 696d 6167 6573 2066 6f72  arity images for
-00001060: 2073 7065 6369 6669 6320 536c 7572 6d20   specific Slurm 
-00001070: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
-00001080: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00001090: 7265 706f 7320 2864 6963 7429 3a20 4120  repos (dict): A 
-000010a0: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-000010b0: 696e 696e 6720 7468 6520 6769 740a 2020  ining the git.  
-000010c0: 2020 2020 2020 2020 2020 7265 706f 7369            reposi
-000010d0: 746f 7269 6573 206f 6620 5369 6e67 756c  tories of Singul
-000010e0: 6172 6974 7920 696d 6167 6573 2066 6f72  arity images for
-000010f0: 2073 7065 6369 6669 6320 536c 7572 6d20   specific Slurm 
-00001100: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
-00001110: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00001120: 696d 6167 6573 2028 6469 6374 293a 2041  images (dict): A
-00001130: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-00001140: 6169 6e69 6e67 2074 6865 2064 6f63 6b65  aining the docke
-00001150: 7268 7562 0a20 2020 2020 2020 2020 2020  rhub.           
-00001160: 206f 6620 7468 6520 5369 6e67 756c 6172   of the Singular
-00001170: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
-00001180: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
-00001190: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
-000011a0: 2020 2020 2020 5769 6c6c 2066 696c 6c20        Will fill 
-000011b0: 6175 746f 6d61 7469 6361 6c6c 7920 6672  automatically fr
-000011c0: 6f6d 2074 6865 2064 6174 6120 696e 2074  om the data in t
-000011d0: 6865 2067 6974 2072 6570 6f73 6974 6f72  he git repositor
-000011e0: 792c 0a20 2020 2020 2020 2020 2020 2069  y,.            i
-000011f0: 6620 796f 7520 7365 7420 696e 6974 5f73  f you set init_s
-00001200: 6c75 726d 2e0a 2020 2020 2020 2020 736c  lurm..        sl
-00001210: 7572 6d5f 7363 7269 7074 5f70 6174 6820  urm_script_path 
-00001220: 2873 7472 293a 2054 6865 2070 6174 6820  (str): The path 
-00001230: 746f 2074 6865 2064 6972 6563 746f 7279  to the directory
-00001240: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
-00001250: 2020 2020 2020 2020 7468 6520 536c 7572          the Slur
-00001260: 6d20 6a6f 6220 7375 626d 6973 7369 6f6e  m job submission
-00001270: 2073 6372 6970 7473 206f 6e20 536c 7572   scripts on Slur
-00001280: 6d2e 0a20 2020 2020 2020 2073 6c75 726d  m..        slurm
-00001290: 5f73 6372 6970 745f 7265 706f 2028 7374  _script_repo (st
-000012a0: 7229 3a20 5468 6520 6769 7420 6874 7470  r): The git http
-000012b0: 7320 5552 4c20 666f 7220 636c 6f6e 696e  s URL for clonin
-000012c0: 6720 7468 6520 7265 706f 0a20 2020 2020  g the repo.     
-000012d0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-000012e0: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
-000012f0: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
-00001300: 7473 2e20 4f70 7469 6f6e 616c 2e0a 0a20  ts. Optional... 
-00001310: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
-00001320: 2020 2020 2320 4372 6561 7465 2061 2053      # Create a S
-00001330: 6c75 726d 436c 6965 6e74 206f 626a 6563  lurmClient objec
-00001340: 7420 6173 2063 6f6e 7465 7874 6d61 6e61  t as contextmana
-00001350: 6765 720a 0a20 2020 2020 2020 2077 6974  ger..        wit
-00001360: 6820 536c 7572 6d43 6c69 656e 742e 6672  h SlurmClient.fr
-00001370: 6f6d 5f63 6f6e 6669 6728 2920 6173 2063  om_config() as c
-00001380: 6c69 656e 743a 0a0a 2020 2020 2020 2020  lient:..        
-00001390: 2020 2020 2320 5275 6e20 6120 636f 6d6d      # Run a comm
-000013a0: 616e 6420 6f6e 2074 6865 2072 656d 6f74  and on the remot
-000013b0: 6520 686f 7374 0a0a 2020 2020 2020 2020  e host..        
-000013c0: 2020 2020 7265 7375 6c74 203d 2063 6c69      result = cli
-000013d0: 656e 742e 7275 6e28 2773 6261 7463 6820  ent.run('sbatch 
-000013e0: 6d79 6a6f 622e 7368 2729 0a0a 2020 2020  myjob.sh')..    
-000013f0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-00001400: 7768 6574 6865 7220 7468 6520 636f 6d6d  whether the comm
-00001410: 616e 6420 7375 6363 6565 6465 640a 0a20  and succeeded.. 
-00001420: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00001430: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
-00001440: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00001450: 4a6f 6220 7375 626d 6974 7465 6420 7375  Job submitted su
-00001460: 6363 6573 7366 756c 6c79 2127 290a 0a20  ccessfully!').. 
-00001470: 2020 2020 2020 2020 2020 2023 2050 7269             # Pri
-00001480: 6e74 2074 6865 206f 7574 7075 7420 6f66  nt the output of
-00001490: 2074 6865 2063 6f6d 6d61 6e64 0a0a 2020   the command..  
-000014a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000014b0: 7265 7375 6c74 2e73 7464 6f75 7429 0a0a  result.stdout)..
-000014c0: 2020 2020 4578 616d 706c 6520 323a 0a20      Example 2:. 
-000014d0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-000014e0: 6120 536c 7572 6d43 6c69 656e 7420 616e  a SlurmClient an
-000014f0: 6420 7365 7475 7020 536c 7572 6d20 2864  d setup Slurm (d
-00001500: 6f77 6e6c 6f61 6420 636f 6e74 6169 6e65  ownload containe
-00001510: 7273 2065 7463 2e29 0a0a 2020 2020 2020  rs etc.)..      
-00001520: 2020 7769 7468 2053 6c75 726d 436c 6965    with SlurmClie
-00001530: 6e74 2e66 726f 6d5f 636f 6e66 6967 2869  nt.from_config(i
-00001540: 6e69 745f 736c 7572 6d3d 5472 7565 2920  nit_slurm=True) 
-00001550: 6173 2063 6c69 656e 743a 0a0a 2020 2020  as client:..    
-00001560: 2020 2020 2020 2020 636c 6965 6e74 2e72          client.r
-00001570: 756e 5f77 6f72 6b66 6c6f 7728 2e2e 2e29  un_workflow(...)
-00001580: 0a0a 2020 2020 2222 220a 2020 2020 5f44  ..    """.    _D
-00001590: 4546 4155 4c54 5f43 4f4e 4649 475f 5041  EFAULT_CONFIG_PA
-000015a0: 5448 5f31 203d 2022 2f65 7463 2f73 6c75  TH_1 = "/etc/slu
-000015b0: 726d 2d63 6f6e 6669 672e 696e 6922 0a20  rm-config.ini". 
-000015c0: 2020 205f 4445 4641 554c 545f 434f 4e46     _DEFAULT_CONF
-000015d0: 4947 5f50 4154 485f 3220 3d20 227e 2f73  IG_PATH_2 = "~/s
-000015e0: 6c75 726d 2d63 6f6e 6669 672e 696e 6922  lurm-config.ini"
-000015f0: 0a20 2020 205f 4445 4641 554c 545f 484f  .    _DEFAULT_HO
-00001600: 5354 203d 2022 736c 7572 6d22 0a20 2020  ST = "slurm".   
-00001610: 205f 4445 4641 554c 545f 494e 4c49 4e45   _DEFAULT_INLINE
-00001620: 5f53 5348 5f45 4e56 203d 2054 7275 650a  _SSH_ENV = True.
-00001630: 2020 2020 5f44 4546 4155 4c54 5f53 4c55      _DEFAULT_SLU
-00001640: 524d 5f44 4154 415f 5041 5448 203d 2022  RM_DATA_PATH = "
-00001650: 6d79 2d73 6372 6174 6368 2f64 6174 6122  my-scratch/data"
-00001660: 0a20 2020 205f 4445 4641 554c 545f 534c  .    _DEFAULT_SL
-00001670: 5552 4d5f 494d 4147 4553 5f50 4154 4820  URM_IMAGES_PATH 
-00001680: 3d20 226d 792d 7363 7261 7463 682f 7369  = "my-scratch/si
-00001690: 6e67 756c 6172 6974 795f 696d 6167 6573  ngularity_images
-000016a0: 2f77 6f72 6b66 6c6f 7773 220a 2020 2020  /workflows".    
-000016b0: 5f44 4546 4155 4c54 5f53 4c55 524d 5f43  _DEFAULT_SLURM_C
-000016c0: 4f4e 5645 5254 4552 535f 5041 5448 203d  ONVERTERS_PATH =
-000016d0: 2022 6d79 2d73 6372 6174 6368 2f73 696e   "my-scratch/sin
-000016e0: 6775 6c61 7269 7479 5f69 6d61 6765 732f  gularity_images/
-000016f0: 636f 6e76 6572 7465 7273 220a 2020 2020  converters".    
-00001700: 5f44 4546 4155 4c54 5f53 4c55 524d 5f47  _DEFAULT_SLURM_G
-00001710: 4954 5f53 4352 4950 545f 5041 5448 203d  IT_SCRIPT_PATH =
-00001720: 2022 736c 7572 6d2d 7363 7269 7074 7322   "slurm-scripts"
-00001730: 0a20 2020 205f 4f55 545f 5345 5020 3d20  .    _OUT_SEP = 
-00001740: 222d 2d73 706c 6974 2d2d 220a 2020 2020  "--split--".    
-00001750: 5f56 4552 5349 4f4e 5f43 4d44 203d 2022  _VERSION_CMD = "
-00001760: 6c73 202d 6820 7b73 6c75 726d 5f69 6d61  ls -h {slurm_ima
-00001770: 6765 735f 7061 7468 7d2f 7b69 6d61 6765  ges_path}/{image
-00001780: 5f70 6174 687d 207c 2067 7265 7020 2d6f  _path} | grep -o
-00001790: 5020 2728 3f3c 3d5c 2d7c 5c5f 2928 762e  P '(?<=\-|\_)(v.
-000017a0: 2b7c 6c61 7465 7374 2928 3f3d 2e73 696d  +|latest)(?=.sim
-000017b0: 677c 2e73 6966 2927 220a 2020 2020 2320  g|.sif)'".    # 
-000017c0: 4e6f 7465 2c20 6772 6570 2072 6574 7572  Note, grep retur
-000017d0: 6e73 2065 7869 7463 6f64 6520 3120 6966  ns exitcode 1 if
-000017e0: 206e 6f20 6d61 7463 6820 6973 2066 6f75   no match is fou
-000017f0: 6e64 210a 2020 2020 2320 5468 6973 2077  nd!.    # This w
-00001800: 696c 6c20 7472 616e 736c 6174 6520 696e  ill translate in
-00001810: 746f 2061 2055 6e65 7870 6563 7465 6445  to a UnexpectedE
-00001820: 7869 7420 6572 726f 722c 2073 6f20 6d75  xit error, so mu
-00001830: 7465 2074 6861 7420 6966 2079 6f75 0a20  te that if you. 
-00001840: 2020 2023 2064 6f6e 2774 2063 6172 6520     # don't care 
-00001850: 6162 6f75 7420 656d 7074 792e 0a20 2020  about empty..   
-00001860: 2023 204c 696b 6520 6265 6c6f 7720 7769   # Like below wi
-00001870: 7468 2074 6865 2022 7c7c 203a 222e 0a20  th the "|| :".. 
-00001880: 2020 2023 2044 6174 6120 636f 756c 6420     # Data could 
-00001890: 6c65 6769 7420 6265 2065 6d70 7479 2e0a  legit be empty..
-000018a0: 2020 2020 5f44 4154 415f 434d 4420 3d20      _DATA_CMD = 
-000018b0: 226c 7320 2d68 207b 736c 7572 6d5f 6461  "ls -h {slurm_da
-000018c0: 7461 5f70 6174 687d 207c 2067 7265 7020  ta_path} | grep 
-000018d0: 2d6f 5020 272e 2b28 3f3d 2e7a 6970 2927  -oP '.+(?=.zip)'
-000018e0: 207c 7c20 3a22 0a20 2020 205f 414c 4c5f   || :".    _ALL_
-000018f0: 4a4f 4253 5f43 4d44 203d 2022 7361 6363  JOBS_CMD = "sacc
-00001900: 7420 2d2d 7374 6172 7474 696d 6520 7b73  t --starttime {s
-00001910: 7461 7274 5f74 696d 657d 202d 2d65 6e64  tart_time} --end
-00001920: 7469 6d65 207b 656e 645f 7469 6d65 7d20  time {end_time} 
-00001930: 2d2d 7374 6174 6520 7b73 7461 7465 737d  --state {states}
-00001940: 202d 6f20 7b63 6f6c 756d 6e73 7d20 2d6e   -o {columns} -n
-00001950: 202d 5820 220a 2020 2020 5f5a 4950 5f43   -X ".    _ZIP_C
-00001960: 4d44 203d 2022 377a 2061 202d 7920 7b66  MD = "7z a -y {f
-00001970: 696c 656e 616d 657d 202d 747a 6970 207b  ilename} -tzip {
-00001980: 6461 7461 5f6c 6f63 6174 696f 6e7d 2f64  data_location}/d
-00001990: 6174 612f 6f75 7422 0a20 2020 205f 4143  ata/out".    _AC
-000019a0: 5449 5645 5f4a 4f42 535f 434d 4420 3d20  TIVE_JOBS_CMD = 
-000019b0: 2273 7175 6575 6520 2d75 2024 5553 4552  "squeue -u $USER
-000019c0: 202d 2d6e 6f68 6561 6420 2d2d 666f 726d   --nohead --form
-000019d0: 6174 2025 4622 0a20 2020 205f 4a4f 425f  at %F".    _JOB_
-000019e0: 5354 4154 5553 5f43 4d44 203d 2022 7361  STATUS_CMD = "sa
-000019f0: 6363 7420 2d6e 202d 6f20 4a6f 6249 642c  cct -n -o JobId,
-00001a00: 5374 6174 652c 456e 6420 2d58 202d 6a20  State,End -X -j 
-00001a10: 7b73 6c75 726d 5f6a 6f62 5f69 647d 220a  {slurm_job_id}".
-00001a20: 2020 2020 2320 544f 444f 206d 6f76 6520      # TODO move 
-00001a30: 616c 6c20 636f 6d6d 616e 6473 2074 6f20  all commands to 
-00001a40: 6120 7369 6d69 6c61 7220 666f 726d 6174  a similar format
-00001a50: 2e0a 2020 2020 2320 5468 656e 206d 6179  ..    # Then may
-00001a60: 6265 2061 6c6c 6f77 206f 7665 7277 7269  be allow overwri
-00001a70: 7465 2066 726f 6d20 736c 7572 6d2d 636f  te from slurm-co
-00001a80: 6e66 6967 2e69 6e69 0a20 2020 205f 4c4f  nfig.ini.    _LO
-00001a90: 4746 494c 4520 3d20 226f 6d65 726f 2d7b  GFILE = "omero-{
-00001aa0: 736c 7572 6d5f 6a6f 625f 6964 7d2e 6c6f  slurm_job_id}.lo
-00001ab0: 6722 0a20 2020 205f 5441 494c 5f4c 4f47  g".    _TAIL_LOG
-00001ac0: 5f43 4d44 203d 2022 7461 696c 202d 6e20  _CMD = "tail -n 
-00001ad0: 7b6e 7d20 7b6c 6f67 5f66 696c 657d 207c  {n} {log_file} |
-00001ae0: 2073 7472 696e 6773 220a 2020 2020 5f4c   strings".    _L
-00001af0: 4f47 4649 4c45 5f44 4154 415f 434d 4420  OGFILE_DATA_CMD 
-00001b00: 3d20 2263 6174 207b 6c6f 675f 6669 6c65  = "cat {log_file
-00001b10: 7d20 7c20 7065 726c 202d 776e 6520 272f  } | perl -wne '/
-00001b20: 5275 6e6e 696e 6720 5b5c 772d 5d2b 3f20  Running [\w-]+? 
-00001b30: 4a6f 6220 775c 2f20 2e2b 3f20 5c7c 202e  Job w\/ .+? \| .
-00001b40: 2b3f 205c 7c20 282e 2b3f 2920 5c7c 2e2a  +? \| (.+?) \|.*
-00001b50: 2f69 2061 6e64 2070 7269 6e74 2431 2722  /i and print$1'"
-00001b60: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00001b70: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
-00001b80: 2020 2020 2020 2020 2020 686f 7374 3d5f            host=_
-00001b90: 4445 4641 554c 545f 484f 5354 2c0a 2020  DEFAULT_HOST,.  
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00001bb0: 7365 723d 4e6f 6e65 2c0a 2020 2020 2020  ser=None,.      
-00001bc0: 2020 2020 2020 2020 2020 2070 6f72 743d             port=
-00001bd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001be0: 2020 2020 2020 2063 6f6e 6669 673d 4e6f         config=No
-00001bf0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001c00: 2020 2020 2067 6174 6577 6179 3d4e 6f6e       gateway=Non
-00001c10: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001c20: 2020 2020 666f 7277 6172 645f 6167 656e      forward_agen
-00001c30: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
-00001c40: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-00001c50: 5f74 696d 656f 7574 3d4e 6f6e 652c 0a20  _timeout=None,. 
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 636f 6e6e 6563 745f 6b77 6172 6773 3d4e  connect_kwargs=N
-00001c80: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001c90: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
-00001ca0: 5f65 6e76 3d5f 4445 4641 554c 545f 494e  _env=_DEFAULT_IN
-00001cb0: 4c49 4e45 5f53 5348 5f45 4e56 2c0a 2020  LINE_SSH_ENV,.  
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001cd0: 6c75 726d 5f64 6174 615f 7061 7468 3a20  lurm_data_path: 
-00001ce0: 7374 7220 3d20 5f44 4546 4155 4c54 5f53  str = _DEFAULT_S
-00001cf0: 4c55 524d 5f44 4154 415f 5041 5448 2c0a  LURM_DATA_PATH,.
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2073 6c75 726d 5f69 6d61 6765 735f 7061   slurm_images_pa
-00001d20: 7468 3a20 7374 7220 3d20 5f44 4546 4155  th: str = _DEFAU
-00001d30: 4c54 5f53 4c55 524d 5f49 4d41 4745 535f  LT_SLURM_IMAGES_
-00001d40: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
-00001d50: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
-00001d60: 7665 7274 6572 735f 7061 7468 3a20 7374  verters_path: st
-00001d70: 7220 3d20 5f44 4546 4155 4c54 5f53 4c55  r = _DEFAULT_SLU
-00001d80: 524d 5f43 4f4e 5645 5254 4552 535f 5041  RM_CONVERTERS_PA
-00001d90: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
-00001da0: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-00001db0: 5f70 6174 6873 3a20 6469 6374 203d 204e  _paths: dict = N
-00001dc0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001dd0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00001de0: 6c5f 7265 706f 733a 2064 6963 7420 3d20  l_repos: dict = 
-00001df0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001e00: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00001e10: 656c 5f69 6d61 6765 733a 2064 6963 7420  el_images: dict 
-00001e20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00001e30: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
-00001e40: 6f64 656c 5f6a 6f62 733a 2064 6963 7420  odel_jobs: dict 
-00001e50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00001e60: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
-00001e70: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
-00001e80: 3a20 6469 6374 203d 204e 6f6e 652c 0a20  : dict = None,. 
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
-00001eb0: 683a 2073 7472 203d 205f 4445 4641 554c  h: str = _DEFAUL
-00001ec0: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
-00001ed0: 5054 5f50 4154 482c 0a20 2020 2020 2020  PT_PATH,.       
-00001ee0: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-00001ef0: 7363 7269 7074 5f72 6570 6f3a 2073 7472  script_repo: str
-00001f00: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00001f10: 2020 2020 2020 2020 2020 696e 6974 5f73            init_s
-00001f20: 6c75 726d 3a20 626f 6f6c 203d 2046 616c  lurm: bool = Fal
-00001f30: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00001f40: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00001f50: 2222 2249 6e69 7469 616c 697a 6573 2061  """Initializes a
-00001f60: 206e 6577 2069 6e73 7461 6e63 6520 6f66   new instance of
-00001f70: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
-00001f80: 2063 6c61 7373 2e0a 0a20 2020 2020 2020   class...       
-00001f90: 2049 7420 6973 2070 7265 6665 7261 626c   It is preferabl
-00001fa0: 6520 746f 2075 7365 2023 6672 6f6d 5f63  e to use #from_c
-00001fb0: 6f6e 6669 6728 2e2e 2e29 206d 6574 686f  onfig(...) metho
-00001fc0: 6420 746f 2069 6e69 7469 616c 697a 650a  d to initialize.
-00001fd0: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
-00001fe0: 7273 2066 726f 6d20 6120 636f 6e66 6967  rs from a config
-00001ff0: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
-00002000: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00002010: 2020 686f 7374 2028 7374 722c 206f 7074    host (str, opt
-00002020: 696f 6e61 6c29 3a20 5468 6520 686f 7374  ional): The host
-00002030: 6e61 6d65 206f 7220 4950 2061 6464 7265  name or IP addre
-00002040: 7373 206f 6620 7468 6520 7265 6d6f 7465  ss of the remote
-00002050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002060: 2073 6572 7665 722e 2044 6566 6175 6c74   server. Default
-00002070: 7320 746f 205f 4445 4641 554c 545f 484f  s to _DEFAULT_HO
-00002080: 5354 2e0a 2020 2020 2020 2020 2020 2020  ST..            
-00002090: 7573 6572 2028 7374 722c 206f 7074 696f  user (str, optio
-000020a0: 6e61 6c29 3a20 5468 6520 7573 6572 6e61  nal): The userna
-000020b0: 6d65 2074 6f20 7573 6520 7768 656e 2063  me to use when c
-000020c0: 6f6e 6e65 6374 696e 6720 746f 200a 2020  onnecting to .  
-000020d0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-000020e0: 6520 7265 6d6f 7465 2073 6572 7665 722e  e remote server.
-000020f0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00002100: 652c 2077 6869 6368 2064 6566 6175 6c74  e, which default
-00002110: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-00002120: 2020 2074 6f20 636f 6e66 6967 2e75 7365     to config.use
-00002130: 722e 0a20 2020 2020 2020 2020 2020 2070  r..            p
-00002140: 6f72 7420 2869 6e74 2c20 6f70 7469 6f6e  ort (int, option
-00002150: 616c 293a 2054 6865 2053 5348 2070 6f72  al): The SSH por
-00002160: 7420 746f 2075 7365 2077 6865 6e20 636f  t to use when co
-00002170: 6e6e 6563 7469 6e67 2e0a 2020 2020 2020  nnecting..      
-00002180: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00002190: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
-000021a0: 6820 6465 6661 756c 7473 2074 6f20 636f  h defaults to co
-000021b0: 6e66 6967 2e70 6f72 742e 0a20 2020 2020  nfig.port..     
-000021c0: 2020 2020 2020 2063 6f6e 6669 6720 2873         config (s
-000021d0: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
-000021e0: 6174 6820 746f 2074 6865 2053 5348 2063  ath to the SSH c
-000021f0: 6f6e 6669 6720 6669 6c65 2e0a 2020 2020  onfig file..    
-00002200: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00002210: 756c 7473 2074 6f20 4e6f 6e65 2c20 7768  ults to None, wh
-00002220: 6963 6820 6465 6661 756c 7473 2074 6f20  ich defaults to 
-00002230: 796f 7572 2053 5348 2063 6f6e 6669 6720  your SSH config 
-00002240: 6669 6c65 2e0a 2020 2020 2020 2020 2020  file..          
-00002250: 2020 6761 7465 7761 7920 2843 6f6e 6e65    gateway (Conne
-00002260: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
-00002270: 3a20 416e 206f 7074 696f 6e61 6c20 6761  : An optional ga
-00002280: 7465 7761 7920 666f 7220 636f 6e6e 6563  teway for connec
-00002290: 7469 6e67 200a 2020 2020 2020 2020 2020  ting .          
-000022a0: 2020 2020 2020 7468 726f 7567 6820 6120        through a 
-000022b0: 6a75 6d70 2068 6f73 742e 2044 6566 6175  jump host. Defau
-000022c0: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
-000022d0: 2020 2020 2020 2020 2066 6f72 7761 7264           forward
-000022e0: 5f61 6765 6e74 2028 626f 6f6c 2c20 6f70  _agent (bool, op
-000022f0: 7469 6f6e 616c 293a 2057 6865 7468 6572  tional): Whether
-00002300: 2074 6f20 666f 7277 6172 6420 7468 6520   to forward the 
-00002310: 6c6f 6361 6c20 5353 4820 0a20 2020 2020  local SSH .     
-00002320: 2020 2020 2020 2020 2020 2061 6765 6e74             agent
-00002330: 2074 6f20 7468 6520 7265 6d6f 7465 2073   to the remote s
-00002340: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
-00002350: 746f 204e 6f6e 652c 2077 6869 6368 200a  to None, which .
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 6465 6661 756c 7473 2074 6f20 636f 6e66  defaults to conf
-00002380: 6967 2e66 6f72 7761 7264 5f61 6765 6e74  ig.forward_agent
-00002390: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000023a0: 6e6e 6563 745f 7469 6d65 6f75 7420 2869  nnect_timeout (i
-000023b0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2054  nt, optional): T
-000023c0: 696d 656f 7574 2066 6f72 2065 7374 6162  imeout for estab
-000023d0: 6c69 7368 696e 6720 7468 6520 5353 4820  lishing the SSH 
-000023e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023f0: 2063 6f6e 6e65 6374 696f 6e2e 2044 6566   connection. Def
-00002400: 6175 6c74 7320 746f 204e 6f6e 652c 2077  aults to None, w
-00002410: 6869 6368 2064 6566 6175 6c74 7320 0a20  hich defaults . 
-00002420: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002430: 6f20 636f 6e66 6967 2e74 696d 656f 7574  o config.timeout
-00002440: 732e 636f 6e6e 6563 742e 0a20 2020 2020  s.connect..     
-00002450: 2020 2020 2020 2063 6f6e 6e65 6374 5f6b         connect_k
-00002460: 7761 7267 7320 2864 6963 742c 206f 7074  wargs (dict, opt
-00002470: 696f 6e61 6c29 3a20 4164 6469 7469 6f6e  ional): Addition
-00002480: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
-00002490: 656e 7473 2066 6f72 200a 2020 2020 2020  ents for .      
-000024a0: 2020 2020 2020 2020 2020 7468 6520 756e            the un
-000024b0: 6465 726c 7969 6e67 2053 5348 2063 6f6e  derlying SSH con
-000024c0: 6e65 6374 696f 6e2e 2048 616e 6465 6420  nection. Handed 
-000024d0: 7665 7262 6174 696d 2074 6f20 0a20 2020  verbatim to .   
-000024e0: 2020 2020 2020 2020 2020 2020 2060 5353               `SS
-000024f0: 4843 6c69 656e 742e 636f 6e6e 6563 7420  HClient.connect 
-00002500: 3c70 6172 616d 696b 6f2e 636c 6965 6e74  <paramiko.client
-00002510: 2e53 5348 436c 6965 6e74 2e63 6f6e 6e65  .SSHClient.conne
-00002520: 6374 3e60 2e20 0a20 2020 2020 2020 2020  ct>`. .         
-00002530: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00002540: 746f 204e 6f6e 652e 200a 2020 2020 2020  to None. .      
-00002550: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
-00002560: 5f65 6e76 2028 626f 6f6c 2c20 6f70 7469  _env (bool, opti
-00002570: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
-00002580: 6f20 7573 6520 696e 6c69 6e65 2053 5348  o use inline SSH
-00002590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000025a0: 2065 6e76 6972 6f6e 6d65 6e74 2e20 5468   environment. Th
-000025b0: 6973 2069 7320 6e65 6365 7373 6172 7920  is is necessary 
-000025c0: 6966 2074 6865 2072 656d 6f74 6520 7365  if the remote se
-000025d0: 7276 6572 2068 6173 200a 2020 2020 2020  rver has .      
-000025e0: 2020 2020 2020 2020 2020 6120 7265 7374            a rest
-000025f0: 7269 6374 6564 2060 6041 6363 6570 7445  ricted ``AcceptE
-00002600: 6e76 6060 2073 6574 7469 6e67 2028 7768  nv`` setting (wh
-00002610: 6963 6820 6973 2074 6865 2063 6f6d 6d6f  ich is the commo
-00002620: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
-00002630: 2020 2064 6566 6175 6c74 292e 2044 6566     default). Def
-00002640: 6175 6c74 7320 746f 205f 4445 4641 554c  aults to _DEFAUL
-00002650: 545f 494e 4c49 4e45 5f53 5348 5f45 4e56  T_INLINE_SSH_ENV
-00002660: 2e0a 2020 2020 2020 2020 2020 2020 736c  ..            sl
-00002670: 7572 6d5f 6461 7461 5f70 6174 6820 2873  urm_data_path (s
-00002680: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-00002690: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
-000026a0: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
-000026b0: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
-000026c0: 696e 6720 7468 6520 6461 7461 2066 696c  ing the data fil
-000026d0: 6573 2066 6f72 2053 6c75 726d 206a 6f62  es for Slurm job
-000026e0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-000026f0: 2020 2044 6566 6175 6c74 7320 746f 205f     Defaults to _
-00002700: 4445 4641 554c 545f 534c 5552 4d5f 4441  DEFAULT_SLURM_DA
-00002710: 5441 5f50 4154 482e 0a20 2020 2020 2020  TA_PATH..       
-00002720: 2020 2020 2073 6c75 726d 5f69 6d61 6765       slurm_image
-00002730: 735f 7061 7468 2028 7374 722c 206f 7074  s_path (str, opt
-00002740: 696f 6e61 6c29 3a20 5468 6520 7061 7468  ional): The path
-00002750: 2074 6f20 7468 6520 6469 7265 6374 6f72   to the director
-00002760: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00002770: 2020 636f 6e74 6169 6e69 6e67 2074 6865    containing the
-00002780: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
-00002790: 6765 7320 666f 7220 536c 7572 6d20 6a6f  ges for Slurm jo
-000027a0: 6273 2e0a 2020 2020 2020 2020 2020 2020  bs..            
-000027b0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-000027c0: 5f44 4546 4155 4c54 5f53 4c55 524d 5f49  _DEFAULT_SLURM_I
-000027d0: 4d41 4745 535f 5041 5448 2e0a 2020 2020  MAGES_PATH..    
-000027e0: 2020 2020 2020 2020 736c 7572 6d5f 636f          slurm_co
-000027f0: 6e76 6572 7465 7273 5f70 6174 6820 2873  nverters_path (s
-00002800: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-00002810: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
-00002820: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
-00002830: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
-00002840: 696e 6720 7468 6520 5369 6e67 756c 6172  ing the Singular
-00002850: 6974 7920 696d 6167 6573 2066 6f72 2066  ity images for f
-00002860: 696c 6520 636f 6e76 6572 7465 7273 2e0a  ile converters..
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 4465 6661 756c 7473 2074 6f20 5f44 4546  Defaults to _DEF
-00002890: 4155 4c54 5f53 4c55 524d 5f43 4f4e 5645  AULT_SLURM_CONVE
-000028a0: 5254 4552 535f 5041 5448 2e0a 2020 2020  RTERS_PATH..    
-000028b0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-000028c0: 6465 6c5f 7061 7468 7320 2864 6963 742c  del_paths (dict,
-000028d0: 206f 7074 696f 6e61 6c29 3a20 4120 6469   optional): A di
-000028e0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-000028f0: 696e 6720 7468 6520 0a20 2020 2020 2020  ing the .       
-00002900: 2020 2020 2020 2020 2070 6174 6873 2074           paths t
-00002910: 6f20 7468 6520 5369 6e67 756c 6172 6974  o the Singularit
-00002920: 7920 696d 6167 6573 2066 6f72 2073 7065  y images for spe
-00002930: 6369 6669 6320 536c 7572 6d20 6a6f 6220  cific Slurm job 
-00002940: 6d6f 6465 6c73 2e0a 2020 2020 2020 2020  models..        
-00002950: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00002960: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
-00002970: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00002980: 6c5f 7265 706f 7320 2864 6963 742c 206f  l_repos (dict, o
-00002990: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
-000029a0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-000029b0: 6720 7468 6520 0a20 2020 2020 2020 2020  g the .         
-000029c0: 2020 2020 2020 2067 6974 2072 6570 6f73         git repos
-000029d0: 6974 6f72 6965 7320 6f66 2053 696e 6775  itories of Singu
-000029e0: 6c61 7269 7479 2069 6d61 6765 7320 666f  larity images fo
-000029f0: 7220 7370 6563 6966 6963 2053 6c75 726d  r specific Slurm
-00002a00: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002a10: 2020 6a6f 6220 6d6f 6465 6c73 2e0a 2020    job models..  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00002a30: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00002a40: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-00002a50: 6d5f 6d6f 6465 6c5f 696d 6167 6573 2028  m_model_images (
-00002a60: 6469 6374 2c20 6f70 7469 6f6e 616c 293a  dict, optional):
-00002a70: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
-00002a80: 6e74 6169 6e69 6e67 2074 6865 200a 2020  ntaining the .  
-00002a90: 2020 2020 2020 2020 2020 2020 2020 646f                do
-00002aa0: 636b 6572 6875 6220 6f66 2074 6865 2053  ckerhub of the S
-00002ab0: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
-00002ac0: 7320 666f 7220 7370 6563 6966 6963 2053  s for specific S
-00002ad0: 6c75 726d 200a 2020 2020 2020 2020 2020  lurm .          
-00002ae0: 2020 2020 2020 6a6f 6220 6d6f 6465 6c73        job models
-00002af0: 2e20 5769 6c6c 2066 696c 6c20 6175 746f  . Will fill auto
-00002b00: 6d61 7469 6361 6c6c 7920 6672 6f6d 2074  matically from t
-00002b10: 6865 2064 6174 6120 696e 2074 6865 2067  he data in the g
-00002b20: 6974 200a 2020 2020 2020 2020 2020 2020  it .            
-00002b30: 2020 2020 7265 706f 7369 746f 7279 2069      repository i
-00002b40: 6620 796f 7520 7365 7420 696e 6974 5f73  f you set init_s
-00002b50: 6c75 726d 2e0a 2020 2020 2020 2020 2020  lurm..          
-00002b60: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002b70: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00002b80: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00002b90: 6a6f 6273 2028 6469 6374 2c20 6f70 7469  jobs (dict, opti
-00002ba0: 6f6e 616c 293a 2041 2064 6963 7469 6f6e  onal): A diction
-00002bb0: 6172 7920 636f 6e74 6169 6e69 6e67 0a20  ary containing. 
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002bd0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00002be0: 2073 7065 6369 6669 6320 536c 7572 6d20   specific Slurm 
-00002bf0: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
-00002c00: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00002c10: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00002c20: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-00002c30: 6d6f 6465 6c5f 6a6f 6273 5f70 6172 616d  model_jobs_param
-00002c40: 7320 2864 6963 742c 206f 7074 696f 6e61  s (dict, optiona
-00002c50: 6c29 3a20 4120 6469 6374 696f 6e61 7279  l): A dictionary
-00002c60: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
-00002c70: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00002c80: 6d65 7465 7273 2066 6f72 2073 7065 6369  meters for speci
-00002c90: 6669 6320 536c 7572 6d20 6a6f 6220 6d6f  fic Slurm job mo
-00002ca0: 6465 6c73 2e0a 2020 2020 2020 2020 2020  dels..          
-00002cb0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002cc0: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00002cd0: 2020 2020 736c 7572 6d5f 7363 7269 7074      slurm_script
-00002ce0: 5f70 6174 6820 2873 7472 2c20 6f70 7469  _path (str, opti
-00002cf0: 6f6e 616c 293a 2054 6865 2070 6174 6820  onal): The path 
-00002d00: 746f 2074 6865 2064 6972 6563 746f 7279  to the directory
-00002d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d20: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00002d30: 536c 7572 6d20 6a6f 6220 7375 626d 6973  Slurm job submis
-00002d40: 7369 6f6e 2073 6372 6970 7473 206f 6e20  sion scripts on 
-00002d50: 536c 7572 6d2e 0a20 2020 2020 2020 2020  Slurm..         
-00002d60: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00002d70: 746f 205f 4445 4641 554c 545f 534c 5552  to _DEFAULT_SLUR
-00002d80: 4d5f 4749 545f 5343 5249 5054 5f50 4154  M_GIT_SCRIPT_PAT
-00002d90: 482e 0a20 2020 2020 2020 2020 2020 2073  H..            s
-00002da0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-00002db0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00002dc0: 3a20 5468 6520 6769 7420 6874 7470 7320  : The git https 
-00002dd0: 5552 4c20 666f 7220 636c 6f6e 696e 670a  URL for cloning.
-00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002df0: 7468 6520 7265 706f 2063 6f6e 7461 696e  the repo contain
-00002e00: 696e 6720 7468 6520 536c 7572 6d20 6a6f  ing the Slurm jo
-00002e10: 6220 7375 626d 6973 7369 6f6e 2073 6372  b submission scr
-00002e20: 6970 7473 2e0a 2020 2020 2020 2020 2020  ipts..          
-00002e30: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002e40: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00002e50: 2020 2020 696e 6974 5f73 6c75 726d 2028      init_slurm (
-00002e60: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
-00002e70: 6f20 7365 7420 7570 2074 6865 2072 6571  o set up the req
-00002e80: 7569 7265 6420 7374 7275 6374 7572 6573  uired structures
-00002e90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002ea0: 2020 6f6e 2053 6c75 726d 2061 6674 6572    on Slurm after
-00002eb0: 2069 6e69 7469 6174 696e 6720 7468 6973   initiating this
-00002ec0: 2063 6c69 656e 742e 2054 6869 7320 696e   client. This in
-00002ed0: 636c 7564 6573 2063 7265 6174 696e 6720  cludes creating 
-00002ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ef0: 206d 6973 7369 6e67 2066 6f6c 6465 7273   missing folders
-00002f00: 2c20 646f 776e 6c6f 6164 696e 6720 636f  , downloading co
-00002f10: 6e74 6169 6e65 7220 696d 6167 6573 2c20  ntainer images, 
-00002f20: 636c 6f6e 696e 6720 6769 742c 6574 632e  cloning git,etc.
-00002f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f40: 2054 6869 7320 7769 6c6c 2074 616b 6520   This will take 
-00002f50: 6120 7768 696c 6520 6174 2066 6972 7374  a while at first
-00002f60: 2062 7574 2077 696c 6c20 7661 6c69 6461   but will valida
-00002f70: 7465 2079 6f75 7220 7365 7475 702e 0a20  te your setup.. 
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00002f90: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00002fa0: 2074 6f20 7361 7665 2074 696d 652e 0a20   to save time.. 
-00002fb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002fc0: 2020 2073 7570 6572 2853 6c75 726d 436c     super(SlurmCl
-00002fd0: 6965 6e74 2c20 7365 6c66 292e 5f5f 696e  ient, self).__in
-00002fe0: 6974 5f5f 2868 6f73 742c 0a20 2020 2020  it__(host,.     
+000008b0: 7573 3a7b 706f 6c6c 5f72 6573 756c 742e  us:{poll_result.
+000008c0: 7374 6465 7272 7d22 290a 2020 2020 2020  stderr}").      
+000008d0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+000008e0: 6f62 5f73 7461 7465 203d 2022 4641 494c  ob_state = "FAIL
+000008f0: 4544 220a 2020 2020 2020 2020 2020 2020  ED".            
+00000900: 7365 6c66 2e6a 6f62 5f73 7461 7465 203d  self.job_state =
+00000910: 206a 6f62 5f73 7461 7475 735f 6469 6374   job_status_dict
+00000920: 5b73 656c 662e 6a6f 625f 6964 5d0a 2020  [self.job_id].  
+00000930: 2020 2020 2020 2020 2020 2320 7761 6974            # wait
+00000940: 2066 6f72 2031 3020 7365 636f 6e64 7320   for 10 seconds 
+00000950: 6265 666f 7265 2063 6865 636b 696e 6720  before checking 
+00000960: 6167 6169 6e0a 2020 2020 2020 2020 2020  again.          
+00000970: 2020 6f6d 6572 6f43 6f6e 6e2e 6b65 6570    omeroConn.keep
+00000980: 416c 6976 6528 2920 2023 206b 6565 7020  Alive()  # keep 
+00000990: 7468 6520 4f4d 4552 4f20 636f 6e6e 6563  the OMERO connec
+000009a0: 7469 6f6e 2061 6c69 7665 0a20 2020 2020  tion alive.     
+000009b0: 2020 2020 2020 2074 696d 6573 6c65 6570         timesleep
+000009c0: 2e73 6c65 6570 2831 3029 0a20 2020 2020  .sleep(10).     
+000009d0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+000009e0: 224a 6f62 207b 7365 6c66 2e6a 6f62 5f69  "Job {self.job_i
+000009f0: 647d 2066 696e 6973 6865 643a 207b 7365  d} finished: {se
+00000a00: 6c66 2e6a 6f62 5f73 7461 7465 7d22 290a  lf.job_state}").
+00000a10: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00000a20: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00000a30: 2066 2259 6f75 2063 616e 2067 6574 2074   f"You can get t
+00000a40: 6865 206c 6f67 6669 6c65 2075 7369 6e67  he logfile using
+00000a50: 2060 536c 7572 6d20 4765 7420 5570 6461   `Slurm Get Upda
+00000a60: 7465 6020 6f6e 206a 6f62 207b 7365 6c66  te` on job {self
+00000a70: 2e6a 6f62 5f69 647d 2229 0a20 2020 2020  .job_id}").     
+00000a80: 2020 2072 6574 7572 6e20 7365 6c66 2e6a     return self.j
+00000a90: 6f62 5f73 7461 7465 0a0a 2020 2020 6465  ob_state..    de
+00000aa0: 6620 636f 6d70 6c65 7465 6428 7365 6c66  f completed(self
+00000ab0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00000ac0: 2020 2020 2020 2043 6865 636b 2069 6620         Check if 
+00000ad0: 7468 6520 536c 7572 6d20 6a6f 6220 6861  the Slurm job ha
+00000ae0: 7320 636f 6d70 6c65 7465 6420 7375 6363  s completed succ
+00000af0: 6573 7366 756c 6c79 2e0a 0a20 2020 2020  essfully...     
+00000b00: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00000b10: 2020 2020 2020 2020 626f 6f6c 3a20 5472          bool: Tr
+00000b20: 7565 2069 6620 7468 6520 6a6f 6220 6861  ue if the job ha
+00000b30: 7320 636f 6d70 6c65 7465 643b 2046 616c  s completed; Fal
+00000b40: 7365 206f 7468 6572 7769 7365 2e0a 2020  se otherwise..  
+00000b50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000b60: 2020 7265 7475 726e 2073 656c 662e 6a6f    return self.jo
+00000b70: 625f 7374 6174 6520 3d3d 2022 434f 4d50  b_state == "COMP
+00000b80: 4c45 5445 4422 0a0a 2020 2020 6465 6620  LETED"..    def 
+00000b90: 5f5f 7374 725f 5f28 7365 6c66 293a 0a20  __str__(self):. 
+00000ba0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000bb0: 2020 2052 6574 7572 6e20 6120 7374 7269     Return a stri
+00000bc0: 6e67 2072 6570 7265 7365 6e74 6174 696f  ng representatio
+00000bd0: 6e20 6f66 2074 6865 2053 6c75 726d 4a6f  n of the SlurmJo
+00000be0: 6220 696e 7374 616e 6365 2e0a 0a20 2020  b instance...   
+00000bf0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00000c00: 2020 2020 2020 2020 2020 7374 723a 2053            str: S
+00000c10: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
+00000c20: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
+00000c30: 220a 2020 2020 2020 2020 7072 6f70 6572  ".        proper
+00000c40: 7469 6573 203d 2027 2c20 272e 6a6f 696e  ties = ', '.join
+00000c50: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00000c60: 7b6b 6579 7d3d 7b76 616c 7565 7d22 2066  {key}={value}" f
+00000c70: 6f72 206b 6579 2c20 7661 6c75 6520 696e  or key, value in
+00000c80: 2073 656c 662e 5f5f 6469 6374 5f5f 2e69   self.__dict__.i
+00000c90: 7465 6d73 2829 290a 2020 2020 2020 2020  tems()).        
+00000ca0: 7265 7475 726e 2066 2253 6c75 726d 4a6f  return f"SlurmJo
+00000cb0: 6228 7b70 726f 7065 7274 6965 737d 2922  b({properties})"
+00000cc0: 0a0a 0a63 6c61 7373 2053 6c75 726d 436c  ...class SlurmCl
+00000cd0: 6965 6e74 2843 6f6e 6e65 6374 696f 6e29  ient(Connection)
+00000ce0: 3a0a 2020 2020 2222 2241 2063 6c69 656e  :.    """A clien
+00000cf0: 7420 666f 7220 636f 6e6e 6563 7469 6e67  t for connecting
+00000d00: 2074 6f20 616e 6420 696e 7465 7261 6374   to and interact
+00000d10: 696e 6720 7769 7468 2061 2053 6c75 726d  ing with a Slurm
+00000d20: 2063 6c75 7374 6572 206f 7665 720a 2020   cluster over.  
+00000d30: 2020 5353 482e 0a0a 2020 2020 5468 6973    SSH...    This
+00000d40: 2063 6c61 7373 2065 7874 656e 6473 2074   class extends t
+00000d50: 6865 2043 6f6e 6e65 6374 696f 6e20 636c  he Connection cl
+00000d60: 6173 732c 2061 6464 696e 6720 6d65 7468  ass, adding meth
+00000d70: 6f64 7320 616e 640a 2020 2020 6174 7472  ods and.    attr
+00000d80: 6962 7574 6573 2073 7065 6369 6669 6320  ibutes specific 
+00000d90: 746f 2077 6f72 6b69 6e67 2077 6974 6820  to working with 
+00000da0: 536c 7572 6d2e 0a0a 2020 2020 536c 7572  Slurm...    Slur
+00000db0: 6d43 6c69 656e 7420 6163 6365 7074 7320  mClient accepts 
+00000dc0: 7468 6520 7361 6d65 2061 7267 756d 656e  the same argumen
+00000dd0: 7473 2061 7320 436f 6e6e 6563 7469 6f6e  ts as Connection
+00000de0: 2e20 4265 6c6f 7720 6f6e 6c79 0a20 2020  . Below only.   
+00000df0: 206d 656e 7469 6f6e 7320 7468 6520 6164   mentions the ad
+00000e00: 6465 6420 6f6e 6573 3a0a 0a20 2020 2054  ded ones:..    T
+00000e10: 6865 2065 6173 6965 7374 2077 6179 2074  he easiest way t
+00000e20: 6f20 7365 7420 7468 6973 2063 6c69 656e  o set this clien
+00000e30: 7420 7570 2069 7320 6279 2075 7369 6e67  t up is by using
+00000e40: 2061 2073 6c75 726d 2d63 6f6e 6669 672e   a slurm-config.
+00000e50: 696e 690a 2020 2020 616e 6420 7468 6520  ini.    and the 
+00000e60: 6672 6f6d 2d63 6f6e 6669 6728 2920 6d65  from-config() me
+00000e70: 7468 6f64 2e0a 0a20 2020 2041 7474 7269  thod...    Attri
+00000e80: 6275 7465 733a 0a20 2020 2020 2020 2073  butes:.        s
+00000e90: 6c75 726d 5f64 6174 615f 7061 7468 2028  lurm_data_path (
+00000ea0: 7374 7229 3a20 5468 6520 7061 7468 2074  str): The path t
+00000eb0: 6f20 7468 6520 6469 7265 6374 6f72 7920  o the directory 
+00000ec0: 636f 6e74 6169 6e69 6e67 2074 6865 0a20  containing the. 
+00000ed0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00000ee0: 6669 6c65 7320 666f 7220 536c 7572 6d20  files for Slurm 
+00000ef0: 6a6f 6273 2e0a 2020 2020 2020 2020 736c  jobs..        sl
+00000f00: 7572 6d5f 696d 6167 6573 5f70 6174 6820  urm_images_path 
+00000f10: 2873 7472 293a 2054 6865 2070 6174 6820  (str): The path 
+00000f20: 746f 2074 6865 2064 6972 6563 746f 7279  to the directory
+00000f30: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
+00000f40: 2020 2020 2020 2020 7468 6520 5369 6e67          the Sing
+00000f50: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
+00000f60: 6f72 2053 6c75 726d 206a 6f62 732e 0a20  or Slurm jobs.. 
+00000f70: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
+00000f80: 7665 7274 6572 735f 7061 7468 2028 7374  verters_path (st
+00000f90: 7229 3a20 5468 6520 7061 7468 2074 6f20  r): The path to 
+00000fa0: 7468 6520 6469 7265 6374 6f72 7920 636f  the directory co
+00000fb0: 6e74 6169 6e69 6e67 0a20 2020 2020 2020  ntaining.       
+00000fc0: 2020 2020 2074 6865 2053 696e 6775 6c61       the Singula
+00000fd0: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
+00000fe0: 6669 6c65 2063 6f6e 7665 7274 6572 732e  file converters.
+00000ff0: 0a20 2020 2020 2020 2073 6c75 726d 5f6d  .        slurm_m
+00001000: 6f64 656c 5f70 6174 6873 2028 6469 6374  odel_paths (dict
+00001010: 293a 2041 2064 6963 7469 6f6e 6172 7920  ): A dictionary 
+00001020: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
+00001030: 6174 6873 2074 6f0a 2020 2020 2020 2020  aths to.        
+00001040: 2020 2020 7468 6520 5369 6e67 756c 6172      the Singular
+00001050: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
+00001060: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
+00001070: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
+00001080: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7265    slurm_model_re
+00001090: 706f 7320 2864 6963 7429 3a20 4120 6469  pos (dict): A di
+000010a0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+000010b0: 696e 6720 7468 6520 6769 740a 2020 2020  ing the git.    
+000010c0: 2020 2020 2020 2020 7265 706f 7369 746f          reposito
+000010d0: 7269 6573 206f 6620 5369 6e67 756c 6172  ries of Singular
+000010e0: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
+000010f0: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
+00001100: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
+00001110: 2020 736c 7572 6d5f 6d6f 6465 6c5f 696d    slurm_model_im
+00001120: 6167 6573 2028 6469 6374 293a 2041 2064  ages (dict): A d
+00001130: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+00001140: 6e69 6e67 2074 6865 2064 6f63 6b65 7268  ning the dockerh
+00001150: 7562 0a20 2020 2020 2020 2020 2020 206f  ub.            o
+00001160: 6620 7468 6520 5369 6e67 756c 6172 6974  f the Singularit
+00001170: 7920 696d 6167 6573 2066 6f72 2073 7065  y images for spe
+00001180: 6369 6669 6320 536c 7572 6d20 6a6f 6220  cific Slurm job 
+00001190: 6d6f 6465 6c73 2e0a 2020 2020 2020 2020  models..        
+000011a0: 2020 2020 5769 6c6c 2066 696c 6c20 6175      Will fill au
+000011b0: 746f 6d61 7469 6361 6c6c 7920 6672 6f6d  tomatically from
+000011c0: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
+000011d0: 2067 6974 2072 6570 6f73 6974 6f72 792c   git repository,
+000011e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000011f0: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
+00001200: 726d 2e0a 2020 2020 2020 2020 736c 7572  rm..        slur
+00001210: 6d5f 7363 7269 7074 5f70 6174 6820 2873  m_script_path (s
+00001220: 7472 293a 2054 6865 2070 6174 6820 746f  tr): The path to
+00001230: 2074 6865 2064 6972 6563 746f 7279 2063   the directory c
+00001240: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
+00001250: 2020 2020 2020 7468 6520 536c 7572 6d20        the Slurm 
+00001260: 6a6f 6220 7375 626d 6973 7369 6f6e 2073  job submission s
+00001270: 6372 6970 7473 206f 6e20 536c 7572 6d2e  cripts on Slurm.
+00001280: 0a20 2020 2020 2020 2073 6c75 726d 5f73  .        slurm_s
+00001290: 6372 6970 745f 7265 706f 2028 7374 7229  cript_repo (str)
+000012a0: 3a20 5468 6520 6769 7420 6874 7470 7320  : The git https 
+000012b0: 5552 4c20 666f 7220 636c 6f6e 696e 6720  URL for cloning 
+000012c0: 7468 6520 7265 706f 0a20 2020 2020 2020  the repo.       
+000012d0: 2020 2020 2063 6f6e 7461 696e 696e 6720       containing 
+000012e0: 7468 6520 536c 7572 6d20 6a6f 6220 7375  the Slurm job su
+000012f0: 626d 6973 7369 6f6e 2073 6372 6970 7473  bmission scripts
+00001300: 2e20 4f70 7469 6f6e 616c 2e0a 0a20 2020  . Optional...   
+00001310: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00001320: 2020 2320 4372 6561 7465 2061 2053 6c75    # Create a Slu
+00001330: 726d 436c 6965 6e74 206f 626a 6563 7420  rmClient object 
+00001340: 6173 2063 6f6e 7465 7874 6d61 6e61 6765  as contextmanage
+00001350: 720a 0a20 2020 2020 2020 2077 6974 6820  r..        with 
+00001360: 536c 7572 6d43 6c69 656e 742e 6672 6f6d  SlurmClient.from
+00001370: 5f63 6f6e 6669 6728 2920 6173 2063 6c69  _config() as cli
+00001380: 656e 743a 0a0a 2020 2020 2020 2020 2020  ent:..          
+00001390: 2020 2320 5275 6e20 6120 636f 6d6d 616e    # Run a comman
+000013a0: 6420 6f6e 2074 6865 2072 656d 6f74 6520  d on the remote 
+000013b0: 686f 7374 0a0a 2020 2020 2020 2020 2020  host..          
+000013c0: 2020 7265 7375 6c74 203d 2063 6c69 656e    result = clien
+000013d0: 742e 7275 6e28 2773 6261 7463 6820 6d79  t.run('sbatch my
+000013e0: 6a6f 622e 7368 2729 0a0a 2020 2020 2020  job.sh')..      
+000013f0: 2020 2020 2020 2320 4368 6563 6b20 7768        # Check wh
+00001400: 6574 6865 7220 7468 6520 636f 6d6d 616e  ether the comman
+00001410: 6420 7375 6363 6565 6465 640a 0a20 2020  d succeeded..   
+00001420: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
+00001430: 6c74 2e6f 6b3a 0a20 2020 2020 2020 2020  lt.ok:.         
+00001440: 2020 2020 2020 2070 7269 6e74 2827 4a6f         print('Jo
+00001450: 6220 7375 626d 6974 7465 6420 7375 6363  b submitted succ
+00001460: 6573 7366 756c 6c79 2127 290a 0a20 2020  essfully!')..   
+00001470: 2020 2020 2020 2020 2023 2050 7269 6e74           # Print
+00001480: 2074 6865 206f 7574 7075 7420 6f66 2074   the output of t
+00001490: 6865 2063 6f6d 6d61 6e64 0a0a 2020 2020  he command..    
+000014a0: 2020 2020 2020 2020 7072 696e 7428 7265          print(re
+000014b0: 7375 6c74 2e73 7464 6f75 7429 0a0a 2020  sult.stdout)..  
+000014c0: 2020 4578 616d 706c 6520 323a 0a20 2020    Example 2:.   
+000014d0: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
+000014e0: 536c 7572 6d43 6c69 656e 7420 616e 6420  SlurmClient and 
+000014f0: 7365 7475 7020 536c 7572 6d20 2864 6f77  setup Slurm (dow
+00001500: 6e6c 6f61 6420 636f 6e74 6169 6e65 7273  nload containers
+00001510: 2065 7463 2e29 0a0a 2020 2020 2020 2020   etc.)..        
+00001520: 7769 7468 2053 6c75 726d 436c 6965 6e74  with SlurmClient
+00001530: 2e66 726f 6d5f 636f 6e66 6967 2869 6e69  .from_config(ini
+00001540: 745f 736c 7572 6d3d 5472 7565 2920 6173  t_slurm=True) as
+00001550: 2063 6c69 656e 743a 0a0a 2020 2020 2020   client:..      
+00001560: 2020 2020 2020 636c 6965 6e74 2e72 756e        client.run
+00001570: 5f77 6f72 6b66 6c6f 7728 2e2e 2e29 0a0a  _workflow(...)..
+00001580: 2020 2020 2222 220a 2020 2020 5f44 4546      """.    _DEF
+00001590: 4155 4c54 5f43 4f4e 4649 475f 5041 5448  AULT_CONFIG_PATH
+000015a0: 5f31 203d 2022 2f65 7463 2f73 6c75 726d  _1 = "/etc/slurm
+000015b0: 2d63 6f6e 6669 672e 696e 6922 0a20 2020  -config.ini".   
+000015c0: 205f 4445 4641 554c 545f 434f 4e46 4947   _DEFAULT_CONFIG
+000015d0: 5f50 4154 485f 3220 3d20 227e 2f73 6c75  _PATH_2 = "~/slu
+000015e0: 726d 2d63 6f6e 6669 672e 696e 6922 0a20  rm-config.ini". 
+000015f0: 2020 205f 4445 4641 554c 545f 484f 5354     _DEFAULT_HOST
+00001600: 203d 2022 736c 7572 6d22 0a20 2020 205f   = "slurm".    _
+00001610: 4445 4641 554c 545f 494e 4c49 4e45 5f53  DEFAULT_INLINE_S
+00001620: 5348 5f45 4e56 203d 2054 7275 650a 2020  SH_ENV = True.  
+00001630: 2020 5f44 4546 4155 4c54 5f53 4c55 524d    _DEFAULT_SLURM
+00001640: 5f44 4154 415f 5041 5448 203d 2022 6d79  _DATA_PATH = "my
+00001650: 2d73 6372 6174 6368 2f64 6174 6122 0a20  -scratch/data". 
+00001660: 2020 205f 4445 4641 554c 545f 534c 5552     _DEFAULT_SLUR
+00001670: 4d5f 494d 4147 4553 5f50 4154 4820 3d20  M_IMAGES_PATH = 
+00001680: 226d 792d 7363 7261 7463 682f 7369 6e67  "my-scratch/sing
+00001690: 756c 6172 6974 795f 696d 6167 6573 2f77  ularity_images/w
+000016a0: 6f72 6b66 6c6f 7773 220a 2020 2020 5f44  orkflows".    _D
+000016b0: 4546 4155 4c54 5f53 4c55 524d 5f43 4f4e  EFAULT_SLURM_CON
+000016c0: 5645 5254 4552 535f 5041 5448 203d 2022  VERTERS_PATH = "
+000016d0: 6d79 2d73 6372 6174 6368 2f73 696e 6775  my-scratch/singu
+000016e0: 6c61 7269 7479 5f69 6d61 6765 732f 636f  larity_images/co
+000016f0: 6e76 6572 7465 7273 220a 2020 2020 5f44  nverters".    _D
+00001700: 4546 4155 4c54 5f53 4c55 524d 5f47 4954  EFAULT_SLURM_GIT
+00001710: 5f53 4352 4950 545f 5041 5448 203d 2022  _SCRIPT_PATH = "
+00001720: 736c 7572 6d2d 7363 7269 7074 7322 0a20  slurm-scripts". 
+00001730: 2020 205f 4f55 545f 5345 5020 3d20 222d     _OUT_SEP = "-
+00001740: 2d73 706c 6974 2d2d 220a 2020 2020 5f56  -split--".    _V
+00001750: 4552 5349 4f4e 5f43 4d44 203d 2022 6c73  ERSION_CMD = "ls
+00001760: 202d 6820 7b73 6c75 726d 5f69 6d61 6765   -h {slurm_image
+00001770: 735f 7061 7468 7d2f 7b69 6d61 6765 5f70  s_path}/{image_p
+00001780: 6174 687d 207c 2067 7265 7020 2d6f 5020  ath} | grep -oP 
+00001790: 2728 3f3c 3d5c 2d7c 5c5f 2928 762e 2b7c  '(?<=\-|\_)(v.+|
+000017a0: 6c61 7465 7374 2928 3f3d 2e73 696d 677c  latest)(?=.simg|
+000017b0: 2e73 6966 2927 220a 2020 2020 2320 4e6f  .sif)'".    # No
+000017c0: 7465 2c20 6772 6570 2072 6574 7572 6e73  te, grep returns
+000017d0: 2065 7869 7463 6f64 6520 3120 6966 206e   exitcode 1 if n
+000017e0: 6f20 6d61 7463 6820 6973 2066 6f75 6e64  o match is found
+000017f0: 210a 2020 2020 2320 5468 6973 2077 696c  !.    # This wil
+00001800: 6c20 7472 616e 736c 6174 6520 696e 746f  l translate into
+00001810: 2061 2055 6e65 7870 6563 7465 6445 7869   a UnexpectedExi
+00001820: 7420 6572 726f 722c 2073 6f20 6d75 7465  t error, so mute
+00001830: 2074 6861 7420 6966 2079 6f75 0a20 2020   that if you.   
+00001840: 2023 2064 6f6e 2774 2063 6172 6520 6162   # don't care ab
+00001850: 6f75 7420 656d 7074 792e 0a20 2020 2023  out empty..    #
+00001860: 204c 696b 6520 6265 6c6f 7720 7769 7468   Like below with
+00001870: 2074 6865 2022 7c7c 203a 222e 0a20 2020   the "|| :"..   
+00001880: 2023 2044 6174 6120 636f 756c 6420 6c65   # Data could le
+00001890: 6769 7420 6265 2065 6d70 7479 2e0a 2020  git be empty..  
+000018a0: 2020 5f44 4154 415f 434d 4420 3d20 226c    _DATA_CMD = "l
+000018b0: 7320 2d68 207b 736c 7572 6d5f 6461 7461  s -h {slurm_data
+000018c0: 5f70 6174 687d 207c 2067 7265 7020 2d6f  _path} | grep -o
+000018d0: 5020 272e 2b28 3f3d 2e7a 6970 2927 207c  P '.+(?=.zip)' |
+000018e0: 7c20 3a22 0a20 2020 205f 414c 4c5f 4a4f  | :".    _ALL_JO
+000018f0: 4253 5f43 4d44 203d 2022 7361 6363 7420  BS_CMD = "sacct 
+00001900: 2d2d 7374 6172 7474 696d 6520 7b73 7461  --starttime {sta
+00001910: 7274 5f74 696d 657d 202d 2d65 6e64 7469  rt_time} --endti
+00001920: 6d65 207b 656e 645f 7469 6d65 7d20 2d2d  me {end_time} --
+00001930: 7374 6174 6520 7b73 7461 7465 737d 202d  state {states} -
+00001940: 6f20 7b63 6f6c 756d 6e73 7d20 2d6e 202d  o {columns} -n -
+00001950: 5820 220a 2020 2020 5f5a 4950 5f43 4d44  X ".    _ZIP_CMD
+00001960: 203d 2022 377a 2061 202d 7920 7b66 696c   = "7z a -y {fil
+00001970: 656e 616d 657d 202d 747a 6970 207b 6461  ename} -tzip {da
+00001980: 7461 5f6c 6f63 6174 696f 6e7d 2f64 6174  ta_location}/dat
+00001990: 612f 6f75 7422 0a20 2020 205f 4143 5449  a/out".    _ACTI
+000019a0: 5645 5f4a 4f42 535f 434d 4420 3d20 2273  VE_JOBS_CMD = "s
+000019b0: 7175 6575 6520 2d75 2024 5553 4552 202d  queue -u $USER -
+000019c0: 2d6e 6f68 6561 6420 2d2d 666f 726d 6174  -nohead --format
+000019d0: 2025 4622 0a20 2020 205f 4a4f 425f 5354   %F".    _JOB_ST
+000019e0: 4154 5553 5f43 4d44 203d 2022 7361 6363  ATUS_CMD = "sacc
+000019f0: 7420 2d6e 202d 6f20 4a6f 6249 642c 5374  t -n -o JobId,St
+00001a00: 6174 652c 456e 6420 2d58 202d 6a20 7b73  ate,End -X -j {s
+00001a10: 6c75 726d 5f6a 6f62 5f69 647d 220a 2020  lurm_job_id}".  
+00001a20: 2020 2320 544f 444f 206d 6f76 6520 616c    # TODO move al
+00001a30: 6c20 636f 6d6d 616e 6473 2074 6f20 6120  l commands to a 
+00001a40: 7369 6d69 6c61 7220 666f 726d 6174 2e0a  similar format..
+00001a50: 2020 2020 2320 5468 656e 206d 6179 6265      # Then maybe
+00001a60: 2061 6c6c 6f77 206f 7665 7277 7269 7465   allow overwrite
+00001a70: 2066 726f 6d20 736c 7572 6d2d 636f 6e66   from slurm-conf
+00001a80: 6967 2e69 6e69 0a20 2020 205f 4c4f 4746  ig.ini.    _LOGF
+00001a90: 494c 4520 3d20 226f 6d65 726f 2d7b 736c  ILE = "omero-{sl
+00001aa0: 7572 6d5f 6a6f 625f 6964 7d2e 6c6f 6722  urm_job_id}.log"
+00001ab0: 0a20 2020 205f 5441 494c 5f4c 4f47 5f43  .    _TAIL_LOG_C
+00001ac0: 4d44 203d 2022 7461 696c 202d 6e20 7b6e  MD = "tail -n {n
+00001ad0: 7d20 7b6c 6f67 5f66 696c 657d 207c 2073  } {log_file} | s
+00001ae0: 7472 696e 6773 220a 2020 2020 5f4c 4f47  trings".    _LOG
+00001af0: 4649 4c45 5f44 4154 415f 434d 4420 3d20  FILE_DATA_CMD = 
+00001b00: 2263 6174 207b 6c6f 675f 6669 6c65 7d20  "cat {log_file} 
+00001b10: 7c20 7065 726c 202d 776e 6520 272f 5275  | perl -wne '/Ru
+00001b20: 6e6e 696e 6720 5b5c 772d 5d2b 3f20 4a6f  nning [\w-]+? Jo
+00001b30: 6220 775c 2f20 2e2b 3f20 5c7c 202e 2b3f  b w\/ .+? \| .+?
+00001b40: 205c 7c20 282e 2b3f 2920 5c7c 2e2a 2f69   \| (.+?) \|.*/i
+00001b50: 2061 6e64 2070 7269 6e74 2431 2722 0a0a   and print$1'"..
+00001b60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001b70: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+00001b80: 2020 2020 2020 2020 686f 7374 3d5f 4445          host=_DE
+00001b90: 4641 554c 545f 484f 5354 2c0a 2020 2020  FAULT_HOST,.    
+00001ba0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00001bb0: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
+00001bc0: 2020 2020 2020 2020 2070 6f72 743d 4e6f           port=No
+00001bd0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001be0: 2020 2020 2063 6f6e 6669 673d 4e6f 6e65       config=None
+00001bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001c00: 2020 2067 6174 6577 6179 3d4e 6f6e 652c     gateway=None,
+00001c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c20: 2020 666f 7277 6172 645f 6167 656e 743d    forward_agent=
+00001c30: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001c40: 2020 2020 2020 2063 6f6e 6e65 6374 5f74         connect_t
+00001c50: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
+00001c60: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001c70: 6e6e 6563 745f 6b77 6172 6773 3d4e 6f6e  nnect_kwargs=Non
+00001c80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001c90: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
+00001ca0: 6e76 3d5f 4445 4641 554c 545f 494e 4c49  nv=_DEFAULT_INLI
+00001cb0: 4e45 5f53 5348 5f45 4e56 2c0a 2020 2020  NE_SSH_ENV,.    
+00001cc0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00001cd0: 726d 5f64 6174 615f 7061 7468 3a20 7374  rm_data_path: st
+00001ce0: 7220 3d20 5f44 4546 4155 4c54 5f53 4c55  r = _DEFAULT_SLU
+00001cf0: 524d 5f44 4154 415f 5041 5448 2c0a 2020  RM_DATA_PATH,.  
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001d10: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+00001d20: 3a20 7374 7220 3d20 5f44 4546 4155 4c54  : str = _DEFAULT
+00001d30: 5f53 4c55 524d 5f49 4d41 4745 535f 5041  _SLURM_IMAGES_PA
+00001d40: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
+00001d50: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
+00001d60: 7274 6572 735f 7061 7468 3a20 7374 7220  rters_path: str 
+00001d70: 3d20 5f44 4546 4155 4c54 5f53 4c55 524d  = _DEFAULT_SLURM
+00001d80: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
+00001d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001da0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00001db0: 6174 6873 3a20 6469 6374 203d 204e 6f6e  aths: dict = Non
+00001dc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001dd0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00001de0: 7265 706f 733a 2064 6963 7420 3d20 4e6f  repos: dict = No
+00001df0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001e00: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+00001e10: 5f69 6d61 6765 733a 2064 6963 7420 3d20  _images: dict = 
+00001e20: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001e30: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00001e40: 656c 5f6a 6f62 733a 2064 6963 7420 3d20  el_jobs: dict = 
+00001e50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001e60: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00001e70: 656c 5f6a 6f62 735f 7061 7261 6d73 3a20  el_jobs_params: 
+00001e80: 6469 6374 203d 204e 6f6e 652c 0a20 2020  dict = None,.   
+00001e90: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00001ea0: 7572 6d5f 7363 7269 7074 5f70 6174 683a  urm_script_path:
+00001eb0: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
+00001ec0: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
+00001ed0: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
+00001ee0: 2020 2020 2020 2020 736c 7572 6d5f 7363          slurm_sc
+00001ef0: 7269 7074 5f72 6570 6f3a 2073 7472 203d  ript_repo: str =
+00001f00: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00001f10: 2020 2020 2020 2020 696e 6974 5f73 6c75          init_slu
+00001f20: 726d 3a20 626f 6f6c 203d 2046 616c 7365  rm: bool = False
+00001f30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001f40: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00001f50: 2249 6e69 7469 616c 697a 6573 2061 206e  "Initializes a n
+00001f60: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
+00001f70: 6865 2053 6c75 726d 436c 6965 6e74 2063  he SlurmClient c
+00001f80: 6c61 7373 2e0a 0a20 2020 2020 2020 2049  lass...        I
+00001f90: 7420 6973 2070 7265 6665 7261 626c 6520  t is preferable 
+00001fa0: 746f 2075 7365 2023 6672 6f6d 5f63 6f6e  to use #from_con
+00001fb0: 6669 6728 2e2e 2e29 206d 6574 686f 6420  fig(...) method 
+00001fc0: 746f 2069 6e69 7469 616c 697a 650a 2020  to initialize.  
+00001fd0: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
+00001fe0: 2066 726f 6d20 6120 636f 6e66 6967 2066   from a config f
+00001ff0: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
+00002000: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002010: 686f 7374 2028 7374 722c 206f 7074 696f  host (str, optio
+00002020: 6e61 6c29 3a20 5468 6520 686f 7374 6e61  nal): The hostna
+00002030: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
+00002040: 206f 6620 7468 6520 7265 6d6f 7465 0a20   of the remote. 
+00002050: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002060: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
+00002070: 746f 205f 4445 4641 554c 545f 484f 5354  to _DEFAULT_HOST
+00002080: 2e0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+00002090: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
+000020a0: 6c29 3a20 5468 6520 7573 6572 6e61 6d65  l): The username
+000020b0: 2074 6f20 7573 6520 7768 656e 2063 6f6e   to use when con
+000020c0: 6e65 6374 696e 6720 746f 200a 2020 2020  necting to .    
+000020d0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+000020e0: 7265 6d6f 7465 2073 6572 7665 722e 2044  remote server. D
+000020f0: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
+00002100: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
+00002110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002120: 2074 6f20 636f 6e66 6967 2e75 7365 722e   to config.user.
+00002130: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
+00002140: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
+00002150: 293a 2054 6865 2053 5348 2070 6f72 7420  ): The SSH port 
+00002160: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
+00002170: 6563 7469 6e67 2e0a 2020 2020 2020 2020  ecting..        
+00002180: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00002190: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
+000021a0: 6465 6661 756c 7473 2074 6f20 636f 6e66  defaults to conf
+000021b0: 6967 2e70 6f72 742e 0a20 2020 2020 2020  ig.port..       
+000021c0: 2020 2020 2063 6f6e 6669 6720 2873 7472       config (str
+000021d0: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
+000021e0: 6820 746f 2074 6865 2053 5348 2063 6f6e  h to the SSH con
+000021f0: 6669 6720 6669 6c65 2e0a 2020 2020 2020  fig file..      
+00002200: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00002210: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
+00002220: 6820 6465 6661 756c 7473 2074 6f20 796f  h defaults to yo
+00002230: 7572 2053 5348 2063 6f6e 6669 6720 6669  ur SSH config fi
+00002240: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+00002250: 6761 7465 7761 7920 2843 6f6e 6e65 6374  gateway (Connect
+00002260: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+00002270: 416e 206f 7074 696f 6e61 6c20 6761 7465  An optional gate
+00002280: 7761 7920 666f 7220 636f 6e6e 6563 7469  way for connecti
+00002290: 6e67 200a 2020 2020 2020 2020 2020 2020  ng .            
+000022a0: 2020 2020 7468 726f 7567 6820 6120 6a75      through a ju
+000022b0: 6d70 2068 6f73 742e 2044 6566 6175 6c74  mp host. Default
+000022c0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+000022d0: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
+000022e0: 6765 6e74 2028 626f 6f6c 2c20 6f70 7469  gent (bool, opti
+000022f0: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
+00002300: 6f20 666f 7277 6172 6420 7468 6520 6c6f  o forward the lo
+00002310: 6361 6c20 5353 4820 0a20 2020 2020 2020  cal SSH .       
+00002320: 2020 2020 2020 2020 2061 6765 6e74 2074           agent t
+00002330: 6f20 7468 6520 7265 6d6f 7465 2073 6572  o the remote ser
+00002340: 7665 722e 2044 6566 6175 6c74 7320 746f  ver. Defaults to
+00002350: 204e 6f6e 652c 2077 6869 6368 200a 2020   None, which .  
+00002360: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00002370: 6661 756c 7473 2074 6f20 636f 6e66 6967  faults to config
+00002380: 2e66 6f72 7761 7264 5f61 6765 6e74 2e0a  .forward_agent..
+00002390: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+000023a0: 6563 745f 7469 6d65 6f75 7420 2869 6e74  ect_timeout (int
+000023b0: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
+000023c0: 656f 7574 2066 6f72 2065 7374 6162 6c69  eout for establi
+000023d0: 7368 696e 6720 7468 6520 5353 4820 0a20  shing the SSH . 
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000023f0: 6f6e 6e65 6374 696f 6e2e 2044 6566 6175  onnection. Defau
+00002400: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
+00002410: 6368 2064 6566 6175 6c74 7320 0a20 2020  ch defaults .   
+00002420: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
+00002430: 636f 6e66 6967 2e74 696d 656f 7574 732e  config.timeouts.
+00002440: 636f 6e6e 6563 742e 0a20 2020 2020 2020  connect..       
+00002450: 2020 2020 2063 6f6e 6e65 6374 5f6b 7761       connect_kwa
+00002460: 7267 7320 2864 6963 742c 206f 7074 696f  rgs (dict, optio
+00002470: 6e61 6c29 3a20 4164 6469 7469 6f6e 616c  nal): Additional
+00002480: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00002490: 7473 2066 6f72 200a 2020 2020 2020 2020  ts for .        
+000024a0: 2020 2020 2020 2020 7468 6520 756e 6465          the unde
+000024b0: 726c 7969 6e67 2053 5348 2063 6f6e 6e65  rlying SSH conne
+000024c0: 6374 696f 6e2e 2048 616e 6465 6420 7665  ction. Handed ve
+000024d0: 7262 6174 696d 2074 6f20 0a20 2020 2020  rbatim to .     
+000024e0: 2020 2020 2020 2020 2020 2060 5353 4843             `SSHC
+000024f0: 6c69 656e 742e 636f 6e6e 6563 7420 3c70  lient.connect <p
+00002500: 6172 616d 696b 6f2e 636c 6965 6e74 2e53  aramiko.client.S
+00002510: 5348 436c 6965 6e74 2e63 6f6e 6e65 6374  SHClient.connect
+00002520: 3e60 2e20 0a20 2020 2020 2020 2020 2020  >`. .           
+00002530: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00002540: 204e 6f6e 652e 200a 2020 2020 2020 2020   None. .        
+00002550: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
+00002560: 6e76 2028 626f 6f6c 2c20 6f70 7469 6f6e  nv (bool, option
+00002570: 616c 293a 2057 6865 7468 6572 2074 6f20  al): Whether to 
+00002580: 7573 6520 696e 6c69 6e65 2053 5348 0a20  use inline SSH. 
+00002590: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000025a0: 6e76 6972 6f6e 6d65 6e74 2e20 5468 6973  nvironment. This
+000025b0: 2069 7320 6e65 6365 7373 6172 7920 6966   is necessary if
+000025c0: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
+000025d0: 6572 2068 6173 200a 2020 2020 2020 2020  er has .        
+000025e0: 2020 2020 2020 2020 6120 7265 7374 7269          a restri
+000025f0: 6374 6564 2060 6041 6363 6570 7445 6e76  cted ``AcceptEnv
+00002600: 6060 2073 6574 7469 6e67 2028 7768 6963  `` setting (whic
+00002610: 6820 6973 2074 6865 2063 6f6d 6d6f 6e20  h is the common 
+00002620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002630: 2064 6566 6175 6c74 292e 2044 6566 6175   default). Defau
+00002640: 6c74 7320 746f 205f 4445 4641 554c 545f  lts to _DEFAULT_
+00002650: 494e 4c49 4e45 5f53 5348 5f45 4e56 2e0a  INLINE_SSH_ENV..
+00002660: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00002670: 6d5f 6461 7461 5f70 6174 6820 2873 7472  m_data_path (str
+00002680: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00002690: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+000026a0: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+000026b0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+000026c0: 6720 7468 6520 6461 7461 2066 696c 6573  g the data files
+000026d0: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
+000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026f0: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
+00002700: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
+00002710: 5f50 4154 482e 0a20 2020 2020 2020 2020  _PATH..         
+00002720: 2020 2073 6c75 726d 5f69 6d61 6765 735f     slurm_images_
+00002730: 7061 7468 2028 7374 722c 206f 7074 696f  path (str, optio
+00002740: 6e61 6c29 3a20 5468 6520 7061 7468 2074  nal): The path t
+00002750: 6f20 7468 6520 6469 7265 6374 6f72 790a  o the directory.
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 636f 6e74 6169 6e69 6e67 2074 6865 2053  containing the S
+00002780: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
+00002790: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
+000027a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000027b0: 2020 4465 6661 756c 7473 2074 6f20 5f44    Defaults to _D
+000027c0: 4546 4155 4c54 5f53 4c55 524d 5f49 4d41  EFAULT_SLURM_IMA
+000027d0: 4745 535f 5041 5448 2e0a 2020 2020 2020  GES_PATH..      
+000027e0: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
+000027f0: 6572 7465 7273 5f70 6174 6820 2873 7472  erters_path (str
+00002800: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00002810: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00002820: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+00002830: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+00002840: 6720 7468 6520 5369 6e67 756c 6172 6974  g the Singularit
+00002850: 7920 696d 6167 6573 2066 6f72 2066 696c  y images for fil
+00002860: 6520 636f 6e76 6572 7465 7273 2e0a 2020  e converters..  
+00002870: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00002880: 6661 756c 7473 2074 6f20 5f44 4546 4155  faults to _DEFAU
+00002890: 4c54 5f53 4c55 524d 5f43 4f4e 5645 5254  LT_SLURM_CONVERT
+000028a0: 4552 535f 5041 5448 2e0a 2020 2020 2020  ERS_PATH..      
+000028b0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+000028c0: 6c5f 7061 7468 7320 2864 6963 742c 206f  l_paths (dict, o
+000028d0: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
+000028e0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+000028f0: 6720 7468 6520 0a20 2020 2020 2020 2020  g the .         
+00002900: 2020 2020 2020 2070 6174 6873 2074 6f20         paths to 
+00002910: 7468 6520 5369 6e67 756c 6172 6974 7920  the Singularity 
+00002920: 696d 6167 6573 2066 6f72 2073 7065 6369  images for speci
+00002930: 6669 6320 536c 7572 6d20 6a6f 6220 6d6f  fic Slurm job mo
+00002940: 6465 6c73 2e0a 2020 2020 2020 2020 2020  dels..          
+00002950: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00002960: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
+00002970: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00002980: 7265 706f 7320 2864 6963 742c 206f 7074  repos (dict, opt
+00002990: 696f 6e61 6c29 3a20 4120 6469 6374 696f  ional): A dictio
+000029a0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+000029b0: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
+000029c0: 2020 2020 2067 6974 2072 6570 6f73 6974       git reposit
+000029d0: 6f72 6965 7320 6f66 2053 696e 6775 6c61  ories of Singula
+000029e0: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
+000029f0: 7370 6563 6966 6963 2053 6c75 726d 200a  specific Slurm .
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
+00002a20: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00002a30: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00002a40: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+00002a50: 6d6f 6465 6c5f 696d 6167 6573 2028 6469  model_images (di
+00002a60: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
+00002a70: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
+00002a80: 6169 6e69 6e67 2074 6865 200a 2020 2020  aining the .    
+00002a90: 2020 2020 2020 2020 2020 2020 646f 636b              dock
+00002aa0: 6572 6875 6220 6f66 2074 6865 2053 696e  erhub of the Sin
+00002ab0: 6775 6c61 7269 7479 2069 6d61 6765 7320  gularity images 
+00002ac0: 666f 7220 7370 6563 6966 6963 2053 6c75  for specific Slu
+00002ad0: 726d 200a 2020 2020 2020 2020 2020 2020  rm .            
+00002ae0: 2020 2020 6a6f 6220 6d6f 6465 6c73 2e20      job models. 
+00002af0: 5769 6c6c 2066 696c 6c20 6175 746f 6d61  Will fill automa
+00002b00: 7469 6361 6c6c 7920 6672 6f6d 2074 6865  tically from the
+00002b10: 2064 6174 6120 696e 2074 6865 2067 6974   data in the git
+00002b20: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002b30: 2020 7265 706f 7369 746f 7279 2069 6620    repository if 
+00002b40: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
+00002b50: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
+00002b60: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002b70: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002b80: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00002b90: 6273 2028 6469 6374 2c20 6f70 7469 6f6e  bs (dict, option
+00002ba0: 616c 293a 2041 2064 6963 7469 6f6e 6172  al): A dictionar
+00002bb0: 7920 636f 6e74 6169 6e69 6e67 0a20 2020  y containing.   
+00002bc0: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00002bd0: 6f72 6d61 7469 6f6e 2061 626f 7574 2073  ormation about s
+00002be0: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
+00002bf0: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
+00002c00: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00002c10: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00002c20: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00002c30: 6465 6c5f 6a6f 6273 5f70 6172 616d 7320  del_jobs_params 
+00002c40: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
+00002c50: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
+00002c60: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
+00002c70: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00002c80: 7465 7273 2066 6f72 2073 7065 6369 6669  ters for specifi
+00002c90: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
+00002ca0: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+00002cb0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002cc0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002cd0: 2020 736c 7572 6d5f 7363 7269 7074 5f70    slurm_script_p
+00002ce0: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
+00002cf0: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
+00002d00: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002d20: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00002d30: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
+00002d40: 6f6e 2073 6372 6970 7473 206f 6e20 536c  on scripts on Sl
+00002d50: 7572 6d2e 0a20 2020 2020 2020 2020 2020  urm..           
+00002d60: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00002d70: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
+00002d80: 4749 545f 5343 5249 5054 5f50 4154 482e  GIT_SCRIPT_PATH.
+00002d90: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
+00002da0: 726d 5f73 6372 6970 745f 7265 706f 2028  rm_script_repo (
+00002db0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00002dc0: 5468 6520 6769 7420 6874 7470 7320 5552  The git https UR
+00002dd0: 4c20 666f 7220 636c 6f6e 696e 670a 2020  L for cloning.  
+00002de0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00002df0: 6520 7265 706f 2063 6f6e 7461 696e 696e  e repo containin
+00002e00: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
+00002e10: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
+00002e20: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00002e30: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002e40: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002e50: 2020 696e 6974 5f73 6c75 726d 2028 626f    init_slurm (bo
+00002e60: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00002e70: 7365 7420 7570 2074 6865 2072 6571 7569  set up the requi
+00002e80: 7265 6420 7374 7275 6374 7572 6573 200a  red structures .
+00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ea0: 6f6e 2053 6c75 726d 2061 6674 6572 2069  on Slurm after i
+00002eb0: 6e69 7469 6174 696e 6720 7468 6973 2063  nitiating this c
+00002ec0: 6c69 656e 742e 2054 6869 7320 696e 636c  lient. This incl
+00002ed0: 7564 6573 2063 7265 6174 696e 6720 0a20  udes creating . 
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00002ef0: 6973 7369 6e67 2066 6f6c 6465 7273 2c20  issing folders, 
+00002f00: 646f 776e 6c6f 6164 696e 6720 636f 6e74  downloading cont
+00002f10: 6169 6e65 7220 696d 6167 6573 2c20 636c  ainer images, cl
+00002f20: 6f6e 696e 6720 6769 742c 6574 632e 0a20  oning git,etc.. 
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00002f40: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
+00002f50: 7768 696c 6520 6174 2066 6972 7374 2062  while at first b
+00002f60: 7574 2077 696c 6c20 7661 6c69 6461 7465  ut will validate
+00002f70: 2079 6f75 7220 7365 7475 702e 0a20 2020   your setup..   
+00002f80: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00002f90: 6175 6c74 7320 746f 2046 616c 7365 2074  aults to False t
+00002fa0: 6f20 7361 7665 2074 696d 652e 0a20 2020  o save time..   
+00002fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002fc0: 2073 7570 6572 2853 6c75 726d 436c 6965   super(SlurmClie
+00002fd0: 6e74 2c20 7365 6c66 292e 5f5f 696e 6974  nt, self).__init
+00002fe0: 5f5f 2868 6f73 742c 0a20 2020 2020 2020  __(host,.       
 00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2075 7365 722c 0a20 2020 2020       user,.     
+00003010: 2020 2075 7365 722c 0a20 2020 2020 2020     user,.       
 00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2070 6f72 742c 0a20 2020 2020       port,.     
+00003040: 2020 2070 6f72 742c 0a20 2020 2020 2020     port,.       
 00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2020 2020 2063 6f6e 6669 672c 0a20 2020       config,.   
+00003070: 2020 2063 6f6e 6669 672c 0a20 2020 2020     config,.     
 00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 2020 2067 6174 6577 6179 2c0a         gateway,.
+000030a0: 2020 2020 2067 6174 6577 6179 2c0a 2020       gateway,.  
 000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 2020 2020 2020 666f 7277 6172            forwar
-000030e0: 645f 6167 656e 742c 0a20 2020 2020 2020  d_agent,.       
+000030d0: 2020 2020 2020 2020 666f 7277 6172 645f          forward_
+000030e0: 6167 656e 742c 0a20 2020 2020 2020 2020  agent,.         
 000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2063 6f6e 6e65 6374 5f74 696d 656f     connect_timeo
-00003120: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
+00003110: 2063 6f6e 6e65 6374 5f74 696d 656f 7574   connect_timeout
+00003120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00003150: 6e6e 6563 745f 6b77 6172 6773 2c0a 2020  nnect_kwargs,.  
+00003140: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00003150: 6563 745f 6b77 6172 6773 2c0a 2020 2020  ect_kwargs,.    
 00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 696e 6c69 6e65 5f73          inline_s
-00003190: 7368 5f65 6e76 290a 2020 2020 2020 2020  sh_env).        
-000031a0: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
-000031b0: 7061 7468 203d 2073 6c75 726d 5f64 6174  path = slurm_dat
-000031c0: 615f 7061 7468 0a20 2020 2020 2020 2073  a_path.        s
-000031d0: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
-000031e0: 5f70 6174 6820 3d20 736c 7572 6d5f 696d  _path = slurm_im
-000031f0: 6167 6573 5f70 6174 680a 2020 2020 2020  ages_path.      
-00003200: 2020 7365 6c66 2e73 6c75 726d 5f63 6f6e    self.slurm_con
-00003210: 7665 7274 6572 735f 7061 7468 203d 2073  verters_path = s
-00003220: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
-00003230: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
-00003240: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
-00003250: 7468 7320 3d20 736c 7572 6d5f 6d6f 6465  ths = slurm_mode
-00003260: 6c5f 7061 7468 730a 2020 2020 2020 2020  l_paths.        
-00003270: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
-00003280: 745f 7061 7468 203d 2073 6c75 726d 5f73  t_path = slurm_s
-00003290: 6372 6970 745f 7061 7468 0a20 2020 2020  cript_path.     
-000032a0: 2020 2073 656c 662e 736c 7572 6d5f 7363     self.slurm_sc
-000032b0: 7269 7074 5f72 6570 6f20 3d20 736c 7572  ript_repo = slur
-000032c0: 6d5f 7363 7269 7074 5f72 6570 6f0a 2020  m_script_repo.  
-000032d0: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
-000032e0: 5f6d 6f64 656c 5f72 6570 6f73 203d 2073  _model_repos = s
-000032f0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-00003300: 0a20 2020 2020 2020 2073 656c 662e 736c  .        self.sl
-00003310: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
-00003320: 203d 2073 6c75 726d 5f6d 6f64 656c 5f69   = slurm_model_i
-00003330: 6d61 6765 730a 2020 2020 2020 2020 7365  mages.        se
-00003340: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f6a  lf.slurm_model_j
-00003350: 6f62 7320 3d20 736c 7572 6d5f 6d6f 6465  obs = slurm_mode
-00003360: 6c5f 6a6f 6273 0a20 2020 2020 2020 2073  l_jobs.        s
-00003370: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-00003380: 6a6f 6273 5f70 6172 616d 7320 3d20 736c  jobs_params = sl
-00003390: 7572 6d5f 6d6f 6465 6c5f 6a6f 6273 5f70  urm_model_jobs_p
-000033a0: 6172 616d 730a 0a20 2020 2020 2020 2023  arams..        #
-000033b0: 2049 6e69 7420 6361 6368 652e 204b 6565   Init cache. Kee
-000033c0: 7020 7265 7370 6f6e 7365 7320 666f 7220  p responses for 
-000033d0: 3336 3020 7365 636f 6e64 730a 2020 2020  360 seconds.    
-000033e0: 2020 2020 7365 6c66 2e63 6163 6865 203d      self.cache =
-000033f0: 2072 6571 7565 7374 735f 6361 6368 652e   requests_cache.
-00003400: 6261 636b 656e 6473 2e73 716c 6974 652e  backends.sqlite.
-00003410: 5351 4c69 7465 4361 6368 6528 0a20 2020  SQLiteCache(.   
-00003420: 2020 2020 2020 2020 2064 625f 7061 7468           db_path
-00003430: 3d22 6769 7468 7562 5f63 6163 6865 222c  ="github_cache",
-00003440: 2075 7365 5f74 656d 703d 5472 7565 290a   use_temp=True).
-00003450: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00003460: 5f6f 725f 6372 6561 7465 5f67 6974 6875  _or_create_githu
-00003470: 625f 7365 7373 696f 6e28 290a 0a20 2020  b_session()..   
-00003480: 2020 2020 2073 656c 662e 696e 6974 5f77       self.init_w
-00003490: 6f72 6b66 6c6f 7773 2829 0a20 2020 2020  orkflows().     
-000034a0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-000034b0: 2876 616c 6964 6174 655f 736c 7572 6d5f  (validate_slurm_
-000034c0: 7365 7475 703d 696e 6974 5f73 6c75 726d  setup=init_slurm
-000034d0: 290a 0a20 2020 2064 6566 2069 6e69 745f  )..    def init_
-000034e0: 776f 726b 666c 6f77 7328 7365 6c66 2c20  workflows(self, 
-000034f0: 666f 7263 655f 7570 6461 7465 3a20 626f  force_update: bo
-00003500: 6f6c 203d 2046 616c 7365 293a 0a20 2020  ol = False):.   
-00003510: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003520: 2052 6574 7269 6576 6573 2074 6865 2072   Retrieves the r
-00003530: 6571 7569 7265 6420 696e 666f 2066 6f72  equired info for
-00003540: 2074 6865 2063 6f6e 6669 6775 7265 6420   the configured 
-00003550: 776f 726b 666c 6f77 7320 6672 6f6d 2067  workflows from g
-00003560: 6974 6875 622e 0a20 2020 2020 2020 2049  ithub..        I
-00003570: 7420 7769 6c6c 2066 696c 6c20 6073 6c75  t will fill `slu
-00003580: 726d 5f6d 6f64 656c 5f69 6d61 6765 7360  rm_model_images`
-00003590: 2077 6974 6820 646f 636b 6572 6875 6220   with dockerhub 
-000035a0: 6c69 6e6b 732e 0a0a 2020 2020 2020 2020  links...        
-000035b0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000035c0: 2020 666f 7263 655f 7570 6461 7465 2028    force_update (
-000035d0: 626f 6f6c 293a 2057 696c 6c20 6f76 6572  bool): Will over
-000035e0: 7772 6974 6520 616c 7265 6164 7920 6769  write already gi
-000035f0: 7665 6e20 7061 7468 730a 2020 2020 2020  ven paths.      
-00003600: 2020 2020 2020 2020 2020 696e 2060 736c            in `sl
-00003610: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
-00003620: 600a 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
-00003630: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00003640: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f69  lf.slurm_model_i
-00003650: 6d61 6765 733a 0a20 2020 2020 2020 2020  mages:.         
-00003660: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
-00003670: 6465 6c5f 696d 6167 6573 203d 207b 7d0a  del_images = {}.
-00003680: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00003690: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-000036a0: 7265 706f 733a 0a20 2020 2020 2020 2020  repos:.         
-000036b0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-000036c0: 6728 224e 6f20 776f 726b 666c 6f77 7320  g("No workflows 
-000036d0: 636f 6e66 6967 7572 6564 2122 290a 2020  configured!").  
-000036e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000036f0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-00003700: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00003710: 2020 2320 736b 6970 7320 7468 6520 7365    # skips the se
-00003720: 7475 700a 2020 2020 2020 2020 666f 7220  tup.        for 
-00003730: 776f 726b 666c 6f77 2069 6e20 7365 6c66  workflow in self
-00003740: 2e73 6c75 726d 5f6d 6f64 656c 5f72 6570  .slurm_model_rep
-00003750: 6f73 2e6b 6579 7328 293a 0a20 2020 2020  os.keys():.     
-00003760: 2020 2020 2020 2069 6620 776f 726b 666c         if workfl
-00003770: 6f77 206e 6f74 2069 6e20 7365 6c66 2e73  ow not in self.s
-00003780: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
-00003790: 7320 6f72 2066 6f72 6365 5f75 7064 6174  s or force_updat
-000037a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000037b0: 2020 206a 736f 6e5f 6465 7363 7269 7074     json_descript
-000037c0: 6f72 203d 2073 656c 662e 7075 6c6c 5f64  or = self.pull_d
-000037d0: 6573 6372 6970 746f 725f 6672 6f6d 5f67  escriptor_from_g
-000037e0: 6974 6875 6228 776f 726b 666c 6f77 290a  ithub(workflow).
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003800: 6c6f 6767 6572 2e64 6562 7567 2827 2573  logger.debug('%s
-00003810: 3a20 2573 272c 2077 6f72 6b66 6c6f 772c  : %s', workflow,
-00003820: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
-00003830: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003840: 2020 696d 6167 6520 3d20 6a73 6f6e 5f64    image = json_d
-00003850: 6573 6372 6970 746f 725b 2763 6f6e 7461  escriptor['conta
-00003860: 696e 6572 2d69 6d61 6765 275d 5b27 696d  iner-image']['im
-00003870: 6167 6527 5d0a 2020 2020 2020 2020 2020  age'].          
-00003880: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
-00003890: 5f6d 6f64 656c 5f69 6d61 6765 735b 776f  _model_images[wo
-000038a0: 726b 666c 6f77 5d20 3d20 696d 6167 650a  rkflow] = image.
-000038b0: 0a20 2020 2064 6566 2073 6574 7570 5f73  .    def setup_s
-000038c0: 6c75 726d 2873 656c 6629 3a0a 2020 2020  lurm(self):.    
-000038d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000038e0: 5661 6c69 6461 7465 7320 6f72 2063 7265  Validates or cre
-000038f0: 6174 6573 2074 6865 2072 6571 7569 7265  ates the require
-00003900: 6420 7365 7475 7020 6f6e 2074 6865 2053  d setup on the S
-00003910: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
-00003920: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00003930: 2020 2020 2020 2020 2020 2053 5348 4578             SSHEx
-00003940: 6365 7074 696f 6e3a 2069 6620 6974 2063  ception: if it c
-00003950: 616e 6e6f 7420 636f 6e6e 6563 7420 746f  annot connect to
-00003960: 2053 6c75 726d 2c20 6f72 2072 756e 7320   Slurm, or runs 
-00003970: 696e 746f 2061 6e20 6572 726f 720a 2020  into an error.  
-00003980: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003990: 2020 6966 2073 656c 662e 7661 6c69 6461    if self.valida
-000039a0: 7465 2829 3a0a 2020 2020 2020 2020 2020  te():.          
-000039b0: 2020 2320 312e 2043 7265 6174 6520 6469    # 1. Create di
-000039c0: 7265 6374 6f72 6965 730a 2020 2020 2020  rectories.      
-000039d0: 2020 2020 2020 6469 725f 636d 6473 203d        dir_cmds =
-000039e0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-000039f0: 2320 612e 2064 6174 610a 2020 2020 2020  # a. data.      
-00003a00: 2020 2020 2020 6966 2073 656c 662e 736c        if self.sl
-00003a10: 7572 6d5f 6461 7461 5f70 6174 683a 0a20  urm_data_path:. 
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003a30: 6972 5f63 6d64 732e 6170 7065 6e64 2866  ir_cmds.append(f
-00003a40: 226d 6b64 6972 202d 7020 7b73 656c 662e  "mkdir -p {self.
-00003a50: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-00003a60: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
-00003a70: 2062 2e20 7363 7269 7074 730a 2020 2020   b. scripts.    
-00003a80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003a90: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
-00003aa0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00003ab0: 2020 2064 6972 5f63 6d64 732e 6170 7065     dir_cmds.appe
-00003ac0: 6e64 2866 226d 6b64 6972 202d 7020 7b73  nd(f"mkdir -p {s
-00003ad0: 656c 662e 736c 7572 6d5f 7363 7269 7074  elf.slurm_script
-00003ae0: 5f70 6174 687d 2229 0a20 2020 2020 2020  _path}").       
-00003af0: 2020 2020 2023 2063 2e20 776f 726b 666c       # c. workfl
-00003b00: 6f77 730a 2020 2020 2020 2020 2020 2020  ows.            
-00003b10: 6966 2073 656c 662e 736c 7572 6d5f 696d  if self.slurm_im
-00003b20: 6167 6573 5f70 6174 683a 0a20 2020 2020  ages_path:.     
-00003b30: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
-00003b40: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-00003b50: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-00003b60: 6d5f 696d 6167 6573 5f70 6174 687d 2229  m_images_path}")
-00003b70: 0a20 2020 2020 2020 2020 2020 2072 203d  .            r =
-00003b80: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00003b90: 6473 2864 6972 5f63 6d64 7329 0a20 2020  ds(dir_cmds).   
-00003ba0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00003bb0: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
-00003bc0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-00003bd0: 7863 6570 7469 6f6e 2872 290a 0a20 2020  xception(r)..   
-00003be0: 2020 2020 2020 2020 2023 2032 2e20 436c           # 2. Cl
-00003bf0: 6f6e 6520 6769 740a 2020 2020 2020 2020  one git.        
-00003c00: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00003c10: 6d5f 7363 7269 7074 5f72 6570 6f20 616e  m_script_repo an
-00003c20: 6420 7365 6c66 2e73 6c75 726d 5f73 6372  d self.slurm_scr
-00003c30: 6970 745f 7061 7468 3a0a 2020 2020 2020  ipt_path:.      
-00003c40: 2020 2020 2020 2020 2020 2320 6769 7420            # git 
-00003c50: 636c 6f6e 6520 696e 746f 2073 6372 6970  clone into scrip
-00003c60: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
-00003c70: 2020 2020 2020 2065 6e76 203d 207b 0a20         env = {. 
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 2022 5245 504f 5352 4322 3a20 7365     "REPOSRC": se
-00003ca0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-00003cb0: 7265 706f 2c0a 2020 2020 2020 2020 2020  repo,.          
-00003cc0: 2020 2020 2020 2020 2020 224c 4f43 414c            "LOCAL
-00003cd0: 5245 504f 223a 2073 656c 662e 736c 7572  REPO": self.slur
-00003ce0: 6d5f 7363 7269 7074 5f70 6174 680a 2020  m_script_path.  
-00003cf0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 636d 6420 3d20 2767 6974 2063 6c6f 6e65  cmd = 'git clone
-00003d20: 2022 2452 4550 4f53 5243 2220 2224 4c4f   "$REPOSRC" "$LO
-00003d30: 4341 4c52 4550 4f22 2032 3e20 2f64 6576  CALREPO" 2> /dev
-00003d40: 2f6e 756c 6c20 7c7c 2067 6974 202d 4320  /null || git -C 
-00003d50: 2224 4c4f 4341 4c52 4550 4f22 2070 756c  "$LOCALREPO" pul
-00003d60: 6c27 0a20 2020 2020 2020 2020 2020 2020  l'.             
-00003d70: 2020 2072 203d 2073 656c 662e 7275 6e5f     r = self.run_
-00003d80: 636f 6d6d 616e 6473 285b 636d 645d 2c20  commands([cmd], 
-00003d90: 656e 7629 0a20 2020 2020 2020 2020 2020  env).           
-00003da0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
-00003db0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003dc0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-00003dd0: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
-00003de0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00003df0: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
-00003e00: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-00003e10: 2020 2020 2023 2067 656e 6572 6174 6520       # generate 
-00003e20: 7363 7269 7074 730a 2020 2020 2020 2020  scripts.        
-00003e30: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
-00003e40: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
-00003e50: 7328 6765 6e65 7261 7465 5f6a 6f62 733d  s(generate_jobs=
-00003e60: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
-00003e70: 2020 2023 2033 2e20 5365 7475 7020 636f     # 3. Setup co
-00003e80: 6e76 6572 7465 7273 0a20 2020 2020 2020  nverters.       
-00003e90: 2020 2020 2063 6f6e 7665 7274 5f63 6d64       convert_cmd
-00003ea0: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-00003eb0: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
-00003ec0: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
-00003ed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ee0: 2020 636f 6e76 6572 745f 636d 6473 2e61    convert_cmds.a
-00003ef0: 7070 656e 6428 6622 6d6b 6469 7220 2d70  ppend(f"mkdir -p
-00003f00: 207b 7365 6c66 2e73 6c75 726d 5f63 6f6e   {self.slurm_con
-00003f10: 7665 7274 6572 735f 7061 7468 7d22 290a  verters_path}").
-00003f20: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
-00003f30: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-00003f40: 7328 636f 6e76 6572 745f 636d 6473 290a  s(convert_cmds).
-00003f50: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00003f60: 7079 2067 656e 6572 6963 206a 6f62 2061  py generic job a
-00003f70: 7272 6179 2073 6372 6970 7420 6f76 6572  rray script over
-00003f80: 2074 6f20 736c 7572 6d0a 2020 2020 2020   to slurm.      
-00003f90: 2020 2020 2020 636f 6e76 6572 745f 6a6f        convert_jo
-00003fa0: 625f 6c6f 6361 6c20 3d20 6669 6c65 7328  b_local = files(
-00003fb0: 2272 6573 6f75 7263 6573 2229 2e6a 6f69  "resources").joi
-00003fc0: 6e70 6174 6828 0a20 2020 2020 2020 2020  npath(.         
-00003fd0: 2020 2020 2020 2022 636f 6e76 6572 745f         "convert_
-00003fe0: 6a6f 625f 6172 7261 792e 7368 2229 0a20  job_array.sh"). 
-00003ff0: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
-00004000: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
-00004010: 6e76 6572 745f 6a6f 625f 6c6f 6361 6c2c  nvert_job_local,
-00004020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004030: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-00004040: 3d73 656c 662e 736c 7572 6d5f 7363 7269  =self.slurm_scri
-00004050: 7074 5f70 6174 6829 0a20 2020 2020 2020  pt_path).       
-00004060: 2020 2020 2023 2063 7572 7265 6e74 6c79       # currently
-00004070: 206b 6e6f 776e 2063 6f6e 7665 7274 6572   known converter
-00004080: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00004090: 3361 2e20 5a41 5252 2074 6f20 5449 4646  3a. ZARR to TIFF
-000040a0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-000040b0: 4f44 4f20 6578 7472 6163 7420 7468 6573  ODO extract thes
-000040c0: 6520 7661 6c75 6573 2074 6f20 652e 672e  e values to e.g.
-000040d0: 2063 6f6e 6669 6720 6966 2077 6520 6861   config if we ha
-000040e0: 7665 206d 6f72 650a 2020 2020 2020 2020  ve more.        
-000040f0: 2020 2020 636f 6e76 6572 745f 6e61 6d65      convert_name
-00004100: 203d 2022 636f 6e76 6572 745f 7a61 7272   = "convert_zarr
-00004110: 5f74 6f5f 7469 6666 220a 2020 2020 2020  _to_tiff".      
-00004120: 2020 2020 2020 636f 6e76 6572 745f 7079        convert_py
-00004130: 203d 2066 227b 636f 6e76 6572 745f 6e61   = f"{convert_na
-00004140: 6d65 7d2e 7079 220a 2020 2020 2020 2020  me}.py".        
-00004150: 2020 2020 636f 6e76 6572 745f 7363 7269      convert_scri
-00004160: 7074 5f6c 6f63 616c 203d 2066 696c 6573  pt_local = files
-00004170: 2822 7265 736f 7572 6365 7322 292e 6a6f  ("resources").jo
-00004180: 696e 7061 7468 280a 2020 2020 2020 2020  inpath(.        
-00004190: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-000041a0: 7079 290a 2020 2020 2020 2020 2020 2020  py).            
-000041b0: 636f 6e76 6572 745f 6465 6620 3d20 6622  convert_def = f"
-000041c0: 7b63 6f6e 7665 7274 5f6e 616d 657d 2e64  {convert_name}.d
-000041d0: 6566 220a 2020 2020 2020 2020 2020 2020  ef".            
-000041e0: 636f 6e76 6572 745f 6465 665f 6c6f 6361  convert_def_loca
-000041f0: 6c20 3d20 6669 6c65 7328 2272 6573 6f75  l = files("resou
-00004200: 7263 6573 2229 2e6a 6f69 6e70 6174 6828  rces").joinpath(
-00004210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004220: 2063 6f6e 7665 7274 5f64 6566 290a 2020   convert_def).  
-00004230: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
-00004240: 6c66 2e70 7574 286c 6f63 616c 3d63 6f6e  lf.put(local=con
-00004250: 7665 7274 5f73 6372 6970 745f 6c6f 6361  vert_script_loca
-00004260: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-00004270: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
-00004280: 7465 3d73 656c 662e 736c 7572 6d5f 636f  te=self.slurm_co
-00004290: 6e76 6572 7465 7273 5f70 6174 6829 0a20  nverters_path). 
-000042a0: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
-000042b0: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
-000042c0: 6e76 6572 745f 6465 665f 6c6f 6361 6c2c  nvert_def_local,
-000042d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042e0: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-000042f0: 3d73 656c 662e 736c 7572 6d5f 636f 6e76  =self.slurm_conv
-00004300: 6572 7465 7273 5f70 6174 6829 0a20 2020  erters_path).   
-00004310: 2020 2020 2020 2020 2023 2042 7569 6c64           # Build
-00004320: 2073 696e 6775 6c61 7269 7479 2063 6f6e   singularity con
-00004330: 7461 696e 6572 2066 726f 6d20 6465 6669  tainer from defi
-00004340: 6e69 7469 6f6e 0a20 2020 2020 2020 2020  nition.         
-00004350: 2020 2077 6974 6820 7365 6c66 2e63 6428     with self.cd(
-00004360: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
-00004370: 7274 6572 735f 7061 7468 293a 0a20 2020  rters_path):.   
-00004380: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00004390: 7665 7274 5f63 6d64 7320 3d20 5b5d 0a20  vert_cmds = []. 
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000043b0: 6620 7365 6c66 2e73 6c75 726d 5f69 6d61  f self.slurm_ima
-000043c0: 6765 735f 7061 7468 3a0a 2020 2020 2020  ges_path:.      
-000043d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000043e0: 544f 444f 2043 6861 6e67 6520 7468 6520  TODO Change the 
-000043f0: 746d 7020 6469 723f 0a20 2020 2020 2020  tmp dir?.       
-00004400: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-00004410: 7870 6f72 7420 5349 4e47 554c 4152 4954  xport SINGULARIT
-00004420: 595f 544d 5044 4952 3d7e 2f6d 792d 7363  Y_TMPDIR=~/my-sc
-00004430: 7261 7463 682f 746d 703b 0a0a 2020 2020  ratch/tmp;..    
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2320 6f6e 6c79 2069 6620 6669 6c65 2064  # only if file d
-00004460: 6f65 7320 6e6f 7420 6578 6973 7420 7965  oes not exist ye
-00004470: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00004480: 2020 2020 2020 2320 636f 6e76 6572 745f        # convert_
-00004490: 636d 6473 2e61 7070 656e 6428 6622 5b20  cmds.append(f"[ 
-000044a0: 2120 2d66 207b 636f 6e76 6572 745f 6e61  ! -f {convert_na
-000044b0: 6d65 7d2e 7369 6620 5d22 290a 2020 2020  me}.sif ]").    
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2320 4544 4954 202d 2d20 4e4f 2c20 7468  # EDIT -- NO, th
-000044e0: 656e 2077 6520 6361 6e27 7420 7570 6461  en we can't upda
-000044f0: 7465 2120 466f 7263 6520 7265 6275 696c  te! Force rebuil
-00004500: 6421 0a0a 2020 2020 2020 2020 2020 2020  d!..            
-00004510: 2020 2020 2020 2020 2320 646f 776e 6c6f          # downlo
-00004520: 6164 202f 6275 696c 6420 6e65 7720 636f  ad /build new co
-00004530: 6e74 6169 6e65 720a 2020 2020 2020 2020  ntainer.        
-00004540: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
-00004550: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
-00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004570: 2020 2020 2020 2020 2066 2273 696e 6775           f"singu
-00004580: 6c61 7269 7479 2062 7569 6c64 202d 4620  larity build -F 
-00004590: 7b63 6f6e 7665 7274 5f6e 616d 657d 2e73  {convert_name}.s
-000045a0: 6966 207b 636f 6e76 6572 745f 6465 667d  if {convert_def}
-000045b0: 203e 3e20 7369 6e67 2e6c 6f67 2032 3e26   >> sing.log 2>&
-000045c0: 3120 3b20 6563 686f 2027 6669 6e69 7368  1 ; echo 'finish
-000045d0: 6564 207b 636f 6e76 6572 745f 6e61 6d65  ed {convert_name
-000045e0: 7d2e 7369 6627 2026 2229 0a20 2020 2020  }.sif' &").     
-000045f0: 2020 2020 2020 2020 2020 2072 203d 2073             r = s
-00004600: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-00004610: 2863 6f6e 7665 7274 5f63 6d64 7329 0a0a  (convert_cmds)..
-00004620: 2020 2020 2020 2020 2020 2020 2320 342e              # 4.
-00004630: 2044 6f77 6e6c 6f61 6420 776f 726b 666c   Download workfl
-00004640: 6f77 2069 6d61 6765 730a 2020 2020 2020  ow images.      
-00004650: 2020 2020 2020 2320 4372 6561 7465 2073        # Create s
-00004660: 7065 6369 6669 6320 776f 726b 666c 6f77  pecific workflow
-00004670: 2064 6972 730a 2020 2020 2020 2020 2020   dirs.          
-00004680: 2020 7769 7468 2073 656c 662e 6364 2873    with self.cd(s
-00004690: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
-000046a0: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-000046b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000046c0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-000046d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000046e0: 2020 2020 2020 206d 6f64 656c 7061 7468         modelpath
-000046f0: 7320 3d20 2220 222e 6a6f 696e 2873 656c  s = " ".join(sel
-00004700: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
-00004710: 7468 732e 7661 6c75 6573 2829 290a 2020  ths.values()).  
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2320 6d6b 6469 7220 6365 6c6c 7072    # mkdir cellpr
-00004740: 6f66 696c 6572 2069 6d61 6765 6a20 2e2e  ofiler imagej ..
-00004750: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004760: 2020 2020 2020 7220 3d20 7365 6c66 2e72        r = self.r
-00004770: 756e 5f63 6f6d 6d61 6e64 7328 5b66 226d  un_commands([f"m
-00004780: 6b64 6972 202d 7020 7b6d 6f64 656c 7061  kdir -p {modelpa
-00004790: 7468 737d 225d 290a 2020 2020 2020 2020  ths}"]).        
-000047a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000047b0: 6f74 2072 2e6f 6b3a 0a20 2020 2020 2020  ot r.ok:.       
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2072 6169 7365 2053 5348 4578 6365 7074   raise SSHExcept
-000047e0: 696f 6e28 7229 0a0a 2020 2020 2020 2020  ion(r)..        
-000047f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004800: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
-00004810: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00004820: 2020 2020 2020 2020 7075 6c6c 5f63 6f6d          pull_com
-00004830: 6d61 6e64 7320 3d20 5b5d 0a20 2020 2020  mands = [].     
-00004840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004850: 6f72 2077 662c 2069 6d61 6765 2069 6e20  or wf, image in 
-00004860: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00004870: 5f69 6d61 6765 732e 6974 656d 7328 293a  _images.items():
-00004880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004890: 2020 2020 2020 2020 2072 6570 6f20 3d20           repo = 
-000048a0: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-000048b0: 5f72 6570 6f73 5b77 665d 0a20 2020 2020  _repos[wf].     
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2070 6174 6820 3d20 7365 6c66 2e73     path = self.s
-000048e0: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
-000048f0: 5b77 665d 0a20 2020 2020 2020 2020 2020  [wf].           
-00004900: 2020 2020 2020 2020 2020 2020 205f 2c20               _, 
-00004910: 7665 7273 696f 6e20 3d20 7365 6c66 2e65  version = self.e
-00004920: 7874 7261 6374 5f70 6172 7473 5f66 726f  xtract_parts_fro
-00004930: 6d5f 7572 6c28 7265 706f 290a 2020 2020  m_url(repo).    
-00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004950: 2020 2020 6966 2076 6572 7369 6f6e 203d      if version =
-00004960: 3d20 226d 6173 7465 7222 3a0a 2020 2020  = "master":.    
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
-00004990: 3d20 226c 6174 6573 7422 0a20 2020 2020  = "latest".     
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2020 2070 756c 6c5f 7465 6d70 6c61 7465     pull_template
-000049c0: 203d 2022 7469 6d65 2073 696e 6775 6c61   = "time singula
-000049d0: 7269 7479 2070 756c 6c20 2d2d 6469 7361  rity pull --disa
-000049e0: 626c 652d 6361 6368 6520 2d2d 6469 7220  ble-cache --dir 
-000049f0: 2470 6174 6820 646f 636b 6572 3a2f 2f24  $path docker://$
-00004a00: 696d 6167 653a 2476 6572 7369 6f6e 2020  image:$version  
-00004a10: 3e3e 2073 696e 672e 6c6f 6720 323e 2631  >> sing.log 2>&1
-00004a20: 203b 2065 6368 6f20 2766 696e 6973 6865   ; echo 'finishe
-00004a30: 6420 2470 6174 6827 2026 220a 2020 2020  d $path' &".    
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 7420 3d20 5465 6d70 6c61 7465      t = Template
-00004a60: 2870 756c 6c5f 7465 6d70 6c61 7465 290a  (pull_template).
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 2020 7375 6273 7469 7475          substitu
-00004a90: 7465 7320 3d20 7b7d 0a20 2020 2020 2020  tes = {}.       
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ab0: 2073 7562 7374 6974 7574 6573 5b27 7061   substitutes['pa
-00004ac0: 7468 275d 203d 2070 6174 680a 2020 2020  th'] = path.    
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 2020 2020 7375 6273 7469 7475 7465 735b      substitutes[
-00004af0: 2769 6d61 6765 275d 203d 2069 6d61 6765  'image'] = image
-00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b10: 2020 2020 2020 2020 2073 7562 7374 6974           substit
-00004b20: 7574 6573 5b27 7665 7273 696f 6e27 5d20  utes['version'] 
-00004b30: 3d20 7665 7273 696f 6e0a 2020 2020 2020  = version.      
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b50: 2020 636d 6420 3d20 742e 7361 6665 5f73    cmd = t.safe_s
-00004b60: 7562 7374 6974 7574 6528 7375 6273 7469  ubstitute(substi
-00004b70: 7475 7465 7329 0a20 2020 2020 2020 2020  tutes).         
-00004b80: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00004b90: 6f67 6765 722e 6465 6275 6728 6622 7375  ogger.debug(f"su
-00004ba0: 6273 7469 7475 7465 643a 207b 636d 647d  bstituted: {cmd}
-00004bb0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00004bc0: 2020 2020 2020 2020 2020 2070 756c 6c5f             pull_
-00004bd0: 636f 6d6d 616e 6473 2e61 7070 656e 6428  commands.append(
-00004be0: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
-00004bf0: 2020 2020 2020 2020 2073 6372 6970 745f           script_
-00004c00: 6e61 6d65 203d 2022 7075 6c6c 5f69 6d61  name = "pull_ima
-00004c10: 6765 732e 7368 220a 2020 2020 2020 2020  ges.sh".        
-00004c20: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00004c30: 6c61 7465 5f73 6372 6970 7420 3d20 6669  late_script = fi
-00004c40: 6c65 7328 2272 6573 6f75 7263 6573 2229  les("resources")
-00004c50: 2e6a 6f69 6e70 6174 6828 7363 7269 7074  .joinpath(script
-00004c60: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-00004c70: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00004c80: 7465 6d70 6c61 7465 5f73 6372 6970 742e  template_script.
-00004c90: 6f70 656e 2827 7227 2920 6173 2066 3a0a  open('r') as f:.
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 2020 2020 2020 7372 6320 3d20 5465          src = Te
-00004cc0: 6d70 6c61 7465 2866 2e72 6561 6428 2929  mplate(f.read())
-00004cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ce0: 2020 2020 2020 2020 2073 7562 7374 6974           substit
-00004cf0: 7574 6520 3d20 7b27 7075 6c6c 636f 6d6d  ute = {'pullcomm
-00004d00: 616e 6473 273a 2022 5c6e 222e 6a6f 696e  ands': "\n".join
-00004d10: 2870 756c 6c5f 636f 6d6d 616e 6473 297d  (pull_commands)}
-00004d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d30: 2020 2020 2020 2020 206a 6f62 5f73 6372           job_scr
-00004d40: 6970 7420 3d20 7372 632e 7361 6665 5f73  ipt = src.safe_s
-00004d50: 7562 7374 6974 7574 6528 7375 6273 7469  ubstitute(substi
-00004d60: 7475 7465 290a 2020 2020 2020 2020 2020  tute).          
-00004d70: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00004d80: 2e64 6562 7567 2866 2273 7562 7374 6974  .debug(f"substit
-00004d90: 7574 6564 3a5c 6e20 7b6a 6f62 5f73 6372  uted:\n {job_scr
-00004da0: 6970 747d 2229 0a20 2020 2020 2020 2020  ipt}").         
-00004db0: 2020 2020 2020 2020 2020 2023 2063 6f70             # cop
-00004dc0: 7920 746f 2072 656d 6f74 6520 6669 6c65  y to remote file
-00004dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004de0: 2020 2020 2066 756c 6c5f 7061 7468 203d       full_path =
-00004df0: 2073 656c 662e 736c 7572 6d5f 696d 6167   self.slurm_imag
-00004e00: 6573 5f70 6174 682b 222f 222b 7363 7269  es_path+"/"+scri
-00004e10: 7074 5f6e 616d 650a 2020 2020 2020 2020  pt_name.        
-00004e20: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
-00004e30: 7365 6c66 2e70 7574 286c 6f63 616c 3d69  self.put(local=i
-00004e40: 6f2e 5374 7269 6e67 494f 286a 6f62 5f73  o.StringIO(job_s
-00004e50: 6372 6970 7429 2c0a 2020 2020 2020 2020  cript),.        
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 2020 2072 656d 6f74 653d           remote=
-00004e80: 6675 6c6c 5f70 6174 6829 0a20 2020 2020  full_path).     
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004ea0: 6d64 203d 2066 2274 696d 6520 7368 207b  md = f"time sh {
-00004eb0: 7363 7269 7074 5f6e 616d 657d 220a 2020  script_name}".  
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 7220 3d20 7365 6c66 2e72 756e 5f63    r = self.run_c
-00004ee0: 6f6d 6d61 6e64 7328 5b63 6d64 5d29 0a20  ommands([cmd]). 
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 2069 6620 6e6f 7420 722e 6f6b 3a0a     if not r.ok:.
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
-00004f30: 4845 7863 6570 7469 6f6e 2872 290a 2020  HException(r).  
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 6c6f 6767 6572 2e69 6e66 6f28 722e    logger.info(r.
-00004f60: 7374 646f 7574 290a 2020 2020 2020 2020  stdout).        
-00004f70: 2020 2020 2020 2020 2020 2020 2320 2320              # # 
-00004f80: 636c 6561 6e75 7020 6769 616e 7420 7369  cleanup giant si
-00004f90: 6e67 756c 6172 6974 7920 6361 6368 6521  ngularity cache!
-00004fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004fb0: 2020 2020 2023 2075 7369 6e67 202d 2d64       # using --d
-00004fc0: 6973 6162 6c65 2d63 6163 6865 2062 6563  isable-cache bec
-00004fd0: 6175 7365 2077 6520 7275 6e20 696e 2074  ause we run in t
-00004fe0: 6865 2062 6163 6b67 726f 756e 640a 2020  he background.  
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2320 636d 6420 3d20 2273 696e 6775    # cmd = "singu
-00005010: 6c61 7269 7479 2063 6163 6865 2063 6c65  larity cache cle
-00005020: 616e 202d 6622 0a20 2020 2020 2020 2020  an -f".         
-00005030: 2020 2020 2020 2020 2020 2023 2072 203d             # r =
-00005040: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00005050: 6473 285b 636d 645d 290a 0a20 2020 2020  ds([cmd])..     
-00005060: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005070: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00005080: 6365 7074 696f 6e28 2246 6169 6c75 7265  ception("Failure
-00005090: 2069 6e20 636f 6e6e 6563 7469 6e67 2074   in connecting t
-000050a0: 6f20 536c 7572 6d20 636c 7573 7465 7222  o Slurm cluster"
-000050b0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-000050c0: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
-000050d0: 5f63 6f6e 6669 6728 636c 732c 2063 6f6e  _config(cls, con
-000050e0: 6669 6766 696c 653a 2073 7472 203d 2027  figfile: str = '
-000050f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00005100: 2020 2020 2020 2069 6e69 745f 736c 7572         init_slur
-00005110: 6d3a 2062 6f6f 6c20 3d20 4661 6c73 6529  m: bool = False)
-00005120: 202d 3e20 2753 6c75 726d 436c 6965 6e74   -> 'SlurmClient
-00005130: 273a 0a20 2020 2020 2020 2022 2222 4372  ':.        """Cr
-00005140: 6561 7465 7320 6120 6e65 7720 536c 7572  eates a new Slur
-00005150: 6d43 6c69 656e 7420 6f62 6a65 6374 2075  mClient object u
-00005160: 7369 6e67 2074 6865 2070 6172 616d 6574  sing the paramet
-00005170: 6572 7320 7265 6164 2066 726f 6d20 610a  ers read from a.
-00005180: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00005190: 6174 696f 6e20 6669 6c65 2028 2e69 6e69  ation file (.ini
-000051a0: 292e 0a0a 2020 2020 2020 2020 4465 6661  )...        Defa
-000051b0: 756c 7473 2070 6174 6873 2074 6f20 6c6f  ults paths to lo
-000051c0: 6f6b 2066 6f72 2063 6f6e 6669 6720 6669  ok for config fi
-000051d0: 6c65 7320 6172 653a 0a20 2020 2020 2020  les are:.       
-000051e0: 2020 2020 202d 202f 6574 632f 736c 7572       - /etc/slur
-000051f0: 6d2d 636f 6e66 6967 2e69 6e69 0a20 2020  m-config.ini.   
-00005200: 2020 2020 2020 2020 202d 207e 2f73 6c75           - ~/slu
-00005210: 726d 2d63 6f6e 6669 672e 696e 690a 0a20  rm-config.ini.. 
-00005220: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00005230: 2074 6869 7320 6973 206f 6e6c 7920 666f   this is only fo
-00005240: 7220 7468 6520 534c 5552 4d20 7370 6563  r the SLURM spec
-00005250: 6966 6963 2076 616c 7565 7320 7468 6174  ific values that
-00005260: 2077 6520 6164 6465 642e 0a20 2020 2020   we added..     
-00005270: 2020 204d 6f73 7420 636f 6e66 6967 7572     Most configur
-00005280: 6174 696f 6e20 7661 6c75 6573 2061 7265  ation values are
-00005290: 2073 6574 2076 6961 2063 6f6e 6669 6775   set via configu
-000052a0: 7261 7469 6f6e 206d 6563 6861 6e69 736d  ration mechanism
-000052b0: 7320 6672 6f6d 0a20 2020 2020 2020 2046  s from.        F
-000052c0: 6162 7269 6320 6c69 6272 6172 792c 0a20  abric library,. 
-000052d0: 2020 2020 2020 206c 696b 6520 5353 4820         like SSH 
-000052e0: 7365 7474 696e 6773 2062 6569 6e67 206c  settings being l
-000052f0: 6f61 6465 6420 6672 6f6d 2053 5348 2063  oaded from SSH c
-00005300: 6f6e 6669 672c 202f 6574 632f 6661 6272  onfig, /etc/fabr
-00005310: 6963 2e79 6d6c 206f 720a 2020 2020 2020  ic.yml or.      
-00005320: 2020 656e 7669 726f 6e6d 656e 7420 7661    environment va
-00005330: 7269 6162 6c65 732e 0a20 2020 2020 2020  riables..       
-00005340: 2053 6565 2046 6162 7269 6327 7320 646f   See Fabric's do
-00005350: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
-00005360: 6d6f 7265 2069 6e66 6f20 6f6e 2063 6f6e  more info on con
-00005370: 6669 6775 7261 7469 6f6e 2069 6620 6e65  figuration if ne
-00005380: 6564 6564 2e0a 0a20 2020 2020 2020 2041  eded...        A
-00005390: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000053a0: 2063 6f6e 6669 6766 696c 6520 2873 7472   configfile (str
-000053b0: 293a 2054 6865 2070 6174 6820 746f 2079  ): The path to y
-000053c0: 6f75 7220 636f 6e66 6967 7572 6174 696f  our configuratio
-000053d0: 6e20 6669 6c65 2e20 4f70 7469 6f6e 616c  n file. Optional
-000053e0: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-000053f0: 6974 5f73 6c75 726d 2028 626f 6f6c 293a  it_slurm (bool):
-00005400: 2049 6e69 7469 6174 6520 2f20 7661 6c69   Initiate / vali
-00005410: 6461 7465 2073 6c75 726d 2073 6574 7570  date slurm setup
-00005420: 2e20 4f70 7469 6f6e 616c 0a20 2020 2020  . Optional.     
-00005430: 2020 2020 2020 2020 2020 204d 6967 6874             Might
-00005440: 2074 616b 6520 736f 6d65 2074 696d 6520   take some time 
-00005450: 7468 6520 6669 7273 7420 7469 6d65 2077  the first time w
-00005460: 6974 6820 646f 776e 6c6f 6164 696e 6720  ith downloading 
-00005470: 6574 632e 0a0a 2020 2020 2020 2020 5265  etc...        Re
-00005480: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00005490: 2020 2053 6c75 726d 436c 6965 6e74 3a20     SlurmClient: 
-000054a0: 4120 6e65 7720 536c 7572 6d43 6c69 656e  A new SlurmClien
-000054b0: 7420 6f62 6a65 6374 2e0a 2020 2020 2020  t object..      
-000054c0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-000054d0: 4c6f 6164 2074 6865 2063 6f6e 6669 6775  Load the configu
-000054e0: 7261 7469 6f6e 2066 696c 650a 2020 2020  ration file.    
-000054f0: 2020 2020 636f 6e66 6967 7320 3d20 636f      configs = co
-00005500: 6e66 6967 7061 7273 6572 2e43 6f6e 6669  nfigparser.Confi
-00005510: 6750 6172 7365 7228 616c 6c6f 775f 6e6f  gParser(allow_no
-00005520: 5f76 616c 7565 3d54 7275 6529 0a20 2020  _value=True).   
-00005530: 2020 2020 2023 204c 6f61 6473 2066 726f       # Loads fro
-00005540: 6d20 6465 6661 756c 7420 6c6f 6361 7469  m default locati
-00005550: 6f6e 7320 616e 6420 6769 7665 6e20 6c6f  ons and given lo
-00005560: 6361 7469 6f6e 2c20 6d69 7373 696e 6720  cation, missing 
-00005570: 6669 6c65 7320 6172 6520 6f6b 0a20 2020  files are ok.   
-00005580: 2020 2020 2063 6f6e 6669 6773 2e72 6561       configs.rea
-00005590: 6428 5b63 6c73 2e5f 4445 4641 554c 545f  d([cls._DEFAULT_
-000055a0: 434f 4e46 4947 5f50 4154 485f 312c 0a20  CONFIG_PATH_1,. 
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 636c 732e 5f44 4546 4155 4c54      cls._DEFAULT
-000055d0: 5f43 4f4e 4649 475f 5041 5448 5f32 2c0a  _CONFIG_PATH_2,.
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2063 6f6e 6669 6766 696c 655d       configfile]
-00005600: 290a 2020 2020 2020 2020 2320 5265 6164  ).        # Read
-00005610: 2074 6865 2072 6571 7569 7265 6420 7061   the required pa
-00005620: 7261 6d65 7465 7273 2066 726f 6d20 7468  rameters from th
-00005630: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00005640: 6669 6c65 2c0a 2020 2020 2020 2020 2320  file,.        # 
-00005650: 6661 6c6c 6261 636b 2074 6f20 6465 6661  fallback to defa
-00005660: 756c 7473 0a20 2020 2020 2020 2068 6f73  ults.        hos
-00005670: 7420 3d20 636f 6e66 6967 732e 6765 7428  t = configs.get(
-00005680: 2253 5348 222c 2022 686f 7374 222c 2066  "SSH", "host", f
-00005690: 616c 6c62 6163 6b3d 636c 732e 5f44 4546  allback=cls._DEF
-000056a0: 4155 4c54 5f48 4f53 5429 0a20 2020 2020  AULT_HOST).     
-000056b0: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
-000056c0: 7620 3d20 636f 6e66 6967 732e 6765 7462  v = configs.getb
-000056d0: 6f6f 6c65 616e 280a 2020 2020 2020 2020  oolean(.        
-000056e0: 2020 2020 2253 5348 222c 2022 696e 6c69      "SSH", "inli
-000056f0: 6e65 5f73 7368 5f65 6e76 222c 2066 616c  ne_ssh_env", fal
-00005700: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
-00005710: 4c54 5f49 4e4c 494e 455f 5353 485f 454e  LT_INLINE_SSH_EN
-00005720: 5629 0a20 2020 2020 2020 2073 6c75 726d  V).        slurm
-00005730: 5f64 6174 615f 7061 7468 203d 2063 6f6e  _data_path = con
-00005740: 6669 6773 2e67 6574 280a 2020 2020 2020  figs.get(.      
-00005750: 2020 2020 2020 2253 4c55 524d 222c 2022        "SLURM", "
-00005760: 736c 7572 6d5f 6461 7461 5f70 6174 6822  slurm_data_path"
-00005770: 2c20 6661 6c6c 6261 636b 3d63 6c73 2e5f  , fallback=cls._
-00005780: 4445 4641 554c 545f 534c 5552 4d5f 4441  DEFAULT_SLURM_DA
-00005790: 5441 5f50 4154 4829 0a20 2020 2020 2020  TA_PATH).       
-000057a0: 2073 6c75 726d 5f69 6d61 6765 735f 7061   slurm_images_pa
-000057b0: 7468 203d 2063 6f6e 6669 6773 2e67 6574  th = configs.get
-000057c0: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
-000057d0: 4c55 524d 222c 2022 736c 7572 6d5f 696d  LURM", "slurm_im
-000057e0: 6167 6573 5f70 6174 6822 2c0a 2020 2020  ages_path",.    
-000057f0: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
-00005800: 3d63 6c73 2e5f 4445 4641 554c 545f 534c  =cls._DEFAULT_SL
-00005810: 5552 4d5f 494d 4147 4553 5f50 4154 4829  URM_IMAGES_PATH)
-00005820: 0a20 2020 2020 2020 2073 6c75 726d 5f63  .        slurm_c
-00005830: 6f6e 7665 7274 6572 735f 7061 7468 203d  onverters_path =
-00005840: 2063 6f6e 6669 6773 2e67 6574 280a 2020   configs.get(.  
-00005850: 2020 2020 2020 2020 2020 2253 4c55 524d            "SLURM
-00005860: 222c 2022 736c 7572 6d5f 636f 6e76 6572  ", "slurm_conver
-00005870: 7465 7273 5f70 6174 6822 2c0a 2020 2020  ters_path",.    
-00005880: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
-00005890: 3d63 6c73 2e5f 4445 4641 554c 545f 534c  =cls._DEFAULT_SL
-000058a0: 5552 4d5f 434f 4e56 4552 5445 5253 5f50  URM_CONVERTERS_P
-000058b0: 4154 4829 0a0a 2020 2020 2020 2020 2320  ATH)..        # 
-000058c0: 5370 6c69 7420 7468 6520 4d4f 4445 4c53  Split the MODELS
-000058d0: 2069 6e74 6f20 7061 7468 732c 2072 6570   into paths, rep
-000058e0: 6f73 2061 6e64 2069 6d61 6765 730a 2020  os and images.  
-000058f0: 2020 2020 2020 6d6f 6465 6c73 5f64 6963        models_dic
-00005900: 7420 3d20 6469 6374 2863 6f6e 6669 6773  t = dict(configs
-00005910: 2e69 7465 6d73 2822 4d4f 4445 4c53 2229  .items("MODELS")
-00005920: 290a 2020 2020 2020 2020 736c 7572 6d5f  ).        slurm_
-00005930: 6d6f 6465 6c5f 7061 7468 7320 3d20 7b7d  model_paths = {}
-00005940: 0a20 2020 2020 2020 2073 6c75 726d 5f6d  .        slurm_m
-00005950: 6f64 656c 5f72 6570 6f73 203d 207b 7d0a  odel_repos = {}.
-00005960: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00005970: 6465 6c5f 6a6f 6273 203d 207b 7d0a 2020  del_jobs = {}.  
-00005980: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00005990: 6c5f 6a6f 6273 5f70 6172 616d 7320 3d20  l_jobs_params = 
-000059a0: 7b7d 0a20 2020 2020 2020 2066 6f72 206b  {}.        for k
-000059b0: 2c20 7620 696e 206d 6f64 656c 735f 6469  , v in models_di
-000059c0: 6374 2e69 7465 6d73 2829 3a0a 2020 2020  ct.items():.    
-000059d0: 2020 2020 2020 2020 7375 6666 6978 5f72          suffix_r
-000059e0: 6570 6f20 3d20 275f 7265 706f 270a 2020  epo = '_repo'.  
-000059f0: 2020 2020 2020 2020 2020 7375 6666 6978            suffix
-00005a00: 5f6a 6f62 203d 2027 5f6a 6f62 270a 2020  _job = '_job'.  
-00005a10: 2020 2020 2020 2020 2020 6a6f 625f 7061            job_pa
-00005a20: 7261 6d5f 7061 7474 6572 6e20 3d20 2228  ram_pattern = "(
-00005a30: 2e2b 295f 6a6f 625f 282e 2b29 220a 2020  .+)_job_(.+)".  
-00005a40: 2020 2020 2020 2020 2020 6a6f 625f 7061            job_pa
-00005a50: 7261 6d5f 6d61 7463 6820 3d20 7265 2e6d  ram_match = re.m
-00005a60: 6174 6368 286a 6f62 5f70 6172 616d 5f70  atch(job_param_p
-00005a70: 6174 7465 726e 2c20 6b29 0a20 2020 2020  attern, k).     
-00005a80: 2020 2020 2020 2069 6620 6b2e 656e 6473         if k.ends
-00005a90: 7769 7468 2873 7566 6669 785f 7265 706f  with(suffix_repo
-00005aa0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005ab0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f72     slurm_model_r
-00005ac0: 6570 6f73 5b6b 5b3a 2d6c 656e 2873 7566  epos[k[:-len(suf
-00005ad0: 6669 785f 7265 706f 295d 5d20 3d20 760a  fix_repo)]] = v.
-00005ae0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00005af0: 206b 2e65 6e64 7377 6974 6828 7375 6666   k.endswith(suff
-00005b00: 6978 5f6a 6f62 293a 0a20 2020 2020 2020  ix_job):.       
-00005b10: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
-00005b20: 6f64 656c 5f6a 6f62 735b 6b5b 3a2d 6c65  odel_jobs[k[:-le
-00005b30: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
-00005b40: 3d20 760a 2020 2020 2020 2020 2020 2020  = v.            
-00005b50: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00005b60: 6a6f 6273 5f70 6172 616d 735b 6b5b 3a2d  jobs_params[k[:-
-00005b70: 6c65 6e28 7375 6666 6978 5f6a 6f62 295d  len(suffix_job)]
-00005b80: 5d20 3d20 5b5d 0a20 2020 2020 2020 2020  ] = [].         
-00005b90: 2020 2065 6c69 6620 6a6f 625f 7061 7261     elif job_para
-00005ba0: 6d5f 6d61 7463 683a 0a20 2020 2020 2020  m_match:.       
-00005bb0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00005bc0: 224d 6174 6368 3a20 7b73 6c75 726d 5f6d  "Match: {slurm_m
-00005bd0: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
-00005be0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00005bf0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00005c00: 6a6f 6273 5f70 6172 616d 735b 6a6f 625f  jobs_params[job_
-00005c10: 7061 7261 6d5f 6d61 7463 682e 6772 6f75  param_match.grou
-00005c20: 7028 3129 5d2e 6170 7065 6e64 280a 2020  p(1)].append(.  
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 6622 202d 2d7b 6a6f 625f 7061 7261    f" --{job_para
-00005c50: 6d5f 6d61 7463 682e 6772 6f75 7028 3229  m_match.group(2)
-00005c60: 7d3d 7b76 7d22 290a 2020 2020 2020 2020  }={v}").        
-00005c70: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00005c80: 4164 6465 643a 207b 736c 7572 6d5f 6d6f  Added: {slurm_mo
-00005c90: 6465 6c5f 6a6f 6273 5f70 6172 616d 737d  del_jobs_params}
-00005ca0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-00005cb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005cc0: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-00005cd0: 5f70 6174 6873 5b6b 5d20 3d20 760a 0a20  _paths[k] = v.. 
-00005ce0: 2020 2020 2020 2073 6c75 726d 5f73 6372         slurm_scr
-00005cf0: 6970 745f 7061 7468 203d 2063 6f6e 6669  ipt_path = confi
-00005d00: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
-00005d10: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
-00005d20: 7572 6d5f 7363 7269 7074 5f70 6174 6822  urm_script_path"
-00005d30: 2c0a 2020 2020 2020 2020 2020 2020 6661  ,.            fa
-00005d40: 6c6c 6261 636b 3d63 6c73 2e5f 4445 4641  llback=cls._DEFA
-00005d50: 554c 545f 534c 5552 4d5f 4749 545f 5343  ULT_SLURM_GIT_SC
-00005d60: 5249 5054 5f50 4154 4829 0a20 2020 2020  RIPT_PATH).     
-00005d70: 2020 2073 6c75 726d 5f73 6372 6970 745f     slurm_script_
-00005d80: 7265 706f 203d 2063 6f6e 6669 6773 2e67  repo = configs.g
-00005d90: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-00005da0: 2253 4c55 524d 222c 2022 736c 7572 6d5f  "SLURM", "slurm_
-00005db0: 7363 7269 7074 5f72 6570 6f22 2c0a 2020  script_repo",.  
-00005dc0: 2020 2020 2020 2020 2020 6661 6c6c 6261            fallba
-00005dd0: 636b 3d4e 6f6e 650a 2020 2020 2020 2020  ck=None.        
-00005de0: 290a 2020 2020 2020 2020 2320 4372 6561  ).        # Crea
-00005df0: 7465 2074 6865 2053 6c75 726d 436c 6965  te the SlurmClie
-00005e00: 6e74 206f 626a 6563 7420 7769 7468 2074  nt object with t
-00005e10: 6865 2070 6172 616d 6574 6572 7320 7265  he parameters re
-00005e20: 6164 2066 726f 6d0a 2020 2020 2020 2020  ad from.        
-00005e30: 2320 7468 6520 636f 6e66 6967 2066 696c  # the config fil
-00005e40: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00005e50: 2063 6c73 2868 6f73 743d 686f 7374 2c0a   cls(host=host,.
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
-00005e80: 763d 696e 6c69 6e65 5f73 7368 5f65 6e76  v=inline_ssh_env
-00005e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005ea0: 2020 2020 2073 6c75 726d 5f64 6174 615f       slurm_data_
-00005eb0: 7061 7468 3d73 6c75 726d 5f64 6174 615f  path=slurm_data_
-00005ec0: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
-00005ed0: 2020 2020 2020 2020 2073 6c75 726d 5f69           slurm_i
-00005ee0: 6d61 6765 735f 7061 7468 3d73 6c75 726d  mages_path=slurm
-00005ef0: 5f69 6d61 6765 735f 7061 7468 2c0a 2020  _images_path,.  
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2073 6c75 726d 5f63 6f6e 7665 7274 6572   slurm_converter
-00005f20: 735f 7061 7468 3d73 6c75 726d 5f63 6f6e  s_path=slurm_con
-00005f30: 7665 7274 6572 735f 7061 7468 2c0a 2020  verters_path,.  
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f50: 2073 6c75 726d 5f6d 6f64 656c 5f70 6174   slurm_model_pat
-00005f60: 6873 3d73 6c75 726d 5f6d 6f64 656c 5f70  hs=slurm_model_p
-00005f70: 6174 6873 2c0a 2020 2020 2020 2020 2020  aths,.          
-00005f80: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
-00005f90: 6f64 656c 5f72 6570 6f73 3d73 6c75 726d  odel_repos=slurm
-00005fa0: 5f6d 6f64 656c 5f72 6570 6f73 2c0a 2020  _model_repos,.  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2073 6c75 726d 5f6d 6f64 656c 5f69 6d61   slurm_model_ima
-00005fd0: 6765 733d 4e6f 6e65 2c0a 2020 2020 2020  ges=None,.      
-00005fe0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00005ff0: 726d 5f6d 6f64 656c 5f6a 6f62 733d 736c  rm_model_jobs=sl
-00006000: 7572 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a  urm_model_jobs,.
-00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006020: 2020 2073 6c75 726d 5f6d 6f64 656c 5f6a     slurm_model_j
-00006030: 6f62 735f 7061 7261 6d73 3d73 6c75 726d  obs_params=slurm
-00006040: 5f6d 6f64 656c 5f6a 6f62 735f 7061 7261  _model_jobs_para
-00006050: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-00006060: 2020 2020 2020 2073 6c75 726d 5f73 6372         slurm_scr
-00006070: 6970 745f 7061 7468 3d73 6c75 726d 5f73  ipt_path=slurm_s
-00006080: 6372 6970 745f 7061 7468 2c0a 2020 2020  cript_path,.    
-00006090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000060a0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-000060b0: 3d73 6c75 726d 5f73 6372 6970 745f 7265  =slurm_script_re
-000060c0: 706f 2c0a 2020 2020 2020 2020 2020 2020  po,.            
-000060d0: 2020 2020 2020 2069 6e69 745f 736c 7572         init_slur
-000060e0: 6d3d 696e 6974 5f73 6c75 726d 290a 0a20  m=init_slurm).. 
-000060f0: 2020 2064 6566 2063 6c65 616e 7570 5f74     def cleanup_t
-00006100: 6d70 5f66 696c 6573 2873 656c 662c 0a20  mp_files(self,. 
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
-00006130: 6f62 5f69 643a 2073 7472 2c0a 2020 2020  ob_id: str,.    
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
-00006160: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-00006170: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006180: 6174 615f 6c6f 6361 7469 6f6e 3a20 7374  ata_location: st
-00006190: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 6c6f 6766 696c 653a 2073 7472      logfile: str
-000061c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2029 202d 3e20 5265 7375 6c74 3a0a     ) -> Result:.
-000061f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006200: 2020 2020 436c 6561 6e75 7020 7a69 7020      Cleanup zip 
-00006210: 616e 6420 756e 7a69 7070 6564 2066 696c  and unzipped fil
-00006220: 6573 2f66 6f6c 6465 7273 2061 7373 6f63  es/folders assoc
-00006230: 6961 7465 6420 7769 7468 2061 2053 6c75  iated with a Slu
-00006240: 726d 206a 6f62 2e0a 0a20 2020 2020 2020  rm job...       
-00006250: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00006260: 2020 2073 6c75 726d 5f6a 6f62 5f69 6420     slurm_job_id 
-00006270: 2873 7472 293a 2054 6865 206a 6f62 2049  (str): The job I
-00006280: 4420 6f66 2074 6865 2053 6c75 726d 2073  D of the Slurm s
-00006290: 6372 6970 742e 0a20 2020 2020 2020 2020  cript..         
-000062a0: 2020 2066 696c 656e 616d 6520 2873 7472     filename (str
-000062b0: 293a 2054 6865 207a 6970 2066 696c 656e  ): The zip filen
-000062c0: 616d 6520 6f6e 2053 6c75 726d 2e0a 2020  ame on Slurm..  
-000062d0: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
-000062e0: 6f63 6174 696f 6e20 2873 7472 2c20 6f70  ocation (str, op
-000062f0: 7469 6f6e 616c 293a 2054 6865 206c 6f63  tional): The loc
-00006300: 6174 696f 6e20 6f66 2064 6174 6120 6669  ation of data fi
-00006310: 6c65 7320 6f6e 2053 6c75 726d 2e0a 2020  les on Slurm..  
-00006320: 2020 2020 2020 2020 2020 2020 2020 4966                If
-00006330: 206e 6f74 2070 726f 7669 6465 642c 2069   not provided, i
-00006340: 7420 7769 6c6c 2062 6520 6578 7472 6163  t will be extrac
-00006350: 7465 6420 6672 6f6d 2074 6865 206c 6f67  ted from the log
-00006360: 2066 696c 652e 0a20 2020 2020 2020 2020   file..         
-00006370: 2020 206c 6f67 6669 6c65 2028 7374 722c     logfile (str,
-00006380: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00006390: 6c6f 6720 6669 6c65 206f 6620 7468 6520  log file of the 
-000063a0: 536c 7572 6d20 6a6f 622e 200a 2020 2020  Slurm job. .    
-000063b0: 2020 2020 2020 2020 2020 2020 4966 206e              If n
-000063c0: 6f74 2070 726f 7669 6465 642c 2061 2064  ot provided, a d
-000063d0: 6566 6175 6c74 206c 6f67 2066 696c 6520  efault log file 
-000063e0: 7769 6c6c 2062 6520 7573 6564 2e0a 0a20  will be used... 
-000063f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00006400: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
-00006410: 6c74 3a20 5468 6520 7265 7375 6c74 206f  lt: The result o
-00006420: 6620 7468 6520 636c 6561 6e75 7020 6f70  f the cleanup op
-00006430: 6572 6174 696f 6e2e 0a0a 2020 2020 2020  eration...      
-00006440: 2020 4e6f 7465 3a0a 2020 2020 2020 2020    Note:.        
-00006450: 2020 2020 5468 6520 636c 6561 6e75 7020      The cleanup 
-00006460: 7072 6f63 6573 7320 696e 766f 6c76 6573  process involves
-00006470: 2072 656d 6f76 696e 6720 7468 6520 7370   removing the sp
-00006480: 6563 6966 6965 6420 7a69 7020 6669 6c65  ecified zip file
-00006490: 2c20 0a20 2020 2020 2020 2020 2020 2074  , .            t
-000064a0: 6865 206c 6f67 2066 696c 652c 2061 6e64  he log file, and
-000064b0: 2061 7373 6f63 6961 7465 6420 6461 7461   associated data
-000064c0: 2066 696c 6573 2061 6e64 2066 6f6c 6465   files and folde
-000064d0: 7273 2e0a 0a20 2020 2020 2020 2045 7861  rs...        Exa
-000064e0: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-000064f0: 2020 2320 436c 6561 6e75 7020 7465 6d70    # Cleanup temp
-00006500: 6f72 6172 7920 6669 6c65 7320 666f 7220  orary files for 
-00006510: 6120 536c 7572 6d20 6a6f 620a 2020 2020  a Slurm job.    
-00006520: 2020 2020 2020 2020 636c 6965 6e74 2e63          client.c
-00006530: 6c65 616e 7570 5f74 6d70 5f66 696c 6573  leanup_tmp_files
-00006540: 2822 3132 3334 3522 2c20 226f 7574 7075  ("12345", "outpu
-00006550: 742e 7a69 7022 290a 2020 2020 2020 2020  t.zip").        
-00006560: 2222 220a 2020 2020 2020 2020 636d 6473  """.        cmds
-00006570: 203d 205b 5d0a 2020 2020 2020 2020 2320   = [].        # 
-00006580: 7a69 700a 2020 2020 2020 2020 726d 7a69  zip.        rmzi
-00006590: 7020 3d20 6622 726d 207b 6669 6c65 6e61  p = f"rm {filena
-000065a0: 6d65 7d2e 2a22 0a20 2020 2020 2020 2063  me}.*".        c
-000065b0: 6d64 732e 6170 7065 6e64 2872 6d7a 6970  mds.append(rmzip
-000065c0: 290a 2020 2020 2020 2020 2320 6c6f 670a  ).        # log.
-000065d0: 2020 2020 2020 2020 6966 206c 6f67 6669          if logfi
-000065e0: 6c65 2069 7320 4e6f 6e65 3a0a 2020 2020  le is None:.    
-000065f0: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
-00006600: 3d20 7365 6c66 2e5f 4c4f 4746 494c 450a  = self._LOGFILE.
-00006610: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
-00006620: 696c 6520 3d20 6c6f 6766 696c 652e 666f  ile = logfile.fo
-00006630: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
-00006640: 643d 736c 7572 6d5f 6a6f 625f 6964 290a  d=slurm_job_id).
-00006650: 2020 2020 2020 2020 726d 6c6f 6720 3d20          rmlog = 
-00006660: 6622 726d 207b 6c6f 6766 696c 657d 220a  f"rm {logfile}".
-00006670: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
-00006680: 656e 6428 726d 6c6f 6729 0a20 2020 2020  end(rmlog).     
-00006690: 2020 2023 2064 6174 610a 2020 2020 2020     # data.      
-000066a0: 2020 6966 2064 6174 615f 6c6f 6361 7469    if data_locati
-000066b0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-000066c0: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
-000066d0: 6174 696f 6e20 3d20 7365 6c66 2e65 7874  ation = self.ext
-000066e0: 7261 6374 5f64 6174 615f 6c6f 6361 7469  ract_data_locati
-000066f0: 6f6e 5f66 726f 6d5f 6c6f 6728 6c6f 6766  on_from_log(logf
-00006700: 696c 6529 0a20 2020 2020 2020 2072 6d64  ile).        rmd
-00006710: 6174 6120 3d20 6622 726d 202d 7266 207b  ata = f"rm -rf {
-00006720: 6461 7461 5f6c 6f63 6174 696f 6e7d 207b  data_location} {
-00006730: 6461 7461 5f6c 6f63 6174 696f 6e7d 2e2a  data_location}.*
-00006740: 220a 2020 2020 2020 2020 636d 6473 2e61  ".        cmds.a
-00006750: 7070 656e 6428 726d 6461 7461 290a 0a20  ppend(rmdata).. 
-00006760: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00006770: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00006780: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00006790: 6473 2863 6d64 7329 0a20 2020 2020 2020  ds(cmds).       
-000067a0: 2065 7863 6570 7420 556e 6578 7065 6374   except Unexpect
-000067b0: 6564 4578 6974 2061 7320 653a 0a20 2020  edExit as e:.   
-000067c0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000067d0: 7761 726e 696e 6728 6529 0a20 2020 2020  warning(e).     
-000067e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000067f0: 652e 7265 7375 6c74 0a20 2020 2020 2020  e.result.       
-00006800: 2072 6574 7572 6e20 7265 7375 6c74 206f   return result o
-00006810: 7220 4e6f 6e65 0a0a 2020 2020 6465 6620  r None..    def 
-00006820: 7661 6c69 6461 7465 2873 656c 662c 2076  validate(self, v
-00006830: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
-00006840: 7475 703a 2062 6f6f 6c20 3d20 4661 6c73  tup: bool = Fals
-00006850: 6529 3a0a 2020 2020 2020 2020 2222 2256  e):.        """V
-00006860: 616c 6964 6174 6520 7468 6520 636f 6e6e  alidate the conn
-00006870: 6563 7469 6f6e 2074 6f20 7468 6520 536c  ection to the Sl
-00006880: 7572 6d20 636c 7573 7465 7220 6279 2072  urm cluster by r
-00006890: 756e 6e69 6e67 0a20 2020 2020 2020 2061  unning.        a
-000068a0: 2073 696d 706c 6520 636f 6d6d 616e 642e   simple command.
-000068b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000068c0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-000068d0: 6461 7465 5f73 6c75 726d 5f73 6574 7570  date_slurm_setup
-000068e0: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-000068f0: 2074 6f20 616c 736f 2063 6865 636b 0a20   to also check. 
-00006900: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00006910: 6e64 2066 6978 2074 6865 2053 6c75 726d  nd fix the Slurm
-00006920: 2073 6574 7570 2028 666f 6c64 6572 732c   setup (folders,
-00006930: 2069 6d61 6765 732c 2065 7463 2e29 0a0a   images, etc.)..
-00006940: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00006950: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
-00006960: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00006970: 2020 2054 7275 6520 6966 2074 6865 2076     True if the v
-00006980: 616c 6964 6174 696f 6e20 6973 2073 7563  alidation is suc
-00006990: 6365 7373 6675 6c2c 0a20 2020 2020 2020  cessful,.       
-000069a0: 2020 2020 2020 2020 2046 616c 7365 206f           False o
-000069b0: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
-000069c0: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
-000069d0: 6e6e 6563 7465 6420 3d20 7365 6c66 2e72  nnected = self.r
-000069e0: 756e 2827 6563 686f 2022 2022 2729 2e6f  un('echo " "').o
-000069f0: 6b0a 2020 2020 2020 2020 6966 2063 6f6e  k.        if con
-00006a00: 6e65 6374 6564 2061 6e64 2076 616c 6964  nected and valid
-00006a10: 6174 655f 736c 7572 6d5f 7365 7475 703a  ate_slurm_setup:
-00006a20: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00006a30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006a40: 2020 7365 6c66 2e73 6574 7570 5f73 6c75    self.setup_slu
-00006a50: 726d 2829 0a20 2020 2020 2020 2020 2020  rm().           
-00006a60: 2065 7863 6570 7420 5353 4845 7863 6570   except SSHExcep
-00006a70: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00006a80: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00006a90: 722e 6572 726f 7228 6529 0a20 2020 2020  r.error(e).     
-00006aa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006ab0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00006ac0: 7265 7475 726e 2063 6f6e 6e65 6374 6564  return connected
-00006ad0: 0a0a 2020 2020 6465 6620 6765 745f 7265  ..    def get_re
-00006ae0: 6365 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64  cent_log_command
-00006af0: 2873 656c 662c 206c 6f67 5f66 696c 653a  (self, log_file:
-00006b00: 2073 7472 2c20 6e3a 2069 6e74 203d 2031   str, n: int = 1
-00006b10: 3029 202d 3e20 7374 723a 0a20 2020 2020  0) -> str:.     
-00006b20: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00006b30: 6574 2074 6865 2063 6f6d 6d61 6e64 2074  et the command t
-00006b40: 6f20 7265 7472 6965 7665 2074 6865 2072  o retrieve the r
-00006b50: 6563 656e 7420 6c6f 6720 656e 7472 6965  ecent log entrie
-00006b60: 7320 6672 6f6d 2061 0a20 2020 2020 2020  s from a.       
-00006b70: 2073 7065 6369 6669 6564 206c 6f67 2066   specified log f
-00006b80: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
-00006b90: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00006ba0: 6c6f 675f 6669 6c65 2028 7374 7229 3a20  log_file (str): 
-00006bb0: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
-00006bc0: 6c6f 6720 6669 6c65 2e0a 2020 2020 2020  log file..      
-00006bd0: 2020 2020 2020 6e20 2869 6e74 2c20 6f70        n (int, op
-00006be0: 7469 6f6e 616c 293a 2054 6865 206e 756d  tional): The num
-00006bf0: 6265 7220 6f66 2072 6563 656e 7420 6c6f  ber of recent lo
-00006c00: 6720 656e 7472 6965 7320 746f 2072 6574  g entries to ret
-00006c10: 7269 6576 652e 0a20 2020 2020 2020 2020  rieve..         
-00006c20: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00006c30: 746f 2031 302e 0a0a 2020 2020 2020 2020  to 10...        
-00006c40: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00006c50: 2020 2020 2073 7472 3a20 5468 6520 636f       str: The co
-00006c60: 6d6d 616e 6420 746f 2072 6574 7269 6576  mmand to retriev
-00006c70: 6520 7468 6520 7265 6365 6e74 206c 6f67  e the recent log
-00006c80: 2065 6e74 7269 6573 2e0a 2020 2020 2020   entries..      
-00006c90: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00006ca0: 7475 726e 2073 656c 662e 5f54 4149 4c5f  turn self._TAIL_
-00006cb0: 4c4f 475f 434d 442e 666f 726d 6174 286e  LOG_CMD.format(n
-00006cc0: 3d6e 2c20 6c6f 675f 6669 6c65 3d6c 6f67  =n, log_file=log
-00006cd0: 5f66 696c 6529 0a0a 2020 2020 6465 6620  _file)..    def 
-00006ce0: 6765 745f 6163 7469 7665 5f6a 6f62 5f70  get_active_job_p
-00006cf0: 726f 6772 6573 7328 7365 6c66 2c0a 2020  rogress(self,.  
-00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d10: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00006d20: 7572 6d5f 6a6f 625f 6964 3a20 7374 722c  urm_job_id: str,
-00006d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d50: 2070 6174 7465 726e 3a20 7374 7220 3d20   pattern: str = 
-00006d60: 7222 5c64 2b25 222c 0a20 2020 2020 2020  r"\d+%",.       
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-00006d90: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00006da0: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
-00006db0: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
-00006dc0: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
-00006dd0: 6865 2070 726f 6772 6573 7320 6f66 2061  he progress of a
-00006de0: 6e20 6163 7469 7665 2053 6c75 726d 206a  n active Slurm j
-00006df0: 6f62 2066 726f 6d20 6974 7320 6c6f 6766  ob from its logf
-00006e00: 696c 6573 2e0a 0a20 2020 2020 2020 2041  iles...        A
-00006e10: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00006e20: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
-00006e30: 7472 293a 2054 6865 2049 4420 6f66 2074  tr): The ID of t
-00006e40: 6865 2053 6c75 726d 206a 6f62 2e0a 2020  he Slurm job..  
-00006e50: 2020 2020 2020 2020 2020 7061 7474 6572            patter
-00006e60: 6e20 2873 7472 293a 2054 6865 2070 6174  n (str): The pat
-00006e70: 7465 726e 2074 6f20 6d61 7463 6820 696e  tern to match in
-00006e80: 2074 6865 206a 6f62 206c 6f67 2074 6f20   the job log to 
-00006e90: 6578 7472 6163 740a 2020 2020 2020 2020  extract.        
-00006ea0: 2020 2020 2020 2020 7468 6520 7072 6f67          the prog
-00006eb0: 7265 7373 2028 6465 6661 756c 743a 2072  ress (default: r
-00006ec0: 225c 642b 2522 292e 0a0a 2020 2020 2020  "\d+%")...      
-00006ed0: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-00006ee0: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-00006ef0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-00006f00: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00006f10: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
-00006f20: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
-00006f30: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-00006f40: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-00006f50: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-00006f60: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00006f70: 2020 2020 2020 2073 7472 3a20 5468 6520         str: The 
-00006f80: 7072 6f67 7265 7373 206f 6620 7468 6520  progress of the 
-00006f90: 536c 7572 6d20 6a6f 622e 0a20 2020 2020  Slurm job..     
-00006fa0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
-00006fb0: 6d64 6c69 7374 203d 205b 5d0a 2020 2020  mdlist = [].    
-00006fc0: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
-00006fd0: 6574 5f72 6563 656e 745f 6c6f 675f 636f  et_recent_log_co
-00006fe0: 6d6d 616e 6428 0a20 2020 2020 2020 2020  mmand(.         
-00006ff0: 2020 206c 6f67 5f66 696c 653d 7365 6c66     log_file=self
-00007000: 2e5f 4c4f 4746 494c 452e 666f 726d 6174  ._LOGFILE.format
-00007010: 2873 6c75 726d 5f6a 6f62 5f69 643d 736c  (slurm_job_id=sl
-00007020: 7572 6d5f 6a6f 625f 6964 2929 0a20 2020  urm_job_id)).   
-00007030: 2020 2020 2063 6d64 6c69 7374 2e61 7070       cmdlist.app
-00007040: 656e 6428 636d 6429 0a20 2020 2020 2020  end(cmd).       
-00007050: 2069 6620 656e 7620 6973 204e 6f6e 653a   if env is None:
-00007060: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
-00007070: 203d 207b 7d0a 2020 2020 2020 2020 7472   = {}.        tr
-00007080: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-00007090: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-000070a0: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
-000070b0: 742c 2065 6e76 3d65 6e76 290a 2020 2020  t, env=env).    
-000070c0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000070d0: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-000070e0: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-000070f0: 726f 7228 6622 4973 7375 6520 7769 7468  ror(f"Issue with
-00007100: 2072 756e 2063 6f6d 6d61 6e64 3a20 7b65   run command: {e
-00007110: 7d22 290a 2020 2020 2020 2020 2320 4d61  }").        # Ma
-00007120: 7463 6820 7468 6520 7370 6563 6966 6965  tch the specifie
-00007130: 6420 7061 7474 6572 6e20 696e 2074 6865  d pattern in the
-00007140: 2072 6573 756c 7427 7320 7374 646f 7574   result's stdout
-00007150: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00007160: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
-00007170: 5f70 726f 6772 6573 7320 3d20 7265 2e66  _progress = re.f
-00007180: 696e 6461 6c6c 280a 2020 2020 2020 2020  indall(.        
-00007190: 2020 2020 2020 2020 7061 7474 6572 6e2c          pattern,
-000071a0: 2072 6573 756c 742e 7374 646f 7574 295b   result.stdout)[
-000071b0: 2d31 5d0a 2020 2020 2020 2020 6578 6365  -1].        exce
-000071c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000071d0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-000071e0: 6f67 6765 722e 6572 726f 7228 6622 4973  ogger.error(f"Is
-000071f0: 7375 6520 7769 7468 2065 7874 7261 6374  sue with extract
-00007200: 696e 6720 7072 6f67 7265 7373 3a20 7b65  ing progress: {e
-00007210: 7d22 290a 0a20 2020 2020 2020 2072 6574  }")..        ret
-00007220: 7572 6e20 6622 5072 6f67 7265 7373 3a20  urn f"Progress: 
-00007230: 7b6c 6174 6573 745f 7072 6f67 7265 7373  {latest_progress
-00007240: 7d5c 6e22 0a0a 2020 2020 6465 6620 7275  }\n"..    def ru
-00007250: 6e5f 636f 6d6d 616e 6473 2873 656c 662c  n_commands(self,
-00007260: 2063 6d64 6c69 7374 3a20 4c69 7374 5b73   cmdlist: List[s
-00007270: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00007280: 2020 2020 2020 2020 2020 656e 763a 204f            env: O
-00007290: 7074 696f 6e61 6c5b 4469 6374 5b73 7472  ptional[Dict[str
-000072a0: 2c20 7374 725d 5d20 3d20 4e6f 6e65 2c0a  , str]] = None,.
-000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2073 6570 3a20 7374 7220 3d20       sep: str = 
-000072d0: 2720 2626 2027 2c0a 2020 2020 2020 2020  ' && ',.        
-000072e0: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-000072f0: 7761 7267 7329 202d 3e20 5265 7375 6c74  wargs) -> Result
-00007300: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007310: 2020 2020 2020 5275 6e20 6120 6c69 7374        Run a list
-00007320: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
-00007330: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
-00007340: 206f 6e20 7468 6520 536c 7572 6d20 636c   on the Slurm cl
-00007350: 7573 7465 722c 0a20 2020 2020 2020 2065  uster,.        e
-00007360: 6e73 7572 696e 6720 7468 6520 7375 6363  nsuring the succ
-00007370: 6573 7320 6f66 2065 6163 6820 6265 666f  ess of each befo
-00007380: 7265 2070 726f 6365 6564 696e 6720 746f  re proceeding to
-00007390: 2074 6865 206e 6578 742e 0a0a 2020 2020   the next...    
-000073a0: 2020 2020 5468 6520 656e 7669 726f 6e6d      The environm
-000073b0: 656e 7420 7661 7269 6162 6c65 7320 6361  ent variables ca
-000073c0: 6e20 6265 2073 6574 2075 7369 6e67 2074  n be set using t
-000073d0: 6865 2060 656e 7660 2061 7267 756d 656e  he `env` argumen
-000073e0: 742e 0a20 2020 2020 2020 2054 6865 7365  t..        These
-000073f0: 2063 6f6d 6d61 6e64 7320 7265 7461 696e   commands retain
-00007400: 2074 6865 2073 616d 6520 7365 7373 696f   the same sessio
-00007410: 6e20 2865 6e76 6972 6f6e 6d65 6e74 2076  n (environment v
-00007420: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
-00007430: 2065 7463 2e29 2c20 756e 6c69 6b65 2072   etc.), unlike r
-00007440: 756e 6e69 6e67 2074 6865 6d20 7365 7061  unning them sepa
-00007450: 7261 7465 6c79 2e0a 0a20 2020 2020 2020  rately...       
-00007460: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00007470: 2020 2063 6d64 6c69 7374 2028 4c69 7374     cmdlist (List
-00007480: 5b73 7472 5d29 3a20 4120 6c69 7374 206f  [str]): A list o
-00007490: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
-000074a0: 2074 6f20 7275 6e20 6f6e 2053 6c75 726d   to run on Slurm
-000074b0: 2e0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-000074c0: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
-000074d0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
-000074e0: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
-000074f0: 6e74 2076 6172 6961 626c 6573 2074 6f0a  nt variables to.
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 7365 7420 7768 656e 2072 756e 6e69 6e67  set when running
-00007520: 2074 6865 2063 6f6d 6d61 6e64 2e20 4465   the command. De
-00007530: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00007540: 2020 2020 2020 2020 2020 2020 7365 7020              sep 
-00007550: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00007560: 2054 6865 2073 6570 6172 6174 6f72 2075   The separator u
-00007570: 7365 6420 746f 2063 6f6e 6361 7465 6e61  sed to concatena
-00007580: 7465 2074 6865 200a 2020 2020 2020 2020  te the .        
-00007590: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-000075a0: 2e20 4465 6661 756c 7473 2074 6f20 2720  . Defaults to ' 
-000075b0: 2626 2027 2e0a 2020 2020 2020 2020 2020  && '..          
-000075c0: 2020 2a2a 6b77 6172 6773 3a20 4164 6469    **kwargs: Addi
-000075d0: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
-000075e0: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
-000075f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00007600: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
-00007610: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
-00007620: 6520 6c61 7374 2063 6f6d 6d61 6e64 2069  e last command i
-00007630: 6e20 7468 6520 6c69 7374 2e0a 2020 2020  n the list..    
-00007640: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007650: 6966 2065 6e76 2069 7320 4e6f 6e65 3a0a  if env is None:.
-00007660: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00007670: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
-00007680: 203d 2073 6570 2e6a 6f69 6e28 636d 646c   = sep.join(cmdl
-00007690: 6973 7429 0a20 2020 2020 2020 206c 6f67  ist).        log
-000076a0: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
-000076b0: 2020 2020 2020 6622 5275 6e6e 696e 6720        f"Running 
-000076c0: 636f 6d6d 616e 6473 2c20 7769 7468 2065  commands, with e
-000076d0: 6e76 207b 656e 767d 2061 6e64 2073 6570  nv {env} and sep
-000076e0: 207b 7365 707d 205c 0a20 2020 2020 2020   {sep} \.       
-000076f0: 2020 2020 2020 2020 2061 6e64 207b 6b77           and {kw
-00007700: 6172 6773 7d3a 207b 636d 647d 2229 0a20  args}: {cmd}"). 
-00007710: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00007720: 7365 6c66 2e72 756e 2863 6d64 2c20 656e  self.run(cmd, en
-00007730: 763d 656e 762c 202a 2a6b 7761 7267 7329  v=env, **kwargs)
-00007740: 2020 2320 6f75 745f 7374 7265 616d 3d6f    # out_stream=o
-00007750: 7574 5f73 7472 6561 6d2c 0a0a 2020 2020  ut_stream,..    
-00007760: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00007770: 2020 2020 2023 2057 6174 6368 206f 7574       # Watch out
-00007780: 2066 6f72 2055 6e69 636f 6465 456e 636f   for UnicodeEnco
-00007790: 6465 4572 726f 7220 7768 656e 2079 6f75  deError when you
-000077a0: 2073 7472 2829 2074 6869 732e 0a20 2020   str() this..   
-000077b0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000077c0: 696e 666f 2866 227b 7265 7375 6c74 2e73  info(f"{result.s
-000077d0: 7464 6f75 747d 2229 0a20 2020 2020 2020  tdout}").       
-000077e0: 2065 7863 6570 7420 556e 6963 6f64 6545   except UnicodeE
-000077f0: 6e63 6f64 6545 7272 6f72 2061 7320 653a  ncodeError as e:
-00007800: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00007810: 6765 722e 6572 726f 7228 6622 556e 6963  ger.error(f"Unic
-00007820: 6f64 6520 6572 726f 723a 207b 657d 2229  ode error: {e}")
-00007830: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00007840: 4f44 4f3a 204f 4e4c 5920 7374 646f 7574  ODO: ONLY stdout
-00007850: 2052 4543 4f44 4520 4e45 4544 4544 3f3f   RECODE NEEDED??
-00007860: 206f 7220 616c 736f 2065 7272 6f72 3f0a   or also error?.
-00007870: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00007880: 6c74 2e73 7464 6f75 7420 3d20 7265 7375  lt.stdout = resu
-00007890: 6c74 2e73 7464 6f75 742e 656e 636f 6465  lt.stdout.encode
-000078a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000078b0: 2020 2775 7466 2d38 272c 2027 6967 6e6f    'utf-8', 'igno
-000078c0: 7265 2729 2e64 6563 6f64 6528 2775 7466  re').decode('utf
-000078d0: 2d38 2729 0a20 2020 2020 2020 2072 6574  -8').        ret
-000078e0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000078f0: 6465 6620 7374 725f 746f 5f63 6c61 7373  def str_to_class
-00007900: 2873 656c 662c 206d 6f64 756c 655f 6e61  (self, module_na
-00007910: 6d65 3a20 7374 722c 2063 6c61 7373 5f6e  me: str, class_n
-00007920: 616d 653a 2073 7472 2c20 2a61 7267 732c  ame: str, *args,
-00007930: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00007940: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007950: 5265 7475 726e 2061 2063 6c61 7373 2069  Return a class i
-00007960: 6e73 7461 6e63 6520 6672 6f6d 2061 2073  nstance from a s
-00007970: 7472 696e 6720 7265 6665 7265 6e63 652e  tring reference.
-00007980: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00007990: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
-000079a0: 6c65 5f6e 616d 6520 2873 7472 293a 2054  le_name (str): T
-000079b0: 6865 206e 616d 6520 6f66 2074 6865 206d  he name of the m
-000079c0: 6f64 756c 652e 0a20 2020 2020 2020 2020  odule..         
-000079d0: 2020 2063 6c61 7373 5f6e 616d 6520 2873     class_name (s
-000079e0: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-000079f0: 2074 6865 2063 6c61 7373 2e0a 2020 2020   the class..    
-00007a00: 2020 2020 2020 2020 2a61 7267 733a 2041          *args: A
-00007a10: 6464 6974 696f 6e61 6c20 706f 7369 7469  dditional positi
-00007a20: 6f6e 616c 2061 7267 756d 656e 7473 2066  onal arguments f
-00007a30: 6f72 2074 6865 2063 6c61 7373 2063 6f6e  or the class con
-00007a40: 7374 7275 6374 6f72 2e0a 2020 2020 2020  structor..      
-00007a50: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-00007a60: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-00007a70: 7264 2061 7267 756d 656e 7473 2066 6f72  rd arguments for
-00007a80: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
-00007a90: 7275 6374 6f72 2e0a 0a20 2020 2020 2020  ructor...       
-00007aa0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00007ab0: 2020 2020 2020 6f62 6a65 6374 3a20 416e        object: An
-00007ac0: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-00007ad0: 2073 7065 6369 6669 6564 2063 6c61 7373   specified class
-00007ae0: 2c20 6f72 204e 6f6e 6520 6966 2074 6865  , or None if the
-00007af0: 2063 6c61 7373 206f 720a 2020 2020 2020   class or.      
-00007b00: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
-00007b10: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-00007b20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007b30: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00007b40: 2020 2020 2020 6d6f 6475 6c65 5f20 3d20        module_ = 
-00007b50: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-00007b60: 5f6d 6f64 756c 6528 6d6f 6475 6c65 5f6e  _module(module_n
-00007b70: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00007b80: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00007b90: 2020 2020 2020 636c 6173 735f 203d 2067        class_ = g
-00007ba0: 6574 6174 7472 286d 6f64 756c 655f 2c20  etattr(module_, 
-00007bb0: 636c 6173 735f 6e61 6d65 2928 2a61 7267  class_name)(*arg
-00007bc0: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
-00007bd0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00007be0: 4174 7472 6962 7574 6545 7272 6f72 3a0a  AttributeError:.
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 6c6f 6767 6572 2e65 7272 6f72 2827 436c  logger.error('Cl
-00007c10: 6173 7320 646f 6573 206e 6f74 2065 7869  ass does not exi
-00007c20: 7374 2729 0a20 2020 2020 2020 2065 7863  st').        exc
-00007c30: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
-00007c40: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00007c50: 6765 722e 6572 726f 7228 274d 6f64 756c  ger.error('Modul
-00007c60: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
-00007c70: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00007c80: 6e20 636c 6173 735f 206f 7220 4e6f 6e65  n class_ or None
-00007c90: 0a0a 2020 2020 6465 6620 7275 6e5f 636f  ..    def run_co
-00007ca0: 6d6d 616e 6473 5f73 706c 6974 5f6f 7574  mmands_split_out
-00007cb0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 636d 646c 6973 743a 204c        cmdlist: L
-00007ce0: 6973 745b 7374 725d 2c0a 2020 2020 2020  ist[str],.      
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-00007d10: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00007d20: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00007d50: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-00007d60: 2020 2020 2022 2222 5275 6e20 6120 6c69       """Run a li
-00007d70: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
-00007d80: 616e 6473 2063 6f6e 7365 6375 7469 7665  ands consecutive
-00007d90: 6c79 2061 6e64 2073 706c 6974 2074 6865  ly and split the
-00007da0: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00007db0: 6f66 2065 6163 6820 636f 6d6d 616e 642e  of each command.
-00007dc0: 0a0a 2020 2020 2020 2020 4561 6368 2063  ..        Each c
-00007dd0: 6f6d 6d61 6e64 2069 6e20 7468 6520 6c69  ommand in the li
-00007de0: 7374 2069 7320 6578 6563 7574 6564 2077  st is executed w
-00007df0: 6974 6820 6120 7365 7061 7261 746f 7220  ith a separator 
-00007e00: 696e 2062 6574 7765 656e 0a20 2020 2020  in between.     
-00007e10: 2020 2074 6861 7420 6973 2075 6e69 7175     that is uniqu
-00007e20: 6520 616e 6420 6361 6e20 6265 2075 7365  e and can be use
-00007e30: 6420 746f 2073 706c 6974 0a20 2020 2020  d to split.     
-00007e40: 2020 2074 6865 206f 7574 7075 7420 6f66     the output of
-00007e50: 2065 6163 6820 636f 6d6d 616e 6420 6c61   each command la
-00007e60: 7465 722e 2054 6865 2073 6570 6172 6174  ter. The separat
-00007e70: 6f72 2075 7365 6420 6973 2073 7065 6369  or used is speci
-00007e80: 6669 6564 0a20 2020 2020 2020 2062 7920  fied.        by 
-00007e90: 7468 6520 605f 4f55 545f 5345 5060 2061  the `_OUT_SEP` a
-00007ea0: 7474 7269 6275 7465 206f 6620 7468 650a  ttribute of the.
-00007eb0: 2020 2020 2020 2020 536c 7572 6d43 6c69          SlurmCli
-00007ec0: 656e 7420 696e 7374 616e 6365 2e0a 0a20  ent instance... 
-00007ed0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00007ee0: 2020 2020 2020 2020 2063 6d64 6c69 7374           cmdlist
-00007ef0: 2028 4c69 7374 5b73 7472 5d29 3a20 4120   (List[str]): A 
-00007f00: 6c69 7374 206f 6620 7368 656c 6c20 636f  list of shell co
-00007f10: 6d6d 616e 6473 2074 6f20 7275 6e2e 0a20  mmands to run.. 
-00007f20: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
-00007f30: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
-00007f40: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
-00007f50: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
-00007f60: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
-00007f70: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
-00007f80: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-00007f90: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-00007fa0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
-00007fb0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00007fc0: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00007fd0: 5b73 7472 5d3a 0a20 2020 2020 2020 2020  [str]:.         
-00007fe0: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
-00007ff0: 2073 7472 696e 6773 2c20 7768 6572 6520   strings, where 
-00008000: 6561 6368 2073 7472 696e 6720 636f 7272  each string corr
-00008010: 6573 706f 6e64 7320 746f 0a20 2020 2020  esponds to.     
-00008020: 2020 2020 2020 2020 2020 2074 6865 206f             the o
-00008030: 7574 7075 7420 6f66 2061 2073 696e 676c  utput of a singl
-00008040: 6520 636f 6d6d 616e 6420 696e 2060 636d  e command in `cm
-00008050: 646c 6973 7460 2073 706c 6974 0a20 2020  dlist` split.   
-00008060: 2020 2020 2020 2020 2020 2020 2062 7920               by 
-00008070: 7468 6520 7365 7061 7261 746f 7220 605f  the separator `_
-00008080: 4f55 545f 5345 5060 2e0a 0a20 2020 2020  OUT_SEP`...     
-00008090: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-000080a0: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
-000080b0: 696f 6e3a 2049 6620 616e 7920 6f66 2074  ion: If any of t
-000080c0: 6865 2063 6f6d 6d61 6e64 7320 6661 696c  he commands fail
-000080d0: 2074 6f20 6578 6563 7574 6520 7375 6363   to execute succ
-000080e0: 6573 7366 756c 6c79 2e0a 2020 2020 2020  essfully..      
-000080f0: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00008100: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-00008110: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-00008120: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
-00008130: 743d 636d 646c 6973 742c 0a20 2020 2020  t=cmdlist,.     
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 656e 763d 656e 762c 0a20 2020 2020    env=env,.     
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 7365 703d 6622 203b 2065 6368 6f20    sep=f" ; echo 
-000081a0: 7b73 656c 662e 5f4f 5554 5f53 4550 7d20  {self._OUT_SEP} 
-000081b0: 3b20 2229 0a20 2020 2020 2020 2065 7863  ; ").        exc
-000081c0: 6570 7420 556e 6578 7065 6374 6564 4578  ept UnexpectedEx
-000081d0: 6974 2061 7320 653a 0a20 2020 2020 2020  it as e:.       
-000081e0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-000081f0: 696e 6728 6529 0a20 2020 2020 2020 2020  ing(e).         
-00008200: 2020 2072 6573 756c 7420 3d20 652e 7265     result = e.re
-00008210: 7375 6c74 0a20 2020 2020 2020 2069 6620  sult.        if 
-00008220: 7265 7375 6c74 2e6f 6b3a 0a20 2020 2020  result.ok:.     
-00008230: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00008240: 3d20 7265 7375 6c74 2e73 7464 6f75 740a  = result.stdout.
-00008250: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
-00008260: 745f 7265 7370 6f6e 7365 7320 3d20 7265  t_responses = re
-00008270: 7370 6f6e 7365 2e73 706c 6974 2873 656c  sponse.split(sel
-00008280: 662e 5f4f 5554 5f53 4550 290a 2020 2020  f._OUT_SEP).    
-00008290: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000082a0: 706c 6974 5f72 6573 706f 6e73 6573 0a20  plit_responses. 
-000082b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000082c0: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
-000082d0: 6520 7265 7375 6c74 2069 7320 6e6f 7420  e result is not 
-000082e0: 6f6b 2c20 6c6f 6720 7468 6520 6572 726f  ok, log the erro
-000082f0: 7220 616e 6420 7261 6973 6520 616e 2053  r and raise an S
-00008300: 5348 4578 6365 7074 696f 6e0a 2020 2020  SHException.    
-00008310: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
-00008320: 6622 5265 7375 6c74 2069 7320 6e6f 7420  f"Result is not 
-00008330: 6f6b 3a20 7b72 6573 756c 747d 220a 2020  ok: {result}".  
-00008340: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00008350: 2e65 7272 6f72 2865 7272 6f72 290a 2020  .error(error).  
-00008360: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00008370: 5353 4845 7863 6570 7469 6f6e 2865 7272  SSHException(err
-00008380: 6f72 290a 0a20 2020 2064 6566 206c 6973  or)..    def lis
-00008390: 745f 6163 7469 7665 5f6a 6f62 7328 7365  t_active_jobs(se
-000083a0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-000083b0: 2020 2020 2020 2020 2020 2020 2065 6e76               env
-000083c0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-000083d0: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
-000083e0: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-000083f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008400: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
-00008410: 6f66 2061 6374 6976 6520 6a6f 6273 2066  of active jobs f
-00008420: 726f 6d20 534c 5552 4d2e 0a0a 2020 2020  rom SLURM...    
-00008430: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00008440: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-00008450: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-00008460: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-00008470: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00008480: 626c 6573 2074 6f20 0a20 2020 2020 2020  bles to .       
-00008490: 2020 2020 2020 2020 2073 6574 2077 6865           set whe
-000084a0: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-000084b0: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-000084c0: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-000084d0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000084e0: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
-000084f0: 3a20 4120 6c69 7374 206f 6620 6a6f 6220  : A list of job 
-00008500: 4944 732e 0a20 2020 2020 2020 2022 2222  IDs..        """
-00008510: 0a20 2020 2020 2020 2023 2063 6d64 203d  .        # cmd =
-00008520: 2073 656c 662e 5f41 4354 4956 455f 4a4f   self._ACTIVE_JO
-00008530: 4253 5f43 4d44 0a20 2020 2020 2020 2063  BS_CMD.        c
-00008540: 6d64 203d 2073 656c 662e 6765 745f 6a6f  md = self.get_jo
-00008550: 6273 5f69 6e66 6f5f 636f 6d6d 616e 6428  bs_info_command(
-00008560: 7374 6172 745f 7469 6d65 3d22 6e6f 7722  start_time="now"
-00008570: 2c20 7374 6174 6573 3d22 7222 290a 2020  , states="r").  
-00008580: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00008590: 6f28 2252 6574 7269 6576 696e 6720 6c69  o("Retrieving li
-000085a0: 7374 206f 6620 6163 7469 7665 206a 6f62  st of active job
-000085b0: 7320 6672 6f6d 2053 6c75 726d 2229 0a20  s from Slurm"). 
-000085c0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000085d0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-000085e0: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
-000085f0: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
-00008600: 7374 203d 2072 6573 756c 742e 7374 646f  st = result.stdo
-00008610: 7574 2e73 7472 6970 2829 2e73 706c 6974  ut.strip().split
-00008620: 2827 5c6e 2729 0a20 2020 2020 2020 206a  ('\n').        j
-00008630: 6f62 5f6c 6973 742e 7265 7665 7273 6528  ob_list.reverse(
-00008640: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00008650: 206a 6f62 5f6c 6973 740a 0a20 2020 2064   job_list..    d
-00008660: 6566 206c 6973 745f 636f 6d70 6c65 7465  ef list_complete
-00008670: 645f 6a6f 6273 2873 656c 662c 0a20 2020  d_jobs(self,.   
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-000086a0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-000086b0: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
-000086c0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-000086d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000086e0: 2047 6574 2061 206c 6973 7420 6f66 2063   Get a list of c
-000086f0: 6f6d 706c 6574 6564 206a 6f62 7320 6672  ompleted jobs fr
-00008700: 6f6d 2053 4c55 524d 2e0a 0a20 2020 2020  om SLURM...     
-00008710: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00008720: 2020 2020 2065 6e76 2028 4469 6374 5b73       env (Dict[s
-00008730: 7472 2c20 7374 725d 2c20 6f70 7469 6f6e  tr, str], option
-00008740: 616c 293a 204f 7074 696f 6e61 6c20 656e  al): Optional en
-00008750: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00008760: 6c65 7320 746f 0a20 2020 2020 2020 2020  les to.         
-00008770: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
-00008780: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00008790: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-000087a0: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-000087b0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000087c0: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
-000087d0: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
-000087e0: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
-000087f0: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00008800: 6c66 2e67 6574 5f6a 6f62 735f 696e 666f  lf.get_jobs_info
-00008810: 5f63 6f6d 6d61 6e64 2873 7461 7465 733d  _command(states=
-00008820: 2263 6422 290a 2020 2020 2020 2020 6c6f  "cd").        lo
-00008830: 6767 6572 2e69 6e66 6f28 2252 6574 7269  gger.info("Retri
-00008840: 6576 696e 6720 6120 6c69 7374 206f 6620  eving a list of 
-00008850: 636f 6d70 6c65 7465 6420 6a6f 6273 2066  completed jobs f
-00008860: 726f 6d20 536c 7572 6d22 290a 2020 2020  rom Slurm").    
-00008870: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00008880: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-00008890: 636d 645d 2c20 656e 763d 656e 7629 0a20  cmd], env=env). 
-000088a0: 2020 2020 2020 206a 6f62 5f6c 6973 7420         job_list 
-000088b0: 3d20 5b6a 6f62 2e73 7472 6970 2829 2066  = [job.strip() f
-000088c0: 6f72 206a 6f62 2069 6e20 7265 7375 6c74  or job in result
-000088d0: 2e73 7464 6f75 742e 7374 7269 7028 292e  .stdout.strip().
-000088e0: 7370 6c69 7428 275c 6e27 295d 0a20 2020  split('\n')].   
-000088f0: 2020 2020 206a 6f62 5f6c 6973 742e 7265       job_list.re
-00008900: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
-00008910: 7265 7475 726e 206a 6f62 5f6c 6973 740a  return job_list.
-00008920: 0a20 2020 2064 6566 206c 6973 745f 616c  .    def list_al
-00008930: 6c5f 6a6f 6273 2873 656c 662c 2065 6e76  l_jobs(self, env
-00008940: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00008950: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
-00008960: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-00008970: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008980: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
-00008990: 6f66 2061 6c6c 206a 6f62 7320 6672 6f6d  of all jobs from
-000089a0: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
-000089b0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-000089c0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-000089d0: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-000089e0: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-000089f0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00008a00: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-00008a10: 2020 2074 6f20 7365 7420 7768 656e 2072     to set when r
-00008a20: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
-00008a30: 6e64 2e20 4465 6661 756c 7473 2074 6f20  nd. Defaults to 
-00008a40: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-00008a50: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00008a60: 2020 2020 4c69 7374 5b73 7472 5d3a 2041      List[str]: A
-00008a70: 206c 6973 7420 6f66 206a 6f62 2049 4473   list of job IDs
-00008a80: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00008a90: 2020 2020 2020 2063 6d64 203d 2073 656c         cmd = sel
-00008aa0: 662e 6765 745f 6a6f 6273 5f69 6e66 6f5f  f.get_jobs_info_
-00008ab0: 636f 6d6d 616e 6428 290a 2020 2020 2020  command().      
-00008ac0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2252    logger.info("R
-00008ad0: 6574 7269 6576 696e 6720 6120 6c69 7374  etrieving a list
-00008ae0: 206f 6620 616c 6c20 6a6f 6273 2066 726f   of all jobs fro
-00008af0: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
-00008b00: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00008b10: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-00008b20: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-00008b30: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
-00008b40: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
-00008b50: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
-00008b60: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
-00008b70: 7374 2e72 6576 6572 7365 2829 0a20 2020  st.reverse().   
-00008b80: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
-00008b90: 6c69 7374 0a0a 2020 2020 6465 6620 6765  list..    def ge
-00008ba0: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
-00008bb0: 616e 6428 7365 6c66 2c20 7374 6172 745f  and(self, start_
-00008bc0: 7469 6d65 3a20 7374 7220 3d20 2232 3032  time: str = "202
-00008bd0: 332d 3031 2d30 3122 2c0a 2020 2020 2020  3-01-01",.      
-00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bf0: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
-00008c00: 3a20 7374 7220 3d20 226e 6f77 222c 0a20  : str = "now",. 
-00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c20: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00008c30: 756d 6e73 3a20 7374 7220 3d20 224a 6f62  umns: str = "Job
-00008c40: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
-00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c60: 2020 2073 7461 7465 733a 2073 7472 203d     states: str =
-00008c70: 2022 722c 6364 2c66 2c74 6f2c 7273 2c64   "r,cd,f,to,rs,d
-00008c80: 6c2c 6e66 2229 202d 3e20 7374 723a 0a20  l,nf") -> str:. 
-00008c90: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00008ca0: 2074 6865 2053 6c75 726d 2063 6f6d 6d61   the Slurm comma
-00008cb0: 6e64 2074 6f20 7265 7472 6965 7665 2069  nd to retrieve i
-00008cc0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00008cd0: 206f 6c64 206a 6f62 732e 0a0a 2020 2020   old jobs...    
-00008ce0: 2020 2020 5468 6520 636f 6d6d 616e 6420      The command 
-00008cf0: 7769 6c6c 2062 6520 666f 726d 6174 7465  will be formatte
-00008d00: 6420 7769 7468 2074 6865 2073 7065 6369  d with the speci
-00008d10: 6669 6564 2073 7461 7274 2074 696d 652c  fied start time,
-00008d20: 2077 6869 6368 2069 730a 2020 2020 2020   which is.      
-00008d30: 2020 6578 7065 6374 6564 2074 6f20 6265    expected to be
-00008d40: 2069 6e20 7468 6520 4953 4f20 666f 726d   in the ISO form
-00008d50: 6174 2022 5959 5959 2d4d 4d2d 4444 222e  at "YYYY-MM-DD".
-00008d60: 0a20 2020 2020 2020 2054 6865 2063 6f6d  .        The com
-00008d70: 6d61 6e64 2077 696c 6c20 7573 6520 7468  mand will use th
-00008d80: 6520 2273 6163 6374 2220 746f 6f6c 2074  e "sacct" tool t
-00008d90: 6f20 7175 6572 7920 7468 650a 2020 2020  o query the.    
-00008da0: 2020 2020 536c 7572 6d20 6163 636f 756e      Slurm accoun
-00008db0: 7469 6e67 2064 6174 6162 6173 6520 666f  ting database fo
-00008dc0: 7220 6a6f 6273 2074 6861 7420 7374 6172  r jobs that star
-00008dd0: 7465 6420 6f6e 206f 7220 6166 7465 7220  ted on or after 
-00008de0: 7468 650a 2020 2020 2020 2020 7370 6563  the.        spec
-00008df0: 6966 6965 6420 7374 6172 7420 7469 6d65  ified start time
-00008e00: 2c20 616e 6420 7769 6c6c 206f 7574 7075  , and will outpu
-00008e10: 7420 6f6e 6c79 2074 6865 206a 6f62 2049  t only the job I
-00008e20: 4473 2028 2d6f 204a 6f62 4964 290a 2020  Ds (-o JobId).  
-00008e30: 2020 2020 2020 7769 7468 6f75 7420 6865        without he
-00008e40: 6164 6572 206f 7220 7472 6169 6c65 7220  ader or trailer 
-00008e50: 6c69 6e65 7320 282d 6e20 2d58 292e 0a0a  lines (-n -X)...
-00008e60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00008e70: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-00008e80: 7469 6d65 2028 7374 7229 3a20 5468 6520  time (str): The 
-00008e90: 7374 6172 7420 7469 6d65 2066 726f 6d20  start time from 
-00008ea0: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
-00008eb0: 6520 6a6f 620a 2020 2020 2020 2020 2020  e job.          
-00008ec0: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-00008ed0: 6e2e 2044 6566 6175 6c74 7320 746f 2022  n. Defaults to "
-00008ee0: 3230 3233 2d30 312d 3031 222e 0a20 2020  2023-01-01"..   
-00008ef0: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
-00008f00: 6520 2873 7472 293a 2054 6865 2065 6e64  e (str): The end
-00008f10: 2074 696d 6520 756e 7469 6c20 7768 6963   time until whic
-00008f20: 6820 746f 2072 6574 7269 6576 6520 6a6f  h to retrieve jo
-00008f30: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00008f40: 2020 696e 666f 726d 6174 696f 6e2e 2044    information. D
-00008f50: 6566 6175 6c74 7320 746f 2022 6e6f 7722  efaults to "now"
-00008f60: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00008f70: 6c75 6d6e 7320 2873 7472 293a 2054 6865  lumns (str): The
-00008f80: 2063 6f6c 756d 6e73 2074 6f20 7265 7472   columns to retr
-00008f90: 6965 7665 2066 726f 6d20 7468 6520 6a6f  ieve from the jo
-00008fa0: 6220 696e 666f 726d 6174 696f 6e2e 0a20  b information.. 
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00008fc0: 6566 6175 6c74 7320 746f 2022 4a6f 6249  efaults to "JobI
-00008fd0: 6422 2e20 4974 2069 7320 636f 6d6d 6120  d". It is comma 
-00008fe0: 7365 7061 7261 7465 642c 2065 2e67 2e20  separated, e.g. 
-00008ff0: 224a 6f62 4964 2c53 7461 7465 222e 0a20  "JobId,State".. 
-00009000: 2020 2020 2020 2020 2020 2073 7461 7465             state
-00009010: 7320 2873 7472 293a 2054 6865 206a 6f62  s (str): The job
-00009020: 2073 7461 7465 7320 746f 2069 6e63 6c75   states to inclu
-00009030: 6465 2069 6e20 7468 6520 7175 6572 792e  de in the query.
-00009040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009050: 2044 6566 6175 6c74 7320 746f 2022 722c   Defaults to "r,
-00009060: 6364 2c66 2c74 6f2c 7273 2c64 6c2c 6e66  cd,f,to,rs,dl,nf
-00009070: 222e 0a0a 2020 2020 2020 2020 5265 7475  "...        Retu
-00009080: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00009090: 2073 7472 3a0a 2020 2020 2020 2020 2020   str:.          
-000090a0: 2020 2020 2020 4120 7374 7269 6e67 2072        A string r
-000090b0: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-000090c0: 536c 7572 6d20 636f 6d6d 616e 6420 746f  Slurm command to
-000090d0: 2072 6574 7269 6576 650a 2020 2020 2020   retrieve.      
-000090e0: 2020 2020 2020 2020 2020 696e 666f 726d            inform
-000090f0: 6174 696f 6e20 6162 6f75 7420 6f6c 6420  ation about old 
-00009100: 6a6f 6273 2e0a 2020 2020 2020 2020 2222  jobs..        ""
-00009110: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00009120: 2073 656c 662e 5f41 4c4c 5f4a 4f42 535f   self._ALL_JOBS_
-00009130: 434d 442e 666f 726d 6174 2873 7461 7274  CMD.format(start
-00009140: 5f74 696d 653d 7374 6172 745f 7469 6d65  _time=start_time
-00009150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 2020 2020 2065 6e64 5f74             end_t
-00009180: 696d 653d 656e 645f 7469 6d65 2c0a 2020  ime=end_time,.  
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091b0: 2020 2020 2020 2073 7461 7465 733d 7374         states=st
-000091c0: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000091f0: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 290a  olumns=columns).
-00009200: 0a20 2020 2064 6566 2074 7261 6e73 6665  .    def transfe
-00009210: 725f 6461 7461 2873 656c 662c 206c 6f63  r_data(self, loc
-00009220: 616c 5f70 6174 683a 2073 7472 2920 2d3e  al_path: str) ->
-00009230: 2052 6573 756c 743a 0a20 2020 2020 2020   Result:.       
-00009240: 2022 2222 0a20 2020 2020 2020 2054 7261   """.        Tra
-00009250: 6e73 6665 7273 2061 2066 696c 6520 6f72  nsfers a file or
-00009260: 2064 6972 6563 746f 7279 2066 726f 6d20   directory from 
-00009270: 7468 6520 6c6f 6361 6c20 6d61 6368 696e  the local machin
-00009280: 6520 746f 2074 6865 2072 656d 6f74 650a  e to the remote.
-00009290: 2020 2020 2020 2020 536c 7572 6d20 636c          Slurm cl
-000092a0: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
-000092b0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000092c0: 2020 6c6f 6361 6c5f 7061 7468 2028 7374    local_path (st
-000092d0: 7229 3a20 5468 6520 6c6f 6361 6c20 7061  r): The local pa
-000092e0: 7468 2074 6f20 7468 6520 6669 6c65 206f  th to the file o
-000092f0: 7220 6469 7265 6374 6f72 7920 746f 0a20  r directory to. 
-00009300: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00009310: 7261 6e73 6665 722e 0a0a 2020 2020 2020  ransfer...      
-00009320: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00009330: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
-00009340: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-00009350: 2066 696c 6520 7472 616e 7366 6572 206f   file transfer o
-00009360: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
-00009370: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
-00009380: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-00009390: 2020 2020 2020 2066 2254 7261 6e73 6665         f"Transfe
-000093a0: 7269 6e67 2066 696c 6520 7b6c 6f63 616c  ring file {local
-000093b0: 5f70 6174 687d 2074 6f20 7b73 656c 662e  _path} to {self.
-000093c0: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-000093d0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-000093e0: 6e20 7365 6c66 2e70 7574 286c 6f63 616c  n self.put(local
-000093f0: 3d6c 6f63 616c 5f70 6174 682c 2072 656d  =local_path, rem
-00009400: 6f74 653d 7365 6c66 2e73 6c75 726d 5f64  ote=self.slurm_d
-00009410: 6174 615f 7061 7468 290a 0a20 2020 2064  ata_path)..    d
-00009420: 6566 2075 6e70 6163 6b5f 6461 7461 2873  ef unpack_data(s
-00009430: 656c 662c 207a 6970 6669 6c65 3a20 7374  elf, zipfile: st
-00009440: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00009450: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00009460: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00009470: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-00009480: 5265 7375 6c74 3a0a 2020 2020 2020 2020  Result:.        
-00009490: 2222 220a 2020 2020 2020 2020 556e 7061  """.        Unpa
-000094a0: 636b 7320 6120 7a69 7070 6564 2066 696c  cks a zipped fil
-000094b0: 6520 6f6e 2074 6865 2072 656d 6f74 6520  e on the remote 
-000094c0: 536c 7572 6d20 636c 7573 7465 722e 0a0a  Slurm cluster...
-000094d0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000094e0: 2020 2020 2020 2020 2020 7a69 7066 696c            zipfil
-000094f0: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
-00009500: 6520 6f66 2074 6865 207a 6970 7065 6420  e of the zipped 
-00009510: 6669 6c65 2074 6f20 6265 2075 6e70 6163  file to be unpac
-00009520: 6b65 642e 0a0a 2020 2020 2020 2020 2020  ked...          
-00009530: 2020 656e 7620 2844 6963 745b 7374 722c    env (Dict[str,
-00009540: 2073 7472 5d2c 206f 7074 696f 6e61 6c29   str], optional)
-00009550: 3a20 4f70 7469 6f6e 616c 2065 6e76 6972  : Optional envir
-00009560: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00009570: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00009580: 2020 746f 2073 6574 2077 6865 6e20 7275    to set when ru
-00009590: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-000095a0: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
-000095b0: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
-000095c0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000095d0: 2020 2052 6573 756c 743a 2054 6865 2072     Result: The r
-000095e0: 6573 756c 7420 6f66 2074 6865 2063 6f6d  esult of the com
-000095f0: 6d61 6e64 2e0a 2020 2020 2020 2020 2222  mand..        ""
-00009600: 220a 2020 2020 2020 2020 636d 6420 3d20  ".        cmd = 
-00009610: 7365 6c66 2e67 6574 5f75 6e7a 6970 5f63  self.get_unzip_c
-00009620: 6f6d 6d61 6e64 287a 6970 6669 6c65 290a  ommand(zipfile).
-00009630: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00009640: 6e66 6f28 6622 556e 7061 636b 696e 6720  nfo(f"Unpacking 
-00009650: 7b7a 6970 6669 6c65 7d20 6f6e 2053 6c75  {zipfile} on Slu
-00009660: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
-00009670: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
-00009680: 6d61 6e64 7328 5b63 6d64 5d2c 2065 6e76  mands([cmd], env
-00009690: 3d65 6e76 290a 0a20 2020 2064 6566 2063  =env)..    def c
-000096a0: 6f6e 7665 7274 5f64 6174 6128 7365 6c66  onvert_data(self
-000096b0: 2c20 7a69 7066 696c 653a 2073 7472 2c0a  , zipfile: str,.
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
-000096e0: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
-000096f0: 5d5d 203d 204e 6f6e 6529 202d 3e20 5265  ]] = None) -> Re
-00009700: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
-00009710: 220a 2020 2020 2020 2020 556e 7061 636b  ".        Unpack
-00009720: 7320 6120 7a69 7070 6564 2066 696c 6520  s a zipped file 
-00009730: 6f6e 2074 6865 2072 656d 6f74 6520 536c  on the remote Sl
-00009740: 7572 6d20 636c 7573 7465 722e 0a0a 2020  urm cluster...  
-00009750: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009760: 2020 2020 2020 2020 7a69 7066 696c 6520          zipfile 
-00009770: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
-00009780: 6f66 2074 6865 207a 6970 7065 6420 6669  of the zipped fi
-00009790: 6c65 2074 6f20 6265 2075 6e70 6163 6b65  le to be unpacke
-000097a0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-000097b0: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
-000097c0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-000097d0: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
-000097e0: 6d65 6e74 2076 6172 6961 626c 6573 200a  ment variables .
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 746f 2073 6574 2077 6865 6e20 7275 6e6e  to set when runn
-00009810: 696e 6720 7468 6520 636f 6d6d 616e 642e  ing the command.
-00009820: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00009830: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00009840: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00009850: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
-00009860: 756c 7420 6f66 2074 6865 2063 6f6d 6d61  ult of the comma
-00009870: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
-00009880: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00009890: 6c66 2e67 6574 5f63 6f6e 7665 7274 5f63  lf.get_convert_c
-000098a0: 6f6d 6d61 6e64 287a 6970 6669 6c65 290a  ommand(zipfile).
-000098b0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-000098c0: 6e66 6f28 6622 436f 6e76 6572 7469 6e67  nfo(f"Converting
-000098d0: 207b 7a69 7066 696c 657d 206f 6e20 536c   {zipfile} on Sl
-000098e0: 7572 6d22 290a 2020 2020 2020 2020 7265  urm").        re
-000098f0: 7475 726e 2073 656c 662e 7275 6e5f 636f  turn self.run_co
-00009900: 6d6d 616e 6473 285b 636d 645d 2c20 656e  mmands([cmd], en
-00009910: 763d 656e 7629 0a0a 2020 2020 6465 6620  v=env)..    def 
-00009920: 6765 6e65 7261 7465 5f73 6c75 726d 5f6a  generate_slurm_j
-00009930: 6f62 5f66 6f72 5f77 6f72 6b66 6c6f 7728  ob_for_workflow(
-00009940: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-00009970: 726b 666c 6f77 3a20 7374 722c 0a20 2020  rkflow: str,.   
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2020 2073 7562 7374 6974 7574 6573       substitutes
-000099b0: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-000099c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
-000099f0: 7465 3a20 7374 7220 3d20 226a 6f62 5f74  te: str = "job_t
-00009a00: 656d 706c 6174 652e 7368 220a 2020 2020  emplate.sh".    
-00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2020 2920 2d3e 2073 7472 3a0a 2020      ) -> str:.  
-00009a40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00009a50: 2020 4765 6e65 7261 7465 2061 2053 6c75    Generate a Slu
-00009a60: 726d 206a 6f62 2073 6372 6970 7420 666f  rm job script fo
-00009a70: 7220 6120 7370 6563 6966 6963 2077 6f72  r a specific wor
-00009a80: 6b66 6c6f 772e 0a0a 2020 2020 2020 2020  kflow...        
-00009a90: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00009aa0: 2020 776f 726b 666c 6f77 2028 7374 7229    workflow (str)
-00009ab0: 3a20 5468 6520 6e61 6d65 206f 6620 7468  : The name of th
-00009ac0: 6520 776f 726b 666c 6f77 2e0a 2020 2020  e workflow..    
-00009ad0: 2020 2020 2020 2020 7375 6273 7469 7475          substitu
-00009ae0: 7465 7320 2844 6963 745b 7374 722c 2073  tes (Dict[str, s
-00009af0: 7472 5d29 3a20 4120 6469 6374 696f 6e61  tr]): A dictiona
-00009b00: 7279 2063 6f6e 7461 696e 696e 6720 6b65  ry containing ke
-00009b10: 792d 7661 6c75 650a 2020 2020 2020 2020  y-value.        
-00009b20: 2020 2020 2020 2020 7061 6972 7320 666f          pairs fo
-00009b30: 7220 7375 6273 7469 7475 7469 6e67 2070  r substituting p
-00009b40: 6c61 6365 686f 6c64 6572 7320 696e 2074  laceholders in t
-00009b50: 6865 206a 6f62 2074 656d 706c 6174 652e  he job template.
-00009b60: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00009b70: 706c 6174 6520 2873 7472 2c20 6f70 7469  plate (str, opti
-00009b80: 6f6e 616c 293a 2054 6865 2066 696c 656e  onal): The filen
-00009b90: 616d 6520 6f66 2074 6865 206a 6f62 2074  ame of the job t
-00009ba0: 656d 706c 6174 652e 0a20 2020 2020 2020  emplate..       
-00009bb0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00009bc0: 7320 746f 2022 6a6f 625f 7465 6d70 6c61  s to "job_templa
-00009bd0: 7465 2e73 6822 2e0a 0a20 2020 2020 2020  te.sh"...       
-00009be0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00009bf0: 2020 2020 2020 7374 723a 2054 6865 2067        str: The g
-00009c00: 656e 6572 6174 6564 2053 6c75 726d 206a  enerated Slurm j
-00009c10: 6f62 2073 6372 6970 7420 6173 2061 2073  ob script as a s
-00009c20: 7472 696e 672e 0a20 2020 2020 2020 2022  tring..        "
-00009c30: 2222 0a20 2020 2020 2020 2023 2061 6464  "".        # add
-00009c40: 2077 6f72 6b66 6c6f 7720 746f 2073 7562   workflow to sub
-00009c50: 7374 6974 7574 6573 0a20 2020 2020 2020  stitutes.       
-00009c60: 2073 7562 7374 6974 7574 6573 5b27 6a6f   substitutes['jo
-00009c70: 626e 616d 6527 5d20 3d20 776f 726b 666c  bname'] = workfl
-00009c80: 6f77 0a20 2020 2020 2020 2023 2067 7261  ow.        # gra
-00009c90: 6220 6a6f 6220 7465 6d70 6c61 7465 0a20  b job template. 
-00009ca0: 2020 2020 2020 2074 656d 706c 6174 655f         template_
-00009cb0: 6620 3d20 6669 6c65 7328 2272 6573 6f75  f = files("resou
-00009cc0: 7263 6573 2229 2e6a 6f69 6e70 6174 6828  rces").joinpath(
-00009cd0: 7465 6d70 6c61 7465 290a 2020 2020 2020  template).      
-00009ce0: 2020 7769 7468 2074 656d 706c 6174 655f    with template_
-00009cf0: 662e 6f70 656e 2827 7227 2920 6173 2066  f.open('r') as f
-00009d00: 3a0a 2020 2020 2020 2020 2020 2020 7372  :.            sr
-00009d10: 6320 3d20 5465 6d70 6c61 7465 2866 2e72  c = Template(f.r
-00009d20: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
-00009d30: 2020 206a 6f62 5f73 6372 6970 7420 3d20     job_script = 
-00009d40: 7372 632e 7361 6665 5f73 7562 7374 6974  src.safe_substit
-00009d50: 7574 6528 7375 6273 7469 7475 7465 7329  ute(substitutes)
-00009d60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009d70: 6a6f 625f 7363 7269 7074 0a0a 2020 2020  job_script..    
-00009d80: 6465 6620 776f 726b 666c 6f77 5f70 6172  def workflow_par
-00009d90: 616d 735f 746f 5f73 7562 7328 7365 6c66  ams_to_subs(self
-00009da0: 2c20 7061 7261 6d73 2920 2d3e 2044 6963  , params) -> Dic
-00009db0: 745b 7374 722c 2073 7472 5d3a 0a20 2020  t[str, str]:.   
-00009dc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009dd0: 2043 6f6e 7665 7274 2077 6f72 6b66 6c6f   Convert workflo
-00009de0: 7720 7061 7261 6d65 7465 7273 2074 6f20  w parameters to 
-00009df0: 7375 6273 7469 7475 7469 6f6e 2064 6963  substitution dic
-00009e00: 7469 6f6e 6172 7920 666f 7220 6a6f 6220  tionary for job 
-00009e10: 7363 7269 7074 2e0a 0a20 2020 2020 2020  script...       
-00009e20: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00009e30: 2020 2070 6172 616d 733a 2041 2064 6963     params: A dic
-00009e40: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-00009e50: 6e67 2077 6f72 6b66 6c6f 7720 7061 7261  ng workflow para
-00009e60: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
-00009e70: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00009e80: 2020 2020 2020 4469 6374 5b73 7472 2c20        Dict[str, 
-00009e90: 7374 725d 3a20 4120 6469 6374 696f 6e61  str]: A dictiona
-00009ea0: 7279 2077 6974 6820 7061 7261 6d65 7465  ry with paramete
-00009eb0: 7220 6e61 6d65 7320 6173 206b 6579 7320  r names as keys 
-00009ec0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00009ed0: 2020 2020 636f 7272 6573 706f 6e64 696e      correspondin
-00009ee0: 6720 666c 6167 7320 7769 7468 2070 6c61  g flags with pla
-00009ef0: 6365 686f 6c64 6572 7320 6173 2076 616c  ceholders as val
-00009f00: 7565 732e 0a20 2020 2020 2020 2022 2222  ues..        """
-00009f10: 0a20 2020 2020 2020 2073 7562 7320 3d20  .        subs = 
-00009f20: 7b7d 0a20 2020 2020 2020 2066 6c61 6773  {}.        flags
-00009f30: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-00009f40: 7220 5f2c 2070 6172 616d 2069 6e20 7061  r _, param in pa
-00009f50: 7261 6d73 2e69 7465 6d73 2829 3a0a 2020  rams.items():.  
-00009f60: 2020 2020 2020 2020 2020 666c 6167 203d            flag =
-00009f70: 2070 6172 616d 5b27 636d 645f 666c 6167   param['cmd_flag
-00009f80: 275d 0a20 2020 2020 2020 2020 2020 2066  '].            f
-00009f90: 6c61 6720 3d20 666c 6167 202b 2022 2024  lag = flag + " $
-00009fa0: 2220 2b20 7061 7261 6d5b 276e 616d 6527  " + param['name'
-00009fb0: 5d2e 7570 7065 7228 290a 2020 2020 2020  ].upper().      
-00009fc0: 2020 2020 2020 666c 6167 732e 6170 7065        flags.appe
-00009fd0: 6e64 2866 6c61 6729 0a20 2020 2020 2020  nd(flag).       
-00009fe0: 2073 7562 735b 2750 4152 414d 5327 5d20   subs['PARAMS'] 
-00009ff0: 3d20 2220 222e 6a6f 696e 2866 6c61 6773  = " ".join(flags
-0000a000: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000a010: 2073 7562 730a 0a20 2020 2064 6566 2075   subs..    def u
-0000a020: 7064 6174 655f 736c 7572 6d5f 7363 7269  pdate_slurm_scri
-0000a030: 7074 7328 7365 6c66 2c0a 2020 2020 2020  pts(self,.      
+00003180: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
+00003190: 5f65 6e76 290a 2020 2020 2020 2020 7365  _env).        se
+000031a0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
+000031b0: 7468 203d 2073 6c75 726d 5f64 6174 615f  th = slurm_data_
+000031c0: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
+000031d0: 662e 736c 7572 6d5f 696d 6167 6573 5f70  f.slurm_images_p
+000031e0: 6174 6820 3d20 736c 7572 6d5f 696d 6167  ath = slurm_imag
+000031f0: 6573 5f70 6174 680a 2020 2020 2020 2020  es_path.        
+00003200: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
+00003210: 7274 6572 735f 7061 7468 203d 2073 6c75  rters_path = slu
+00003220: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+00003230: 7468 0a20 2020 2020 2020 2073 656c 662e  th.        self.
+00003240: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
+00003250: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
+00003260: 7061 7468 730a 2020 2020 2020 2020 7365  paths.        se
+00003270: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
+00003280: 7061 7468 203d 2073 6c75 726d 5f73 6372  path = slurm_scr
+00003290: 6970 745f 7061 7468 0a20 2020 2020 2020  ipt_path.       
+000032a0: 2073 656c 662e 736c 7572 6d5f 7363 7269   self.slurm_scri
+000032b0: 7074 5f72 6570 6f20 3d20 736c 7572 6d5f  pt_repo = slurm_
+000032c0: 7363 7269 7074 5f72 6570 6f0a 2020 2020  script_repo.    
+000032d0: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
+000032e0: 6f64 656c 5f72 6570 6f73 203d 2073 6c75  odel_repos = slu
+000032f0: 726d 5f6d 6f64 656c 5f72 6570 6f73 0a20  rm_model_repos. 
+00003300: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
+00003310: 6d5f 6d6f 6465 6c5f 696d 6167 6573 203d  m_model_images =
+00003320: 2073 6c75 726d 5f6d 6f64 656c 5f69 6d61   slurm_model_ima
+00003330: 6765 730a 2020 2020 2020 2020 7365 6c66  ges.        self
+00003340: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
+00003350: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
+00003360: 6a6f 6273 0a20 2020 2020 2020 2073 656c  jobs.        sel
+00003370: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
+00003380: 6273 5f70 6172 616d 7320 3d20 736c 7572  bs_params = slur
+00003390: 6d5f 6d6f 6465 6c5f 6a6f 6273 5f70 6172  m_model_jobs_par
+000033a0: 616d 730a 0a20 2020 2020 2020 2023 2049  ams..        # I
+000033b0: 6e69 7420 6361 6368 652e 204b 6565 7020  nit cache. Keep 
+000033c0: 7265 7370 6f6e 7365 7320 666f 7220 3336  responses for 36
+000033d0: 3020 7365 636f 6e64 730a 2020 2020 2020  0 seconds.      
+000033e0: 2020 7365 6c66 2e63 6163 6865 203d 2072    self.cache = r
+000033f0: 6571 7565 7374 735f 6361 6368 652e 6261  equests_cache.ba
+00003400: 636b 656e 6473 2e73 716c 6974 652e 5351  ckends.sqlite.SQ
+00003410: 4c69 7465 4361 6368 6528 0a20 2020 2020  LiteCache(.     
+00003420: 2020 2020 2020 2064 625f 7061 7468 3d22         db_path="
+00003430: 6769 7468 7562 5f63 6163 6865 222c 2075  github_cache", u
+00003440: 7365 5f74 656d 703d 5472 7565 290a 2020  se_temp=True).  
+00003450: 2020 2020 2020 7365 6c66 2e67 6574 5f6f        self.get_o
+00003460: 725f 6372 6561 7465 5f67 6974 6875 625f  r_create_github_
+00003470: 7365 7373 696f 6e28 290a 0a20 2020 2020  session()..     
+00003480: 2020 2073 656c 662e 696e 6974 5f77 6f72     self.init_wor
+00003490: 6b66 6c6f 7773 2829 0a20 2020 2020 2020  kflows().       
+000034a0: 2073 656c 662e 7661 6c69 6461 7465 2876   self.validate(v
+000034b0: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
+000034c0: 7475 703d 696e 6974 5f73 6c75 726d 290a  tup=init_slurm).
+000034d0: 0a20 2020 2064 6566 2069 6e69 745f 776f  .    def init_wo
+000034e0: 726b 666c 6f77 7328 7365 6c66 2c20 666f  rkflows(self, fo
+000034f0: 7263 655f 7570 6461 7465 3a20 626f 6f6c  rce_update: bool
+00003500: 203d 2046 616c 7365 293a 0a20 2020 2020   = False):.     
+00003510: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00003520: 6574 7269 6576 6573 2074 6865 2072 6571  etrieves the req
+00003530: 7569 7265 6420 696e 666f 2066 6f72 2074  uired info for t
+00003540: 6865 2063 6f6e 6669 6775 7265 6420 776f  he configured wo
+00003550: 726b 666c 6f77 7320 6672 6f6d 2067 6974  rkflows from git
+00003560: 6875 622e 0a20 2020 2020 2020 2049 7420  hub..        It 
+00003570: 7769 6c6c 2066 696c 6c20 6073 6c75 726d  will fill `slurm
+00003580: 5f6d 6f64 656c 5f69 6d61 6765 7360 2077  _model_images` w
+00003590: 6974 6820 646f 636b 6572 6875 6220 6c69  ith dockerhub li
+000035a0: 6e6b 732e 0a0a 2020 2020 2020 2020 4172  nks...        Ar
+000035b0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000035c0: 666f 7263 655f 7570 6461 7465 2028 626f  force_update (bo
+000035d0: 6f6c 293a 2057 696c 6c20 6f76 6572 7772  ol): Will overwr
+000035e0: 6974 6520 616c 7265 6164 7920 6769 7665  ite already give
+000035f0: 6e20 7061 7468 730a 2020 2020 2020 2020  n paths.        
+00003600: 2020 2020 2020 2020 696e 2060 736c 7572          in `slur
+00003610: 6d5f 6d6f 6465 6c5f 696d 6167 6573 600a  m_model_images`.
+00003620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003630: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00003640: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
+00003650: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+00003660: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+00003670: 6c5f 696d 6167 6573 203d 207b 7d0a 2020  l_images = {}.  
+00003680: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00003690: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7265  f.slurm_model_re
+000036a0: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
+000036b0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+000036c0: 224e 6f20 776f 726b 666c 6f77 7320 636f  "No workflows co
+000036d0: 6e66 6967 7572 6564 2122 290a 2020 2020  nfigured!").    
+000036e0: 2020 2020 2020 2020 7365 6c66 2e73 6c75          self.slu
+000036f0: 726d 5f6d 6f64 656c 5f72 6570 6f73 203d  rm_model_repos =
+00003700: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00003710: 2320 736b 6970 7320 7468 6520 7365 7475  # skips the setu
+00003720: 700a 2020 2020 2020 2020 666f 7220 776f  p.        for wo
+00003730: 726b 666c 6f77 2069 6e20 7365 6c66 2e73  rkflow in self.s
+00003740: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
+00003750: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00003760: 2020 2020 2069 6620 776f 726b 666c 6f77       if workflow
+00003770: 206e 6f74 2069 6e20 7365 6c66 2e73 6c75   not in self.slu
+00003780: 726d 5f6d 6f64 656c 5f69 6d61 6765 7320  rm_model_images 
+00003790: 6f72 2066 6f72 6365 5f75 7064 6174 653a  or force_update:
+000037a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037b0: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
+000037c0: 203d 2073 656c 662e 7075 6c6c 5f64 6573   = self.pull_des
+000037d0: 6372 6970 746f 725f 6672 6f6d 5f67 6974  criptor_from_git
+000037e0: 6875 6228 776f 726b 666c 6f77 290a 2020  hub(workflow).  
+000037f0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00003800: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
+00003810: 2573 272c 2077 6f72 6b66 6c6f 772c 206a  %s', workflow, j
+00003820: 736f 6e5f 6465 7363 7269 7074 6f72 290a  son_descriptor).
+00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003840: 696d 6167 6520 3d20 6a73 6f6e 5f64 6573  image = json_des
+00003850: 6372 6970 746f 725b 2763 6f6e 7461 696e  criptor['contain
+00003860: 6572 2d69 6d61 6765 275d 5b27 696d 6167  er-image']['imag
+00003870: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+00003880: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
+00003890: 6f64 656c 5f69 6d61 6765 735b 776f 726b  odel_images[work
+000038a0: 666c 6f77 5d20 3d20 696d 6167 650a 0a20  flow] = image.. 
+000038b0: 2020 2064 6566 2073 6574 7570 5f73 6c75     def setup_slu
+000038c0: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
+000038d0: 2020 2222 220a 2020 2020 2020 2020 5661    """.        Va
+000038e0: 6c69 6461 7465 7320 6f72 2063 7265 6174  lidates or creat
+000038f0: 6573 2074 6865 2072 6571 7569 7265 6420  es the required 
+00003900: 7365 7475 7020 6f6e 2074 6865 2053 6c75  setup on the Slu
+00003910: 726d 2063 6c75 7374 6572 2e0a 0a20 2020  rm cluster...   
+00003920: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+00003930: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
+00003940: 7074 696f 6e3a 2069 6620 6974 2063 616e  ption: if it can
+00003950: 6e6f 7420 636f 6e6e 6563 7420 746f 2053  not connect to S
+00003960: 6c75 726d 2c20 6f72 2072 756e 7320 696e  lurm, or runs in
+00003970: 746f 2061 6e20 6572 726f 720a 2020 2020  to an error.    
+00003980: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00003990: 6966 2073 656c 662e 7661 6c69 6461 7465  if self.validate
+000039a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000039b0: 2320 312e 2043 7265 6174 6520 6469 7265  # 1. Create dire
+000039c0: 6374 6f72 6965 730a 2020 2020 2020 2020  ctories.        
+000039d0: 2020 2020 7365 6c66 2e73 6574 7570 5f64      self.setup_d
+000039e0: 6972 6563 746f 7269 6573 2829 0a0a 2020  irectories()..  
+000039f0: 2020 2020 2020 2020 2020 2320 322e 2043            # 2. C
+00003a00: 6c6f 6e65 2067 6974 0a20 2020 2020 2020  lone git.       
+00003a10: 2020 2020 2073 656c 662e 7365 7475 705f       self.setup_
+00003a20: 6a6f 625f 7363 7269 7074 7328 290a 0a20  job_scripts().. 
+00003a30: 2020 2020 2020 2020 2020 2023 2033 2e20             # 3. 
+00003a40: 5365 7475 7020 636f 6e76 6572 7465 7273  Setup converters
+00003a50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003a60: 662e 7365 7475 705f 636f 6e76 6572 7465  f.setup_converte
+00003a70: 7273 2829 0a0a 2020 2020 2020 2020 2020  rs()..          
+00003a80: 2020 2320 342e 2044 6f77 6e6c 6f61 6420    # 4. Download 
+00003a90: 776f 726b 666c 6f77 2069 6d61 6765 730a  workflow images.
+00003aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003ab0: 2e73 6574 7570 5f63 6f6e 7461 696e 6572  .setup_container
+00003ac0: 5f69 6d61 6765 7328 290a 0a20 2020 2020  _images()..     
+00003ad0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003ae0: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00003af0: 6365 7074 696f 6e28 2246 6169 6c75 7265  ception("Failure
+00003b00: 2069 6e20 636f 6e6e 6563 7469 6e67 2074   in connecting t
+00003b10: 6f20 536c 7572 6d20 636c 7573 7465 7222  o Slurm cluster"
+00003b20: 290a 0a20 2020 2064 6566 2073 6574 7570  )..    def setup
+00003b30: 5f63 6f6e 7461 696e 6572 5f69 6d61 6765  _container_image
+00003b40: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00003b50: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+00003b60: 7320 7570 2063 6f6e 7461 696e 6572 2069  s up container i
+00003b70: 6d61 6765 7320 666f 7220 536c 7572 6d20  mages for Slurm 
+00003b80: 6f70 6572 6174 696f 6e73 2e0a 0a20 2020  operations...   
+00003b90: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00003ba0: 6f6e 2063 7265 6174 6573 2073 7065 6369  on creates speci
+00003bb0: 6669 6320 6469 7265 6374 6f72 6965 7320  fic directories 
+00003bc0: 666f 7220 636f 6e74 6169 6e65 7220 696d  for container im
+00003bd0: 6167 6573 2061 6e64 2070 756c 6c73 0a20  ages and pulls. 
+00003be0: 2020 2020 2020 206e 6563 6573 7361 7279         necessary
+00003bf0: 2069 6d61 6765 7320 6672 6f6d 2044 6f63   images from Doc
+00003c00: 6b65 7220 7265 706f 7369 746f 7269 6573  ker repositories
+00003c10: 2e20 4974 2067 656e 6572 6174 6573 2061  . It generates a
+00003c20: 6e64 2065 7865 6375 7465 730a 2020 2020  nd executes.    
+00003c30: 2020 2020 6120 7363 7269 7074 2074 6f20      a script to 
+00003c40: 7075 6c6c 2069 6d61 6765 7320 616e 6420  pull images and 
+00003c50: 636f 7069 6573 2069 7420 746f 2074 6865  copies it to the
+00003c60: 2072 656d 6f74 6520 6c6f 6361 7469 6f6e   remote location
+00003c70: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00003c80: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+00003c90: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
+00003ca0: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
+00003cb0: 6520 6578 6563 7574 696e 6720 636f 6d6d  e executing comm
+00003cc0: 616e 6473 206f 7220 636f 7079 696e 6720  ands or copying 
+00003cd0: 6669 6c65 732e 0a20 2020 2020 2020 2022  files..        "
+00003ce0: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
+00003cf0: 6174 6520 7370 6563 6966 6963 2077 6f72  ate specific wor
+00003d00: 6b66 6c6f 7720 6469 7273 0a20 2020 2020  kflow dirs.     
+00003d10: 2020 2077 6974 6820 7365 6c66 2e63 6428     with self.cd(
+00003d20: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
+00003d30: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
+00003d40: 2020 2020 2069 6620 7365 6c66 2e73 6c75       if self.slu
+00003d50: 726d 5f6d 6f64 656c 5f70 6174 6873 3a0a  rm_model_paths:.
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 6d6f 6465 6c70 6174 6873 203d 2022 2022  modelpaths = " "
+00003d80: 2e6a 6f69 6e28 7365 6c66 2e73 6c75 726d  .join(self.slurm
+00003d90: 5f6d 6f64 656c 5f70 6174 6873 2e76 616c  _model_paths.val
+00003da0: 7565 7328 2929 0a20 2020 2020 2020 2020  ues()).         
+00003db0: 2020 2020 2020 2023 206d 6b64 6972 2063         # mkdir c
+00003dc0: 656c 6c70 726f 6669 6c65 7220 696d 6167  ellprofiler imag
+00003dd0: 656a 202e 2e2e 0a20 2020 2020 2020 2020  ej ....         
+00003de0: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
+00003df0: 7275 6e5f 636f 6d6d 616e 6473 285b 6622  run_commands([f"
+00003e00: 6d6b 6469 7220 2d70 207b 6d6f 6465 6c70  mkdir -p {modelp
+00003e10: 6174 6873 7d22 5d29 0a20 2020 2020 2020  aths}"]).       
+00003e20: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00003e30: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
+00003e40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00003e50: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+00003e60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003e70: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00003e80: 5f69 6d61 6765 733a 0a20 2020 2020 2020  _images:.       
+00003e90: 2020 2020 2020 2020 2070 756c 6c5f 636f           pull_co
+00003ea0: 6d6d 616e 6473 203d 205b 5d0a 2020 2020  mmands = [].    
+00003eb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00003ec0: 7766 2c20 696d 6167 6520 696e 2073 656c  wf, image in sel
+00003ed0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 696d  f.slurm_model_im
+00003ee0: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 7265 706f 203d 2073 656c 662e 736c    repo = self.sl
+00003f10: 7572 6d5f 6d6f 6465 6c5f 7265 706f 735b  urm_model_repos[
+00003f20: 7766 5d0a 2020 2020 2020 2020 2020 2020  wf].            
+00003f30: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
+00003f40: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+00003f50: 7061 7468 735b 7766 5d0a 2020 2020 2020  paths[wf].      
+00003f60: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
+00003f70: 2076 6572 7369 6f6e 203d 2073 656c 662e   version = self.
+00003f80: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
+00003f90: 6f6d 5f75 726c 2872 6570 6f29 0a20 2020  om_url(repo).   
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 2069 6620 7665 7273 696f 6e20 3d3d 2022   if version == "
+00003fc0: 6d61 7374 6572 223a 0a20 2020 2020 2020  master":.       
+00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fe0: 2076 6572 7369 6f6e 203d 2022 6c61 7465   version = "late
+00003ff0: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
+00004000: 2020 2020 2020 2020 7075 6c6c 5f74 656d          pull_tem
+00004010: 706c 6174 6520 3d20 2265 6368 6f20 2773  plate = "echo 's
+00004020: 7461 7274 696e 6720 2470 6174 6820 2476  tarting $path $v
+00004030: 6572 7369 6f6e 2720 3e3e 2073 696e 672e  ersion' >> sing.
+00004040: 6c6f 675c 6e6e 6f68 7570 2073 6820 2d63  log\nnohup sh -c
+00004050: 205c 2273 696e 6775 6c61 7269 7479 2070   \"singularity p
+00004060: 756c 6c20 2d2d 6469 7361 626c 652d 6361  ull --disable-ca
+00004070: 6368 6520 2d2d 6469 7220 2470 6174 6820  che --dir $path 
+00004080: 646f 636b 6572 3a2f 2f24 696d 6167 653a  docker://$image:
+00004090: 2476 6572 7369 6f6e 3b20 6563 686f 2027  $version; echo '
+000040a0: 6669 6e69 7368 6564 2024 7061 7468 2024  finished $path $
+000040b0: 7665 7273 696f 6e27 5c22 203e 3e20 7369  version'\" >> si
+000040c0: 6e67 2e6c 6f67 2032 3e26 3120 2620 6469  ng.log 2>&1 & di
+000040d0: 736f 776e 220a 2020 2020 2020 2020 2020  sown".          
+000040e0: 2020 2020 2020 2020 2020 7420 3d20 5465            t = Te
+000040f0: 6d70 6c61 7465 2870 756c 6c5f 7465 6d70  mplate(pull_temp
+00004100: 6c61 7465 290a 2020 2020 2020 2020 2020  late).          
+00004110: 2020 2020 2020 2020 2020 7375 6273 7469            substi
+00004120: 7475 7465 7320 3d20 7b7d 0a20 2020 2020  tutes = {}.     
+00004130: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004140: 7562 7374 6974 7574 6573 5b27 7061 7468  ubstitutes['path
+00004150: 275d 203d 2070 6174 680a 2020 2020 2020  '] = path.      
+00004160: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00004170: 6273 7469 7475 7465 735b 2769 6d61 6765  bstitutes['image
+00004180: 275d 203d 2069 6d61 6765 0a20 2020 2020  '] = image.     
+00004190: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000041a0: 7562 7374 6974 7574 6573 5b27 7665 7273  ubstitutes['vers
+000041b0: 696f 6e27 5d20 3d20 7665 7273 696f 6e0a  ion'] = version.
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041d0: 2020 2020 636d 6420 3d20 742e 7361 6665      cmd = t.safe
+000041e0: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+000041f0: 7469 7475 7465 7329 0a20 2020 2020 2020  titutes).       
+00004200: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00004210: 6765 722e 6465 6275 6728 6622 7375 6273  ger.debug(f"subs
+00004220: 7469 7475 7465 643a 207b 636d 647d 2229  tituted: {cmd}")
+00004230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004240: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
+00004250: 6473 2e61 7070 656e 6428 636d 6429 0a20  ds.append(cmd). 
+00004260: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004270: 6372 6970 745f 6e61 6d65 203d 2022 7075  cript_name = "pu
+00004280: 6c6c 5f69 6d61 6765 732e 7368 220a 2020  ll_images.sh".  
+00004290: 2020 2020 2020 2020 2020 2020 2020 7465                te
+000042a0: 6d70 6c61 7465 5f73 6372 6970 7420 3d20  mplate_script = 
+000042b0: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+000042c0: 2229 2e6a 6f69 6e70 6174 6828 7363 7269  ").joinpath(scri
+000042d0: 7074 5f6e 616d 6529 0a20 2020 2020 2020  pt_name).       
+000042e0: 2020 2020 2020 2020 2077 6974 6820 7465           with te
+000042f0: 6d70 6c61 7465 5f73 6372 6970 742e 6f70  mplate_script.op
+00004300: 656e 2827 7227 2920 6173 2066 3a0a 2020  en('r') as f:.  
+00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004320: 2020 7372 6320 3d20 5465 6d70 6c61 7465    src = Template
+00004330: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
+00004340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004350: 7562 7374 6974 7574 6520 3d20 7b27 7075  ubstitute = {'pu
+00004360: 6c6c 636f 6d6d 616e 6473 273a 2022 5c6e  llcommands': "\n
+00004370: 222e 6a6f 696e 2870 756c 6c5f 636f 6d6d  ".join(pull_comm
+00004380: 616e 6473 297d 0a20 2020 2020 2020 2020  ands)}.         
+00004390: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
+000043a0: 6372 6970 7420 3d20 7372 632e 7361 6665  cript = src.safe
+000043b0: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+000043c0: 7469 7475 7465 290a 2020 2020 2020 2020  titute).        
+000043d0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000043e0: 6562 7567 2866 2273 7562 7374 6974 7574  ebug(f"substitut
+000043f0: 6564 3a5c 6e20 7b6a 6f62 5f73 6372 6970  ed:\n {job_scrip
+00004400: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
+00004410: 2020 2020 2023 2063 6f70 7920 746f 2072       # copy to r
+00004420: 656d 6f74 6520 6669 6c65 0a20 2020 2020  emote file.     
+00004430: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+00004440: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
+00004450: 6d5f 696d 6167 6573 5f70 6174 682b 222f  m_images_path+"/
+00004460: 222b 7363 7269 7074 5f6e 616d 650a 2020  "+script_name.  
+00004470: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
+00004480: 3d20 7365 6c66 2e70 7574 286c 6f63 616c  = self.put(local
+00004490: 3d69 6f2e 5374 7269 6e67 494f 286a 6f62  =io.StringIO(job
+000044a0: 5f73 6372 6970 7429 2c0a 2020 2020 2020  _script),.      
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044c0: 2020 2020 2020 2072 656d 6f74 653d 6675         remote=fu
+000044d0: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
+000044e0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+000044f0: 2274 696d 6520 7368 207b 7363 7269 7074  "time sh {script
+00004500: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
+00004510: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+00004520: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
+00004530: 6d64 5d29 0a20 2020 2020 2020 2020 2020  md]).           
+00004540: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
+00004550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004560: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+00004570: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
+00004580: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00004590: 6572 2e69 6e66 6f28 722e 7374 646f 7574  er.info(r.stdout
+000045a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000045b0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2249    logger.info("I
+000045c0: 6e69 7469 6174 6564 2064 6f77 6e6c 6f61  nitiated downloa
+000045d0: 6469 6e67 2061 6e64 2062 7569 6c64 696e  ding and buildin
+000045e0: 6722 202b 0a20 2020 2020 2020 2020 2020  g" +.           
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2022 2063 6f6e 7461 696e 6572 2069 6d61   " container ima
+00004610: 6765 7320 6f6e 2053 6c75 726d 2e22 202b  ges on Slurm." +
+00004620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004630: 2020 2020 2020 2020 2020 2020 2022 2054               " T
+00004640: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
+00004650: 7768 696c 6520 696e 2074 6865 2062 6163  while in the bac
+00004660: 6b67 726f 756e 642e 2220 2b20 0a20 2020  kground." + .   
+00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004680: 2020 2020 2020 2020 2022 2043 6865 636b           " Check
+00004690: 2027 7369 6e67 2e6c 6f67 2720 6f6e 2053   'sing.log' on S
+000046a0: 6c75 726d 2066 6f72 2070 726f 6772 6573  lurm for progres
+000046b0: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
+000046c0: 2020 2020 2023 2023 2063 6c65 616e 7570       # # cleanup
+000046d0: 2067 6961 6e74 2073 696e 6775 6c61 7269   giant singulari
+000046e0: 7479 2063 6163 6865 210a 2020 2020 2020  ty cache!.      
+000046f0: 2020 2020 2020 2020 2020 2320 7573 696e            # usin
+00004700: 6720 2d2d 6469 7361 626c 652d 6361 6368  g --disable-cach
+00004710: 6520 6265 6361 7573 6520 7765 2072 756e  e because we run
+00004720: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
+00004730: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00004740: 2020 2023 2063 6d64 203d 2022 7369 6e67     # cmd = "sing
+00004750: 756c 6172 6974 7920 6361 6368 6520 636c  ularity cache cl
+00004760: 6561 6e20 2d66 220a 2020 2020 2020 2020  ean -f".        
+00004770: 2020 2020 2020 2020 2320 7220 3d20 7365          # r = se
+00004780: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00004790: 5b63 6d64 5d29 0a0a 2020 2020 6465 6620  [cmd])..    def 
+000047a0: 7365 7475 705f 636f 6e76 6572 7465 7273  setup_converters
+000047b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000047c0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
+000047d0: 2075 7020 636f 6e76 6572 7465 7273 2066   up converters f
+000047e0: 6f72 2053 6c75 726d 206f 7065 7261 7469  or Slurm operati
+000047f0: 6f6e 732e 0a0a 2020 2020 2020 2020 5468  ons...        Th
+00004800: 6973 2066 756e 6374 696f 6e20 6372 6561  is function crea
+00004810: 7465 7320 6e65 6365 7373 6172 7920 6469  tes necessary di
+00004820: 7265 6374 6f72 6965 7320 666f 7220 636f  rectories for co
+00004830: 6e76 6572 7465 7273 2061 6e64 2063 6f70  nverters and cop
+00004840: 6965 730a 2020 2020 2020 2020 636f 6e76  ies.        conv
+00004850: 6572 7465 7220 7363 7269 7074 7320 616e  erter scripts an
+00004860: 6420 6465 6669 6e69 7469 6f6e 7320 746f  d definitions to
+00004870: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
+00004880: 206c 6f63 6174 696f 6e73 2e20 4974 2061   locations. It a
+00004890: 6c73 6f0a 2020 2020 2020 2020 6275 696c  lso.        buil
+000048a0: 6473 2053 696e 6775 6c61 7269 7479 2063  ds Singularity c
+000048b0: 6f6e 7461 696e 6572 7320 6672 6f6d 2074  ontainers from t
+000048c0: 6865 2070 726f 7669 6465 6420 6465 6669  he provided defi
+000048d0: 6e69 7469 6f6e 732e 0a0a 2020 2020 2020  nitions...      
+000048e0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+000048f0: 2020 2020 2020 5353 4845 7863 6570 7469        SSHExcepti
+00004900: 6f6e 3a20 4966 2074 6865 7265 2069 7320  on: If there is 
+00004910: 616e 2069 7373 7565 2065 7865 6375 7469  an issue executi
+00004920: 6e67 2063 6f6d 6d61 6e64 7320 6f72 2063  ng commands or c
+00004930: 6f70 7969 6e67 2066 696c 6573 2e0a 2020  opying files..  
+00004940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004950: 2020 636f 6e76 6572 745f 636d 6473 203d    convert_cmds =
+00004960: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
+00004970: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
+00004980: 7465 7273 5f70 6174 683a 0a20 2020 2020  ters_path:.     
+00004990: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
+000049a0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+000049b0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+000049c0: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
+000049d0: 687d 2229 0a20 2020 2020 2020 2072 203d  h}").        r =
+000049e0: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+000049f0: 6473 2863 6f6e 7665 7274 5f63 6d64 7329  ds(convert_cmds)
+00004a00: 0a20 2020 2020 2020 2023 2063 6f70 7920  .        # copy 
+00004a10: 6765 6e65 7269 6320 6a6f 6220 6172 7261  generic job arra
+00004a20: 7920 7363 7269 7074 206f 7665 7220 746f  y script over to
+00004a30: 2073 6c75 726d 0a20 2020 2020 2020 2063   slurm.        c
+00004a40: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
+00004a50: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
+00004a60: 6365 7322 292e 6a6f 696e 7061 7468 280a  ces").joinpath(.
+00004a70: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00004a80: 7665 7274 5f6a 6f62 5f61 7272 6179 2e73  vert_job_array.s
+00004a90: 6822 290a 2020 2020 2020 2020 5f20 3d20  h").        _ = 
+00004aa0: 7365 6c66 2e70 7574 286c 6f63 616c 3d63  self.put(local=c
+00004ab0: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
+00004ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004ad0: 2020 2020 2020 2072 656d 6f74 653d 7365         remote=se
+00004ae0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
+00004af0: 7061 7468 290a 2020 2020 2020 2020 2320  path).        # 
+00004b00: 6375 7272 656e 746c 7920 6b6e 6f77 6e20  currently known 
+00004b10: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
+00004b20: 2020 2023 2033 612e 205a 4152 5220 746f     # 3a. ZARR to
+00004b30: 2054 4946 460a 2020 2020 2020 2020 2320   TIFF.        # 
+00004b40: 544f 444f 2065 7874 7261 6374 2074 6865  TODO extract the
+00004b50: 7365 2076 616c 7565 7320 746f 2065 2e67  se values to e.g
+00004b60: 2e20 636f 6e66 6967 2069 6620 7765 2068  . config if we h
+00004b70: 6176 6520 6d6f 7265 0a20 2020 2020 2020  ave more.       
+00004b80: 2063 6f6e 7665 7274 5f6e 616d 6520 3d20   convert_name = 
+00004b90: 2263 6f6e 7665 7274 5f7a 6172 725f 746f  "convert_zarr_to
+00004ba0: 5f74 6966 6622 0a20 2020 2020 2020 2063  _tiff".        c
+00004bb0: 6f6e 7665 7274 5f70 7920 3d20 6622 7b63  onvert_py = f"{c
+00004bc0: 6f6e 7665 7274 5f6e 616d 657d 2e70 7922  onvert_name}.py"
+00004bd0: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
+00004be0: 5f73 6372 6970 745f 6c6f 6361 6c20 3d20  _script_local = 
+00004bf0: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+00004c00: 2229 2e6a 6f69 6e70 6174 6828 0a20 2020  ").joinpath(.   
+00004c10: 2020 2020 2020 2020 2063 6f6e 7665 7274           convert
+00004c20: 5f70 7929 0a20 2020 2020 2020 2063 6f6e  _py).        con
+00004c30: 7665 7274 5f64 6566 203d 2066 227b 636f  vert_def = f"{co
+00004c40: 6e76 6572 745f 6e61 6d65 7d2e 6465 6622  nvert_name}.def"
+00004c50: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
+00004c60: 5f64 6566 5f6c 6f63 616c 203d 2066 696c  _def_local = fil
+00004c70: 6573 2822 7265 736f 7572 6365 7322 292e  es("resources").
+00004c80: 6a6f 696e 7061 7468 280a 2020 2020 2020  joinpath(.      
+00004c90: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
+00004ca0: 6629 0a20 2020 2020 2020 205f 203d 2073  f).        _ = s
+00004cb0: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
+00004cc0: 6e76 6572 745f 7363 7269 7074 5f6c 6f63  nvert_script_loc
+00004cd0: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
+00004ce0: 2020 2020 2020 2020 2072 656d 6f74 653d           remote=
+00004cf0: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
+00004d00: 7274 6572 735f 7061 7468 290a 2020 2020  rters_path).    
+00004d10: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
+00004d20: 286c 6f63 616c 3d63 6f6e 7665 7274 5f64  (local=convert_d
+00004d30: 6566 5f6c 6f63 616c 2c0a 2020 2020 2020  ef_local,.      
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004d50: 656d 6f74 653d 7365 6c66 2e73 6c75 726d  emote=self.slurm
+00004d60: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
+00004d70: 290a 2020 2020 2020 2020 2320 4275 696c  ).        # Buil
+00004d80: 6420 7369 6e67 756c 6172 6974 7920 636f  d singularity co
+00004d90: 6e74 6169 6e65 7220 6672 6f6d 2064 6566  ntainer from def
+00004da0: 696e 6974 696f 6e0a 2020 2020 2020 2020  inition.        
+00004db0: 7769 7468 2073 656c 662e 6364 2873 656c  with self.cd(sel
+00004dc0: 662e 736c 7572 6d5f 636f 6e76 6572 7465  f.slurm_converte
+00004dd0: 7273 5f70 6174 6829 3a0a 2020 2020 2020  rs_path):.      
+00004de0: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
+00004df0: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
+00004e00: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00004e10: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004e30: 2054 4f44 4f20 4368 616e 6765 2074 6865   TODO Change the
+00004e40: 2074 6d70 2064 6972 3f0a 2020 2020 2020   tmp dir?.      
+00004e50: 2020 2020 2020 2020 2020 2320 6578 706f            # expo
+00004e60: 7274 2053 494e 4755 4c41 5249 5459 5f54  rt SINGULARITY_T
+00004e70: 4d50 4449 523d 7e2f 6d79 2d73 6372 6174  MPDIR=~/my-scrat
+00004e80: 6368 2f74 6d70 3b0a 2020 2020 2020 2020  ch/tmp;.        
+00004e90: 2020 2020 2020 2020 2320 6f6e 6c79 2069          # only i
+00004ea0: 6620 6669 6c65 2064 6f65 7320 6e6f 7420  f file does not 
+00004eb0: 6578 6973 7420 7965 740a 2020 2020 2020  exist yet.      
+00004ec0: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
+00004ed0: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
+00004ee0: 6622 5b20 2120 2d66 207b 636f 6e76 6572  f"[ ! -f {conver
+00004ef0: 745f 6e61 6d65 7d2e 7369 6620 5d22 290a  t_name}.sif ]").
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f10: 2320 4544 4954 202d 2d20 4e4f 2c20 7468  # EDIT -- NO, th
+00004f20: 656e 2077 6520 6361 6e27 7420 7570 6461  en we can't upda
+00004f30: 7465 2120 466f 7263 6520 7265 6275 696c  te! Force rebuil
+00004f40: 6421 0a20 2020 2020 2020 2020 2020 2020  d!.             
+00004f50: 2020 2023 2064 6f77 6e6c 6f61 6420 2f62     # download /b
+00004f60: 7569 6c64 206e 6577 2063 6f6e 7461 696e  uild new contain
+00004f70: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+00004f80: 2020 2063 6f6e 7665 7274 5f63 6d64 732e     convert_cmds.
+00004f90: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+00004fa0: 2020 2020 2020 2020 2020 2020 6622 7369              f"si
+00004fb0: 6e67 756c 6172 6974 7920 6275 696c 6420  ngularity build 
+00004fc0: 2d46 207b 636f 6e76 6572 745f 6e61 6d65  -F {convert_name
+00004fd0: 7d2e 7369 6620 7b63 6f6e 7665 7274 5f64  }.sif {convert_d
+00004fe0: 6566 7d20 3e3e 2073 696e 672e 6c6f 6720  ef} >> sing.log 
+00004ff0: 323e 2631 203b 2065 6368 6f20 2766 696e  2>&1 ; echo 'fin
+00005000: 6973 6865 6420 7b63 6f6e 7665 7274 5f6e  ished {convert_n
+00005010: 616d 657d 2e73 6966 2720 2622 290a 2020  ame}.sif' &").  
+00005020: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
+00005030: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00005040: 636f 6e76 6572 745f 636d 6473 290a 0a20  convert_cmds).. 
+00005050: 2020 2064 6566 2073 6574 7570 5f6a 6f62     def setup_job
+00005060: 5f73 6372 6970 7473 2873 656c 6629 3a0a  _scripts(self):.
+00005070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005080: 2020 2020 5365 7473 2075 7020 6a6f 6220      Sets up job 
+00005090: 7363 7269 7074 7320 666f 7220 536c 7572  scripts for Slur
+000050a0: 6d20 6f70 6572 6174 696f 6e73 2e0a 0a20  m operations... 
+000050b0: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
+000050c0: 7469 6f6e 2065 6974 6865 7220 636c 6f6e  tion either clon
+000050d0: 6573 2061 2047 6974 2072 6570 6f73 6974  es a Git reposit
+000050e0: 6f72 7920 636f 6e74 6169 6e69 6e67 206a  ory containing j
+000050f0: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
+00005100: 2020 2069 6e74 6f20 7468 6520 7370 6563     into the spec
+00005110: 6966 6965 6420 7363 7269 7074 2070 6174  ified script pat
+00005120: 6820 6f72 2067 656e 6572 6174 6573 2073  h or generates s
+00005130: 6372 6970 7473 206c 6f63 616c 6c79 2069  cripts locally i
+00005140: 6620 6e6f 2072 6570 6f73 6974 6f72 790a  f no repository.
+00005150: 2020 2020 2020 2020 6973 2070 726f 7669          is provi
+00005160: 6465 642e 0a0a 2020 2020 2020 2020 5261  ded...        Ra
+00005170: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00005180: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
+00005190: 4966 2074 6865 7265 2069 7320 616e 2069  If there is an i
+000051a0: 7373 7565 2065 7865 6375 7469 6e67 2047  ssue executing G
+000051b0: 6974 2063 6f6d 6d61 6e64 7320 6f72 2067  it commands or g
+000051c0: 656e 6572 6174 696e 6720 7363 7269 7074  enerating script
+000051d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+000051e0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000051f0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+00005200: 2061 6e64 2073 656c 662e 736c 7572 6d5f   and self.slurm_
+00005210: 7363 7269 7074 5f70 6174 683a 0a20 2020  script_path:.   
+00005220: 2020 2020 2020 2020 2023 2067 6974 2063           # git c
+00005230: 6c6f 6e65 2069 6e74 6f20 7363 7269 7074  lone into script
+00005240: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
+00005250: 2020 656e 7620 3d20 7b0a 2020 2020 2020    env = {.      
+00005260: 2020 2020 2020 2020 2020 2252 4550 4f53            "REPOS
+00005270: 5243 223a 2073 656c 662e 736c 7572 6d5f  RC": self.slurm_
+00005280: 7363 7269 7074 5f72 6570 6f2c 0a20 2020  script_repo,.   
+00005290: 2020 2020 2020 2020 2020 2020 2022 4c4f               "LO
+000052a0: 4341 4c52 4550 4f22 3a20 7365 6c66 2e73  CALREPO": self.s
+000052b0: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
+000052c0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+000052d0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+000052e0: 2027 6769 7420 636c 6f6e 6520 2224 5245   'git clone "$RE
+000052f0: 504f 5352 4322 2022 244c 4f43 414c 5245  POSRC" "$LOCALRE
+00005300: 504f 2220 323e 202f 6465 762f 6e75 6c6c  PO" 2> /dev/null
+00005310: 207c 7c20 6769 7420 2d43 2022 244c 4f43   || git -C "$LOC
+00005320: 414c 5245 504f 2220 7075 6c6c 270a 2020  ALREPO" pull'.  
+00005330: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
+00005340: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00005350: 5b63 6d64 5d2c 2065 6e76 290a 2020 2020  [cmd], env).    
+00005360: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00005370: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
+00005380: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00005390: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
+000053a0: 2020 2065 6c69 6620 7365 6c66 2e73 6c75     elif self.slu
+000053b0: 726d 5f73 6372 6970 745f 7061 7468 3a0a  rm_script_path:.
+000053c0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+000053d0: 6e65 7261 7465 2073 6372 6970 7473 0a20  nerate scripts. 
+000053e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000053f0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
+00005400: 6970 7473 2867 656e 6572 6174 655f 6a6f  ipts(generate_jo
+00005410: 6273 3d54 7275 6529 0a0a 2020 2020 6465  bs=True)..    de
+00005420: 6620 7365 7475 705f 6469 7265 6374 6f72  f setup_director
+00005430: 6965 7328 7365 6c66 293a 0a20 2020 2020  ies(self):.     
+00005440: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00005450: 7265 6174 6573 206e 6563 6573 7361 7279  reates necessary
+00005460: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
+00005470: 2053 6c75 726d 206f 7065 7261 7469 6f6e   Slurm operation
+00005480: 732e 0a0a 2020 2020 2020 2020 5468 6973  s...        This
+00005490: 2066 756e 6374 696f 6e20 6372 6561 7465   function create
+000054a0: 7320 6469 7265 6374 6f72 6965 7320 666f  s directories fo
+000054b0: 7220 6461 7461 2073 746f 7261 6765 2c20  r data storage, 
+000054c0: 7363 7269 7074 732c 2061 6e64 2077 6f72  scripts, and wor
+000054d0: 6b66 6c6f 7773 0a20 2020 2020 2020 2061  kflows.        a
+000054e0: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
+000054f0: 6865 2053 6c75 726d 436c 6965 6e74 206f  he SlurmClient o
+00005500: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
+00005510: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00005520: 2020 2020 5353 4845 7863 6570 7469 6f6e      SSHException
+00005530: 3a20 4966 2074 6865 7265 2069 7320 616e  : If there is an
+00005540: 2069 7373 7565 2065 7865 6375 7469 6e67   issue executing
+00005550: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
+00005560: 696f 6e20 636f 6d6d 616e 6473 2e0a 2020  ion commands..  
+00005570: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005580: 2020 6469 725f 636d 6473 203d 205b 5d0a    dir_cmds = [].
+00005590: 2020 2020 2020 2020 2320 612e 2064 6174          # a. dat
+000055a0: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
+000055b0: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
+000055c0: 683a 0a20 2020 2020 2020 2020 2020 2064  h:.            d
+000055d0: 6972 5f63 6d64 732e 6170 7065 6e64 2866  ir_cmds.append(f
+000055e0: 226d 6b64 6972 202d 7020 7b73 656c 662e  "mkdir -p {self.
+000055f0: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
+00005600: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
+00005610: 2062 2e20 7363 7269 7074 730a 2020 2020   b. scripts.    
+00005620: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00005630: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
+00005640: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
+00005650: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+00005660: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+00005670: 6d5f 7363 7269 7074 5f70 6174 687d 2229  m_script_path}")
+00005680: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00005690: 2e20 776f 726b 666c 6f77 730a 2020 2020  . workflows.    
+000056a0: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+000056b0: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
+000056c0: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
+000056d0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+000056e0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+000056f0: 6d5f 696d 6167 6573 5f70 6174 687d 2229  m_images_path}")
+00005700: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
+00005710: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
+00005720: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
+00005730: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
+00005740: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00005750: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+00005760: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00005770: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
+00005780: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
+00005790: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
+000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057b0: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
+000057c0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+000057d0: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
+000057e0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+000057f0: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
+00005800: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
+00005810: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
+00005820: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
+00005830: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+00005840: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
+00005850: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+00005860: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
+00005870: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
+00005880: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
+00005890: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
+000058a0: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
+000058b0: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
+000058c0: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
+000058d0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
+000058e0: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
+000058f0: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
+00005900: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
+00005910: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
+00005920: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
+00005930: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
+00005940: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
+00005950: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
+00005960: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
+00005970: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
+00005980: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
+00005990: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
+000059a0: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
+000059b0: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
+000059c0: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
+000059d0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+000059e0: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
+000059f0: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
+00005a00: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
+00005a10: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
+00005a20: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
+00005a30: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
+00005a40: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00005a50: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
+00005a60: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
+00005a70: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
+00005a80: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
+00005a90: 2020 2020 2020 2020 2020 2020 696e 6974              init
+00005aa0: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
+00005ab0: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
+00005ac0: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
+00005ad0: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
+00005ae0: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
+00005af0: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
+00005b00: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
+00005b10: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
+00005b20: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
+00005b30: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00005b40: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
+00005b50: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
+00005b60: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00005b70: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
+00005b80: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
+00005b90: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
+00005ba0: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
+00005bb0: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
+00005bc0: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
+00005bd0: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
+00005be0: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
+00005bf0: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
+00005c00: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
+00005c10: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
+00005c20: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
+00005c30: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
+00005c40: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
+00005c50: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
+00005c80: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
+00005cb0: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
+00005cc0: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
+00005cd0: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
+00005ce0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00005cf0: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
+00005d00: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
+00005d10: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
+00005d20: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
+00005d30: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
+00005d40: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
+00005d50: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
+00005d60: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
+00005d70: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
+00005d80: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
+00005d90: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
+00005da0: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
+00005db0: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
+00005dc0: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
+00005dd0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
+00005de0: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
+00005df0: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
+00005e00: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
+00005e10: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
+00005e20: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
+00005e30: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
+00005e40: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+00005e50: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+00005e60: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
+00005e70: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
+00005e80: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
+00005e90: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
+00005ea0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+00005eb0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+00005ec0: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
+00005ed0: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
+00005ee0: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
+00005ef0: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
+00005f00: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
+00005f10: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
+00005f20: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
+00005f30: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+00005f40: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+00005f50: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
+00005f60: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
+00005f70: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
+00005f80: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
+00005f90: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
+00005fa0: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
+00005fb0: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
+00005fc0: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
+00005fd0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00005fe0: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
+00005ff0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006000: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
+00006010: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006020: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
+00006030: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00006040: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
+00006050: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
+00006060: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
+00006070: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00006080: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
+00006090: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
+000060a0: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
+000060b0: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
+000060c0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+000060d0: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
+000060e0: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
+000060f0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00006100: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
+00006110: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
+00006120: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
+00006130: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
+00006140: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
+00006150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006160: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
+00006170: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
+00006180: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
+00006190: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+000061a0: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
+000061b0: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
+000061c0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+000061d0: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
+000061e0: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
+000061f0: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
+00006200: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00006210: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
+00006220: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
+00006230: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00006240: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
+00006250: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
+00006260: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
+00006270: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
+00006280: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
+00006290: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000062a0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+000062b0: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
+000062c0: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
+000062d0: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
+00006300: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
+00006310: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
+00006320: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
+00006330: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
+00006340: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
+00006350: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006360: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006370: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00006380: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
+00006390: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+000063a0: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
+000063b0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
+000063c0: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
+000063d0: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
+000063e0: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
+000063f0: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
+00006400: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
+00006410: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
+00006420: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
+00006430: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
+00006440: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+00006450: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
+00006460: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
+00006470: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
+00006480: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
+00006490: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+000064a0: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
+000064b0: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+000064c0: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
+000064d0: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
+000064e0: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
+000064f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00006500: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
+00006530: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
+00006560: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
+00006570: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00006580: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
+00006590: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
+000065a0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
+000065b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000065c0: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
+000065d0: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
+000065e0: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006600: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+00006610: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
+00006620: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
+00006630: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006640: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
+00006650: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
+00006660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006670: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
+00006680: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+00006690: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+000066a0: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
+000066b0: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066d0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+000066e0: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
+000066f0: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
+00006700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006710: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00006720: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
+00006730: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
+00006740: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00006750: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
+00006760: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+00006770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006780: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
+00006790: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
+000067a0: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
+000067b0: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
+000067e0: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006800: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
+00006810: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00006820: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00006830: 615f 6c6f 6361 7469 6f6e 3a20 7374 7220  a_location: str 
+00006840: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
+00006870: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2029 202d 3e20 5265 7375 6c74 3a0a 2020   ) -> Result:.  
+000068a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000068b0: 2020 436c 6561 6e75 7020 7a69 7020 616e    Cleanup zip an
+000068c0: 6420 756e 7a69 7070 6564 2066 696c 6573  d unzipped files
+000068d0: 2f66 6f6c 6465 7273 2061 7373 6f63 6961  /folders associa
+000068e0: 7465 6420 7769 7468 2061 2053 6c75 726d  ted with a Slurm
+000068f0: 206a 6f62 2e0a 0a20 2020 2020 2020 2041   job...        A
+00006900: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00006910: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
+00006920: 7472 293a 2054 6865 206a 6f62 2049 4420  tr): The job ID 
+00006930: 6f66 2074 6865 2053 6c75 726d 2073 6372  of the Slurm scr
+00006940: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
+00006950: 2066 696c 656e 616d 6520 2873 7472 293a   filename (str):
+00006960: 2054 6865 207a 6970 2066 696c 656e 616d   The zip filenam
+00006970: 6520 6f6e 2053 6c75 726d 2e0a 2020 2020  e on Slurm..    
+00006980: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
+00006990: 6174 696f 6e20 2873 7472 2c20 6f70 7469  ation (str, opti
+000069a0: 6f6e 616c 293a 2054 6865 206c 6f63 6174  onal): The locat
+000069b0: 696f 6e20 6f66 2064 6174 6120 6669 6c65  ion of data file
+000069c0: 7320 6f6e 2053 6c75 726d 2e0a 2020 2020  s on Slurm..    
+000069d0: 2020 2020 2020 2020 2020 2020 4966 206e              If n
+000069e0: 6f74 2070 726f 7669 6465 642c 2069 7420  ot provided, it 
+000069f0: 7769 6c6c 2062 6520 6578 7472 6163 7465  will be extracte
+00006a00: 6420 6672 6f6d 2074 6865 206c 6f67 2066  d from the log f
+00006a10: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
+00006a20: 206c 6f67 6669 6c65 2028 7374 722c 206f   logfile (str, o
+00006a30: 7074 696f 6e61 6c29 3a20 5468 6520 6c6f  ptional): The lo
+00006a40: 6720 6669 6c65 206f 6620 7468 6520 536c  g file of the Sl
+00006a50: 7572 6d20 6a6f 622e 200a 2020 2020 2020  urm job. .      
+00006a60: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
+00006a70: 2070 726f 7669 6465 642c 2061 2064 6566   provided, a def
+00006a80: 6175 6c74 206c 6f67 2066 696c 6520 7769  ault log file wi
+00006a90: 6c6c 2062 6520 7573 6564 2e0a 0a20 2020  ll be used...   
+00006aa0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00006ab0: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
+00006ac0: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
+00006ad0: 7468 6520 636c 6561 6e75 7020 6f70 6572  the cleanup oper
+00006ae0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00006af0: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
+00006b00: 2020 5468 6520 636c 6561 6e75 7020 7072    The cleanup pr
+00006b10: 6f63 6573 7320 696e 766f 6c76 6573 2072  ocess involves r
+00006b20: 656d 6f76 696e 6720 7468 6520 7370 6563  emoving the spec
+00006b30: 6966 6965 6420 7a69 7020 6669 6c65 2c20  ified zip file, 
+00006b40: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00006b50: 206c 6f67 2066 696c 652c 2061 6e64 2061   log file, and a
+00006b60: 7373 6f63 6961 7465 6420 6461 7461 2066  ssociated data f
+00006b70: 696c 6573 2061 6e64 2066 6f6c 6465 7273  iles and folders
+00006b80: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00006b90: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00006ba0: 2320 436c 6561 6e75 7020 7465 6d70 6f72  # Cleanup tempor
+00006bb0: 6172 7920 6669 6c65 7320 666f 7220 6120  ary files for a 
+00006bc0: 536c 7572 6d20 6a6f 620a 2020 2020 2020  Slurm job.      
+00006bd0: 2020 2020 2020 636c 6965 6e74 2e63 6c65        client.cle
+00006be0: 616e 7570 5f74 6d70 5f66 696c 6573 2822  anup_tmp_files("
+00006bf0: 3132 3334 3522 2c20 226f 7574 7075 742e  12345", "output.
+00006c00: 7a69 7022 290a 2020 2020 2020 2020 2222  zip").        ""
+00006c10: 220a 2020 2020 2020 2020 636d 6473 203d  ".        cmds =
+00006c20: 205b 5d0a 2020 2020 2020 2020 2320 7a69   [].        # zi
+00006c30: 700a 2020 2020 2020 2020 726d 7a69 7020  p.        rmzip 
+00006c40: 3d20 6622 726d 207b 6669 6c65 6e61 6d65  = f"rm {filename
+00006c50: 7d2e 2a22 0a20 2020 2020 2020 2063 6d64  }.*".        cmd
+00006c60: 732e 6170 7065 6e64 2872 6d7a 6970 290a  s.append(rmzip).
+00006c70: 2020 2020 2020 2020 2320 6c6f 670a 2020          # log.  
+00006c80: 2020 2020 2020 6966 206c 6f67 6669 6c65        if logfile
+00006c90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006ca0: 2020 2020 2020 6c6f 6766 696c 6520 3d20        logfile = 
+00006cb0: 7365 6c66 2e5f 4c4f 4746 494c 450a 2020  self._LOGFILE.  
+00006cc0: 2020 2020 2020 2020 2020 6c6f 6766 696c            logfil
+00006cd0: 6520 3d20 6c6f 6766 696c 652e 666f 726d  e = logfile.form
+00006ce0: 6174 2873 6c75 726d 5f6a 6f62 5f69 643d  at(slurm_job_id=
+00006cf0: 736c 7572 6d5f 6a6f 625f 6964 290a 2020  slurm_job_id).  
+00006d00: 2020 2020 2020 726d 6c6f 6720 3d20 6622        rmlog = f"
+00006d10: 726d 207b 6c6f 6766 696c 657d 220a 2020  rm {logfile}".  
+00006d20: 2020 2020 2020 636d 6473 2e61 7070 656e        cmds.appen
+00006d30: 6428 726d 6c6f 6729 0a20 2020 2020 2020  d(rmlog).       
+00006d40: 2023 2064 6174 610a 2020 2020 2020 2020   # data.        
+00006d50: 6966 2064 6174 615f 6c6f 6361 7469 6f6e  if data_location
+00006d60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006d70: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
+00006d80: 696f 6e20 3d20 7365 6c66 2e65 7874 7261  ion = self.extra
+00006d90: 6374 5f64 6174 615f 6c6f 6361 7469 6f6e  ct_data_location
+00006da0: 5f66 726f 6d5f 6c6f 6728 6c6f 6766 696c  _from_log(logfil
+00006db0: 6529 0a20 2020 2020 2020 2072 6d64 6174  e).        rmdat
+00006dc0: 6120 3d20 6622 726d 202d 7266 207b 6461  a = f"rm -rf {da
+00006dd0: 7461 5f6c 6f63 6174 696f 6e7d 207b 6461  ta_location} {da
+00006de0: 7461 5f6c 6f63 6174 696f 6e7d 2e2a 220a  ta_location}.*".
+00006df0: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
+00006e00: 656e 6428 726d 6461 7461 290a 0a20 2020  end(rmdata)..   
+00006e10: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00006e20: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00006e30: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+00006e40: 2863 6d64 7329 0a20 2020 2020 2020 2065  (cmds).        e
+00006e50: 7863 6570 7420 556e 6578 7065 6374 6564  xcept Unexpected
+00006e60: 4578 6974 2061 7320 653a 0a20 2020 2020  Exit as e:.     
+00006e70: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+00006e80: 726e 696e 6728 6529 0a20 2020 2020 2020  rning(e).       
+00006e90: 2020 2020 2072 6573 756c 7420 3d20 652e       result = e.
+00006ea0: 7265 7375 6c74 0a20 2020 2020 2020 2072  result.        r
+00006eb0: 6574 7572 6e20 7265 7375 6c74 206f 7220  eturn result or 
+00006ec0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7661  None..    def va
+00006ed0: 6c69 6461 7465 2873 656c 662c 2076 616c  lidate(self, val
+00006ee0: 6964 6174 655f 736c 7572 6d5f 7365 7475  idate_slurm_setu
+00006ef0: 703a 2062 6f6f 6c20 3d20 4661 6c73 6529  p: bool = False)
+00006f00: 3a0a 2020 2020 2020 2020 2222 2256 616c  :.        """Val
+00006f10: 6964 6174 6520 7468 6520 636f 6e6e 6563  idate the connec
+00006f20: 7469 6f6e 2074 6f20 7468 6520 536c 7572  tion to the Slur
+00006f30: 6d20 636c 7573 7465 7220 6279 2072 756e  m cluster by run
+00006f40: 6e69 6e67 0a20 2020 2020 2020 2061 2073  ning.        a s
+00006f50: 696d 706c 6520 636f 6d6d 616e 642e 0a0a  imple command...
+00006f60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00006f70: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+00006f80: 7465 5f73 6c75 726d 5f73 6574 7570 2028  te_slurm_setup (
+00006f90: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+00006fa0: 6f20 616c 736f 2063 6865 636b 0a20 2020  o also check.   
+00006fb0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00006fc0: 2066 6978 2074 6865 2053 6c75 726d 2073   fix the Slurm s
+00006fd0: 6574 7570 2028 666f 6c64 6572 732c 2069  etup (folders, i
+00006fe0: 6d61 6765 732c 2065 7463 2e29 0a0a 2020  mages, etc.)..  
+00006ff0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00007000: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
+00007010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007020: 2054 7275 6520 6966 2074 6865 2076 616c   True if the val
+00007030: 6964 6174 696f 6e20 6973 2073 7563 6365  idation is succe
+00007040: 7373 6675 6c2c 0a20 2020 2020 2020 2020  ssful,.         
+00007050: 2020 2020 2020 2046 616c 7365 206f 7468         False oth
+00007060: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
+00007070: 2222 220a 2020 2020 2020 2020 636f 6e6e  """.        conn
+00007080: 6563 7465 6420 3d20 7365 6c66 2e72 756e  ected = self.run
+00007090: 2827 6563 686f 2022 2022 2729 2e6f 6b0a  ('echo " "').ok.
+000070a0: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
+000070b0: 6374 6564 2061 6e64 2076 616c 6964 6174  cted and validat
+000070c0: 655f 736c 7572 6d5f 7365 7475 703a 0a20  e_slurm_setup:. 
+000070d0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 7365 6c66 2e73 6574 7570 5f73 6c75 726d  self.setup_slurm
+00007100: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
+00007110: 7863 6570 7420 5353 4845 7863 6570 7469  xcept SSHExcepti
+00007120: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00007130: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00007140: 6572 726f 7228 6529 0a20 2020 2020 2020  error(e).       
+00007150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007160: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
+00007170: 7475 726e 2063 6f6e 6e65 6374 6564 0a0a  turn connected..
+00007180: 2020 2020 6465 6620 6765 745f 7265 6365      def get_rece
+00007190: 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64 2873  nt_log_command(s
+000071a0: 656c 662c 206c 6f67 5f66 696c 653a 2073  elf, log_file: s
+000071b0: 7472 2c20 6e3a 2069 6e74 203d 2031 3029  tr, n: int = 10)
+000071c0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+000071d0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
+000071e0: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
+000071f0: 7265 7472 6965 7665 2074 6865 2072 6563  retrieve the rec
+00007200: 656e 7420 6c6f 6720 656e 7472 6965 7320  ent log entries 
+00007210: 6672 6f6d 2061 0a20 2020 2020 2020 2073  from a.        s
+00007220: 7065 6369 6669 6564 206c 6f67 2066 696c  pecified log fil
+00007230: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+00007240: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00007250: 675f 6669 6c65 2028 7374 7229 3a20 5468  g_file (str): Th
+00007260: 6520 7061 7468 2074 6f20 7468 6520 6c6f  e path to the lo
+00007270: 6720 6669 6c65 2e0a 2020 2020 2020 2020  g file..        
+00007280: 2020 2020 6e20 2869 6e74 2c20 6f70 7469      n (int, opti
+00007290: 6f6e 616c 293a 2054 6865 206e 756d 6265  onal): The numbe
+000072a0: 7220 6f66 2072 6563 656e 7420 6c6f 6720  r of recent log 
+000072b0: 656e 7472 6965 7320 746f 2072 6574 7269  entries to retri
+000072c0: 6576 652e 0a20 2020 2020 2020 2020 2020  eve..           
+000072d0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+000072e0: 2031 302e 0a0a 2020 2020 2020 2020 5265   10...        Re
+000072f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00007300: 2020 2073 7472 3a20 5468 6520 636f 6d6d     str: The comm
+00007310: 616e 6420 746f 2072 6574 7269 6576 6520  and to retrieve 
+00007320: 7468 6520 7265 6365 6e74 206c 6f67 2065  the recent log e
+00007330: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
+00007340: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00007350: 726e 2073 656c 662e 5f54 4149 4c5f 4c4f  rn self._TAIL_LO
+00007360: 475f 434d 442e 666f 726d 6174 286e 3d6e  G_CMD.format(n=n
+00007370: 2c20 6c6f 675f 6669 6c65 3d6c 6f67 5f66  , log_file=log_f
+00007380: 696c 6529 0a0a 2020 2020 6465 6620 6765  ile)..    def ge
+00007390: 745f 6163 7469 7665 5f6a 6f62 5f70 726f  t_active_job_pro
+000073a0: 6772 6573 7328 7365 6c66 2c0a 2020 2020  gress(self,.    
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+000073d0: 6d5f 6a6f 625f 6964 3a20 7374 722c 0a20  m_job_id: str,. 
+000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007400: 6174 7465 726e 3a20 7374 7220 3d20 7222  attern: str = r"
+00007410: 5c64 2b25 222c 0a20 2020 2020 2020 2020  \d+%",.         
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+00007440: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+00007450: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+00007460: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
+00007470: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+00007480: 2070 726f 6772 6573 7320 6f66 2061 6e20   progress of an 
+00007490: 6163 7469 7665 2053 6c75 726d 206a 6f62  active Slurm job
+000074a0: 2066 726f 6d20 6974 7320 6c6f 6766 696c   from its logfil
+000074b0: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
+000074c0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+000074d0: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
+000074e0: 293a 2054 6865 2049 4420 6f66 2074 6865  ): The ID of the
+000074f0: 2053 6c75 726d 206a 6f62 2e0a 2020 2020   Slurm job..    
+00007500: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
+00007510: 2873 7472 293a 2054 6865 2070 6174 7465  (str): The patte
+00007520: 726e 2074 6f20 6d61 7463 6820 696e 2074  rn to match in t
+00007530: 6865 206a 6f62 206c 6f67 2074 6f20 6578  he job log to ex
+00007540: 7472 6163 740a 2020 2020 2020 2020 2020  tract.          
+00007550: 2020 2020 2020 7468 6520 7072 6f67 7265        the progre
+00007560: 7373 2028 6465 6661 756c 743a 2072 225c  ss (default: r"\
+00007570: 642b 2522 292e 0a0a 2020 2020 2020 2020  d+%")...        
+00007580: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
+00007590: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
+000075a0: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
+000075b0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+000075c0: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
+000075d0: 2020 2020 746f 2073 6574 2077 6865 6e20      to set when 
+000075e0: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+000075f0: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
+00007600: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+00007610: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00007620: 2020 2020 2073 7472 3a20 5468 6520 7072       str: The pr
+00007630: 6f67 7265 7373 206f 6620 7468 6520 536c  ogress of the Sl
+00007640: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
+00007650: 2022 2222 0a20 2020 2020 2020 2063 6d64   """.        cmd
+00007660: 6c69 7374 203d 205b 5d0a 2020 2020 2020  list = [].      
+00007670: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
+00007680: 5f72 6563 656e 745f 6c6f 675f 636f 6d6d  _recent_log_comm
+00007690: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
+000076a0: 206c 6f67 5f66 696c 653d 7365 6c66 2e5f   log_file=self._
+000076b0: 4c4f 4746 494c 452e 666f 726d 6174 2873  LOGFILE.format(s
+000076c0: 6c75 726d 5f6a 6f62 5f69 643d 736c 7572  lurm_job_id=slur
+000076d0: 6d5f 6a6f 625f 6964 2929 0a20 2020 2020  m_job_id)).     
+000076e0: 2020 2063 6d64 6c69 7374 2e61 7070 656e     cmdlist.appen
+000076f0: 6428 636d 6429 0a20 2020 2020 2020 2069  d(cmd).        i
+00007700: 6620 656e 7620 6973 204e 6f6e 653a 0a20  f env is None:. 
+00007710: 2020 2020 2020 2020 2020 2065 6e76 203d             env =
+00007720: 207b 7d0a 2020 2020 2020 2020 7472 793a   {}.        try:
+00007730: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00007740: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+00007750: 6f6d 6d61 6e64 7328 636d 646c 6973 742c  ommands(cmdlist,
+00007760: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
+00007770: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00007780: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00007790: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
+000077a0: 7228 6622 4973 7375 6520 7769 7468 2072  r(f"Issue with r
+000077b0: 756e 2063 6f6d 6d61 6e64 3a20 7b65 7d22  un command: {e}"
+000077c0: 290a 2020 2020 2020 2020 2320 4d61 7463  ).        # Matc
+000077d0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
+000077e0: 7061 7474 6572 6e20 696e 2074 6865 2072  pattern in the r
+000077f0: 6573 756c 7427 7320 7374 646f 7574 0a20  esult's stdout. 
+00007800: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00007810: 2020 2020 2020 2020 6c61 7465 7374 5f70          latest_p
+00007820: 726f 6772 6573 7320 3d20 7265 2e66 696e  rogress = re.fin
+00007830: 6461 6c6c 280a 2020 2020 2020 2020 2020  dall(.          
+00007840: 2020 2020 2020 7061 7474 6572 6e2c 2072        pattern, r
+00007850: 6573 756c 742e 7374 646f 7574 295b 2d31  esult.stdout)[-1
+00007860: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
+00007870: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00007880: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00007890: 6765 722e 6572 726f 7228 6622 4973 7375  ger.error(f"Issu
+000078a0: 6520 7769 7468 2065 7874 7261 6374 696e  e with extractin
+000078b0: 6720 7072 6f67 7265 7373 3a20 7b65 7d22  g progress: {e}"
+000078c0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000078d0: 6e20 6622 5072 6f67 7265 7373 3a20 7b6c  n f"Progress: {l
+000078e0: 6174 6573 745f 7072 6f67 7265 7373 7d5c  atest_progress}\
+000078f0: 6e22 0a0a 2020 2020 6465 6620 7275 6e5f  n"..    def run_
+00007900: 636f 6d6d 616e 6473 2873 656c 662c 2063  commands(self, c
+00007910: 6d64 6c69 7374 3a20 4c69 7374 5b73 7472  mdlist: List[str
+00007920: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007930: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
+00007940: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00007950: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 2073 6570 3a20 7374 7220 3d20 2720     sep: str = ' 
+00007980: 2626 2027 2c0a 2020 2020 2020 2020 2020  && ',.          
+00007990: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+000079a0: 7267 7329 202d 3e20 5265 7375 6c74 3a0a  rgs) -> Result:.
+000079b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000079c0: 2020 2020 5275 6e20 6120 6c69 7374 206f      Run a list o
+000079d0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
+000079e0: 2063 6f6e 7365 6375 7469 7665 6c79 206f   consecutively o
+000079f0: 6e20 7468 6520 536c 7572 6d20 636c 7573  n the Slurm clus
+00007a00: 7465 722c 0a20 2020 2020 2020 2065 6e73  ter,.        ens
+00007a10: 7572 696e 6720 7468 6520 7375 6363 6573  uring the succes
+00007a20: 7320 6f66 2065 6163 6820 6265 666f 7265  s of each before
+00007a30: 2070 726f 6365 6564 696e 6720 746f 2074   proceeding to t
+00007a40: 6865 206e 6578 742e 0a0a 2020 2020 2020  he next...      
+00007a50: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
+00007a60: 7420 7661 7269 6162 6c65 7320 6361 6e20  t variables can 
+00007a70: 6265 2073 6574 2075 7369 6e67 2074 6865  be set using the
+00007a80: 2060 656e 7660 2061 7267 756d 656e 742e   `env` argument.
+00007a90: 0a20 2020 2020 2020 2054 6865 7365 2063  .        These c
+00007aa0: 6f6d 6d61 6e64 7320 7265 7461 696e 2074  ommands retain t
+00007ab0: 6865 2073 616d 6520 7365 7373 696f 6e20  he same session 
+00007ac0: 2865 6e76 6972 6f6e 6d65 6e74 2076 6172  (environment var
+00007ad0: 6961 626c 6573 0a20 2020 2020 2020 2065  iables.        e
+00007ae0: 7463 2e29 2c20 756e 6c69 6b65 2072 756e  tc.), unlike run
+00007af0: 6e69 6e67 2074 6865 6d20 7365 7061 7261  ning them separa
+00007b00: 7465 6c79 2e0a 0a20 2020 2020 2020 2041  tely...        A
+00007b10: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00007b20: 2063 6d64 6c69 7374 2028 4c69 7374 5b73   cmdlist (List[s
+00007b30: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
+00007b40: 7368 656c 6c20 636f 6d6d 616e 6473 2074  shell commands t
+00007b50: 6f20 7275 6e20 6f6e 2053 6c75 726d 2e0a  o run on Slurm..
+00007b60: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+00007b70: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
+00007b80: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
+00007b90: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
+00007ba0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007bc0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+00007bd0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+00007be0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00007bf0: 2020 2020 2020 2020 2020 7365 7020 2873            sep (s
+00007c00: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
+00007c10: 6865 2073 6570 6172 6174 6f72 2075 7365  he separator use
+00007c20: 6420 746f 2063 6f6e 6361 7465 6e61 7465  d to concatenate
+00007c30: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+00007c40: 2020 2020 2020 636f 6d6d 616e 6473 2e20        commands. 
+00007c50: 4465 6661 756c 7473 2074 6f20 2720 2626  Defaults to ' &&
+00007c60: 2027 2e0a 2020 2020 2020 2020 2020 2020   '..            
+00007c70: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
+00007c80: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+00007c90: 756d 656e 7473 2e0a 0a20 2020 2020 2020  uments...       
+00007ca0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00007cb0: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
+00007cc0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+00007cd0: 6c61 7374 2063 6f6d 6d61 6e64 2069 6e20  last command in 
+00007ce0: 7468 6520 6c69 7374 2e0a 2020 2020 2020  the list..      
+00007cf0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00007d00: 2065 6e76 2069 7320 4e6f 6e65 3a0a 2020   env is None:.  
+00007d10: 2020 2020 2020 2020 2020 656e 7620 3d20            env = 
+00007d20: 7b7d 0a20 2020 2020 2020 2063 6d64 203d  {}.        cmd =
+00007d30: 2073 6570 2e6a 6f69 6e28 636d 646c 6973   sep.join(cmdlis
+00007d40: 7429 0a20 2020 2020 2020 206c 6f67 6765  t).        logge
+00007d50: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+00007d60: 2020 2020 6622 5275 6e6e 696e 6720 636f      f"Running co
+00007d70: 6d6d 616e 6473 2c20 7769 7468 2065 6e76  mmands, with env
+00007d80: 207b 656e 767d 2061 6e64 2073 6570 207b   {env} and sep {
+00007d90: 7365 707d 205c 0a20 2020 2020 2020 2020  sep} \.         
+00007da0: 2020 2020 2020 2061 6e64 207b 6b77 6172         and {kwar
+00007db0: 6773 7d3a 207b 636d 647d 2229 0a20 2020  gs}: {cmd}").   
+00007dc0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00007dd0: 6c66 2e72 756e 2863 6d64 2c20 656e 763d  lf.run(cmd, env=
+00007de0: 656e 762c 202a 2a6b 7761 7267 7329 2020  env, **kwargs)  
+00007df0: 2320 6f75 745f 7374 7265 616d 3d6f 7574  # out_stream=out
+00007e00: 5f73 7472 6561 6d2c 0a0a 2020 2020 2020  _stream,..      
+00007e10: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00007e20: 2020 2023 2057 6174 6368 206f 7574 2066     # Watch out f
+00007e30: 6f72 2055 6e69 636f 6465 456e 636f 6465  or UnicodeEncode
+00007e40: 4572 726f 7220 7768 656e 2079 6f75 2073  Error when you s
+00007e50: 7472 2829 2074 6869 732e 0a20 2020 2020  tr() this..     
+00007e60: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00007e70: 666f 2866 227b 7265 7375 6c74 2e73 7464  fo(f"{result.std
+00007e80: 6f75 747d 2229 0a20 2020 2020 2020 2065  out}").        e
+00007e90: 7863 6570 7420 556e 6963 6f64 6545 6e63  xcept UnicodeEnc
+00007ea0: 6f64 6545 7272 6f72 2061 7320 653a 0a20  odeError as e:. 
+00007eb0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00007ec0: 722e 6572 726f 7228 6622 556e 6963 6f64  r.error(f"Unicod
+00007ed0: 6520 6572 726f 723a 207b 657d 2229 0a20  e error: {e}"). 
+00007ee0: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00007ef0: 4f3a 204f 4e4c 5920 7374 646f 7574 2052  O: ONLY stdout R
+00007f00: 4543 4f44 4520 4e45 4544 4544 3f3f 206f  ECODE NEEDED?? o
+00007f10: 7220 616c 736f 2065 7272 6f72 3f0a 2020  r also error?.  
+00007f20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00007f30: 2e73 7464 6f75 7420 3d20 7265 7375 6c74  .stdout = result
+00007f40: 2e73 7464 6f75 742e 656e 636f 6465 280a  .stdout.encode(.
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2775 7466 2d38 272c 2027 6967 6e6f 7265  'utf-8', 'ignore
+00007f70: 2729 2e64 6563 6f64 6528 2775 7466 2d38  ').decode('utf-8
+00007f80: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00007f90: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00007fa0: 6620 7374 725f 746f 5f63 6c61 7373 2873  f str_to_class(s
+00007fb0: 656c 662c 206d 6f64 756c 655f 6e61 6d65  elf, module_name
+00007fc0: 3a20 7374 722c 2063 6c61 7373 5f6e 616d  : str, class_nam
+00007fd0: 653a 2073 7472 2c20 2a61 7267 732c 202a  e: str, *args, *
+00007fe0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00007ff0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00008000: 7475 726e 2061 2063 6c61 7373 2069 6e73  turn a class ins
+00008010: 7461 6e63 6520 6672 6f6d 2061 2073 7472  tance from a str
+00008020: 696e 6720 7265 6665 7265 6e63 652e 0a0a  ing reference...
+00008030: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00008040: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
+00008050: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
+00008060: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
+00008070: 756c 652e 0a20 2020 2020 2020 2020 2020  ule..           
+00008080: 2063 6c61 7373 5f6e 616d 6520 2873 7472   class_name (str
+00008090: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+000080a0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
+000080b0: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
+000080c0: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
+000080d0: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
+000080e0: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
+000080f0: 7275 6374 6f72 2e0a 2020 2020 2020 2020  ructor..        
+00008100: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
+00008110: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+00008120: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
+00008130: 6865 2063 6c61 7373 2063 6f6e 7374 7275  he class constru
+00008140: 6374 6f72 2e0a 0a20 2020 2020 2020 2052  ctor...        R
+00008150: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00008160: 2020 2020 6f62 6a65 6374 3a20 416e 2069      object: An i
+00008170: 6e73 7461 6e63 6520 6f66 2074 6865 2073  nstance of the s
+00008180: 7065 6369 6669 6564 2063 6c61 7373 2c20  pecified class, 
+00008190: 6f72 204e 6f6e 6520 6966 2074 6865 2063  or None if the c
+000081a0: 6c61 7373 206f 720a 2020 2020 2020 2020  lass or.        
+000081b0: 2020 2020 2020 2020 6d6f 6475 6c65 2064          module d
+000081c0: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
+000081d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000081e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000081f0: 2020 2020 6d6f 6475 6c65 5f20 3d20 696d      module_ = im
+00008200: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
+00008210: 6f64 756c 6528 6d6f 6475 6c65 5f6e 616d  odule(module_nam
+00008220: 6529 0a20 2020 2020 2020 2020 2020 2074  e).            t
+00008230: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00008240: 2020 2020 636c 6173 735f 203d 2067 6574      class_ = get
+00008250: 6174 7472 286d 6f64 756c 655f 2c20 636c  attr(module_, cl
+00008260: 6173 735f 6e61 6d65 2928 2a61 7267 732c  ass_name)(*args,
+00008270: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00008280: 2020 2020 2020 2065 7863 6570 7420 4174         except At
+00008290: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
+000082a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000082b0: 6767 6572 2e65 7272 6f72 2827 436c 6173  gger.error('Clas
+000082c0: 7320 646f 6573 206e 6f74 2065 7869 7374  s does not exist
+000082d0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
+000082e0: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+000082f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00008300: 722e 6572 726f 7228 274d 6f64 756c 6520  r.error('Module 
+00008310: 646f 6573 206e 6f74 2065 7869 7374 2729  does not exist')
+00008320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008330: 636c 6173 735f 206f 7220 4e6f 6e65 0a0a  class_ or None..
+00008340: 2020 2020 6465 6620 7275 6e5f 636f 6d6d      def run_comm
+00008350: 616e 6473 5f73 706c 6974 5f6f 7574 2873  ands_split_out(s
+00008360: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 2020 2020 636d 646c 6973 743a 204c 6973      cmdlist: Lis
+00008390: 745b 7374 725d 2c0a 2020 2020 2020 2020  t[str],.        
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+000083c0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+000083d0: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+00008400: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
+00008410: 2020 2022 2222 5275 6e20 6120 6c69 7374     """Run a list
+00008420: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
+00008430: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
+00008440: 2061 6e64 2073 706c 6974 2074 6865 206f   and split the o
+00008450: 7574 7075 740a 2020 2020 2020 2020 6f66  utput.        of
+00008460: 2065 6163 6820 636f 6d6d 616e 642e 0a0a   each command...
+00008470: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
+00008480: 6d61 6e64 2069 6e20 7468 6520 6c69 7374  mand in the list
+00008490: 2069 7320 6578 6563 7574 6564 2077 6974   is executed wit
+000084a0: 6820 6120 7365 7061 7261 746f 7220 696e  h a separator in
+000084b0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
+000084c0: 2074 6861 7420 6973 2075 6e69 7175 6520   that is unique 
+000084d0: 616e 6420 6361 6e20 6265 2075 7365 6420  and can be used 
+000084e0: 746f 2073 706c 6974 0a20 2020 2020 2020  to split.       
+000084f0: 2074 6865 206f 7574 7075 7420 6f66 2065   the output of e
+00008500: 6163 6820 636f 6d6d 616e 6420 6c61 7465  ach command late
+00008510: 722e 2054 6865 2073 6570 6172 6174 6f72  r. The separator
+00008520: 2075 7365 6420 6973 2073 7065 6369 6669   used is specifi
+00008530: 6564 0a20 2020 2020 2020 2062 7920 7468  ed.        by th
+00008540: 6520 605f 4f55 545f 5345 5060 2061 7474  e `_OUT_SEP` att
+00008550: 7269 6275 7465 206f 6620 7468 650a 2020  ribute of the.  
+00008560: 2020 2020 2020 536c 7572 6d43 6c69 656e        SlurmClien
+00008570: 7420 696e 7374 616e 6365 2e0a 0a20 2020  t instance...   
+00008580: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00008590: 2020 2020 2020 2063 6d64 6c69 7374 2028         cmdlist (
+000085a0: 4c69 7374 5b73 7472 5d29 3a20 4120 6c69  List[str]): A li
+000085b0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
+000085c0: 616e 6473 2074 6f20 7275 6e2e 0a20 2020  ands to run..   
+000085d0: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+000085e0: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+000085f0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+00008600: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+00008610: 7269 6162 6c65 7320 0a20 2020 2020 2020  riables .       
+00008620: 2020 2020 2020 2020 2074 6f20 7365 7420           to set 
+00008630: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
+00008640: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
+00008650: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
+00008660: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00008670: 2020 2020 2020 2020 2020 4c69 7374 5b73            List[s
+00008680: 7472 5d3a 0a20 2020 2020 2020 2020 2020  tr]:.           
+00008690: 2020 2020 2041 206c 6973 7420 6f66 2073       A list of s
+000086a0: 7472 696e 6773 2c20 7768 6572 6520 6561  trings, where ea
+000086b0: 6368 2073 7472 696e 6720 636f 7272 6573  ch string corres
+000086c0: 706f 6e64 7320 746f 0a20 2020 2020 2020  ponds to.       
+000086d0: 2020 2020 2020 2020 2074 6865 206f 7574           the out
+000086e0: 7075 7420 6f66 2061 2073 696e 676c 6520  put of a single 
+000086f0: 636f 6d6d 616e 6420 696e 2060 636d 646c  command in `cmdl
+00008700: 6973 7460 2073 706c 6974 0a20 2020 2020  ist` split.     
+00008710: 2020 2020 2020 2020 2020 2062 7920 7468             by th
+00008720: 6520 7365 7061 7261 746f 7220 605f 4f55  e separator `_OU
+00008730: 545f 5345 5060 2e0a 0a20 2020 2020 2020  T_SEP`...       
+00008740: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00008750: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
+00008760: 6e3a 2049 6620 616e 7920 6f66 2074 6865  n: If any of the
+00008770: 2063 6f6d 6d61 6e64 7320 6661 696c 2074   commands fail t
+00008780: 6f20 6578 6563 7574 6520 7375 6363 6573  o execute succes
+00008790: 7366 756c 6c79 2e0a 2020 2020 2020 2020  sfully..        
+000087a0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
+000087b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000087c0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+000087d0: 6f6d 6d61 6e64 7328 636d 646c 6973 743d  ommands(cmdlist=
+000087e0: 636d 646c 6973 742c 0a20 2020 2020 2020  cmdlist,.       
+000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008810: 656e 763d 656e 762c 0a20 2020 2020 2020  env=env,.       
+00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 7365 703d 6622 203b 2065 6368 6f20 7b73  sep=f" ; echo {s
+00008850: 656c 662e 5f4f 5554 5f53 4550 7d20 3b20  elf._OUT_SEP} ; 
+00008860: 2229 0a20 2020 2020 2020 2065 7863 6570  ").        excep
+00008870: 7420 556e 6578 7065 6374 6564 4578 6974  t UnexpectedExit
+00008880: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00008890: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+000088a0: 6728 6529 0a20 2020 2020 2020 2020 2020  g(e).           
+000088b0: 2072 6573 756c 7420 3d20 652e 7265 7375   result = e.resu
+000088c0: 6c74 0a20 2020 2020 2020 2069 6620 7265  lt.        if re
+000088d0: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
+000088e0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000088f0: 7265 7375 6c74 2e73 7464 6f75 740a 2020  result.stdout.  
+00008900: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
+00008910: 7265 7370 6f6e 7365 7320 3d20 7265 7370  responses = resp
+00008920: 6f6e 7365 2e73 706c 6974 2873 656c 662e  onse.split(self.
+00008930: 5f4f 5554 5f53 4550 290a 2020 2020 2020  _OUT_SEP).      
+00008940: 2020 2020 2020 7265 7475 726e 2073 706c        return spl
+00008950: 6974 5f72 6573 706f 6e73 6573 0a20 2020  it_responses.   
+00008960: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008970: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00008980: 7265 7375 6c74 2069 7320 6e6f 7420 6f6b  result is not ok
+00008990: 2c20 6c6f 6720 7468 6520 6572 726f 7220  , log the error 
+000089a0: 616e 6420 7261 6973 6520 616e 2053 5348  and raise an SSH
+000089b0: 4578 6365 7074 696f 6e0a 2020 2020 2020  Exception.      
+000089c0: 2020 2020 2020 6572 726f 7220 3d20 6622        error = f"
+000089d0: 5265 7375 6c74 2069 7320 6e6f 7420 6f6b  Result is not ok
+000089e0: 3a20 7b72 6573 756c 747d 220a 2020 2020  : {result}".    
+000089f0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00008a00: 7272 6f72 2865 7272 6f72 290a 2020 2020  rror(error).    
+00008a10: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
+00008a20: 4845 7863 6570 7469 6f6e 2865 7272 6f72  HException(error
+00008a30: 290a 0a20 2020 2064 6566 206c 6973 745f  )..    def list_
+00008a40: 6163 7469 7665 5f6a 6f62 7328 7365 6c66  active_jobs(self
+00008a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008a60: 2020 2020 2020 2020 2020 2065 6e76 3a20             env: 
+00008a70: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00008a80: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
+00008a90: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
+00008aa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008ab0: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
+00008ac0: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
+00008ad0: 6d20 534c 5552 4d2e 0a0a 2020 2020 2020  m SLURM...      
+00008ae0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008af0: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
+00008b00: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
+00008b10: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
+00008b20: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00008b30: 6573 2074 6f20 0a20 2020 2020 2020 2020  es to .         
+00008b40: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
+00008b50: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+00008b60: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
+00008b70: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+00008b80: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00008b90: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
+00008ba0: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
+00008bb0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00008bc0: 2020 2020 2020 2023 2063 6d64 203d 2073         # cmd = s
+00008bd0: 656c 662e 5f41 4354 4956 455f 4a4f 4253  elf._ACTIVE_JOBS
+00008be0: 5f43 4d44 0a20 2020 2020 2020 2063 6d64  _CMD.        cmd
+00008bf0: 203d 2073 656c 662e 6765 745f 6a6f 6273   = self.get_jobs
+00008c00: 5f69 6e66 6f5f 636f 6d6d 616e 6428 7374  _info_command(st
+00008c10: 6172 745f 7469 6d65 3d22 6e6f 7722 2c20  art_time="now", 
+00008c20: 7374 6174 6573 3d22 7222 290a 2020 2020  states="r").    
+00008c30: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00008c40: 2252 6574 7269 6576 696e 6720 6c69 7374  "Retrieving list
+00008c50: 206f 6620 6163 7469 7665 206a 6f62 7320   of active jobs 
+00008c60: 6672 6f6d 2053 6c75 726d 2229 0a20 2020  from Slurm").   
+00008c70: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00008c80: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00008c90: 5b63 6d64 5d2c 2065 6e76 3d65 6e76 290a  [cmd], env=env).
+00008ca0: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
+00008cb0: 203d 2072 6573 756c 742e 7374 646f 7574   = result.stdout
+00008cc0: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
+00008cd0: 5c6e 2729 0a20 2020 2020 2020 206a 6f62  \n').        job
+00008ce0: 5f6c 6973 742e 7265 7665 7273 6528 290a  _list.reverse().
+00008cf0: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+00008d00: 6f62 5f6c 6973 740a 0a20 2020 2064 6566  ob_list..    def
+00008d10: 206c 6973 745f 636f 6d70 6c65 7465 645f   list_completed_
+00008d20: 6a6f 6273 2873 656c 662c 0a20 2020 2020  jobs(self,.     
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+00008d50: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+00008d60: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+00008d70: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
+00008d80: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00008d90: 6574 2061 206c 6973 7420 6f66 2063 6f6d  et a list of com
+00008da0: 706c 6574 6564 206a 6f62 7320 6672 6f6d  pleted jobs from
+00008db0: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
+00008dc0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00008dd0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
+00008de0: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
+00008df0: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
+00008e00: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00008e10: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
+00008e20: 2020 2020 2073 6574 2077 6865 6e20 7275       set when ru
+00008e30: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
+00008e40: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
+00008e50: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
+00008e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00008e70: 2020 204c 6973 745b 7374 725d 3a20 4120     List[str]: A 
+00008e80: 6c69 7374 206f 6620 6a6f 6220 4944 732e  list of job IDs.
+00008e90: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00008ea0: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
+00008eb0: 2e67 6574 5f6a 6f62 735f 696e 666f 5f63  .get_jobs_info_c
+00008ec0: 6f6d 6d61 6e64 2873 7461 7465 733d 2263  ommand(states="c
+00008ed0: 6422 290a 2020 2020 2020 2020 6c6f 6767  d").        logg
+00008ee0: 6572 2e69 6e66 6f28 2252 6574 7269 6576  er.info("Retriev
+00008ef0: 696e 6720 6120 6c69 7374 206f 6620 636f  ing a list of co
+00008f00: 6d70 6c65 7465 6420 6a6f 6273 2066 726f  mpleted jobs fro
+00008f10: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
+00008f20: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00008f30: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+00008f40: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
+00008f50: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
+00008f60: 5b6a 6f62 2e73 7472 6970 2829 2066 6f72  [job.strip() for
+00008f70: 206a 6f62 2069 6e20 7265 7375 6c74 2e73   job in result.s
+00008f80: 7464 6f75 742e 7374 7269 7028 292e 7370  tdout.strip().sp
+00008f90: 6c69 7428 275c 6e27 295d 0a20 2020 2020  lit('\n')].     
+00008fa0: 2020 206a 6f62 5f6c 6973 742e 7265 7665     job_list.reve
+00008fb0: 7273 6528 290a 2020 2020 2020 2020 7265  rse().        re
+00008fc0: 7475 726e 206a 6f62 5f6c 6973 740a 0a20  turn job_list.. 
+00008fd0: 2020 2064 6566 206c 6973 745f 616c 6c5f     def list_all_
+00008fe0: 6a6f 6273 2873 656c 662c 2065 6e76 3a20  jobs(self, env: 
+00008ff0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00009000: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
+00009010: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
+00009020: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009030: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
+00009040: 2061 6c6c 206a 6f62 7320 6672 6f6d 2053   all jobs from S
+00009050: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
+00009060: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00009070: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
+00009080: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
+00009090: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
+000090a0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+000090b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000090c0: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
+000090d0: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
+000090e0: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+000090f0: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
+00009100: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00009110: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
+00009120: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
+00009130: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00009140: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
+00009150: 6765 745f 6a6f 6273 5f69 6e66 6f5f 636f  get_jobs_info_co
+00009160: 6d6d 616e 6428 290a 2020 2020 2020 2020  mmand().        
+00009170: 6c6f 6767 6572 2e69 6e66 6f28 2252 6574  logger.info("Ret
+00009180: 7269 6576 696e 6720 6120 6c69 7374 206f  rieving a list o
+00009190: 6620 616c 6c20 6a6f 6273 2066 726f 6d20  f all jobs from 
+000091a0: 536c 7572 6d22 290a 2020 2020 2020 2020  Slurm").        
+000091b0: 7265 7375 6c74 203d 2073 656c 662e 7275  result = self.ru
+000091c0: 6e5f 636f 6d6d 616e 6473 285b 636d 645d  n_commands([cmd]
+000091d0: 2c20 656e 763d 656e 7629 0a20 2020 2020  , env=env).     
+000091e0: 2020 206a 6f62 5f6c 6973 7420 3d20 7265     job_list = re
+000091f0: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
+00009200: 7028 292e 7370 6c69 7428 275c 6e27 290a  p().split('\n').
+00009210: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
+00009220: 2e72 6576 6572 7365 2829 0a20 2020 2020  .reverse().     
+00009230: 2020 2072 6574 7572 6e20 6a6f 625f 6c69     return job_li
+00009240: 7374 0a0a 2020 2020 6465 6620 6765 745f  st..    def get_
+00009250: 6a6f 6273 5f69 6e66 6f5f 636f 6d6d 616e  jobs_info_comman
+00009260: 6428 7365 6c66 2c20 7374 6172 745f 7469  d(self, start_ti
+00009270: 6d65 3a20 7374 7220 3d20 2232 3032 332d  me: str = "2023-
+00009280: 3031 2d30 3122 2c0a 2020 2020 2020 2020  01-01",.        
+00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092a0: 2020 2020 2020 656e 645f 7469 6d65 3a20        end_time: 
+000092b0: 7374 7220 3d20 226e 6f77 222c 0a20 2020  str = "now",.   
+000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092d0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+000092e0: 6e73 3a20 7374 7220 3d20 224a 6f62 4964  ns: str = "JobId
+000092f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2073 7461 7465 733a 2073 7472 203d 2022   states: str = "
+00009320: 722c 6364 2c66 2c74 6f2c 7273 2c64 6c2c  r,cd,f,to,rs,dl,
+00009330: 6e66 2229 202d 3e20 7374 723a 0a20 2020  nf") -> str:.   
+00009340: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+00009350: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
+00009360: 2074 6f20 7265 7472 6965 7665 2069 6e66   to retrieve inf
+00009370: 6f72 6d61 7469 6f6e 2061 626f 7574 206f  ormation about o
+00009380: 6c64 206a 6f62 732e 0a0a 2020 2020 2020  ld jobs...      
+00009390: 2020 5468 6520 636f 6d6d 616e 6420 7769    The command wi
+000093a0: 6c6c 2062 6520 666f 726d 6174 7465 6420  ll be formatted 
+000093b0: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
+000093c0: 6564 2073 7461 7274 2074 696d 652c 2077  ed start time, w
+000093d0: 6869 6368 2069 730a 2020 2020 2020 2020  hich is.        
+000093e0: 6578 7065 6374 6564 2074 6f20 6265 2069  expected to be i
+000093f0: 6e20 7468 6520 4953 4f20 666f 726d 6174  n the ISO format
+00009400: 2022 5959 5959 2d4d 4d2d 4444 222e 0a20   "YYYY-MM-DD".. 
+00009410: 2020 2020 2020 2054 6865 2063 6f6d 6d61         The comma
+00009420: 6e64 2077 696c 6c20 7573 6520 7468 6520  nd will use the 
+00009430: 2273 6163 6374 2220 746f 6f6c 2074 6f20  "sacct" tool to 
+00009440: 7175 6572 7920 7468 650a 2020 2020 2020  query the.      
+00009450: 2020 536c 7572 6d20 6163 636f 756e 7469    Slurm accounti
+00009460: 6e67 2064 6174 6162 6173 6520 666f 7220  ng database for 
+00009470: 6a6f 6273 2074 6861 7420 7374 6172 7465  jobs that starte
+00009480: 6420 6f6e 206f 7220 6166 7465 7220 7468  d on or after th
+00009490: 650a 2020 2020 2020 2020 7370 6563 6966  e.        specif
+000094a0: 6965 6420 7374 6172 7420 7469 6d65 2c20  ied start time, 
+000094b0: 616e 6420 7769 6c6c 206f 7574 7075 7420  and will output 
+000094c0: 6f6e 6c79 2074 6865 206a 6f62 2049 4473  only the job IDs
+000094d0: 2028 2d6f 204a 6f62 4964 290a 2020 2020   (-o JobId).    
+000094e0: 2020 2020 7769 7468 6f75 7420 6865 6164      without head
+000094f0: 6572 206f 7220 7472 6169 6c65 7220 6c69  er or trailer li
+00009500: 6e65 7320 282d 6e20 2d58 292e 0a0a 2020  nes (-n -X)...  
+00009510: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00009520: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+00009530: 6d65 2028 7374 7229 3a20 5468 6520 7374  me (str): The st
+00009540: 6172 7420 7469 6d65 2066 726f 6d20 7768  art time from wh
+00009550: 6963 6820 746f 2072 6574 7269 6576 6520  ich to retrieve 
+00009560: 6a6f 620a 2020 2020 2020 2020 2020 2020  job.            
+00009570: 2020 2020 696e 666f 726d 6174 696f 6e2e      information.
+00009580: 2044 6566 6175 6c74 7320 746f 2022 3230   Defaults to "20
+00009590: 3233 2d30 312d 3031 222e 0a20 2020 2020  23-01-01"..     
+000095a0: 2020 2020 2020 2065 6e64 5f74 696d 6520         end_time 
+000095b0: 2873 7472 293a 2054 6865 2065 6e64 2074  (str): The end t
+000095c0: 696d 6520 756e 7469 6c20 7768 6963 6820  ime until which 
+000095d0: 746f 2072 6574 7269 6576 6520 6a6f 620a  to retrieve job.
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 696e 666f 726d 6174 696f 6e2e 2044 6566  information. Def
+00009600: 6175 6c74 7320 746f 2022 6e6f 7722 2e0a  aults to "now"..
+00009610: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00009620: 6d6e 7320 2873 7472 293a 2054 6865 2063  mns (str): The c
+00009630: 6f6c 756d 6e73 2074 6f20 7265 7472 6965  olumns to retrie
+00009640: 7665 2066 726f 6d20 7468 6520 6a6f 6220  ve from the job 
+00009650: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+00009660: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00009670: 6175 6c74 7320 746f 2022 4a6f 6249 6422  aults to "JobId"
+00009680: 2e20 4974 2069 7320 636f 6d6d 6120 7365  . It is comma se
+00009690: 7061 7261 7465 642c 2065 2e67 2e20 224a  parated, e.g. "J
+000096a0: 6f62 4964 2c53 7461 7465 222e 0a20 2020  obId,State"..   
+000096b0: 2020 2020 2020 2020 2073 7461 7465 7320           states 
+000096c0: 2873 7472 293a 2054 6865 206a 6f62 2073  (str): The job s
+000096d0: 7461 7465 7320 746f 2069 6e63 6c75 6465  tates to include
+000096e0: 2069 6e20 7468 6520 7175 6572 792e 0a20   in the query.. 
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00009700: 6566 6175 6c74 7320 746f 2022 722c 6364  efaults to "r,cd
+00009710: 2c66 2c74 6f2c 7273 2c64 6c2c 6e66 222e  ,f,to,rs,dl,nf".
+00009720: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009730: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00009740: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
+00009750: 2020 2020 4120 7374 7269 6e67 2072 6570      A string rep
+00009760: 7265 7365 6e74 696e 6720 7468 6520 536c  resenting the Sl
+00009770: 7572 6d20 636f 6d6d 616e 6420 746f 2072  urm command to r
+00009780: 6574 7269 6576 650a 2020 2020 2020 2020  etrieve.        
+00009790: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+000097a0: 696f 6e20 6162 6f75 7420 6f6c 6420 6a6f  ion about old jo
+000097b0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
+000097c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000097d0: 656c 662e 5f41 4c4c 5f4a 4f42 535f 434d  elf._ALL_JOBS_CM
+000097e0: 442e 666f 726d 6174 2873 7461 7274 5f74  D.format(start_t
+000097f0: 696d 653d 7374 6172 745f 7469 6d65 2c0a  ime=start_time,.
+00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
+00009830: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009860: 2020 2020 2073 7461 7465 733d 7374 6174       states=stat
+00009870: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000098a0: 756d 6e73 3d63 6f6c 756d 6e73 290a 0a20  umns=columns).. 
+000098b0: 2020 2064 6566 2074 7261 6e73 6665 725f     def transfer_
+000098c0: 6461 7461 2873 656c 662c 206c 6f63 616c  data(self, local
+000098d0: 5f70 6174 683a 2073 7472 2920 2d3e 2052  _path: str) -> R
+000098e0: 6573 756c 743a 0a20 2020 2020 2020 2022  esult:.        "
+000098f0: 2222 0a20 2020 2020 2020 2054 7261 6e73  "".        Trans
+00009900: 6665 7273 2061 2066 696c 6520 6f72 2064  fers a file or d
+00009910: 6972 6563 746f 7279 2066 726f 6d20 7468  irectory from th
+00009920: 6520 6c6f 6361 6c20 6d61 6368 696e 6520  e local machine 
+00009930: 746f 2074 6865 2072 656d 6f74 650a 2020  to the remote.  
+00009940: 2020 2020 2020 536c 7572 6d20 636c 7573        Slurm clus
+00009950: 7465 722e 0a0a 2020 2020 2020 2020 4172  ter...        Ar
+00009960: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00009970: 6c6f 6361 6c5f 7061 7468 2028 7374 7229  local_path (str)
+00009980: 3a20 5468 6520 6c6f 6361 6c20 7061 7468  : The local path
+00009990: 2074 6f20 7468 6520 6669 6c65 206f 7220   to the file or 
+000099a0: 6469 7265 6374 6f72 7920 746f 0a20 2020  directory to.   
+000099b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000099c0: 6e73 6665 722e 0a0a 2020 2020 2020 2020  nsfer...        
+000099d0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000099e0: 2020 2020 2052 6573 756c 743a 2054 6865       Result: The
+000099f0: 2072 6573 756c 7420 6f66 2074 6865 2066   result of the f
+00009a00: 696c 6520 7472 616e 7366 6572 206f 7065  ile transfer ope
+00009a10: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00009a20: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+00009a30: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00009a40: 2020 2020 2066 2254 7261 6e73 6665 7269       f"Transferi
+00009a50: 6e67 2066 696c 6520 7b6c 6f63 616c 5f70  ng file {local_p
+00009a60: 6174 687d 2074 6f20 7b73 656c 662e 736c  ath} to {self.sl
+00009a70: 7572 6d5f 6461 7461 5f70 6174 687d 2229  urm_data_path}")
+00009a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009a90: 7365 6c66 2e70 7574 286c 6f63 616c 3d6c  self.put(local=l
+00009aa0: 6f63 616c 5f70 6174 682c 2072 656d 6f74  ocal_path, remot
+00009ab0: 653d 7365 6c66 2e73 6c75 726d 5f64 6174  e=self.slurm_dat
+00009ac0: 615f 7061 7468 290a 0a20 2020 2064 6566  a_path)..    def
+00009ad0: 2075 6e70 6163 6b5f 6461 7461 2873 656c   unpack_data(sel
+00009ae0: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
+00009af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b00: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
+00009b10: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
+00009b20: 5d5d 203d 204e 6f6e 6529 202d 3e20 5265  ]] = None) -> Re
+00009b30: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
+00009b40: 220a 2020 2020 2020 2020 556e 7061 636b  ".        Unpack
+00009b50: 7320 6120 7a69 7070 6564 2066 696c 6520  s a zipped file 
+00009b60: 6f6e 2074 6865 2072 656d 6f74 6520 536c  on the remote Sl
+00009b70: 7572 6d20 636c 7573 7465 722e 0a0a 2020  urm cluster...  
+00009b80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00009b90: 2020 2020 2020 2020 7a69 7066 696c 6520          zipfile 
+00009ba0: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
+00009bb0: 6f66 2074 6865 207a 6970 7065 6420 6669  of the zipped fi
+00009bc0: 6c65 2074 6f20 6265 2075 6e70 6163 6b65  le to be unpacke
+00009bd0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
+00009be0: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
+00009bf0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+00009c00: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
+00009c10: 6d65 6e74 2076 6172 6961 626c 6573 200a  ment variables .
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 746f 2073 6574 2077 6865 6e20 7275 6e6e  to set when runn
+00009c40: 696e 6720 7468 6520 636f 6d6d 616e 642e  ing the command.
+00009c50: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00009c60: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+00009c70: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00009c80: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
+00009c90: 756c 7420 6f66 2074 6865 2063 6f6d 6d61  ult of the comma
+00009ca0: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+00009cb0: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+00009cc0: 6c66 2e67 6574 5f75 6e7a 6970 5f63 6f6d  lf.get_unzip_com
+00009cd0: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
+00009ce0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00009cf0: 6f28 6622 556e 7061 636b 696e 6720 7b7a  o(f"Unpacking {z
+00009d00: 6970 6669 6c65 7d20 6f6e 2053 6c75 726d  ipfile} on Slurm
+00009d10: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00009d20: 6e20 7365 6c66 2e72 756e 5f63 6f6d 6d61  n self.run_comma
+00009d30: 6e64 7328 5b63 6d64 5d2c 2065 6e76 3d65  nds([cmd], env=e
+00009d40: 6e76 290a 0a20 2020 2064 6566 2063 6f6e  nv)..    def con
+00009d50: 7665 7274 5f64 6174 6128 7365 6c66 2c20  vert_data(self, 
+00009d60: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2065 6e76 3a20 4f70 7469 6f6e 616c     env: Optional
+00009d90: 5b44 6963 745b 7374 722c 2073 7472 5d5d  [Dict[str, str]]
+00009da0: 203d 204e 6f6e 6529 202d 3e20 5265 7375   = None) -> Resu
+00009db0: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
+00009dc0: 2020 2020 2020 2020 556e 7061 636b 7320          Unpacks 
+00009dd0: 6120 7a69 7070 6564 2066 696c 6520 6f6e  a zipped file on
+00009de0: 2074 6865 2072 656d 6f74 6520 536c 7572   the remote Slur
+00009df0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
+00009e00: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00009e10: 2020 2020 2020 7a69 7066 696c 6520 2873        zipfile (s
+00009e20: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+00009e30: 2074 6865 207a 6970 7065 6420 6669 6c65   the zipped file
+00009e40: 2074 6f20 6265 2075 6e70 6163 6b65 642e   to be unpacked.
+00009e50: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00009e60: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
+00009e70: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
+00009e80: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
+00009e90: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00009eb0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
+00009ec0: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
+00009ed0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00009ee0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009ef0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+00009f00: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
+00009f10: 7420 6f66 2074 6865 2063 6f6d 6d61 6e64  t of the command
+00009f20: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00009f30: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
+00009f40: 2e67 6574 5f63 6f6e 7665 7274 5f63 6f6d  .get_convert_com
+00009f50: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
+00009f60: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00009f70: 6f28 6622 436f 6e76 6572 7469 6e67 207b  o(f"Converting {
+00009f80: 7a69 7066 696c 657d 206f 6e20 536c 7572  zipfile} on Slur
+00009f90: 6d22 290a 2020 2020 2020 2020 7265 7475  m").        retu
+00009fa0: 726e 2073 656c 662e 7275 6e5f 636f 6d6d  rn self.run_comm
+00009fb0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
+00009fc0: 656e 7629 0a0a 2020 2020 6465 6620 6765  env)..    def ge
+00009fd0: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
+00009fe0: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7365  _for_workflow(se
+00009ff0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a010: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000a020: 666c 6f77 3a20 7374 722c 0a20 2020 2020  flow: str,.     
+0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
-0000a060: 6a6f 6273 3a20 626f 6f6c 203d 2046 616c  jobs: bool = Fal
-0000a070: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0000a050: 2020 2073 7562 7374 6974 7574 6573 3a20     substitutes: 
+0000a060: 4469 6374 5b73 7472 2c20 7374 725d 2c0a  Dict[str, str],.
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 2065 6e76 3a20 4f70 7469 6f6e 616c 5b44   env: Optional[D
-0000a0a0: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
-0000a0b0: 204e 6f6e 6529 202d 3e20 5265 7375 6c74   None) -> Result
-0000a0c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000a0d0: 2020 2020 2020 5570 6461 7465 7320 7468        Updates th
-0000a0e0: 6520 6c6f 6361 6c20 636f 7079 206f 6620  e local copy of 
-0000a0f0: 7468 6520 536c 7572 6d20 6a6f 6220 7375  the Slurm job su
-0000a100: 626d 6973 7369 6f6e 2073 6372 6970 7473  bmission scripts
-0000a110: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-0000a120: 6675 6e63 7469 6f6e 2070 756c 6c73 2074  function pulls t
-0000a130: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
-0000a140: 6e20 6f66 2074 6865 2073 6372 6970 7473  n of the scripts
-0000a150: 2066 726f 6d20 7468 6520 4769 740a 2020   from the Git.  
-0000a160: 2020 2020 2020 7265 706f 7369 746f 7279        repository
-0000a170: 2061 6e64 2063 6f70 6965 7320 7468 656d   and copies them
-0000a180: 2074 6f20 7468 6520 736c 7572 6d5f 7363   to the slurm_sc
-0000a190: 7269 7074 5f70 6174 6820 6469 7265 6374  ript_path direct
-0000a1a0: 6f72 792e 0a20 2020 2020 2020 2041 6c74  ory..        Alt
-0000a1b0: 6572 6e61 7469 7665 6c79 2c20 6974 2063  ernatively, it c
-0000a1c0: 616e 2067 656e 6572 6174 6520 7363 7269  an generate scri
-0000a1d0: 7074 7320 6672 6f6d 2061 2074 656d 706c  pts from a templ
-0000a1e0: 6174 652e 2054 6869 7320 6973 2074 6865  ate. This is the
-0000a1f0: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
-0000a200: 2062 6568 6176 696f 7220 6966 206e 6f20   behavior if no 
-0000a210: 4769 7420 7265 706f 2069 7320 7072 6f76  Git repo is prov
-0000a220: 6964 6564 206f 7220 6361 6e20 6265 2066  ided or can be f
-0000a230: 6f72 6365 6420 7669 6120 7468 650a 2020  orced via the.  
-0000a240: 2020 2020 2020 6067 656e 6572 6174 655f        `generate_
-0000a250: 6a6f 6273 6020 7061 7261 6d65 7465 722e  jobs` parameter.
-0000a260: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000a270: 2020 2020 2020 2020 2020 2020 6765 6e65              gene
-0000a280: 7261 7465 5f6a 6f62 7320 2862 6f6f 6c29  rate_jobs (bool)
-0000a290: 3a20 5768 6574 6865 7220 746f 2067 656e  : Whether to gen
-0000a2a0: 6572 6174 6520 6e65 7720 736c 7572 6d20  erate new slurm 
-0000a2b0: 6a6f 6220 7363 7269 7074 730a 2020 2020  job scripts.    
-0000a2c0: 2020 2020 2020 2020 2020 2020 494e 5354              INST
-0000a2d0: 4541 4420 286f 6620 7075 6c6c 696e 6720  EAD (of pulling 
-0000a2e0: 6672 6f6d 2067 6974 292e 2044 6566 6175  from git). Defau
-0000a2f0: 6c74 7320 746f 2046 616c 7365 2c20 6578  lts to False, ex
-0000a300: 6365 7074 0a20 2020 2020 2020 2020 2020  cept.           
-0000a310: 2020 2020 2069 6620 6e6f 2073 6c75 726d       if no slurm
-0000a320: 5f73 6372 6970 745f 7265 706f 2069 7320  _script_repo is 
-0000a330: 636f 6e66 6967 7572 6564 2e0a 2020 2020  configured..    
-0000a340: 2020 2020 2020 2020 656e 7620 2844 6963          env (Dic
-0000a350: 745b 7374 722c 2073 7472 5d2c 206f 7074  t[str, str], opt
-0000a360: 696f 6e61 6c29 3a20 4f70 7469 6f6e 616c  ional): Optional
-0000a370: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-0000a380: 6961 626c 6573 200a 2020 2020 2020 2020  iables .        
-0000a390: 2020 2020 2020 2020 746f 2073 6574 2077          to set w
-0000a3a0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
-0000a3b0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
-0000a3c0: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
-0000a3d0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000a3e0: 2020 2020 2020 2020 2052 6573 756c 743a           Result:
-0000a3f0: 2054 6865 2072 6573 756c 7420 6f66 2074   The result of t
-0000a400: 6865 2063 6f6d 6d61 6e64 2e0a 2020 2020  he command..    
-0000a410: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a420: 6966 206e 6f74 2073 656c 662e 736c 7572  if not self.slur
-0000a430: 6d5f 7363 7269 7074 5f72 6570 6f3a 0a20  m_script_repo:. 
-0000a440: 2020 2020 2020 2020 2020 2067 656e 6572             gener
-0000a450: 6174 655f 6a6f 6273 203d 2054 7275 650a  ate_jobs = True.
-0000a460: 0a20 2020 2020 2020 2069 6620 6765 6e65  .        if gene
-0000a470: 7261 7465 5f6a 6f62 733a 0a20 2020 2020  rate_jobs:.     
-0000a480: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000a490: 666f 2822 4765 6e65 7261 7469 6e67 2053  fo("Generating S
-0000a4a0: 6c75 726d 206a 6f62 2073 6372 6970 7473  lurm job scripts
-0000a4b0: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
-0000a4c0: 6f72 2077 662c 206a 6f62 5f70 6174 6820  or wf, job_path 
-0000a4d0: 696e 2073 656c 662e 736c 7572 6d5f 6d6f  in self.slurm_mo
-0000a4e0: 6465 6c5f 6a6f 6273 2e69 7465 6d73 2829  del_jobs.items()
-0000a4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a500: 2020 2320 6765 6e65 7261 7465 206a 6f62    # generate job
-0000a510: 2073 6372 6970 740a 2020 2020 2020 2020   script.        
-0000a520: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-0000a530: 2073 656c 662e 6765 745f 776f 726b 666c   self.get_workfl
-0000a540: 6f77 5f70 6172 616d 6574 6572 7328 7766  ow_parameters(wf
-0000a550: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a560: 2020 7375 6273 203d 2073 656c 662e 776f    subs = self.wo
-0000a570: 726b 666c 6f77 5f70 6172 616d 735f 746f  rkflow_params_to
-0000a580: 5f73 7562 7328 7061 7261 6d73 290a 2020  _subs(params).  
-0000a590: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000a5a0: 625f 7363 7269 7074 203d 2073 656c 662e  b_script = self.
-0000a5b0: 6765 6e65 7261 7465 5f73 6c75 726d 5f6a  generate_slurm_j
-0000a5c0: 6f62 5f66 6f72 5f77 6f72 6b66 6c6f 7728  ob_for_workflow(
-0000a5d0: 7766 2c20 7375 6273 290a 2020 2020 2020  wf, subs).      
-0000a5e0: 2020 2020 2020 2020 2020 2320 656e 7375            # ensu
-0000a5f0: 7265 2061 6c6c 2064 6972 7320 6578 6973  re all dirs exis
-0000a600: 7420 7265 6d6f 7465 6c79 0a20 2020 2020  t remotely.     
-0000a610: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-0000a620: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
-0000a630: 6d5f 7363 7269 7074 5f70 6174 682b 222f  m_script_path+"/
-0000a640: 222b 6a6f 625f 7061 7468 0a20 2020 2020  "+job_path.     
-0000a650: 2020 2020 2020 2020 2020 206a 6f62 5f64             job_d
-0000a660: 6972 2c20 5f20 3d20 6f73 2e70 6174 682e  ir, _ = os.path.
-0000a670: 7370 6c69 7428 6675 6c6c 5f70 6174 6829  split(full_path)
-0000a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a690: 2073 656c 662e 7275 6e28 6622 6d6b 6469   self.run(f"mkdi
-0000a6a0: 7220 2d70 207b 6a6f 625f 6469 727d 2229  r -p {job_dir}")
-0000a6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a6c0: 2023 2063 6f70 7920 746f 2072 656d 6f74   # copy to remot
-0000a6d0: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
-0000a6e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000a6f0: 7365 6c66 2e70 7574 286c 6f63 616c 3d69  self.put(local=i
-0000a700: 6f2e 5374 7269 6e67 494f 286a 6f62 5f73  o.StringIO(job_s
-0000a710: 6372 6970 7429 2c0a 2020 2020 2020 2020  cript),.        
-0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a730: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-0000a740: 3d66 756c 6c5f 7061 7468 290a 2020 2020  =full_path).    
-0000a750: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a760: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-0000a770: 2e67 6574 5f75 7064 6174 655f 736c 7572  .get_update_slur
-0000a780: 6d5f 7363 7269 7074 735f 636f 6d6d 616e  m_scripts_comman
-0000a790: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000a7a0: 6c6f 6767 6572 2e69 6e66 6f28 2255 7064  logger.info("Upd
-0000a7b0: 6174 696e 6720 536c 7572 6d20 6a6f 6220  ating Slurm job 
-0000a7c0: 7363 7269 7074 7320 6f6e 2053 6c75 726d  scripts on Slurm
-0000a7d0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-0000a7e0: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-0000a7f0: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d2c  _commands([cmd],
-0000a800: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
-0000a810: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0000a820: 0a20 2020 2064 6566 2072 756e 5f77 6f72  .    def run_wor
-0000a830: 6b66 6c6f 7728 7365 6c66 2c0a 2020 2020  kflow(self,.    
-0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a850: 2077 6f72 6b66 6c6f 775f 6e61 6d65 3a20   workflow_name: 
-0000a860: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000a870: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000a880: 6f77 5f76 6572 7369 6f6e 3a20 7374 722c  ow_version: str,
-0000a890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a8a0: 2020 2020 2020 696e 7075 745f 6461 7461        input_data
-0000a8b0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-0000a8c0: 2020 2020 2020 2020 2020 2020 656d 6169              emai
-0000a8d0: 6c3a 204f 7074 696f 6e61 6c5b 7374 725d  l: Optional[str]
-0000a8e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-0000a900: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-0000a910: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000a920: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000a930: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
-0000a940: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-0000a950: 3e20 5475 706c 655b 5265 7375 6c74 2c20  > Tuple[Result, 
-0000a960: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
-0000a970: 220a 2020 2020 2020 2020 5275 6e20 6120  ".        Run a 
-0000a980: 7370 6563 6966 6965 6420 776f 726b 666c  specified workfl
-0000a990: 6f77 206f 6e20 536c 7572 6d20 7573 696e  ow on Slurm usin
-0000a9a0: 6720 7468 6520 6769 7665 6e20 7061 7261  g the given para
-0000a9b0: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
-0000a9c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000a9d0: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
-0000a9e0: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
-0000a9f0: 7468 6520 776f 726b 666c 6f77 2074 6f20  the workflow to 
-0000aa00: 6578 6563 7574 652e 0a20 2020 2020 2020  execute..       
-0000aa10: 2020 2020 2077 6f72 6b66 6c6f 775f 7665       workflow_ve
-0000aa20: 7273 696f 6e20 2873 7472 293a 2056 6572  rsion (str): Ver
-0000aa30: 7369 6f6e 206f 6620 7468 6520 776f 726b  sion of the work
-0000aa40: 666c 6f77 2028 696d 6167 6520 7665 7273  flow (image vers
-0000aa50: 696f 6e20 0a20 2020 2020 2020 2020 2020  ion .           
-0000aa60: 2020 2020 206f 6e20 536c 7572 6d29 2e0a       on Slurm)..
-0000aa70: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000aa80: 745f 6461 7461 2028 7374 7229 3a20 4e61  t_data (str): Na
-0000aa90: 6d65 206f 6620 7468 6520 696e 7075 7420  me of the input 
-0000aaa0: 6461 7461 2066 6f6c 6465 7220 636f 6e74  data folder cont
-0000aab0: 6169 6e69 6e67 2069 6e70 7574 0a20 2020  aining input.   
-0000aac0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0000aad0: 6765 2066 696c 6573 2e0a 2020 2020 2020  ge files..      
-0000aae0: 2020 2020 2020 656d 6169 6c20 2873 7472        email (str
-0000aaf0: 2c20 6f70 7469 6f6e 616c 293a 2045 6d61  , optional): Ema
-0000ab00: 696c 2061 6464 7265 7373 2066 6f72 2053  il address for S
-0000ab10: 6c75 726d 206a 6f62 206e 6f74 6966 6963  lurm job notific
-0000ab20: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
-0000ab30: 2020 2020 7469 6d65 2028 7374 722c 206f      time (str, o
-0000ab40: 7074 696f 6e61 6c29 3a20 5469 6d65 206c  ptional): Time l
-0000ab50: 696d 6974 2066 6f72 2074 6865 2053 6c75  imit for the Slu
-0000ab60: 726d 206a 6f62 2069 6e20 7468 6520 0a20  rm job in the . 
-0000ab70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ab80: 6f72 6d61 7420 4848 3a4d 4d3a 5353 2e0a  ormat HH:MM:SS..
-0000ab90: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-0000aba0: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
-0000abb0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-0000abc0: 7473 2066 6f72 2074 6865 2077 6f72 6b66  ts for the workf
-0000abd0: 6c6f 772e 0a0a 2020 2020 2020 2020 5265  low...        Re
-0000abe0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000abf0: 2020 2054 7570 6c65 5b52 6573 756c 742c     Tuple[Result,
-0000ac00: 2069 6e74 5d3a 0a20 2020 2020 2020 2020   int]:.         
-0000ac10: 2020 2020 2020 2041 2074 7570 6c65 2063         A tuple c
-0000ac20: 6f6e 7461 696e 696e 6720 7468 6520 7265  ontaining the re
-0000ac30: 7375 6c74 206f 6620 7374 6172 7469 6e67  sult of starting
-0000ac40: 2074 6865 2077 6f72 6b66 6c6f 7720 6a6f   the workflow jo
-0000ac50: 6220 616e 640a 2020 2020 2020 2020 2020  b and.          
-0000ac60: 2020 2020 2020 7468 6520 536c 7572 6d20        the Slurm 
-0000ac70: 6a6f 6220 4944 2c20 6f72 202d 3120 6966  job ID, or -1 if
-0000ac80: 2074 6865 206a 6f62 2049 4420 636f 756c   the job ID coul
-0000ac90: 6420 6e6f 7420 6265 2065 7874 7261 6374  d not be extract
-0000aca0: 6564 2e0a 0a20 2020 2020 2020 204e 6f74  ed...        Not
-0000acb0: 653a 0a20 2020 2020 2020 2020 2020 2054  e:.            T
-0000acc0: 6865 2053 6c75 726d 206a 6f62 2049 4420  he Slurm job ID 
-0000acd0: 6973 2065 7874 7261 6374 6564 2066 726f  is extracted fro
-0000ace0: 6d20 7468 6520 7265 7375 6c74 206f 6620  m the result of 
-0000acf0: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
-0000ad00: 2060 7275 6e5f 636f 6d6d 616e 6473 6020   `run_commands` 
-0000ad10: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-0000ad20: 2222 220a 2020 2020 2020 2020 7362 6174  """.        sbat
-0000ad30: 6368 5f63 6d64 2c20 7362 6174 6368 5f65  ch_cmd, sbatch_e
-0000ad40: 6e76 203d 2073 656c 662e 6765 745f 776f  nv = self.get_wo
-0000ad50: 726b 666c 6f77 5f63 6f6d 6d61 6e64 280a  rkflow_command(.
-0000ad60: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000ad70: 666c 6f77 5f6e 616d 652c 2077 6f72 6b66  flow_name, workf
-0000ad80: 6c6f 775f 7665 7273 696f 6e2c 2069 6e70  low_version, inp
-0000ad90: 7574 5f64 6174 612c 2065 6d61 696c 2c20  ut_data, email, 
-0000ada0: 7469 6d65 2c20 2a2a 6b77 6172 6773 290a  time, **kwargs).
-0000adb0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-0000adc0: 5275 6e6e 696e 6720 7b77 6f72 6b66 6c6f  Running {workflo
-0000add0: 775f 6e61 6d65 7d20 6a6f 6220 6f6e 207b  w_name} job on {
-0000ade0: 696e 7075 745f 6461 7461 7d20 6f6e 2053  input_data} on S
-0000adf0: 6c75 726d 3a5c 0a20 2020 2020 2020 2020  lurm:\.         
-0000ae00: 2020 207b 7362 6174 6368 5f63 6d64 7d20     {sbatch_cmd} 
-0000ae10: 772f 207b 7362 6174 6368 5f65 6e76 7d22  w/ {sbatch_env}"
-0000ae20: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-0000ae30: 2e69 6e66 6f28 6622 5275 6e6e 696e 6720  .info(f"Running 
-0000ae40: 7b77 6f72 6b66 6c6f 775f 6e61 6d65 7d20  {workflow_name} 
-0000ae50: 6a6f 6220 6f6e 207b 696e 7075 745f 6461  job on {input_da
-0000ae60: 7461 7d20 6f6e 2053 6c75 726d 2229 0a20  ta} on Slurm"). 
-0000ae70: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-0000ae80: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-0000ae90: 7362 6174 6368 5f63 6d64 5d2c 2073 6261  sbatch_cmd], sba
-0000aea0: 7463 685f 656e 7629 0a20 2020 2020 2020  tch_env).       
-0000aeb0: 2072 6574 7572 6e20 7265 732c 2073 656c   return res, sel
-0000aec0: 662e 6578 7472 6163 745f 6a6f 625f 6964  f.extract_job_id
-0000aed0: 2872 6573 290a 0a20 2020 2064 6566 2072  (res)..    def r
-0000aee0: 756e 5f77 6f72 6b66 6c6f 775f 6a6f 6228  un_workflow_job(
-0000aef0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000af10: 6f72 6b66 6c6f 775f 6e61 6d65 3a20 7374  orkflow_name: st
-0000af20: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000af30: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000af40: 666c 6f77 5f76 6572 7369 6f6e 3a20 7374  flow_version: st
-0000af50: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000af60: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000af70: 745f 6461 7461 3a20 7374 722c 0a20 2020  t_data: str,.   
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2020 2020 2020 656d 6169 6c3a 204f 7074        email: Opt
-0000afa0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000afb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000afc0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000afd0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000afe0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b020: 2020 2029 202d 3e20 536c 7572 6d4a 6f62     ) -> SlurmJob
-0000b030: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000b040: 2020 2020 2020 5275 6e20 6120 7370 6563        Run a spec
-0000b050: 6966 6965 6420 776f 726b 666c 6f77 206f  ified workflow o
-0000b060: 6e20 536c 7572 6d20 7573 696e 6720 7468  n Slurm using th
-0000b070: 6520 6769 7665 6e20 7061 7261 6d65 7465  e given paramete
-0000b080: 7273 2061 6e64 2072 6574 7572 6e20 6120  rs and return a 
-0000b090: 536c 7572 6d4a 6f62 2069 6e73 7461 6e63  SlurmJob instanc
-0000b0a0: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-0000b0b0: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
-0000b0c0: 726b 666c 6f77 5f6e 616d 6520 2873 7472  rkflow_name (str
-0000b0d0: 293a 204e 616d 6520 6f66 2074 6865 2077  ): Name of the w
-0000b0e0: 6f72 6b66 6c6f 7720 746f 2065 7865 6375  orkflow to execu
-0000b0f0: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
-0000b100: 776f 726b 666c 6f77 5f76 6572 7369 6f6e  workflow_version
-0000b110: 2028 7374 7229 3a20 5665 7273 696f 6e20   (str): Version 
-0000b120: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
-0000b130: 2869 6d61 6765 2076 6572 7369 6f6e 206f  (image version o
-0000b140: 6e20 536c 7572 6d29 2e0a 2020 2020 2020  n Slurm)..      
-0000b150: 2020 2020 2020 696e 7075 745f 6461 7461        input_data
-0000b160: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
-0000b170: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
-0000b180: 6f6c 6465 7220 636f 6e74 6169 6e69 6e67  older containing
-0000b190: 2069 6e70 7574 2069 6d61 6765 2066 696c   input image fil
-0000b1a0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0000b1b0: 656d 6169 6c20 2873 7472 2c20 6f70 7469  email (str, opti
-0000b1c0: 6f6e 616c 293a 2045 6d61 696c 2061 6464  onal): Email add
-0000b1d0: 7265 7373 2066 6f72 2053 6c75 726d 206a  ress for Slurm j
-0000b1e0: 6f62 206e 6f74 6966 6963 6174 696f 6e73  ob notifications
-0000b1f0: 2e0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-0000b200: 6d65 2028 7374 722c 206f 7074 696f 6e61  me (str, optiona
-0000b210: 6c29 3a20 5469 6d65 206c 696d 6974 2066  l): Time limit f
-0000b220: 6f72 2074 6865 2053 6c75 726d 206a 6f62  or the Slurm job
-0000b230: 2069 6e20 7468 6520 666f 726d 6174 2048   in the format H
-0000b240: 483a 4d4d 3a53 532e 0a20 2020 2020 2020  H:MM:SS..       
-0000b250: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
-0000b260: 6464 6974 696f 6e61 6c20 6b65 7977 6f72  dditional keywor
-0000b270: 6420 6172 6775 6d65 6e74 7320 666f 7220  d arguments for 
-0000b280: 7468 6520 776f 726b 666c 6f77 2e0a 0a20  the workflow... 
-0000b290: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000b2a0: 2020 2020 2020 2020 2020 2020 536c 7572              Slur
-0000b2b0: 6d4a 6f62 3a20 4120 536c 7572 6d4a 6f62  mJob: A SlurmJob
-0000b2c0: 2069 6e73 7461 6e63 6520 7265 7072 6573   instance repres
-0000b2d0: 656e 7469 6e67 2074 6865 2073 7461 7274  enting the start
-0000b2e0: 6564 2077 6f72 6b66 6c6f 7720 6a6f 622e  ed workflow job.
-0000b2f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b300: 2020 2020 2072 6573 756c 742c 206a 6f62       result, job
-0000b310: 5f69 6420 3d20 7365 6c66 2e72 756e 5f77  _id = self.run_w
-0000b320: 6f72 6b66 6c6f 7728 0a20 2020 2020 2020  orkflow(.       
-0000b330: 2020 2020 2077 6f72 6b66 6c6f 775f 6e61       workflow_na
-0000b340: 6d65 2c20 776f 726b 666c 6f77 5f76 6572  me, workflow_ver
-0000b350: 7369 6f6e 2c20 696e 7075 745f 6461 7461  sion, input_data
-0000b360: 2c20 656d 6169 6c2c 2074 696d 652c 202a  , email, time, *
-0000b370: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-0000b380: 2072 6574 7572 6e20 536c 7572 6d4a 6f62   return SlurmJob
-0000b390: 2872 6573 756c 742c 206a 6f62 5f69 6429  (result, job_id)
-0000b3a0: 0a0a 2020 2020 6465 6620 7275 6e5f 636f  ..    def run_co
-0000b3b0: 6e76 6572 7369 6f6e 5f77 6f72 6b66 6c6f  nversion_workflo
-0000b3c0: 775f 6a6f 6228 7365 6c66 2c20 666f 6c64  w_job(self, fold
-0000b3d0: 6572 5f6e 616d 653a 2073 7472 2c0a 2020  er_name: str,.  
-0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 736f 7572 6365 5f66 6f72 6d61 743a    source_format:
-0000b410: 2073 7472 203d 2027 7a61 7272 272c 0a20   str = 'zarr',. 
-0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2074 6172 6765 745f 666f 726d 6174     target_format
-0000b450: 3a20 7374 7220 3d20 2774 6966 6627 0a20  : str = 'tiff'. 
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2020 2029 202d 3e20 5475 706c 655b 5265     ) -> Tuple[Re
-0000b490: 7375 6c74 2c20 696e 745d 3a0a 2020 2020  sult, int]:.    
-0000b4a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000b4b0: 5275 6e20 7468 6520 6461 7461 2063 6f6e  Run the data con
-0000b4c0: 7665 7273 696f 6e20 776f 726b 666c 6f77  version workflow
-0000b4d0: 206f 6e20 536c 7572 6d20 7573 696e 6720   on Slurm using 
-0000b4e0: 7468 6520 6769 7665 6e20 6461 7461 2066  the given data f
-0000b4f0: 6f6c 6465 722e 0a0a 2020 2020 2020 2020  older...        
-0000b500: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000b510: 2020 666f 6c64 6572 5f6e 616d 6520 2873    folder_name (s
-0000b520: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-0000b530: 2074 6865 2064 6174 6120 666f 6c64 6572   the data folder
-0000b540: 2063 6f6e 7461 696e 696e 6720 736f 7572   containing sour
-0000b550: 6365 2066 6f72 6d61 7420 6669 6c65 732e  ce format files.
-0000b560: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-0000b570: 7263 655f 666f 726d 6174 2028 7374 7229  rce_format (str)
-0000b580: 3a20 536f 7572 6365 2064 6174 6120 666f  : Source data fo
-0000b590: 726d 6174 2066 6f72 2063 6f6e 7665 7273  rmat for convers
-0000b5a0: 696f 6e20 2864 6566 6175 6c74 2069 7320  ion (default is 
-0000b5b0: 277a 6172 7227 292e 0a20 2020 2020 2020  'zarr')..       
-0000b5c0: 2020 2020 2074 6172 6765 745f 666f 726d       target_form
-0000b5d0: 6174 2028 7374 7229 3a20 5461 7267 6574  at (str): Target
-0000b5e0: 2064 6174 6120 666f 726d 6174 2061 6674   data format aft
-0000b5f0: 6572 2063 6f6e 7665 7273 696f 6e20 2864  er conversion (d
-0000b600: 6566 6175 6c74 2069 7320 2774 6966 6627  efault is 'tiff'
-0000b610: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
-0000b620: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000b630: 2054 7570 6c65 5b52 6573 756c 742c 2069   Tuple[Result, i
-0000b640: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
-0000b650: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
-0000b660: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
-0000b670: 6c74 206f 6620 7374 6172 7469 6e67 2074  lt of starting t
-0000b680: 6865 2063 6f6e 7665 7273 696f 6e20 6a6f  he conversion jo
-0000b690: 6220 616e 640a 2020 2020 2020 2020 2020  b and.          
-0000b6a0: 2020 2020 2020 7468 6520 536c 7572 6d20        the Slurm 
-0000b6b0: 6a6f 6220 4944 2c20 6f72 202d 3120 6966  job ID, or -1 if
-0000b6c0: 2074 6865 206a 6f62 2049 4420 636f 756c   the job ID coul
-0000b6d0: 6420 6e6f 7420 6265 2065 7874 7261 6374  d not be extract
-0000b6e0: 6564 2e0a 0a20 2020 2020 2020 2057 6172  ed...        War
-0000b6f0: 6e69 6e67 3a0a 2020 2020 2020 2020 2020  ning:.          
-0000b700: 2020 5468 6520 6465 6661 756c 7420 696d    The default im
-0000b710: 706c 656d 656e 7461 7469 6f6e 206f 6e6c  plementation onl
-0000b720: 7920 7375 7070 6f72 7473 2063 6f6e 7665  y supports conve
-0000b730: 7273 696f 6e20 6672 6f6d 2027 7a61 7272  rsion from 'zarr
-0000b740: 2720 746f 2027 7469 6666 272e 0a20 2020  ' to 'tiff'..   
-0000b750: 2020 2020 2020 2020 2049 6620 7573 696e           If usin
-0000b760: 6720 6f74 6865 7220 736f 7572 6365 206f  g other source o
-0000b770: 7220 7461 7267 6574 2066 6f72 6d61 7473  r target formats
-0000b780: 2c20 7573 6572 7320 6d75 7374 2069 6d70  , users must imp
-0000b790: 6c65 6d65 6e74 2061 6e64 2063 6f6e 6669  lement and confi
-0000b7a0: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
-0000b7b0: 2061 6464 6974 696f 6e61 6c20 636f 6e76   additional conv
-0000b7c0: 6572 7465 7273 2074 6865 6d73 656c 7665  erters themselve
-0000b7d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0000b7e0: 2020 2020 2020 2023 2047 656e 6572 6174         # Generat
-0000b7f0: 6520 6120 756e 6971 7565 2063 6f6e 6669  e a unique confi
-0000b800: 6720 6669 6c65 206e 616d 650a 2020 2020  g file name.    
-0000b810: 2020 2020 636f 6e66 6967 5f66 696c 6520      config_file 
-0000b820: 3d20 6622 636f 6e66 6967 5f7b 666f 6c64  = f"config_{fold
-0000b830: 6572 5f6e 616d 657d 2e74 7874 220a 0a20  er_name}.txt".. 
-0000b840: 2020 2020 2020 2023 2043 6f6e 7374 7275         # Constru
-0000b850: 6374 2061 6c6c 2063 6f6d 6d61 6e64 7320  ct all commands 
-0000b860: 746f 2072 756e 2063 6f6e 7365 6375 7469  to run consecuti
-0000b870: 7665 6c79 0a20 2020 2020 2020 2064 6174  vely.        dat
-0000b880: 615f 7061 7468 203d 2066 227b 7365 6c66  a_path = f"{self
-0000b890: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-0000b8a0: 7d2f 7b66 6f6c 6465 725f 6e61 6d65 7d22  }/{folder_name}"
-0000b8b0: 0a20 2020 2020 2020 2063 6f6e 7665 7273  .        convers
-0000b8c0: 696f 6e5f 636d 642c 2073 6261 7463 685f  ion_cmd, sbatch_
-0000b8d0: 656e 7620 3d20 7365 6c66 2e67 6574 5f63  env = self.get_c
-0000b8e0: 6f6e 7665 7273 696f 6e5f 636f 6d6d 616e  onversion_comman
-0000b8f0: 6428 0a20 2020 2020 2020 2020 2020 2064  d(.            d
-0000b900: 6174 615f 7061 7468 2c20 636f 6e66 6967  ata_path, config
-0000b910: 5f66 696c 652c 2073 6f75 7263 655f 666f  _file, source_fo
-0000b920: 726d 6174 2c20 7461 7267 6574 5f66 6f72  rmat, target_for
-0000b930: 6d61 7429 0a20 2020 2020 2020 2063 6f6d  mat).        com
-0000b940: 6d61 6e64 7320 3d20 5b0a 2020 2020 2020  mands = [.      
-0000b950: 2020 2020 2020 6622 6669 6e64 207b 6461        f"find {da
-0000b960: 7461 5f70 6174 687d 2f64 6174 612f 696e  ta_path}/data/in
-0000b970: 202d 6e61 6d65 2027 2a2e 7b73 6f75 7263   -name '*.{sourc
-0000b980: 655f 666f 726d 6174 7d27 207c 2061 776b  e_format}' | awk
-0000b990: 2027 7b7b 7072 696e 7420 4e52 2c20 2430   '{{print NR, $0
-0000b9a0: 7d7d 2720 3e20 7b63 6f6e 6669 675f 6669  }}' > {config_fi
-0000b9b0: 6c65 7d22 2c0a 2020 2020 2020 2020 2020  le}",.          
-0000b9c0: 2020 6622 4e3d 2428 7763 202d 6c20 3c20    f"N=$(wc -l < 
-0000b9d0: 5c22 7b63 6f6e 6669 675f 6669 6c65 7d5c  \"{config_file}\
-0000b9e0: 2229 222c 0a20 2020 2020 2020 2020 2020  ")",.           
-0000b9f0: 2066 2265 6368 6f20 5c22 4e75 6d62 6572   f"echo \"Number
-0000ba00: 206f 6620 2e7b 736f 7572 6365 5f66 6f72   of .{source_for
-0000ba10: 6d61 747d 2066 696c 6573 3a20 244e 5c22  mat} files: $N\"
-0000ba20: 222c 0a20 2020 2020 2020 2020 2020 2063  ",.            c
-0000ba30: 6f6e 7665 7273 696f 6e5f 636d 640a 2020  onversion_cmd.  
-0000ba40: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-0000ba50: 2023 2052 756e 2061 6c6c 2063 6f6d 6d61   # Run all comma
-0000ba60: 6e64 7320 636f 6e73 6563 7574 6976 656c  nds consecutivel
-0000ba70: 790a 2020 2020 2020 2020 7265 7320 3d20  y.        res = 
-0000ba80: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000ba90: 7328 636f 6d6d 616e 6473 2c20 7362 6174  s(commands, sbat
-0000baa0: 6368 5f65 6e76 290a 0a20 2020 2020 2020  ch_env)..       
-0000bab0: 2072 6574 7572 6e20 536c 7572 6d4a 6f62   return SlurmJob
-0000bac0: 2872 6573 2c20 7365 6c66 2e65 7874 7261  (res, self.extra
-0000bad0: 6374 5f6a 6f62 5f69 6428 7265 7329 290a  ct_job_id(res)).
-0000bae0: 0a20 2020 2064 6566 2065 7874 7261 6374  .    def extract
-0000baf0: 5f6a 6f62 5f69 6428 7365 6c66 2c20 7265  _job_id(self, re
-0000bb00: 7375 6c74 3a20 5265 7375 6c74 2920 2d3e  sult: Result) ->
-0000bb10: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000bb20: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
-0000bb30: 7420 7468 6520 536c 7572 6d20 6a6f 6220  t the Slurm job 
-0000bb40: 4944 2066 726f 6d20 7468 6520 7265 7375  ID from the resu
-0000bb50: 6c74 206f 6620 6120 636f 6d6d 616e 642e  lt of a command.
-0000bb60: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000bb70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000bb80: 6c74 2028 5265 7375 6c74 293a 2054 6865  lt (Result): The
-0000bb90: 2072 6573 756c 7420 6f66 2061 2063 6f6d   result of a com
-0000bba0: 6d61 6e64 2065 7865 6375 7469 6f6e 2e0a  mand execution..
-0000bbb0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000bbc0: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-0000bbd0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000bbe0: 2020 2054 6865 2053 6c75 726d 206a 6f62     The Slurm job
-0000bbf0: 2049 4420 6578 7472 6163 7465 6420 6672   ID extracted fr
-0000bc00: 6f6d 2074 6865 2072 6573 756c 742c 0a20  om the result,. 
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000bc20: 7220 2d31 2069 6620 6e6f 7420 666f 756e  r -1 if not foun
-0000bc30: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-0000bc40: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-0000bc50: 5f69 6420 3d20 6e65 7874 2828 696e 7428  _id = next((int(
-0000bc60: 732e 7374 7269 7028 2929 2066 6f72 2073  s.strip()) for s
-0000bc70: 2069 6e20 7265 7375 6c74 2e73 7464 6f75   in result.stdou
-0000bc80: 742e 7370 6c69 7428 0a20 2020 2020 2020  t.split(.       
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2022 5375 626d 6974 7465 6420       "Submitted 
-0000bcb0: 6261 7463 6820 6a6f 6222 2920 6966 2073  batch job") if s
-0000bcc0: 2e73 7472 6970 2829 2e69 7364 6967 6974  .strip().isdigit
-0000bcd0: 2829 292c 202d 3129 0a20 2020 2020 2020  ()), -1).       
-0000bce0: 2072 6574 7572 6e20 736c 7572 6d5f 6a6f   return slurm_jo
-0000bcf0: 625f 6964 0a0a 2020 2020 6465 6620 6765  b_id..    def ge
-0000bd00: 745f 7570 6461 7465 5f73 6c75 726d 5f73  t_update_slurm_s
-0000bd10: 6372 6970 7473 5f63 6f6d 6d61 6e64 2873  cripts_command(s
-0000bd20: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-0000bd30: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-0000bd40: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
-0000bd50: 7570 6461 7465 2074 6865 2047 6974 2072  update the Git r
-0000bd60: 6570 6f73 6974 6f72 7920 636f 6e74 6169  epository contai
-0000bd70: 6e69 6e67 0a20 2020 2020 2020 2074 6865  ning.        the
-0000bd80: 2053 6c75 726d 2073 6372 6970 7473 2c20   Slurm scripts, 
-0000bd90: 6966 206e 6563 6573 7361 7279 2e0a 0a20  if necessary... 
-0000bda0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000bdb0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-0000bdc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bdd0: 2041 2073 7472 696e 6720 636f 6e74 6169   A string contai
-0000bde0: 6e69 6e67 2074 6865 2047 6974 2063 6f6d  ning the Git com
-0000bdf0: 6d61 6e64 0a20 2020 2020 2020 2020 2020  mand.           
-0000be00: 2020 2020 2074 6f20 7570 6461 7465 2074       to update t
-0000be10: 6865 2053 6c75 726d 2073 6372 6970 7473  he Slurm scripts
-0000be20: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000be30: 2020 2020 2020 7570 6461 7465 5f63 6d64        update_cmd
-0000be40: 203d 2066 2267 6974 202d 4320 7b73 656c   = f"git -C {sel
-0000be50: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
-0000be60: 6174 687d 2070 756c 6c22 0a20 2020 2020  ath} pull".     
-0000be70: 2020 2072 6574 7572 6e20 7570 6461 7465     return update
-0000be80: 5f63 6d64 0a0a 2020 2020 6465 6620 6368  _cmd..    def ch
-0000be90: 6563 6b5f 6a6f 625f 7374 6174 7573 2873  eck_job_status(s
-0000bea0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-0000bec0: 7572 6d5f 6a6f 625f 6964 733a 204c 6973  urm_job_ids: Lis
-0000bed0: 745b 696e 745d 2c0a 2020 2020 2020 2020  t[int],.        
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2065 6e76 3a20 4f70 7469 6f6e 616c 5b44   env: Optional[D
-0000bf00: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
-0000bf10: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000bf30: 202d 3e20 5475 706c 655b 4469 6374 5b69   -> Tuple[Dict[i
-0000bf40: 6e74 2c20 7374 725d 2c20 5265 7375 6c74  nt, str], Result
-0000bf50: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0000bf60: 2020 2020 2020 2043 6865 636b 2074 6865         Check the
-0000bf70: 2073 7461 7475 7320 6f66 2053 6c75 726d   status of Slurm
-0000bf80: 206a 6f62 7320 7769 7468 2074 6865 2067   jobs with the g
-0000bf90: 6976 656e 206a 6f62 2049 4473 2e0a 2020  iven job IDs..  
-0000bfa0: 2020 2020 2020 0a20 2020 2020 2020 204e        .        N
-0000bfb0: 6f74 653a 2054 6869 7320 646f 6573 6e27  ote: This doesn'
-0000bfc0: 7420 7265 7475 726e 206a 6f62 2061 7272  t return job arr
-0000bfd0: 6179 7320 696e 6469 7669 6475 616c 6c79  ays individually
-0000bfe0: 2e0a 2020 2020 2020 2020 4974 2074 616b  ..        It tak
-0000bff0: 6573 2074 6865 206c 6173 7420 7661 6c75  es the last valu
-0000c000: 6520 7265 7475 726e 6564 2066 6f72 2074  e returned for t
-0000c010: 686f 7365 2073 7562 2069 6473 200a 2020  hose sub ids .  
-0000c020: 2020 2020 2020 2867 656e 6572 616c 6c79        (generally
-0000c030: 2074 6865 206f 6e65 2073 7469 6c6c 2050   the one still P
-0000c040: 454e 4449 4e47 292e 0a0a 2020 2020 2020  ENDING)...      
-0000c050: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000c060: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
-0000c070: 7320 284c 6973 745b 696e 745d 293a 2054  s (List[int]): T
-0000c080: 6865 206a 6f62 2049 4473 206f 6620 7468  he job IDs of th
-0000c090: 6520 536c 7572 6d20 6a6f 6273 2074 6f20  e Slurm jobs to 
-0000c0a0: 6368 6563 6b2e 0a20 2020 2020 2020 2020  check..         
-0000c0b0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-0000c0c0: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-0000c0d0: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-0000c0e0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-0000c0f0: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
-0000c100: 2020 2020 2073 6574 2077 6865 6e20 7275       set when ru
-0000c110: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-0000c120: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
-0000c130: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
-0000c140: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000c150: 2020 2054 7570 6c65 5b44 6963 745b 696e     Tuple[Dict[in
-0000c160: 742c 2073 7472 5d2c 2052 6573 756c 745d  t, str], Result]
-0000c170: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c180: 2020 4120 7475 706c 6520 636f 6e74 6169    A tuple contai
-0000c190: 6e69 6e67 2074 6865 2073 7461 7475 7320  ning the status 
-0000c1a0: 7065 7220 696e 7075 7420 4944 2061 6e64  per input ID and
-0000c1b0: 2074 6865 2072 6573 756c 7420 6f66 200a   the result of .
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 7468 6520 636f 6d6d 616e 6420 6578 6563  the command exec
-0000c1e0: 7574 696f 6e2e 0a0a 2020 2020 2020 2020  ution...        
-0000c1f0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-0000c200: 2020 2020 5353 4845 7863 6570 7469 6f6e      SSHException
-0000c210: 3a20 4966 2074 6865 2063 6f6d 6d61 6e64  : If the command
-0000c220: 2065 7865 6375 7469 6f6e 2066 6169 6c73   execution fails
-0000c230: 206f 7220 6e6f 2072 6573 706f 6e73 6520   or no response 
-0000c240: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
-0000c250: 2020 2072 6563 6569 7665 6420 6166 7465     received afte
-0000c260: 7220 6d75 6c74 6970 6c65 2072 6574 7269  r multiple retri
-0000c270: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-0000c280: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-0000c290: 6c66 2e67 6574 5f6a 6f62 5f73 7461 7475  lf.get_job_statu
-0000c2a0: 735f 636f 6d6d 616e 6428 736c 7572 6d5f  s_command(slurm_
-0000c2b0: 6a6f 625f 6964 7329 0a20 2020 2020 2020  job_ids).       
-0000c2c0: 206c 6f67 6765 722e 696e 666f 2866 2247   logger.info(f"G
-0000c2d0: 6574 7469 6e67 2073 7461 7475 7320 6f66  etting status of
-0000c2e0: 207b 736c 7572 6d5f 6a6f 625f 6964 737d   {slurm_job_ids}
-0000c2f0: 206f 6e20 536c 7572 6d22 290a 2020 2020   on Slurm").    
-0000c300: 2020 2020 7265 7472 795f 7374 6174 7573      retry_status
-0000c310: 203d 2030 0a20 2020 2020 2020 2077 6869   = 0.        whi
-0000c320: 6c65 2072 6574 7279 5f73 7461 7475 7320  le retry_status 
-0000c330: 3c20 333a 0a20 2020 2020 2020 2020 2020  < 3:.           
-0000c340: 2072 6573 756c 7420 3d20 7365 6c66 2e72   result = self.r
-0000c350: 756e 5f63 6f6d 6d61 6e64 7328 5b63 6d64  un_commands([cmd
-0000c360: 5d2c 2065 6e76 3d65 6e76 290a 2020 2020  ], env=env).    
-0000c370: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-0000c380: 6e66 6f28 7265 7375 6c74 290a 2020 2020  nfo(result).    
-0000c390: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-0000c3a0: 742e 6f6b 3a0a 2020 2020 2020 2020 2020  t.ok:.          
-0000c3b0: 2020 2020 2020 6966 206e 6f74 2072 6573        if not res
-0000c3c0: 756c 742e 7374 646f 7574 3a0a 2020 2020  ult.stdout:.    
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3e0: 2320 7761 6974 2066 6f72 2033 2073 6563  # wait for 3 sec
-0000c3f0: 6f6e 6473 2062 6566 6f72 6520 6368 6563  onds before chec
-0000c400: 6b69 6e67 2061 6761 696e 0a20 2020 2020  king again.     
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c420: 696d 6573 6c65 6570 2e73 6c65 6570 2833  imesleep.sleep(3
-0000c430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c440: 2020 2020 2020 2320 7265 7472 790a 2020        # retry.  
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 7265 7472 795f 7374 6174 7573 202b    retry_status +
-0000c470: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-0000c480: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000c490: 6562 7567 280a 2020 2020 2020 2020 2020  ebug(.          
-0000c4a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000c4b0: 5265 7472 7920 7b72 6574 7279 5f73 7461  Retry {retry_sta
-0000c4c0: 7475 737d 2067 6574 7469 6e67 2073 7461  tus} getting sta
-0000c4d0: 7475 7320 5c0a 2020 2020 2020 2020 2020  tus \.          
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2020 6f66 207b 736c 7572 6d5f 6a6f 625f    of {slurm_job_
-0000c500: 6964 737d 2122 290a 2020 2020 2020 2020  ids}!").        
-0000c510: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 2020 2320 0a20 2020 2020 2020 2020 2020    # .           
-0000c540: 2020 2020 2020 2020 206a 6f62 5f73 7461           job_sta
-0000c550: 7475 735f 6469 6374 203d 207b 696e 7428  tus_dict = {int(
-0000c560: 6c69 6e65 2e73 706c 6974 2829 5b30 5d2e  line.split()[0].
-0000c570: 7370 6c69 7428 275f 2729 5b30 5d29 3a20  split('_')[0]): 
-0000c580: 6c69 6e65 2e73 706c 6974 280a 2020 2020  line.split(.    
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5a0: 295b 315d 2066 6f72 206c 696e 6520 696e  )[1] for line in
-0000c5b0: 2072 6573 756c 742e 7374 646f 7574 2e73   result.stdout.s
-0000c5c0: 706c 6974 2822 5c6e 2229 2069 6620 6c69  plit("\n") if li
-0000c5d0: 6e65 7d0a 2020 2020 2020 2020 2020 2020  ne}.            
-0000c5e0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000c5f0: 6562 7567 2866 224a 6f62 2073 7461 7475  ebug(f"Job statu
-0000c600: 7365 733a 207b 6a6f 625f 7374 6174 7573  ses: {job_status
-0000c610: 5f64 6963 747d 2229 0a20 2020 2020 2020  _dict}").       
-0000c620: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000c630: 7572 6e20 6a6f 625f 7374 6174 7573 5f64  urn job_status_d
-0000c640: 6963 742c 2072 6573 756c 740a 2020 2020  ict, result.    
-0000c650: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000c660: 2020 2020 2020 2020 2020 2020 2020 6572                er
-0000c670: 726f 7220 3d20 6622 5265 7375 6c74 2069  ror = f"Result i
-0000c680: 7320 6e6f 7420 6f6b 3a20 7b72 6573 756c  s not ok: {resul
-0000c690: 747d 220a 2020 2020 2020 2020 2020 2020  t}".            
-0000c6a0: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
-0000c6b0: 2865 7272 6f72 290a 2020 2020 2020 2020  (error).        
-0000c6c0: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
-0000c6d0: 4845 7863 6570 7469 6f6e 2865 7272 6f72  HException(error
-0000c6e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000c6f0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-0000c700: 7220 3d20 6622 4572 726f 723a 2052 6574  r = f"Error: Ret
-0000c710: 7269 6564 207b 7265 7472 795f 7374 6174  ried {retry_stat
-0000c720: 7573 7d20 7469 6d65 7320 746f 2067 6574  us} times to get
-0000c730: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0000c740: 2020 2073 7461 7475 7320 6f66 207b 736c     status of {sl
-0000c750: 7572 6d5f 6a6f 625f 6964 737d 2c20 6275  urm_job_ids}, bu
-0000c760: 7420 6e6f 2072 6573 706f 6e73 652e 220a  t no response.".
-0000c770: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000c780: 6572 2e65 7272 6f72 2865 7272 6f72 290a  er.error(error).
-0000c790: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000c7a0: 6520 5353 4845 7863 6570 7469 6f6e 2865  e SSHException(e
-0000c7b0: 7272 6f72 290a 0a20 2020 2064 6566 2067  rror)..    def g
-0000c7c0: 6574 5f6a 6f62 5f73 7461 7475 735f 636f  et_job_status_co
-0000c7d0: 6d6d 616e 6428 7365 6c66 2c20 736c 7572  mmand(self, slur
-0000c7e0: 6d5f 6a6f 625f 6964 733a 204c 6973 745b  m_job_ids: List[
-0000c7f0: 696e 745d 2920 2d3e 2073 7472 3a0a 2020  int]) -> str:.  
-0000c800: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c810: 2020 5265 7475 726e 2074 6865 2053 6c75    Return the Slu
-0000c820: 726d 2063 6f6d 6d61 6e64 2074 6f20 6765  rm command to ge
-0000c830: 7420 7468 6520 7374 6174 7573 206f 6620  t the status of 
-0000c840: 6a6f 6273 2077 6974 6820 7468 6520 6769  jobs with the gi
-0000c850: 7665 6e0a 2020 2020 2020 2020 6a6f 6220  ven.        job 
-0000c860: 4944 732e 0a0a 2020 2020 2020 2020 4172  IDs...        Ar
-0000c870: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000c880: 736c 7572 6d5f 6a6f 625f 6964 7320 284c  slurm_job_ids (L
-0000c890: 6973 745b 696e 745d 293a 2054 6865 206a  ist[int]): The j
-0000c8a0: 6f62 2049 4473 206f 6620 7468 6520 6a6f  ob IDs of the jo
-0000c8b0: 6273 2074 6f20 6368 6563 6b2e 0a0a 2020  bs to check...  
-0000c8c0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000c8d0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
-0000c8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8f0: 2054 6865 2053 6c75 726d 2063 6f6d 6d61   The Slurm comma
-0000c900: 6e64 2074 6f20 6765 7420 7468 6520 7374  nd to get the st
-0000c910: 6174 7573 206f 6620 7468 6520 6a6f 6273  atus of the jobs
-0000c920: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000c930: 2020 2020 2020 2320 636f 6e63 6174 206d        # concat m
-0000c940: 756c 7469 706c 6520 6a6f 6273 2069 6620  ultiple jobs if 
-0000c950: 6e65 6564 6564 0a20 2020 2020 2020 2073  needed.        s
-0000c960: 6c75 726d 5f6a 6f62 5f69 6420 3d20 2220  lurm_job_id = " 
-0000c970: 2d6a 2022 2e6a 6f69 6e28 5b73 7472 2869  -j ".join([str(i
-0000c980: 6429 2066 6f72 2069 6420 696e 2073 6c75  d) for id in slu
-0000c990: 726d 5f6a 6f62 5f69 6473 5d29 0a20 2020  rm_job_ids]).   
-0000c9a0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c9b0: 2e5f 4a4f 425f 5354 4154 5553 5f43 4d44  ._JOB_STATUS_CMD
-0000c9c0: 2e66 6f72 6d61 7428 736c 7572 6d5f 6a6f  .format(slurm_jo
-0000c9d0: 625f 6964 3d73 6c75 726d 5f6a 6f62 5f69  b_id=slurm_job_i
-0000c9e0: 6429 0a0a 2020 2020 6465 6620 6578 7472  d)..    def extr
-0000c9f0: 6163 745f 6461 7461 5f6c 6f63 6174 696f  act_data_locatio
-0000ca00: 6e5f 6672 6f6d 5f6c 6f67 2873 656c 662c  n_from_log(self,
-0000ca10: 2073 6c75 726d 5f6a 6f62 5f69 643a 2073   slurm_job_id: s
-0000ca20: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
-0000ca60: 204e 6f6e 6529 202d 3e20 7374 723a 0a20   None) -> str:. 
-0000ca70: 2020 2020 2020 2022 2222 5265 6164 2053         """Read S
-0000ca80: 4c55 524d 206a 6f62 206c 6f67 6669 6c65  LURM job logfile
-0000ca90: 2074 6f20 6669 6e64 206c 6f63 6174 696f   to find locatio
-0000caa0: 6e20 6f66 2074 6865 2064 6174 612e 0a0a  n of the data...
-0000cab0: 2020 2020 2020 2020 4f6e 6520 6f66 2074          One of t
-0000cac0: 6865 2070 6172 616d 6574 6572 7320 6973  he parameters is
-0000cad0: 2072 6571 7569 7265 642c 2065 6974 6865   required, eithe
-0000cae0: 7220 6964 206f 7220 6669 6c65 2e0a 0a20  r id or file... 
-0000caf0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000cb00: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
-0000cb10: 6f62 5f69 6420 2873 7472 293a 2049 6420  ob_id (str): Id 
-0000cb20: 6f66 2074 6865 2073 6c75 726d 206a 6f62  of the slurm job
-0000cb30: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0000cb40: 6669 6c65 2028 7374 7229 3a20 5061 7468  file (str): Path
-0000cb50: 2074 6f20 7468 6520 6c6f 6766 696c 650a   to the logfile.
-0000cb60: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000cb70: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
-0000cb80: 723a 2044 6174 6120 6c6f 6361 7469 6f6e  r: Data location
-0000cb90: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
-0000cba0: 6520 6c6f 670a 0a20 2020 2020 2020 2052  e log..        R
-0000cbb0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-0000cbc0: 2020 2053 5348 4578 6365 7074 696f 6e3a     SSHException:
-0000cbd0: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
-0000cbe0: 6973 7375 6520 7769 7468 2074 6865 2063  issue with the c
-0000cbf0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
-0000cc00: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000cc10: 2020 2020 2020 6966 206c 6f67 6669 6c65        if logfile
-0000cc20: 2069 7320 4e6f 6e65 2061 6e64 2073 6c75   is None and slu
-0000cc30: 726d 5f6a 6f62 5f69 6420 6973 206e 6f74  rm_job_id is not
-0000cc40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000cc50: 2020 206c 6f67 6669 6c65 203d 2073 656c     logfile = sel
-0000cc60: 662e 5f4c 4f47 4649 4c45 0a20 2020 2020  f._LOGFILE.     
-0000cc70: 2020 2020 2020 206c 6f67 6669 6c65 203d         logfile =
-0000cc80: 206c 6f67 6669 6c65 2e66 6f72 6d61 7428   logfile.format(
-0000cc90: 736c 7572 6d5f 6a6f 625f 6964 3d73 6c75  slurm_job_id=slu
-0000cca0: 726d 5f6a 6f62 5f69 6429 0a20 2020 2020  rm_job_id).     
-0000ccb0: 2020 2063 6d64 203d 2073 656c 662e 5f4c     cmd = self._L
-0000ccc0: 4f47 4649 4c45 5f44 4154 415f 434d 442e  OGFILE_DATA_CMD.
-0000ccd0: 666f 726d 6174 286c 6f67 5f66 696c 653d  format(log_file=
-0000cce0: 6c6f 6766 696c 6529 0a20 2020 2020 2020  logfile).       
-0000ccf0: 2072 6573 756c 7420 3d20 7365 6c66 2e72   result = self.r
-0000cd00: 756e 5f63 6f6d 6d61 6e64 7328 5b63 6d64  un_commands([cmd
-0000cd10: 5d29 0a20 2020 2020 2020 2069 6620 7265  ]).        if re
-0000cd20: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
-0000cd30: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000cd40: 6c74 2e73 7464 6f75 740a 2020 2020 2020  lt.stdout.      
-0000cd50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cd60: 2020 2020 7261 6973 6520 5353 4845 7863      raise SSHExc
-0000cd70: 6570 7469 6f6e 2872 6573 756c 7429 0a0a  eption(result)..
-0000cd80: 2020 2020 6465 6620 6765 745f 776f 726b      def get_work
-0000cd90: 666c 6f77 5f70 6172 616d 6574 6572 7328  flow_parameters(
-0000cda0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2020 2020 776f 726b 666c 6f77 3a20        workflow: 
-0000cdd0: 7374 7229 202d 3e20 4469 6374 5b73 7472  str) -> Dict[str
-0000cde0: 2c20 4469 6374 5b73 7472 2c20 416e 795d  , Dict[str, Any]
-0000cdf0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0000ce00: 2020 2020 2020 2052 6574 7269 6576 6520         Retrieve 
-0000ce10: 7468 6520 7061 7261 6d65 7465 7273 206f  the parameters o
-0000ce20: 6620 6120 776f 726b 666c 6f77 2e0a 0a20  f a workflow... 
-0000ce30: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000ce40: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000ce50: 7720 2873 7472 293a 2054 6865 2077 6f72  w (str): The wor
-0000ce60: 6b66 6c6f 7720 666f 7220 7768 6963 6820  kflow for which 
-0000ce70: 746f 2072 6574 7269 6576 6520 7468 6520  to retrieve the 
-0000ce80: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
-0000ce90: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000cea0: 2020 2020 2020 2020 2020 4469 6374 5b73            Dict[s
-0000ceb0: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
-0000cec0: 795d 5d3a 0a20 2020 2020 2020 2020 2020  y]]:.           
-0000ced0: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
-0000cee0: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-0000cef0: 2077 6f72 6b66 6c6f 7720 7061 7261 6d65   workflow parame
-0000cf00: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
-0000cf10: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-0000cf20: 2020 2056 616c 7565 4572 726f 723a 2049     ValueError: I
-0000cf30: 6620 616e 2065 7272 6f72 206f 6363 7572  f an error occur
-0000cf40: 7320 7768 696c 6520 7265 7472 6965 7669  s while retrievi
-0000cf50: 6e67 2074 6865 2077 6f72 6b66 6c6f 770a  ng the workflow.
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
-0000cf80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000cf90: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
-0000cfa0: 3d20 7365 6c66 2e70 756c 6c5f 6465 7363  = self.pull_desc
-0000cfb0: 7269 7074 6f72 5f66 726f 6d5f 6769 7468  riptor_from_gith
-0000cfc0: 7562 2877 6f72 6b66 6c6f 7729 0a20 2020  ub(workflow).   
-0000cfd0: 2020 2020 2023 2063 6f6e 7665 7274 2074       # convert t
-0000cfe0: 6f20 6f6d 6572 6f20 7479 7065 730a 2020  o omero types.  
-0000cff0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000d000: 7567 286a 736f 6e5f 6465 7363 7269 7074  ug(json_descript
-0000d010: 6f72 290a 2020 2020 2020 2020 776f 726b  or).        work
-0000d020: 666c 6f77 5f64 6963 7420 3d20 7b7d 0a20  flow_dict = {}. 
-0000d030: 2020 2020 2020 2066 6f72 2069 6e70 7574         for input
-0000d040: 2069 6e20 6a73 6f6e 5f64 6573 6372 6970   in json_descrip
-0000d050: 746f 725b 2769 6e70 7574 7327 5d3a 0a20  tor['inputs']:. 
-0000d060: 2020 2020 2020 2020 2020 2023 2066 696c             # fil
-0000d070: 7465 7220 6379 746f 6d69 6e65 2070 6172  ter cytomine par
-0000d080: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000d090: 2020 2020 6966 206e 6f74 2069 6e70 7574      if not input
-0000d0a0: 5b27 6964 275d 2e73 7461 7274 7377 6974  ['id'].startswit
-0000d0b0: 6828 2763 7974 6f6d 696e 6527 293a 0a20  h('cytomine'):. 
-0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000d0d0: 6f72 6b66 6c6f 775f 7061 7261 6d73 203d  orkflow_params =
-0000d0e0: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-0000d0f0: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
-0000d100: 616d 735b 276e 616d 6527 5d20 3d20 696e  ams['name'] = in
-0000d110: 7075 745b 2769 6427 5d0a 2020 2020 2020  put['id'].      
-0000d120: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000d130: 6f77 5f70 6172 616d 735b 2764 6566 6175  ow_params['defau
-0000d140: 6c74 275d 203d 2069 6e70 7574 5b27 6465  lt'] = input['de
-0000d150: 6661 756c 742d 7661 6c75 6527 5d0a 2020  fault-value'].  
-0000d160: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0000d170: 726b 666c 6f77 5f70 6172 616d 735b 2763  rkflow_params['c
-0000d180: 7974 7970 6527 5d20 3d20 696e 7075 745b  ytype'] = input[
-0000d190: 2774 7970 6527 5d0a 2020 2020 2020 2020  'type'].        
-0000d1a0: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000d1b0: 5f70 6172 616d 735b 276f 7074 696f 6e61  _params['optiona
-0000d1c0: 6c27 5d20 3d20 696e 7075 745b 276f 7074  l'] = input['opt
-0000d1d0: 696f 6e61 6c27 5d0a 2020 2020 2020 2020  ional'].        
-0000d1e0: 2020 2020 2020 2020 636d 645f 666c 6167          cmd_flag
-0000d1f0: 203d 2069 6e70 7574 5b27 636f 6d6d 616e   = input['comman
-0000d200: 642d 6c69 6e65 2d66 6c61 6727 5d0a 2020  d-line-flag'].  
-0000d210: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000d220: 645f 666c 6167 203d 2063 6d64 5f66 6c61  d_flag = cmd_fla
-0000d230: 672e 7265 706c 6163 6528 2240 6964 222c  g.replace("@id",
-0000d240: 2069 6e70 7574 5b27 6964 275d 290a 2020   input['id']).  
-0000d250: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0000d260: 726b 666c 6f77 5f70 6172 616d 735b 2763  rkflow_params['c
-0000d270: 6d64 5f66 6c61 6727 5d20 3d20 636d 645f  md_flag'] = cmd_
-0000d280: 666c 6167 0a20 2020 2020 2020 2020 2020  flag.           
-0000d290: 2020 2020 2077 6f72 6b66 6c6f 775f 7061       workflow_pa
-0000d2a0: 7261 6d73 5b27 6465 7363 7269 7074 696f  rams['descriptio
-0000d2b0: 6e27 5d20 3d20 696e 7075 745b 2764 6573  n'] = input['des
-0000d2c0: 6372 6970 7469 6f6e 275d 0a20 2020 2020  cription'].     
-0000d2d0: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000d2e0: 6c6f 775f 6469 6374 5b69 6e70 7574 5b27  low_dict[input['
-0000d2f0: 6964 275d 5d20 3d20 776f 726b 666c 6f77  id']] = workflow
-0000d300: 5f70 6172 616d 730a 2020 2020 2020 2020  _params.        
-0000d310: 7265 7475 726e 2077 6f72 6b66 6c6f 775f  return workflow_
-0000d320: 6469 6374 0a0a 2020 2020 6465 6620 636f  dict..    def co
-0000d330: 6e76 6572 745f 6379 7479 7065 5f74 6f5f  nvert_cytype_to_
-0000d340: 6f6d 7479 7065 2873 656c 662c 0a20 2020  omtype(self,.   
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2020 2020 2020 2020 2020 2020 2020 6379                cy
-0000d370: 7479 7065 3a20 7374 722c 205f 6465 6661  type: str, _defa
-0000d380: 756c 742c 202a 6172 6773 2c20 2a2a 6b77  ult, *args, **kw
-0000d390: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3b0: 2020 2020 2020 2920 2d3e 2041 6e79 3a0a        ) -> Any:.
-0000d3c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d3d0: 2020 2020 436f 6e76 6572 7420 6120 4379      Convert a Cy
-0000d3e0: 746f 6d69 6e65 2074 7970 6520 746f 2061  tomine type to a
-0000d3f0: 6e20 4f4d 4552 4f20 7479 7065 2061 6e64  n OMERO type and
-0000d400: 2069 6e73 7461 6e74 6961 7465 7320 6974   instantiates it
-0000d410: 0a20 2020 2020 2020 2077 6974 6820 6172  .        with ar
-0000d420: 6773 2f6b 7761 7267 732e 0a0a 2020 2020  gs/kwargs...    
-0000d430: 2020 2020 4e6f 7465 2074 6861 7420 4379      Note that Cy
-0000d440: 746f 6d69 6e65 2068 6173 2061 2050 7974  tomine has a Pyt
-0000d450: 686f 6e20 436c 6965 6e74 2c20 616e 6420  hon Client, and 
-0000d460: 736f 6d65 2063 6f6e 7665 7273 696f 6e20  some conversion 
-0000d470: 6d65 7468 6f64 730a 2020 2020 2020 2020  methods.        
-0000d480: 746f 2070 7974 686f 6e20 7479 7065 732c  to python types,
-0000d490: 2062 7574 206e 6f74 6869 6e67 2070 6172   but nothing par
-0000d4a0: 7469 6375 6c61 726c 7920 776f 7274 6820  ticularly worth 
-0000d4b0: 6465 7065 6e64 696e 6720 6f6e 2074 6861  depending on tha
-0000d4c0: 740a 2020 2020 2020 2020 6c69 6272 6172  t.        librar
-0000d4d0: 7920 666f 7220 7965 742e 204d 6967 6874  y for yet. Might
-0000d4e0: 2062 6520 7573 6566 756c 2069 6e20 7468   be useful in th
-0000d4f0: 6520 6675 7475 7265 2070 6572 6861 7073  e future perhaps
-0000d500: 2e0a 2020 2020 2020 2020 2865 2e67 2e20  ..        (e.g. 
-0000d510: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000d520: 6f6d 2f43 7974 6f6d 696e 652d 554c 6965  om/Cytomine-ULie
-0000d530: 6765 2f43 7974 6f6d 696e 652d 7079 7468  ge/Cytomine-pyth
-0000d540: 6f6e 2d63 6c69 656e 742f 0a20 2020 2020  on-client/.     
-0000d550: 2020 2062 6c6f 622f 6d61 7374 6572 2f63     blob/master/c
-0000d560: 7974 6f6d 696e 652f 6379 746f 6d69 6e65  ytomine/cytomine
-0000d570: 5f6a 6f62 2e70 7929 0a0a 2020 2020 2020  _job.py)..      
-0000d580: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000d590: 2020 2020 6379 7479 7065 2028 7374 7229      cytype (str)
-0000d5a0: 3a20 5468 6520 4379 746f 6d69 6e65 2074  : The Cytomine t
-0000d5b0: 7970 6520 746f 2063 6f6e 7665 7274 2e0a  ype to convert..
-0000d5c0: 2020 2020 2020 2020 2020 2020 5f64 6566              _def
-0000d5d0: 6175 6c74 3a20 5468 6520 6465 6661 756c  ault: The defaul
-0000d5e0: 7420 7661 6c75 652e 2052 6571 7569 7265  t value. Require
-0000d5f0: 6420 746f 2064 6973 7469 6e67 7569 7368  d to distinguish
-0000d600: 2062 6574 7765 656e 2066 6c6f 6174 0a20   between float. 
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000d620: 6e64 2069 6e74 2e0a 2020 2020 2020 2020  nd int..        
-0000d630: 2020 2020 2a61 7267 733a 2041 6464 6974      *args: Addit
-0000d640: 696f 6e61 6c20 706f 7369 7469 6f6e 616c  ional positional
-0000d650: 2061 7267 756d 656e 7473 2e0a 2020 2020   arguments..    
-0000d660: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-0000d670: 3a20 4164 6469 7469 6f6e 616c 206b 6579  : Additional key
-0000d680: 776f 7264 2061 7267 756d 656e 7473 2e0a  word arguments..
-0000d690: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000d6a0: 3a0a 2020 2020 2020 2020 2020 2020 416e  :.            An
-0000d6b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000d6c0: 2020 2054 6865 2063 6f6e 7665 7274 6564     The converted
-0000d6d0: 204f 4d45 524f 2074 7970 6520 636c 6173   OMERO type clas
-0000d6e0: 7320 696e 7374 616e 6365 0a20 2020 2020  s instance.     
-0000d6f0: 2020 2020 2020 2020 2020 206f 7220 4e6f             or No
-0000d700: 6e65 2069 6620 6572 726f 7273 206f 6363  ne if errors occ
-0000d710: 7572 6564 2e0a 0a20 2020 2020 2020 2022  ured...        "
-0000d720: 2222 0a20 2020 2020 2020 2023 2054 4f44  "".        # TOD
-0000d730: 4f20 6d61 6b65 2045 6e75 6d20 3f0a 2020  O make Enum ?.  
-0000d740: 2020 2020 2020 6966 2063 7974 7970 6520        if cytype 
-0000d750: 3d3d 2027 4e75 6d62 6572 273a 0a20 2020  == 'Number':.   
-0000d760: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000d770: 7374 616e 6365 285f 6465 6661 756c 742c  stance(_default,
-0000d780: 2066 6c6f 6174 293a 0a20 2020 2020 2020   float):.       
-0000d790: 2020 2020 2020 2020 2023 2066 6c6f 6174           # float
-0000d7a0: 2069 6e73 7465 6164 0a20 2020 2020 2020   instead.       
-0000d7b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000d7c0: 7365 6c66 2e73 7472 5f74 6f5f 636c 6173  self.str_to_clas
-0000d7d0: 7328 226f 6d65 726f 2e73 6372 6970 7473  s("omero.scripts
-0000d7e0: 222c 2022 466c 6f61 7422 2c0a 2020 2020  ", "Float",.    
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2020 2020 202a 6172 6773 2c20 2a2a 6b77       *args, **kw
-0000d820: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
-0000d830: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000d840: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d850: 656c 662e 7374 725f 746f 5f63 6c61 7373  elf.str_to_class
-0000d860: 2822 6f6d 6572 6f2e 7363 7269 7074 7322  ("omero.scripts"
-0000d870: 2c20 2249 6e74 222c 0a20 2020 2020 2020  , "Int",.       
-0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 2a61 7267 732c 202a 2a6b 7761 7267    *args, **kwarg
-0000d8b0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
-0000d8c0: 6379 7479 7065 203d 3d20 2742 6f6f 6c65  cytype == 'Boole
-0000d8d0: 616e 273a 0a20 2020 2020 2020 2020 2020  an':.           
-0000d8e0: 2072 6574 7572 6e20 7365 6c66 2e73 7472   return self.str
-0000d8f0: 5f74 6f5f 636c 6173 7328 226f 6d65 726f  _to_class("omero
-0000d900: 2e73 6372 6970 7473 222c 2022 426f 6f6c  .scripts", "Bool
-0000d910: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d930: 2020 2020 2020 2020 2a61 7267 732c 202a          *args, *
-0000d940: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-0000d950: 2065 6c69 6620 6379 7479 7065 203d 3d20   elif cytype == 
-0000d960: 2753 7472 696e 6727 3a0a 2020 2020 2020  'String':.      
-0000d970: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d980: 662e 7374 725f 746f 5f63 6c61 7373 2822  f.str_to_class("
-0000d990: 6f6d 6572 6f2e 7363 7269 7074 7322 2c20  omero.scripts", 
-0000d9a0: 2253 7472 696e 6722 2c0a 2020 2020 2020  "String",.      
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000d9d0: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-0000d9e0: 0a20 2020 2064 6566 2065 7874 7261 6374  .    def extract
-0000d9f0: 5f70 6172 7473 5f66 726f 6d5f 7572 6c28  _parts_from_url(
-0000da00: 7365 6c66 2c20 696e 7075 745f 7572 6c3a  self, input_url:
-0000da10: 2073 7472 2920 2d3e 2054 7570 6c65 5b4c   str) -> Tuple[L
-0000da20: 6973 745b 7374 725d 2c20 7374 725d 3a0a  ist[str], str]:.
-0000da30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000da40: 2020 2020 4578 7472 6163 7420 7468 6520      Extract the 
-0000da50: 7265 706f 7369 746f 7279 2061 6e64 2062  repository and b
-0000da60: 7261 6e63 6820 696e 666f 726d 6174 696f  ranch informatio
-0000da70: 6e20 6672 6f6d 2074 6865 2069 6e70 7574  n from the input
-0000da80: 2055 524c 2e0a 0a20 2020 2020 2020 2041   URL...        A
-0000da90: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000daa0: 2069 6e70 7574 5f75 726c 2028 7374 7229   input_url (str)
-0000dab0: 3a20 5468 6520 696e 7075 7420 4769 7448  : The input GitH
-0000dac0: 7562 2055 524c 2e0a 0a20 2020 2020 2020  ub URL...       
-0000dad0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000dae0: 2020 2020 2020 5475 706c 655b 4c69 7374        Tuple[List
-0000daf0: 5b73 7472 5d2c 2073 7472 5d3a 0a20 2020  [str], str]:.   
-0000db00: 2020 2020 2020 2020 2020 2020 2054 6865               The
-0000db10: 206c 6973 7420 6f66 2075 726c 2070 6172   list of url par
-0000db20: 7473 2061 6e64 2074 6865 2062 7261 6e63  ts and the branc
-0000db30: 682f 7665 7273 696f 6e2e 0a20 2020 2020  h/version..     
-0000db40: 2020 2020 2020 2020 2020 2049 6620 6e6f             If no
-0000db50: 2062 7261 6e63 6820 6973 2066 6f75 6e64   branch is found
-0000db60: 2c20 6974 2077 696c 6c20 7265 7475 726e  , it will return
-0000db70: 2022 6d61 7374 6572 220a 0a20 2020 2020   "master"..     
-0000db80: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-0000db90: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
-0000dba0: 723a 2049 6620 7468 6520 696e 7075 7420  r: If the input 
-0000dbb0: 5552 4c20 6973 206e 6f74 2061 2076 616c  URL is not a val
-0000dbc0: 6964 2047 6974 4875 6220 5552 4c2e 0a20  id GitHub URL.. 
-0000dbd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000dbe0: 2020 2075 726c 5f70 6172 7473 203d 2069     url_parts = i
-0000dbf0: 6e70 7574 5f75 726c 2e73 706c 6974 2822  nput_url.split("
-0000dc00: 2f22 290a 2020 2020 2020 2020 6966 206c  /").        if l
-0000dc10: 656e 2875 726c 5f70 6172 7473 2920 3c20  en(url_parts) < 
-0000dc20: 3520 6f72 2075 726c 5f70 6172 7473 5b32  5 or url_parts[2
-0000dc30: 5d20 213d 2022 6769 7468 7562 2e63 6f6d  ] != "github.com
-0000dc40: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
-0000dc50: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000dc60: 2249 6e76 616c 6964 2047 6974 4875 6220  "Invalid GitHub 
-0000dc70: 5552 4c22 290a 0a20 2020 2020 2020 2069  URL")..        i
-0000dc80: 6620 2274 7265 6522 2069 6e20 7572 6c5f  f "tree" in url_
-0000dc90: 7061 7274 733a 0a20 2020 2020 2020 2020  parts:.         
-0000dca0: 2020 2023 2043 6173 653a 2055 524c 2063     # Case: URL c
-0000dcb0: 6f6e 7461 696e 7320 6120 6272 616e 6368  ontains a branch
-0000dcc0: 0a20 2020 2020 2020 2020 2020 2062 7261  .            bra
-0000dcd0: 6e63 685f 696e 6465 7820 3d20 7572 6c5f  nch_index = url_
-0000dce0: 7061 7274 732e 696e 6465 7828 2274 7265  parts.index("tre
-0000dcf0: 6522 2920 2b20 310a 2020 2020 2020 2020  e") + 1.        
-0000dd00: 2020 2020 6272 616e 6368 203d 2075 726c      branch = url
-0000dd10: 5f70 6172 7473 5b62 7261 6e63 685f 696e  _parts[branch_in
-0000dd20: 6465 785d 0a20 2020 2020 2020 2065 6c73  dex].        els
-0000dd30: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000dd40: 2043 6173 653a 2055 524c 2064 6f65 7320   Case: URL does 
-0000dd50: 6e6f 7420 7370 6563 6966 7920 6120 6272  not specify a br
-0000dd60: 616e 6368 0a20 2020 2020 2020 2020 2020  anch.           
-0000dd70: 2062 7261 6e63 6820 3d20 226d 6173 7465   branch = "maste
-0000dd80: 7222 0a0a 2020 2020 2020 2020 7265 7475  r"..        retu
-0000dd90: 726e 2075 726c 5f70 6172 7473 2c20 6272  rn url_parts, br
-0000dda0: 616e 6368 0a0a 2020 2020 6465 6620 636f  anch..    def co
-0000ddb0: 6e76 6572 745f 7572 6c28 7365 6c66 2c20  nvert_url(self, 
-0000ddc0: 696e 7075 745f 7572 6c3a 2073 7472 2920  input_url: str) 
-0000ddd0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0000dde0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
-0000ddf0: 6572 7420 7468 6520 696e 7075 7420 4769  ert the input Gi
-0000de00: 7448 7562 2055 524c 2074 6f20 616e 206f  tHub URL to an o
-0000de10: 7574 7075 7420 5552 4c20 7468 6174 2072  utput URL that r
-0000de20: 6574 7269 6576 6573 0a20 2020 2020 2020  etrieves.       
-0000de30: 2074 6865 2027 6465 7363 7269 7074 6f72   the 'descriptor
-0000de40: 2e6a 736f 6e27 2066 696c 6520 696e 2072  .json' file in r
-0000de50: 6177 2066 6f72 6d61 742e 0a0a 2020 2020  aw format...    
-0000de60: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000de70: 2020 2020 2020 696e 7075 745f 7572 6c20        input_url 
-0000de80: 2873 7472 293a 2054 6865 2069 6e70 7574  (str): The input
-0000de90: 2047 6974 4875 6220 5552 4c2e 0a0a 2020   GitHub URL...  
-0000dea0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000deb0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
-0000dec0: 5468 6520 6f75 7470 7574 2055 524c 2074  The output URL t
-0000ded0: 6f20 7468 6520 2764 6573 6372 6970 746f  o the 'descripto
-0000dee0: 722e 6a73 6f6e 2720 6669 6c65 2e0a 0a20  r.json' file... 
-0000def0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-0000df00: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-0000df10: 4572 726f 723a 2049 6620 7468 6520 696e  Error: If the in
-0000df20: 7075 7420 5552 4c20 6973 206e 6f74 2061  put URL is not a
-0000df30: 2076 616c 6964 2047 6974 4875 6220 5552   valid GitHub UR
-0000df40: 4c2e 0a20 2020 2020 2020 2022 2222 0a20  L..        """. 
-0000df50: 2020 2020 2020 2075 726c 5f70 6172 7473         url_parts
-0000df60: 2c20 6272 616e 6368 203d 2073 656c 662e  , branch = self.
-0000df70: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
-0000df80: 6f6d 5f75 726c 2869 6e70 7574 5f75 726c  om_url(input_url
-0000df90: 290a 0a20 2020 2020 2020 2023 2043 6f6e  )..        # Con
-0000dfa0: 7374 7275 6374 2074 6865 206f 7574 7075  struct the outpu
-0000dfb0: 7420 5552 4c20 6279 2063 6f6d 6269 6e69  t URL by combini
-0000dfc0: 6e67 2074 6865 2065 7874 7261 6374 6564  ng the extracted
-0000dfd0: 2069 6e66 6f72 6d61 7469 6f6e 0a20 2020   information.   
-0000dfe0: 2020 2020 2023 2077 6974 6820 7468 6520       # with the 
-0000dff0: 6465 7369 7265 6420 6669 6c65 2070 6174  desired file pat
-0000e000: 680a 2020 2020 2020 2020 6f75 7470 7574  h.        output
-0000e010: 5f75 726c 203d 2066 2268 7474 7073 3a2f  _url = f"https:/
-0000e020: 2f67 6974 6875 622e 636f 6d2f 7b75 726c  /github.com/{url
-0000e030: 5f70 6172 7473 5b33 5d7d 2f7b 7572 6c5f  _parts[3]}/{url_
-0000e040: 7061 7274 735b 345d 7d2f 7261 772f 7b62  parts[4]}/raw/{b
-0000e050: 7261 6e63 687d 2f64 6573 6372 6970 746f  ranch}/descripto
-0000e060: 722e 6a73 6f6e 220a 0a20 2020 2020 2020  r.json"..       
-0000e070: 2072 6574 7572 6e20 6f75 7470 7574 5f75   return output_u
-0000e080: 726c 0a0a 2020 2020 6465 6620 7075 6c6c  rl..    def pull
-0000e090: 5f64 6573 6372 6970 746f 725f 6672 6f6d  _descriptor_from
-0000e0a0: 5f67 6974 6875 6228 7365 6c66 2c20 776f  _github(self, wo
-0000e0b0: 726b 666c 6f77 3a20 7374 7229 202d 3e20  rkflow: str) -> 
-0000e0c0: 4469 6374 3a0a 2020 2020 2020 2020 2222  Dict:.        ""
-0000e0d0: 220a 2020 2020 2020 2020 5075 6c6c 2074  ".        Pull t
-0000e0e0: 6865 2077 6f72 6b66 6c6f 7720 6465 7363  he workflow desc
-0000e0f0: 7269 7074 6f72 2066 726f 6d20 4769 7448  riptor from GitH
-0000e100: 7562 2e0a 0a20 2020 2020 2020 2041 7267  ub...        Arg
-0000e110: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
-0000e120: 6f72 6b66 6c6f 7720 2873 7472 293a 2054  orkflow (str): T
-0000e130: 6865 2077 6f72 6b66 6c6f 7720 666f 7220  he workflow for 
-0000e140: 7768 6963 6820 746f 2070 756c 6c20 7468  which to pull th
-0000e150: 6520 6465 7363 7269 7074 6f72 2e0a 0a20  e descriptor... 
-0000e160: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000e170: 2020 2020 2020 2020 2020 2020 4469 6374              Dict
-0000e180: 3a20 5468 6520 4a53 4f4e 2064 6573 6372  : The JSON descr
-0000e190: 6970 746f 722e 0a0a 2020 2020 2020 2020  iptor...        
-0000e1a0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-0000e1b0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-0000e1c0: 4966 2061 6e20 6572 726f 7220 6f63 6375  If an error occu
-0000e1d0: 7273 2077 6869 6c65 2070 756c 6c69 6e67  rs while pulling
-0000e1e0: 2074 6865 2064 6573 6372 6970 746f 7220   the descriptor 
-0000e1f0: 6669 6c65 2e0a 2020 2020 2020 2020 2222  file..        ""
-0000e200: 220a 2020 2020 2020 2020 6769 745f 7265  ".        git_re
-0000e210: 706f 203d 2073 656c 662e 736c 7572 6d5f  po = self.slurm_
-0000e220: 6d6f 6465 6c5f 7265 706f 735b 776f 726b  model_repos[work
-0000e230: 666c 6f77 5d0a 2020 2020 2020 2020 2320  flow].        # 
-0000e240: 636f 6e76 6572 7420 6769 7420 7265 706f  convert git repo
-0000e250: 2074 6f20 6a73 6f6e 2066 696c 650a 2020   to json file.  
-0000e260: 2020 2020 2020 7261 775f 7572 6c20 3d20        raw_url = 
-0000e270: 7365 6c66 2e63 6f6e 7665 7274 5f75 726c  self.convert_url
-0000e280: 2867 6974 5f72 6570 6f29 0a20 2020 2020  (git_repo).     
-0000e290: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e2a0: 6622 5075 6c6c 2077 6f72 6b66 6c6f 773a  f"Pull workflow:
-0000e2b0: 207b 776f 726b 666c 6f77 7d3a 207b 6769   {workflow}: {gi
-0000e2c0: 745f 7265 706f 7d20 3e3e 207b 7261 775f  t_repo} >> {raw_
-0000e2d0: 7572 6c7d 2229 0a20 2020 2020 2020 2023  url}").        #
-0000e2e0: 2070 756c 6c20 776f 726b 666c 6f77 2070   pull workflow p
-0000e2f0: 6172 616d 730a 2020 2020 2020 2020 6769  arams.        gi
-0000e300: 7468 7562 5f73 6573 7369 6f6e 203d 2073  thub_session = s
-0000e310: 656c 662e 6765 745f 6f72 5f63 7265 6174  elf.get_or_creat
-0000e320: 655f 6769 7468 7562 5f73 6573 7369 6f6e  e_github_session
-0000e330: 2829 0a20 2020 2020 2020 2067 6866 696c  ().        ghfil
-0000e340: 6520 3d20 6769 7468 7562 5f73 6573 7369  e = github_sessi
-0000e350: 6f6e 2e67 6574 2872 6177 5f75 726c 290a  on.get(raw_url).
-0000e360: 2020 2020 2020 2020 6966 2067 6866 696c          if ghfil
-0000e370: 652e 6f6b 3a0a 2020 2020 2020 2020 2020  e.ok:.          
-0000e380: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-0000e390: 2243 6163 6865 643f 207b 6768 6669 6c65  "Cached? {ghfile
-0000e3a0: 2e66 726f 6d5f 6361 6368 657d 2229 0a20  .from_cache}"). 
-0000e3b0: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-0000e3c0: 6465 7363 7269 7074 6f72 203d 2067 6866  descriptor = ghf
-0000e3d0: 696c 652e 6a73 6f6e 2829 0a20 2020 2020  ile.json().     
-0000e3e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e3f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000e400: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0000e410: 2020 2020 2020 2066 2745 7272 6f72 2077         f'Error w
-0000e420: 6869 6c65 2070 756c 6c69 6e67 2064 6573  hile pulling des
-0000e430: 6372 6970 746f 7220 6669 6c65 2066 6f72  criptor file for
-0000e440: 2077 6f72 6b66 6c6f 7720 7b77 6f72 6b66   workflow {workf
-0000e450: 6c6f 777d 2c5c 0a20 2020 2020 2020 2020  low},\.         
-0000e460: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-0000e470: 7b72 6177 5f75 726c 7d3a 207b 6768 6669  {raw_url}: {ghfi
-0000e480: 6c65 2e5f 5f64 6963 745f 5f7d 2729 0a20  le.__dict__}'). 
-0000e490: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
-0000e4a0: 6f6e 5f64 6573 6372 6970 746f 720a 0a20  on_descriptor.. 
-0000e4b0: 2020 2064 6566 2067 6574 5f6f 725f 6372     def get_or_cr
-0000e4c0: 6561 7465 5f67 6974 6875 625f 7365 7373  eate_github_sess
-0000e4d0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
-0000e4e0: 2020 2023 204e 6f74 652c 2075 7369 6e67     # Note, using
-0000e4f0: 2072 6571 7565 7374 735f 6361 6368 6520   requests_cache 
-0000e500: 312e 312e 312c 2063 6f6e 6469 7469 6f6e  1.1.1, condition
-0000e510: 616c 2071 7565 7269 6573 2061 7265 2064  al queries are d
-0000e520: 6566 6175 6c74 3a0a 2020 2020 2020 2020  efault:.        
-0000e530: 2320 5468 6520 6361 6368 6564 2072 6573  # The cached res
-0000e540: 706f 6e73 6520 7769 6c6c 2073 7469 6c6c  ponse will still
-0000e550: 2062 6520 7573 6564 2075 6e74 696c 2074   be used until t
-0000e560: 6865 2072 656d 6f74 6520 636f 6e74 656e  he remote conten
-0000e570: 7420 6163 7475 616c 6c79 2063 6861 6e67  t actually chang
-0000e580: 6573 0a20 2020 2020 2020 2023 2045 7665  es.        # Eve
-0000e590: 6e20 6966 2074 6865 2027 6578 7069 7265  n if the 'expire
-0000e5a0: 5f61 6674 6572 2720 6973 2074 7269 6767  _after' is trigg
-0000e5b0: 6572 6564 2e20 5468 6973 2069 7320 6275  ered. This is bu
-0000e5c0: 696c 7420 696e 746f 2047 6974 4875 622c  ilt into GitHub,
-0000e5d0: 2077 6869 6368 2072 6574 7572 6e73 0a20   which returns. 
-0000e5e0: 2020 2020 2020 2023 2061 2045 7461 6720         # a Etag 
-0000e5f0: 696e 2074 6865 2068 6561 6465 7220 7468  in the header th
-0000e600: 6174 206f 6e6c 7920 6368 616e 6765 7320  at only changes 
-0000e610: 7768 656e 2074 6865 2063 6f6e 7465 6e74  when the content
-0000e620: 2028 652e 672e 2074 6865 2064 6573 6372   (e.g. the descr
-0000e630: 6970 746f 7229 2063 6861 6e67 6573 2e0a  iptor) changes..
-0000e640: 2020 2020 2020 2020 2320 4966 2079 6f75          # If you
-0000e650: 2070 726f 7669 6465 2074 6869 7320 4574   provide this Et
-0000e660: 6167 2077 6865 6e20 7175 6572 7969 6e67  ag when querying
-0000e670: 2c20 796f 7520 7769 6c6c 2067 6574 2061  , you will get a
-0000e680: 2033 3034 2028 276e 6f20 6368 616e 6765   304 ('no change
-0000e690: 2729 2061 6e64 2069 7420 7769 6c6c 0a20  ') and it will. 
-0000e6a0: 2020 2020 2020 2023 204e 4f54 2063 6f75         # NOT cou
-0000e6b0: 6e74 2074 6f77 6172 6473 2079 6f75 7220  nt towards your 
-0000e6c0: 4769 7468 7562 206c 696d 6974 732e 2041  Github limits. A
-0000e6d0: 6e64 2072 6571 7565 7374 735f 6361 6368  nd requests_cach
-0000e6e0: 6520 646f 6573 2074 6861 7420 666f 7220  e does that for 
-0000e6f0: 7573 206e 6f77 2e0a 2020 2020 2020 2020  us now..        
-0000e700: 2320 4e6f 7420 6176 6169 6c61 626c 6520  # Not available 
-0000e710: 696e 2050 7974 686f 6e33 2e36 2074 686f  in Python3.6 tho
-0000e720: 7567 682e 0a20 2020 2020 2020 2073 203d  ugh..        s =
-0000e730: 2072 6571 7565 7374 735f 6361 6368 652e   requests_cache.
-0000e740: 4361 6368 6564 5365 7373 696f 6e28 2767  CachedSession('g
-0000e750: 6974 6875 625f 6361 6368 6527 2c0a 2020  ithub_cache',.  
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 2020 2020 2020 2062 6163 6b65 6e64 3d73         backend=s
-0000e790: 656c 662e 6361 6368 652c 0a20 2020 2020  elf.cache,.     
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 6578 7069 7265 5f61 6674 6572      expire_after
-0000e7d0: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7f0: 2020 2020 2020 2020 2020 2020 2063 6163               cac
-0000e800: 6865 5f63 6f6e 7472 6f6c 3d54 7275 650a  he_control=True.
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e840: 2020 2023 204d 6967 6874 2068 6176 6520     # Might have 
-0000e850: 6269 6767 6572 2069 7373 7565 732c 2074  bigger issues, t
-0000e860: 6869 7320 6973 2072 656c 6174 6564 2074  his is related t
-0000e870: 6f20 7261 7465 206c 696d 6974 7320 6f6e  o rate limits on
-0000e880: 2047 6974 4875 620a 2020 2020 2020 2020   GitHub.        
-0000e890: 2320 6874 7470 733a 2f2f 646f 6373 2e67  # https://docs.g
-0000e8a0: 6974 6875 622e 636f 6d2f 656e 2f72 6573  ithub.com/en/res
-0000e8b0: 742f 7573 696e 672d 7468 652d 7265 7374  t/using-the-rest
-0000e8c0: 2d61 7069 2f72 6174 652d 6c69 6d69 7473  -api/rate-limits
-0000e8d0: 2d66 6f72 2d74 6865 2d72 6573 742d 6170  -for-the-rest-ap
-0000e8e0: 690a 2020 2020 2020 2020 2320 4966 2069  i.        # If i
-0000e8f0: 7420 7374 6179 7320 6120 7072 6f62 6c65  t stays a proble
-0000e900: 6d2c 2077 6520 6861 7665 2074 6f20 6164  m, we have to ad
-0000e910: 6420 616e 206f 7074 696f 6e20 746f 2061  d an option to a
-0000e920: 6464 2061 2047 4820 6b65 7920 746f 2074  dd a GH key to t
-0000e930: 6865 2063 6f6e 6669 670a 2020 2020 2020  he config.      
-0000e940: 2020 2320 452e 672e 2073 6565 2068 7474    # E.g. see htt
-0000e950: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000e960: 7265 7175 6573 7473 2d63 6163 6865 2f72  requests-cache/r
-0000e970: 6571 7565 7374 732d 6361 6368 652f 626c  equests-cache/bl
-0000e980: 6f62 2f35 3331 3334 6566 3065 3939 6437  ob/53134ef0e99d7
-0000e990: 3133 6665 6436 3235 3135 6466 6237 6263  13fed62515dfb7bc
-0000e9a0: 6661 6163 3566 3633 6639 642f 6578 616d  faac5f63f9d/exam
-0000e9b0: 706c 6573 2f70 7967 6974 6875 622e 7079  ples/pygithub.py
-0000e9c0: 0a20 2020 2020 2020 2023 2048 6572 6520  .        # Here 
-0000e9d0: 796f 7520 636f 756c 6420 6861 7665 2061  you could have a
-0000e9e0: 6e20 4143 4345 5353 5f54 4f4b 454e 2e0a  n ACCESS_TOKEN..
-0000e9f0: 2020 2020 2020 2020 2320 416e 2041 4343          # An ACC
-0000ea00: 4553 535f 544f 4b45 4e20 636f 756c 6420  ESS_TOKEN could 
-0000ea10: 696d 7072 6f76 6520 6170 6920 6c69 6d69  improve api limi
-0000ea20: 7473 2074 6f20 3530 3030 2f68 2028 6672  ts to 5000/h (fr
-0000ea30: 6f6d 2036 302f 6829 2e0a 2020 2020 2020  om 60/h)..      
-0000ea40: 2020 7265 7472 795f 7374 7261 7465 6779    retry_strategy
-0000ea50: 203d 2052 6574 7279 280a 2020 2020 2020   = Retry(.      
-0000ea60: 2020 2020 2020 746f 7461 6c3d 352c 2020        total=5,  
-0000ea70: 2020 2020 2020 2020 2020 2020 2023 204d               # M
-0000ea80: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-0000ea90: 2072 6574 7269 6573 0a20 2020 2020 2020   retries.       
-0000eaa0: 2020 2020 2023 2045 7870 6f6e 656e 7469       # Exponenti
-0000eab0: 616c 2062 6163 6b6f 6666 2066 6163 746f  al backoff facto
-0000eac0: 7220 2864 656c 6179 2062 6574 7765 656e  r (delay between
-0000ead0: 2072 6574 7269 6573 290a 2020 2020 2020   retries).      
-0000eae0: 2020 2020 2020 6261 636b 6f66 665f 6661        backoff_fa
-0000eaf0: 6374 6f72 3d35 2c0a 2020 2020 2020 2020  ctor=5,.        
-0000eb00: 2020 2020 2320 5265 7472 7920 6f6e 2074      # Retry on t
-0000eb10: 6865 7365 2048 5454 5020 7374 6174 7573  hese HTTP status
-0000eb20: 2063 6f64 6573 0a20 2020 2020 2020 2020   codes.         
-0000eb30: 2020 2073 7461 7475 735f 666f 7263 656c     status_forcel
-0000eb40: 6973 743d 5b35 3030 2c20 3530 322c 2035  ist=[500, 502, 5
-0000eb50: 3033 2c20 3530 342c 2034 3033 2c20 3432  03, 504, 403, 42
-0000eb60: 395d 2c0a 2020 2020 2020 2020 2020 2020  9],.            
-0000eb70: 616c 6c6f 7765 645f 6d65 7468 6f64 733d  allowed_methods=
-0000eb80: 6672 6f7a 656e 7365 7428 5b27 4745 5427  frozenset(['GET'
-0000eb90: 5d29 2020 2320 4f6e 6c79 2072 6574 7279  ])  # Only retry
-0000eba0: 2066 6f72 2047 4554 2072 6571 7565 7374   for GET request
-0000ebb0: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
-0000ebc0: 2020 2020 732e 6d6f 756e 7428 2768 7474      s.mount('htt
-0000ebd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000ebe0: 272c 2048 5454 5041 6461 7074 6572 286d  ', HTTPAdapter(m
-0000ebf0: 6178 5f72 6574 7269 6573 3d72 6574 7279  ax_retries=retry
-0000ec00: 5f73 7472 6174 6567 7929 290a 2020 2020  _strategy)).    
-0000ec10: 2020 2020 732e 6d6f 756e 7428 2768 7474      s.mount('htt
-0000ec20: 703a 2f2f 6769 7468 7562 2e63 6f6d 2f27  p://github.com/'
-0000ec30: 2c20 4854 5450 4164 6170 7465 7228 6d61  , HTTPAdapter(ma
-0000ec40: 785f 7265 7472 6965 733d 7265 7472 795f  x_retries=retry_
-0000ec50: 7374 7261 7465 6779 2929 0a20 2020 2020  strategy)).     
-0000ec60: 2020 2072 6574 7572 6e20 730a 0a20 2020     return s..   
-0000ec70: 2064 6566 2067 6574 5f77 6f72 6b66 6c6f   def get_workflo
-0000ec80: 775f 636f 6d6d 616e 6428 7365 6c66 2c0a  w_command(self,.
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000ecb0: 6b66 6c6f 773a 2073 7472 2c0a 2020 2020  kflow: str,.    
-0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000ece0: 775f 7665 7273 696f 6e3a 2073 7472 2c0a  w_version: str,.
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
-0000ed10: 7574 5f64 6174 613a 2073 7472 2c0a 2020  ut_data: str,.  
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 2020 2020 2020 2065 6d61 696c             email
-0000ed40: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000ed50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 2020 2020 2074 696d 653a 204f 7074 696f       time: Optio
-0000ed80: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000ed90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eda0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-0000edb0: 6b77 6172 6773 2920 2d3e 2054 7570 6c65  kwargs) -> Tuple
-0000edc0: 5b73 7472 2c20 4469 6374 5d3a 0a20 2020  [str, Dict]:.   
-0000edd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ede0: 2047 656e 6572 6174 6520 7468 6520 536c   Generate the Sl
-0000edf0: 7572 6d20 776f 726b 666c 6f77 2063 6f6d  urm workflow com
-0000ee00: 6d61 6e64 2061 6e64 2065 6e76 6972 6f6e  mand and environ
-0000ee10: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-0000ee20: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000ee30: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000ee40: 6c6f 7720 2873 7472 293a 2054 6865 206e  low (str): The n
-0000ee50: 616d 6520 6f66 2074 6865 2077 6f72 6b66  ame of the workf
-0000ee60: 6c6f 772e 0a20 2020 2020 2020 2020 2020  low..           
-0000ee70: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
-0000ee80: 6e20 2873 7472 293a 2054 6865 2076 6572  n (str): The ver
-0000ee90: 7369 6f6e 206f 6620 7468 6520 776f 726b  sion of the work
-0000eea0: 666c 6f77 2e0a 2020 2020 2020 2020 2020  flow..          
-0000eeb0: 2020 696e 7075 745f 6461 7461 2028 7374    input_data (st
-0000eec0: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
-0000eed0: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
-0000eee0: 6f6c 6465 7220 636f 6e74 6169 6e69 6e67  older containing
-0000eef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef00: 2074 6865 2069 6e70 7574 2069 6d61 6765   the input image
-0000ef10: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
-0000ef20: 2020 2020 656d 6169 6c20 2873 7472 2c20      email (str, 
-0000ef30: 6f70 7469 6f6e 616c 293a 2054 6865 2065  optional): The e
-0000ef40: 6d61 696c 2061 6464 7265 7373 2066 6f72  mail address for
-0000ef50: 206a 6f62 206e 6f74 6966 6963 6174 696f   job notificatio
-0000ef60: 6e73 2e0a 2020 2020 2020 2020 2020 2020  ns..            
-0000ef70: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-0000ef80: 4e6f 6e65 2c20 7768 6963 6820 6465 6661  None, which defa
-0000ef90: 756c 7473 2074 6f20 7768 6174 2069 7320  ults to what is 
-0000efa0: 696e 2074 6865 206a 6f62 2073 6372 6970  in the job scrip
-0000efb0: 742e 0a20 2020 2020 2020 2020 2020 2074  t..            t
-0000efc0: 696d 6520 2873 7472 2c20 6f70 7469 6f6e  ime (str, option
-0000efd0: 616c 293a 2054 6865 2074 696d 6520 6c69  al): The time li
-0000efe0: 6d69 7420 666f 7220 7468 6520 6a6f 6220  mit for the job 
-0000eff0: 696e 2074 6865 200a 2020 2020 2020 2020  in the .        
-0000f000: 2020 2020 2020 2020 666f 726d 6174 2048          format H
-0000f010: 483a 4d4d 3a53 532e 2044 6566 6175 6c74  H:MM:SS. Default
-0000f020: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
-0000f030: 2064 6566 6175 6c74 7320 746f 2077 6861   defaults to wha
-0000f040: 7420 0a20 2020 2020 2020 2020 2020 2020  t .             
-0000f050: 2020 2069 7320 696e 2074 6865 206a 6f62     is in the job
-0000f060: 2073 6372 6970 742e 0a20 2020 2020 2020   script..       
-0000f070: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
-0000f080: 6464 6974 696f 6e61 6c20 6b65 7977 6f72  dditional keywor
-0000f090: 6420 6172 6775 6d65 6e74 7320 666f 7220  d arguments for 
-0000f0a0: 7468 6520 776f 726b 666c 6f77 2e0a 0a20  the workflow... 
-0000f0b0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000f0c0: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
-0000f0d0: 655b 7374 722c 2044 6963 745d 3a0a 2020  e[str, Dict]:.  
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-0000f0f0: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-0000f100: 2074 6865 2053 6c75 726d 2077 6f72 6b66   the Slurm workf
-0000f110: 6c6f 7720 636f 6d6d 616e 6420 616e 640a  low command and.
-0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f130: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-0000f140: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
-0000f150: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f160: 6d6f 6465 6c5f 7061 7468 203d 2073 656c  model_path = sel
-0000f170: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
-0000f180: 7468 735b 776f 726b 666c 6f77 2e6c 6f77  ths[workflow.low
-0000f190: 6572 2829 5d0a 2020 2020 2020 2020 6a6f  er()].        jo
-0000f1a0: 625f 7363 7269 7074 203d 2073 656c 662e  b_script = self.
-0000f1b0: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
-0000f1c0: 5b77 6f72 6b66 6c6f 772e 6c6f 7765 7228  [workflow.lower(
-0000f1d0: 295d 0a20 2020 2020 2020 206a 6f62 5f70  )].        job_p
-0000f1e0: 6172 616d 7320 3d20 7365 6c66 2e73 6c75  arams = self.slu
-0000f1f0: 726d 5f6d 6f64 656c 5f6a 6f62 735f 7061  rm_model_jobs_pa
-0000f200: 7261 6d73 5b77 6f72 6b66 6c6f 772e 6c6f  rams[workflow.lo
-0000f210: 7765 7228 295d 0a20 2020 2020 2020 2023  wer()].        #
-0000f220: 2067 7261 6220 6f6e 6c79 2074 6865 2069   grab only the i
-0000f230: 6d61 6765 206e 616d 652c 206e 6f74 2074  mage name, not t
-0000f240: 6865 2067 726f 7570 2f63 7265 6174 6f72  he group/creator
-0000f250: 0a20 2020 2020 2020 2069 6d61 6765 203d  .        image =
-0000f260: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-0000f270: 6c5f 696d 6167 6573 5b77 6f72 6b66 6c6f  l_images[workflo
-0000f280: 772e 6c6f 7765 7228 295d 2e73 706c 6974  w.lower()].split
-0000f290: 2822 2f22 295b 315d 0a0a 2020 2020 2020  ("/")[1]..      
-0000f2a0: 2020 7362 6174 6368 5f65 6e76 203d 207b    sbatch_env = {
-0000f2b0: 0a20 2020 2020 2020 2020 2020 2022 4441  .            "DA
-0000f2c0: 5441 5f50 4154 4822 3a20 6622 7b73 656c  TA_PATH": f"{sel
-0000f2d0: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-0000f2e0: 687d 2f7b 696e 7075 745f 6461 7461 7d22  h}/{input_data}"
-0000f2f0: 2c0a 2020 2020 2020 2020 2020 2020 2249  ,.            "I
-0000f300: 4d41 4745 5f50 4154 4822 3a20 6622 7b73  MAGE_PATH": f"{s
-0000f310: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
-0000f320: 5f70 6174 687d 2f7b 6d6f 6465 6c5f 7061  _path}/{model_pa
-0000f330: 7468 7d22 2c0a 2020 2020 2020 2020 2020  th}",.          
-0000f340: 2020 2249 4d41 4745 5f56 4552 5349 4f4e    "IMAGE_VERSION
-0000f350: 223a 2066 227b 776f 726b 666c 6f77 5f76  ": f"{workflow_v
-0000f360: 6572 7369 6f6e 7d22 2c0a 2020 2020 2020  ersion}",.      
-0000f370: 2020 2020 2020 2253 494e 4755 4c41 5249        "SINGULARI
-0000f380: 5459 5f49 4d41 4745 223a 2066 227b 696d  TY_IMAGE": f"{im
-0000f390: 6167 657d 5f7b 776f 726b 666c 6f77 5f76  age}_{workflow_v
-0000f3a0: 6572 7369 6f6e 7d2e 7369 6622 2c0a 2020  ersion}.sif",.  
-0000f3b0: 2020 2020 2020 2020 2020 2253 4352 4950            "SCRIP
-0000f3c0: 545f 5041 5448 223a 2066 227b 7365 6c66  T_PATH": f"{self
-0000f3d0: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
-0000f3e0: 7468 7d22 0a20 2020 2020 2020 207d 0a20  th}".        }. 
-0000f3f0: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
-0000f400: 656e 7620 3d20 7365 6c66 2e77 6f72 6b66  env = self.workf
-0000f410: 6c6f 775f 7061 7261 6d73 5f74 6f5f 656e  low_params_to_en
-0000f420: 7676 6172 7328 2a2a 6b77 6172 6773 290a  vvars(**kwargs).
-0000f430: 2020 2020 2020 2020 656e 7620 3d20 7b2a          env = {*
-0000f440: 2a73 6261 7463 685f 656e 762c 202a 2a77  *sbatch_env, **w
-0000f450: 6f72 6b66 6c6f 775f 656e 767d 0a0a 2020  orkflow_env}..  
-0000f460: 2020 2020 2020 656d 6169 6c5f 7061 7261        email_para
-0000f470: 6d20 3d20 2222 2069 6620 656d 6169 6c20  m = "" if email 
-0000f480: 6973 204e 6f6e 6520 656c 7365 2066 2220  is None else f" 
-0000f490: 2d2d 6d61 696c 2d75 7365 723d 7b65 6d61  --mail-user={ema
-0000f4a0: 696c 7d22 0a20 2020 2020 2020 2074 696d  il}".        tim
-0000f4b0: 655f 7061 7261 6d20 3d20 2222 2069 6620  e_param = "" if 
-0000f4c0: 7469 6d65 2069 7320 4e6f 6e65 2065 6c73  time is None els
-0000f4d0: 6520 6622 202d 2d74 696d 653d 7b74 696d  e f" --time={tim
-0000f4e0: 657d 220a 2020 2020 2020 2020 6a6f 625f  e}".        job_
-0000f4f0: 7061 7261 6d73 2e61 7070 656e 6428 7469  params.append(ti
-0000f500: 6d65 5f70 6172 616d 290a 2020 2020 2020  me_param).      
-0000f510: 2020 6a6f 625f 7061 7261 6d73 2e61 7070    job_params.app
-0000f520: 656e 6428 656d 6169 6c5f 7061 7261 6d29  end(email_param)
-0000f530: 0a20 2020 2020 2020 206a 6f62 5f70 6172  .        job_par
-0000f540: 616d 203d 2022 222e 6a6f 696e 286a 6f62  am = "".join(job
-0000f550: 5f70 6172 616d 7329 0a20 2020 2020 2020  _params).       
-0000f560: 2073 6261 7463 685f 636d 6420 3d20 6622   sbatch_cmd = f"
-0000f570: 7362 6174 6368 7b6a 6f62 5f70 6172 616d  sbatch{job_param
-0000f580: 7d20 2d2d 6f75 7470 7574 3d6f 6d65 726f  } --output=omero
-0000f590: 2d25 6a2e 6c6f 6720 5c0a 2020 2020 2020  -%j.log \.      
-0000f5a0: 2020 2020 2020 7b73 656c 662e 736c 7572        {self.slur
-0000f5b0: 6d5f 7363 7269 7074 5f70 6174 687d 2f7b  m_script_path}/{
-0000f5c0: 6a6f 625f 7363 7269 7074 7d22 0a0a 2020  job_script}"..  
-0000f5d0: 2020 2020 2020 7265 7475 726e 2073 6261        return sba
-0000f5e0: 7463 685f 636d 642c 2065 6e76 0a0a 2020  tch_cmd, env..  
-0000f5f0: 2020 6465 6620 6765 745f 636f 6e76 6572    def get_conver
-0000f600: 7369 6f6e 5f63 6f6d 6d61 6e64 2873 656c  sion_command(sel
-0000f610: 662c 2064 6174 615f 7061 7468 3a20 7374  f, data_path: st
-0000f620: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 636f 6e66 6967 5f66 696c 653a 2073    config_file: s
-0000f650: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 2020 2073 6f75 7263 655f 666f 726d 6174     source_format
-0000f680: 3a20 7374 7220 3d20 277a 6172 7227 2c0a  : str = 'zarr',.
-0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000f6b0: 6172 6765 745f 666f 726d 6174 3a20 7374  arget_format: st
-0000f6c0: 7220 3d20 2774 6966 6627 2920 2d3e 2054  r = 'tiff') -> T
-0000f6d0: 7570 6c65 5b73 7472 2c20 4469 6374 5d3a  uple[str, Dict]:
-0000f6e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f6f0: 2020 2020 2047 656e 6572 6174 6520 536c       Generate Sl
-0000f700: 7572 6d20 636f 6e76 6572 7369 6f6e 2063  urm conversion c
-0000f710: 6f6d 6d61 6e64 2061 6e64 2065 6e76 6972  ommand and envir
-0000f720: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-0000f730: 2066 6f72 2064 6174 6120 636f 6e76 6572   for data conver
-0000f740: 7369 6f6e 2e0a 0a20 2020 2020 2020 2041  sion...        A
-0000f750: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000f760: 2064 6174 615f 7061 7468 2028 7374 7229   data_path (str)
-0000f770: 3a20 5061 7468 2074 6f20 7468 6520 6461  : Path to the da
-0000f780: 7461 2066 6f6c 6465 722e 0a20 2020 2020  ta folder..     
-0000f790: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
-0000f7a0: 6c65 2028 7374 7229 3a20 5061 7468 2074  le (str): Path t
-0000f7b0: 6f20 7468 6520 636f 6e66 6967 7572 6174  o the configurat
-0000f7c0: 696f 6e20 6669 6c65 2e0a 2020 2020 2020  ion file..      
-0000f7d0: 2020 2020 2020 736f 7572 6365 5f66 6f72        source_for
-0000f7e0: 6d61 7420 2873 7472 293a 2053 6f75 7263  mat (str): Sourc
-0000f7f0: 6520 6461 7461 2066 6f72 6d61 7420 2864  e data format (d
-0000f800: 6566 6175 6c74 2069 7320 277a 6172 7227  efault is 'zarr'
-0000f810: 292e 0a20 2020 2020 2020 2020 2020 2074  )..            t
-0000f820: 6172 6765 745f 666f 726d 6174 2028 7374  arget_format (st
-0000f830: 7229 3a20 5461 7267 6574 2064 6174 6120  r): Target data 
-0000f840: 666f 726d 6174 2028 6465 6661 756c 7420  format (default 
-0000f850: 6973 2027 7469 6666 2729 2e0a 0a20 2020  is 'tiff')...   
-0000f860: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000f870: 2020 2020 2020 2020 2020 5475 706c 655b            Tuple[
-0000f880: 7374 722c 2044 6963 745d 3a0a 2020 2020  str, Dict]:.    
-0000f890: 2020 2020 2020 2020 2020 2020 4120 7475              A tu
-0000f8a0: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
-0000f8b0: 6865 2053 6c75 726d 2063 6f6e 7665 7273  he Slurm convers
-0000f8c0: 696f 6e20 636f 6d6d 616e 6420 616e 640a  ion command and.
-0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8e0: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-0000f8f0: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
-0000f900: 2020 2020 5761 726e 696e 673a 0a20 2020      Warning:.   
-0000f910: 2020 2020 2020 2020 2054 6865 2064 6566           The def
-0000f920: 6175 6c74 2069 6d70 6c65 6d65 6e74 6174  ault implementat
-0000f930: 696f 6e20 6f6e 6c79 2073 7570 706f 7274  ion only support
-0000f940: 7320 636f 6e76 6572 7369 6f6e 2066 726f  s conversion fro
-0000f950: 6d20 277a 6172 7227 2074 6f20 2774 6966  m 'zarr' to 'tif
-0000f960: 6627 2e0a 2020 2020 2020 2020 2020 2020  f'..            
-0000f970: 4966 2075 7369 6e67 206f 7468 6572 2073  If using other s
-0000f980: 6f75 7263 6520 6f72 2074 6172 6765 7420  ource or target 
-0000f990: 666f 726d 6174 732c 2075 7365 7273 206d  formats, users m
-0000f9a0: 7573 7420 696d 706c 656d 656e 7420 616e  ust implement an
-0000f9b0: 6420 636f 6e66 6967 7572 650a 2020 2020  d configure.    
-0000f9c0: 2020 2020 2020 2020 6164 6469 7469 6f6e          addition
-0000f9d0: 616c 2063 6f6e 7665 7274 6572 7320 7468  al converters th
-0000f9e0: 656d 7365 6c76 6573 2e0a 2020 2020 2020  emselves..      
-0000f9f0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000fa00: 2073 6f75 7263 655f 666f 726d 6174 2021   source_format !
-0000fa10: 3d20 227a 6172 7222 206f 7220 7461 7267  = "zarr" or targ
-0000fa20: 6574 5f66 6f72 6d61 7420 213d 2022 7469  et_format != "ti
-0000fa30: 6666 223a 0a20 2020 2020 2020 2020 2020  ff":.           
-0000fa40: 2023 2057 6172 6e20 6162 6f75 7420 756e   # Warn about un
-0000fa50: 7375 7070 6f72 7465 6420 636f 6e76 6572  supported conver
-0000fa60: 7369 6f6e 3b20 6164 6469 7469 6f6e 616c  sion; additional
-0000fa70: 2063 6f6e 7665 7274 6572 7320 6361 6e20   converters can 
-0000fa80: 6265 0a20 2020 2020 2020 2020 2020 2023  be.            #
-0000fa90: 2061 6464 6564 206f 7574 7369 6465 206f   added outside o
-0000faa0: 7572 206b 6e6f 776c 6564 6765 2e0a 2020  ur knowledge..  
-0000fab0: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
-0000fac0: 6b69 6e67 2053 6c75 726d 2773 2060 736c  king Slurm's `sl
-0000fad0: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
-0000fae0: 6174 6860 2069 7320 736b 6970 7065 6420  ath` is skipped 
-0000faf0: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
-0000fb00: 2320 7065 7266 6f72 6d61 6e63 6520 7265  # performance re
-0000fb10: 6173 6f6e 732e 0a20 2020 2020 2020 2020  asons..         
-0000fb20: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-0000fb30: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-0000fb40: 2020 2066 2243 6f6e 7665 7273 696f 6e20     f"Conversion 
-0000fb50: 6672 6f6d 207b 736f 7572 6365 5f66 6f72  from {source_for
-0000fb60: 6d61 747d 2074 6f20 7b74 6172 6765 745f  mat} to {target_
-0000fb70: 666f 726d 6174 7d20 6973 206e 6f74 2073  format} is not s
-0000fb80: 7570 706f 7274 6564 2062 7920 6465 6661  upported by defa
-0000fb90: 756c 7421 2229 0a0a 2020 2020 2020 2020  ult!")..        
-0000fba0: 6368 6f73 656e 5f63 6f6e 7665 7274 6572  chosen_converter
-0000fbb0: 203d 2066 2263 6f6e 7665 7274 5f7b 736f   = f"convert_{so
-0000fbc0: 7572 6365 5f66 6f72 6d61 747d 5f74 6f5f  urce_format}_to_
-0000fbd0: 7b74 6172 6765 745f 666f 726d 6174 7d2e  {target_format}.
-0000fbe0: 7369 6622 0a20 2020 2020 2020 2073 6261  sif".        sba
-0000fbf0: 7463 685f 656e 7620 3d20 7b0a 2020 2020  tch_env = {.    
-0000fc00: 2020 2020 2020 2020 2244 4154 415f 5041          "DATA_PA
-0000fc10: 5448 223a 2066 227b 6461 7461 5f70 6174  TH": f"{data_pat
-0000fc20: 687d 222c 0a20 2020 2020 2020 2020 2020  h}",.           
-0000fc30: 2022 434f 4e56 4552 5349 4f4e 5f50 4154   "CONVERSION_PAT
-0000fc40: 4822 3a20 6622 7b73 656c 662e 736c 7572  H": f"{self.slur
-0000fc50: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
-0000fc60: 687d 222c 0a20 2020 2020 2020 2020 2020  h}",.           
-0000fc70: 2022 434f 4e56 4552 5445 525f 494d 4147   "CONVERTER_IMAG
-0000fc80: 4522 3a20 6368 6f73 656e 5f63 6f6e 7665  E": chosen_conve
-0000fc90: 7274 6572 2c0a 2020 2020 2020 2020 2020  rter,.          
-0000fca0: 2020 2253 4352 4950 545f 5041 5448 223a    "SCRIPT_PATH":
-0000fcb0: 2066 227b 7365 6c66 2e73 6c75 726d 5f73   f"{self.slurm_s
-0000fcc0: 6372 6970 745f 7061 7468 7d22 2c0a 2020  cript_path}",.  
-0000fcd0: 2020 2020 2020 2020 2020 2243 4f4e 4649            "CONFI
-0000fce0: 475f 4649 4c45 223a 2066 227b 636f 6e66  G_FILE": f"{conf
-0000fcf0: 6967 5f66 696c 657d 220a 2020 2020 2020  ig_file}".      
-0000fd00: 2020 7d0a 0a20 2020 2020 2020 2063 6f6e    }..        con
-0000fd10: 7665 7273 696f 6e5f 636d 6420 3d20 2273  version_cmd = "s
-0000fd20: 6261 7463 6820 2d2d 6a6f 622d 6e61 6d65  batch --job-name
-0000fd30: 3d63 6f6e 7665 7273 696f 6e20 2d2d 6578  =conversion --ex
-0000fd40: 706f 7274 3d41 4c4c 2c43 4f4e 4649 475f  port=ALL,CONFIG_
-0000fd50: 5041 5448 3d5c 2224 5057 442f 2443 4f4e  PATH=\"$PWD/$CON
-0000fd60: 4649 475f 4649 4c45 5c22 202d 2d61 7272  FIG_FILE\" --arr
-0000fd70: 6179 3d31 2d24 4e20 2453 4352 4950 545f  ay=1-$N $SCRIPT_
-0000fd80: 5041 5448 2f63 6f6e 7665 7274 5f6a 6f62  PATH/convert_job
-0000fd90: 5f61 7272 6179 2e73 6822 0a20 2020 2020  _array.sh".     
-0000fda0: 2020 2023 2063 6f6e 7665 7273 696f 6e5f     # conversion_
-0000fdb0: 636d 645f 7761 6974 696e 6720 3d20 2273  cmd_waiting = "s
-0000fdc0: 6261 7463 6820 2d2d 6a6f 622d 6e61 6d65  batch --job-name
-0000fdd0: 3d63 6f6e 7665 7273 696f 6e20 2d2d 6578  =conversion --ex
-0000fde0: 706f 7274 3d41 4c4c 2c43 4f4e 4649 475f  port=ALL,CONFIG_
-0000fdf0: 5041 5448 3d5c 2224 5057 442f 2443 4f4e  PATH=\"$PWD/$CON
-0000fe00: 4649 475f 4649 4c45 5c22 202d 2d61 7272  FIG_FILE\" --arr
-0000fe10: 6179 3d31 2d24 4e20 2d2d 7761 6974 2024  ay=1-$N --wait $
-0000fe20: 5343 5249 5054 5f50 4154 482f 636f 6e76  SCRIPT_PATH/conv
-0000fe30: 6572 745f 6a6f 625f 6172 7261 792e 7368  ert_job_array.sh
-0000fe40: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000fe50: 6e20 636f 6e76 6572 7369 6f6e 5f63 6d64  n conversion_cmd
-0000fe60: 2c20 7362 6174 6368 5f65 6e76 0a0a 2020  , sbatch_env..  
-0000fe70: 2020 6465 6620 776f 726b 666c 6f77 5f70    def workflow_p
-0000fe80: 6172 616d 735f 746f 5f65 6e76 7661 7273  arams_to_envvars
-0000fe90: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-0000fea0: 202d 3e20 4469 6374 3a0a 2020 2020 2020   -> Dict:.      
-0000feb0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
-0000fec0: 6e76 6572 7420 776f 726b 666c 6f77 2070  nvert workflow p
-0000fed0: 6172 616d 6574 6572 7320 746f 2065 6e76  arameters to env
-0000fee0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-0000fef0: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
-0000ff00: 733a 0a20 2020 2020 2020 2020 2020 202a  s:.            *
-0000ff10: 2a6b 7761 7267 733a 2041 6464 6974 696f  *kwargs: Additio
-0000ff20: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
-0000ff30: 6d65 6e74 7320 666f 7220 7468 6520 776f  ments for the wo
-0000ff40: 726b 666c 6f77 2e0a 0a20 2020 2020 2020  rkflow...       
-0000ff50: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000ff60: 2020 2020 2020 4469 6374 3a20 4120 6469        Dict: A di
-0000ff70: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-0000ff80: 696e 6720 7468 6520 656e 7669 726f 6e6d  ing the environm
-0000ff90: 656e 7420 7661 7269 6162 6c65 732e 0a20  ent variables.. 
-0000ffa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ffb0: 2020 2077 6f72 6b66 6c6f 775f 656e 7620     workflow_env 
-0000ffc0: 3d20 7b6b 6579 2e75 7070 6572 2829 3a20  = {key.upper(): 
-0000ffd0: 6622 7b76 616c 7565 7d22 2066 6f72 206b  f"{value}" for k
-0000ffe0: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
-0000fff0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00010000: 6520 696e 206b 7761 7267 732e 6974 656d  e in kwargs.item
-00010010: 7328 297d 0a20 2020 2020 2020 206c 6f67  s()}.        log
-00010020: 6765 722e 6465 6275 6728 776f 726b 666c  ger.debug(workfl
-00010030: 6f77 5f65 6e76 290a 2020 2020 2020 2020  ow_env).        
-00010040: 7265 7475 726e 2077 6f72 6b66 6c6f 775f  return workflow_
-00010050: 656e 760a 0a20 2020 2064 6566 2067 6574  env..    def get
-00010060: 5f63 656c 6c70 6f73 655f 636f 6d6d 616e  _cellpose_comman
-00010070: 6428 7365 6c66 2c20 696d 6167 655f 7665  d(self, image_ve
-00010080: 7273 696f 6e3a 2073 7472 2c0a 2020 2020  rsion: str,.    
-00010090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100a0: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
-000100b0: 6174 613a 2073 7472 2c0a 2020 2020 2020  ata: str,.      
-000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100d0: 2020 2020 2020 2063 705f 6d6f 6465 6c3a         cp_model:
-000100e0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010100: 2020 206e 7563 5f63 6861 6e6e 656c 3a20     nuc_channel: 
-00010110: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010130: 2020 7072 6f62 5f74 6872 6573 686f 6c64    prob_threshold
-00010140: 3a20 666c 6f61 742c 0a20 2020 2020 2020  : float,.       
-00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010160: 2020 2020 2020 6365 6c6c 5f64 6961 6d65        cell_diame
-00010170: 7465 723a 2066 6c6f 6174 2c0a 2020 2020  ter: float,.    
-00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2020 2020 2020 2020 2065 6d61 696c 3a20           email: 
-000101a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000101b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2074 696d 653a 204f 7074 696f 6e61     time: Optiona
-000101e0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010200: 2020 2020 2020 2020 2020 2020 7573 655f              use_
-00010210: 6770 753a 2062 6f6f 6c20 3d20 5472 7565  gpu: bool = True
-00010220: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010230: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00010240: 6f64 656c 3a20 7374 7220 3d20 2263 656c  odel: str = "cel
-00010250: 6c70 6f73 6522 2920 2d3e 2054 7570 6c65  lpose") -> Tuple
-00010260: 5b73 7472 2c20 4469 6374 5d3a 0a20 2020  [str, Dict]:.   
-00010270: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010280: 2052 6574 7572 6e20 7468 6520 636f 6d6d   Return the comm
-00010290: 616e 6420 616e 6420 656e 7669 726f 6e6d  and and environm
-000102a0: 656e 7420 6469 6374 696f 6e61 7279 2074  ent dictionary t
-000102b0: 6f20 7275 6e20 6120 4365 6c6c 506f 7365  o run a CellPose
-000102c0: 206a 6f62 0a20 2020 2020 2020 206f 6e20   job.        on 
-000102d0: 7468 6520 536c 7572 6d20 776f 726b 6c6f  the Slurm worklo
-000102e0: 6164 206d 616e 6167 6572 2e0a 2020 2020  ad manager..    
-000102f0: 2020 2020 4120 7370 6563 6966 6963 2065      A specific e
-00010300: 7861 6d70 6c65 206f 6620 7573 696e 6720  xample of using 
-00010310: 7468 6520 6765 6e65 7269 6320 2767 6574  the generic 'get
-00010320: 5f77 6f72 6b66 6c6f 775f 636f 6d6d 616e  _workflow_comman
-00010330: 6427 2e0a 0a20 2020 2020 2020 2041 7267  d'...        Arg
-00010340: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00010350: 6d61 6765 5f76 6572 7369 6f6e 2028 7374  mage_version (st
-00010360: 7229 3a20 5468 6520 7665 7273 696f 6e20  r): The version 
-00010370: 6f66 2074 6865 2053 696e 6775 6c61 7269  of the Singulari
-00010380: 7479 2069 6d61 6765 2074 6f20 7573 652e  ty image to use.
-00010390: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-000103a0: 7574 5f64 6174 6120 2873 7472 293a 2054  ut_data (str): T
-000103b0: 6865 206e 616d 6520 6f66 2074 6865 2069  he name of the i
-000103c0: 6e70 7574 2064 6174 6120 666f 6c64 6572  nput data folder
-000103d0: 206f 6e20 7468 6520 7368 6172 6564 0a20   on the shared. 
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000103f0: 696c 6520 7379 7374 656d 2e0a 2020 2020  ile system..    
-00010400: 2020 2020 2020 2020 6370 5f6d 6f64 656c          cp_model
-00010410: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
-00010420: 206f 6620 7468 6520 4365 6c6c 506f 7365   of the CellPose
-00010430: 206d 6f64 656c 2074 6f20 7573 652e 0a20   model to use.. 
-00010440: 2020 2020 2020 2020 2020 206e 7563 5f63             nuc_c
-00010450: 6861 6e6e 656c 2028 696e 7429 3a20 5468  hannel (int): Th
-00010460: 6520 696e 6465 7820 6f66 2074 6865 206e  e index of the n
-00010470: 7563 6c65 6172 2063 6861 6e6e 656c 2e0a  uclear channel..
-00010480: 2020 2020 2020 2020 2020 2020 7072 6f62              prob
-00010490: 5f74 6872 6573 686f 6c64 2028 666c 6f61  _threshold (floa
-000104a0: 7429 3a20 5468 6520 7072 6f62 6162 696c  t): The probabil
-000104b0: 6974 7920 7468 7265 7368 6f6c 6420 666f  ity threshold fo
-000104c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-000104d0: 2020 6e75 636c 6569 2064 6574 6563 7469    nuclei detecti
-000104e0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-000104f0: 6365 6c6c 5f64 6961 6d65 7465 7220 2866  cell_diameter (f
-00010500: 6c6f 6174 293a 2054 6865 2065 7870 6563  loat): The expec
-00010510: 7465 6420 6365 6c6c 2064 6961 6d65 7465  ted cell diamete
-00010520: 7220 696e 2070 6978 656c 732e 0a20 2020  r in pixels..   
-00010530: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
-00010540: 4f70 7469 6f6e 616c 5b73 7472 5d29 3a20  Optional[str]): 
-00010550: 5468 6520 656d 6169 6c20 6164 6472 6573  The email addres
-00010560: 7320 746f 2073 656e 6420 6e6f 7469 6669  s to send notifi
-00010570: 6361 7469 6f6e 7320 746f 2e0a 2020 2020  cations to..    
-00010580: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00010590: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-000105a0: 2020 2020 2020 2020 2020 7469 6d65 2028            time (
-000105b0: 4f70 7469 6f6e 616c 5b73 7472 5d29 3a20  Optional[str]): 
-000105c0: 5468 6520 6d61 7869 6d75 6d20 7469 6d65  The maximum time
-000105d0: 2066 6f72 2074 6865 206a 6f62 2074 6f20   for the job to 
-000105e0: 7275 6e2e 0a20 2020 2020 2020 2020 2020  run..           
-000105f0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00010600: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
-00010610: 2020 2075 7365 5f67 7075 2028 626f 6f6c     use_gpu (bool
-00010620: 293a 2057 6865 7468 6572 2074 6f20 7573  ): Whether to us
-00010630: 6520 4750 5520 666f 7220 7468 6520 4365  e GPU for the Ce
-00010640: 6c6c 506f 7365 206a 6f62 2e0a 2020 2020  llPose job..    
-00010650: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00010660: 756c 7473 2074 6f20 5472 7565 2e0a 2020  ults to True..  
-00010670: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
-00010680: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
-00010690: 6f66 2074 6865 2066 6f6c 6465 7220 6f66  of the folder of
-000106a0: 2074 6865 2044 6f63 6b65 7220 696d 6167   the Docker imag
-000106b0: 6520 746f 2075 7365 2e0a 2020 2020 2020  e to use..      
-000106c0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-000106d0: 7473 2074 6f20 2263 656c 6c70 6f73 6522  ts to "cellpose"
-000106e0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000106f0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00010700: 5475 706c 655b 7374 722c 2064 6963 745d  Tuple[str, dict]
-00010710: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010720: 2020 4120 7475 706c 6520 636f 6e74 6169    A tuple contai
-00010730: 6e69 6e67 2074 6865 2053 6c75 726d 2073  ning the Slurm s
-00010740: 6261 7463 6820 636f 6d6d 616e 640a 2020  batch command.  
-00010750: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00010760: 6420 7468 6520 656e 7669 726f 6e6d 656e  d the environmen
-00010770: 7420 6469 6374 696f 6e61 7279 2e0a 2020  t dictionary..  
-00010780: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010790: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-000107a0: 745f 776f 726b 666c 6f77 5f63 6f6d 6d61  t_workflow_comma
-000107b0: 6e64 2877 6f72 6b66 6c6f 773d 6d6f 6465  nd(workflow=mode
-000107c0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107e0: 2020 2020 2020 2020 2020 2020 776f 726b              work
-000107f0: 666c 6f77 5f76 6572 7369 6f6e 3d69 6d61  flow_version=ima
-00010800: 6765 5f76 6572 7369 6f6e 2c0a 2020 2020  ge_version,.    
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 2020 2069 6e70 7574 5f64 6174 613d       input_data=
-00010840: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a090: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
+0000a0a0: 3a20 7374 7220 3d20 226a 6f62 5f74 656d  : str = "job_tem
+0000a0b0: 706c 6174 652e 7368 220a 2020 2020 2020  plate.sh".      
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0e0: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
+0000a0f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a100: 4765 6e65 7261 7465 2061 2053 6c75 726d  Generate a Slurm
+0000a110: 206a 6f62 2073 6372 6970 7420 666f 7220   job script for 
+0000a120: 6120 7370 6563 6966 6963 2077 6f72 6b66  a specific workf
+0000a130: 6c6f 772e 0a0a 2020 2020 2020 2020 4172  low...        Ar
+0000a140: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000a150: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
+0000a160: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0000a170: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
+0000a180: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
+0000a190: 7320 2844 6963 745b 7374 722c 2073 7472  s (Dict[str, str
+0000a1a0: 5d29 3a20 4120 6469 6374 696f 6e61 7279  ]): A dictionary
+0000a1b0: 2063 6f6e 7461 696e 696e 6720 6b65 792d   containing key-
+0000a1c0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
+0000a1d0: 2020 2020 2020 7061 6972 7320 666f 7220        pairs for 
+0000a1e0: 7375 6273 7469 7475 7469 6e67 2070 6c61  substituting pla
+0000a1f0: 6365 686f 6c64 6572 7320 696e 2074 6865  ceholders in the
+0000a200: 206a 6f62 2074 656d 706c 6174 652e 0a20   job template.. 
+0000a210: 2020 2020 2020 2020 2020 2074 656d 706c             templ
+0000a220: 6174 6520 2873 7472 2c20 6f70 7469 6f6e  ate (str, option
+0000a230: 616c 293a 2054 6865 2066 696c 656e 616d  al): The filenam
+0000a240: 6520 6f66 2074 6865 206a 6f62 2074 656d  e of the job tem
+0000a250: 706c 6174 652e 0a20 2020 2020 2020 2020  plate..         
+0000a260: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+0000a270: 746f 2022 6a6f 625f 7465 6d70 6c61 7465  to "job_template
+0000a280: 2e73 6822 2e0a 0a20 2020 2020 2020 2052  .sh"...        R
+0000a290: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000a2a0: 2020 2020 7374 723a 2054 6865 2067 656e      str: The gen
+0000a2b0: 6572 6174 6564 2053 6c75 726d 206a 6f62  erated Slurm job
+0000a2c0: 2073 6372 6970 7420 6173 2061 2073 7472   script as a str
+0000a2d0: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
+0000a2e0: 0a20 2020 2020 2020 2023 2061 6464 2077  .        # add w
+0000a2f0: 6f72 6b66 6c6f 7720 746f 2073 7562 7374  orkflow to subst
+0000a300: 6974 7574 6573 0a20 2020 2020 2020 2073  itutes.        s
+0000a310: 7562 7374 6974 7574 6573 5b27 6a6f 626e  ubstitutes['jobn
+0000a320: 616d 6527 5d20 3d20 776f 726b 666c 6f77  ame'] = workflow
+0000a330: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
+0000a340: 6a6f 6220 7465 6d70 6c61 7465 0a20 2020  job template.   
+0000a350: 2020 2020 2074 656d 706c 6174 655f 6620       template_f 
+0000a360: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
+0000a370: 6573 2229 2e6a 6f69 6e70 6174 6828 7465  es").joinpath(te
+0000a380: 6d70 6c61 7465 290a 2020 2020 2020 2020  mplate).        
+0000a390: 7769 7468 2074 656d 706c 6174 655f 662e  with template_f.
+0000a3a0: 6f70 656e 2827 7227 2920 6173 2066 3a0a  open('r') as f:.
+0000a3b0: 2020 2020 2020 2020 2020 2020 7372 6320              src 
+0000a3c0: 3d20 5465 6d70 6c61 7465 2866 2e72 6561  = Template(f.rea
+0000a3d0: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+0000a3e0: 206a 6f62 5f73 6372 6970 7420 3d20 7372   job_script = sr
+0000a3f0: 632e 7361 6665 5f73 7562 7374 6974 7574  c.safe_substitut
+0000a400: 6528 7375 6273 7469 7475 7465 7329 0a20  e(substitutes). 
+0000a410: 2020 2020 2020 2072 6574 7572 6e20 6a6f         return jo
+0000a420: 625f 7363 7269 7074 0a0a 2020 2020 6465  b_script..    de
+0000a430: 6620 776f 726b 666c 6f77 5f70 6172 616d  f workflow_param
+0000a440: 735f 746f 5f73 7562 7328 7365 6c66 2c20  s_to_subs(self, 
+0000a450: 7061 7261 6d73 2920 2d3e 2044 6963 745b  params) -> Dict[
+0000a460: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
+0000a470: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000a480: 6f6e 7665 7274 2077 6f72 6b66 6c6f 7720  onvert workflow 
+0000a490: 7061 7261 6d65 7465 7273 2074 6f20 7375  parameters to su
+0000a4a0: 6273 7469 7475 7469 6f6e 2064 6963 7469  bstitution dicti
+0000a4b0: 6f6e 6172 7920 666f 7220 6a6f 6220 7363  onary for job sc
+0000a4c0: 7269 7074 2e0a 0a20 2020 2020 2020 2041  ript...        A
+0000a4d0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000a4e0: 2070 6172 616d 733a 2041 2064 6963 7469   params: A dicti
+0000a4f0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+0000a500: 2077 6f72 6b66 6c6f 7720 7061 7261 6d65   workflow parame
+0000a510: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
+0000a520: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000a530: 2020 2020 4469 6374 5b73 7472 2c20 7374      Dict[str, st
+0000a540: 725d 3a20 4120 6469 6374 696f 6e61 7279  r]: A dictionary
+0000a550: 2077 6974 6820 7061 7261 6d65 7465 7220   with parameter 
+0000a560: 6e61 6d65 7320 6173 206b 6579 7320 616e  names as keys an
+0000a570: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000a580: 2020 636f 7272 6573 706f 6e64 696e 6720    corresponding 
+0000a590: 666c 6167 7320 7769 7468 2070 6c61 6365  flags with place
+0000a5a0: 686f 6c64 6572 7320 6173 2076 616c 7565  holders as value
+0000a5b0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0000a5c0: 2020 2020 2020 2073 7562 7320 3d20 7b7d         subs = {}
+0000a5d0: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
+0000a5e0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0000a5f0: 5f2c 2070 6172 616d 2069 6e20 7061 7261  _, param in para
+0000a600: 6d73 2e69 7465 6d73 2829 3a0a 2020 2020  ms.items():.    
+0000a610: 2020 2020 2020 2020 666c 6167 203d 2070          flag = p
+0000a620: 6172 616d 5b27 636d 645f 666c 6167 275d  aram['cmd_flag']
+0000a630: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
+0000a640: 6720 3d20 666c 6167 202b 2022 2024 2220  g = flag + " $" 
+0000a650: 2b20 7061 7261 6d5b 276e 616d 6527 5d2e  + param['name'].
+0000a660: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+0000a670: 2020 2020 666c 6167 732e 6170 7065 6e64      flags.append
+0000a680: 2866 6c61 6729 0a20 2020 2020 2020 2073  (flag).        s
+0000a690: 7562 735b 2750 4152 414d 5327 5d20 3d20  ubs['PARAMS'] = 
+0000a6a0: 2220 222e 6a6f 696e 2866 6c61 6773 290a  " ".join(flags).
+0000a6b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000a6c0: 7562 730a 0a20 2020 2064 6566 2075 7064  ubs..    def upd
+0000a6d0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
+0000a6e0: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2067 656e 6572 6174 655f 6a6f       generate_jo
+0000a710: 6273 3a20 626f 6f6c 203d 2046 616c 7365  bs: bool = False
+0000a720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a730: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a740: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
+0000a750: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
+0000a760: 6f6e 6529 202d 3e20 5265 7375 6c74 3a0a  one) -> Result:.
+0000a770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000a780: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
+0000a790: 6c6f 6361 6c20 636f 7079 206f 6620 7468  local copy of th
+0000a7a0: 6520 536c 7572 6d20 6a6f 6220 7375 626d  e Slurm job subm
+0000a7b0: 6973 7369 6f6e 2073 6372 6970 7473 2e0a  ission scripts..
+0000a7c0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
+0000a7d0: 6e63 7469 6f6e 2070 756c 6c73 2074 6865  nction pulls the
+0000a7e0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+0000a7f0: 6f66 2074 6865 2073 6372 6970 7473 2066  of the scripts f
+0000a800: 726f 6d20 7468 6520 4769 740a 2020 2020  rom the Git.    
+0000a810: 2020 2020 7265 706f 7369 746f 7279 2061      repository a
+0000a820: 6e64 2063 6f70 6965 7320 7468 656d 2074  nd copies them t
+0000a830: 6f20 7468 6520 736c 7572 6d5f 7363 7269  o the slurm_scri
+0000a840: 7074 5f70 6174 6820 6469 7265 6374 6f72  pt_path director
+0000a850: 792e 0a20 2020 2020 2020 2041 6c74 6572  y..        Alter
+0000a860: 6e61 7469 7665 6c79 2c20 6974 2063 616e  natively, it can
+0000a870: 2067 656e 6572 6174 6520 7363 7269 7074   generate script
+0000a880: 7320 6672 6f6d 2061 2074 656d 706c 6174  s from a templat
+0000a890: 652e 2054 6869 7320 6973 2074 6865 0a20  e. This is the. 
+0000a8a0: 2020 2020 2020 2064 6566 6175 6c74 2062         default b
+0000a8b0: 6568 6176 696f 7220 6966 206e 6f20 4769  ehavior if no Gi
+0000a8c0: 7420 7265 706f 2069 7320 7072 6f76 6964  t repo is provid
+0000a8d0: 6564 206f 7220 6361 6e20 6265 2066 6f72  ed or can be for
+0000a8e0: 6365 6420 7669 6120 7468 650a 2020 2020  ced via the.    
+0000a8f0: 2020 2020 6067 656e 6572 6174 655f 6a6f      `generate_jo
+0000a900: 6273 6020 7061 7261 6d65 7465 722e 0a0a  bs` parameter...
+0000a910: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000a920: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+0000a930: 7465 5f6a 6f62 7320 2862 6f6f 6c29 3a20  te_jobs (bool): 
+0000a940: 5768 6574 6865 7220 746f 2067 656e 6572  Whether to gener
+0000a950: 6174 6520 6e65 7720 736c 7572 6d20 6a6f  ate new slurm jo
+0000a960: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
+0000a970: 2020 2020 2020 2020 2020 494e 5354 4541            INSTEA
+0000a980: 4420 286f 6620 7075 6c6c 696e 6720 6672  D (of pulling fr
+0000a990: 6f6d 2067 6974 292e 2044 6566 6175 6c74  om git). Default
+0000a9a0: 7320 746f 2046 616c 7365 2c20 6578 6365  s to False, exce
+0000a9b0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
+0000a9c0: 2020 2069 6620 6e6f 2073 6c75 726d 5f73     if no slurm_s
+0000a9d0: 6372 6970 745f 7265 706f 2069 7320 636f  cript_repo is co
+0000a9e0: 6e66 6967 7572 6564 2e0a 2020 2020 2020  nfigured..      
+0000a9f0: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+0000aa00: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+0000aa10: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+0000aa20: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+0000aa30: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
+0000aa40: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
+0000aa50: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+0000aa60: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+0000aa70: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+0000aa80: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000aa90: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
+0000aaa0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+0000aab0: 2063 6f6d 6d61 6e64 2e0a 2020 2020 2020   command..      
+0000aac0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000aad0: 206e 6f74 2073 656c 662e 736c 7572 6d5f   not self.slurm_
+0000aae0: 7363 7269 7074 5f72 6570 6f3a 0a20 2020  script_repo:.   
+0000aaf0: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+0000ab00: 655f 6a6f 6273 203d 2054 7275 650a 0a20  e_jobs = True.. 
+0000ab10: 2020 2020 2020 2069 6620 6765 6e65 7261         if genera
+0000ab20: 7465 5f6a 6f62 733a 0a20 2020 2020 2020  te_jobs:.       
+0000ab30: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000ab40: 2822 4765 6e65 7261 7469 6e67 2053 6c75  ("Generating Slu
+0000ab50: 726d 206a 6f62 2073 6372 6970 7473 2229  rm job scripts")
+0000ab60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000ab70: 2077 662c 206a 6f62 5f70 6174 6820 696e   wf, job_path in
+0000ab80: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+0000ab90: 6c5f 6a6f 6273 2e69 7465 6d73 2829 3a0a  l_jobs.items():.
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 2320 6765 6e65 7261 7465 206a 6f62 2073  # generate job s
+0000abc0: 6372 6970 740a 2020 2020 2020 2020 2020  cript.          
+0000abd0: 2020 2020 2020 7061 7261 6d73 203d 2073        params = s
+0000abe0: 656c 662e 6765 745f 776f 726b 666c 6f77  elf.get_workflow
+0000abf0: 5f70 6172 616d 6574 6572 7328 7766 290a  _parameters(wf).
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 7375 6273 203d 2073 656c 662e 776f 726b  subs = self.work
+0000ac20: 666c 6f77 5f70 6172 616d 735f 746f 5f73  flow_params_to_s
+0000ac30: 7562 7328 7061 7261 6d73 290a 2020 2020  ubs(params).    
+0000ac40: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000ac50: 7363 7269 7074 203d 2073 656c 662e 6765  script = self.ge
+0000ac60: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
+0000ac70: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7766  _for_workflow(wf
+0000ac80: 2c20 7375 6273 290a 2020 2020 2020 2020  , subs).        
+0000ac90: 2020 2020 2020 2020 2320 656e 7375 7265          # ensure
+0000aca0: 2061 6c6c 2064 6972 7320 6578 6973 7420   all dirs exist 
+0000acb0: 7265 6d6f 7465 6c79 0a20 2020 2020 2020  remotely.       
+0000acc0: 2020 2020 2020 2020 2066 756c 6c5f 7061           full_pa
+0000acd0: 7468 203d 2073 656c 662e 736c 7572 6d5f  th = self.slurm_
+0000ace0: 7363 7269 7074 5f70 6174 682b 222f 222b  script_path+"/"+
+0000acf0: 6a6f 625f 7061 7468 0a20 2020 2020 2020  job_path.       
+0000ad00: 2020 2020 2020 2020 206a 6f62 5f64 6972           job_dir
+0000ad10: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
+0000ad20: 6c69 7428 6675 6c6c 5f70 6174 6829 0a20  lit(full_path). 
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ad40: 656c 662e 7275 6e28 6622 6d6b 6469 7220  elf.run(f"mkdir 
+0000ad50: 2d70 207b 6a6f 625f 6469 727d 2229 0a20  -p {job_dir}"). 
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000ad70: 2063 6f70 7920 746f 2072 656d 6f74 6520   copy to remote 
+0000ad80: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
+0000ad90: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+0000ada0: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
+0000adb0: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
+0000adc0: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
+0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ade0: 2020 2020 2020 2020 7265 6d6f 7465 3d66          remote=f
+0000adf0: 756c 6c5f 7061 7468 290a 2020 2020 2020  ull_path).      
+0000ae00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ae10: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
+0000ae20: 6574 5f75 7064 6174 655f 736c 7572 6d5f  et_update_slurm_
+0000ae30: 7363 7269 7074 735f 636f 6d6d 616e 6428  scripts_command(
+0000ae40: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+0000ae50: 6767 6572 2e69 6e66 6f28 2255 7064 6174  gger.info("Updat
+0000ae60: 696e 6720 536c 7572 6d20 6a6f 6220 7363  ing Slurm job sc
+0000ae70: 7269 7074 7320 6f6e 2053 6c75 726d 2229  ripts on Slurm")
+0000ae80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000ae90: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+0000aea0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
+0000aeb0: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
+0000aec0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0000aed0: 2020 2064 6566 2072 756e 5f77 6f72 6b66     def run_workf
+0000aee0: 6c6f 7728 7365 6c66 2c0a 2020 2020 2020  low(self,.      
+0000aef0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000af00: 6f72 6b66 6c6f 775f 6e61 6d65 3a20 7374  orkflow_name: st
+0000af10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000af20: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000af30: 5f76 6572 7369 6f6e 3a20 7374 722c 0a20  _version: str,. 
+0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af50: 2020 2020 696e 7075 745f 6461 7461 3a20      input_data: 
+0000af60: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000af70: 2020 2020 2020 2020 2020 656d 6169 6c3a            email:
+0000af80: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000af90: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000afa0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000afb0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000afc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000afd0: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+0000afe0: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
+0000aff0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+0000b000: 5475 706c 655b 5265 7375 6c74 2c20 696e  Tuple[Result, in
+0000b010: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
+0000b020: 2020 2020 2020 2020 5275 6e20 6120 7370          Run a sp
+0000b030: 6563 6966 6965 6420 776f 726b 666c 6f77  ecified workflow
+0000b040: 206f 6e20 536c 7572 6d20 7573 696e 6720   on Slurm using 
+0000b050: 7468 6520 6769 7665 6e20 7061 7261 6d65  the given parame
+0000b060: 7465 7273 2e0a 0a20 2020 2020 2020 2041  ters...        A
+0000b070: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000b080: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
+0000b090: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
+0000b0a0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
+0000b0b0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
+0000b0c0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+0000b0d0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
+0000b0e0: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
+0000b0f0: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
+0000b100: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
+0000b110: 2020 206f 6e20 536c 7572 6d29 2e0a 2020     on Slurm)..  
+0000b120: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000b130: 6461 7461 2028 7374 7229 3a20 4e61 6d65  data (str): Name
+0000b140: 206f 6620 7468 6520 696e 7075 7420 6461   of the input da
+0000b150: 7461 2066 6f6c 6465 7220 636f 6e74 6169  ta folder contai
+0000b160: 6e69 6e67 2069 6e70 7574 0a20 2020 2020  ning input.     
+0000b170: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0000b180: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
+0000b190: 2020 2020 656d 6169 6c20 2873 7472 2c20      email (str, 
+0000b1a0: 6f70 7469 6f6e 616c 293a 2045 6d61 696c  optional): Email
+0000b1b0: 2061 6464 7265 7373 2066 6f72 2053 6c75   address for Slu
+0000b1c0: 726d 206a 6f62 206e 6f74 6966 6963 6174  rm job notificat
+0000b1d0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+0000b1e0: 2020 7469 6d65 2028 7374 722c 206f 7074    time (str, opt
+0000b1f0: 696f 6e61 6c29 3a20 5469 6d65 206c 696d  ional): Time lim
+0000b200: 6974 2066 6f72 2074 6865 2053 6c75 726d  it for the Slurm
+0000b210: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
+0000b220: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000b230: 6d61 7420 4848 3a4d 4d3a 5353 2e0a 2020  mat HH:MM:SS..  
+0000b240: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000b250: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000b260: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000b270: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
+0000b280: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
+0000b290: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000b2a0: 2054 7570 6c65 5b52 6573 756c 742c 2069   Tuple[Result, i
+0000b2b0: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
+0000b2c0: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
+0000b2d0: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
+0000b2e0: 6c74 206f 6620 7374 6172 7469 6e67 2074  lt of starting t
+0000b2f0: 6865 2077 6f72 6b66 6c6f 7720 6a6f 6220  he workflow job 
+0000b300: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+0000b310: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
+0000b320: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
+0000b330: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
+0000b340: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
+0000b350: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
+0000b360: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000b370: 2053 6c75 726d 206a 6f62 2049 4420 6973   Slurm job ID is
+0000b380: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
+0000b390: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
+0000b3a0: 6520 0a20 2020 2020 2020 2020 2020 2060  e .            `
+0000b3b0: 7275 6e5f 636f 6d6d 616e 6473 6020 6d65  run_commands` me
+0000b3c0: 7468 6f64 2e0a 2020 2020 2020 2020 2222  thod..        ""
+0000b3d0: 220a 2020 2020 2020 2020 7362 6174 6368  ".        sbatch
+0000b3e0: 5f63 6d64 2c20 7362 6174 6368 5f65 6e76  _cmd, sbatch_env
+0000b3f0: 203d 2073 656c 662e 6765 745f 776f 726b   = self.get_work
+0000b400: 666c 6f77 5f63 6f6d 6d61 6e64 280a 2020  flow_command(.  
+0000b410: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000b420: 6f77 5f6e 616d 652c 2077 6f72 6b66 6c6f  ow_name, workflo
+0000b430: 775f 7665 7273 696f 6e2c 2069 6e70 7574  w_version, input
+0000b440: 5f64 6174 612c 2065 6d61 696c 2c20 7469  _data, email, ti
+0000b450: 6d65 2c20 2a2a 6b77 6172 6773 290a 2020  me, **kwargs).  
+0000b460: 2020 2020 2020 7072 696e 7428 6622 5275        print(f"Ru
+0000b470: 6e6e 696e 6720 7b77 6f72 6b66 6c6f 775f  nning {workflow_
+0000b480: 6e61 6d65 7d20 6a6f 6220 6f6e 207b 696e  name} job on {in
+0000b490: 7075 745f 6461 7461 7d20 6f6e 2053 6c75  put_data} on Slu
+0000b4a0: 726d 3a5c 0a20 2020 2020 2020 2020 2020  rm:\.           
+0000b4b0: 207b 7362 6174 6368 5f63 6d64 7d20 772f   {sbatch_cmd} w/
+0000b4c0: 207b 7362 6174 6368 5f65 6e76 7d22 290a   {sbatch_env}").
+0000b4d0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000b4e0: 6e66 6f28 6622 5275 6e6e 696e 6720 7b77  nfo(f"Running {w
+0000b4f0: 6f72 6b66 6c6f 775f 6e61 6d65 7d20 6a6f  orkflow_name} jo
+0000b500: 6220 6f6e 207b 696e 7075 745f 6461 7461  b on {input_data
+0000b510: 7d20 6f6e 2053 6c75 726d 2229 0a20 2020  } on Slurm").   
+0000b520: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+0000b530: 7275 6e5f 636f 6d6d 616e 6473 285b 7362  run_commands([sb
+0000b540: 6174 6368 5f63 6d64 5d2c 2073 6261 7463  atch_cmd], sbatc
+0000b550: 685f 656e 7629 0a20 2020 2020 2020 2072  h_env).        r
+0000b560: 6574 7572 6e20 7265 732c 2073 656c 662e  eturn res, self.
+0000b570: 6578 7472 6163 745f 6a6f 625f 6964 2872  extract_job_id(r
+0000b580: 6573 290a 0a20 2020 2064 6566 2072 756e  es)..    def run
+0000b590: 5f77 6f72 6b66 6c6f 775f 6a6f 6228 7365  _workflow_job(se
+0000b5a0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000b5b0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000b5c0: 6b66 6c6f 775f 6e61 6d65 3a20 7374 722c  kflow_name: str,
+0000b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5e0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000b5f0: 6f77 5f76 6572 7369 6f6e 3a20 7374 722c  ow_version: str,
+0000b600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b610: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000b620: 6461 7461 3a20 7374 722c 0a20 2020 2020  data: str,.     
+0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b640: 2020 2020 656d 6169 6c3a 204f 7074 696f      email: Optio
+0000b650: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000b660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b670: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
+0000b680: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000b690: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000b6a0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000b6b0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6d0: 2029 202d 3e20 536c 7572 6d4a 6f62 3a0a   ) -> SlurmJob:.
+0000b6e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b6f0: 2020 2020 5275 6e20 6120 7370 6563 6966      Run a specif
+0000b700: 6965 6420 776f 726b 666c 6f77 206f 6e20  ied workflow on 
+0000b710: 536c 7572 6d20 7573 696e 6720 7468 6520  Slurm using the 
+0000b720: 6769 7665 6e20 7061 7261 6d65 7465 7273  given parameters
+0000b730: 2061 6e64 2072 6574 7572 6e20 6120 536c   and return a Sl
+0000b740: 7572 6d4a 6f62 2069 6e73 7461 6e63 652e  urmJob instance.
+0000b750: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000b760: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000b770: 666c 6f77 5f6e 616d 6520 2873 7472 293a  flow_name (str):
+0000b780: 204e 616d 6520 6f66 2074 6865 2077 6f72   Name of the wor
+0000b790: 6b66 6c6f 7720 746f 2065 7865 6375 7465  kflow to execute
+0000b7a0: 2e0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+0000b7b0: 726b 666c 6f77 5f76 6572 7369 6f6e 2028  rkflow_version (
+0000b7c0: 7374 7229 3a20 5665 7273 696f 6e20 6f66  str): Version of
+0000b7d0: 2074 6865 2077 6f72 6b66 6c6f 7720 2869   the workflow (i
+0000b7e0: 6d61 6765 2076 6572 7369 6f6e 206f 6e20  mage version on 
+0000b7f0: 536c 7572 6d29 2e0a 2020 2020 2020 2020  Slurm)..        
+0000b800: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
+0000b810: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
+0000b820: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
+0000b830: 6465 7220 636f 6e74 6169 6e69 6e67 2069  der containing i
+0000b840: 6e70 7574 2069 6d61 6765 2066 696c 6573  nput image files
+0000b850: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+0000b860: 6169 6c20 2873 7472 2c20 6f70 7469 6f6e  ail (str, option
+0000b870: 616c 293a 2045 6d61 696c 2061 6464 7265  al): Email addre
+0000b880: 7373 2066 6f72 2053 6c75 726d 206a 6f62  ss for Slurm job
+0000b890: 206e 6f74 6966 6963 6174 696f 6e73 2e0a   notifications..
+0000b8a0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000b8b0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+0000b8c0: 3a20 5469 6d65 206c 696d 6974 2066 6f72  : Time limit for
+0000b8d0: 2074 6865 2053 6c75 726d 206a 6f62 2069   the Slurm job i
+0000b8e0: 6e20 7468 6520 666f 726d 6174 2048 483a  n the format HH:
+0000b8f0: 4d4d 3a53 532e 0a20 2020 2020 2020 2020  MM:SS..         
+0000b900: 2020 202a 2a6b 7761 7267 733a 2041 6464     **kwargs: Add
+0000b910: 6974 696f 6e61 6c20 6b65 7977 6f72 6420  itional keyword 
+0000b920: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
+0000b930: 6520 776f 726b 666c 6f77 2e0a 0a20 2020  e workflow...   
+0000b940: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000b950: 2020 2020 2020 2020 2020 536c 7572 6d4a            SlurmJ
+0000b960: 6f62 3a20 4120 536c 7572 6d4a 6f62 2069  ob: A SlurmJob i
+0000b970: 6e73 7461 6e63 6520 7265 7072 6573 656e  nstance represen
+0000b980: 7469 6e67 2074 6865 2073 7461 7274 6564  ting the started
+0000b990: 2077 6f72 6b66 6c6f 7720 6a6f 622e 0a20   workflow job.. 
+0000b9a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000b9b0: 2020 2072 6573 756c 742c 206a 6f62 5f69     result, job_i
+0000b9c0: 6420 3d20 7365 6c66 2e72 756e 5f77 6f72  d = self.run_wor
+0000b9d0: 6b66 6c6f 7728 0a20 2020 2020 2020 2020  kflow(.         
+0000b9e0: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
+0000b9f0: 2c20 776f 726b 666c 6f77 5f76 6572 7369  , workflow_versi
+0000ba00: 6f6e 2c20 696e 7075 745f 6461 7461 2c20  on, input_data, 
+0000ba10: 656d 6169 6c2c 2074 696d 652c 202a 2a6b  email, time, **k
+0000ba20: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
+0000ba30: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
+0000ba40: 6573 756c 742c 206a 6f62 5f69 6429 0a0a  esult, job_id)..
+0000ba50: 2020 2020 6465 6620 7275 6e5f 636f 6e76      def run_conv
+0000ba60: 6572 7369 6f6e 5f77 6f72 6b66 6c6f 775f  ersion_workflow_
+0000ba70: 6a6f 6228 7365 6c66 2c20 666f 6c64 6572  job(self, folder
+0000ba80: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 736f 7572 6365 5f66 6f72 6d61 743a 2073  source_format: s
+0000bac0: 7472 203d 2027 7a61 7272 272c 0a20 2020  tr = 'zarr',.   
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baf0: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
+0000bb00: 7374 7220 3d20 2774 6966 6627 0a20 2020  str = 'tiff'.   
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2029 202d 3e20 5475 706c 655b 5265 7375   ) -> Tuple[Resu
+0000bb40: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
+0000bb50: 2020 2222 220a 2020 2020 2020 2020 5275    """.        Ru
+0000bb60: 6e20 7468 6520 6461 7461 2063 6f6e 7665  n the data conve
+0000bb70: 7273 696f 6e20 776f 726b 666c 6f77 206f  rsion workflow o
+0000bb80: 6e20 536c 7572 6d20 7573 696e 6720 7468  n Slurm using th
+0000bb90: 6520 6769 7665 6e20 6461 7461 2066 6f6c  e given data fol
+0000bba0: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
+0000bbb0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000bbc0: 666f 6c64 6572 5f6e 616d 6520 2873 7472  folder_name (str
+0000bbd0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+0000bbe0: 6865 2064 6174 6120 666f 6c64 6572 2063  he data folder c
+0000bbf0: 6f6e 7461 696e 696e 6720 736f 7572 6365  ontaining source
+0000bc00: 2066 6f72 6d61 7420 6669 6c65 732e 0a20   format files.. 
+0000bc10: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+0000bc20: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
+0000bc30: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
+0000bc40: 6174 2066 6f72 2063 6f6e 7665 7273 696f  at for conversio
+0000bc50: 6e20 2864 6566 6175 6c74 2069 7320 277a  n (default is 'z
+0000bc60: 6172 7227 292e 0a20 2020 2020 2020 2020  arr')..         
+0000bc70: 2020 2074 6172 6765 745f 666f 726d 6174     target_format
+0000bc80: 2028 7374 7229 3a20 5461 7267 6574 2064   (str): Target d
+0000bc90: 6174 6120 666f 726d 6174 2061 6674 6572  ata format after
+0000bca0: 2063 6f6e 7665 7273 696f 6e20 2864 6566   conversion (def
+0000bcb0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
+0000bcc0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000bcd0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+0000bce0: 7570 6c65 5b52 6573 756c 742c 2069 6e74  uple[Result, int
+0000bcf0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000bd00: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+0000bd10: 696e 696e 6720 7468 6520 7265 7375 6c74  ining the result
+0000bd20: 206f 6620 7374 6172 7469 6e67 2074 6865   of starting the
+0000bd30: 2063 6f6e 7665 7273 696f 6e20 6a6f 6220   conversion job 
+0000bd40: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+0000bd50: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
+0000bd60: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
+0000bd70: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
+0000bd80: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
+0000bd90: 2e0a 0a20 2020 2020 2020 2057 6172 6e69  ...        Warni
+0000bda0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+0000bdb0: 5468 6520 6465 6661 756c 7420 696d 706c  The default impl
+0000bdc0: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
+0000bdd0: 7375 7070 6f72 7473 2063 6f6e 7665 7273  supports convers
+0000bde0: 696f 6e20 6672 6f6d 2027 7a61 7272 2720  ion from 'zarr' 
+0000bdf0: 746f 2027 7469 6666 272e 0a20 2020 2020  to 'tiff'..     
+0000be00: 2020 2020 2020 2049 6620 7573 696e 6720         If using 
+0000be10: 6f74 6865 7220 736f 7572 6365 206f 7220  other source or 
+0000be20: 7461 7267 6574 2066 6f72 6d61 7473 2c20  target formats, 
+0000be30: 7573 6572 7320 6d75 7374 2069 6d70 6c65  users must imple
+0000be40: 6d65 6e74 2061 6e64 2063 6f6e 6669 6775  ment and configu
+0000be50: 7265 0a20 2020 2020 2020 2020 2020 2061  re.            a
+0000be60: 6464 6974 696f 6e61 6c20 636f 6e76 6572  dditional conver
+0000be70: 7465 7273 2074 6865 6d73 656c 7665 732e  ters themselves.
+0000be80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000be90: 2020 2020 2023 2047 656e 6572 6174 6520       # Generate 
+0000bea0: 6120 756e 6971 7565 2063 6f6e 6669 6720  a unique config 
+0000beb0: 6669 6c65 206e 616d 650a 2020 2020 2020  file name.      
+0000bec0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
+0000bed0: 6622 636f 6e66 6967 5f7b 666f 6c64 6572  f"config_{folder
+0000bee0: 5f6e 616d 657d 2e74 7874 220a 0a20 2020  _name}.txt"..   
+0000bef0: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
+0000bf00: 2061 6c6c 2063 6f6d 6d61 6e64 7320 746f   all commands to
+0000bf10: 2072 756e 2063 6f6e 7365 6375 7469 7665   run consecutive
+0000bf20: 6c79 0a20 2020 2020 2020 2064 6174 615f  ly.        data_
+0000bf30: 7061 7468 203d 2066 227b 7365 6c66 2e73  path = f"{self.s
+0000bf40: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
+0000bf50: 7b66 6f6c 6465 725f 6e61 6d65 7d22 0a20  {folder_name}". 
+0000bf60: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
+0000bf70: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
+0000bf80: 7620 3d20 7365 6c66 2e67 6574 5f63 6f6e  v = self.get_con
+0000bf90: 7665 7273 696f 6e5f 636f 6d6d 616e 6428  version_command(
+0000bfa0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000bfb0: 615f 7061 7468 2c20 636f 6e66 6967 5f66  a_path, config_f
+0000bfc0: 696c 652c 2073 6f75 7263 655f 666f 726d  ile, source_form
+0000bfd0: 6174 2c20 7461 7267 6574 5f66 6f72 6d61  at, target_forma
+0000bfe0: 7429 0a20 2020 2020 2020 2063 6f6d 6d61  t).        comma
+0000bff0: 6e64 7320 3d20 5b0a 2020 2020 2020 2020  nds = [.        
+0000c000: 2020 2020 6622 6669 6e64 207b 6461 7461      f"find {data
+0000c010: 5f70 6174 687d 2f64 6174 612f 696e 202d  _path}/data/in -
+0000c020: 6e61 6d65 2027 2a2e 7b73 6f75 7263 655f  name '*.{source_
+0000c030: 666f 726d 6174 7d27 207c 2061 776b 2027  format}' | awk '
+0000c040: 7b7b 7072 696e 7420 4e52 2c20 2430 7d7d  {{print NR, $0}}
+0000c050: 2720 3e20 7b63 6f6e 6669 675f 6669 6c65  ' > {config_file
+0000c060: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+0000c070: 6622 4e3d 2428 7763 202d 6c20 3c20 5c22  f"N=$(wc -l < \"
+0000c080: 7b63 6f6e 6669 675f 6669 6c65 7d5c 2229  {config_file}\")
+0000c090: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+0000c0a0: 2265 6368 6f20 5c22 4e75 6d62 6572 206f  "echo \"Number o
+0000c0b0: 6620 2e7b 736f 7572 6365 5f66 6f72 6d61  f .{source_forma
+0000c0c0: 747d 2066 696c 6573 3a20 244e 5c22 222c  t} files: $N\"",
+0000c0d0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000c0e0: 7665 7273 696f 6e5f 636d 640a 2020 2020  version_cmd.    
+0000c0f0: 2020 2020 5d0a 0a20 2020 2020 2020 2023      ]..        #
+0000c100: 2052 756e 2061 6c6c 2063 6f6d 6d61 6e64   Run all command
+0000c110: 7320 636f 6e73 6563 7574 6976 656c 790a  s consecutively.
+0000c120: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+0000c130: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+0000c140: 636f 6d6d 616e 6473 2c20 7362 6174 6368  commands, sbatch
+0000c150: 5f65 6e76 290a 0a20 2020 2020 2020 2072  _env)..        r
+0000c160: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
+0000c170: 6573 2c20 7365 6c66 2e65 7874 7261 6374  es, self.extract
+0000c180: 5f6a 6f62 5f69 6428 7265 7329 290a 0a20  _job_id(res)).. 
+0000c190: 2020 2064 6566 2065 7874 7261 6374 5f6a     def extract_j
+0000c1a0: 6f62 5f69 6428 7365 6c66 2c20 7265 7375  ob_id(self, resu
+0000c1b0: 6c74 3a20 5265 7375 6c74 2920 2d3e 2069  lt: Result) -> i
+0000c1c0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+0000c1d0: 2020 2020 2020 2020 4578 7472 6163 7420          Extract 
+0000c1e0: 7468 6520 536c 7572 6d20 6a6f 6220 4944  the Slurm job ID
+0000c1f0: 2066 726f 6d20 7468 6520 7265 7375 6c74   from the result
+0000c200: 206f 6620 6120 636f 6d6d 616e 642e 0a0a   of a command...
+0000c210: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000c220: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000c230: 2028 5265 7375 6c74 293a 2054 6865 2072   (Result): The r
+0000c240: 6573 756c 7420 6f66 2061 2063 6f6d 6d61  esult of a comma
+0000c250: 6e64 2065 7865 6375 7469 6f6e 2e0a 0a20  nd execution... 
+0000c260: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000c270: 2020 2020 2020 2020 2020 2020 696e 743a              int:
+0000c280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c290: 2054 6865 2053 6c75 726d 206a 6f62 2049   The Slurm job I
+0000c2a0: 4420 6578 7472 6163 7465 6420 6672 6f6d  D extracted from
+0000c2b0: 2074 6865 2072 6573 756c 742c 0a20 2020   the result,.   
+0000c2c0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000c2d0: 2d31 2069 6620 6e6f 7420 666f 756e 642e  -1 if not found.
+0000c2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c2f0: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+0000c300: 6420 3d20 6e65 7874 2828 696e 7428 732e  d = next((int(s.
+0000c310: 7374 7269 7028 2929 2066 6f72 2073 2069  strip()) for s i
+0000c320: 6e20 7265 7375 6c74 2e73 7464 6f75 742e  n result.stdout.
+0000c330: 7370 6c69 7428 0a20 2020 2020 2020 2020  split(.         
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 2020 2022 5375 626d 6974 7465 6420 6261     "Submitted ba
+0000c360: 7463 6820 6a6f 6222 2920 6966 2073 2e73  tch job") if s.s
+0000c370: 7472 6970 2829 2e69 7364 6967 6974 2829  trip().isdigit()
+0000c380: 292c 202d 3129 0a20 2020 2020 2020 2072  ), -1).        r
+0000c390: 6574 7572 6e20 736c 7572 6d5f 6a6f 625f  eturn slurm_job_
+0000c3a0: 6964 0a0a 2020 2020 6465 6620 6765 745f  id..    def get_
+0000c3b0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
+0000c3c0: 6970 7473 5f63 6f6d 6d61 6e64 2873 656c  ipts_command(sel
+0000c3d0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+0000c3e0: 2020 2022 2222 4765 6e65 7261 7465 2074     """Generate t
+0000c3f0: 6865 2063 6f6d 6d61 6e64 2074 6f20 7570  he command to up
+0000c400: 6461 7465 2074 6865 2047 6974 2072 6570  date the Git rep
+0000c410: 6f73 6974 6f72 7920 636f 6e74 6169 6e69  ository containi
+0000c420: 6e67 0a20 2020 2020 2020 2074 6865 2053  ng.        the S
+0000c430: 6c75 726d 2073 6372 6970 7473 2c20 6966  lurm scripts, if
+0000c440: 206e 6563 6573 7361 7279 2e0a 0a20 2020   necessary...   
+0000c450: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000c460: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
+0000c470: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0000c480: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
+0000c490: 6e67 2074 6865 2047 6974 2063 6f6d 6d61  ng the Git comma
+0000c4a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0000c4b0: 2020 2074 6f20 7570 6461 7465 2074 6865     to update the
+0000c4c0: 2053 6c75 726d 2073 6372 6970 7473 2e0a   Slurm scripts..
+0000c4d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c4e0: 2020 2020 7570 6461 7465 5f63 6d64 203d      update_cmd =
+0000c4f0: 2066 2267 6974 202d 4320 7b73 656c 662e   f"git -C {self.
+0000c500: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
+0000c510: 687d 2070 756c 6c22 0a20 2020 2020 2020  h} pull".       
+0000c520: 2072 6574 7572 6e20 7570 6461 7465 5f63   return update_c
+0000c530: 6d64 0a0a 2020 2020 6465 6620 6368 6563  md..    def chec
+0000c540: 6b5f 6a6f 625f 7374 6174 7573 2873 656c  k_job_status(sel
+0000c550: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000c560: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+0000c570: 6d5f 6a6f 625f 6964 733a 204c 6973 745b  m_job_ids: List[
+0000c580: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000c5a0: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
+0000c5b0: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
+0000c5c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000c5d0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+0000c5e0: 3e20 5475 706c 655b 4469 6374 5b69 6e74  > Tuple[Dict[int
+0000c5f0: 2c20 7374 725d 2c20 5265 7375 6c74 5d3a  , str], Result]:
+0000c600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c610: 2020 2020 2043 6865 636b 2074 6865 2073       Check the s
+0000c620: 7461 7475 7320 6f66 2053 6c75 726d 206a  tatus of Slurm j
+0000c630: 6f62 7320 7769 7468 2074 6865 2067 6976  obs with the giv
+0000c640: 656e 206a 6f62 2049 4473 2e0a 0a20 2020  en job IDs...   
+0000c650: 2020 2020 204e 6f74 653a 2054 6869 7320       Note: This 
+0000c660: 646f 6573 6e27 7420 7265 7475 726e 206a  doesn't return j
+0000c670: 6f62 2061 7272 6179 7320 696e 6469 7669  ob arrays indivi
+0000c680: 6475 616c 6c79 2e0a 2020 2020 2020 2020  dually..        
+0000c690: 4974 2074 616b 6573 2074 6865 206c 6173  It takes the las
+0000c6a0: 7420 7661 6c75 6520 7265 7475 726e 6564  t value returned
+0000c6b0: 2066 6f72 2074 686f 7365 2073 7562 2069   for those sub i
+0000c6c0: 6473 200a 2020 2020 2020 2020 2867 656e  ds .        (gen
+0000c6d0: 6572 616c 6c79 2074 6865 206f 6e65 2073  erally the one s
+0000c6e0: 7469 6c6c 2050 454e 4449 4e47 292e 0a0a  till PENDING)...
+0000c6f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000c700: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+0000c710: 6a6f 625f 6964 7320 284c 6973 745b 696e  job_ids (List[in
+0000c720: 745d 293a 2054 6865 206a 6f62 2049 4473  t]): The job IDs
+0000c730: 206f 6620 7468 6520 536c 7572 6d20 6a6f   of the Slurm jo
+0000c740: 6273 2074 6f20 6368 6563 6b2e 0a20 2020  bs to check..   
+0000c750: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+0000c760: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+0000c770: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+0000c780: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+0000c790: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
+0000c7a0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
+0000c7b0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
+0000c7c0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
+0000c7d0: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
+0000c7e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000c7f0: 2020 2020 2020 2020 2054 7570 6c65 5b44           Tuple[D
+0000c800: 6963 745b 696e 742c 2073 7472 5d2c 2052  ict[int, str], R
+0000c810: 6573 756c 745d 3a0a 2020 2020 2020 2020  esult]:.        
+0000c820: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+0000c830: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
+0000c840: 7461 7475 7320 7065 7220 696e 7075 7420  tatus per input 
+0000c850: 4944 2061 6e64 2074 6865 2072 6573 756c  ID and the resul
+0000c860: 7420 6f66 200a 2020 2020 2020 2020 2020  t of .          
+0000c870: 2020 2020 2020 7468 6520 636f 6d6d 616e        the comman
+0000c880: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
+0000c890: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+0000c8a0: 2020 2020 2020 2020 2020 5353 4845 7863            SSHExc
+0000c8b0: 6570 7469 6f6e 3a20 4966 2074 6865 2063  eption: If the c
+0000c8c0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
+0000c8d0: 2066 6169 6c73 206f 7220 6e6f 2072 6573   fails or no res
+0000c8e0: 706f 6e73 6520 6973 0a20 2020 2020 2020  ponse is.       
+0000c8f0: 2020 2020 2020 2020 2072 6563 6569 7665           receive
+0000c900: 6420 6166 7465 7220 6d75 6c74 6970 6c65  d after multiple
+0000c910: 2072 6574 7269 6573 2e0a 2020 2020 2020   retries..      
+0000c920: 2020 2222 220a 2020 2020 2020 2020 636d    """.        cm
+0000c930: 6420 3d20 7365 6c66 2e67 6574 5f6a 6f62  d = self.get_job
+0000c940: 5f73 7461 7475 735f 636f 6d6d 616e 6428  _status_command(
+0000c950: 736c 7572 6d5f 6a6f 625f 6964 7329 0a20  slurm_job_ids). 
+0000c960: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000c970: 666f 2866 2247 6574 7469 6e67 2073 7461  fo(f"Getting sta
+0000c980: 7475 7320 6f66 207b 736c 7572 6d5f 6a6f  tus of {slurm_jo
+0000c990: 625f 6964 737d 206f 6e20 536c 7572 6d22  b_ids} on Slurm"
+0000c9a0: 290a 2020 2020 2020 2020 7265 7472 795f  ).        retry_
+0000c9b0: 7374 6174 7573 203d 2030 0a20 2020 2020  status = 0.     
+0000c9c0: 2020 2077 6869 6c65 2072 6574 7279 5f73     while retry_s
+0000c9d0: 7461 7475 7320 3c20 333a 0a20 2020 2020  tatus < 3:.     
+0000c9e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000c9f0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+0000ca00: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
+0000ca10: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+0000ca20: 6767 6572 2e69 6e66 6f28 7265 7375 6c74  gger.info(result
+0000ca30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000ca40: 2072 6573 756c 742e 6f6b 3a0a 2020 2020   result.ok:.    
+0000ca50: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000ca60: 6f74 2072 6573 756c 742e 7374 646f 7574  ot result.stdout
+0000ca70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ca80: 2020 2020 2020 2320 7761 6974 2066 6f72        # wait for
+0000ca90: 2033 2073 6563 6f6e 6473 2062 6566 6f72   3 seconds befor
+0000caa0: 6520 6368 6563 6b69 6e67 2061 6761 696e  e checking again
+0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cac0: 2020 2020 2074 696d 6573 6c65 6570 2e73       timesleep.s
+0000cad0: 6c65 6570 2833 290a 2020 2020 2020 2020  leep(3).        
+0000cae0: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+0000caf0: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
+0000cb00: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
+0000cb10: 6174 7573 202b 3d20 310a 2020 2020 2020  atus += 1.      
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000cb30: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb50: 2020 2020 6622 5265 7472 7920 7b72 6574      f"Retry {ret
+0000cb60: 7279 5f73 7461 7475 737d 2067 6574 7469  ry_status} getti
+0000cb70: 6e67 2073 7461 7475 7320 5c0a 2020 2020  ng status \.    
+0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb90: 2020 2020 2020 2020 6f66 207b 736c 7572          of {slur
+0000cba0: 6d5f 6a6f 625f 6964 737d 2122 290a 2020  m_job_ids}!").  
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000cbc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000cbd0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
+0000cbf0: 625f 7374 6174 7573 5f64 6963 7420 3d20  b_status_dict = 
+0000cc00: 7b69 6e74 286c 696e 652e 7370 6c69 7428  {int(line.split(
+0000cc10: 295b 305d 2e73 706c 6974 2827 5f27 295b  )[0].split('_')[
+0000cc20: 305d 293a 206c 696e 652e 7370 6c69 7428  0]): line.split(
+0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc40: 2020 2020 2029 5b31 5d20 666f 7220 6c69       )[1] for li
+0000cc50: 6e65 2069 6e20 7265 7375 6c74 2e73 7464  ne in result.std
+0000cc60: 6f75 742e 7370 6c69 7428 225c 6e22 2920  out.split("\n") 
+0000cc70: 6966 206c 696e 657d 0a20 2020 2020 2020  if line}.       
+0000cc80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000cc90: 6765 722e 6465 6275 6728 6622 4a6f 6220  ger.debug(f"Job 
+0000cca0: 7374 6174 7573 6573 3a20 7b6a 6f62 5f73  statuses: {job_s
+0000ccb0: 7461 7475 735f 6469 6374 7d22 290a 2020  tatus_dict}").  
+0000ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccd0: 2020 7265 7475 726e 206a 6f62 5f73 7461    return job_sta
+0000cce0: 7475 735f 6469 6374 2c20 7265 7375 6c74  tus_dict, result
+0000ccf0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000cd00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000cd10: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
+0000cd20: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
+0000cd30: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
+0000cd40: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000cd50: 6572 726f 7228 6572 726f 7229 0a20 2020  error(error).   
+0000cd60: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000cd70: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
+0000cd80: 6572 726f 7229 0a20 2020 2020 2020 2065  error).        e
+0000cd90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000cda0: 2065 7272 6f72 203d 2066 2245 7272 6f72   error = f"Error
+0000cdb0: 3a20 5265 7472 6965 6420 7b72 6574 7279  : Retried {retry
+0000cdc0: 5f73 7461 7475 737d 2074 696d 6573 2074  _status} times t
+0000cdd0: 6f20 6765 7420 5c0a 2020 2020 2020 2020  o get \.        
+0000cde0: 2020 2020 2020 2020 7374 6174 7573 206f          status o
+0000cdf0: 6620 7b73 6c75 726d 5f6a 6f62 5f69 6473  f {slurm_job_ids
+0000ce00: 7d2c 2062 7574 206e 6f20 7265 7370 6f6e  }, but no respon
+0000ce10: 7365 2e22 0a20 2020 2020 2020 2020 2020  se.".           
+0000ce20: 206c 6f67 6765 722e 6572 726f 7228 6572   logger.error(er
+0000ce30: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+0000ce40: 2072 6169 7365 2053 5348 4578 6365 7074   raise SSHExcept
+0000ce50: 696f 6e28 6572 726f 7229 0a0a 2020 2020  ion(error)..    
+0000ce60: 6465 6620 6765 745f 6a6f 625f 7374 6174  def get_job_stat
+0000ce70: 7573 5f63 6f6d 6d61 6e64 2873 656c 662c  us_command(self,
+0000ce80: 2073 6c75 726d 5f6a 6f62 5f69 6473 3a20   slurm_job_ids: 
+0000ce90: 4c69 7374 5b69 6e74 5d29 202d 3e20 7374  List[int]) -> st
+0000cea0: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+0000ceb0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+0000cec0: 6520 536c 7572 6d20 636f 6d6d 616e 6420  e Slurm command 
+0000ced0: 746f 2067 6574 2074 6865 2073 7461 7475  to get the statu
+0000cee0: 7320 6f66 206a 6f62 7320 7769 7468 2074  s of jobs with t
+0000cef0: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
+0000cf00: 206a 6f62 2049 4473 2e0a 0a20 2020 2020   job IDs...     
+0000cf10: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000cf20: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+0000cf30: 6473 2028 4c69 7374 5b69 6e74 5d29 3a20  ds (List[int]): 
+0000cf40: 5468 6520 6a6f 6220 4944 7320 6f66 2074  The job IDs of t
+0000cf50: 6865 206a 6f62 7320 746f 2063 6865 636b  he jobs to check
+0000cf60: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000cf70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000cf80: 7374 723a 200a 2020 2020 2020 2020 2020  str: .          
+0000cf90: 2020 2020 2020 5468 6520 536c 7572 6d20        The Slurm 
+0000cfa0: 636f 6d6d 616e 6420 746f 2067 6574 2074  command to get t
+0000cfb0: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
+0000cfc0: 206a 6f62 732e 0a20 2020 2020 2020 2022   jobs..        "
+0000cfd0: 2222 0a20 2020 2020 2020 2023 2063 6f6e  "".        # con
+0000cfe0: 6361 7420 6d75 6c74 6970 6c65 206a 6f62  cat multiple job
+0000cff0: 7320 6966 206e 6565 6465 640a 2020 2020  s if needed.    
+0000d000: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
+0000d010: 203d 2022 202d 6a20 222e 6a6f 696e 285b   = " -j ".join([
+0000d020: 7374 7228 6964 2920 666f 7220 6964 2069  str(id) for id i
+0000d030: 6e20 736c 7572 6d5f 6a6f 625f 6964 735d  n slurm_job_ids]
+0000d040: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d050: 2073 656c 662e 5f4a 4f42 5f53 5441 5455   self._JOB_STATU
+0000d060: 535f 434d 442e 666f 726d 6174 2873 6c75  S_CMD.format(slu
+0000d070: 726d 5f6a 6f62 5f69 643d 736c 7572 6d5f  rm_job_id=slurm_
+0000d080: 6a6f 625f 6964 290a 0a20 2020 2064 6566  job_id)..    def
+0000d090: 2065 7874 7261 6374 5f64 6174 615f 6c6f   extract_data_lo
+0000d0a0: 6361 7469 6f6e 5f66 726f 6d5f 6c6f 6728  cation_from_log(
+0000d0b0: 7365 6c66 2c20 736c 7572 6d5f 6a6f 625f  self, slurm_job_
+0000d0c0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2020 2020 206c 6f67 6669 6c65 3a20         logfile: 
+0000d100: 7374 7220 3d20 4e6f 6e65 2920 2d3e 2073  str = None) -> s
+0000d110: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
+0000d120: 6561 6420 534c 5552 4d20 6a6f 6220 6c6f  ead SLURM job lo
+0000d130: 6766 696c 6520 746f 2066 696e 6420 6c6f  gfile to find lo
+0000d140: 6361 7469 6f6e 206f 6620 7468 6520 6461  cation of the da
+0000d150: 7461 2e0a 0a20 2020 2020 2020 204f 6e65  ta...        One
+0000d160: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
+0000d170: 7273 2069 7320 7265 7175 6972 6564 2c20  rs is required, 
+0000d180: 6569 7468 6572 2069 6420 6f72 2066 696c  either id or fil
+0000d190: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+0000d1a0: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
+0000d1b0: 7572 6d5f 6a6f 625f 6964 2028 7374 7229  urm_job_id (str)
+0000d1c0: 3a20 4964 206f 6620 7468 6520 736c 7572  : Id of the slur
+0000d1d0: 6d20 6a6f 620a 2020 2020 2020 2020 2020  m job.          
+0000d1e0: 2020 6c6f 6766 696c 6520 2873 7472 293a    logfile (str):
+0000d1f0: 2050 6174 6820 746f 2074 6865 206c 6f67   Path to the log
+0000d200: 6669 6c65 0a0a 2020 2020 2020 2020 5265  file..        Re
+0000d210: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000d220: 2020 2073 7472 3a20 4461 7461 206c 6f63     str: Data loc
+0000d230: 6174 696f 6e20 6163 636f 7264 696e 6720  ation according 
+0000d240: 746f 2074 6865 206c 6f67 0a0a 2020 2020  to the log..    
+0000d250: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000d260: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
+0000d270: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
+0000d280: 7320 616e 2069 7373 7565 2077 6974 6820  s an issue with 
+0000d290: 7468 6520 636f 6d6d 616e 6420 6578 6563  the command exec
+0000d2a0: 7574 696f 6e2e 0a20 2020 2020 2020 2022  ution..        "
+0000d2b0: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
+0000d2c0: 6766 696c 6520 6973 204e 6f6e 6520 616e  gfile is None an
+0000d2d0: 6420 736c 7572 6d5f 6a6f 625f 6964 2069  d slurm_job_id i
+0000d2e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000d2f0: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
+0000d300: 3d20 7365 6c66 2e5f 4c4f 4746 494c 450a  = self._LOGFILE.
+0000d310: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
+0000d320: 696c 6520 3d20 6c6f 6766 696c 652e 666f  ile = logfile.fo
+0000d330: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
+0000d340: 643d 736c 7572 6d5f 6a6f 625f 6964 290a  d=slurm_job_id).
+0000d350: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+0000d360: 6c66 2e5f 4c4f 4746 494c 455f 4441 5441  lf._LOGFILE_DATA
+0000d370: 5f43 4d44 2e66 6f72 6d61 7428 6c6f 675f  _CMD.format(log_
+0000d380: 6669 6c65 3d6c 6f67 6669 6c65 290a 2020  file=logfile).  
+0000d390: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d3a0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+0000d3b0: 285b 636d 645d 290a 2020 2020 2020 2020  ([cmd]).        
+0000d3c0: 6966 2072 6573 756c 742e 6f6b 3a0a 2020  if result.ok:.  
+0000d3d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d3e0: 2072 6573 756c 742e 7374 646f 7574 0a20   result.stdout. 
+0000d3f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000d400: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+0000d410: 5348 4578 6365 7074 696f 6e28 7265 7375  SHException(resu
+0000d420: 6c74 290a 0a20 2020 2064 6566 2067 6574  lt)..    def get
+0000d430: 5f77 6f72 6b66 6c6f 775f 7061 7261 6d65  _workflow_parame
+0000d440: 7465 7273 2873 656c 662c 0a20 2020 2020  ters(self,.     
+0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d460: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000d470: 6c6f 773a 2073 7472 2920 2d3e 2044 6963  low: str) -> Dic
+0000d480: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
+0000d490: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
+0000d4a0: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
+0000d4b0: 6965 7665 2074 6865 2070 6172 616d 6574  ieve the paramet
+0000d4c0: 6572 7320 6f66 2061 2077 6f72 6b66 6c6f  ers of a workflo
+0000d4d0: 772e 0a0a 2020 2020 2020 2020 4172 6773  w...        Args
+0000d4e0: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
+0000d4f0: 726b 666c 6f77 2028 7374 7229 3a20 5468  rkflow (str): Th
+0000d500: 6520 776f 726b 666c 6f77 2066 6f72 2077  e workflow for w
+0000d510: 6869 6368 2074 6f20 7265 7472 6965 7665  hich to retrieve
+0000d520: 2074 6865 2070 6172 616d 6574 6572 732e   the parameters.
+0000d530: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000d540: 733a 0a20 2020 2020 2020 2020 2020 2044  s:.            D
+0000d550: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
+0000d560: 722c 2041 6e79 5d5d 3a0a 2020 2020 2020  r, Any]]:.      
+0000d570: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
+0000d580: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+0000d590: 6720 7468 6520 776f 726b 666c 6f77 2070  g the workflow p
+0000d5a0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+0000d5b0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000d5c0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+0000d5d0: 6f72 3a20 4966 2061 6e20 6572 726f 7220  or: If an error 
+0000d5e0: 6f63 6375 7273 2077 6869 6c65 2072 6574  occurs while ret
+0000d5f0: 7269 6576 696e 6720 7468 6520 776f 726b  rieving the work
+0000d600: 666c 6f77 0a20 2020 2020 2020 2020 2020  flow.           
+0000d610: 2020 2020 2070 6172 616d 6574 6572 732e       parameters.
+0000d620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d630: 2020 2020 206a 736f 6e5f 6465 7363 7269       json_descri
+0000d640: 7074 6f72 203d 2073 656c 662e 7075 6c6c  ptor = self.pull
+0000d650: 5f64 6573 6372 6970 746f 725f 6672 6f6d  _descriptor_from
+0000d660: 5f67 6974 6875 6228 776f 726b 666c 6f77  _github(workflow
+0000d670: 290a 2020 2020 2020 2020 2320 636f 6e76  ).        # conv
+0000d680: 6572 7420 746f 206f 6d65 726f 2074 7970  ert to omero typ
+0000d690: 6573 0a20 2020 2020 2020 206c 6f67 6765  es.        logge
+0000d6a0: 722e 6465 6275 6728 6a73 6f6e 5f64 6573  r.debug(json_des
+0000d6b0: 6372 6970 746f 7229 0a20 2020 2020 2020  criptor).       
+0000d6c0: 2077 6f72 6b66 6c6f 775f 6469 6374 203d   workflow_dict =
+0000d6d0: 207b 7d0a 2020 2020 2020 2020 666f 7220   {}.        for 
+0000d6e0: 696e 7075 7420 696e 206a 736f 6e5f 6465  input in json_de
+0000d6f0: 7363 7269 7074 6f72 5b27 696e 7075 7473  scriptor['inputs
+0000d700: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0000d710: 2320 6669 6c74 6572 2063 7974 6f6d 696e  # filter cytomin
+0000d720: 6520 7061 7261 6d65 7465 7273 0a20 2020  e parameters.   
+0000d730: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000d740: 696e 7075 745b 2769 6427 5d2e 7374 6172  input['id'].star
+0000d750: 7473 7769 7468 2827 6379 746f 6d69 6e65  tswith('cytomine
+0000d760: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000d770: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
+0000d780: 616d 7320 3d20 7b7d 0a20 2020 2020 2020  ams = {}.       
+0000d790: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000d7a0: 775f 7061 7261 6d73 5b27 6e61 6d65 275d  w_params['name']
+0000d7b0: 203d 2069 6e70 7574 5b27 6964 275d 0a20   = input['id']. 
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000d7d0: 6f72 6b66 6c6f 775f 7061 7261 6d73 5b27  orkflow_params['
+0000d7e0: 6465 6661 756c 7427 5d20 3d20 696e 7075  default'] = inpu
+0000d7f0: 745b 2764 6566 6175 6c74 2d76 616c 7565  t['default-value
+0000d800: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000d810: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
+0000d820: 6d73 5b27 6379 7479 7065 275d 203d 2069  ms['cytype'] = i
+0000d830: 6e70 7574 5b27 7479 7065 275d 0a20 2020  nput['type'].   
+0000d840: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000d850: 6b66 6c6f 775f 7061 7261 6d73 5b27 6f70  kflow_params['op
+0000d860: 7469 6f6e 616c 275d 203d 2069 6e70 7574  tional'] = input
+0000d870: 5b27 6f70 7469 6f6e 616c 275d 0a20 2020  ['optional'].   
+0000d880: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+0000d890: 5f66 6c61 6720 3d20 696e 7075 745b 2763  _flag = input['c
+0000d8a0: 6f6d 6d61 6e64 2d6c 696e 652d 666c 6167  ommand-line-flag
+0000d8b0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000d8c0: 2020 2063 6d64 5f66 6c61 6720 3d20 636d     cmd_flag = cm
+0000d8d0: 645f 666c 6167 2e72 6570 6c61 6365 2822  d_flag.replace("
+0000d8e0: 4069 6422 2c20 696e 7075 745b 2769 6427  @id", input['id'
+0000d8f0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000d900: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
+0000d910: 6d73 5b27 636d 645f 666c 6167 275d 203d  ms['cmd_flag'] =
+0000d920: 2063 6d64 5f66 6c61 670a 2020 2020 2020   cmd_flag.      
+0000d930: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000d940: 6f77 5f70 6172 616d 735b 2764 6573 6372  ow_params['descr
+0000d950: 6970 7469 6f6e 275d 203d 2069 6e70 7574  iption'] = input
+0000d960: 5b27 6465 7363 7269 7074 696f 6e27 5d0a  ['description'].
+0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d980: 776f 726b 666c 6f77 5f64 6963 745b 696e  workflow_dict[in
+0000d990: 7075 745b 2769 6427 5d5d 203d 2077 6f72  put['id']] = wor
+0000d9a0: 6b66 6c6f 775f 7061 7261 6d73 0a20 2020  kflow_params.   
+0000d9b0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
+0000d9c0: 666c 6f77 5f64 6963 740a 0a20 2020 2064  flow_dict..    d
+0000d9d0: 6566 2063 6f6e 7665 7274 5f63 7974 7970  ef convert_cytyp
+0000d9e0: 655f 746f 5f6f 6d74 7970 6528 7365 6c66  e_to_omtype(self
+0000d9f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 2020 2063 7974 7970 653a 2073 7472 2c20     cytype: str, 
+0000da20: 5f64 6566 6175 6c74 2c20 2a61 7267 732c  _default, *args,
+0000da30: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+0000da60: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+0000da70: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
+0000da80: 2061 2043 7974 6f6d 696e 6520 7479 7065   a Cytomine type
+0000da90: 2074 6f20 616e 204f 4d45 524f 2074 7970   to an OMERO typ
+0000daa0: 6520 616e 6420 696e 7374 616e 7469 6174  e and instantiat
+0000dab0: 6573 2069 740a 2020 2020 2020 2020 7769  es it.        wi
+0000dac0: 7468 2061 7267 732f 6b77 6172 6773 2e0a  th args/kwargs..
+0000dad0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
+0000dae0: 6174 2043 7974 6f6d 696e 6520 6861 7320  at Cytomine has 
+0000daf0: 6120 5079 7468 6f6e 2043 6c69 656e 742c  a Python Client,
+0000db00: 2061 6e64 2073 6f6d 6520 636f 6e76 6572   and some conver
+0000db10: 7369 6f6e 206d 6574 686f 6473 0a20 2020  sion methods.   
+0000db20: 2020 2020 2074 6f20 7079 7468 6f6e 2074       to python t
+0000db30: 7970 6573 2c20 6275 7420 6e6f 7468 696e  ypes, but nothin
+0000db40: 6720 7061 7274 6963 756c 6172 6c79 2077  g particularly w
+0000db50: 6f72 7468 2064 6570 656e 6469 6e67 206f  orth depending o
+0000db60: 6e20 7468 6174 0a20 2020 2020 2020 206c  n that.        l
+0000db70: 6962 7261 7279 2066 6f72 2079 6574 2e20  ibrary for yet. 
+0000db80: 4d69 6768 7420 6265 2075 7365 6675 6c20  Might be useful 
+0000db90: 696e 2074 6865 2066 7574 7572 6520 7065  in the future pe
+0000dba0: 7268 6170 732e 0a20 2020 2020 2020 2028  rhaps..        (
+0000dbb0: 652e 672e 2068 7474 7073 3a2f 2f67 6974  e.g. https://git
+0000dbc0: 6875 622e 636f 6d2f 4379 746f 6d69 6e65  hub.com/Cytomine
+0000dbd0: 2d55 4c69 6567 652f 4379 746f 6d69 6e65  -ULiege/Cytomine
+0000dbe0: 2d70 7974 686f 6e2d 636c 6965 6e74 2f0a  -python-client/.
+0000dbf0: 2020 2020 2020 2020 626c 6f62 2f6d 6173          blob/mas
+0000dc00: 7465 722f 6379 746f 6d69 6e65 2f63 7974  ter/cytomine/cyt
+0000dc10: 6f6d 696e 655f 6a6f 622e 7079 290a 0a20  omine_job.py).. 
+0000dc20: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000dc30: 2020 2020 2020 2020 2063 7974 7970 6520           cytype 
+0000dc40: 2873 7472 293a 2054 6865 2043 7974 6f6d  (str): The Cytom
+0000dc50: 696e 6520 7479 7065 2074 6f20 636f 6e76  ine type to conv
+0000dc60: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
+0000dc70: 205f 6465 6661 756c 743a 2054 6865 2064   _default: The d
+0000dc80: 6566 6175 6c74 2076 616c 7565 2e20 5265  efault value. Re
+0000dc90: 7175 6972 6564 2074 6f20 6469 7374 696e  quired to distin
+0000dca0: 6775 6973 6820 6265 7477 6565 6e20 666c  guish between fl
+0000dcb0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+0000dcc0: 2020 2020 616e 6420 696e 742e 0a20 2020      and int..   
+0000dcd0: 2020 2020 2020 2020 202a 6172 6773 3a20           *args: 
+0000dce0: 4164 6469 7469 6f6e 616c 2070 6f73 6974  Additional posit
+0000dcf0: 696f 6e61 6c20 6172 6775 6d65 6e74 732e  ional arguments.
+0000dd00: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000dd10: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
+0000dd20: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+0000dd30: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
+0000dd40: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000dd50: 2020 2041 6e79 3a0a 2020 2020 2020 2020     Any:.        
+0000dd60: 2020 2020 2020 2020 5468 6520 636f 6e76          The conv
+0000dd70: 6572 7465 6420 4f4d 4552 4f20 7479 7065  erted OMERO type
+0000dd80: 2063 6c61 7373 2069 6e73 7461 6e63 650a   class instance.
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 6f72 204e 6f6e 6520 6966 2065 7272 6f72  or None if error
+0000ddb0: 7320 6f63 6375 7265 642e 0a0a 2020 2020  s occured...    
+0000ddc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ddd0: 2320 544f 444f 206d 616b 6520 456e 756d  # TODO make Enum
+0000dde0: 203f 0a20 2020 2020 2020 2069 6620 6379   ?.        if cy
+0000ddf0: 7479 7065 203d 3d20 274e 756d 6265 7227  type == 'Number'
+0000de00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000de10: 2069 7369 6e73 7461 6e63 6528 5f64 6566   isinstance(_def
+0000de20: 6175 6c74 2c20 666c 6f61 7429 3a0a 2020  ault, float):.  
+0000de30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000de40: 666c 6f61 7420 696e 7374 6561 640a 2020  float instead.  
+0000de50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000de60: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
+0000de70: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
+0000de80: 7269 7074 7322 2c20 2246 6c6f 6174 222c  ripts", "Float",
+0000de90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000deb0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
+0000dec0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000ded0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000dee0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000def0: 7572 6e20 7365 6c66 2e73 7472 5f74 6f5f  urn self.str_to_
+0000df00: 636c 6173 7328 226f 6d65 726f 2e73 6372  class("omero.scr
+0000df10: 6970 7473 222c 2022 496e 7422 2c0a 2020  ipts", "Int",.  
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df40: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
+0000df50: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+0000df60: 656c 6966 2063 7974 7970 6520 3d3d 2027  elif cytype == '
+0000df70: 426f 6f6c 6561 6e27 3a0a 2020 2020 2020  Boolean':.      
+0000df80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000df90: 662e 7374 725f 746f 5f63 6c61 7373 2822  f.str_to_class("
+0000dfa0: 6f6d 6572 6f2e 7363 7269 7074 7322 2c20  omero.scripts", 
+0000dfb0: 2242 6f6f 6c22 2c0a 2020 2020 2020 2020  "Bool",.        
+0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfd0: 2020 2020 2020 2020 2020 2020 202a 6172               *ar
+0000dfe0: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+0000dff0: 2020 2020 2020 656c 6966 2063 7974 7970        elif cytyp
+0000e000: 6520 3d3d 2027 5374 7269 6e67 273a 0a20  e == 'String':. 
+0000e010: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e020: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
+0000e030: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
+0000e040: 7473 222c 2022 5374 7269 6e67 222c 0a20  ts", "String",. 
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e070: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
+0000e080: 7267 7329 0a0a 2020 2020 6465 6620 6578  rgs)..    def ex
+0000e090: 7472 6163 745f 7061 7274 735f 6672 6f6d  tract_parts_from
+0000e0a0: 5f75 726c 2873 656c 662c 2069 6e70 7574  _url(self, input
+0000e0b0: 5f75 726c 3a20 7374 7229 202d 3e20 5475  _url: str) -> Tu
+0000e0c0: 706c 655b 4c69 7374 5b73 7472 5d2c 2073  ple[List[str], s
+0000e0d0: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
+0000e0e0: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
+0000e0f0: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
+0000e100: 616e 6420 6272 616e 6368 2069 6e66 6f72  and branch infor
+0000e110: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
+0000e120: 696e 7075 7420 5552 4c2e 0a0a 2020 2020  input URL...    
+0000e130: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000e140: 2020 2020 2020 696e 7075 745f 7572 6c20        input_url 
+0000e150: 2873 7472 293a 2054 6865 2069 6e70 7574  (str): The input
+0000e160: 2047 6974 4875 6220 5552 4c2e 0a0a 2020   GitHub URL...  
+0000e170: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0000e180: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+0000e190: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
+0000e1a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e1b0: 2020 5468 6520 6c69 7374 206f 6620 7572    The list of ur
+0000e1c0: 6c20 7061 7274 7320 616e 6420 7468 6520  l parts and the 
+0000e1d0: 6272 616e 6368 2f76 6572 7369 6f6e 2e0a  branch/version..
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 4966 206e 6f20 6272 616e 6368 2069 7320  If no branch is 
+0000e200: 666f 756e 642c 2069 7420 7769 6c6c 2072  found, it will r
+0000e210: 6574 7572 6e20 226d 6173 7465 7222 0a0a  eturn "master"..
+0000e220: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+0000e230: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+0000e240: 6545 7272 6f72 3a20 4966 2074 6865 2069  eError: If the i
+0000e250: 6e70 7574 2055 524c 2069 7320 6e6f 7420  nput URL is not 
+0000e260: 6120 7661 6c69 6420 4769 7448 7562 2055  a valid GitHub U
+0000e270: 524c 2e0a 2020 2020 2020 2020 2222 220a  RL..        """.
+0000e280: 2020 2020 2020 2020 7572 6c5f 7061 7274          url_part
+0000e290: 7320 3d20 696e 7075 745f 7572 6c2e 7370  s = input_url.sp
+0000e2a0: 6c69 7428 222f 2229 0a20 2020 2020 2020  lit("/").       
+0000e2b0: 2069 6620 6c65 6e28 7572 6c5f 7061 7274   if len(url_part
+0000e2c0: 7329 203c 2035 206f 7220 7572 6c5f 7061  s) < 5 or url_pa
+0000e2d0: 7274 735b 325d 2021 3d20 2267 6974 6875  rts[2] != "githu
+0000e2e0: 622e 636f 6d22 3a0a 2020 2020 2020 2020  b.com":.        
+0000e2f0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000e300: 7272 6f72 2822 496e 7661 6c69 6420 4769  rror("Invalid Gi
+0000e310: 7448 7562 2055 524c 2229 0a0a 2020 2020  tHub URL")..    
+0000e320: 2020 2020 6966 2022 7472 6565 2220 696e      if "tree" in
+0000e330: 2075 726c 5f70 6172 7473 3a0a 2020 2020   url_parts:.    
+0000e340: 2020 2020 2020 2020 2320 4361 7365 3a20          # Case: 
+0000e350: 5552 4c20 636f 6e74 6169 6e73 2061 2062  URL contains a b
+0000e360: 7261 6e63 680a 2020 2020 2020 2020 2020  ranch.          
+0000e370: 2020 6272 616e 6368 5f69 6e64 6578 203d    branch_index =
+0000e380: 2075 726c 5f70 6172 7473 2e69 6e64 6578   url_parts.index
+0000e390: 2822 7472 6565 2229 202b 2031 0a20 2020  ("tree") + 1.   
+0000e3a0: 2020 2020 2020 2020 2062 7261 6e63 6820           branch 
+0000e3b0: 3d20 7572 6c5f 7061 7274 735b 6272 616e  = url_parts[bran
+0000e3c0: 6368 5f69 6e64 6578 5d0a 2020 2020 2020  ch_index].      
+0000e3d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000e3e0: 2020 2020 2320 4361 7365 3a20 5552 4c20      # Case: URL 
+0000e3f0: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
+0000e400: 2061 2062 7261 6e63 680a 2020 2020 2020   a branch.      
+0000e410: 2020 2020 2020 6272 616e 6368 203d 2022        branch = "
+0000e420: 6d61 7374 6572 220a 0a20 2020 2020 2020  master"..       
+0000e430: 2072 6574 7572 6e20 7572 6c5f 7061 7274   return url_part
+0000e440: 732c 2062 7261 6e63 680a 0a20 2020 2064  s, branch..    d
+0000e450: 6566 2063 6f6e 7665 7274 5f75 726c 2873  ef convert_url(s
+0000e460: 656c 662c 2069 6e70 7574 5f75 726c 3a20  elf, input_url: 
+0000e470: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
+0000e480: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000e490: 2043 6f6e 7665 7274 2074 6865 2069 6e70   Convert the inp
+0000e4a0: 7574 2047 6974 4875 6220 5552 4c20 746f  ut GitHub URL to
+0000e4b0: 2061 6e20 6f75 7470 7574 2055 524c 2074   an output URL t
+0000e4c0: 6861 7420 7265 7472 6965 7665 730a 2020  hat retrieves.  
+0000e4d0: 2020 2020 2020 7468 6520 2764 6573 6372        the 'descr
+0000e4e0: 6970 746f 722e 6a73 6f6e 2720 6669 6c65  iptor.json' file
+0000e4f0: 2069 6e20 7261 7720 666f 726d 6174 2e0a   in raw format..
+0000e500: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000e510: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000e520: 5f75 726c 2028 7374 7229 3a20 5468 6520  _url (str): The 
+0000e530: 696e 7075 7420 4769 7448 7562 2055 524c  input GitHub URL
+0000e540: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000e550: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000e560: 7374 723a 2054 6865 206f 7574 7075 7420  str: The output 
+0000e570: 5552 4c20 746f 2074 6865 2027 6465 7363  URL to the 'desc
+0000e580: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
+0000e590: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
+0000e5a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000e5b0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
+0000e5c0: 6865 2069 6e70 7574 2055 524c 2069 7320  he input URL is 
+0000e5d0: 6e6f 7420 6120 7661 6c69 6420 4769 7448  not a valid GitH
+0000e5e0: 7562 2055 524c 2e0a 2020 2020 2020 2020  ub URL..        
+0000e5f0: 2222 220a 2020 2020 2020 2020 7572 6c5f  """.        url_
+0000e600: 7061 7274 732c 2062 7261 6e63 6820 3d20  parts, branch = 
+0000e610: 7365 6c66 2e65 7874 7261 6374 5f70 6172  self.extract_par
+0000e620: 7473 5f66 726f 6d5f 7572 6c28 696e 7075  ts_from_url(inpu
+0000e630: 745f 7572 6c29 0a0a 2020 2020 2020 2020  t_url)..        
+0000e640: 2320 436f 6e73 7472 7563 7420 7468 6520  # Construct the 
+0000e650: 6f75 7470 7574 2055 524c 2062 7920 636f  output URL by co
+0000e660: 6d62 696e 696e 6720 7468 6520 6578 7472  mbining the extr
+0000e670: 6163 7465 6420 696e 666f 726d 6174 696f  acted informatio
+0000e680: 6e0a 2020 2020 2020 2020 2320 7769 7468  n.        # with
+0000e690: 2074 6865 2064 6573 6972 6564 2066 696c   the desired fil
+0000e6a0: 6520 7061 7468 0a20 2020 2020 2020 206f  e path.        o
+0000e6b0: 7574 7075 745f 7572 6c20 3d20 6622 6874  utput_url = f"ht
+0000e6c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e6d0: 2f7b 7572 6c5f 7061 7274 735b 335d 7d2f  /{url_parts[3]}/
+0000e6e0: 7b75 726c 5f70 6172 7473 5b34 5d7d 2f72  {url_parts[4]}/r
+0000e6f0: 6177 2f7b 6272 616e 6368 7d2f 6465 7363  aw/{branch}/desc
+0000e700: 7269 7074 6f72 2e6a 736f 6e22 0a0a 2020  riptor.json"..  
+0000e710: 2020 2020 2020 7265 7475 726e 206f 7574        return out
+0000e720: 7075 745f 7572 6c0a 0a20 2020 2064 6566  put_url..    def
+0000e730: 2070 756c 6c5f 6465 7363 7269 7074 6f72   pull_descriptor
+0000e740: 5f66 726f 6d5f 6769 7468 7562 2873 656c  _from_github(sel
+0000e750: 662c 2077 6f72 6b66 6c6f 773a 2073 7472  f, workflow: str
+0000e760: 2920 2d3e 2044 6963 743a 0a20 2020 2020  ) -> Dict:.     
+0000e770: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+0000e780: 756c 6c20 7468 6520 776f 726b 666c 6f77  ull the workflow
+0000e790: 2064 6573 6372 6970 746f 7220 6672 6f6d   descriptor from
+0000e7a0: 2047 6974 4875 622e 0a0a 2020 2020 2020   GitHub...      
+0000e7b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000e7c0: 2020 2020 776f 726b 666c 6f77 2028 7374      workflow (st
+0000e7d0: 7229 3a20 5468 6520 776f 726b 666c 6f77  r): The workflow
+0000e7e0: 2066 6f72 2077 6869 6368 2074 6f20 7075   for which to pu
+0000e7f0: 6c6c 2074 6865 2064 6573 6372 6970 746f  ll the descripto
+0000e800: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
+0000e810: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000e820: 2044 6963 743a 2054 6865 204a 534f 4e20   Dict: The JSON 
+0000e830: 6465 7363 7269 7074 6f72 2e0a 0a20 2020  descriptor...   
+0000e840: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0000e850: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+0000e860: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
+0000e870: 206f 6363 7572 7320 7768 696c 6520 7075   occurs while pu
+0000e880: 6c6c 696e 6720 7468 6520 6465 7363 7269  lling the descri
+0000e890: 7074 6f72 2066 696c 652e 0a20 2020 2020  ptor file..     
+0000e8a0: 2020 2022 2222 0a20 2020 2020 2020 2067     """.        g
+0000e8b0: 6974 5f72 6570 6f20 3d20 7365 6c66 2e73  it_repo = self.s
+0000e8c0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
+0000e8d0: 5b77 6f72 6b66 6c6f 775d 0a20 2020 2020  [workflow].     
+0000e8e0: 2020 2023 2063 6f6e 7665 7274 2067 6974     # convert git
+0000e8f0: 2072 6570 6f20 746f 206a 736f 6e20 6669   repo to json fi
+0000e900: 6c65 0a20 2020 2020 2020 2072 6177 5f75  le.        raw_u
+0000e910: 726c 203d 2073 656c 662e 636f 6e76 6572  rl = self.conver
+0000e920: 745f 7572 6c28 6769 745f 7265 706f 290a  t_url(git_repo).
+0000e930: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000e940: 6562 7567 2866 2250 756c 6c20 776f 726b  ebug(f"Pull work
+0000e950: 666c 6f77 3a20 7b77 6f72 6b66 6c6f 777d  flow: {workflow}
+0000e960: 3a20 7b67 6974 5f72 6570 6f7d 203e 3e20  : {git_repo} >> 
+0000e970: 7b72 6177 5f75 726c 7d22 290a 2020 2020  {raw_url}").    
+0000e980: 2020 2020 2320 7075 6c6c 2077 6f72 6b66      # pull workf
+0000e990: 6c6f 7720 7061 7261 6d73 0a20 2020 2020  low params.     
+0000e9a0: 2020 2067 6974 6875 625f 7365 7373 696f     github_sessio
+0000e9b0: 6e20 3d20 7365 6c66 2e67 6574 5f6f 725f  n = self.get_or_
+0000e9c0: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
+0000e9d0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
+0000e9e0: 6768 6669 6c65 203d 2067 6974 6875 625f  ghfile = github_
+0000e9f0: 7365 7373 696f 6e2e 6765 7428 7261 775f  session.get(raw_
+0000ea00: 7572 6c29 0a20 2020 2020 2020 2069 6620  url).        if 
+0000ea10: 6768 6669 6c65 2e6f 6b3a 0a20 2020 2020  ghfile.ok:.     
+0000ea20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000ea30: 6275 6728 6622 4361 6368 6564 3f20 7b67  bug(f"Cached? {g
+0000ea40: 6866 696c 652e 6672 6f6d 5f63 6163 6865  hfile.from_cache
+0000ea50: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000ea60: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
+0000ea70: 3d20 6768 6669 6c65 2e6a 736f 6e28 290a  = ghfile.json().
+0000ea80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ea90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000eaa0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+0000eab0: 2020 2020 2020 2020 2020 2020 6627 4572              f'Er
+0000eac0: 726f 7220 7768 696c 6520 7075 6c6c 696e  ror while pullin
+0000ead0: 6720 6465 7363 7269 7074 6f72 2066 696c  g descriptor fil
+0000eae0: 6520 666f 7220 776f 726b 666c 6f77 207b  e for workflow {
+0000eaf0: 776f 726b 666c 6f77 7d2c 5c0a 2020 2020  workflow},\.    
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 6672 6f6d 207b 7261 775f 7572 6c7d 3a20  from {raw_url}: 
+0000eb20: 7b67 6866 696c 652e 5f5f 6469 6374 5f5f  {ghfile.__dict__
+0000eb30: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
+0000eb40: 726e 206a 736f 6e5f 6465 7363 7269 7074  rn json_descript
+0000eb50: 6f72 0a0a 2020 2020 6465 6620 6765 745f  or..    def get_
+0000eb60: 6f72 5f63 7265 6174 655f 6769 7468 7562  or_create_github
+0000eb70: 5f73 6573 7369 6f6e 2873 656c 6629 3a0a  _session(self):.
+0000eb80: 2020 2020 2020 2020 2320 4e6f 7465 2c20          # Note, 
+0000eb90: 7573 696e 6720 7265 7175 6573 7473 5f63  using requests_c
+0000eba0: 6163 6865 2031 2e31 2e31 2c20 636f 6e64  ache 1.1.1, cond
+0000ebb0: 6974 696f 6e61 6c20 7175 6572 6965 7320  itional queries 
+0000ebc0: 6172 6520 6465 6661 756c 743a 0a20 2020  are default:.   
+0000ebd0: 2020 2020 2023 2054 6865 2063 6163 6865       # The cache
+0000ebe0: 6420 7265 7370 6f6e 7365 2077 696c 6c20  d response will 
+0000ebf0: 7374 696c 6c20 6265 2075 7365 6420 756e  still be used un
+0000ec00: 7469 6c20 7468 6520 7265 6d6f 7465 2063  til the remote c
+0000ec10: 6f6e 7465 6e74 2061 6374 7561 6c6c 7920  ontent actually 
+0000ec20: 6368 616e 6765 730a 2020 2020 2020 2020  changes.        
+0000ec30: 2320 4576 656e 2069 6620 7468 6520 2765  # Even if the 'e
+0000ec40: 7870 6972 655f 6166 7465 7227 2069 7320  xpire_after' is 
+0000ec50: 7472 6967 6765 7265 642e 2054 6869 7320  triggered. This 
+0000ec60: 6973 2062 7569 6c74 2069 6e74 6f20 4769  is built into Gi
+0000ec70: 7448 7562 2c20 7768 6963 6820 7265 7475  tHub, which retu
+0000ec80: 726e 730a 2020 2020 2020 2020 2320 6120  rns.        # a 
+0000ec90: 4574 6167 2069 6e20 7468 6520 6865 6164  Etag in the head
+0000eca0: 6572 2074 6861 7420 6f6e 6c79 2063 6861  er that only cha
+0000ecb0: 6e67 6573 2077 6865 6e20 7468 6520 636f  nges when the co
+0000ecc0: 6e74 656e 7420 2865 2e67 2e20 7468 6520  ntent (e.g. the 
+0000ecd0: 6465 7363 7269 7074 6f72 2920 6368 616e  descriptor) chan
+0000ece0: 6765 732e 0a20 2020 2020 2020 2023 2049  ges..        # I
+0000ecf0: 6620 796f 7520 7072 6f76 6964 6520 7468  f you provide th
+0000ed00: 6973 2045 7461 6720 7768 656e 2071 7565  is Etag when que
+0000ed10: 7279 696e 672c 2079 6f75 2077 696c 6c20  rying, you will 
+0000ed20: 6765 7420 6120 3330 3420 2827 6e6f 2063  get a 304 ('no c
+0000ed30: 6861 6e67 6527 2920 616e 6420 6974 2077  hange') and it w
+0000ed40: 696c 6c0a 2020 2020 2020 2020 2320 4e4f  ill.        # NO
+0000ed50: 5420 636f 756e 7420 746f 7761 7264 7320  T count towards 
+0000ed60: 796f 7572 2047 6974 6875 6220 6c69 6d69  your Github limi
+0000ed70: 7473 2e20 416e 6420 7265 7175 6573 7473  ts. And requests
+0000ed80: 5f63 6163 6865 2064 6f65 7320 7468 6174  _cache does that
+0000ed90: 2066 6f72 2075 7320 6e6f 772e 0a20 2020   for us now..   
+0000eda0: 2020 2020 2023 204e 6f74 2061 7661 696c       # Not avail
+0000edb0: 6162 6c65 2069 6e20 5079 7468 6f6e 332e  able in Python3.
+0000edc0: 3620 7468 6f75 6768 2e0a 2020 2020 2020  6 though..      
+0000edd0: 2020 7320 3d20 7265 7175 6573 7473 5f63    s = requests_c
+0000ede0: 6163 6865 2e43 6163 6865 6453 6573 7369  ache.CachedSessi
+0000edf0: 6f6e 2827 6769 7468 7562 5f63 6163 6865  on('github_cache
+0000ee00: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee20: 2020 2020 2020 2020 2020 2020 6261 636b              back
+0000ee30: 656e 643d 7365 6c66 2e63 6163 6865 2c0a  end=self.cache,.
+0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee60: 2020 2020 2020 2020 2065 7870 6972 655f           expire_
+0000ee70: 6166 7465 723d 312c 0a20 2020 2020 2020  after=1,.       
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eea0: 2020 6361 6368 655f 636f 6e74 726f 6c3d    cache_control=
+0000eeb0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eed0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000eee0: 2020 2020 2020 2020 2320 4d69 6768 7420          # Might 
+0000eef0: 6861 7665 2062 6967 6765 7220 6973 7375  have bigger issu
+0000ef00: 6573 2c20 7468 6973 2069 7320 7265 6c61  es, this is rela
+0000ef10: 7465 6420 746f 2072 6174 6520 6c69 6d69  ted to rate limi
+0000ef20: 7473 206f 6e20 4769 7448 7562 0a20 2020  ts on GitHub.   
+0000ef30: 2020 2020 2023 2068 7474 7073 3a2f 2f64       # https://d
+0000ef40: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+0000ef50: 6e2f 7265 7374 2f75 7369 6e67 2d74 6865  n/rest/using-the
+0000ef60: 2d72 6573 742d 6170 692f 7261 7465 2d6c  -rest-api/rate-l
+0000ef70: 696d 6974 732d 666f 722d 7468 652d 7265  imits-for-the-re
+0000ef80: 7374 2d61 7069 0a20 2020 2020 2020 2023  st-api.        #
+0000ef90: 2049 6620 6974 2073 7461 7973 2061 2070   If it stays a p
+0000efa0: 726f 626c 656d 2c20 7765 2068 6176 6520  roblem, we have 
+0000efb0: 746f 2061 6464 2061 6e20 6f70 7469 6f6e  to add an option
+0000efc0: 2074 6f20 6164 6420 6120 4748 206b 6579   to add a GH key
+0000efd0: 2074 6f20 7468 6520 636f 6e66 6967 0a20   to the config. 
+0000efe0: 2020 2020 2020 2023 2045 2e67 2e20 7365         # E.g. se
+0000eff0: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+0000f000: 2e63 6f6d 2f72 6571 7565 7374 732d 6361  .com/requests-ca
+0000f010: 6368 652f 7265 7175 6573 7473 2d63 6163  che/requests-cac
+0000f020: 6865 2f62 6c6f 622f 3533 3133 3465 6630  he/blob/53134ef0
+0000f030: 6539 3964 3731 3366 6564 3632 3531 3564  e99d713fed62515d
+0000f040: 6662 3762 6366 6161 6335 6636 3366 3964  fb7bcfaac5f63f9d
+0000f050: 2f65 7861 6d70 6c65 732f 7079 6769 7468  /examples/pygith
+0000f060: 7562 2e70 790a 2020 2020 2020 2020 2320  ub.py.        # 
+0000f070: 4865 7265 2079 6f75 2063 6f75 6c64 2068  Here you could h
+0000f080: 6176 6520 616e 2041 4343 4553 535f 544f  ave an ACCESS_TO
+0000f090: 4b45 4e2e 0a20 2020 2020 2020 2023 2041  KEN..        # A
+0000f0a0: 6e20 4143 4345 5353 5f54 4f4b 454e 2063  n ACCESS_TOKEN c
+0000f0b0: 6f75 6c64 2069 6d70 726f 7665 2061 7069  ould improve api
+0000f0c0: 206c 696d 6974 7320 746f 2035 3030 302f   limits to 5000/
+0000f0d0: 6820 2866 726f 6d20 3630 2f68 292e 0a20  h (from 60/h).. 
+0000f0e0: 2020 2020 2020 2072 6574 7279 5f73 7472         retry_str
+0000f0f0: 6174 6567 7920 3d20 5265 7472 7928 0a20  ategy = Retry(. 
+0000f100: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+0000f110: 3d35 2c20 2020 2020 2020 2020 2020 2020  =5,             
+0000f120: 2020 2320 4d61 7869 6d75 6d20 6e75 6d62    # Maximum numb
+0000f130: 6572 206f 6620 7265 7472 6965 730a 2020  er of retries.  
+0000f140: 2020 2020 2020 2020 2020 2320 4578 706f            # Expo
+0000f150: 6e65 6e74 6961 6c20 6261 636b 6f66 6620  nential backoff 
+0000f160: 6661 6374 6f72 2028 6465 6c61 7920 6265  factor (delay be
+0000f170: 7477 6565 6e20 7265 7472 6965 7329 0a20  tween retries). 
+0000f180: 2020 2020 2020 2020 2020 2062 6163 6b6f             backo
+0000f190: 6666 5f66 6163 746f 723d 352c 0a20 2020  ff_factor=5,.   
+0000f1a0: 2020 2020 2020 2020 2023 2052 6574 7279           # Retry
+0000f1b0: 206f 6e20 7468 6573 6520 4854 5450 2073   on these HTTP s
+0000f1c0: 7461 7475 7320 636f 6465 730a 2020 2020  tatus codes.    
+0000f1d0: 2020 2020 2020 2020 7374 6174 7573 5f66          status_f
+0000f1e0: 6f72 6365 6c69 7374 3d5b 3530 302c 2035  orcelist=[500, 5
+0000f1f0: 3032 2c20 3530 332c 2035 3034 2c20 3430  02, 503, 504, 40
+0000f200: 332c 2034 3239 5d2c 0a20 2020 2020 2020  3, 429],.       
+0000f210: 2020 2020 2061 6c6c 6f77 6564 5f6d 6574       allowed_met
+0000f220: 686f 6473 3d66 726f 7a65 6e73 6574 285b  hods=frozenset([
+0000f230: 2747 4554 275d 2920 2023 204f 6e6c 7920  'GET'])  # Only 
+0000f240: 7265 7472 7920 666f 7220 4745 5420 7265  retry for GET re
+0000f250: 7175 6573 7473 0a20 2020 2020 2020 2029  quests.        )
+0000f260: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
+0000f270: 2827 6874 7470 733a 2f2f 6769 7468 7562  ('https://github
+0000f280: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
+0000f290: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
+0000f2a0: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
+0000f2b0: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
+0000f2c0: 2827 6874 7470 3a2f 2f67 6974 6875 622e  ('http://github.
+0000f2d0: 636f 6d2f 272c 2048 5454 5041 6461 7074  com/', HTTPAdapt
+0000f2e0: 6572 286d 6178 5f72 6574 7269 6573 3d72  er(max_retries=r
+0000f2f0: 6574 7279 5f73 7472 6174 6567 7929 290a  etry_strategy)).
+0000f300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000f310: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
+0000f320: 726b 666c 6f77 5f63 6f6d 6d61 6e64 2873  rkflow_command(s
+0000f330: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f350: 2020 776f 726b 666c 6f77 3a20 7374 722c    workflow: str,
+0000f360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f370: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+0000f380: 726b 666c 6f77 5f76 6572 7369 6f6e 3a20  rkflow_version: 
+0000f390: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 2020 696e 7075 745f 6461 7461 3a20 7374    input_data: st
+0000f3c0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 656d 6169 6c3a 204f 7074 696f 6e61 6c5b  email: Optional[
+0000f3f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f410: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
+0000f420: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000f430: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 2020 202a 2a6b 7761 7267 7329 202d 3e20     **kwargs) -> 
+0000f460: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
+0000f470: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f480: 2020 2020 2020 4765 6e65 7261 7465 2074        Generate t
+0000f490: 6865 2053 6c75 726d 2077 6f72 6b66 6c6f  he Slurm workflo
+0000f4a0: 7720 636f 6d6d 616e 6420 616e 6420 656e  w command and en
+0000f4b0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+0000f4c0: 6c65 732e 0a0a 2020 2020 2020 2020 4172  les...        Ar
+0000f4d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000f4e0: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
+0000f4f0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0000f500: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
+0000f510: 2020 2020 2020 776f 726b 666c 6f77 5f76        workflow_v
+0000f520: 6572 7369 6f6e 2028 7374 7229 3a20 5468  ersion (str): Th
+0000f530: 6520 7665 7273 696f 6e20 6f66 2074 6865  e version of the
+0000f540: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+0000f550: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+0000f560: 6120 2873 7472 293a 2054 6865 206e 616d  a (str): The nam
+0000f570: 6520 6f66 2074 6865 2069 6e70 7574 2064  e of the input d
+0000f580: 6174 6120 666f 6c64 6572 2063 6f6e 7461  ata folder conta
+0000f590: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
+0000f5a0: 2020 2020 2020 7468 6520 696e 7075 7420        the input 
+0000f5b0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
+0000f5c0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
+0000f5d0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0000f5e0: 5468 6520 656d 6169 6c20 6164 6472 6573  The email addres
+0000f5f0: 7320 666f 7220 6a6f 6220 6e6f 7469 6669  s for job notifi
+0000f600: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
+0000f610: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+0000f620: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
+0000f630: 2064 6566 6175 6c74 7320 746f 2077 6861   defaults to wha
+0000f640: 7420 6973 2069 6e20 7468 6520 6a6f 6220  t is in the job 
+0000f650: 7363 7269 7074 2e0a 2020 2020 2020 2020  script..        
+0000f660: 2020 2020 7469 6d65 2028 7374 722c 206f      time (str, o
+0000f670: 7074 696f 6e61 6c29 3a20 5468 6520 7469  ptional): The ti
+0000f680: 6d65 206c 696d 6974 2066 6f72 2074 6865  me limit for the
+0000f690: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
+0000f6a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f6b0: 6d61 7420 4848 3a4d 4d3a 5353 2e20 4465  mat HH:MM:SS. De
+0000f6c0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
+0000f6d0: 7768 6963 6820 6465 6661 756c 7473 2074  which defaults t
+0000f6e0: 6f20 7768 6174 200a 2020 2020 2020 2020  o what .        
+0000f6f0: 2020 2020 2020 2020 6973 2069 6e20 7468          is in th
+0000f700: 6520 6a6f 6220 7363 7269 7074 2e0a 2020  e job script..  
+0000f710: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000f720: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000f730: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000f740: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
+0000f750: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
+0000f760: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000f770: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
+0000f780: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000f790: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+0000f7a0: 696e 696e 6720 7468 6520 536c 7572 6d20  ining the Slurm 
+0000f7b0: 776f 726b 666c 6f77 2063 6f6d 6d61 6e64  workflow command
+0000f7c0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000f7d0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
+0000f7e0: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
+0000f7f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f800: 2020 2020 206d 6f64 656c 5f70 6174 6820       model_path 
+0000f810: 3d20 7365 6c66 2e73 6c75 726d 5f6d 6f64  = self.slurm_mod
+0000f820: 656c 5f70 6174 6873 5b77 6f72 6b66 6c6f  el_paths[workflo
+0000f830: 772e 6c6f 7765 7228 295d 0a20 2020 2020  w.lower()].     
+0000f840: 2020 206a 6f62 5f73 6372 6970 7420 3d20     job_script = 
+0000f850: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+0000f860: 5f6a 6f62 735b 776f 726b 666c 6f77 2e6c  _jobs[workflow.l
+0000f870: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
+0000f880: 6a6f 625f 7061 7261 6d73 203d 2073 656c  job_params = sel
+0000f890: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
+0000f8a0: 6273 5f70 6172 616d 735b 776f 726b 666c  bs_params[workfl
+0000f8b0: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
+0000f8c0: 2020 2020 2320 6772 6162 206f 6e6c 7920      # grab only 
+0000f8d0: 7468 6520 696d 6167 6520 6e61 6d65 2c20  the image name, 
+0000f8e0: 6e6f 7420 7468 6520 6772 6f75 702f 6372  not the group/cr
+0000f8f0: 6561 746f 720a 2020 2020 2020 2020 696d  eator.        im
+0000f900: 6167 6520 3d20 7365 6c66 2e73 6c75 726d  age = self.slurm
+0000f910: 5f6d 6f64 656c 5f69 6d61 6765 735b 776f  _model_images[wo
+0000f920: 726b 666c 6f77 2e6c 6f77 6572 2829 5d2e  rkflow.lower()].
+0000f930: 7370 6c69 7428 222f 2229 5b31 5d0a 0a20  split("/")[1].. 
+0000f940: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
+0000f950: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
+0000f960: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
+0000f970: 227b 7365 6c66 2e73 6c75 726d 5f64 6174  "{self.slurm_dat
+0000f980: 615f 7061 7468 7d2f 7b69 6e70 7574 5f64  a_path}/{input_d
+0000f990: 6174 617d 222c 0a20 2020 2020 2020 2020  ata}",.         
+0000f9a0: 2020 2022 494d 4147 455f 5041 5448 223a     "IMAGE_PATH":
+0000f9b0: 2066 227b 7365 6c66 2e73 6c75 726d 5f69   f"{self.slurm_i
+0000f9c0: 6d61 6765 735f 7061 7468 7d2f 7b6d 6f64  mages_path}/{mod
+0000f9d0: 656c 5f70 6174 687d 222c 0a20 2020 2020  el_path}",.     
+0000f9e0: 2020 2020 2020 2022 494d 4147 455f 5645         "IMAGE_VE
+0000f9f0: 5253 494f 4e22 3a20 6622 7b77 6f72 6b66  RSION": f"{workf
+0000fa00: 6c6f 775f 7665 7273 696f 6e7d 222c 0a20  low_version}",. 
+0000fa10: 2020 2020 2020 2020 2020 2022 5349 4e47             "SING
+0000fa20: 554c 4152 4954 595f 494d 4147 4522 3a20  ULARITY_IMAGE": 
+0000fa30: 6622 7b69 6d61 6765 7d5f 7b77 6f72 6b66  f"{image}_{workf
+0000fa40: 6c6f 775f 7665 7273 696f 6e7d 2e73 6966  low_version}.sif
+0000fa50: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000fa60: 5343 5249 5054 5f50 4154 4822 3a20 6622  SCRIPT_PATH": f"
+0000fa70: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
+0000fa80: 7074 5f70 6174 687d 220a 2020 2020 2020  pt_path}".      
+0000fa90: 2020 7d0a 2020 2020 2020 2020 776f 726b    }.        work
+0000faa0: 666c 6f77 5f65 6e76 203d 2073 656c 662e  flow_env = self.
+0000fab0: 776f 726b 666c 6f77 5f70 6172 616d 735f  workflow_params_
+0000fac0: 746f 5f65 6e76 7661 7273 282a 2a6b 7761  to_envvars(**kwa
+0000fad0: 7267 7329 0a20 2020 2020 2020 2065 6e76  rgs).        env
+0000fae0: 203d 207b 2a2a 7362 6174 6368 5f65 6e76   = {**sbatch_env
+0000faf0: 2c20 2a2a 776f 726b 666c 6f77 5f65 6e76  , **workflow_env
+0000fb00: 7d0a 0a20 2020 2020 2020 2065 6d61 696c  }..        email
+0000fb10: 5f70 6172 616d 203d 2022 2220 6966 2065  _param = "" if e
+0000fb20: 6d61 696c 2069 7320 4e6f 6e65 2065 6c73  mail is None els
+0000fb30: 6520 6622 202d 2d6d 6169 6c2d 7573 6572  e f" --mail-user
+0000fb40: 3d7b 656d 6169 6c7d 220a 2020 2020 2020  ={email}".      
+0000fb50: 2020 7469 6d65 5f70 6172 616d 203d 2022    time_param = "
+0000fb60: 2220 6966 2074 696d 6520 6973 204e 6f6e  " if time is Non
+0000fb70: 6520 656c 7365 2066 2220 2d2d 7469 6d65  e else f" --time
+0000fb80: 3d7b 7469 6d65 7d22 0a20 2020 2020 2020  ={time}".       
+0000fb90: 206a 6f62 5f70 6172 616d 732e 6170 7065   job_params.appe
+0000fba0: 6e64 2874 696d 655f 7061 7261 6d29 0a20  nd(time_param). 
+0000fbb0: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
+0000fbc0: 732e 6170 7065 6e64 2865 6d61 696c 5f70  s.append(email_p
+0000fbd0: 6172 616d 290a 2020 2020 2020 2020 6a6f  aram).        jo
+0000fbe0: 625f 7061 7261 6d20 3d20 2222 2e6a 6f69  b_param = "".joi
+0000fbf0: 6e28 6a6f 625f 7061 7261 6d73 290a 2020  n(job_params).  
+0000fc00: 2020 2020 2020 7362 6174 6368 5f63 6d64        sbatch_cmd
+0000fc10: 203d 2066 2273 6261 7463 687b 6a6f 625f   = f"sbatch{job_
+0000fc20: 7061 7261 6d7d 202d 2d6f 7574 7075 743d  param} --output=
+0000fc30: 6f6d 6572 6f2d 256a 2e6c 6f67 205c 0a20  omero-%j.log \. 
+0000fc40: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+0000fc50: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
+0000fc60: 7468 7d2f 7b6a 6f62 5f73 6372 6970 747d  th}/{job_script}
+0000fc70: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000fc80: 6e20 7362 6174 6368 5f63 6d64 2c20 656e  n sbatch_cmd, en
+0000fc90: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
+0000fca0: 6f6e 7665 7273 696f 6e5f 636f 6d6d 616e  onversion_comman
+0000fcb0: 6428 7365 6c66 2c20 6461 7461 5f70 6174  d(self, data_pat
+0000fcc0: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
+0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fce0: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
+0000fcf0: 6c65 3a20 7374 722c 0a20 2020 2020 2020  le: str,.       
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
+0000fd20: 6f72 6d61 743a 2073 7472 203d 2027 7a61  ormat: str = 'za
+0000fd30: 7272 272c 0a20 2020 2020 2020 2020 2020  rr',.           
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd50: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
+0000fd60: 743a 2073 7472 203d 2027 7469 6666 2729  t: str = 'tiff')
+0000fd70: 202d 3e20 5475 706c 655b 7374 722c 2044   -> Tuple[str, D
+0000fd80: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+0000fd90: 220a 2020 2020 2020 2020 4765 6e65 7261  ".        Genera
+0000fda0: 7465 2053 6c75 726d 2063 6f6e 7665 7273  te Slurm convers
+0000fdb0: 696f 6e20 636f 6d6d 616e 6420 616e 6420  ion command and 
+0000fdc0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+0000fdd0: 6162 6c65 7320 666f 7220 6461 7461 2063  ables for data c
+0000fde0: 6f6e 7665 7273 696f 6e2e 0a0a 2020 2020  onversion...    
+0000fdf0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000fe00: 2020 2020 2020 6461 7461 5f70 6174 6820        data_path 
+0000fe10: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
+0000fe20: 6865 2064 6174 6120 666f 6c64 6572 2e0a  he data folder..
+0000fe30: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000fe40: 6967 5f66 696c 6520 2873 7472 293a 2050  ig_file (str): P
+0000fe50: 6174 6820 746f 2074 6865 2063 6f6e 6669  ath to the confi
+0000fe60: 6775 7261 7469 6f6e 2066 696c 652e 0a20  guration file.. 
+0000fe70: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+0000fe80: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
+0000fe90: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
+0000fea0: 6174 2028 6465 6661 756c 7420 6973 2027  at (default is '
+0000feb0: 7a61 7272 2729 2e0a 2020 2020 2020 2020  zarr')..        
+0000fec0: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
+0000fed0: 7420 2873 7472 293a 2054 6172 6765 7420  t (str): Target 
+0000fee0: 6461 7461 2066 6f72 6d61 7420 2864 6566  data format (def
+0000fef0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
+0000ff00: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000ff10: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+0000ff20: 7570 6c65 5b73 7472 2c20 4469 6374 5d3a  uple[str, Dict]:
+0000ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff40: 2041 2074 7570 6c65 2063 6f6e 7461 696e   A tuple contain
+0000ff50: 696e 6720 7468 6520 536c 7572 6d20 636f  ing the Slurm co
+0000ff60: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
+0000ff70: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000ff80: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
+0000ff90: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
+0000ffa0: 0a20 2020 2020 2020 2057 6172 6e69 6e67  .        Warning
+0000ffb0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+0000ffc0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
+0000ffd0: 656e 7461 7469 6f6e 206f 6e6c 7920 7375  entation only su
+0000ffe0: 7070 6f72 7473 2063 6f6e 7665 7273 696f  pports conversio
+0000fff0: 6e20 6672 6f6d 2027 7a61 7272 2720 746f  n from 'zarr' to
+00010000: 2027 7469 6666 272e 0a20 2020 2020 2020   'tiff'..       
+00010010: 2020 2020 2049 6620 7573 696e 6720 6f74       If using ot
+00010020: 6865 7220 736f 7572 6365 206f 7220 7461  her source or ta
+00010030: 7267 6574 2066 6f72 6d61 7473 2c20 7573  rget formats, us
+00010040: 6572 7320 6d75 7374 2069 6d70 6c65 6d65  ers must impleme
+00010050: 6e74 2061 6e64 2063 6f6e 6669 6775 7265  nt and configure
+00010060: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00010070: 6974 696f 6e61 6c20 636f 6e76 6572 7465  itional converte
+00010080: 7273 2074 6865 6d73 656c 7665 732e 0a20  rs themselves.. 
+00010090: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000100a0: 2020 2069 6620 736f 7572 6365 5f66 6f72     if source_for
+000100b0: 6d61 7420 213d 2022 7a61 7272 2220 6f72  mat != "zarr" or
+000100c0: 2074 6172 6765 745f 666f 726d 6174 2021   target_format !
+000100d0: 3d20 2274 6966 6622 3a0a 2020 2020 2020  = "tiff":.      
+000100e0: 2020 2020 2020 2320 5761 726e 2061 626f        # Warn abo
+000100f0: 7574 2075 6e73 7570 706f 7274 6564 2063  ut unsupported c
+00010100: 6f6e 7665 7273 696f 6e3b 2061 6464 6974  onversion; addit
+00010110: 696f 6e61 6c20 636f 6e76 6572 7465 7273  ional converters
+00010120: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00010130: 2020 2020 2320 6164 6465 6420 6f75 7473      # added outs
+00010140: 6964 6520 6f75 7220 6b6e 6f77 6c65 6467  ide our knowledg
+00010150: 652e 0a20 2020 2020 2020 2020 2020 2023  e..            #
+00010160: 2043 6865 636b 696e 6720 536c 7572 6d27   Checking Slurm'
+00010170: 7320 6073 6c75 726d 5f63 6f6e 7665 7274  s `slurm_convert
+00010180: 6572 735f 7061 7468 6020 6973 2073 6b69  ers_path` is ski
+00010190: 7070 6564 2066 6f72 0a20 2020 2020 2020  pped for.       
+000101a0: 2020 2020 2023 2070 6572 666f 726d 616e       # performan
+000101b0: 6365 2072 6561 736f 6e73 2e0a 2020 2020  ce reasons..    
+000101c0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+000101d0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+000101e0: 2020 2020 2020 2020 6622 436f 6e76 6572          f"Conver
+000101f0: 7369 6f6e 2066 726f 6d20 7b73 6f75 7263  sion from {sourc
+00010200: 655f 666f 726d 6174 7d20 746f 207b 7461  e_format} to {ta
+00010210: 7267 6574 5f66 6f72 6d61 747d 2069 7320  rget_format} is 
+00010220: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00010230: 2064 6566 6175 6c74 2122 290a 0a20 2020   default!")..   
+00010240: 2020 2020 2063 686f 7365 6e5f 636f 6e76       chosen_conv
+00010250: 6572 7465 7220 3d20 6622 636f 6e76 6572  erter = f"conver
+00010260: 745f 7b73 6f75 7263 655f 666f 726d 6174  t_{source_format
+00010270: 7d5f 746f 5f7b 7461 7267 6574 5f66 6f72  }_to_{target_for
+00010280: 6d61 747d 2e73 6966 220a 2020 2020 2020  mat}.sif".      
+00010290: 2020 7362 6174 6368 5f65 6e76 203d 207b    sbatch_env = {
+000102a0: 0a20 2020 2020 2020 2020 2020 2022 4441  .            "DA
+000102b0: 5441 5f50 4154 4822 3a20 6622 7b64 6174  TA_PATH": f"{dat
+000102c0: 615f 7061 7468 7d22 2c0a 2020 2020 2020  a_path}",.      
+000102d0: 2020 2020 2020 2243 4f4e 5645 5253 494f        "CONVERSIO
+000102e0: 4e5f 5041 5448 223a 2066 227b 7365 6c66  N_PATH": f"{self
+000102f0: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
+00010300: 735f 7061 7468 7d22 2c0a 2020 2020 2020  s_path}",.      
+00010310: 2020 2020 2020 2243 4f4e 5645 5254 4552        "CONVERTER
+00010320: 5f49 4d41 4745 223a 2063 686f 7365 6e5f  _IMAGE": chosen_
+00010330: 636f 6e76 6572 7465 722c 0a20 2020 2020  converter,.     
+00010340: 2020 2020 2020 2022 5343 5249 5054 5f50         "SCRIPT_P
+00010350: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
+00010360: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
+00010370: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00010380: 434f 4e46 4947 5f46 494c 4522 3a20 6622  CONFIG_FILE": f"
+00010390: 7b63 6f6e 6669 675f 6669 6c65 7d22 0a20  {config_file}". 
+000103a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+000103b0: 2020 636f 6e76 6572 7369 6f6e 5f63 6d64    conversion_cmd
+000103c0: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
+000103d0: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
+000103e0: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
+000103f0: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
+00010400: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
+00010410: 2d2d 6172 7261 793d 312d 244e 2024 5343  --array=1-$N $SC
+00010420: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
+00010430: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
+00010440: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
+00010450: 7369 6f6e 5f63 6d64 5f77 6169 7469 6e67  sion_cmd_waiting
+00010460: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
+00010470: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
+00010480: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
+00010490: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
+000104a0: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
+000104b0: 2d2d 6172 7261 793d 312d 244e 202d 2d77  --array=1-$N --w
+000104c0: 6169 7420 2453 4352 4950 545f 5041 5448  ait $SCRIPT_PATH
+000104d0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
+000104e0: 6179 2e73 6822 0a0a 2020 2020 2020 2020  ay.sh"..        
+000104f0: 7265 7475 726e 2063 6f6e 7665 7273 696f  return conversio
+00010500: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
+00010510: 760a 0a20 2020 2064 6566 2077 6f72 6b66  v..    def workf
+00010520: 6c6f 775f 7061 7261 6d73 5f74 6f5f 656e  low_params_to_en
+00010530: 7676 6172 7328 7365 6c66 2c20 2a2a 6b77  vvars(self, **kw
+00010540: 6172 6773 2920 2d3e 2044 6963 743a 0a20  args) -> Dict:. 
+00010550: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010560: 2020 2043 6f6e 7665 7274 2077 6f72 6b66     Convert workf
+00010570: 6c6f 7720 7061 7261 6d65 7465 7273 2074  low parameters t
+00010580: 6f20 656e 7669 726f 6e6d 656e 7420 7661  o environment va
+00010590: 7269 6162 6c65 732e 0a0a 2020 2020 2020  riables...      
+000105a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000105b0: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
+000105c0: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+000105d0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
+000105e0: 6865 2077 6f72 6b66 6c6f 772e 0a0a 2020  he workflow...  
+000105f0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00010600: 2020 2020 2020 2020 2020 2044 6963 743a             Dict:
+00010610: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00010620: 6e74 6169 6e69 6e67 2074 6865 2065 6e76  ntaining the env
+00010630: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00010640: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00010650: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+00010660: 5f65 6e76 203d 207b 6b65 792e 7570 7065  _env = {key.uppe
+00010670: 7228 293a 2066 227b 7661 6c75 657d 2220  r(): f"{value}" 
+00010680: 666f 7220 6b65 792c 0a20 2020 2020 2020  for key,.       
+00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106a0: 2076 616c 7565 2069 6e20 6b77 6172 6773   value in kwargs
+000106b0: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
+000106c0: 2020 6c6f 6767 6572 2e64 6562 7567 2877    logger.debug(w
+000106d0: 6f72 6b66 6c6f 775f 656e 7629 0a20 2020  orkflow_env).   
+000106e0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
+000106f0: 666c 6f77 5f65 6e76 0a0a 2020 2020 6465  flow_env..    de
+00010700: 6620 6765 745f 6365 6c6c 706f 7365 5f63  f get_cellpose_c
+00010710: 6f6d 6d61 6e64 2873 656c 662c 2069 6d61  ommand(self, ima
+00010720: 6765 5f76 6572 7369 6f6e 3a20 7374 722c  ge_version: str,
+00010730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010740: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00010750: 7075 745f 6461 7461 3a20 7374 722c 0a20  put_data: str,. 
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2020 2020 2020 2020 2020 2020 6370 5f6d              cp_m
+00010780: 6f64 656c 3a20 7374 722c 0a20 2020 2020  odel: str,.     
+00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107a0: 2020 2020 2020 2020 6e75 635f 6368 616e          nuc_chan
+000107b0: 6e65 6c3a 2069 6e74 2c0a 2020 2020 2020  nel: int,.      
+000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107d0: 2020 2020 2020 2070 726f 625f 7468 7265         prob_thre
+000107e0: 7368 6f6c 643a 2066 6c6f 6174 2c0a 2020  shold: float,.  
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010800: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00010810: 6469 616d 6574 6572 3a20 666c 6f61 742c  diameter: float,
+00010820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010830: 2020 2020 2020 2020 2020 2020 2020 656d                em
+00010840: 6169 6c3a 204f 7074 696f 6e61 6c5b 7374  ail: Optional[st
+00010850: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
 00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2020 2065 6d61 696c 3d65 6d61 696c       email=email
-00010880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 2020 2020 2020 2020 2074 696d 653d             time=
-000108b0: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000108e0: 705f 6d6f 6465 6c3d 6370 5f6d 6f64 656c  p_model=cp_model
-000108f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2020 2020 2020 2020 2020 206e 7563 5f63             nuc_c
-00010920: 6861 6e6e 656c 3d6e 7563 5f63 6861 6e6e  hannel=nuc_chann
-00010930: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-00010960: 625f 7468 7265 7368 6f6c 643d 7072 6f62  b_threshold=prob
-00010970: 5f74 6872 6573 686f 6c64 2c0a 2020 2020  _threshold,.    
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 2063 656c 6c5f 6469 616d 6574       cell_diamet
-000109b0: 6572 3d63 656c 6c5f 6469 616d 6574 6572  er=cell_diameter
-000109c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 2020 2020 2020 2075 7365 5f67             use_g
-000109f0: 7075 3d75 7365 5f67 7075 290a 0a20 2020  pu=use_gpu)..   
-00010a00: 2064 6566 2063 6f70 795f 7a69 705f 6c6f   def copy_zip_lo
-00010a10: 6361 6c6c 7928 7365 6c66 2c20 6c6f 6361  cally(self, loca
-00010a20: 6c5f 746d 705f 7374 6f72 6167 653a 2073  l_tmp_storage: s
-00010a30: 7472 2c20 6669 6c65 6e61 6d65 3a20 7374  tr, filename: st
-00010a40: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00010a50: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00010a60: 5472 616e 7366 6572 5265 7375 6c74 3a0a  TransferResult:.
-00010a70: 2020 2020 2020 2020 2222 2220 436f 7079          """ Copy
-00010a80: 2061 207a 6970 2066 696c 6520 6672 6f6d   a zip file from
-00010a90: 2053 6c75 726d 2074 6f20 7468 6520 6c6f   Slurm to the lo
-00010aa0: 6361 6c20 7365 7276 6572 2e0a 0a20 2020  cal server...   
-00010ab0: 2020 2020 204e 6f74 6520 6162 6f75 7420       Note about 
-00010ac0: 2854 7261 6e73 6665 7229 5265 7375 6c74  (Transfer)Result
-00010ad0: 3a0a 0a20 2020 2020 2020 2055 6e6c 696b  :..        Unlik
-00010ae0: 6520 7369 6d69 6c61 7220 636c 6173 7365  e similar classe
-00010af0: 7320 7375 6368 2061 7320 696e 766f 6b65  s such as invoke
-00010b00: 2e72 756e 6e65 7273 2e52 6573 756c 7420  .runners.Result 
-00010b10: 6f72 0a20 2020 2020 2020 2066 6162 7269  or.        fabri
-00010b20: 632e 7275 6e6e 6572 732e 5265 7375 6c74  c.runners.Result
-00010b30: 0a20 2020 2020 2020 2028 7768 6963 6820  .        (which 
-00010b40: 6861 7665 2061 2063 6f6e 6365 7074 206f  have a concept o
-00010b50: 6620 e280 9c77 6172 6e20 616e 6420 7265  f ...warn and re
-00010b60: 7475 726e 2061 6e79 7761 7973 206f 6e20  turn anyways on 
-00010b70: 6661 696c 7572 65e2 809d 290a 2020 2020  failure...).    
-00010b80: 2020 2020 7468 6973 2063 6c61 7373 2068      this class h
-00010b90: 6173 206e 6f20 7573 6566 756c 2074 7275  as no useful tru
-00010ba0: 7468 696e 6573 7320 6265 6861 7669 6f72  thiness behavior
-00010bb0: 2e0a 2020 2020 2020 2020 4966 2061 2066  ..        If a f
-00010bc0: 696c 6520 7472 616e 7366 6572 2066 6169  ile transfer fai
-00010bd0: 6c73 2c20 736f 6d65 2065 7863 6570 7469  ls, some excepti
-00010be0: 6f6e 2077 696c 6c20 6265 2072 6169 7365  on will be raise
-00010bf0: 642c 0a20 2020 2020 2020 2065 6974 6865  d,.        eithe
-00010c00: 7220 616e 204f 5345 7272 6f72 206f 7220  r an OSError or 
-00010c10: 616e 2065 7272 6f72 2066 726f 6d20 7769  an error from wi
-00010c20: 7468 696e 2050 6172 616d 696b 6f2e 0a0a  thin Paramiko...
-00010c30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00010c40: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
-00010c50: 746d 705f 7374 6f72 6167 6520 2853 7472  tmp_storage (Str
-00010c60: 696e 6729 3a20 5061 7468 2074 6f20 7374  ing): Path to st
-00010c70: 6f72 6520 7468 6520 7a69 7020 6669 6c65  ore the zip file
-00010c80: 206c 6f63 616c 6c79 2e0a 2020 2020 2020   locally..      
-00010c90: 2020 2020 2020 6669 6c65 6e61 6d65 2028        filename (
-00010ca0: 5374 7269 6e67 293a 205a 6970 2066 696c  String): Zip fil
-00010cb0: 656e 616d 6520 6f6e 2053 6c75 726d 2e0a  ename on Slurm..
-00010cc0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00010cd0: 3a0a 2020 2020 2020 2020 2020 2020 5472  :.            Tr
-00010ce0: 616e 7366 6572 5265 7375 6c74 3a20 5468  ansferResult: Th
-00010cf0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
-00010d00: 7363 7020 6174 7465 6d70 742e 0a20 2020  scp attempt..   
-00010d10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010d20: 206c 6f67 6765 722e 696e 666f 2866 2243   logger.info(f"C
-00010d30: 6f70 7969 6e67 207a 6970 207b 6669 6c65  opying zip {file
-00010d40: 6e61 6d65 7d20 6672 6f6d 5c0a 2020 2020  name} from\.    
-00010d50: 2020 2020 2020 2020 536c 7572 6d20 746f          Slurm to
-00010d60: 207b 6c6f 6361 6c5f 746d 705f 7374 6f72   {local_tmp_stor
-00010d70: 6167 657d 2229 0a20 2020 2020 2020 2072  age}").        r
-00010d80: 6574 7572 6e20 7365 6c66 2e67 6574 280a  eturn self.get(.
-00010d90: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
-00010da0: 7465 3d66 227b 6669 6c65 6e61 6d65 7d2e  te=f"{filename}.
-00010db0: 7a69 7022 2c0a 2020 2020 2020 2020 2020  zip",.          
-00010dc0: 2020 6c6f 6361 6c3d 6c6f 6361 6c5f 746d    local=local_tm
-00010dd0: 705f 7374 6f72 6167 6529 0a0a 2020 2020  p_storage)..    
-00010de0: 6465 6620 7a69 705f 6461 7461 5f6f 6e5f  def zip_data_on_
-00010df0: 736c 7572 6d5f 7365 7276 6572 2873 656c  slurm_server(sel
-00010e00: 662c 2064 6174 615f 6c6f 6361 7469 6f6e  f, data_location
-00010e10: 3a20 7374 722c 2066 696c 656e 616d 653a  : str, filename:
-00010e20: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00010e50: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00010e60: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+00010870: 2020 2020 2020 2020 7469 6d65 3a20 4f70          time: Op
+00010880: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00010890: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 2075 7365 5f67 7075 3a20 626f 6f6c 203d   use_gpu: bool =
+000108c0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2020 2020 6d6f 6465 6c3a 2073 7472 203d      model: str =
+000108f0: 2022 6365 6c6c 706f 7365 2229 202d 3e20   "cellpose") -> 
+00010900: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
+00010910: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010920: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00010930: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
+00010940: 6972 6f6e 6d65 6e74 2064 6963 7469 6f6e  ironment diction
+00010950: 6172 7920 746f 2072 756e 2061 2043 656c  ary to run a Cel
+00010960: 6c50 6f73 6520 6a6f 620a 2020 2020 2020  lPose job.      
+00010970: 2020 6f6e 2074 6865 2053 6c75 726d 2077    on the Slurm w
+00010980: 6f72 6b6c 6f61 6420 6d61 6e61 6765 722e  orkload manager.
+00010990: 0a20 2020 2020 2020 2041 2073 7065 6369  .        A speci
+000109a0: 6669 6320 6578 616d 706c 6520 6f66 2075  fic example of u
+000109b0: 7369 6e67 2074 6865 2067 656e 6572 6963  sing the generic
+000109c0: 2027 6765 745f 776f 726b 666c 6f77 5f63   'get_workflow_c
+000109d0: 6f6d 6d61 6e64 272e 0a0a 2020 2020 2020  ommand'...      
+000109e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000109f0: 2020 2020 696d 6167 655f 7665 7273 696f      image_versio
+00010a00: 6e20 2873 7472 293a 2054 6865 2076 6572  n (str): The ver
+00010a10: 7369 6f6e 206f 6620 7468 6520 5369 6e67  sion of the Sing
+00010a20: 756c 6172 6974 7920 696d 6167 6520 746f  ularity image to
+00010a30: 2075 7365 2e0a 2020 2020 2020 2020 2020   use..          
+00010a40: 2020 696e 7075 745f 6461 7461 2028 7374    input_data (st
+00010a50: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
+00010a60: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
+00010a70: 6f6c 6465 7220 6f6e 2074 6865 2073 6861  older on the sha
+00010a80: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
+00010a90: 2020 2020 6669 6c65 2073 7973 7465 6d2e      file system.
+00010aa0: 0a20 2020 2020 2020 2020 2020 2063 705f  .            cp_
+00010ab0: 6d6f 6465 6c20 2873 7472 293a 2054 6865  model (str): The
+00010ac0: 206e 616d 6520 6f66 2074 6865 2043 656c   name of the Cel
+00010ad0: 6c50 6f73 6520 6d6f 6465 6c20 746f 2075  lPose model to u
+00010ae0: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+00010af0: 6e75 635f 6368 616e 6e65 6c20 2869 6e74  nuc_channel (int
+00010b00: 293a 2054 6865 2069 6e64 6578 206f 6620  ): The index of 
+00010b10: 7468 6520 6e75 636c 6561 7220 6368 616e  the nuclear chan
+00010b20: 6e65 6c2e 0a20 2020 2020 2020 2020 2020  nel..           
+00010b30: 2070 726f 625f 7468 7265 7368 6f6c 6420   prob_threshold 
+00010b40: 2866 6c6f 6174 293a 2054 6865 2070 726f  (float): The pro
+00010b50: 6261 6269 6c69 7479 2074 6872 6573 686f  bability thresho
+00010b60: 6c64 2066 6f72 0a20 2020 2020 2020 2020  ld for.         
+00010b70: 2020 2020 2020 206e 7563 6c65 6920 6465         nuclei de
+00010b80: 7465 6374 696f 6e2e 0a20 2020 2020 2020  tection..       
+00010b90: 2020 2020 2063 656c 6c5f 6469 616d 6574       cell_diamet
+00010ba0: 6572 2028 666c 6f61 7429 3a20 5468 6520  er (float): The 
+00010bb0: 6578 7065 6374 6564 2063 656c 6c20 6469  expected cell di
+00010bc0: 616d 6574 6572 2069 6e20 7069 7865 6c73  ameter in pixels
+00010bd0: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+00010be0: 6169 6c20 284f 7074 696f 6e61 6c5b 7374  ail (Optional[st
+00010bf0: 725d 293a 2054 6865 2065 6d61 696c 2061  r]): The email a
+00010c00: 6464 7265 7373 2074 6f20 7365 6e64 206e  ddress to send n
+00010c10: 6f74 6966 6963 6174 696f 6e73 2074 6f2e  otifications to.
+00010c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c30: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00010c40: 652e 0a20 2020 2020 2020 2020 2020 2074  e..            t
+00010c50: 696d 6520 284f 7074 696f 6e61 6c5b 7374  ime (Optional[st
+00010c60: 725d 293a 2054 6865 206d 6178 696d 756d  r]): The maximum
+00010c70: 2074 696d 6520 666f 7220 7468 6520 6a6f   time for the jo
+00010c80: 6220 746f 2072 756e 2e0a 2020 2020 2020  b to run..      
+00010c90: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00010ca0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00010cb0: 2020 2020 2020 2020 7573 655f 6770 7520          use_gpu 
+00010cc0: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+00010cd0: 746f 2075 7365 2047 5055 2066 6f72 2074  to use GPU for t
+00010ce0: 6865 2043 656c 6c50 6f73 6520 6a6f 622e  he CellPose job.
+00010cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d00: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+00010d10: 652e 0a20 2020 2020 2020 2020 2020 206d  e..            m
+00010d20: 6f64 656c 2028 7374 7229 3a20 5468 6520  odel (str): The 
+00010d30: 6e61 6d65 206f 6620 7468 6520 666f 6c64  name of the fold
+00010d40: 6572 206f 6620 7468 6520 446f 636b 6572  er of the Docker
+00010d50: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00010d70: 6566 6175 6c74 7320 746f 2022 6365 6c6c  efaults to "cell
+00010d80: 706f 7365 222e 0a0a 2020 2020 2020 2020  pose"...        
+00010d90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00010da0: 2020 2020 2054 7570 6c65 5b73 7472 2c20       Tuple[str, 
+00010db0: 6469 6374 5d3a 0a20 2020 2020 2020 2020  dict]:.         
+00010dc0: 2020 2020 2020 2041 2074 7570 6c65 2063         A tuple c
+00010dd0: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00010de0: 7572 6d20 7362 6174 6368 2063 6f6d 6d61  urm sbatch comma
+00010df0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00010e00: 2020 2061 6e64 2074 6865 2065 6e76 6972     and the envir
+00010e10: 6f6e 6d65 6e74 2064 6963 7469 6f6e 6172  onment dictionar
+00010e20: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+00010e30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00010e40: 6c66 2e67 6574 5f77 6f72 6b66 6c6f 775f  lf.get_workflow_
+00010e50: 636f 6d6d 616e 6428 776f 726b 666c 6f77  command(workflow
+00010e60: 3d6d 6f64 656c 2c0a 2020 2020 2020 2020  =model,.        
 00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e80: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00010e90: 3e20 5265 7375 6c74 3a0a 2020 2020 2020  > Result:.      
-00010ea0: 2020 2222 225a 6970 2074 6865 206f 7574    """Zip the out
-00010eb0: 7075 7420 666f 6c64 6572 206f 6620 6120  put folder of a 
-00010ec0: 6a6f 6220 6f6e 2053 6c75 726d 0a0a 2020  job on Slurm..  
-00010ed0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00010ee0: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
-00010ef0: 6174 696f 6e20 2853 7472 696e 6729 3a20  ation (String): 
-00010f00: 466f 6c64 6572 206f 6e20 534c 5552 4d20  Folder on SLURM 
-00010f10: 7769 7468 2074 6865 2022 6461 7461 2f6f  with the "data/o
-00010f20: 7574 220a 2020 2020 2020 2020 2020 2020  ut".            
-00010f30: 2020 2020 7375 6266 6f6c 6465 722e 0a20      subfolder.. 
-00010f40: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-00010f50: 616d 6520 2853 7472 696e 6729 3a20 4e61  ame (String): Na
-00010f60: 6d65 2074 6f20 6769 7665 2074 6f20 7468  me to give to th
-00010f70: 6520 7a69 7066 696c 652e 0a20 2020 2020  e zipfile..     
-00010f80: 2020 2020 2020 2065 6e76 2028 4469 6374         env (Dict
-00010f90: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
-00010fa0: 6f6e 616c 293a 204f 7074 696f 6e61 6c20  onal): Optional 
-00010fb0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00010fc0: 6162 6c65 7320 746f 200a 2020 2020 2020  ables to .      
-00010fd0: 2020 2020 2020 2020 2020 7365 7420 7768            set wh
-00010fe0: 656e 2072 756e 6e69 6e67 2074 6865 2063  en running the c
-00010ff0: 6f6d 6d61 6e64 2e20 4465 6661 756c 7473  ommand. Defaults
-00011000: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
-00011010: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00011020: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
-00011030: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
-00011040: 6520 7a69 7020 6174 7465 6d70 742e 0a20  e zip attempt.. 
-00011050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011060: 2020 2023 207a 6970 0a20 2020 2020 2020     # zip.       
-00011070: 207a 6970 5f63 6d64 203d 2073 656c 662e   zip_cmd = self.
-00011080: 6765 745f 7a69 705f 636f 6d6d 616e 6428  get_zip_command(
-00011090: 6461 7461 5f6c 6f63 6174 696f 6e2c 2066  data_location, f
-000110a0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-000110b0: 206c 6f67 6765 722e 696e 666f 2866 225a   logger.info(f"Z
-000110c0: 6970 7069 6e67 207b 6461 7461 5f6c 6f63  ipping {data_loc
-000110d0: 6174 696f 6e7d 2061 7320 7b66 696c 656e  ation} as {filen
-000110e0: 616d 657d 206f 6e20 536c 7572 6d22 290a  ame} on Slurm").
-000110f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011100: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-00011110: 285b 7a69 705f 636d 645d 2c20 656e 763d  ([zip_cmd], env=
-00011120: 656e 7629 0a0a 2020 2020 6465 6620 6765  env)..    def ge
-00011130: 745f 7a69 705f 636f 6d6d 616e 6428 7365  t_zip_command(se
-00011140: 6c66 2c20 6461 7461 5f6c 6f63 6174 696f  lf, data_locatio
-00011150: 6e3a 2073 7472 2c20 6669 6c65 6e61 6d65  n: str, filename
-00011160: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
-00011170: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011180: 2020 2047 656e 6572 6174 6520 6120 636f     Generate a co
-00011190: 6d6d 616e 6420 7374 7269 6e67 2066 6f72  mmand string for
-000111a0: 207a 6970 7069 6e67 2074 6865 2064 6174   zipping the dat
-000111b0: 6120 6f6e 2053 6c75 726d 2e0a 0a20 2020  a on Slurm...   
-000111c0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000111d0: 2020 2020 2020 2064 6174 615f 6c6f 6361         data_loca
-000111e0: 7469 6f6e 2028 7374 7229 3a20 5468 6520  tion (str): The 
-000111f0: 666f 6c64 6572 2074 6f20 6265 207a 6970  folder to be zip
-00011200: 7065 642e 0a20 2020 2020 2020 2020 2020  ped..           
-00011210: 2066 696c 656e 616d 6520 2873 7472 293a   filename (str):
-00011220: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00011230: 207a 6970 2061 7263 6869 7665 2066 696c   zip archive fil
-00011240: 6520 746f 2065 7874 7261 6374 2e0a 2020  e to extract..  
-00011250: 2020 2020 2020 2020 2020 2020 2020 5769                Wi
-00011260: 7468 6f75 7420 6578 7465 6e73 696f 6e2e  thout extension.
-00011270: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00011280: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00011290: 7472 3a20 5468 6520 636f 6d6d 616e 6420  tr: The command 
-000112a0: 746f 2063 7265 6174 6520 7468 6520 7a69  to create the zi
-000112b0: 7020 6669 6c65 2e0a 2020 2020 2020 2020  p file..        
-000112c0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-000112d0: 726e 2073 656c 662e 5f5a 4950 5f43 4d44  rn self._ZIP_CMD
-000112e0: 2e66 6f72 6d61 7428 6669 6c65 6e61 6d65  .format(filename
-000112f0: 3d66 696c 656e 616d 652c 0a20 2020 2020  =filename,.     
-00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011310: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011320: 6174 615f 6c6f 6361 7469 6f6e 3d64 6174  ata_location=dat
-00011330: 615f 6c6f 6361 7469 6f6e 290a 0a20 2020  a_location)..   
-00011340: 2064 6566 2067 6574 5f6c 6f67 6669 6c65   def get_logfile
-00011350: 5f66 726f 6d5f 736c 7572 6d28 7365 6c66  _from_slurm(self
-00011360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011380: 2073 6c75 726d 5f6a 6f62 5f69 643a 2073   slurm_job_id: s
-00011390: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 206c 6f63 616c 5f74 6d70 5f73 746f     local_tmp_sto
-000113c0: 7261 6765 3a20 7374 7220 3d20 222f 746d  rage: str = "/tm
-000113d0: 702f 222c 0a20 2020 2020 2020 2020 2020  p/",.           
-000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 6c6f 6766 696c 653a 2073 7472      logfile: str
-00011400: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011420: 2020 2020 2020 2029 202d 3e20 5475 706c         ) -> Tupl
-00011430: 655b 7374 722c 2073 7472 2c20 5472 616e  e[str, str, Tran
-00011440: 7366 6572 5265 7375 6c74 5d3a 0a20 2020  sferResult]:.   
-00011450: 2020 2020 2022 2222 436f 7079 2074 6865       """Copy the
-00011460: 206c 6f67 6669 6c65 206f 6620 7468 6520   logfile of the 
-00011470: 6769 7665 6e20 534c 5552 4d20 6a6f 6220  given SLURM job 
-00011480: 746f 2074 6865 206c 6f63 616c 2073 6572  to the local ser
-00011490: 7665 722e 0a0a 2020 2020 2020 2020 4e6f  ver...        No
-000114a0: 7465 2061 626f 7574 2028 5472 616e 7366  te about (Transf
-000114b0: 6572 2952 6573 756c 743a 0a0a 2020 2020  er)Result:..    
-000114c0: 2020 2020 556e 6c69 6b65 2073 696d 696c      Unlike simil
-000114d0: 6172 2063 6c61 7373 6573 2073 7563 6820  ar classes such 
-000114e0: 6173 2069 6e76 6f6b 652e 7275 6e6e 6572  as invoke.runner
-000114f0: 732e 5265 7375 6c74 0a20 2020 2020 2020  s.Result.       
-00011500: 206f 7220 6661 6272 6963 2e72 756e 6e65   or fabric.runne
-00011510: 7273 2e52 6573 756c 740a 2020 2020 2020  rs.Result.      
-00011520: 2020 2877 6869 6368 2068 6176 6520 6120    (which have a 
-00011530: 636f 6e63 6570 7420 6f66 20e2 809c 7761  concept of ...wa
-00011540: 726e 2061 6e64 2072 6574 7572 6e20 616e  rn and return an
-00011550: 7977 6179 7320 6f6e 2066 6169 6c75 7265  yways on failure
-00011560: e280 9d29 0a20 2020 2020 2020 2074 6869  ...).        thi
-00011570: 7320 636c 6173 7320 6861 7320 6e6f 2075  s class has no u
-00011580: 7365 6675 6c20 7472 7574 6869 6e65 7373  seful truthiness
-00011590: 2062 6568 6176 696f 722e 0a20 2020 2020   behavior..     
-000115a0: 2020 2049 6620 6120 6669 6c65 2074 7261     If a file tra
-000115b0: 6e73 6665 7220 6661 696c 732c 2073 6f6d  nsfer fails, som
-000115c0: 6520 6578 6365 7074 696f 6e20 7769 6c6c  e exception will
-000115d0: 2062 6520 7261 6973 6564 2c0a 2020 2020   be raised,.    
-000115e0: 2020 2020 6569 7468 6572 2061 6e20 4f53      either an OS
-000115f0: 4572 726f 7220 6f72 2061 6e20 6572 726f  Error or an erro
-00011600: 7220 6672 6f6d 2077 6974 6869 6e20 5061  r from within Pa
-00011610: 7261 6d69 6b6f 2e0a 0a20 2020 2020 2020  ramiko...       
-00011620: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00011630: 2020 2073 6c75 726d 5f6a 6f62 5f69 6420     slurm_job_id 
-00011640: 2873 7472 293a 2054 6865 2049 4420 6f66  (str): The ID of
-00011650: 2074 6865 2053 4c55 524d 206a 6f62 2e0a   the SLURM job..
-00011660: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00011670: 6c5f 746d 705f 7374 6f72 6167 6520 2873  l_tmp_storage (s
-00011680: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
-00011690: 6174 6820 746f 2073 746f 7265 2074 6865  ath to store the
-000116a0: 206c 6f67 6669 6c65 200a 2020 2020 2020   logfile .      
-000116b0: 2020 2020 2020 2020 2020 6c6f 6361 6c6c            locall
-000116c0: 792e 2044 6566 6175 6c74 7320 746f 2022  y. Defaults to "
-000116d0: 2f74 6d70 2f22 2e0a 2020 2020 2020 2020  /tmp/"..        
-000116e0: 2020 2020 6c6f 6766 696c 6520 2873 7472      logfile (str
-000116f0: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
-00011700: 6820 746f 2074 6865 206c 6f67 6669 6c65  h to the logfile
-00011710: 206f 6e20 7468 6520 534c 5552 4d20 7365   on the SLURM se
-00011720: 7276 6572 2e0a 2020 2020 2020 2020 2020  rver..          
-00011730: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00011740: 6f20 4e6f 6e65 2e0a 0a20 2020 2020 2020  o None...       
-00011750: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00011760: 2020 2020 2020 5475 706c 653a 2064 6972        Tuple: dir
-00011770: 6563 746f 7279 2c20 6675 6c6c 2070 6174  ectory, full pat
-00011780: 6820 6f66 2074 6865 206c 6f67 6669 6c65  h of the logfile
-00011790: 2c20 616e 6420 5472 616e 7366 6572 5265  , and TransferRe
-000117a0: 7375 6c74 0a20 2020 2020 2020 2022 2222  sult.        """
-000117b0: 0a20 2020 2020 2020 2069 6620 6c6f 6766  .        if logf
-000117c0: 696c 6520 6973 204e 6f6e 653a 0a20 2020  ile is None:.   
-000117d0: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-000117e0: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
-000117f0: 0a20 2020 2020 2020 206c 6f67 6669 6c65  .        logfile
-00011800: 203d 206c 6f67 6669 6c65 2e66 6f72 6d61   = logfile.forma
-00011810: 7428 736c 7572 6d5f 6a6f 625f 6964 3d73  t(slurm_job_id=s
-00011820: 6c75 726d 5f6a 6f62 5f69 6429 0a20 2020  lurm_job_id).   
-00011830: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00011840: 2866 2243 6f70 7969 6e67 206c 6f67 6669  (f"Copying logfi
-00011850: 6c65 207b 6c6f 6766 696c 657d 2066 726f  le {logfile} fro
-00011860: 6d20 536c 7572 6d5c 0a20 2020 2020 2020  m Slurm\.       
-00011870: 2020 2020 2074 6f20 7b6c 6f63 616c 5f74       to {local_t
-00011880: 6d70 5f73 746f 7261 6765 7d22 290a 2020  mp_storage}").  
-00011890: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-000118a0: 656c 662e 6765 7428 0a20 2020 2020 2020  elf.get(.       
-000118b0: 2020 2020 2072 656d 6f74 653d 6c6f 6766       remote=logf
-000118c0: 696c 652c 0a20 2020 2020 2020 2020 2020  ile,.           
-000118d0: 206c 6f63 616c 3d6c 6f63 616c 5f74 6d70   local=local_tmp
-000118e0: 5f73 746f 7261 6765 290a 2020 2020 2020  _storage).      
-000118f0: 2020 6578 706f 7274 5f66 696c 6520 3d20    export_file = 
-00011900: 6c6f 6361 6c5f 746d 705f 7374 6f72 6167  local_tmp_storag
-00011910: 652b 6c6f 6766 696c 650a 2020 2020 2020  e+logfile.      
-00011920: 2020 7265 7475 726e 206c 6f63 616c 5f74    return local_t
-00011930: 6d70 5f73 746f 7261 6765 2c20 6578 706f  mp_storage, expo
-00011940: 7274 5f66 696c 652c 2072 6573 756c 740a  rt_file, result.
-00011950: 0a20 2020 2064 6566 2067 6574 5f75 6e7a  .    def get_unz
-00011960: 6970 5f63 6f6d 6d61 6e64 2873 656c 662c  ip_command(self,
-00011970: 207a 6970 6669 6c65 3a20 7374 722c 0a20   zipfile: str,. 
-00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011990: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
-000119a0: 6669 6c65 7479 7065 733a 2073 7472 203d  filetypes: str =
-000119b0: 2022 2a2e 7a61 7272 202a 2e74 6966 6620   "*.zarr *.tiff 
-000119c0: 2a2e 7469 6622 0a20 2020 2020 2020 2020  *.tif".         
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2029 202d 3e20 7374 723a 0a20 2020 2020   ) -> str:.     
-000119f0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00011a00: 656e 6572 6174 6520 6120 636f 6d6d 616e  enerate a comman
-00011a10: 6420 7374 7269 6e67 2066 6f72 2075 6e7a  d string for unz
-00011a20: 6970 7069 6e67 2061 2064 6174 6120 6172  ipping a data ar
-00011a30: 6368 6976 6520 616e 6420 6372 6561 7469  chive and creati
-00011a40: 6e67 0a20 2020 2020 2020 2072 6571 7569  ng.        requi
-00011a50: 7265 6420 6469 7265 6374 6f72 6965 7320  red directories 
-00011a60: 666f 7220 536c 7572 6d20 6a6f 6273 2e0a  for Slurm jobs..
-00011a70: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00011a80: 2020 2020 2020 2020 2020 207a 6970 6669             zipfi
-00011a90: 6c65 2028 7374 7229 3a20 5468 6520 6e61  le (str): The na
-00011aa0: 6d65 206f 6620 7468 6520 7a69 7020 6172  me of the zip ar
-00011ab0: 6368 6976 6520 6669 6c65 2074 6f20 6578  chive file to ex
-00011ac0: 7472 6163 742e 0a20 2020 2020 2020 2020  tract..         
-00011ad0: 2020 2020 2020 2057 6974 686f 7574 2065         Without e
-00011ae0: 7874 656e 7369 6f6e 2e0a 2020 2020 2020  xtension..      
-00011af0: 2020 2020 2020 6669 6c74 6572 5f66 696c        filter_fil
-00011b00: 6574 7970 6573 2028 7374 722c 206f 7074  etypes (str, opt
-00011b10: 696f 6e61 6c29 3a20 4120 7370 6163 652d  ional): A space-
-00011b20: 7365 7061 7261 7465 6420 7374 7269 6e67  separated string
-00011b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b40: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00011b50: 6669 6c65 2065 7874 656e 7369 6f6e 7320  file extensions 
-00011b60: 746f 2065 7874 7261 6374 2066 726f 6d20  to extract from 
-00011b70: 7468 6520 7a69 7020 6669 6c65 2e0a 2020  the zip file..  
-00011b80: 2020 2020 2020 2020 2020 2020 2020 452e                E.
-00011b90: 672e 2064 6566 6175 6c74 7320 746f 2022  g. defaults to "
-00011ba0: 2a2e 7a61 7272 202a 2e74 6966 6620 2a2e  *.zarr *.tiff *.
-00011bb0: 7469 6622 2e0a 2020 2020 2020 2020 2020  tif"..          
-00011bc0: 2020 2020 2020 5365 7474 696e 6720 7468        Setting th
-00011bd0: 6973 2061 7267 756d 656e 7420 746f 2060  is argument to `
-00011be0: 4e6f 6e65 6020 7769 6c6c 206f 6d69 7420  None` will omit 
-00011bf0: 7468 6520 6669 6c65 0a20 2020 2020 2020  the file.       
-00011c00: 2020 2020 2020 2020 2066 696c 7465 7220           filter 
-00011c10: 616e 6420 6578 7472 6163 7420 616c 6c20  and extract all 
-00011c20: 6669 6c65 732e 0a0a 2020 2020 2020 2020  files...        
-00011c30: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00011c40: 2020 2020 2073 7472 3a0a 2020 2020 2020       str:.      
-00011c50: 2020 2020 2020 2020 2020 5468 6520 636f            The co
-00011c60: 6d6d 616e 6420 746f 2065 7874 7261 6374  mmand to extract
-00011c70: 2074 6865 2073 7065 6369 6669 6564 0a20   the specified. 
-00011c80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011c90: 696c 6574 7970 6573 2066 726f 6d20 7468  iletypes from th
-00011ca0: 6520 7a69 7020 6669 6c65 2e0a 2020 2020  e zip file..    
-00011cb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011cc0: 756e 7a69 705f 636d 6420 3d20 6622 6d6b  unzip_cmd = f"mk
-00011cd0: 6469 7220 7b73 656c 662e 736c 7572 6d5f  dir {self.slurm_
-00011ce0: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
-00011cf0: 696c 657d 205c 0a20 2020 2020 2020 2020  ile} \.         
-00011d00: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00011d10: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-00011d20: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
-00011d30: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00011d40: 2020 2020 2020 207b 7365 6c66 2e73 6c75         {self.slu
-00011d50: 726d 5f64 6174 615f 7061 7468 7d2f 7b7a  rm_data_path}/{z
-00011d60: 6970 6669 6c65 7d2f 6461 7461 2f69 6e20  ipfile}/data/in 
-00011d70: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00011d80: 2020 2020 2020 7b73 656c 662e 736c 7572        {self.slur
-00011d90: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
-00011da0: 7066 696c 657d 2f64 6174 612f 6f75 7420  pfile}/data/out 
-00011db0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00011dc0: 2020 2020 2020 7b73 656c 662e 736c 7572        {self.slur
-00011dd0: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
-00011de0: 7066 696c 657d 2f64 6174 612f 6774 3b20  pfile}/data/gt; 
-00011df0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00011e00: 2020 2020 2020 377a 2078 202d 7920 2d6f        7z x -y -o
-00011e10: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
-00011e20: 5f70 6174 687d 2f7b 7a69 7066 696c 657d  _path}/{zipfile}
-00011e30: 2f64 6174 612f 696e 205c 0a20 2020 2020  /data/in \.     
-00011e40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00011e50: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
-00011e60: 7061 7468 7d2f 7b7a 6970 6669 6c65 7d2e  path}/{zipfile}.
-00011e70: 7a69 7020 7b66 696c 7465 725f 6669 6c65  zip {filter_file
-00011e80: 7479 7065 737d 220a 0a20 2020 2020 2020  types}"..       
-00011e90: 2072 6574 7572 6e20 756e 7a69 705f 636d   return unzip_cm
-00011ea0: 640a 0a20 2020 2064 6566 2067 6574 5f69  d..    def get_i
-00011eb0: 6d61 6765 5f76 6572 7369 6f6e 735f 616e  mage_versions_an
-00011ec0: 645f 6461 7461 5f66 696c 6573 2873 656c  d_data_files(sel
-00011ed0: 662c 206d 6f64 656c 3a20 7374 720a 2020  f, model: str.  
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
-00011f10: 6c65 5b4c 6973 745b 7374 725d 2c20 4c69  le[List[str], Li
-00011f20: 7374 5b73 7472 5d5d 3a0a 2020 2020 2020  st[str]]:.      
-00011f30: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00011f40: 7472 6965 7665 2074 6865 2061 7661 696c  trieve the avail
-00011f50: 6162 6c65 2069 6d61 6765 2076 6572 7369  able image versi
-00011f60: 6f6e 7320 616e 6420 696e 7075 7420 6461  ons and input da
-00011f70: 7461 2066 696c 6573 2066 6f72 2061 0a20  ta files for a. 
-00011f80: 2020 2020 2020 2067 6976 656e 206d 6f64         given mod
-00011f90: 656c 2e0a 0a20 2020 2020 2020 2041 7267  el...        Arg
-00011fa0: 733a 0a20 2020 2020 2020 2020 2020 206d  s:.            m
-00011fb0: 6f64 656c 2028 7374 7229 3a20 5468 6520  odel (str): The 
-00011fc0: 6e61 6d65 206f 6620 7468 6520 6d6f 6465  name of the mode
-00011fd0: 6c20 746f 2071 7565 7279 2066 6f72 2e0a  l to query for..
-00011fe0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00011ff0: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
-00012000: 706c 655b 4c69 7374 5b73 7472 5d2c 204c  ple[List[str], L
-00012010: 6973 745b 7374 725d 5d3a 0a20 2020 2020  ist[str]]:.     
-00012020: 2020 2020 2020 2020 2020 2041 2074 7570             A tup
-00012030: 6c65 2063 6f6e 7461 696e 696e 6720 7477  le containing tw
-00012040: 6f20 6c69 7374 733a 0a20 2020 2020 2020  o lists:.       
-00012050: 2020 2020 2020 2020 202d 2054 6865 2066           - The f
-00012060: 6972 7374 206c 6973 7420 696e 636c 7564  irst list includ
-00012070: 6573 2074 6865 2061 7661 696c 6162 6c65  es the available
-00012080: 2069 6d61 6765 2076 6572 7369 6f6e 732c   image versions,
-00012090: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000120a0: 2020 2020 2020 736f 7274 6564 2069 6e20        sorted in 
-000120b0: 6465 7363 656e 6469 6e67 206f 7264 6572  descending order
-000120c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000120d0: 2020 2d20 5468 6520 7365 636f 6e64 206c    - The second l
-000120e0: 6973 7420 696e 636c 7564 6573 2074 6865  ist includes the
-000120f0: 2061 7661 696c 6162 6c65 2064 6174 6120   available data 
-00012100: 6669 6c65 732e 0a0a 2020 2020 2020 2020  files...        
-00012110: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00012120: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00012130: 4966 2074 6865 2070 726f 7669 6465 6420  If the provided 
-00012140: 6d6f 6465 6c20 6973 206e 6f74 2066 6f75  model is not fou
-00012150: 6e64 2069 6e20 7468 650a 2020 2020 2020  nd in the.      
-00012160: 2020 2020 2020 2020 2020 536c 7572 6d43            SlurmC
-00012170: 6c69 656e 7427 7320 6b6e 6f77 6e20 6d6f  lient's known mo
-00012180: 6465 6c20 7061 7468 732e 0a20 2020 2020  del paths..     
-00012190: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000121a0: 6d61 6765 5f70 6174 6820 3d20 7365 6c66  mage_path = self
-000121b0: 2e73 6c75 726d 5f6d 6f64 656c 5f70 6174  .slurm_model_pat
-000121c0: 6873 2e67 6574 286d 6f64 656c 290a 2020  hs.get(model).  
-000121d0: 2020 2020 2020 6966 206e 6f74 2069 6d61        if not ima
-000121e0: 6765 5f70 6174 683a 0a20 2020 2020 2020  ge_path:.       
-000121f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00012200: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00012210: 2020 2020 2020 2066 224e 6f20 7061 7468         f"No path
-00012220: 206b 6e6f 776e 2066 6f72 2070 726f 7669   known for provi
-00012230: 6465 6420 6d6f 6465 6c20 7b6d 6f64 656c  ded model {model
-00012240: 7d2c 205c 0a20 2020 2020 2020 2020 2020  }, \.           
-00012250: 2020 2020 2020 2020 2069 6e20 7b73 656c           in {sel
-00012260: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
-00012270: 7468 737d 2229 0a20 2020 2020 2020 2063  ths}").        c
-00012280: 6d64 6c69 7374 203d 205b 0a20 2020 2020  mdlist = [.     
-00012290: 2020 2020 2020 2073 656c 662e 5f56 4552         self._VER
-000122a0: 5349 4f4e 5f43 4d44 2e66 6f72 6d61 7428  SION_CMD.format(
-000122b0: 736c 7572 6d5f 696d 6167 6573 5f70 6174  slurm_images_pat
-000122c0: 683d 7365 6c66 2e73 6c75 726d 5f69 6d61  h=self.slurm_ima
-000122d0: 6765 735f 7061 7468 2c0a 2020 2020 2020  ges_path,.      
-000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012300: 6d61 6765 5f70 6174 683d 696d 6167 655f  mage_path=image_
-00012310: 7061 7468 292c 0a20 2020 2020 2020 2020  path),.         
-00012320: 2020 2073 656c 662e 5f44 4154 415f 434d     self._DATA_CM
-00012330: 442e 666f 726d 6174 2873 6c75 726d 5f64  D.format(slurm_d
-00012340: 6174 615f 7061 7468 3d73 656c 662e 736c  ata_path=self.sl
-00012350: 7572 6d5f 6461 7461 5f70 6174 6829 5d0a  urm_data_path)].
-00012360: 2020 2020 2020 2020 2320 7370 6c69 7420          # split 
-00012370: 7265 7370 6f6e 7365 7320 7065 7220 636f  responses per co
-00012380: 6d6d 616e 640a 2020 2020 2020 2020 7265  mmand.        re
-00012390: 7370 6f6e 7365 5f6c 6973 7420 3d20 7365  sponse_list = se
-000123a0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 735f  lf.run_commands_
-000123b0: 7370 6c69 745f 6f75 7428 636d 646c 6973  split_out(cmdlis
-000123c0: 7429 0a20 2020 2020 2020 2023 2073 706c  t).        # spl
-000123d0: 6974 206c 696e 6573 2066 7572 7468 6572  it lines further
-000123e0: 2069 6e74 6f20 7375 626c 6973 7473 0a20   into sublists. 
-000123f0: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
-00012400: 6c69 7374 203d 205b 7265 7370 6f6e 7365  list = [response
-00012410: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
-00012420: 5c6e 2729 0a20 2020 2020 2020 2020 2020  \n').           
-00012430: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012440: 7220 7265 7370 6f6e 7365 2069 6e20 7265  r response in re
-00012450: 7370 6f6e 7365 5f6c 6973 745d 0a20 2020  sponse_list].   
-00012460: 2020 2020 2072 6573 706f 6e73 655f 6c69       response_li
-00012470: 7374 5b30 5d20 3d20 736f 7274 6564 2872  st[0] = sorted(r
-00012480: 6573 706f 6e73 655f 6c69 7374 5b30 5d2c  esponse_list[0],
-00012490: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
-000124a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000124b0: 7370 6f6e 7365 5f6c 6973 745b 305d 2c20  sponse_list[0], 
-000124c0: 7265 7370 6f6e 7365 5f6c 6973 745b 315d  response_list[1]
-000124d0: 0a0a 2020 2020 6465 6620 6765 745f 616c  ..    def get_al
-000124e0: 6c5f 696d 6167 655f 7665 7273 696f 6e73  l_image_versions
-000124f0: 5f61 6e64 5f64 6174 615f 6669 6c65 7328  _and_data_files(
-00012500: 7365 6c66 0a20 2020 2020 2020 2020 2020  self.           
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012530: 2020 2029 202d 3e20 5475 706c 655b 4469     ) -> Tuple[Di
-00012540: 6374 5b73 7472 2c20 4c69 7374 5b73 7472  ct[str, List[str
-00012550: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 2020 2020 2020 2020 2020 204c 6973               Lis
-00012590: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
-000125a0: 2022 2222 5265 7472 6965 7665 2061 6c6c   """Retrieve all
-000125b0: 2061 7661 696c 6162 6c65 2069 6d61 6765   available image
-000125c0: 2076 6572 7369 6f6e 7320 616e 6420 6461   versions and da
-000125d0: 7461 2066 696c 6573 2066 726f 6d0a 2020  ta files from.  
-000125e0: 2020 2020 2020 7468 6520 536c 7572 6d20        the Slurm 
-000125f0: 636c 7573 7465 722e 0a0a 2020 2020 2020  cluster...      
-00012600: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00012610: 2020 2020 2020 5475 706c 655b 4469 6374        Tuple[Dict
-00012620: 5b73 7472 2c20 4c69 7374 5b73 7472 5d5d  [str, List[str]]
-00012630: 2c20 4c69 7374 5b73 7472 5d5d 3a0a 2020  , List[str]]:.  
-00012640: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00012650: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-00012660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012670: 2020 2d20 4120 6469 6374 696f 6e61 7279    - A dictionary
-00012680: 206d 6170 7069 6e67 206d 6f64 656c 7320   mapping models 
-00012690: 746f 2061 7661 696c 6162 6c65 2076 6572  to available ver
-000126a0: 7369 6f6e 732e 0a20 2020 2020 2020 2020  sions..         
-000126b0: 2020 2020 2020 202d 2041 206c 6973 7420         - A list 
-000126c0: 6f66 2061 7661 696c 6162 6c65 2069 6e70  of available inp
-000126d0: 7574 2064 6174 6120 666f 6c64 6572 732e  ut data folders.
-000126e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000126f0: 2020 2020 2072 6573 756c 7464 6963 7420       resultdict 
-00012700: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
-00012710: 6c69 7374 203d 205b 5d0a 0a20 2020 2020  list = []..     
-00012720: 2020 2066 6f72 2070 6174 6820 696e 2073     for path in s
-00012730: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-00012740: 7061 7468 732e 7661 6c75 6573 2829 3a0a  paths.values():.
-00012750: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00012760: 636d 6420 3d20 7365 6c66 2e5f 5645 5253  cmd = self._VERS
-00012770: 494f 4e5f 434d 442e 666f 726d 6174 280a  ION_CMD.format(.
-00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012790: 736c 7572 6d5f 696d 6167 6573 5f70 6174  slurm_images_pat
-000127a0: 683d 7365 6c66 2e73 6c75 726d 5f69 6d61  h=self.slurm_ima
-000127b0: 6765 735f 7061 7468 2c0a 2020 2020 2020  ges_path,.      
-000127c0: 2020 2020 2020 2020 2020 696d 6167 655f            image_
-000127d0: 7061 7468 3d70 6174 6829 0a20 2020 2020  path=path).     
-000127e0: 2020 2020 2020 2063 6d64 6c69 7374 2e61         cmdlist.a
-000127f0: 7070 656e 6428 7061 7468 636d 6429 0a0a  ppend(pathcmd)..
-00012800: 2020 2020 2020 2020 2320 4164 6420 6461          # Add da
-00012810: 7461 2070 6174 6820 746f 6f0a 2020 2020  ta path too.    
-00012820: 2020 2020 636d 646c 6973 742e 6170 7065      cmdlist.appe
-00012830: 6e64 2873 656c 662e 5f44 4154 415f 434d  nd(self._DATA_CM
-00012840: 442e 666f 726d 6174 280a 2020 2020 2020  D.format(.      
-00012850: 2020 2020 2020 736c 7572 6d5f 6461 7461        slurm_data
-00012860: 5f70 6174 683d 7365 6c66 2e73 6c75 726d  _path=self.slurm
-00012870: 5f64 6174 615f 7061 7468 2929 0a0a 2020  _data_path))..  
-00012880: 2020 2020 2020 2320 5370 6c69 7420 7265        # Split re
-00012890: 7370 6f6e 7365 7320 7065 7220 636f 6d6d  sponses per comm
-000128a0: 616e 640a 2020 2020 2020 2020 7265 7370  and.        resp
-000128b0: 6f6e 7365 5f6c 6973 7420 3d20 7365 6c66  onse_list = self
-000128c0: 2e72 756e 5f63 6f6d 6d61 6e64 735f 7370  .run_commands_sp
-000128d0: 6c69 745f 6f75 7428 636d 646c 6973 7429  lit_out(cmdlist)
-000128e0: 0a0a 2020 2020 2020 2020 2320 5370 6c69  ..        # Spli
-000128f0: 7420 6c69 6e65 7320 6675 7274 6865 7220  t lines further 
-00012900: 696e 746f 2073 7562 6c69 7374 730a 2020  into sublists.  
-00012910: 2020 2020 2020 7265 7370 6f6e 7365 5f6c        response_l
-00012920: 6973 7420 3d20 5b72 6573 706f 6e73 652e  ist = [response.
-00012930: 7374 7269 7028 292e 7370 6c69 7428 275c  strip().split('\
-00012940: 6e27 290a 2020 2020 2020 2020 2020 2020  n').            
-00012950: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00012960: 2072 6573 706f 6e73 6520 696e 2072 6573   response in res
-00012970: 706f 6e73 655f 6c69 7374 5d0a 0a20 2020  ponse_list]..   
-00012980: 2020 2020 2066 6f72 2069 2c20 6b20 696e       for i, k in
-00012990: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-000129a0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-000129b0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000129c0: 2320 5265 7475 726e 2068 6967 6865 7374  # Return highest
-000129d0: 2076 6572 7369 6f6e 2066 6972 7374 0a20   version first. 
-000129e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000129f0: 7464 6963 745b 6b5d 203d 2073 6f72 7465  tdict[k] = sorte
-00012a00: 6428 7265 7370 6f6e 7365 5f6c 6973 745b  d(response_list[
-00012a10: 695d 2c20 7265 7665 7273 653d 5472 7565  i], reverse=True
-00012a20: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00012a30: 6e20 7265 7375 6c74 6469 6374 2c20 7265  n resultdict, re
-00012a40: 7370 6f6e 7365 5f6c 6973 745b 2d31 5d0a  sponse_list[-1].
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
+00010ea0: 6e3d 696d 6167 655f 7665 7273 696f 6e2c  n=image_version,
+00010eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+00010ee0: 6461 7461 3d69 6e70 7574 5f64 6174 612c  data=input_data,
+00010ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2020 2020 2020 2020 2020 656d 6169 6c3d            email=
+00010f20: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 7469 6d65 3d74 696d 652c 0a20 2020 2020  time=time,.     
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 6370 5f6d 6f64 656c 3d63 705f      cp_model=cp_
+00010f90: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fc0: 6e75 635f 6368 616e 6e65 6c3d 6e75 635f  nuc_channel=nuc_
+00010fd0: 6368 616e 6e65 6c2c 0a20 2020 2020 2020  channel,.       
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 7072 6f62 5f74 6872 6573 686f 6c64    prob_threshold
+00011010: 3d70 726f 625f 7468 7265 7368 6f6c 642c  =prob_threshold,
+00011020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 2020 2020 2020 2020 6365 6c6c 5f64            cell_d
+00011050: 6961 6d65 7465 723d 6365 6c6c 5f64 6961  iameter=cell_dia
+00011060: 6d65 7465 722c 0a20 2020 2020 2020 2020  meter,.         
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 7573 655f 6770 753d 7573 655f 6770 7529  use_gpu=use_gpu)
+000110a0: 0a0a 2020 2020 6465 6620 636f 7079 5f7a  ..    def copy_z
+000110b0: 6970 5f6c 6f63 616c 6c79 2873 656c 662c  ip_locally(self,
+000110c0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
+000110d0: 6765 3a20 7374 722c 2066 696c 656e 616d  ge: str, filenam
+000110e0: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011100: 2920 2d3e 2054 7261 6e73 6665 7252 6573  ) -> TransferRes
+00011110: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
+00011120: 2043 6f70 7920 6120 7a69 7020 6669 6c65   Copy a zip file
+00011130: 2066 726f 6d20 536c 7572 6d20 746f 2074   from Slurm to t
+00011140: 6865 206c 6f63 616c 2073 6572 7665 722e  he local server.
+00011150: 0a0a 2020 2020 2020 2020 4e6f 7465 2061  ..        Note a
+00011160: 626f 7574 2028 5472 616e 7366 6572 2952  bout (Transfer)R
+00011170: 6573 756c 743a 0a0a 2020 2020 2020 2020  esult:..        
+00011180: 556e 6c69 6b65 2073 696d 696c 6172 2063  Unlike similar c
+00011190: 6c61 7373 6573 2073 7563 6820 6173 2069  lasses such as i
+000111a0: 6e76 6f6b 652e 7275 6e6e 6572 732e 5265  nvoke.runners.Re
+000111b0: 7375 6c74 206f 720a 2020 2020 2020 2020  sult or.        
+000111c0: 6661 6272 6963 2e72 756e 6e65 7273 2e52  fabric.runners.R
+000111d0: 6573 756c 740a 2020 2020 2020 2020 2877  esult.        (w
+000111e0: 6869 6368 2068 6176 6520 6120 636f 6e63  hich have a conc
+000111f0: 6570 7420 6f66 20e2 809c 7761 726e 2061  ept of ...warn a
+00011200: 6e64 2072 6574 7572 6e20 616e 7977 6179  nd return anyway
+00011210: 7320 6f6e 2066 6169 6c75 7265 e280 9d29  s on failure...)
+00011220: 0a20 2020 2020 2020 2074 6869 7320 636c  .        this cl
+00011230: 6173 7320 6861 7320 6e6f 2075 7365 6675  ass has no usefu
+00011240: 6c20 7472 7574 6869 6e65 7373 2062 6568  l truthiness beh
+00011250: 6176 696f 722e 0a20 2020 2020 2020 2049  avior..        I
+00011260: 6620 6120 6669 6c65 2074 7261 6e73 6665  f a file transfe
+00011270: 7220 6661 696c 732c 2073 6f6d 6520 6578  r fails, some ex
+00011280: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
+00011290: 7261 6973 6564 2c0a 2020 2020 2020 2020  raised,.        
+000112a0: 6569 7468 6572 2061 6e20 4f53 4572 726f  either an OSErro
+000112b0: 7220 6f72 2061 6e20 6572 726f 7220 6672  r or an error fr
+000112c0: 6f6d 2077 6974 6869 6e20 5061 7261 6d69  om within Parami
+000112d0: 6b6f 2e0a 0a20 2020 2020 2020 2041 7267  ko...        Arg
+000112e0: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+000112f0: 6f63 616c 5f74 6d70 5f73 746f 7261 6765  ocal_tmp_storage
+00011300: 2028 5374 7269 6e67 293a 2050 6174 6820   (String): Path 
+00011310: 746f 2073 746f 7265 2074 6865 207a 6970  to store the zip
+00011320: 2066 696c 6520 6c6f 6361 6c6c 792e 0a20   file locally.. 
+00011330: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+00011340: 616d 6520 2853 7472 696e 6729 3a20 5a69  ame (String): Zi
+00011350: 7020 6669 6c65 6e61 6d65 206f 6e20 536c  p filename on Sl
+00011360: 7572 6d2e 0a0a 2020 2020 2020 2020 5265  urm...        Re
+00011370: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00011380: 2020 2054 7261 6e73 6665 7252 6573 756c     TransferResul
+00011390: 743a 2054 6865 2072 6573 756c 7420 6f66  t: The result of
+000113a0: 2074 6865 2073 6370 2061 7474 656d 7074   the scp attempt
+000113b0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000113c0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+000113d0: 6f28 6622 436f 7079 696e 6720 7a69 7020  o(f"Copying zip 
+000113e0: 7b66 696c 656e 616d 657d 2066 726f 6d5c  {filename} from\
+000113f0: 0a20 2020 2020 2020 2020 2020 2053 6c75  .            Slu
+00011400: 726d 2074 6f20 7b6c 6f63 616c 5f74 6d70  rm to {local_tmp
+00011410: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
+00011420: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00011430: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
+00011440: 2072 656d 6f74 653d 6622 7b66 696c 656e   remote=f"{filen
+00011450: 616d 657d 2e7a 6970 222c 0a20 2020 2020  ame}.zip",.     
+00011460: 2020 2020 2020 206c 6f63 616c 3d6c 6f63         local=loc
+00011470: 616c 5f74 6d70 5f73 746f 7261 6765 290a  al_tmp_storage).
+00011480: 0a20 2020 2064 6566 207a 6970 5f64 6174  .    def zip_dat
+00011490: 615f 6f6e 5f73 6c75 726d 5f73 6572 7665  a_on_slurm_serve
+000114a0: 7228 7365 6c66 2c20 6461 7461 5f6c 6f63  r(self, data_loc
+000114b0: 6174 696f 6e3a 2073 7472 2c20 6669 6c65  ation: str, file
+000114c0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2020 2020 2020 2020 2020 656e 763a              env:
+000114f0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00011500: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
+00011510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011530: 2020 2920 2d3e 2052 6573 756c 743a 0a20    ) -> Result:. 
+00011540: 2020 2020 2020 2022 2222 5a69 7020 7468         """Zip th
+00011550: 6520 6f75 7470 7574 2066 6f6c 6465 7220  e output folder 
+00011560: 6f66 2061 206a 6f62 206f 6e20 536c 7572  of a job on Slur
+00011570: 6d0a 0a20 2020 2020 2020 2041 7267 733a  m..        Args:
+00011580: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00011590: 615f 6c6f 6361 7469 6f6e 2028 5374 7269  a_location (Stri
+000115a0: 6e67 293a 2046 6f6c 6465 7220 6f6e 2053  ng): Folder on S
+000115b0: 4c55 524d 2077 6974 6820 7468 6520 2264  LURM with the "d
+000115c0: 6174 612f 6f75 7422 0a20 2020 2020 2020  ata/out".       
+000115d0: 2020 2020 2020 2020 2073 7562 666f 6c64           subfold
+000115e0: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+000115f0: 6669 6c65 6e61 6d65 2028 5374 7269 6e67  filename (String
+00011600: 293a 204e 616d 6520 746f 2067 6976 6520  ): Name to give 
+00011610: 746f 2074 6865 207a 6970 6669 6c65 2e0a  to the zipfile..
+00011620: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+00011630: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
+00011640: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
+00011650: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
+00011660: 2076 6172 6961 626c 6573 2074 6f20 0a20   variables to . 
+00011670: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011680: 6574 2077 6865 6e20 7275 6e6e 696e 6720  et when running 
+00011690: 7468 6520 636f 6d6d 616e 642e 2044 6566  the command. Def
+000116a0: 6175 6c74 7320 746f 204e 6f6e 652e 0a0a  aults to None...
+000116b0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000116c0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+000116d0: 756c 743a 2054 6865 2072 6573 756c 7420  ult: The result 
+000116e0: 6f66 2074 6865 207a 6970 2061 7474 656d  of the zip attem
+000116f0: 7074 2e0a 2020 2020 2020 2020 2222 220a  pt..        """.
+00011700: 2020 2020 2020 2020 2320 7a69 700a 2020          # zip.  
+00011710: 2020 2020 2020 7a69 705f 636d 6420 3d20        zip_cmd = 
+00011720: 7365 6c66 2e67 6574 5f7a 6970 5f63 6f6d  self.get_zip_com
+00011730: 6d61 6e64 2864 6174 615f 6c6f 6361 7469  mand(data_locati
+00011740: 6f6e 2c20 6669 6c65 6e61 6d65 290a 2020  on, filename).  
+00011750: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00011760: 6f28 6622 5a69 7070 696e 6720 7b64 6174  o(f"Zipping {dat
+00011770: 615f 6c6f 6361 7469 6f6e 7d20 6173 207b  a_location} as {
+00011780: 6669 6c65 6e61 6d65 7d20 6f6e 2053 6c75  filename} on Slu
+00011790: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
+000117a0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
+000117b0: 6d61 6e64 7328 5b7a 6970 5f63 6d64 5d2c  mands([zip_cmd],
+000117c0: 2065 6e76 3d65 6e76 290a 0a20 2020 2064   env=env)..    d
+000117d0: 6566 2067 6574 5f7a 6970 5f63 6f6d 6d61  ef get_zip_comma
+000117e0: 6e64 2873 656c 662c 2064 6174 615f 6c6f  nd(self, data_lo
+000117f0: 6361 7469 6f6e 3a20 7374 722c 2066 696c  cation: str, fil
+00011800: 656e 616d 653a 2073 7472 2920 2d3e 2073  ename: str) -> s
+00011810: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
+00011820: 2020 2020 2020 2020 4765 6e65 7261 7465          Generate
+00011830: 2061 2063 6f6d 6d61 6e64 2073 7472 696e   a command strin
+00011840: 6720 666f 7220 7a69 7070 696e 6720 7468  g for zipping th
+00011850: 6520 6461 7461 206f 6e20 536c 7572 6d2e  e data on Slurm.
+00011860: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00011870: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00011880: 5f6c 6f63 6174 696f 6e20 2873 7472 293a  _location (str):
+00011890: 2054 6865 2066 6f6c 6465 7220 746f 2062   The folder to b
+000118a0: 6520 7a69 7070 6564 2e0a 2020 2020 2020  e zipped..      
+000118b0: 2020 2020 2020 6669 6c65 6e61 6d65 2028        filename (
+000118c0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+000118d0: 6620 7468 6520 7a69 7020 6172 6368 6976  f the zip archiv
+000118e0: 6520 6669 6c65 2074 6f20 6578 7472 6163  e file to extrac
+000118f0: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+00011900: 2020 2057 6974 686f 7574 2065 7874 656e     Without exten
+00011910: 7369 6f6e 2e0a 0a20 2020 2020 2020 2052  sion...        R
+00011920: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00011930: 2020 2020 7374 723a 2054 6865 2063 6f6d      str: The com
+00011940: 6d61 6e64 2074 6f20 6372 6561 7465 2074  mand to create t
+00011950: 6865 207a 6970 2066 696c 652e 0a20 2020  he zip file..   
+00011960: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011970: 2072 6574 7572 6e20 7365 6c66 2e5f 5a49   return self._ZI
+00011980: 505f 434d 442e 666f 726d 6174 2866 696c  P_CMD.format(fil
+00011990: 656e 616d 653d 6669 6c65 6e61 6d65 2c0a  ename=filename,.
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
+000119d0: 6e3d 6461 7461 5f6c 6f63 6174 696f 6e29  n=data_location)
+000119e0: 0a0a 2020 2020 6465 6620 6765 745f 6c6f  ..    def get_lo
+000119f0: 6766 696c 655f 6672 6f6d 5f73 6c75 726d  gfile_from_slurm
+00011a00: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
+00011a30: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
+00011a60: 705f 7374 6f72 6167 653a 2073 7472 203d  p_storage: str =
+00011a70: 2022 2f74 6d70 2f22 2c0a 2020 2020 2020   "/tmp/",.      
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00011aa0: 3a20 7374 7220 3d20 4e6f 6e65 0a20 2020  : str = None.   
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ac0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
+00011ad0: 2054 7570 6c65 5b73 7472 2c20 7374 722c   Tuple[str, str,
+00011ae0: 2054 7261 6e73 6665 7252 6573 756c 745d   TransferResult]
+00011af0: 3a0a 2020 2020 2020 2020 2222 2243 6f70  :.        """Cop
+00011b00: 7920 7468 6520 6c6f 6766 696c 6520 6f66  y the logfile of
+00011b10: 2074 6865 2067 6976 656e 2053 4c55 524d   the given SLURM
+00011b20: 206a 6f62 2074 6f20 7468 6520 6c6f 6361   job to the loca
+00011b30: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
+00011b40: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
+00011b50: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
+00011b60: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
+00011b70: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
+00011b80: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
+00011b90: 756e 6e65 7273 2e52 6573 756c 740a 2020  unners.Result.  
+00011ba0: 2020 2020 2020 6f72 2066 6162 7269 632e        or fabric.
+00011bb0: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
+00011bc0: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
+00011bd0: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
+00011be0: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
+00011bf0: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
+00011c00: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
+00011c10: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
+00011c20: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
+00011c30: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
+00011c40: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
+00011c50: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
+00011c60: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
+00011c70: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
+00011c80: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
+00011c90: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
+00011ca0: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
+00011cb0: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
+00011cc0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00011cd0: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
+00011ce0: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
+00011cf0: 4944 206f 6620 7468 6520 534c 5552 4d20  ID of the SLURM 
+00011d00: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
+00011d10: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
+00011d20: 6765 2028 7374 722c 206f 7074 696f 6e61  ge (str, optiona
+00011d30: 6c29 3a20 5061 7468 2074 6f20 7374 6f72  l): Path to stor
+00011d40: 6520 7468 6520 6c6f 6766 696c 6520 0a20  e the logfile . 
+00011d50: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011d60: 6f63 616c 6c79 2e20 4465 6661 756c 7473  ocally. Defaults
+00011d70: 2074 6f20 222f 746d 702f 222e 0a20 2020   to "/tmp/"..   
+00011d80: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00011d90: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00011da0: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
+00011db0: 6766 696c 6520 6f6e 2074 6865 2053 4c55  gfile on the SLU
+00011dc0: 524d 2073 6572 7665 722e 0a20 2020 2020  RM server..     
+00011dd0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00011de0: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
+00011df0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00011e00: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+00011e10: 3a20 6469 7265 6374 6f72 792c 2066 756c  : directory, ful
+00011e20: 6c20 7061 7468 206f 6620 7468 6520 6c6f  l path of the lo
+00011e30: 6766 696c 652c 2061 6e64 2054 7261 6e73  gfile, and Trans
+00011e40: 6665 7252 6573 756c 740a 2020 2020 2020  ferResult.      
+00011e50: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00011e60: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
+00011e70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00011e80: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
+00011e90: 4746 494c 450a 2020 2020 2020 2020 6c6f  GFILE.        lo
+00011ea0: 6766 696c 6520 3d20 6c6f 6766 696c 652e  gfile = logfile.
+00011eb0: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
+00011ec0: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
+00011ed0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00011ee0: 2e69 6e66 6f28 6622 436f 7079 696e 6720  .info(f"Copying 
+00011ef0: 6c6f 6766 696c 6520 7b6c 6f67 6669 6c65  logfile {logfile
+00011f00: 7d20 6672 6f6d 2053 6c75 726d 5c0a 2020  } from Slurm\.  
+00011f10: 2020 2020 2020 2020 2020 746f 207b 6c6f            to {lo
+00011f20: 6361 6c5f 746d 705f 7374 6f72 6167 657d  cal_tmp_storage}
+00011f30: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
+00011f40: 7420 3d20 7365 6c66 2e67 6574 280a 2020  t = self.get(.  
+00011f50: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
+00011f60: 3d6c 6f67 6669 6c65 2c0a 2020 2020 2020  =logfile,.      
+00011f70: 2020 2020 2020 6c6f 6361 6c3d 6c6f 6361        local=loca
+00011f80: 6c5f 746d 705f 7374 6f72 6167 6529 0a20  l_tmp_storage). 
+00011f90: 2020 2020 2020 2065 7870 6f72 745f 6669         export_fi
+00011fa0: 6c65 203d 206c 6f63 616c 5f74 6d70 5f73  le = local_tmp_s
+00011fb0: 746f 7261 6765 2b6c 6f67 6669 6c65 0a20  torage+logfile. 
+00011fc0: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+00011fd0: 6361 6c5f 746d 705f 7374 6f72 6167 652c  cal_tmp_storage,
+00011fe0: 2065 7870 6f72 745f 6669 6c65 2c20 7265   export_file, re
+00011ff0: 7375 6c74 0a0a 2020 2020 6465 6620 6765  sult..    def ge
+00012000: 745f 756e 7a69 705f 636f 6d6d 616e 6428  t_unzip_command(
+00012010: 7365 6c66 2c20 7a69 7066 696c 653a 2073  self, zipfile: s
+00012020: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00012030: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00012040: 6c74 6572 5f66 696c 6574 7970 6573 3a20  lter_filetypes: 
+00012050: 7374 7220 3d20 222a 2e7a 6172 7220 2a2e  str = "*.zarr *.
+00012060: 7469 6666 202a 2e74 6966 220a 2020 2020  tiff *.tif".    
+00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012080: 2020 2020 2020 2920 2d3e 2073 7472 3a0a        ) -> str:.
+00012090: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000120a0: 2020 2020 4765 6e65 7261 7465 2061 2063      Generate a c
+000120b0: 6f6d 6d61 6e64 2073 7472 696e 6720 666f  ommand string fo
+000120c0: 7220 756e 7a69 7070 696e 6720 6120 6461  r unzipping a da
+000120d0: 7461 2061 7263 6869 7665 2061 6e64 2063  ta archive and c
+000120e0: 7265 6174 696e 670a 2020 2020 2020 2020  reating.        
+000120f0: 7265 7175 6972 6564 2064 6972 6563 746f  required directo
+00012100: 7269 6573 2066 6f72 2053 6c75 726d 206a  ries for Slurm j
+00012110: 6f62 732e 0a0a 2020 2020 2020 2020 4172  obs...        Ar
+00012120: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00012130: 7a69 7066 696c 6520 2873 7472 293a 2054  zipfile (str): T
+00012140: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
+00012150: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
+00012160: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
+00012170: 2020 2020 2020 2020 2020 2020 5769 7468              With
+00012180: 6f75 7420 6578 7465 6e73 696f 6e2e 0a20  out extension.. 
+00012190: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+000121a0: 725f 6669 6c65 7479 7065 7320 2873 7472  r_filetypes (str
+000121b0: 2c20 6f70 7469 6f6e 616c 293a 2041 2073  , optional): A s
+000121c0: 7061 6365 2d73 6570 6172 6174 6564 2073  pace-separated s
+000121d0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+000121e0: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
+000121f0: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
+00012200: 696f 6e73 2074 6f20 6578 7472 6163 7420  ions to extract 
+00012210: 6672 6f6d 2074 6865 207a 6970 2066 696c  from the zip fil
+00012220: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00012230: 2020 2045 2e67 2e20 6465 6661 756c 7473     E.g. defaults
+00012240: 2074 6f20 222a 2e7a 6172 7220 2a2e 7469   to "*.zarr *.ti
+00012250: 6666 202a 2e74 6966 222e 0a20 2020 2020  ff *.tif"..     
+00012260: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
+00012270: 6e67 2074 6869 7320 6172 6775 6d65 6e74  ng this argument
+00012280: 2074 6f20 604e 6f6e 6560 2077 696c 6c20   to `None` will 
+00012290: 6f6d 6974 2074 6865 2066 696c 650a 2020  omit the file.  
+000122a0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000122b0: 6c74 6572 2061 6e64 2065 7874 7261 6374  lter and extract
+000122c0: 2061 6c6c 2066 696c 6573 2e0a 0a20 2020   all files...   
+000122d0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+000122e0: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00012300: 6865 2063 6f6d 6d61 6e64 2074 6f20 6578  he command to ex
+00012310: 7472 6163 7420 7468 6520 7370 6563 6966  tract the specif
+00012320: 6965 640a 2020 2020 2020 2020 2020 2020  ied.            
+00012330: 2020 2020 6669 6c65 7479 7065 7320 6672      filetypes fr
+00012340: 6f6d 2074 6865 207a 6970 2066 696c 652e  om the zip file.
+00012350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012360: 2020 2020 2075 6e7a 6970 5f63 6d64 203d       unzip_cmd =
+00012370: 2066 226d 6b64 6972 207b 7365 6c66 2e73   f"mkdir {self.s
+00012380: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
+00012390: 7b7a 6970 6669 6c65 7d20 5c0a 2020 2020  {zipfile} \.    
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
+000123c0: 5f70 6174 687d 2f7b 7a69 7066 696c 657d  _path}/{zipfile}
+000123d0: 2f64 6174 6120 5c0a 2020 2020 2020 2020  /data \.        
+000123e0: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
+000123f0: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
+00012400: 687d 2f7b 7a69 7066 696c 657d 2f64 6174  h}/{zipfile}/dat
+00012410: 612f 696e 205c 0a20 2020 2020 2020 2020  a/in \.         
+00012420: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+00012430: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+00012440: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
+00012450: 2f6f 7574 205c 0a20 2020 2020 2020 2020  /out \.         
+00012460: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+00012470: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+00012480: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
+00012490: 2f67 743b 205c 0a20 2020 2020 2020 2020  /gt; \.         
+000124a0: 2020 2020 2020 2020 2020 2037 7a20 7820             7z x 
+000124b0: 2d79 202d 6f7b 7365 6c66 2e73 6c75 726d  -y -o{self.slurm
+000124c0: 5f64 6174 615f 7061 7468 7d2f 7b7a 6970  _data_path}/{zip
+000124d0: 6669 6c65 7d2f 6461 7461 2f69 6e20 5c0a  file}/data/in \.
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124f0: 2020 2020 7b73 656c 662e 736c 7572 6d5f      {self.slurm_
+00012500: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
+00012510: 696c 657d 2e7a 6970 207b 6669 6c74 6572  ile}.zip {filter
+00012520: 5f66 696c 6574 7970 6573 7d22 0a0a 2020  _filetypes}"..  
+00012530: 2020 2020 2020 7265 7475 726e 2075 6e7a        return unz
+00012540: 6970 5f63 6d64 0a0a 2020 2020 6465 6620  ip_cmd..    def 
+00012550: 6765 745f 696d 6167 655f 7665 7273 696f  get_image_versio
+00012560: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
+00012570: 7328 7365 6c66 2c20 6d6f 6465 6c3a 2073  s(self, model: s
+00012580: 7472 0a20 2020 2020 2020 2020 2020 2020  tr.             
+00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125a0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+000125b0: 3e20 5475 706c 655b 4c69 7374 5b73 7472  > Tuple[List[str
+000125c0: 5d2c 204c 6973 745b 7374 725d 5d3a 0a20  ], List[str]]:. 
+000125d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000125e0: 2020 2052 6574 7269 6576 6520 7468 6520     Retrieve the 
+000125f0: 6176 6169 6c61 626c 6520 696d 6167 6520  available image 
+00012600: 7665 7273 696f 6e73 2061 6e64 2069 6e70  versions and inp
+00012610: 7574 2064 6174 6120 6669 6c65 7320 666f  ut data files fo
+00012620: 7220 610a 2020 2020 2020 2020 6769 7665  r a.        give
+00012630: 6e20 6d6f 6465 6c2e 0a0a 2020 2020 2020  n model...      
+00012640: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00012650: 2020 2020 6d6f 6465 6c20 2873 7472 293a      model (str):
+00012660: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00012670: 206d 6f64 656c 2074 6f20 7175 6572 7920   model to query 
+00012680: 666f 722e 0a0a 2020 2020 2020 2020 5265  for...        Re
+00012690: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000126a0: 2020 2054 7570 6c65 5b4c 6973 745b 7374     Tuple[List[st
+000126b0: 725d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  r], List[str]]:.
+000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126d0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+000126e0: 6e67 2074 776f 206c 6973 7473 3a0a 2020  ng two lists:.  
+000126f0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00012700: 5468 6520 6669 7273 7420 6c69 7374 2069  The first list i
+00012710: 6e63 6c75 6465 7320 7468 6520 6176 6169  ncludes the avai
+00012720: 6c61 626c 6520 696d 6167 6520 7665 7273  lable image vers
+00012730: 696f 6e73 2c20 0a20 2020 2020 2020 2020  ions, .         
+00012740: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00012750: 6420 696e 2064 6573 6365 6e64 696e 6720  d in descending 
+00012760: 6f72 6465 722e 0a20 2020 2020 2020 2020  order..         
+00012770: 2020 2020 2020 202d 2054 6865 2073 6563         - The sec
+00012780: 6f6e 6420 6c69 7374 2069 6e63 6c75 6465  ond list include
+00012790: 7320 7468 6520 6176 6169 6c61 626c 6520  s the available 
+000127a0: 6461 7461 2066 696c 6573 2e0a 0a20 2020  data files...   
+000127b0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+000127c0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+000127d0: 726f 723a 2049 6620 7468 6520 7072 6f76  ror: If the prov
+000127e0: 6964 6564 206d 6f64 656c 2069 7320 6e6f  ided model is no
+000127f0: 7420 666f 756e 6420 696e 2074 6865 0a20  t found in the. 
+00012800: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00012810: 6c75 726d 436c 6965 6e74 2773 206b 6e6f  lurmClient's kno
+00012820: 776e 206d 6f64 656c 2070 6174 6873 2e0a  wn model paths..
+00012830: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012840: 2020 2020 696d 6167 655f 7061 7468 203d      image_path =
+00012850: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+00012860: 6c5f 7061 7468 732e 6765 7428 6d6f 6465  l_paths.get(mode
+00012870: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
+00012880: 7420 696d 6167 655f 7061 7468 3a0a 2020  t image_path:.  
+00012890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000128a0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+000128b0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
+000128c0: 2070 6174 6820 6b6e 6f77 6e20 666f 7220   path known for 
+000128d0: 7072 6f76 6964 6564 206d 6f64 656c 207b  provided model {
+000128e0: 6d6f 6465 6c7d 2c20 5c0a 2020 2020 2020  model}, \.      
+000128f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00012900: 207b 7365 6c66 2e73 6c75 726d 5f6d 6f64   {self.slurm_mod
+00012910: 656c 5f70 6174 6873 7d22 290a 2020 2020  el_paths}").    
+00012920: 2020 2020 636d 646c 6973 7420 3d20 5b0a      cmdlist = [.
+00012930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012940: 2e5f 5645 5253 494f 4e5f 434d 442e 666f  ._VERSION_CMD.fo
+00012950: 726d 6174 2873 6c75 726d 5f69 6d61 6765  rmat(slurm_image
+00012960: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
+00012970: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
+00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 2020 2020 696d 6167 655f 7061 7468 3d69      image_path=i
+000129b0: 6d61 6765 5f70 6174 6829 2c0a 2020 2020  mage_path),.    
+000129c0: 2020 2020 2020 2020 7365 6c66 2e5f 4441          self._DA
+000129d0: 5441 5f43 4d44 2e66 6f72 6d61 7428 736c  TA_CMD.format(sl
+000129e0: 7572 6d5f 6461 7461 5f70 6174 683d 7365  urm_data_path=se
+000129f0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
+00012a00: 7468 295d 0a20 2020 2020 2020 2023 2073  th)].        # s
+00012a10: 706c 6974 2072 6573 706f 6e73 6573 2070  plit responses p
+00012a20: 6572 2063 6f6d 6d61 6e64 0a20 2020 2020  er command.     
+00012a30: 2020 2072 6573 706f 6e73 655f 6c69 7374     response_list
+00012a40: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00012a50: 616e 6473 5f73 706c 6974 5f6f 7574 2863  ands_split_out(c
+00012a60: 6d64 6c69 7374 290a 2020 2020 2020 2020  mdlist).        
+00012a70: 2320 7370 6c69 7420 6c69 6e65 7320 6675  # split lines fu
+00012a80: 7274 6865 7220 696e 746f 2073 7562 6c69  rther into subli
+00012a90: 7374 730a 2020 2020 2020 2020 7265 7370  sts.        resp
+00012aa0: 6f6e 7365 5f6c 6973 7420 3d20 5b72 6573  onse_list = [res
+00012ab0: 706f 6e73 652e 7374 7269 7028 292e 7370  ponse.strip().sp
+00012ac0: 6c69 7428 275c 6e27 290a 2020 2020 2020  lit('\n').      
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2066 6f72 2072 6573 706f 6e73 6520     for response 
+00012af0: 696e 2072 6573 706f 6e73 655f 6c69 7374  in response_list
+00012b00: 5d0a 2020 2020 2020 2020 7265 7370 6f6e  ].        respon
+00012b10: 7365 5f6c 6973 745b 305d 203d 2073 6f72  se_list[0] = sor
+00012b20: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
+00012b30: 745b 305d 2c20 7265 7665 7273 653d 5472  t[0], reverse=Tr
+00012b40: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+00012b50: 726e 2072 6573 706f 6e73 655f 6c69 7374  rn response_list
+00012b60: 5b30 5d2c 2072 6573 706f 6e73 655f 6c69  [0], response_li
+00012b70: 7374 5b31 5d0a 0a20 2020 2064 6566 2067  st[1]..    def g
+00012b80: 6574 5f61 6c6c 5f69 6d61 6765 5f76 6572  et_all_image_ver
+00012b90: 7369 6f6e 735f 616e 645f 6461 7461 5f66  sions_and_data_f
+00012ba0: 696c 6573 2873 656c 660a 2020 2020 2020  iles(self.      
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
+00012be0: 6c65 5b44 6963 745b 7374 722c 204c 6973  le[Dict[str, Lis
+00012bf0: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 4c69 7374 5b73 7472 5d5d 3a0a 2020    List[str]]:.  
+00012c40: 2020 2020 2020 2222 2252 6574 7269 6576        """Retriev
+00012c50: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
+00012c60: 696d 6167 6520 7665 7273 696f 6e73 2061  image versions a
+00012c70: 6e64 2064 6174 6120 6669 6c65 7320 6672  nd data files fr
+00012c80: 6f6d 0a20 2020 2020 2020 2074 6865 2053  om.        the S
+00012c90: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
+00012ca0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00012cb0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+00012cc0: 5b44 6963 745b 7374 722c 204c 6973 745b  [Dict[str, List[
+00012cd0: 7374 725d 5d2c 204c 6973 745b 7374 725d  str]], List[str]
+00012ce0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00012cf0: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+00012d00: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+00012d10: 2020 2020 2020 202d 2041 2064 6963 7469         - A dicti
+00012d20: 6f6e 6172 7920 6d61 7070 696e 6720 6d6f  onary mapping mo
+00012d30: 6465 6c73 2074 6f20 6176 6169 6c61 626c  dels to availabl
+00012d40: 6520 7665 7273 696f 6e73 2e0a 2020 2020  e versions..    
+00012d50: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
+00012d60: 6c69 7374 206f 6620 6176 6169 6c61 626c  list of availabl
+00012d70: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
+00012d80: 6465 7273 2e0a 2020 2020 2020 2020 2222  ders..        ""
+00012d90: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
+00012da0: 6469 6374 203d 207b 7d0a 2020 2020 2020  dict = {}.      
+00012db0: 2020 636d 646c 6973 7420 3d20 5b5d 0a0a    cmdlist = []..
+00012dc0: 2020 2020 2020 2020 666f 7220 7061 7468          for path
+00012dd0: 2069 6e20 7365 6c66 2e73 6c75 726d 5f6d   in self.slurm_m
+00012de0: 6f64 656c 5f70 6174 6873 2e76 616c 7565  odel_paths.value
+00012df0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00012e00: 2070 6174 6863 6d64 203d 2073 656c 662e   pathcmd = self.
+00012e10: 5f56 4552 5349 4f4e 5f43 4d44 2e66 6f72  _VERSION_CMD.for
+00012e20: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00012e30: 2020 2020 2073 6c75 726d 5f69 6d61 6765       slurm_image
+00012e40: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
+00012e50: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012e70: 6d61 6765 5f70 6174 683d 7061 7468 290a  mage_path=path).
+00012e80: 2020 2020 2020 2020 2020 2020 636d 646c              cmdl
+00012e90: 6973 742e 6170 7065 6e64 2870 6174 6863  ist.append(pathc
+00012ea0: 6d64 290a 0a20 2020 2020 2020 2023 2041  md)..        # A
+00012eb0: 6464 2064 6174 6120 7061 7468 2074 6f6f  dd data path too
+00012ec0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
+00012ed0: 2e61 7070 656e 6428 7365 6c66 2e5f 4441  .append(self._DA
+00012ee0: 5441 5f43 4d44 2e66 6f72 6d61 7428 0a20  TA_CMD.format(. 
+00012ef0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00012f00: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
+00012f10: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
+00012f20: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
+00012f30: 6974 2072 6573 706f 6e73 6573 2070 6572  it responses per
+00012f40: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
+00012f50: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
+00012f60: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00012f70: 6473 5f73 706c 6974 5f6f 7574 2863 6d64  ds_split_out(cmd
+00012f80: 6c69 7374 290a 0a20 2020 2020 2020 2023  list)..        #
+00012f90: 2053 706c 6974 206c 696e 6573 2066 7572   Split lines fur
+00012fa0: 7468 6572 2069 6e74 6f20 7375 626c 6973  ther into sublis
+00012fb0: 7473 0a20 2020 2020 2020 2072 6573 706f  ts.        respo
+00012fc0: 6e73 655f 6c69 7374 203d 205b 7265 7370  nse_list = [resp
+00012fd0: 6f6e 7365 2e73 7472 6970 2829 2e73 706c  onse.strip().spl
+00012fe0: 6974 2827 5c6e 2729 0a20 2020 2020 2020  it('\n').       
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 666f 7220 7265 7370 6f6e 7365 2069    for response i
+00013010: 6e20 7265 7370 6f6e 7365 5f6c 6973 745d  n response_list]
+00013020: 0a0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
+00013030: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
+00013040: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00013050: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
+00013060: 2020 2020 2023 2052 6574 7572 6e20 6869       # Return hi
+00013070: 6768 6573 7420 7665 7273 696f 6e20 6669  ghest version fi
+00013080: 7273 740a 2020 2020 2020 2020 2020 2020  rst.            
+00013090: 7265 7375 6c74 6469 6374 5b6b 5d20 3d20  resultdict[k] = 
+000130a0: 736f 7274 6564 2872 6573 706f 6e73 655f  sorted(response_
+000130b0: 6c69 7374 5b69 5d2c 2072 6576 6572 7365  list[i], reverse
+000130c0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+000130d0: 7265 7475 726e 2072 6573 756c 7464 6963  return resultdic
+000130e0: 742c 2072 6573 706f 6e73 655f 6c69 7374  t, response_list
+000130f0: 5b2d 315d 0a                             [-1].
```

### Comparing `biomero-1.6.0/biomero.egg-info/PKG-INFO` & `biomero-1.7.0/biomero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -276,25 +276,26 @@
 
 Your Slurm cluster/login node needs to have:
 1. SSH access w/ public key (headless)
 2. SCP access (generally comes with SSH)
 3. 7zip installed
 4. Singularity/Apptainer installed
 5. (Optional) Git installed, if you want your own job scripts
+6. Slurm accounting enabled
 
 ## OMERO Requirements
 
 Your OMERO _processing_ node needs to have:
 1. SSH client and access to the Slurm cluster (w/ private key / headless)
 2. SCP access to the Slurm cluster
 3. Python3.7+
 4. This library installed 
     - Latest release on PyPI `python3 -m pip install biomero`
     - or latest Github version `python3 -m pip install 'git+https://github.com/NL-BioImaging/biomero'`
-5. uration setup at `/etc/slurm-.ini`
+5. Configuration setup at `/etc/slurm-.ini`
 6. Requirements for some scripts: `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` and the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr).
 
 Your OMERO _server_ node needs to have:
 1. Some OMERO example scripts installed to interact with this library:
     - My examples on github: `https://github.com/NL-BioImaging/biomero-scripts`
     - Install those at `/opt/omero/server/OMERO.server/lib/scripts/slurm/`, e.g. `git clone https://github.com/NL-BioImaging/biomero-scripts.git <path>/slurm`
```

### Comparing `biomero-1.6.0/biomero.egg-info/SOURCES.txt` & `biomero-1.7.0/biomero.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 resources/convert_job_array.sh
 resources/convert_zarr_to_tiff.def
 resources/convert_zarr_to_tiff.py
 resources/example.config
 resources/job_template.sh
 resources/pull_images.sh
 resources/slurm-config.ini
+resources/tutorials/tutorial_Azure_slurm.md
 resources/tutorials/tutorial_GoogleCloud_slurm.md
 resources/tutorials/tutorial_cellexpansion.md
 resources/tutorials/tutorial_cellprofiler.md
 resources/tutorials/tutorial_local_slurm.md
 resources/tutorials/images/Cells.tif
 resources/tutorials/images/cellexpansion.png
 resources/tutorials/images/gc_allow_ssh.PNG
```

### Comparing `biomero-1.6.0/docs/Makefile` & `biomero-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/docs/conf.py` & `biomero-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/docs/index.rst` & `biomero-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/docs/make.bat` & `biomero-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/pyproject.toml` & `biomero-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/convert_job_array.sh` & `biomero-1.7.0/resources/convert_job_array.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/convert_zarr_to_tiff.py` & `biomero-1.7.0/resources/convert_zarr_to_tiff.py`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/job_template.sh` & `biomero-1.7.0/resources/job_template.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/slurm-config.ini` & `biomero-1.7.0/resources/slurm-config.ini`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/Cells.tif` & `biomero-1.7.0/resources/tutorials/images/Cells.tif`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/cellexpansion.png` & `biomero-1.7.0/resources/tutorials/images/cellexpansion.png`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/gc_allow_ssh.PNG` & `biomero-1.7.0/resources/tutorials/images/gc_allow_ssh.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/nuclei_labels.png` & `biomero-1.7.0/resources/tutorials/images/nuclei_labels.png`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/webclient_init_env.PNG` & `biomero-1.7.0/resources/tutorials/images/webclient_init_env.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/webclient_init_env_done.PNG` & `biomero-1.7.0/resources/tutorials/images/webclient_init_env_done.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/webclient_run_cellpose.PNG` & `biomero-1.7.0/resources/tutorials/images/webclient_run_cellpose.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/images/webclient_run_workflow.PNG` & `biomero-1.7.0/resources/tutorials/images/webclient_run_workflow.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/tutorial_GoogleCloud_slurm.md` & `biomero-1.7.0/resources/tutorials/tutorial_GoogleCloud_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/tutorial_cellexpansion.md` & `biomero-1.7.0/resources/tutorials/tutorial_cellexpansion.md`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/tutorial_cellprofiler.md` & `biomero-1.7.0/resources/tutorials/tutorial_cellprofiler.md`

 * *Files identical despite different names*

### Comparing `biomero-1.6.0/resources/tutorials/tutorial_local_slurm.md` & `biomero-1.7.0/resources/tutorials/tutorial_local_slurm.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 However, if you don't have ready access (yet) to such a cluster, you might want to spin some test environment up locally and connect your (local) OMERO to it. 
 This is what we will cover in this tutorial.
 
 ## 0. Requirements
 
 To follow this tutorial, you need:
 - Git
-- Docker
+- Docker (Desktop for Windows)
 - OMERO Insight
 - \> 18GB memory
 - \> 8 CPU cores
 
-I use Windows here, but it should work on Linux/Mac too. If not, let me know.
+**Warning**: I tested with Windows here, and I've heard a few issues with (command-line) Linux:
+
+  1. `host.docker.internal` address does not work to communicate via the host machine on (command-line) Linux. 
+  2. If you don't run Docker as root, it won't have access to the mounted SSH keys because of file rights. 
+      - As an example, we run a setup on (rootless) Podman where we add SSH keys as (podman) secrets instead.
+
 
 System requirements could be less, but then you have to change some configurations for Slurm.
 
 I provide ready-to-go TL;DR, but in the details of each chapter I walk through the steps I took to make these containers ready.
 
 ## 1. Setup Docker containers for Slurm
```

### Comparing `biomero-1.6.0/tests/unit/test_slurm_client.py` & `biomero-1.7.0/tests/unit/test_slurm_client.py`

 * *Files identical despite different names*

