# Comparing `tmp/tscode-0.4.8.tar.gz` & `tmp/tscode-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscode-0.4.8.tar", last modified: Fri Feb  2 15:47:15 2024, max compression
+gzip compressed data, was "tscode-0.4.9.tar", last modified: Thu Feb 22 21:26:11 2024, max compression
```

## Comparing `tscode-0.4.8.tar` & `tscode-0.4.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.422058 tscode-0.4.8/
--rw-r--r--   0 root         (0) root         (0)    21216 2024-02-02 15:45:47.000000 tscode-0.4.8/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-10-04 02:19:23.000000 tscode-0.4.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      138 2023-10-04 02:19:23.000000 tscode-0.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22586 2024-02-02 15:47:15.422058 tscode-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2508 2023-11-18 22:24:31.000000 tscode-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.389558 tscode-0.4.8/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     2138 2024-01-28 16:37:38.000000 tscode-0.4.8/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     6432 2024-01-14 16:20:58.000000 tscode-0.4.8/docs/examples.rst
--rw-r--r--   0 root         (0) root         (0)      226 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3356 2023-11-26 16:07:46.000000 tscode-0.4.8/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     4384 2023-11-26 16:07:12.000000 tscode-0.4.8/docs/introduction.rst
--rw-r--r--   0 root         (0) root         (0)    28351 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       64 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/modules.rst
--rw-r--r--   0 root         (0) root         (0)    12928 2024-01-21 22:40:24.000000 tscode-0.4.8/docs/operators_keywords.rst
--rw-r--r--   0 root         (0) root         (0)       46 2023-10-27 18:05:28.000000 tscode-0.4.8/docs/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/setup.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/tscode.calculators.rst
--rw-r--r--   0 root         (0) root         (0)     4609 2023-10-04 02:19:26.000000 tscode-0.4.8/docs/tscode.rst
--rw-r--r--   0 root         (0) root         (0)     7841 2023-10-23 13:11:17.000000 tscode-0.4.8/docs/usage.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-02 15:47:15.422058 tscode-0.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2352 2024-02-02 15:44:50.000000 tscode-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.411225 tscode-0.4.8/tscode/
--rw-r--r--   0 root         (0) root         (0)   191635 2023-11-26 15:34:07.000000 tscode-0.4.8/tscode/TEST_NOTEBOOK.ipynb
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-01 18:35:50.000000 tscode-0.4.8/tscode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4990 2024-02-02 15:45:11.000000 tscode-0.4.8/tscode/__main__.py
--rw-r--r--   0 root         (0) root         (0)    12546 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/algebra.py
--rw-r--r--   0 root         (0) root         (0)    33291 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/ase_manipulations.py
--rw-r--r--   0 root         (0) root         (0)    20727 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/atropisomer_module.py
--rw-r--r--   0 root         (0) root         (0)     3470 2023-10-09 01:36:51.000000 tscode-0.4.8/tscode/automep.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.411225 tscode-0.4.8/tscode/calculators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-01 18:35:50.000000 tscode-0.4.8/tscode/calculators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/calculators/_gaussian.py
--rw-r--r--   0 root         (0) root         (0)     9505 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/calculators/_mopac.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/calculators/_openbabel.py
--rw-r--r--   0 root         (0) root         (0)     3675 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/calculators/_orca.py
--rw-r--r--   0 root         (0) root         (0)    24559 2024-01-21 22:17:15.000000 tscode-0.4.8/tscode/calculators/_xtb.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-10-29 20:43:07.000000 tscode-0.4.8/tscode/concurrent_test.py
--rw-r--r--   0 root         (0) root         (0)   110572 2024-01-28 17:22:03.000000 tscode-0.4.8/tscode/embedder.py
--rw-r--r--   0 root         (0) root         (0)    22825 2024-01-21 20:35:16.000000 tscode-0.4.8/tscode/embedder_options.py
--rw-r--r--   0 root         (0) root         (0)    44325 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/embeds.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/errors.py
--rw-r--r--   0 root         (0) root         (0)    10299 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/graph_manipulations.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-10-27 15:37:53.000000 tscode-0.4.8/tscode/hypermolecule_class.py
--rw-r--r--   0 root         (0) root         (0)     7064 2023-11-26 18:34:47.000000 tscode-0.4.8/tscode/mep_relaxer.py
--rw-r--r--   0 root         (0) root         (0)     7349 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/modify_settings.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-10-23 14:44:00.000000 tscode-0.4.8/tscode/mprof.py
--rw-r--r--   0 root         (0) root         (0)     5525 2023-11-15 20:35:23.000000 tscode-0.4.8/tscode/multiembed.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/nci.py
--rw-r--r--   0 root         (0) root         (0)    29290 2024-01-28 17:22:38.000000 tscode-0.4.8/tscode/operators.py
--rw-r--r--   0 root         (0) root         (0)    26016 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/optimization_methods.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/parameters.py
--rw-r--r--   0 root         (0) root         (0)    10939 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/pka.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-10-07 22:49:38.000000 tscode-0.4.8/tscode/profiler.py
--rw-r--r--   0 root         (0) root         (0)      721 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/pt.py
--rw-r--r--   0 root         (0) root         (0)     9244 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/python_functions.py
--rw-r--r--   0 root         (0) root         (0)   221347 2023-10-01 18:35:50.000000 tscode-0.4.8/tscode/quotes.json
--rw-r--r--   0 root         (0) root         (0)   201639 2023-10-01 18:35:50.000000 tscode-0.4.8/tscode/quotes.py
--rw-r--r--   0 root         (0) root         (0)    26255 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/reactive_atoms_classes.py
--rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 16:43:52.000000 tscode-0.4.8/tscode/references.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-11-26 15:34:02.000000 tscode-0.4.8/tscode/rmsd_pruning.py
--rw-r--r--   0 root         (0) root         (0)     2053 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/settings.py
--rw-r--r--   0 root         (0) root         (0)     3066 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/solvents.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.422058 tscode-0.4.8/tscode/tests/
--rw-r--r--   0 root         (0) root         (0)      419 2023-10-04 02:27:28.000000 tscode-0.4.8/tscode/tests/C2F2H4.xyz
--rw-r--r--   0 root         (0) root         (0)      302 2023-10-04 02:27:29.000000 tscode-0.4.8/tscode/tests/C2H4.xyz
--rw-r--r--   0 root         (0) root         (0)      253 2023-10-04 02:27:30.000000 tscode-0.4.8/tscode/tests/CH3Cl.xyz
--rw-r--r--   0 root         (0) root         (0)      253 2023-10-04 02:27:37.000000 tscode-0.4.8/tscode/tests/HCOOH.xyz
--rw-r--r--   0 root         (0) root         (0)      331 2023-10-04 02:27:38.000000 tscode-0.4.8/tscode/tests/HCOOOH.xyz
--rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 13:31:26.000000 tscode-0.4.8/tscode/tests/chelotropic.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 15:39:01.000000 tscode-0.4.8/tscode/tests/cyclical.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-10-22 13:38:12.000000 tscode-0.4.8/tscode/tests/dihedral.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 13:29:37.000000 tscode-0.4.8/tscode/tests/string.txt
--rw-r--r--   0 root         (0) root         (0)      222 2023-10-23 15:39:15.000000 tscode-0.4.8/tscode/tests/trimolecular.txt
--rw-r--r--   0 root         (0) root         (0)     5280 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/tests.py
--rw-r--r--   0 root         (0) root         (0)    45848 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/torsion_module.py
--rw-r--r--   0 root         (0) root         (0)    14998 2024-01-11 16:35:05.000000 tscode-0.4.8/tscode/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 15:47:15.422058 tscode-0.4.8/tscode.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22586 2024-02-02 15:47:15.000000 tscode-0.4.8/tscode.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1683 2024-02-02 15:47:15.000000 tscode-0.4.8/tscode.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 15:47:15.000000 tscode-0.4.8/tscode.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      268 2024-02-02 15:47:15.000000 tscode-0.4.8/tscode.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-02 15:47:15.000000 tscode-0.4.8/tscode.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.827358 tscode-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)    22013 2024-02-22 21:21:56.000000 tscode-0.4.9/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-10-04 02:19:23.000000 tscode-0.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      138 2023-10-04 02:19:23.000000 tscode-0.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23383 2024-02-22 21:26:11.827358 tscode-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-11-18 22:24:31.000000 tscode-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.784024 tscode-0.4.9/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-01-28 16:37:38.000000 tscode-0.4.9/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2024-01-14 16:20:58.000000 tscode-0.4.9/docs/examples.rst
+-rw-r--r--   0 root         (0) root         (0)      226 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-11-26 16:07:46.000000 tscode-0.4.9/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-11-26 16:07:12.000000 tscode-0.4.9/docs/introduction.rst
+-rw-r--r--   0 root         (0) root         (0)    28351 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       64 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/modules.rst
+-rw-r--r--   0 root         (0) root         (0)    12928 2024-01-21 22:40:24.000000 tscode-0.4.9/docs/operators_keywords.rst
+-rw-r--r--   0 root         (0) root         (0)       46 2023-10-27 18:05:28.000000 tscode-0.4.9/docs/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/setup.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/tscode.calculators.rst
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-10-04 02:19:26.000000 tscode-0.4.9/docs/tscode.rst
+-rw-r--r--   0 root         (0) root         (0)     7841 2023-10-23 13:11:17.000000 tscode-0.4.9/docs/usage.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 21:26:11.827358 tscode-0.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-02-02 15:44:50.000000 tscode-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.816524 tscode-0.4.9/tscode/
+-rw-r--r--   0 root         (0) root         (0)   191635 2023-11-26 15:34:07.000000 tscode-0.4.9/tscode/TEST_NOTEBOOK.ipynb
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-01 18:35:50.000000 tscode-0.4.9/tscode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4990 2024-02-22 21:22:10.000000 tscode-0.4.9/tscode/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/algebra.py
+-rw-r--r--   0 root         (0) root         (0)    33291 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/ase_manipulations.py
+-rw-r--r--   0 root         (0) root         (0)    20727 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/atropisomer_module.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-10-09 01:36:51.000000 tscode-0.4.9/tscode/automep.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.816524 tscode-0.4.9/tscode/calculators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-01 18:35:50.000000 tscode-0.4.9/tscode/calculators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/calculators/_gaussian.py
+-rw-r--r--   0 root         (0) root         (0)     9505 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/calculators/_mopac.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/calculators/_openbabel.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/calculators/_orca.py
+-rw-r--r--   0 root         (0) root         (0)    24829 2024-02-22 18:11:54.000000 tscode-0.4.9/tscode/calculators/_xtb.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-10-29 20:43:07.000000 tscode-0.4.9/tscode/concurrent_test.py
+-rw-r--r--   0 root         (0) root         (0)   110575 2024-02-22 21:10:55.000000 tscode-0.4.9/tscode/embedder.py
+-rw-r--r--   0 root         (0) root         (0)    22825 2024-01-21 20:35:16.000000 tscode-0.4.9/tscode/embedder_options.py
+-rw-r--r--   0 root         (0) root         (0)    44325 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/embeds.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/errors.py
+-rw-r--r--   0 root         (0) root         (0)    10299 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/graph_manipulations.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-10-27 15:37:53.000000 tscode-0.4.9/tscode/hypermolecule_class.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-02-18 20:47:02.000000 tscode-0.4.9/tscode/mep_relaxer.py
+-rw-r--r--   0 root         (0) root         (0)     7349 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/modify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-10-23 14:44:00.000000 tscode-0.4.9/tscode/mprof.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2024-02-22 21:10:55.000000 tscode-0.4.9/tscode/multiembed.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/nci.py
+-rw-r--r--   0 root         (0) root         (0)    30871 2024-02-22 18:06:39.000000 tscode-0.4.9/tscode/operators.py
+-rw-r--r--   0 root         (0) root         (0)    26016 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/optimization_methods.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/parameters.py
+-rw-r--r--   0 root         (0) root         (0)    10939 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/pka.py
+-rw-r--r--   0 root         (0) root         (0)      548 2024-02-22 21:10:55.000000 tscode-0.4.9/tscode/profiler.py
+-rw-r--r--   0 root         (0) root         (0)      834 2024-02-22 21:16:19.000000 tscode-0.4.9/tscode/pt.py
+-rw-r--r--   0 root         (0) root         (0)     9244 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/python_functions.py
+-rw-r--r--   0 root         (0) root         (0)   221347 2023-10-01 18:35:50.000000 tscode-0.4.9/tscode/quotes.json
+-rw-r--r--   0 root         (0) root         (0)   201639 2023-10-01 18:35:50.000000 tscode-0.4.9/tscode/quotes.py
+-rw-r--r--   0 root         (0) root         (0)    26255 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/reactive_atoms_classes.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 16:43:52.000000 tscode-0.4.9/tscode/references.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-11-26 15:34:02.000000 tscode-0.4.9/tscode/rmsd_pruning.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/solvents.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.827358 tscode-0.4.9/tscode/tests/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-10-04 02:27:28.000000 tscode-0.4.9/tscode/tests/C2F2H4.xyz
+-rw-r--r--   0 root         (0) root         (0)      302 2023-10-04 02:27:29.000000 tscode-0.4.9/tscode/tests/C2H4.xyz
+-rw-r--r--   0 root         (0) root         (0)      253 2023-10-04 02:27:30.000000 tscode-0.4.9/tscode/tests/CH3Cl.xyz
+-rw-r--r--   0 root         (0) root         (0)      253 2023-10-04 02:27:37.000000 tscode-0.4.9/tscode/tests/HCOOH.xyz
+-rw-r--r--   0 root         (0) root         (0)      331 2023-10-04 02:27:38.000000 tscode-0.4.9/tscode/tests/HCOOOH.xyz
+-rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 13:31:26.000000 tscode-0.4.9/tscode/tests/chelotropic.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 15:39:01.000000 tscode-0.4.9/tscode/tests/cyclical.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-10-22 13:38:12.000000 tscode-0.4.9/tscode/tests/dihedral.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-10-23 13:29:37.000000 tscode-0.4.9/tscode/tests/string.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2023-10-23 15:39:15.000000 tscode-0.4.9/tscode/tests/trimolecular.txt
+-rw-r--r--   0 root         (0) root         (0)     5280 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/tests.py
+-rw-r--r--   0 root         (0) root         (0)    45848 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/torsion_module.py
+-rw-r--r--   0 root         (0) root         (0)    14998 2024-01-11 16:35:05.000000 tscode-0.4.9/tscode/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 21:26:11.827358 tscode-0.4.9/tscode.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23383 2024-02-22 21:26:11.000000 tscode-0.4.9/tscode.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-02-22 21:26:11.000000 tscode-0.4.9/tscode.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 21:26:11.000000 tscode-0.4.9/tscode.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      268 2024-02-22 21:26:11.000000 tscode-0.4.9/tscode.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-02-22 21:26:11.000000 tscode-0.4.9/tscode.egg-info/top_level.txt
```

### Comparing `tscode-0.4.8/CHANGELOG.md` & `tscode-0.4.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ## TSCoDe Changelog
 
 <!-- - Introduced compatibility of SADDLE and NEB keywords for scan> runs with both 2 indices (distance scans) and 4 indices (distance scans) -->
 
 <!-- - ... mep_relax> BETA
 - ... IMAGES kw, also implement it for neb>-->
 
+## 0.4.9 (February 22, 2024)
+- CREST constraints (mtd_search>) are now passed as distance constraints instead of atom fixing (forgot to implement it this way before?).
+- CREST metadynamics input/output files are all retained now and not deleted after execution.
+- Output names changed from starting with "TSCoDe" to "tscode" for easier typing.
+- Modified variable definition of periodic table in tscode.pt to avoid ValueError(s).
+- Added the mep_relax> operator (beta, not present in documentation) to relax chains of images along the PES. Useful to get good starting points for higher-level NEB calculations. First, the optimization is performed by retaining all bond distances, which are then relaxed after the first cycle is converged (developed to find atropisomer interconversion pathways).
+
 ## 0.4.8 (February 2, 2024)
 - Updated library dependency versions.
 
 ## 0.4.7 (Januray 28, 2024)
 - Restyled copy of input in the log file.
 - Added citations to the main program and external modules if they are used (references.py, embedder.py/_print_references).
 - In runs with operators, t_start_run is set before running the first operator, and it is not overwritten by RunEmbedding if it was already set. This makes sure that the final time always includes the time spent executing the operators.
```

### Comparing `tscode-0.4.8/LICENSE` & `tscode-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/PKG-INFO` & `tscode-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscode
-Version: 0.4.8
+Version: 0.4.9
 Summary: Computational chemistry general purpose transition state builder and ensemble optimizer
 Home-page: https://www.github.com/ntampellini/tscode
 Author: Nicolò Tampellini
 Author-email: nicolo.tampellini@yale.edu
 Keywords: computational chemistry,ASE,transition state,xtb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -36,14 +36,21 @@
 ## TSCoDe Changelog
 
 <!-- - Introduced compatibility of SADDLE and NEB keywords for scan> runs with both 2 indices (distance scans) and 4 indices (distance scans) -->
 
 <!-- - ... mep_relax> BETA
 - ... IMAGES kw, also implement it for neb>-->
 
+## 0.4.9 (February 22, 2024)
+- CREST constraints (mtd_search>) are now passed as distance constraints instead of atom fixing (forgot to implement it this way before?).
+- CREST metadynamics input/output files are all retained now and not deleted after execution.
+- Output names changed from starting with "TSCoDe" to "tscode" for easier typing.
+- Modified variable definition of periodic table in tscode.pt to avoid ValueError(s).
+- Added the mep_relax> operator (beta, not present in documentation) to relax chains of images along the PES. Useful to get good starting points for higher-level NEB calculations. First, the optimization is performed by retaining all bond distances, which are then relaxed after the first cycle is converged (developed to find atropisomer interconversion pathways).
+
 ## 0.4.8 (February 2, 2024)
 - Updated library dependency versions.
 
 ## 0.4.7 (Januray 28, 2024)
 - Restyled copy of input in the log file.
 - Added citations to the main program and external modules if they are used (references.py, embedder.py/_print_references).
 - In runs with operators, t_start_run is set before running the first operator, and it is not overwritten by RunEmbedding if it was already set. This makes sure that the final time always includes the time spent executing the operators.
```

### Comparing `tscode-0.4.8/README.md` & `tscode-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/Makefile` & `tscode-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/conf.py` & `tscode-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/examples.rst` & `tscode-0.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/installation.rst` & `tscode-0.4.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/introduction.rst` & `tscode-0.4.9/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/license.rst` & `tscode-0.4.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/make.bat` & `tscode-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/operators_keywords.rst` & `tscode-0.4.9/docs/operators_keywords.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/tscode.rst` & `tscode-0.4.9/docs/tscode.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/docs/usage.rst` & `tscode-0.4.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/setup.py` & `tscode-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/TEST_NOTEBOOK.ipynb` & `tscode-0.4.9/tscode/TEST_NOTEBOOK.ipynb`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/__main__.py` & `tscode-0.4.9/tscode/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Nicolo' Tampellini - nicolo.tampellini@yale.edu
 
 '''
 import argparse
 import os
 import sys
 
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 
 if __name__ == '__main__':
 
 
     usage = '''python -m tscode [-h] [-s] [-t] inputfile [-n NAME]
         
         positional arguments:
```

### Comparing `tscode-0.4.8/tscode/algebra.py` & `tscode-0.4.9/tscode/algebra.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/ase_manipulations.py` & `tscode-0.4.9/tscode/ase_manipulations.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/atropisomer_module.py` & `tscode-0.4.9/tscode/atropisomer_module.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/automep.py` & `tscode-0.4.9/tscode/automep.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/calculators/_gaussian.py` & `tscode-0.4.9/tscode/calculators/_gaussian.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/calculators/_mopac.py` & `tscode-0.4.9/tscode/calculators/_mopac.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/calculators/_openbabel.py` & `tscode-0.4.9/tscode/calculators/_openbabel.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/calculators/_orca.py` & `tscode-0.4.9/tscode/calculators/_orca.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/calculators/_xtb.py` & `tscode-0.4.9/tscode/calculators/_xtb.py`

 * *Files 1% similar despite different names*

```diff
@@ -640,17 +640,19 @@
 
     procs: number of cores to be used for the calculation.
 
     threads: number of parallel threads to be used by the process. 
 
     '''
 
+    # Remove title directory, if already present
     if title in os.listdir():
         shutil.rmtree(os.path.join(os.getcwd(), title))
         
+    # make title directory and cd into it
     os.mkdir(title)
     os.chdir(os.path.join(os.getcwd(), title))
 
     if constrained_indices is not None:
         if len(constrained_indices) == 0:
             constrained_indices = None
 
@@ -660,18 +662,22 @@
 
     with open(f'{title}.xyz', 'w') as f:
         write_xyz(coords, atomnos, f, title=title)
 
     s = f'$opt\n   '
          
     if constrained_indices is not None:  
-        s += '\n$constrain\n   atoms: '
-        for i in np.unique(np.array(constrained_indices).flatten()):
-            s += f"{i+1},"
-        s = s[:-1] + "\n"
+        s += '\n$constrain\n'
+        # s += '   atoms: '
+        # for i in np.unique(np.array(constrained_indices).flatten()):
+        #     s += f"{i+1},"
+
+        for (c1, c2), cd in zip(constrained_indices, constrained_distances):
+            cd = "auto" if cd is None else cd
+            s += f"    distance: {c1+1}, {c2+1}, {cd}\n"
 
     if constrained_dihedrals is not None:
         assert len(constrained_dihedrals) == len(constrained_dih_angles)
         s += '\n$constrain\n' if constrained_indices is None else ''
         for (a, b, c, d), angle in zip(constrained_dihedrals, constrained_dih_angles):
             s += f"   dihedral: {a+1}, {b+1}, {c+1}, {d+1}, {angle}\n"  
  
@@ -761,15 +767,15 @@
     # if CREST crashes, cd into the parent folder before propagating the error
     except CalledProcessError:
         os.chdir(os.path.dirname(os.getcwd()))
         raise CalledProcessError
 
     new_coords = read_xyz('crest_conformers.xyz').atomcoords
 
-    clean_directory((f'{title}.inp', f'{title}.xyz', f"{title}.out"))     
+    # clean_directory((f'{title}.inp', f'{title}.xyz', f"{title}.out"))     
 
     for filename in ('gfnff_topo',
                         'charges',
                         'wbo',
                         'xtbrestart',
                         'xtbtopo.mol', 
                         '.xtboptok',
```

### Comparing `tscode-0.4.8/tscode/concurrent_test.py` & `tscode-0.4.9/tscode/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/embedder.py` & `tscode-0.4.9/tscode/embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,20 +87,20 @@
             self.stamp = stamp
 
         self.avail_cpus = len(os.sched_getaffinity(0))
         self.threads = int(threads) if threads is not None else THREADS or self.avail_cpus//4 or 1
         self.procs = int(procs) if procs is not None else PROCS or 4
 
         try:
-            os.remove(f'TSCoDe_{self.stamp}.log')
+            os.remove(f'tscode_{self.stamp}.log')
 
         except FileNotFoundError:
             pass
 
-        log_filename = f'TSCoDe_{self.stamp}.log'
+        log_filename = f'tscode_{self.stamp}.log'
         self.logfile = open(log_filename, 'a', buffering=1, encoding="utf-8")
         logging.basicConfig(filename=log_filename, filemode='a')
 
         try:
 
             self.write_banner_and_info()
             # Write banner to log file
@@ -244,16 +244,16 @@
             lines = f.readlines()
 
         # write a formatted copy of the input file to the log
         self.log(f'--> Input file: {filename}\n')
         longest = max(len(line.rstrip('\n')) for line in lines)
         self.log('   '+'-'*(longest+3))
         for l, line in enumerate(lines):
-            self.log(f'{l+1}> | '+line.rstrip('\n').ljust(longest)+'|')
-        self.log('   '+'-'*(longest+3)+'\n')
+            self.log(f'{l+1}> | '+line.rstrip('\n').ljust(longest)+'   |')
+        self.log('   '+'-'*(longest+6)+'\n')
 
         # start parsing: get rid of comment and blank lines
         lines = [line.replace(', ',',') for line in lines if line[0] not in ('#', '\n')]
         
         def _remove_internal_constraints(string):
             numbers = [int(re.sub('[^0-9]', '', i)) for i in string]
             letters = [re.sub('[^A-Za-z]', '', i) for i in string]
@@ -866,16 +866,16 @@
         self._set_reactive_atoms_cumnums()
 
         # resetting the attribute
         self.embed = None
 
     def _extract_filename(self, input_string):
         '''
-        Input: 'refine> TSCoDe_unoptimized_comp_check.xyz 5a 36a 0b 43b 33c 60c'
-        Output: 'TSCoDe_unoptimized_comp_check.xyz'
+        Input: 'refine> tscode_unoptimized_comp_check.xyz 5a 36a 0b 43b 33c 60c'
+        Output: 'tscode_unoptimized_comp_check.xyz'
         '''
         input_string = input_string.split('>')[-1].lstrip()
         # remove operator and whitespaces after it
 
         input_string = input_string.split()[0]
         # remove pairing numbers/letters and newline chars
 
@@ -887,15 +887,15 @@
 
         self.log('--> Structures check requested. Shutting down after last window is closed.\n')
 
         for mol in self.objects:
             ase_view(mol)
         
         self.logfile.close()
-        os.remove(f'TSCoDe_{self.stamp}.log')
+        os.remove(f'tscode_{self.stamp}.log')
 
         sys.exit()
 
     def scramble(self, array, sequence):
         return np.array([array[s] for s in sequence])
 
     def get_pairing_dist_from_letter(self, letter):
@@ -984,15 +984,15 @@
         # truncate if there are too many (embed debug first dump)
         if len(self.structures) > 10000 and not self.options.let:
             self.log(f'Truncated {tag} output structures to 10000 (from {len(self.structures)} - keyword LET to override).')
             output_structures = self.structures[0:10000]
         else:
             output_structures = self.structures
 
-        self.outname = f'TSCoDe_{tag}_{self.stamp}.xyz'
+        self.outname = f'tscode_{tag}_{self.stamp}.xyz'
         with open(self.outname, 'w') as f:        
 
             for i, structure in enumerate(align_functions[align](output_structures, atomnos=self.atomnos, indices=indices)):
                 title = f'Strucure {i+1} - {tag}'
 
                 if energies:
                     title += f' - Rel. E. = {round(rel_e[i], 3)} kcal/mol '
@@ -1360,15 +1360,15 @@
         only_fixed_constraints: only uses fixed (UPPERCASE) constraints in optimization
         prevent_scrambling: preserves molecular identities constraining bonds present in graphs (XTB only)
         '''
 
         ################################################# CHECKPOINT BEFORE FF OPTIMIZATION
 
         if not only_fixed_constraints:
-            self.outname = f'TSCoDe_checkpoint_{self.stamp}.xyz'
+            self.outname = f'tscode_checkpoint_{self.stamp}.xyz'
             with open(self.outname, 'w') as f:        
                 for i, structure in enumerate(align_structures(self.structures)):
                     write_xyz(structure, self.atomnos, f, title=f'TS candidate {i+1} - Checkpoint before FF optimization')
             self.log(f'\n--> Checkpoint output - Wrote {len(self.structures)} unoptimized structures to {self.outname} file before FF optimization.\n')
 
         ################################################# GEOMETRY OPTIMIZATION - FORCE FIELD
 
@@ -1525,15 +1525,15 @@
         
         s = f'--> Checkpoint output - Updated {len(self.structures)} optimized structures to {self.outname} file'
 
         if self.options.optimization and (self.options.ff_level != self.options.theory_level) and conv_thr != "tight":
             s += f' before {self.options.calculator} optimization.'
 
         else:
-            self.outname = f'TSCoDe_{"ensemble" if self.embed == "refine" else "poses"}_{self.stamp}.xyz'
+            self.outname = f'tscode_{"ensemble" if self.embed == "refine" else "poses"}_{self.stamp}.xyz'
             # if the FF optimization was the last one, call the outfile accordingly
 
 
         self.log(s+'\n')
 
         with open(self.outname, 'w') as f:        
             for i, (structure, status, energy) in enumerate(zip(align_structures(self.structures),
@@ -1597,15 +1597,15 @@
         discarding similar ones and scrambled ones.
         maxiter - int, number of max iterations for the optimization
         conv_thr: convergence threshold, passed to calculator
         only_fixed_constraints: only uses fixed (UPPERCASE) constraints in optimization
 
         '''
 
-        self.outname = f'TSCoDe_{"ensemble" if self.embed == "refine" else "poses"}_{self.stamp}.xyz'
+        self.outname = f'tscode_{"ensemble" if self.embed == "refine" else "poses"}_{self.stamp}.xyz'
 
 
         task = 'Relaxing interactions' if only_fixed_constraints else 'Structure optimization'
         self.log(f'--> {task} ({self.options.theory_level}{f"/{self.options.solvent}" if self.options.solvent is not None else ""} level via {self.options.calculator}, {self.threads} thread{"s" if self.threads>1 else ""})')
 
         self.energies.fill(0)
         # Resetting all energies since we changed theory level
@@ -1983,15 +1983,15 @@
 
             _, sequence = zip(*sorted(zip(self.energies, range(len(self.energies))), key=lambda x: x[0]))
             self.energies = scramble(self.energies, sequence)
             self.structures = scramble(self.structures, sequence)
             self.constrained_indices = scramble(self.constrained_indices, sequence)
             # sorting structures based on energy
 
-            self.outname = f'TSCoDe_SADDLE_TSs_{self.stamp}.xyz'
+            self.outname = f'tscode_SADDLE_TSs_{self.stamp}.xyz'
             with open(self.outname, 'w') as f:        
                 for structure, energy in zip(align_structures(self.structures), self.rel_energies()):
                     write_xyz(structure, self.atomnos, f, title=f'Structure {i+1} - TS - Rel. E. = {round(energy, 3)} kcal/mol')
 
             self.log(f'Wrote {len(self.structures)} saddle-optimized structures to {self.outname} file\n')
 
         else:
```

### Comparing `tscode-0.4.8/tscode/embedder_options.py` & `tscode-0.4.9/tscode/embedder_options.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/embeds.py` & `tscode-0.4.9/tscode/embeds.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/errors.py` & `tscode-0.4.9/tscode/errors.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/graph_manipulations.py` & `tscode-0.4.9/tscode/graph_manipulations.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/hypermolecule_class.py` & `tscode-0.4.9/tscode/hypermolecule_class.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/mep_relaxer.py` & `tscode-0.4.9/tscode/mep_relaxer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 from ase import Atoms
 from ase.calculators.calculator import (CalculationFailed,
                                         PropertyNotImplementedError)
 from ase.dyneb import DyNEB
 from ase.optimize import LBFGS
 
-from tscode.ase_manipulations import ase_dump, get_ase_calc
+from tscode.ase_manipulations import ase_dump, get_ase_calc, PreventScramblingConstraint
 from tscode.hypermolecule_class import align_structures
 from tscode.utils import time_to_string
 
 
 def ase_mep_relax(
         embedder,
         structures,
@@ -21,14 +21,15 @@
         n_images=None,
         maxiter=200,
         title='temp',
         optimizer=LBFGS,
         logfunction=None,
         write_plot=False,
         verbose_print=False,
+        safe=False,
     ):
     '''
     embedder: tscode embedder object
     structures: array of coordinates to be used as starting points
     atomnos: 1-d array of atomic numbers
     n_images: total number of optimized images connecting reag/prods
     maxiter: maximum number of ensemble optimization steps
@@ -75,14 +76,19 @@
                 allow_shared_calculator=True,
                 )
   
     # Set calculators for all images
     for _, image in enumerate(images):
         image.calc = get_ase_calc(embedder)
 
+        if safe:
+            bond_constr = PreventScramblingConstraint(embedder.objects[0].graph, image)
+            image.set_constraint([bond_constr])
+
+
     t_start = time.perf_counter()
 
     # Set the optimizer and optimize
     try:
         
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
@@ -138,15 +144,15 @@
 
         plt.legend()
         plt.title(title)
         plt.xlabel(f'Image number')
         plt.ylabel('Rel. E. (kcal/mol)')
         plt.savefig(f'{title.replace(" ", "_")}_plt.svg')
 
-    mep = [image.get_positions() for image in images]
+    mep = np.array([image.get_positions() for image in images])
 
     return mep, energies, exit_status
 
 def interpolate_structures(structures, atomnos, n, method='idpp'):
     '''
     Return n interpolated structures from the
     first to the last present in structures
```

### Comparing `tscode-0.4.8/tscode/modify_settings.py` & `tscode-0.4.9/tscode/modify_settings.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/mprof.py` & `tscode-0.4.9/tscode/mprof.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/multiembed.py` & `tscode-0.4.9/tscode/multiembed.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                         i,
                         options,
                     ):
 
     from tscode.embedder import Embedder, RunEmbedding
 
     start_dir = os.getcwd()
-    foldername = f'TSCoDe_embed{i+1}'
+    foldername = f'tscode_embed{i+1}'
     (ix_1, ix_2), (iy_1, iy_2) = constrained_indices
 
     # create a dedicated folder
     if not os.path.isdir(os.path.join(os.getcwd(), foldername)):
         os.mkdir(foldername)
 
     # copy structure files into it
```

### Comparing `tscode-0.4.8/tscode/nci.py` & `tscode-0.4.9/tscode/nci.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/operators.py` & `tscode-0.4.9/tscode/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,53 @@
         pka_routine(filename, embedder)
         outname = filename
 
     elif 'mep_relax>' in input_string:
 
         data = read_xyz(filename)
 
-        ase_mep_relax(
-            embedder,
-            data.atomcoords,
-            data.atomnos,
-            title=embedder.stamp,
-            n_images=embedder.options.images if hasattr(embedder.options, 'images') else None,
-            logfunction=embedder.log,
-            write_plot=True,
-            verbose_print=True,
-            )
+        # can implement a smart safety feature that is
+        # disabled when some bonds have to be let free to break
+        no_bonds_breaking = True
+
+        if no_bonds_breaking:
+
+            mep, _, exit_status = ase_mep_relax(
+                                                embedder,
+                                                data.atomcoords,
+                                                data.atomnos,
+                                                title=embedder.stamp+"_safe",
+                                                n_images=embedder.options.images if hasattr(embedder.options, 'images') else None,
+                                                logfunction=embedder.log,
+                                                write_plot=True,
+                                                verbose_print=True,
+                                                safe=True
+                                                )
+            
+        else:
+            mep = data.atomcoords
+            exit_status = True
+        
+        if exit_status:
+
+            if no_bonds_breaking:
+                print("--> Completed safe optimization, relaxing bond distance constraints.")
+
+            ase_mep_relax(
+                embedder,
+                mep,
+                data.atomnos,
+                title=embedder.stamp,
+                n_images=embedder.options.images if hasattr(embedder.options, 'images') else None,
+                logfunction=embedder.log,
+                write_plot=True,
+                verbose_print=True,
+                safe=True
+                )
+        
         embedder.normal_termination()
 
     else:
         op = input_string.split('>')[0]
         raise Exception(f'Operator {op} not recognized.')
 
     return outname
@@ -433,20 +462,22 @@
                       'an individual search from each conformer (might be time-consuming).')
 
     t_start = time.perf_counter()
     conformers = []
     for i, coords in enumerate(mol.atomcoords):
 
         t_start_conf = time.perf_counter()
-
+        constrained_indices = _get_internal_constraints(filename, embedder)
+        constrained_distances = [embedder.get_pairing_dists_from_constrained_indices(cp) for cp in constrained_indices]
         try:
             conf_batch = crest_mtd_search(
                                             coords,
                                             mol.atomnos,
-                                            constrained_indices=_get_internal_constraints(filename, embedder),
+                                            constrained_indices=constrained_indices,
+                                            constrained_distances=constrained_distances,
                                             solvent=embedder.options.solvent,
                                             charge=mol.charge,
                                             kcal=embedder.options.kcal_thresh,
                                             ncimode=embedder.options.crestnci,
                                             title=mol.rootname+"_mtd_csearch",
                                             procs=2,
                                             threads=max_workers,
@@ -454,15 +485,16 @@
             
         # if the run errors out, we retry with XTB2
         except CalledProcessError:
             logfunction(f'--> Metadynamics run failed with GFN2-XTB//GFN-FF, retrying with just GFN2-XTB (slower but more stable)')
             conf_batch = crest_mtd_search(
                                             coords,
                                             mol.atomnos,
-                                            constrained_indices=_get_internal_constraints(filename, embedder),
+                                            constrained_indices=constrained_indices,
+                                            constrained_distances=constrained_distances,
                                             solvent=embedder.options.solvent,
                                             charge=mol.charge,
                                             method='GFN2-XTB', # try with XTB2
                                             kcal=embedder.options.kcal_thresh,
                                             ncimode=embedder.options.crestnci,
                                             title=mol.rootname+"_mtd_csearch",
                                             procs=2,
```

### Comparing `tscode-0.4.8/tscode/optimization_methods.py` & `tscode-0.4.9/tscode/optimization_methods.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/parameters.py` & `tscode-0.4.9/tscode/parameters.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/pka.py` & `tscode-0.4.9/tscode/pka.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/profiler.py` & `tscode-0.4.9/tscode/profiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pstats import Stats
 
 from tscode.embedder import Embedder
 
 
 def profiled_wrapper(filename, name):
 
-    datafile = f"TSCoDe_{name}_cProfile.dat"
+    datafile = f"tscode_{name}_cProfile.dat"
     cProfile.run("Embedder(filename, args.name).run()", datafile)
 
-    with open(f"TSCoDe_{name}_cProfile_output_time.txt", "w") as f:
+    with open(f"tscode_{name}_cProfile_output_time.txt", "w") as f:
         p = Stats(datafile, stream=f)
         p.sort_stats("time").print_stats()
 
-    with open(f"TSCoDe_{name}_cProfile_output_cumtime.txt", "w") as f:
+    with open(f"tscode_{name}_cProfile_output_cumtime.txt", "w") as f:
         p = Stats(datafile, stream=f)
         p.sort_stats("cumtime").print_stats()
```

### Comparing `tscode-0.4.8/tscode/pt.py` & `tscode-0.4.9/tscode/pt.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,10 +13,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 '''
 from periodictable import core, covalent_radius, mass
 
-pt = core.PeriodicTable(table="H=1")
-covalent_radius.init(pt)
-mass.init(pt)
+for pt_n in range(5):
+    try:
+        pt = core.PeriodicTable(table=f"H={pt_n+1}")
+        covalent_radius.init(pt)
+        mass.init(pt)
+    except ValueError:
+        continue
+    break
```

### Comparing `tscode-0.4.8/tscode/python_functions.py` & `tscode-0.4.9/tscode/python_functions.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/quotes.json` & `tscode-0.4.9/tscode/quotes.json`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/quotes.py` & `tscode-0.4.9/tscode/quotes.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/reactive_atoms_classes.py` & `tscode-0.4.9/tscode/reactive_atoms_classes.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/references.py` & `tscode-0.4.9/tscode/references.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/rmsd_pruning.py` & `tscode-0.4.9/tscode/rmsd_pruning.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/settings.py` & `tscode-0.4.9/tscode/settings.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/solvents.py` & `tscode-0.4.9/tscode/solvents.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/tests.py` & `tscode-0.4.9/tscode/tests.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/torsion_module.py` & `tscode-0.4.9/tscode/torsion_module.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode/utils.py` & `tscode-0.4.9/tscode/utils.py`

 * *Files identical despite different names*

### Comparing `tscode-0.4.8/tscode.egg-info/PKG-INFO` & `tscode-0.4.9/tscode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscode
-Version: 0.4.8
+Version: 0.4.9
 Summary: Computational chemistry general purpose transition state builder and ensemble optimizer
 Home-page: https://www.github.com/ntampellini/tscode
 Author: Nicolò Tampellini
 Author-email: nicolo.tampellini@yale.edu
 Keywords: computational chemistry,ASE,transition state,xtb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -36,14 +36,21 @@
 ## TSCoDe Changelog
 
 <!-- - Introduced compatibility of SADDLE and NEB keywords for scan> runs with both 2 indices (distance scans) and 4 indices (distance scans) -->
 
 <!-- - ... mep_relax> BETA
 - ... IMAGES kw, also implement it for neb>-->
 
+## 0.4.9 (February 22, 2024)
+- CREST constraints (mtd_search>) are now passed as distance constraints instead of atom fixing (forgot to implement it this way before?).
+- CREST metadynamics input/output files are all retained now and not deleted after execution.
+- Output names changed from starting with "TSCoDe" to "tscode" for easier typing.
+- Modified variable definition of periodic table in tscode.pt to avoid ValueError(s).
+- Added the mep_relax> operator (beta, not present in documentation) to relax chains of images along the PES. Useful to get good starting points for higher-level NEB calculations. First, the optimization is performed by retaining all bond distances, which are then relaxed after the first cycle is converged (developed to find atropisomer interconversion pathways).
+
 ## 0.4.8 (February 2, 2024)
 - Updated library dependency versions.
 
 ## 0.4.7 (Januray 28, 2024)
 - Restyled copy of input in the log file.
 - Added citations to the main program and external modules if they are used (references.py, embedder.py/_print_references).
 - In runs with operators, t_start_run is set before running the first operator, and it is not overwritten by RunEmbedding if it was already set. This makes sure that the final time always includes the time spent executing the operators.
```

### Comparing `tscode-0.4.8/tscode.egg-info/SOURCES.txt` & `tscode-0.4.9/tscode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

