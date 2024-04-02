# Comparing `tmp/PyPartMC-1.1.3.tar.gz` & `tmp/PyPartMC-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPartMC-1.1.3.tar", last modified: Thu Mar 21 23:11:07 2024, max compression
+gzip compressed data, was "PyPartMC-1.1.4.tar", last modified: Tue Apr  2 06:58:12 2024, max compression
```

## Comparing `PyPartMC-1.1.3.tar` & `PyPartMC-1.1.4.tar`

### file list

```diff
@@ -1,953 +1,953 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.276281 PyPartMC-1.1.3/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.727076 PyPartMC-1.1.3/.binder/
--rwxr-xr-x   0 runner     (501) staff       (20)       58 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.binder/postBuild
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.binder/requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.686423 PyPartMC-1.1.3/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.733322 PyPartMC-1.1.3/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)      283 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/cancel.yml
--rw-r--r--   0 runner     (501) staff       (20)      735 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/conda.yml
--rw-r--r--   0 runner     (501) staff       (20)      278 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/cpplint.yml
--rw-r--r--   0 runner     (501) staff       (20)      301 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/forlint.yml
--rw-r--r--   0 runner     (501) staff       (20)      831 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/pdoc.yml
--rw-r--r--   0 runner     (501) staff       (20)      414 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner     (501) staff       (20)      939 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner     (501) staff       (20)     4388 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/readme_listings.yml
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/stale.yml
--rw-r--r--   0 runner     (501) staff       (20)     8587 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.github/workflows/tests+pypi.yml
--rw-r--r--   0 runner     (501) staff       (20)       18 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1740 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)      455 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1383 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/.zenodo.json
--rw-r--r--   0 runner     (501) staff       (20)      836 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/CITATION.cff
--rw-r--r--   0 runner     (501) staff       (20)    20001 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    35149 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    11316 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    21216 2024-03-21 23:11:07.275305 PyPartMC-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.733892 PyPartMC-1.1.3/PyPartMC/
--rw-r--r--   0 runner     (501) staff       (20)     2183 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/PyPartMC/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.273389 PyPartMC-1.1.3/PyPartMC.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    21216 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    37381 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       57 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       19 2024-03-21 23:11:06.000000 PyPartMC-1.1.3/PyPartMC.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)    20491 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.750585 PyPartMC-1.1.3/examples/
--rw-r--r--   0 runner     (501) staff       (20)   205868 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/cloud_parcel.ipynb
--rw-r--r--   0 runner     (501) staff       (20)     2973 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/hello_world.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    18157 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/lognorm_ex.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   239412 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/mie_optical.ipynb
--rw-r--r--   0 runner     (501) staff       (20)  1128494 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/particle_simulation.ipynb
--rw-r--r--   0 runner     (501) staff       (20)  1681038 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/process_simulation_output.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    45354 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/terminal_velocities.ipynb
--rw-r--r--   0 runner     (501) staff       (20)     6243 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/examples/widgets_playground.ipynb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.707254 PyPartMC-1.1.3/gitmodules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.751184 PyPartMC-1.1.3/gitmodules/SuiteSparse/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.688666 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.752897 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Include/
--rw-r--r--   0 runner     (501) staff       (20)    17821 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Include/amd.h
--rw-r--r--   0 runner     (501) staff       (20)     8238 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Include/amd_internal.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.761631 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/
--rw-r--r--   0 runner     (501) staff       (20)    52625 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd.f
--rw-r--r--   0 runner     (501) staff       (20)     5710 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_1.c
--rw-r--r--   0 runner     (501) staff       (20)    64825 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_2.c
--rw-r--r--   0 runner     (501) staff       (20)     4847 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_aat.c
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_control.c
--rw-r--r--   0 runner     (501) staff       (20)     1253 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c
--rw-r--r--   0 runner     (501) staff       (20)     5012 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_dump.c
--rw-r--r--   0 runner     (501) staff       (20)      837 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_global.c
--rw-r--r--   0 runner     (501) staff       (20)     4293 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_info.c
--rw-r--r--   0 runner     (501) staff       (20)     6031 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_order.c
--rw-r--r--   0 runner     (501) staff       (20)     3703 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c
--rw-r--r--   0 runner     (501) staff       (20)     5509 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c
--rw-r--r--   0 runner     (501) staff       (20)     3808 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c
--rw-r--r--   0 runner     (501) staff       (20)     2980 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_valid.c
--rw-r--r--   0 runner     (501) staff       (20)    52282 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amdbar.f
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.689556 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.762756 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Include/
--rw-r--r--   0 runner     (501) staff       (20)    12382 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Include/btf.h
--rw-r--r--   0 runner     (501) staff       (20)     1427 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Include/btf_internal.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.764221 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/
--rw-r--r--   0 runner     (501) staff       (20)    15950 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_order.c
--rw-r--r--   0 runner     (501) staff       (20)    24167 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.690834 PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.764911 PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Include/
--rw-r--r--   0 runner     (501) staff       (20)     8361 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Include/colamd.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.765603 PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Source/
--rw-r--r--   0 runner     (501) staff       (20)   107525 2024-03-21 23:09:50.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Source/colamd.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.691759 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.767655 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/
--rw-r--r--   0 runner     (501) staff       (20)    29763 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu.h
--rw-r--r--   0 runner     (501) staff       (20)     6581 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu_internal.h
--rw-r--r--   0 runner     (501) staff       (20)    19461 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu_version.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.780927 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/
--rw-r--r--   0 runner     (501) staff       (20)    24701 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu.c
--rw-r--r--   0 runner     (501) staff       (20)    16732 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c
--rw-r--r--   0 runner     (501) staff       (20)    11585 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c
--rw-r--r--   0 runner     (501) staff       (20)     1923 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c
--rw-r--r--   0 runner     (501) staff       (20)    16659 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c
--rw-r--r--   0 runner     (501) staff       (20)     4560 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_dump.c
--rw-r--r--   0 runner     (501) staff       (20)     8011 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_extract.c
--rw-r--r--   0 runner     (501) staff       (20)    18700 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_factor.c
--rw-r--r--   0 runner     (501) staff       (20)     1992 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c
--rw-r--r--   0 runner     (501) staff       (20)      982 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c
--rw-r--r--   0 runner     (501) staff       (20)    34162 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c
--rw-r--r--   0 runner     (501) staff       (20)     7002 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_memory.c
--rw-r--r--   0 runner     (501) staff       (20)    17034 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c
--rw-r--r--   0 runner     (501) staff       (20)     4627 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_scale.c
--rw-r--r--   0 runner     (501) staff       (20)    13209 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_solve.c
--rw-r--r--   0 runner     (501) staff       (20)     4261 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_sort.c
--rw-r--r--   0 runner     (501) staff       (20)    15641 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c
--rw-r--r--   0 runner     (501) staff       (20)    51560 2024-03-21 23:09:52.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/LICENSE.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.782465 PyPartMC-1.1.3/gitmodules/SuiteSparse/SuiteSparse_config/
--rw-r--r--   0 runner     (501) staff       (20)    16453 2024-03-21 23:09:53.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
--rw-r--r--   0 runner     (501) staff       (20)     7692 2024-03-21 23:09:53.000000 PyPartMC-1.1.3/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.783500 PyPartMC-1.1.3/gitmodules/camp/
--rw-r--r--   0 runner     (501) staff       (20)    28281 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1122 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/COPYING
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.811745 PyPartMC-1.1.3/gitmodules/camp/src/
--rw-r--r--   0 runner     (501) staff       (20)     9605 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/Jacobian.c
--rw-r--r--   0 runner     (501) staff       (20)     5319 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/Jacobian.h
--rw-r--r--   0 runner     (501) staff       (20)    24549 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     9949 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1311 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_solver.h
--rw-r--r--   0 runner     (501) staff       (20)    29175 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    14653 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    23664 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     2489 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.814366 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/
--rw-r--r--   0 runner     (501) staff       (20)    48515 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90
--rw-r--r--   0 runner     (501) staff       (20)    29575 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c
--rw-r--r--   0 runner     (501) staff       (20)    27555 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)    18689 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c
--rw-r--r--   0 runner     (501) staff       (20)     7067 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/aero_reps.h
--rw-r--r--   0 runner     (501) staff       (20)    11196 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_common.h
--rw-r--r--   0 runner     (501) staff       (20)    67931 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_core.F90
--rw-r--r--   0 runner     (501) staff       (20)     8991 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_debug.h
--rw-r--r--   0 runner     (501) staff       (20)    71748 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     3852 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_solver.h
--rw-r--r--   0 runner     (501) staff       (20)    40570 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_solver_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     5666 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/camp_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    27287 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/chem_spec_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     3018 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/constants.F90
--rw-r--r--   0 runner     (501) staff       (20)     1076 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.F90
--rw-r--r--   0 runner     (501) staff       (20)    12725 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.c
--rw-r--r--   0 runner     (501) staff       (20)      722 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.h
--rw-r--r--   0 runner     (501) staff       (20)    14448 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    14432 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/mechanism_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    53674 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/mpi.F90
--rw-r--r--   0 runner     (501) staff       (20)    28496 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/property.F90
--rw-r--r--   0 runner     (501) staff       (20)    18982 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)     4783 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rand_gsl.c
--rw-r--r--   0 runner     (501) staff       (20)    24970 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxn_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    19550 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxn_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    34236 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxn_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1741 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxn_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.835687 PyPartMC-1.1.3/gitmodules/camp/src/rxns/
--rw-r--r--   0 runner     (501) staff       (20)    10318 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90
--rw-r--r--   0 runner     (501) staff       (20)     8481 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c
--rw-r--r--   0 runner     (501) staff       (20)    11012 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90
--rw-r--r--   0 runner     (501) staff       (20)     8771 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c
--rw-r--r--   0 runner     (501) staff       (20)    18534 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90
--rw-r--r--   0 runner     (501) staff       (20)    21438 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c
--rw-r--r--   0 runner     (501) staff       (20)    19588 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90
--rw-r--r--   0 runner     (501) staff       (20)    33922 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c
--rw-r--r--   0 runner     (501) staff       (20)    19694 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90
--rw-r--r--   0 runner     (501) staff       (20)    23125 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c
--rw-r--r--   0 runner     (501) staff       (20)    10732 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_arrhenius.F90
--rw-r--r--   0 runner     (501) staff       (20)     8214 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_arrhenius.c
--rw-r--r--   0 runner     (501) staff       (20)    19396 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90
--rw-r--r--   0 runner     (501) staff       (20)    17290 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c
--rw-r--r--   0 runner     (501) staff       (20)    23968 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)    18987 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.c
--rw-r--r--   0 runner     (501) staff       (20)    12259 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_emission.F90
--rw-r--r--   0 runner     (501) staff       (20)     7225 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_emission.c
--rw-r--r--   0 runner     (501) staff       (20)    12745 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_first_order_loss.F90
--rw-r--r--   0 runner     (501) staff       (20)     7978 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_first_order_loss.c
--rw-r--r--   0 runner     (501) staff       (20)    16156 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)    10155 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_photolysis.c
--rw-r--r--   0 runner     (501) staff       (20)    12152 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_surface.F90
--rw-r--r--   0 runner     (501) staff       (20)    16686 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_surface.c
--rw-r--r--   0 runner     (501) staff       (20)    11433 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90
--rw-r--r--   0 runner     (501) staff       (20)     9118 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c
--rw-r--r--   0 runner     (501) staff       (20)    10906 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_troe.F90
--rw-r--r--   0 runner     (501) staff       (20)     8616 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_troe.c
--rw-r--r--   0 runner     (501) staff       (20)    12325 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90
--rw-r--r--   0 runner     (501) staff       (20)    10741 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c
--rw-r--r--   0 runner     (501) staff       (20)     9518 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90
--rw-r--r--   0 runner     (501) staff       (20)     8366 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c
--rw-r--r--   0 runner     (501) staff       (20)    14382 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wet_deposition.F90
--rw-r--r--   0 runner     (501) staff       (20)     8365 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wet_deposition.c
--rw-r--r--   0 runner     (501) staff       (20)    24567 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/rxns.h
--rw-r--r--   0 runner     (501) staff       (20)     5440 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/solver_stats.F90
--rw-r--r--   0 runner     (501) staff       (20)    21468 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_model_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     8903 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_model_factory.F90
--rw-r--r--   0 runner     (501) staff       (20)    20633 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_model_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     1390 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_model_solver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.839884 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/
--rw-r--r--   0 runner     (501) staff       (20)    35354 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90
--rw-r--r--   0 runner     (501) staff       (20)    23405 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c
--rw-r--r--   0 runner     (501) staff       (20)    31875 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90
--rw-r--r--   0 runner     (501) staff       (20)    34859 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c
--rw-r--r--   0 runner     (501) staff       (20)    29725 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90
--rw-r--r--   0 runner     (501) staff       (20)    22008 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c
--rw-r--r--   0 runner     (501) staff       (20)     4665 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/sub_models.h
--rw-r--r--   0 runner     (501) staff       (20)     3081 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/time_derivative.c
--rw-r--r--   0 runner     (501) staff       (20)     2734 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/time_derivative.h
--rw-r--r--   0 runner     (501) staff       (20)    56058 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/util.F90
--rw-r--r--   0 runner     (501) staff       (20)     9473 2024-03-21 23:09:54.000000 PyPartMC-1.1.3/gitmodules/camp/src/util.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.840517 PyPartMC-1.1.3/gitmodules/json/
--rw-r--r--   0 runner     (501) staff       (20)     1076 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/LICENSE.MIT
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.695732 PyPartMC-1.1.3/gitmodules/json/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.886039 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/
--rw-r--r--   0 runner     (501) staff       (20)     2000 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/adl_serializer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3183 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.891997 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.894400 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/
--rw-r--r--   0 runner     (501) staff       (20)    18439 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp
--rw-r--r--   0 runner     (501) staff       (20)    38114 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp
--rw-r--r--   0 runner     (501) staff       (20)    14612 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8820 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/exceptions.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3710 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/hash.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.899480 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/
--rw-r--r--   0 runner     (501) staff       (20)    95726 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp
--rw-r--r--   0 runner     (501) staff       (20)    17017 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp
--rw-r--r--   0 runner     (501) staff       (20)    20782 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp
--rw-r--r--   0 runner     (501) staff       (20)    54235 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/lexer.hpp
--rw-r--r--   0 runner     (501) staff       (20)    18415 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/parser.hpp
--rw-r--r--   0 runner     (501) staff       (20)      605 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/position_t.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.903720 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/
--rw-r--r--   0 runner     (501) staff       (20)      720 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23112 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5838 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1404 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3509 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2918 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp
--rw-r--r--   0 runner     (501) staff       (20)    32304 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/json_pointer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1460 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/json_ref.hpp
--rw-r--r--   0 runner     (501) staff       (20)    41851 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/macro_scope.hpp
--rw-r--r--   0 runner     (501) staff       (20)      749 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.908062 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.909408 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/call_std/
--rw-r--r--   0 runner     (501) staff       (20)      143 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/call_std/begin.hpp
--rw-r--r--   0 runner     (501) staff       (20)      142 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/call_std/end.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4609 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1800 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/detected.hpp
--rw-r--r--   0 runner     (501) staff       (20)      174 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/identity_tag.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6609 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp
--rw-r--r--   0 runner     (501) staff       (20)    22856 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp
--rw-r--r--   0 runner     (501) staff       (20)      244 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/void_t.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.911584 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/
--rw-r--r--   0 runner     (501) staff       (20)    69584 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3773 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp
--rw-r--r--   0 runner     (501) staff       (20)    39511 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/serializer.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5697 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/string_concat.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1860 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/string_escape.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3098 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/value_t.hpp
--rw-r--r--   0 runner     (501) staff       (20)   186996 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/json.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2118 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/json_fwd.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7469 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/ordered_map.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.698185 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.913500 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/hedley/
--rw-r--r--   0 runner     (501) staff       (20)    86041 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5205 2024-03-21 23:10:08.000000 PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.841092 PyPartMC-1.1.3/gitmodules/json-fortran/
--rw-r--r--   0 runner     (501) staff       (20)     2849 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.848574 PyPartMC-1.1.3/gitmodules/json-fortran/src/
--rw-r--r--   0 runner     (501) staff       (20)   121590 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_file_module.F90
--rw-r--r--   0 runner     (501) staff       (20)      842 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_scalar_by_path.inc
--rw-r--r--   0 runner     (501) staff       (20)      767 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_vec_by_path.inc
--rw-r--r--   0 runner     (501) staff       (20)     1264 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc
--rw-r--r--   0 runner     (501) staff       (20)     4725 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_initialize_arguments.inc
--rw-r--r--   0 runner     (501) staff       (20)      499 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_initialize_dummy_arguments.inc
--rw-r--r--   0 runner     (501) staff       (20)     5759 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_kinds.F90
--rw-r--r--   0 runner     (501) staff       (20)     2480 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_macros.inc
--rw-r--r--   0 runner     (501) staff       (20)     4027 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_module.F90
--rw-r--r--   0 runner     (501) staff       (20)     9238 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_parameters.F90
--rw-r--r--   0 runner     (501) staff       (20)    31512 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_string_utilities.F90
--rw-r--r--   0 runner     (501) staff       (20)   456578 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/json_value_module.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.882719 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.883209 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/introspection/
--rw-r--r--   0 runner     (501) staff       (20)     1194 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90
--rw-r--r--   0 runner     (501) staff       (20)    16922 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_01.F90
--rw-r--r--   0 runner     (501) staff       (20)    14591 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_02.F90
--rw-r--r--   0 runner     (501) staff       (20)     4824 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_03.F90
--rw-r--r--   0 runner     (501) staff       (20)     5454 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_04.F90
--rw-r--r--   0 runner     (501) staff       (20)     3597 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_05.F90
--rw-r--r--   0 runner     (501) staff       (20)     4648 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_06.F90
--rw-r--r--   0 runner     (501) staff       (20)     7880 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_07.F90
--rw-r--r--   0 runner     (501) staff       (20)     4903 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_08.F90
--rw-r--r--   0 runner     (501) staff       (20)     4843 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_09.F90
--rw-r--r--   0 runner     (501) staff       (20)    11909 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_10.F90
--rw-r--r--   0 runner     (501) staff       (20)     9207 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_11.F90
--rw-r--r--   0 runner     (501) staff       (20)     8710 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_12.F90
--rw-r--r--   0 runner     (501) staff       (20)     2173 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_13.F90
--rw-r--r--   0 runner     (501) staff       (20)     4981 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_14.F90
--rw-r--r--   0 runner     (501) staff       (20)     8746 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_15.F90
--rw-r--r--   0 runner     (501) staff       (20)     7282 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_16.F90
--rw-r--r--   0 runner     (501) staff       (20)     5649 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_17.F90
--rw-r--r--   0 runner     (501) staff       (20)     3614 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_18.F90
--rw-r--r--   0 runner     (501) staff       (20)     5793 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_19.F90
--rw-r--r--   0 runner     (501) staff       (20)     7724 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_20.F90
--rw-r--r--   0 runner     (501) staff       (20)     2620 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_21.F90
--rw-r--r--   0 runner     (501) staff       (20)     2648 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_22.F90
--rw-r--r--   0 runner     (501) staff       (20)     8627 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_23.F90
--rw-r--r--   0 runner     (501) staff       (20)     6317 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_24.F90
--rw-r--r--   0 runner     (501) staff       (20)     4863 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_25.F90
--rw-r--r--   0 runner     (501) staff       (20)     2645 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_26.F90
--rw-r--r--   0 runner     (501) staff       (20)     2569 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_27.F90
--rw-r--r--   0 runner     (501) staff       (20)     3824 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_28.F90
--rw-r--r--   0 runner     (501) staff       (20)     5889 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_29.F90
--rw-r--r--   0 runner     (501) staff       (20)     2342 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_30.F90
--rw-r--r--   0 runner     (501) staff       (20)     4697 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_31.F90
--rw-r--r--   0 runner     (501) staff       (20)     3853 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_32.F90
--rw-r--r--   0 runner     (501) staff       (20)     3607 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_33.F90
--rw-r--r--   0 runner     (501) staff       (20)     5045 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_34.F90
--rw-r--r--   0 runner     (501) staff       (20)     3079 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_35.F90
--rw-r--r--   0 runner     (501) staff       (20)     4194 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_36.F90
--rw-r--r--   0 runner     (501) staff       (20)     3650 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_37.F90
--rw-r--r--   0 runner     (501) staff       (20)     4150 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_38.F90
--rw-r--r--   0 runner     (501) staff       (20)     2407 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_39.F90
--rw-r--r--   0 runner     (501) staff       (20)     1803 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_40.F90
--rw-r--r--   0 runner     (501) staff       (20)     3928 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_41.F90
--rw-r--r--   0 runner     (501) staff       (20)     4079 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_42.F90
--rw-r--r--   0 runner     (501) staff       (20)     2687 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_43.F90
--rw-r--r--   0 runner     (501) staff       (20)     3060 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_44.F90
--rw-r--r--   0 runner     (501) staff       (20)     4378 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_45.F90
--rw-r--r--   0 runner     (501) staff       (20)    12438 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_46.F90
--rw-r--r--   0 runner     (501) staff       (20)     4331 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_47.F90
--rw-r--r--   0 runner     (501) staff       (20)     2691 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_48.F90
--rw-r--r--   0 runner     (501) staff       (20)     1976 2024-03-21 23:10:10.000000 PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_49.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.915524 PyPartMC-1.1.3/gitmodules/netcdf-c/
--rw-r--r--   0 runner     (501) staff       (20)    90875 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1452 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/COPYRIGHT
--rw-r--r--   0 runner     (501) staff       (20)    18999 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/config.h.cmake.in
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.939899 PyPartMC-1.1.3/gitmodules/netcdf-c/include/
--rw-r--r--   0 runner     (501) staff       (20)      643 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/fbits.h
--rw-r--r--   0 runner     (501) staff       (20)     4907 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc.h
--rw-r--r--   0 runner     (501) staff       (20)     5614 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc3dispatch.h
--rw-r--r--   0 runner     (501) staff       (20)     8982 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc3internal.h
--rw-r--r--   0 runner     (501) staff       (20)     6820 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc4dispatch.h
--rw-r--r--   0 runner     (501) staff       (20)    23203 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc4internal.h
--rw-r--r--   0 runner     (501) staff       (20)     1659 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc_logging.h
--rw-r--r--   0 runner     (501) staff       (20)     2621 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc_provenance.h
--rw-r--r--   0 runner     (501) staff       (20)     2062 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncauth.h
--rw-r--r--   0 runner     (501) staff       (20)     2261 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncbytes.h
--rw-r--r--   0 runner     (501) staff       (20)     3295 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncconfigure.h
--rw-r--r--   0 runner     (501) staff       (20)      410 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nccrc.h
--rw-r--r--   0 runner     (501) staff       (20)     7474 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncdispatch.h
--rw-r--r--   0 runner     (501) staff       (20)      674 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncexternl.h
--rw-r--r--   0 runner     (501) staff       (20)     3607 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nchashmap.h
--rw-r--r--   0 runner     (501) staff       (20)     1906 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nchttp.h
--rw-r--r--   0 runner     (501) staff       (20)     3226 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncindex.h
--rw-r--r--   0 runner     (501) staff       (20)     2254 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nclist.h
--rw-r--r--   0 runner     (501) staff       (20)     1851 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/nclog.h
--rw-r--r--   0 runner     (501) staff       (20)     1086 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncmodel.h
--rw-r--r--   0 runner     (501) staff       (20)     2215 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncoffsets.h
--rw-r--r--   0 runner     (501) staff       (20)     8248 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncpathmgr.h
--rw-r--r--   0 runner     (501) staff       (20)     3396 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncrc.h
--rw-r--r--   0 runner     (501) staff       (20)     2079 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncs3sdk.h
--rw-r--r--   0 runner     (501) staff       (20)     4264 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncuri.h
--rw-r--r--   0 runner     (501) staff       (20)     1420 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncutf8.h
--rw-r--r--   0 runner     (501) staff       (20)     1210 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncxml.h
--rw-r--r--   0 runner     (501) staff       (20)    73732 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf.h
--rw-r--r--   0 runner     (501) staff       (20)     4090 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_aux.h
--rw-r--r--   0 runner     (501) staff       (20)    13091 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_dispatch.h.in
--rw-r--r--   0 runner     (501) staff       (20)     1606 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_f.h
--rw-r--r--   0 runner     (501) staff       (20)     4065 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_filter.h
--rw-r--r--   0 runner     (501) staff       (20)     1337 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_mem.h
--rw-r--r--   0 runner     (501) staff       (20)     3835 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_meta.h.in
--rw-r--r--   0 runner     (501) staff       (20)     1971 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/onstack.h
--rw-r--r--   0 runner     (501) staff       (20)      569 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/include/rnd.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.973271 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/
--rw-r--r--   0 runner     (501) staff       (20)     6128 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/datt.c
--rw-r--r--   0 runner     (501) staff       (20)    23572 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattget.c
--rw-r--r--   0 runner     (501) staff       (20)    13788 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattinq.c
--rw-r--r--   0 runner     (501) staff       (20)    21685 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattput.c
--rw-r--r--   0 runner     (501) staff       (20)    12111 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dauth.c
--rw-r--r--   0 runner     (501) staff       (20)    27254 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/daux.c
--rw-r--r--   0 runner     (501) staff       (20)    14827 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcompound.c
--rw-r--r--   0 runner     (501) staff       (20)    21188 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcopy.c
--rw-r--r--   0 runner     (501) staff       (20)    10910 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcrc64.c
--rw-r--r--   0 runner     (501) staff       (20)    16745 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ddim.c
--rw-r--r--   0 runner     (501) staff       (20)     3272 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ddispatch.c
--rw-r--r--   0 runner     (501) staff       (20)     5448 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/denum.c
--rw-r--r--   0 runner     (501) staff       (20)    10328 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/derror.c
--rw-r--r--   0 runner     (501) staff       (20)    75413 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dfile.c
--rw-r--r--   0 runner     (501) staff       (20)    16459 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dfilter.c
--rw-r--r--   0 runner     (501) staff       (20)     9601 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dgroup.c
--rw-r--r--   0 runner     (501) staff       (20)    43874 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinfermodel.c
--rw-r--r--   0 runner     (501) staff       (20)    16008 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinstance.c
--rw-r--r--   0 runner     (501) staff       (20)    19387 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinstance_intern.c
--rw-r--r--   0 runner     (501) staff       (20)     6562 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dmissing.c
--rw-r--r--   0 runner     (501) staff       (20)    15177 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dnotnc4.c
--rw-r--r--   0 runner     (501) staff       (20)    11901 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/doffsets.c
--rw-r--r--   0 runner     (501) staff       (20)     2170 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dopaque.c
--rw-r--r--   0 runner     (501) staff       (20)    32961 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dpathmgr.c
--rw-r--r--   0 runner     (501) staff       (20)    32946 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/drc.c
--rw-r--r--   0 runner     (501) staff       (20)     9341 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ds3util.c
--rw-r--r--   0 runner     (501) staff       (20)     7588 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dstring.c
--rw-r--r--   0 runner     (501) staff       (20)     5453 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dtype.c
--rw-r--r--   0 runner     (501) staff       (20)     4527 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dutf8.c
--rw-r--r--   0 runner     (501) staff       (20)    10862 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dutil.c
--rw-r--r--   0 runner     (501) staff       (20)    52386 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvar.c
--rw-r--r--   0 runner     (501) staff       (20)    41839 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarget.c
--rw-r--r--   0 runner     (501) staff       (20)    22318 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarinq.c
--rw-r--r--   0 runner     (501) staff       (20)    38016 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarput.c
--rw-r--r--   0 runner     (501) staff       (20)     5687 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvlen.c
--rw-r--r--   0 runner     (501) staff       (20)     4039 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nc.c
--rw-r--r--   0 runner     (501) staff       (20)     4595 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ncbytes.c
--rw-r--r--   0 runner     (501) staff       (20)   149230 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nchashmap.c
--rw-r--r--   0 runner     (501) staff       (20)     6328 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclist.c
--rw-r--r--   0 runner     (501) staff       (20)     6507 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclistmgr.c
--rw-r--r--   0 runner     (501) staff       (20)     7281 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclog.c
--rw-r--r--   0 runner     (501) staff       (20)    34144 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ncuri.c
--rw-r--r--   0 runner     (501) staff       (20)    30569 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc.c
--rw-r--r--   0 runner     (501) staff       (20)    29211 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc.h
--rw-r--r--   0 runner     (501) staff       (20)  1621941 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc_data.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.978794 PyPartMC-1.1.3/gitmodules/netcdf-c/liblib/
--rw-r--r--   0 runner     (501) staff       (20)     4004 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/liblib/nc_initialize.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.988877 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/
--rw-r--r--   0 runner     (501) staff       (20)    22640 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/attr.m4
--rw-r--r--   0 runner     (501) staff       (20)    10107 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/dim.c
--rw-r--r--   0 runner     (501) staff       (20)    20016 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/memio.c
--rw-r--r--   0 runner     (501) staff       (20)    12218 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/nc3dispatch.c
--rw-r--r--   0 runner     (501) staff       (20)    42563 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/nc3internal.c
--rw-r--r--   0 runner     (501) staff       (20)     5804 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncio.c
--rw-r--r--   0 runner     (501) staff       (20)     4986 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncio.h
--rw-r--r--   0 runner     (501) staff       (20)    38570 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncx.h
--rw-r--r--   0 runner     (501) staff       (20)    91027 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncx.m4
--rw-r--r--   0 runner     (501) staff       (20)    45195 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/posixio.c
--rw-r--r--   0 runner     (501) staff       (20)    56656 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/putget.m4
--rw-r--r--   0 runner     (501) staff       (20)    34650 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/v1hpg.c
--rw-r--r--   0 runner     (501) staff       (20)    17812 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/var.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.992910 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/
--rw-r--r--   0 runner     (501) staff       (20)     6166 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4cache.c
--rw-r--r--   0 runner     (501) staff       (20)     1933 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4dispatch.c
--rw-r--r--   0 runner     (501) staff       (20)    12192 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4grp.c
--rw-r--r--   0 runner     (501) staff       (20)    60959 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4internal.c
--rw-r--r--   0 runner     (501) staff       (20)    22718 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4type.c
--rw-r--r--   0 runner     (501) staff       (20)    62575 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4var.c
--rw-r--r--   0 runner     (501) staff       (20)    10546 2024-03-21 23:10:17.000000 PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/ncindex.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.993713 PyPartMC-1.1.3/gitmodules/netcdf-fortran/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.994291 PyPartMC-1.1.3/gitmodules/netcdf-fortran/CMakeExtras/
--rw-r--r--   0 runner     (501) staff       (20)     2443 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake
--rw-r--r--   0 runner     (501) staff       (20)     2417 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/COPYRIGHT
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.018206 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/
--rwxr-xr-x   0 runner     (501) staff       (20)    35483 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    33291 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    17109 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    80960 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    15589 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    56443 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90
--rw-r--r--   0 runner     (501) staff       (20)     2732 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4.F90
--rw-r--r--   0 runner     (501) staff       (20)    38904 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90
--rw-r--r--   0 runner     (501) staff       (20)     1899 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90
--rw-r--r--   0 runner     (501) staff       (20)     5233 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_file.F90
--rw-r--r--   0 runner     (501) staff       (20)    33491 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_func.F90
--rw-r--r--   0 runner     (501) staff       (20)      789 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90
--rw-r--r--   0 runner     (501) staff       (20)    16715 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90
--rw-r--r--   0 runner     (501) staff       (20)    16718 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90
--rw-r--r--   0 runner     (501) staff       (20)    11047 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_constants.F90
--rw-r--r--   0 runner     (501) staff       (20)     1719 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_dims.F90
--rw-r--r--   0 runner     (501) staff       (20)   124466 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90
--rw-r--r--   0 runner     (501) staff       (20)     3537 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_externals.F90
--rw-r--r--   0 runner     (501) staff       (20)     5101 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_file.F90
--rw-r--r--   0 runner     (501) staff       (20)     6806 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90
--rw-r--r--   0 runner     (501) staff       (20)    23015 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90
--rw-r--r--   0 runner     (501) staff       (20)     3802 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_variables.F90
--rw-r--r--   0 runner     (501) staff       (20)      959 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    20393 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_attio.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    16094 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_control.F90
--rwxr-xr-x   0 runner     (501) staff       (20)     6572 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_dim.F90
--rwxr-xr-x   0 runner     (501) staff       (20)     8623 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_genatt.F90
--rwxr-xr-x   0 runner     (501) staff       (20)     5086 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_geninq.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    10775 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_genvar.F90
--rwxr-xr-x   0 runner     (501) staff       (20)     7909 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_lib.c
--rwxr-xr-x   0 runner     (501) staff       (20)     4428 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_misc.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    58343 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_nc4.F90
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    23742 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_var1io.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    31119 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varaio.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    38708 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varmio.F90
--rwxr-xr-x   0 runner     (501) staff       (20)    37941 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varsio.F90
--rw-r--r--   0 runner     (501) staff       (20)     2601 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/typeSizes.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.018863 PyPartMC-1.1.3/gitmodules/optional/
--rw-r--r--   0 runner     (501) staff       (20)     7048 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/optional/COPYING
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.701617 PyPartMC-1.1.3/gitmodules/optional/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.019487 PyPartMC-1.1.3/gitmodules/optional/include/tl/
--rw-r--r--   0 runner     (501) staff       (20)    73584 2024-03-21 23:10:20.000000 PyPartMC-1.1.3/gitmodules/optional/include/tl/optional.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.020716 PyPartMC-1.1.3/gitmodules/partmc/
--rw-r--r--   0 runner     (501) staff       (20)    18015 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/COPYING
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.063645 PyPartMC-1.1.3/gitmodules/partmc/src/
--rw-r--r--   0 runner     (501) staff       (20)    18941 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_binned.F90
--rw-r--r--   0 runner     (501) staff       (20)    37336 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    17040 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)     4584 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_info.F90
--rw-r--r--   0 runner     (501) staff       (20)     9722 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_info_array.F90
--rw-r--r--   0 runner     (501) staff       (20)    49450 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_mode.F90
--rw-r--r--   0 runner     (501) staff       (20)    36702 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)    10615 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_particle_array.F90
--rw-r--r--   0 runner     (501) staff       (20)    23922 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_sorted.F90
--rw-r--r--   0 runner     (501) staff       (20)   124072 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    13932 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_weight.F90
--rw-r--r--   0 runner     (501) staff       (20)    27073 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/aero_weight_array.F90
--rw-r--r--   0 runner     (501) staff       (20)     2924 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/bin_average_comp.F90
--rw-r--r--   0 runner     (501) staff       (20)     3825 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/bin_average_size.F90
--rw-r--r--   0 runner     (501) staff       (20)    20694 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/bin_grid.F90
--rw-r--r--   0 runner     (501) staff       (20)     7275 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/camp_interface.F90
--rw-r--r--   0 runner     (501) staff       (20)     8917 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/chamber.F90
--rw-r--r--   0 runner     (501) staff       (20)    19523 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel.F90
--rw-r--r--   0 runner     (501) staff       (20)    11888 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_additive.F90
--rw-r--r--   0 runner     (501) staff       (20)     7285 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown.F90
--rw-r--r--   0 runner     (501) staff       (20)     4941 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown_cont.F90
--rw-r--r--   0 runner     (501) staff       (20)     5034 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown_free.F90
--rw-r--r--   0 runner     (501) staff       (20)     4927 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_constant.F90
--rw-r--r--   0 runner     (501) staff       (20)    11095 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_sedi.F90
--rw-r--r--   0 runner     (501) staff       (20)     7469 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_zero.F90
--rw-r--r--   0 runner     (501) staff       (20)    35666 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coagulation.F90
--rw-r--r--   0 runner     (501) staff       (20)    34136 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/coagulation_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)    30923 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/condense.F90
--rw-r--r--   0 runner     (501) staff       (20)     9565 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/condense_solver.c
--rw-r--r--   0 runner     (501) staff       (20)     2913 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/constants.F90
--rw-r--r--   0 runner     (501) staff       (20)    20205 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     4419 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/exact_soln.F90
--rw-r--r--   0 runner     (501) staff       (20)     3949 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_particles.F90
--rw-r--r--   0 runner     (501) staff       (20)     6528 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_size.F90
--rw-r--r--   0 runner     (501) staff       (20)     5072 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_time.F90
--rw-r--r--   0 runner     (501) staff       (20)     4227 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_env.F90
--rw-r--r--   0 runner     (501) staff       (20)     3867 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_gas.F90
--rw-r--r--   0 runner     (501) staff       (20)     5692 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_sectional_aero_size.F90
--rw-r--r--   0 runner     (501) staff       (20)     4858 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/extract_sectional_aero_time.F90
--rw-r--r--   0 runner     (501) staff       (20)    23458 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/fractal.F90
--rw-r--r--   0 runner     (501) staff       (20)    16247 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/gas_data.F90
--rw-r--r--   0 runner     (501) staff       (20)    22073 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/gas_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     7566 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/getopt.F90
--rw-r--r--   0 runner     (501) staff       (20)    15007 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/integer_rmap.F90
--rw-r--r--   0 runner     (501) staff       (20)    19200 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/integer_rmap2.F90
--rw-r--r--   0 runner     (501) staff       (20)     8378 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/integer_varray.F90
--rw-r--r--   0 runner     (501) staff       (20)    18380 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/mosaic.F90
--rw-r--r--   0 runner     (501) staff       (20)    47083 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/mpi.F90
--rw-r--r--   0 runner     (501) staff       (20)    27550 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/netcdf.F90
--rw-r--r--   0 runner     (501) staff       (20)     8579 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/nucleate.F90
--rw-r--r--   0 runner     (501) staff       (20)     7062 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/numeric_average.F90
--rw-r--r--   0 runner     (501) staff       (20)    10911 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/numeric_diff.F90
--rw-r--r--   0 runner     (501) staff       (20)    30038 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/output.F90
--rw-r--r--   0 runner     (501) staff       (20)    48249 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/partmc.F90
--rw-r--r--   0 runner     (501) staff       (20)     8459 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)    18343 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)     4712 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/rand_gsl.c
--rw-r--r--   0 runner     (501) staff       (20)     2837 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/run_exact.F90
--rw-r--r--   0 runner     (501) staff       (20)    31148 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/run_part.F90
--rw-r--r--   0 runner     (501) staff       (20)    12069 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/run_sect.F90
--rw-r--r--   0 runner     (501) staff       (20)    47571 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/scenario.F90
--rw-r--r--   0 runner     (501) staff       (20)     1563 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/sort.c
--rw-r--r--   0 runner     (501) staff       (20)    23797 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/spec_file.F90
--rw-r--r--   0 runner     (501) staff       (20)     3063 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/spec_line.F90
--rw-r--r--   0 runner     (501) staff       (20)    23957 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/stats.F90
--rw-r--r--   0 runner     (501) staff       (20)      482 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/sys.F90
--rw-r--r--   0 runner     (501) staff       (20)    49504 2024-03-21 23:10:22.000000 PyPartMC-1.1.3/gitmodules/partmc/src/util.F90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.064961 PyPartMC-1.1.3/gitmodules/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    10999 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.703058 PyPartMC-1.1.3/gitmodules/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.075916 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23883 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65224 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.080004 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28078 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    49007 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17971 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    23981 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    44230 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1513 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    31685 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    10728 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4658 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     6923 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8851 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    78946 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9051 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125304 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    80981 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.080482 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    14535 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.081943 PyPartMC-1.1.3/gitmodules/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)    10455 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)    13460 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     7270 2024-03-21 23:10:25.000000 PyPartMC-1.1.3/gitmodules/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.704307 PyPartMC-1.1.3/gitmodules/pybind11_json/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.704518 PyPartMC-1.1.3/gitmodules/pybind11_json/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.082464 PyPartMC-1.1.3/gitmodules/pybind11_json/include/pybind11_json/
--rw-r--r--   0 runner     (501) staff       (20)     7219 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.083057 PyPartMC-1.1.3/gitmodules/span/
--rw-r--r--   0 runner     (501) staff       (20)     1338 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/span/LICENSE_1_0.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.705405 PyPartMC-1.1.3/gitmodules/span/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.083673 PyPartMC-1.1.3/gitmodules/span/include/tcb/
--rw-r--r--   0 runner     (501) staff       (20)    18165 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/span/include/tcb/span.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.084264 PyPartMC-1.1.3/gitmodules/string_view-standalone/
--rw-r--r--   0 runner     (501) staff       (20)     1077 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/string_view-standalone/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.706512 PyPartMC-1.1.3/gitmodules/string_view-standalone/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.084741 PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.085283 PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/detail/
--rw-r--r--   0 runner     (501) staff       (20)    29304 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl
--rw-r--r--   0 runner     (501) staff       (20)    20256 2024-03-21 23:10:26.000000 PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/string_view.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.086403 PyPartMC-1.1.3/gitmodules/sundials/
--rw-r--r--   0 runner     (501) staff       (20)     8077 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1576 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.087854 PyPartMC-1.1.3/gitmodules/sundials/cmake/
--rw-r--r--   0 runner     (501) staff       (20)     2962 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsIndexSize.cmake
--rw-r--r--   0 runner     (501) staff       (20)    10395 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake
--rw-r--r--   0 runner     (501) staff       (20)     4883 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsSetupConfig.cmake
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.709857 PyPartMC-1.1.3/gitmodules/sundials/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.092916 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/
--rw-r--r--   0 runner     (501) staff       (20)     9544 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode.h
--rw-r--r--   0 runner     (501) staff       (20)     1525 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_bandpre.h
--rw-r--r--   0 runner     (501) staff       (20)     2182 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_bbdpre.h
--rw-r--r--   0 runner     (501) staff       (20)     1790 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_diag.h
--rw-r--r--   0 runner     (501) staff       (20)     2035 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_direct.h
--rw-r--r--   0 runner     (501) staff       (20)    10422 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_hypamgpre.h
--rw-r--r--   0 runner     (501) staff       (20)     6515 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_ls.h
--rw-r--r--   0 runner     (501) staff       (20)     2266 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_proj.h
--rw-r--r--   0 runner     (501) staff       (20)     2873 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_spils.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.100732 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/
--rw-r--r--   0 runner     (501) staff       (20)     9721 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_cuda.h
--rw-r--r--   0 runner     (501) staff       (20)     9653 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_hip.h
--rw-r--r--   0 runner     (501) staff       (20)     8671 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_manyvector.h
--rw-r--r--   0 runner     (501) staff       (20)     9959 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h
--rw-r--r--   0 runner     (501) staff       (20)     1644 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_mpiplusx.h
--rw-r--r--   0 runner     (501) staff       (20)     9487 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_openmp.h
--rw-r--r--   0 runner     (501) staff       (20)     9612 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_openmpdev.h
--rw-r--r--   0 runner     (501) staff       (20)    10795 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_parallel.h
--rw-r--r--   0 runner     (501) staff       (20)     9697 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_parhyp.h
--rw-r--r--   0 runner     (501) staff       (20)     9419 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_petsc.h
--rw-r--r--   0 runner     (501) staff       (20)    11042 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_pthreads.h
--rw-r--r--   0 runner     (501) staff       (20)     8267 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_raja.h
--rw-r--r--   0 runner     (501) staff       (20)     8934 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_serial.h
--rw-r--r--   0 runner     (501) staff       (20)    10053 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_sycl.h
--rw-r--r--   0 runner     (501) staff       (20)     5824 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_trilinos.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.101885 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/trilinos/
--rw-r--r--   0 runner     (501) staff       (20)     1819 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23964 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.114716 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/
--rw-r--r--   0 runner     (501) staff       (20)     7791 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_band.h
--rw-r--r--   0 runner     (501) staff       (20)     5329 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_config.in
--rw-r--r--   0 runner     (501) staff       (20)     5520 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8997 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_dense.h
--rw-r--r--   0 runner     (501) staff       (20)    13330 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_direct.h
--rw-r--r--   0 runner     (501) staff       (20)     1690 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_fconfig.in
--rw-r--r--   0 runner     (501) staff       (20)     1123 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_fnvector.h
--rw-r--r--   0 runner     (501) staff       (20)     1128 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_futils.h
--rw-r--r--   0 runner     (501) staff       (20)     5478 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)    10283 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_iterative.h
--rw-r--r--   0 runner     (501) staff       (20)    10707 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_lapack.h
--rw-r--r--   0 runner     (501) staff       (20)     9633 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 runner     (501) staff       (20)     7839 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_math.h
--rw-r--r--   0 runner     (501) staff       (20)     5466 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_matrix.h
--rw-r--r--   0 runner     (501) staff       (20)     4527 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_memory.h
--rw-r--r--   0 runner     (501) staff       (20)     1399 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_mpi_types.h
--rw-r--r--   0 runner     (501) staff       (20)     9190 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 runner     (501) staff       (20)    12719 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nvector.h
--rw-r--r--   0 runner     (501) staff       (20)     4744 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h
--rw-r--r--   0 runner     (501) staff       (20)     4567 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5165 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_types.h
--rw-r--r--   0 runner     (501) staff       (20)     1266 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_version.h
--rw-r--r--   0 runner     (501) staff       (20)     4024 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_xbraid.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.122730 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     2649 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h
--rw-r--r--   0 runner     (501) staff       (20)     4768 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h
--rw-r--r--   0 runner     (501) staff       (20)     2983 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     5603 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h
--rw-r--r--   0 runner     (501) staff       (20)     3142 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h
--rw-r--r--   0 runner     (501) staff       (20)     3171 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h
--rw-r--r--   0 runner     (501) staff       (20)     2751 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h
--rw-r--r--   0 runner     (501) staff       (20)     3052 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h
--rw-r--r--   0 runner     (501) staff       (20)     4553 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h
--rw-r--r--   0 runner     (501) staff       (20)     4872 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h
--rw-r--r--   0 runner     (501) staff       (20)     5330 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h
--rw-r--r--   0 runner     (501) staff       (20)     5237 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h
--rw-r--r--   0 runner     (501) staff       (20)     5621 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h
--rw-r--r--   0 runner     (501) staff       (20)     4533 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.126381 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/
--rw-r--r--   0 runner     (501) staff       (20)     4552 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h
--rw-r--r--   0 runner     (501) staff       (20)     5233 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h
--rw-r--r--   0 runner     (501) staff       (20)     3647 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     5083 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h
--rw-r--r--   0 runner     (501) staff       (20)     5776 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h
--rw-r--r--   0 runner     (501) staff       (20)     3245 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h
--rw-r--r--   0 runner     (501) staff       (20)     5136 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.127836 PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     6202 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h
--rw-r--r--   0 runner     (501) staff       (20)     5449 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h
--rw-r--r--   0 runner     (501) staff       (20)     4071 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:06.717966 PyPartMC-1.1.3/gitmodules/sundials/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.142974 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/
--rw-r--r--   0 runner     (501) staff       (20)     1972 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/CHANGES
--rw-r--r--   0 runner     (501) staff       (20)     3549 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1576 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1166 2024-03-21 23:10:38.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/NOTICE
--rw-r--r--   0 runner     (501) staff       (20)     2708 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/README.md
--rw-r--r--   0 runner     (501) staff       (20)   135753 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode.c
--rw-r--r--   0 runner     (501) staff       (20)    18212 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bandpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2383 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    22668 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bbdpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2621 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    13629 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_diag.c
--rw-r--r--   0 runner     (501) staff       (20)     2240 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_diag_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     1956 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_direct.c
--rw-r--r--   0 runner     (501) staff       (20)    14722 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5554 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_fused_stubs.c
--rw-r--r--   0 runner     (501) staff       (20)    14959 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_hypamgpre.c
--rw-r--r--   0 runner     (501) staff       (20)     2766 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    29404 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    28172 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_io.c
--rw-r--r--   0 runner     (501) staff       (20)    58312 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_ls.c
--rw-r--r--   0 runner     (501) staff       (20)     8077 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_ls_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    12911 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_nls.c
--rw-r--r--   0 runner     (501) staff       (20)    12603 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_proj.c
--rw-r--r--   0 runner     (501) staff       (20)     3079 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_proj_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     2943 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_spils.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.153455 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/
--rw-r--r--   0 runner     (501) staff       (20)     1734 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     4616 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/Makefile.in
--rw-r--r--   0 runner     (501) staff       (20)     3464 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvband.c
--rw-r--r--   0 runner     (501) staff       (20)     4950 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c
--rw-r--r--   0 runner     (501) staff       (20)    22548 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h
--rw-r--r--   0 runner     (501) staff       (20)     2063 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbp.c
--rw-r--r--   0 runner     (501) staff       (20)    14934 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbp.h
--rw-r--r--   0 runner     (501) staff       (20)     2952 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvdense.c
--rw-r--r--   0 runner     (501) staff       (20)     2046 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvewt.c
--rw-r--r--   0 runner     (501) staff       (20)     3904 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c
--rw-r--r--   0 runner     (501) staff       (20)     1370 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c
--rw-r--r--   0 runner     (501) staff       (20)     1344 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c
--rw-r--r--   0 runner     (501) staff       (20)     1502 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c
--rw-r--r--   0 runner     (501) staff       (20)    15564 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvode.c
--rw-r--r--   0 runner     (501) staff       (20)    49120 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvode.h
--rw-r--r--   0 runner     (501) staff       (20)     4190 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c
--rw-r--r--   0 runner     (501) staff       (20)     2399 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvroot.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvroot.h
--rw-r--r--   0 runner     (501) staff       (20)     2921 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.156278 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1483 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    43017 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    83166 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.157079 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/
--rw-r--r--   0 runner     (501) staff       (20)     1562 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.160721 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/
--rw-r--r--   0 runner     (501) staff       (20)     1648 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.162803 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/
--rw-r--r--   0 runner     (501) staff       (20)      979 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    25549 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    40279 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     3740 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fnvector_serial.c
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fnvector_serial.h
--rw-r--r--   0 runner     (501) staff       (20)    47581 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/nvector_serial.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.173914 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/
--rw-r--r--   0 runner     (501) staff       (20)     3022 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.180863 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1109 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     7228 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     2922 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    13682 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    19932 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     9392 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     9541 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    11515 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    12797 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)    24749 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    42038 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     6561 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c
--rw-r--r--   0 runner     (501) staff       (20)      957 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     6784 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_band.c
--rw-r--r--   0 runner     (501) staff       (20)     3712 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_cuda.h
--rw-r--r--   0 runner     (501) staff       (20)     7056 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh
--rw-r--r--   0 runner     (501) staff       (20)     1403 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_debug.h
--rw-r--r--   0 runner     (501) staff       (20)     9098 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_dense.c
--rw-r--r--   0 runner     (501) staff       (20)     6468 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_direct.c
--rw-r--r--   0 runner     (501) staff       (20)      964 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_futils.c
--rw-r--r--   0 runner     (501) staff       (20)     2500 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_hip.h
--rw-r--r--   0 runner     (501) staff       (20)     7260 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8008 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_iterative.c
--rw-r--r--   0 runner     (501) staff       (20)     5667 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_linearsolver.c
--rw-r--r--   0 runner     (501) staff       (20)     2956 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_math.c
--rw-r--r--   0 runner     (501) staff       (20)     4633 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_matrix.c
--rw-r--r--   0 runner     (501) staff       (20)     4810 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_memory.c
--rw-r--r--   0 runner     (501) staff       (20)     6479 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c
--rw-r--r--   0 runner     (501) staff       (20)    20704 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nvector.c
--rw-r--r--   0 runner     (501) staff       (20)    13469 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c
--rw-r--r--   0 runner     (501) staff       (20)     3051 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_sycl.h
--rw-r--r--   0 runner     (501) staff       (20)     1592 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_version.c
--rw-r--r--   0 runner     (501) staff       (20)     6371 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_xbraid.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.181342 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/
--rw-r--r--   0 runner     (501) staff       (20)     1481 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.183154 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/
--rw-r--r--   0 runner     (501) staff       (20)     1798 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.184774 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1085 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     9961 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     7950 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2963 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c
--rw-r--r--   0 runner     (501) staff       (20)     1892 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h
--rw-r--r--   0 runner     (501) staff       (20)     7118 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.186797 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/
--rw-r--r--   0 runner     (501) staff       (20)     1844 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.188305 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1091 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     9982 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c
--rw-r--r--   0 runner     (501) staff       (20)     8001 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2978 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c
--rw-r--r--   0 runner     (501) staff       (20)     1930 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h
--rw-r--r--   0 runner     (501) staff       (20)     6580 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.190517 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.192061 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1053 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13106 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    13874 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     4522 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c
--rw-r--r--   0 runner     (501) staff       (20)     3046 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h
--rw-r--r--   0 runner     (501) staff       (20)    13160 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.194967 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/pcg/
--rw-r--r--   0 runner     (501) staff       (20)     1709 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    16843 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.197310 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spbcgs/
--rw-r--r--   0 runner     (501) staff       (20)     1743 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    22722 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.199295 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spfgmr/
--rw-r--r--   0 runner     (501) staff       (20)     1700 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    25504 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.201213 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spgmr/
--rw-r--r--   0 runner     (501) staff       (20)     1687 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    26697 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.203034 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/sptfqmr/
--rw-r--r--   0 runner     (501) staff       (20)     1713 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    28426 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.204335 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/
--rw-r--r--   0 runner     (501) staff       (20)     1085 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.205934 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/band/
--rw-r--r--   0 runner     (501) staff       (20)     1691 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13124 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.207649 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/dense/
--rw-r--r--   0 runner     (501) staff       (20)     1742 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     8906 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.209491 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/sparse/
--rw-r--r--   0 runner     (501) staff       (20)     1760 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    34432 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.210314 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/
--rw-r--r--   0 runner     (501) staff       (20)      842 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.213196 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/
--rw-r--r--   0 runner     (501) staff       (20)     1855 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.215306 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1064 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    12989 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    13798 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2718 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c
--rw-r--r--   0 runner     (501) staff       (20)     2126 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h
--rw-r--r--   0 runner     (501) staff       (20)    23849 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.217700 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/
--rw-r--r--   0 runner     (501) staff       (20)     1801 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.219433 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/
--rw-r--r--   0 runner     (501) staff       (20)     1039 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13234 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c
--rw-r--r--   0 runner     (501) staff       (20)    14015 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90
--rw-r--r--   0 runner     (501) staff       (20)     2672 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c
--rw-r--r--   0 runner     (501) staff       (20)     2051 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h
--rw-r--r--   0 runner     (501) staff       (20)    16132 2024-03-21 23:10:39.000000 PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.223435 PyPartMC-1.1.3/readme_fortran/
--rw-r--r--   0 runner     (501) staff       (20)     1437 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/aero_data.dat
--rw-r--r--   0 runner     (501) staff       (20)      320 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/aero_dist.dat
--rw-r--r--   0 runner     (501) staff       (20)       37 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/cooking_comp.dat
--rw-r--r--   0 runner     (501) staff       (20)       56 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/diesel_comp.dat
--rw-r--r--   0 runner     (501) staff       (20)     1223 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/readme_fortran/main.f90
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-03-21 23:11:07.276425 PyPartMC-1.1.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     6785 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.258376 PyPartMC-1.1.3/src/
--rw-r--r--   0 runner     (501) staff       (20)     7750 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     8585 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_data.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2474 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_dist.F90
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_dist.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7465 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_mode.F90
--rw-r--r--   0 runner     (501) staff       (20)     8728 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_mode.hpp
--rw-r--r--   0 runner     (501) staff       (20)    18162 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_particle.F90
--rw-r--r--   0 runner     (501) staff       (20)    13629 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_particle.hpp
--rw-r--r--   0 runner     (501) staff       (20)    22886 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_state.F90
--rw-r--r--   0 runner     (501) staff       (20)    17437 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/aero_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4355 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/bin_grid.F90
--rw-r--r--   0 runner     (501) staff       (20)     1984 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/bin_grid.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3337 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/bin_grid.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1104 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/camp_core.F90
--rw-r--r--   0 runner     (501) staff       (20)      807 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/camp_core.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2152 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/condense.F90
--rw-r--r--   0 runner     (501) staff       (20)     1073 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/condense.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1108 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/condense.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4543 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/env_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     3923 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/env_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2832 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/gas_data.F90
--rw-r--r--   0 runner     (501) staff       (20)     2936 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/gas_data.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3220 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/gas_state.F90
--rw-r--r--   0 runner     (501) staff       (20)     4102 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/gas_state.hpp
--rw-r--r--   0 runner     (501) staff       (20)      716 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/json_resource.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10279 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/json_resource.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3808 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/output.F90
--rw-r--r--   0 runner     (501) staff       (20)     1826 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/output.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1781 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/output.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/photolysis.F90
--rw-r--r--   0 runner     (501) staff       (20)      815 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/photolysis.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1127 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/pmc_resource.hpp
--rw-r--r--   0 runner     (501) staff       (20)    27377 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/pypartmc.cpp
--rw-r--r--   0 runner     (501) staff       (20)      955 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/rand.F90
--rw-r--r--   0 runner     (501) staff       (20)      699 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/rand.cpp
--rw-r--r--   0 runner     (501) staff       (20)      705 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/rand.hpp
--rw-r--r--   0 runner     (501) staff       (20)     9630 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/run_part.F90
--rw-r--r--   0 runner     (501) staff       (20)     3193 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/run_part.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2687 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/run_part.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5918 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/run_part_opt.F90
--rw-r--r--   0 runner     (501) staff       (20)     2466 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/run_part_opt.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6950 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/scenario.F90
--rw-r--r--   0 runner     (501) staff       (20)     1189 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/scenario.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7521 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/scenario.hpp
--rw-r--r--   0 runner     (501) staff       (20)     9937 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/spec_file_pypartmc.F90
--rw-r--r--   0 runner     (501) staff       (20)     6894 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/spec_file_pypartmc.cpp
--rw-r--r--   0 runner     (501) staff       (20)      782 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/sys.F90
--rw-r--r--   0 runner     (501) staff       (20)      711 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/sys.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1373 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/util.F90
--rw-r--r--   0 runner     (501) staff       (20)      988 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/util.cpp
--rw-r--r--   0 runner     (501) staff       (20)      971 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/src/util.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 23:11:07.272627 PyPartMC-1.1.3/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      672 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/common.py
--rw-r--r--   0 runner     (501) staff       (20)      111 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/conftest.py
--rw-r--r--   0 runner     (501) staff       (20)    14763 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_aero_data.py
--rw-r--r--   0 runner     (501) staff       (20)     6483 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_aero_dist.py
--rw-r--r--   0 runner     (501) staff       (20)     8661 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_aero_mode.py
--rw-r--r--   0 runner     (501) staff       (20)    19981 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_aero_particle.py
--rw-r--r--   0 runner     (501) staff       (20)    15532 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_aero_state.py
--rw-r--r--   0 runner     (501) staff       (20)     6061 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_bin_grid.py
--rw-r--r--   0 runner     (501) staff       (20)     2427 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_condense.py
--rw-r--r--   0 runner     (501) staff       (20)     1806 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_dtors.py
--rw-r--r--   0 runner     (501) staff       (20)     3021 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_env_state.py
--rw-r--r--   0 runner     (501) staff       (20)     2423 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_gas_data.py
--rw-r--r--   0 runner     (501) staff       (20)     3743 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_gas_state.py
--rw-r--r--   0 runner     (501) staff       (20)     2847 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_loss_rate.py
--rw-r--r--   0 runner     (501) staff       (20)     3762 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_output.py
--rw-r--r--   0 runner     (501) staff       (20)      986 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_rand.py
--rw-r--r--   0 runner     (501) staff       (20)     3916 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_run_part.py
--rw-r--r--   0 runner     (501) staff       (20)     2324 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_run_part_opt.py
--rw-r--r--   0 runner     (501) staff       (20)    11751 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_scenario.py
--rw-r--r--   0 runner     (501) staff       (20)     1062 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_units.py
--rw-r--r--   0 runner     (501) staff       (20)     1624 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_util.py
--rw-r--r--   0 runner     (501) staff       (20)     1024 2024-03-21 23:09:25.000000 PyPartMC-1.1.3/tests/test_version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.163160 PyPartMC-1.1.4/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.958567 PyPartMC-1.1.4/.binder/
+-rwxr-xr-x   0 runner     (501) staff       (20)       58 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.binder/postBuild
+-rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.binder/requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.949403 PyPartMC-1.1.4/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.960143 PyPartMC-1.1.4/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)      283 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/cancel.yml
+-rw-r--r--   0 runner     (501) staff       (20)      735 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/conda.yml
+-rw-r--r--   0 runner     (501) staff       (20)      278 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/cpplint.yml
+-rw-r--r--   0 runner     (501) staff       (20)      301 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/forlint.yml
+-rw-r--r--   0 runner     (501) staff       (20)      831 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/pdoc.yml
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner     (501) staff       (20)      939 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner     (501) staff       (20)     4430 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/readme_listings.yml
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/stale.yml
+-rw-r--r--   0 runner     (501) staff       (20)     8869 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.github/workflows/tests+pypi.yml
+-rw-r--r--   0 runner     (501) staff       (20)       18 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     1740 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)      455 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     1383 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/.zenodo.json
+-rw-r--r--   0 runner     (501) staff       (20)      836 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/CITATION.cff
+-rw-r--r--   0 runner     (501) staff       (20)    20001 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    11316 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    22094 2024-04-02 06:58:12.162839 PyPartMC-1.1.4/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.960285 PyPartMC-1.1.4/PyPartMC/
+-rw-r--r--   0 runner     (501) staff       (20)     2183 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/PyPartMC/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.162114 PyPartMC-1.1.4/PyPartMC.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    22094 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    37381 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       57 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       19 2024-04-02 06:58:11.000000 PyPartMC-1.1.4/PyPartMC.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)    21369 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.964384 PyPartMC-1.1.4/examples/
+-rw-r--r--   0 runner     (501) staff       (20)   205868 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/cloud_parcel.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)     2973 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/hello_world.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    18157 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/lognorm_ex.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   239412 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/mie_optical.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)  1128494 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/particle_simulation.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)  1681038 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/process_simulation_output.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    45354 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/terminal_velocities.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)     6243 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/examples/widgets_playground.ipynb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.953782 PyPartMC-1.1.4/gitmodules/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.964597 PyPartMC-1.1.4/gitmodules/SuiteSparse/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.949888 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.965431 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    17821 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Include/amd.h
+-rw-r--r--   0 runner     (501) staff       (20)     8238 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Include/amd_internal.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.970995 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    52625 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd.f
+-rw-r--r--   0 runner     (501) staff       (20)     5710 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_1.c
+-rw-r--r--   0 runner     (501) staff       (20)    64825 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_2.c
+-rw-r--r--   0 runner     (501) staff       (20)     4847 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_aat.c
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_control.c
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c
+-rw-r--r--   0 runner     (501) staff       (20)     5012 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_dump.c
+-rw-r--r--   0 runner     (501) staff       (20)      837 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_global.c
+-rw-r--r--   0 runner     (501) staff       (20)     4293 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_info.c
+-rw-r--r--   0 runner     (501) staff       (20)     6031 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_order.c
+-rw-r--r--   0 runner     (501) staff       (20)     3703 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c
+-rw-r--r--   0 runner     (501) staff       (20)     5509 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c
+-rw-r--r--   0 runner     (501) staff       (20)     3808 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c
+-rw-r--r--   0 runner     (501) staff       (20)     2980 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_valid.c
+-rw-r--r--   0 runner     (501) staff       (20)    52282 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amdbar.f
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.950053 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.972441 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    12382 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Include/btf.h
+-rw-r--r--   0 runner     (501) staff       (20)     1427 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Include/btf_internal.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.973315 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    15950 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_order.c
+-rw-r--r--   0 runner     (501) staff       (20)    24167 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.950299 PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.973978 PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Include/
+-rw-r--r--   0 runner     (501) staff       (20)     8361 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Include/colamd.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.974154 PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Source/
+-rw-r--r--   0 runner     (501) staff       (20)   107525 2024-04-02 06:57:25.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Source/colamd.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.950473 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.974890 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/
+-rw-r--r--   0 runner     (501) staff       (20)    29763 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu.h
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu_internal.h
+-rw-r--r--   0 runner     (501) staff       (20)    19461 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu_version.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.977261 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/
+-rw-r--r--   0 runner     (501) staff       (20)    24701 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu.c
+-rw-r--r--   0 runner     (501) staff       (20)    16732 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c
+-rw-r--r--   0 runner     (501) staff       (20)    11585 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c
+-rw-r--r--   0 runner     (501) staff       (20)     1923 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c
+-rw-r--r--   0 runner     (501) staff       (20)    16659 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c
+-rw-r--r--   0 runner     (501) staff       (20)     4560 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_dump.c
+-rw-r--r--   0 runner     (501) staff       (20)     8011 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_extract.c
+-rw-r--r--   0 runner     (501) staff       (20)    18700 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_factor.c
+-rw-r--r--   0 runner     (501) staff       (20)     1992 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c
+-rw-r--r--   0 runner     (501) staff       (20)      982 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c
+-rw-r--r--   0 runner     (501) staff       (20)    34162 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c
+-rw-r--r--   0 runner     (501) staff       (20)     7002 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_memory.c
+-rw-r--r--   0 runner     (501) staff       (20)    17034 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c
+-rw-r--r--   0 runner     (501) staff       (20)     4627 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_scale.c
+-rw-r--r--   0 runner     (501) staff       (20)    13209 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_solve.c
+-rw-r--r--   0 runner     (501) staff       (20)     4261 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_sort.c
+-rw-r--r--   0 runner     (501) staff       (20)    15641 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c
+-rw-r--r--   0 runner     (501) staff       (20)    51560 2024-04-02 06:57:26.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/LICENSE.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.977539 PyPartMC-1.1.4/gitmodules/SuiteSparse/SuiteSparse_config/
+-rw-r--r--   0 runner     (501) staff       (20)    16453 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
+-rw-r--r--   0 runner     (501) staff       (20)     7692 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.977815 PyPartMC-1.1.4/gitmodules/camp/
+-rw-r--r--   0 runner     (501) staff       (20)    28281 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1122 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/COPYING
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.984011 PyPartMC-1.1.4/gitmodules/camp/src/
+-rw-r--r--   0 runner     (501) staff       (20)     9605 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/Jacobian.c
+-rw-r--r--   0 runner     (501) staff       (20)     5319 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/Jacobian.h
+-rw-r--r--   0 runner     (501) staff       (20)    24549 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9949 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1311 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_solver.h
+-rw-r--r--   0 runner     (501) staff       (20)    29175 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14653 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23664 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2489 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.984611 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/
+-rw-r--r--   0 runner     (501) staff       (20)    48515 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90
+-rw-r--r--   0 runner     (501) staff       (20)    29575 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c
+-rw-r--r--   0 runner     (501) staff       (20)    27555 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18689 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c
+-rw-r--r--   0 runner     (501) staff       (20)     7067 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/aero_reps.h
+-rw-r--r--   0 runner     (501) staff       (20)    11196 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    67931 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_core.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8991 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_debug.h
+-rw-r--r--   0 runner     (501) staff       (20)    71748 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     3852 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_solver.h
+-rw-r--r--   0 runner     (501) staff       (20)    40570 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_solver_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5666 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/camp_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27287 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/chem_spec_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3018 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12725 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.c
+-rw-r--r--   0 runner     (501) staff       (20)      722 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.h
+-rw-r--r--   0 runner     (501) staff       (20)    14448 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14432 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/mechanism_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    53674 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/mpi.F90
+-rw-r--r--   0 runner     (501) staff       (20)    28496 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/property.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18982 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4783 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rand_gsl.c
+-rw-r--r--   0 runner     (501) staff       (20)    24970 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxn_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    19550 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxn_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    34236 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxn_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1741 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxn_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.990209 PyPartMC-1.1.4/gitmodules/camp/src/rxns/
+-rw-r--r--   0 runner     (501) staff       (20)    10318 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8481 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c
+-rw-r--r--   0 runner     (501) staff       (20)    11012 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8771 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c
+-rw-r--r--   0 runner     (501) staff       (20)    18534 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90
+-rw-r--r--   0 runner     (501) staff       (20)    21438 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c
+-rw-r--r--   0 runner     (501) staff       (20)    19588 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90
+-rw-r--r--   0 runner     (501) staff       (20)    33922 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c
+-rw-r--r--   0 runner     (501) staff       (20)    19694 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23125 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c
+-rw-r--r--   0 runner     (501) staff       (20)    10732 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_arrhenius.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8214 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_arrhenius.c
+-rw-r--r--   0 runner     (501) staff       (20)    19396 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90
+-rw-r--r--   0 runner     (501) staff       (20)    17290 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c
+-rw-r--r--   0 runner     (501) staff       (20)    23968 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18987 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.c
+-rw-r--r--   0 runner     (501) staff       (20)    12259 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_emission.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7225 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_emission.c
+-rw-r--r--   0 runner     (501) staff       (20)    12745 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_first_order_loss.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7978 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_first_order_loss.c
+-rw-r--r--   0 runner     (501) staff       (20)    16156 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10155 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_photolysis.c
+-rw-r--r--   0 runner     (501) staff       (20)    12152 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_surface.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16686 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_surface.c
+-rw-r--r--   0 runner     (501) staff       (20)    11433 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9118 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c
+-rw-r--r--   0 runner     (501) staff       (20)    10906 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_troe.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8616 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_troe.c
+-rw-r--r--   0 runner     (501) staff       (20)    12325 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10741 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c
+-rw-r--r--   0 runner     (501) staff       (20)     9518 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8366 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c
+-rw-r--r--   0 runner     (501) staff       (20)    14382 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wet_deposition.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8365 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wet_deposition.c
+-rw-r--r--   0 runner     (501) staff       (20)    24567 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/rxns.h
+-rw-r--r--   0 runner     (501) staff       (20)     5440 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/solver_stats.F90
+-rw-r--r--   0 runner     (501) staff       (20)    21468 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_model_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8903 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_model_factory.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20633 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_model_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     1390 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_model_solver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.991617 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/
+-rw-r--r--   0 runner     (501) staff       (20)    35354 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23405 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c
+-rw-r--r--   0 runner     (501) staff       (20)    31875 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90
+-rw-r--r--   0 runner     (501) staff       (20)    34859 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c
+-rw-r--r--   0 runner     (501) staff       (20)    29725 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90
+-rw-r--r--   0 runner     (501) staff       (20)    22008 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c
+-rw-r--r--   0 runner     (501) staff       (20)     4665 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/sub_models.h
+-rw-r--r--   0 runner     (501) staff       (20)     3081 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/time_derivative.c
+-rw-r--r--   0 runner     (501) staff       (20)     2734 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/time_derivative.h
+-rw-r--r--   0 runner     (501) staff       (20)    56058 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/util.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9473 2024-04-02 06:57:27.000000 PyPartMC-1.1.4/gitmodules/camp/src/util.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.991804 PyPartMC-1.1.4/gitmodules/json/
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/LICENSE.MIT
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.951259 PyPartMC-1.1.4/gitmodules/json/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.006742 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/
+-rw-r--r--   0 runner     (501) staff       (20)     2000 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/adl_serializer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3183 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.008785 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.009302 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/
+-rw-r--r--   0 runner     (501) staff       (20)    18439 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    38114 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    14612 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8820 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/exceptions.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3710 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/hash.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.010274 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/
+-rw-r--r--   0 runner     (501) staff       (20)    95726 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    17017 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    20782 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    54235 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/lexer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    18415 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/parser.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      605 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/position_t.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.011235 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/
+-rw-r--r--   0 runner     (501) staff       (20)      720 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    23112 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5838 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1404 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3509 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2918 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    32304 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/json_pointer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/json_ref.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    41851 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/macro_scope.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      749 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.012154 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.012529 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/call_std/
+-rw-r--r--   0 runner     (501) staff       (20)      143 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/call_std/begin.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      142 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/call_std/end.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4609 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1800 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/detected.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      174 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/identity_tag.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6609 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    22856 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      244 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/void_t.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.013103 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/
+-rw-r--r--   0 runner     (501) staff       (20)    69584 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3773 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    39511 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/serializer.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5697 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/string_concat.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1860 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/string_escape.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3098 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/value_t.hpp
+-rw-r--r--   0 runner     (501) staff       (20)   186996 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/json.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/json_fwd.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7469 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/ordered_map.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.951803 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.013557 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/hedley/
+-rw-r--r--   0 runner     (501) staff       (20)    86041 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5205 2024-04-02 06:57:38.000000 PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.991937 PyPartMC-1.1.4/gitmodules/json-fortran/
+-rw-r--r--   0 runner     (501) staff       (20)     2849 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.993844 PyPartMC-1.1.4/gitmodules/json-fortran/src/
+-rw-r--r--   0 runner     (501) staff       (20)   121590 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_file_module.F90
+-rw-r--r--   0 runner     (501) staff       (20)      842 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_scalar_by_path.inc
+-rw-r--r--   0 runner     (501) staff       (20)      767 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_vec_by_path.inc
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc
+-rw-r--r--   0 runner     (501) staff       (20)     4725 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_initialize_arguments.inc
+-rw-r--r--   0 runner     (501) staff       (20)      499 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_initialize_dummy_arguments.inc
+-rw-r--r--   0 runner     (501) staff       (20)     5759 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_kinds.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2480 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_macros.inc
+-rw-r--r--   0 runner     (501) staff       (20)     4027 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_module.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9238 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_parameters.F90
+-rw-r--r--   0 runner     (501) staff       (20)    31512 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_string_utilities.F90
+-rw-r--r--   0 runner     (501) staff       (20)   456578 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/json_value_module.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.005747 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.005893 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/introspection/
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90
+-rw-r--r--   0 runner     (501) staff       (20)    16922 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_01.F90
+-rw-r--r--   0 runner     (501) staff       (20)    14591 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_02.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4824 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_03.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5454 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_04.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3597 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_05.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4648 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_06.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_07.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_08.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4843 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_09.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11909 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_10.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_11.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8710 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_12.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2173 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_13.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4981 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_14.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8746 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_15.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7282 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_16.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5649 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_17.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3614 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_18.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5793 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_19.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7724 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_20.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2620 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_21.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2648 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_22.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8627 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_23.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6317 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_24.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4863 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_25.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2645 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_26.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2569 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_27.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3824 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_28.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5889 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_29.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2342 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_30.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4697 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_31.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3853 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_32.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_33.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5045 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_34.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_35.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4194 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_36.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_37.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4150 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_38.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2407 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_39.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_40.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3928 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_41.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4079 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_42.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2687 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_43.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3060 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_44.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4378 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_45.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12438 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_46.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4331 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_47.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2691 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_48.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1976 2024-04-02 06:57:40.000000 PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_49.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.015488 PyPartMC-1.1.4/gitmodules/netcdf-c/
+-rw-r--r--   0 runner     (501) staff       (20)    90875 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1452 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/COPYRIGHT
+-rw-r--r--   0 runner     (501) staff       (20)    18999 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/config.h.cmake.in
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.026437 PyPartMC-1.1.4/gitmodules/netcdf-c/include/
+-rw-r--r--   0 runner     (501) staff       (20)      643 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/fbits.h
+-rw-r--r--   0 runner     (501) staff       (20)     4907 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc.h
+-rw-r--r--   0 runner     (501) staff       (20)     5614 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc3dispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)     8982 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc3internal.h
+-rw-r--r--   0 runner     (501) staff       (20)     6820 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc4dispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)    23203 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc4internal.h
+-rw-r--r--   0 runner     (501) staff       (20)     1659 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)     2621 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc_provenance.h
+-rw-r--r--   0 runner     (501) staff       (20)     2062 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncauth.h
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncbytes.h
+-rw-r--r--   0 runner     (501) staff       (20)     3295 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncconfigure.h
+-rw-r--r--   0 runner     (501) staff       (20)      410 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nccrc.h
+-rw-r--r--   0 runner     (501) staff       (20)     7474 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncdispatch.h
+-rw-r--r--   0 runner     (501) staff       (20)      674 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncexternl.h
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nchashmap.h
+-rw-r--r--   0 runner     (501) staff       (20)     1906 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nchttp.h
+-rw-r--r--   0 runner     (501) staff       (20)     3226 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncindex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2254 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nclist.h
+-rw-r--r--   0 runner     (501) staff       (20)     1851 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/nclog.h
+-rw-r--r--   0 runner     (501) staff       (20)     1086 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncmodel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2215 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncoffsets.h
+-rw-r--r--   0 runner     (501) staff       (20)     8248 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncpathmgr.h
+-rw-r--r--   0 runner     (501) staff       (20)     3396 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncrc.h
+-rw-r--r--   0 runner     (501) staff       (20)     2079 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncs3sdk.h
+-rw-r--r--   0 runner     (501) staff       (20)     4264 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncuri.h
+-rw-r--r--   0 runner     (501) staff       (20)     1420 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncutf8.h
+-rw-r--r--   0 runner     (501) staff       (20)     1210 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncxml.h
+-rw-r--r--   0 runner     (501) staff       (20)    73732 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf.h
+-rw-r--r--   0 runner     (501) staff       (20)     4090 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_aux.h
+-rw-r--r--   0 runner     (501) staff       (20)    13091 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_dispatch.h.in
+-rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_f.h
+-rw-r--r--   0 runner     (501) staff       (20)     4065 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_filter.h
+-rw-r--r--   0 runner     (501) staff       (20)     1337 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_mem.h
+-rw-r--r--   0 runner     (501) staff       (20)     3835 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_meta.h.in
+-rw-r--r--   0 runner     (501) staff       (20)     1971 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/onstack.h
+-rw-r--r--   0 runner     (501) staff       (20)      569 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/include/rnd.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.045369 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/
+-rw-r--r--   0 runner     (501) staff       (20)     6128 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/datt.c
+-rw-r--r--   0 runner     (501) staff       (20)    23572 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattget.c
+-rw-r--r--   0 runner     (501) staff       (20)    13788 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattinq.c
+-rw-r--r--   0 runner     (501) staff       (20)    21685 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattput.c
+-rw-r--r--   0 runner     (501) staff       (20)    12111 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dauth.c
+-rw-r--r--   0 runner     (501) staff       (20)    27254 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/daux.c
+-rw-r--r--   0 runner     (501) staff       (20)    14827 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcompound.c
+-rw-r--r--   0 runner     (501) staff       (20)    21188 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcopy.c
+-rw-r--r--   0 runner     (501) staff       (20)    10910 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcrc64.c
+-rw-r--r--   0 runner     (501) staff       (20)    16745 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ddim.c
+-rw-r--r--   0 runner     (501) staff       (20)     3272 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ddispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)     5448 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/denum.c
+-rw-r--r--   0 runner     (501) staff       (20)    10328 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/derror.c
+-rw-r--r--   0 runner     (501) staff       (20)    75413 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dfile.c
+-rw-r--r--   0 runner     (501) staff       (20)    16459 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dfilter.c
+-rw-r--r--   0 runner     (501) staff       (20)     9601 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dgroup.c
+-rw-r--r--   0 runner     (501) staff       (20)    43874 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinfermodel.c
+-rw-r--r--   0 runner     (501) staff       (20)    16008 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinstance.c
+-rw-r--r--   0 runner     (501) staff       (20)    19387 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinstance_intern.c
+-rw-r--r--   0 runner     (501) staff       (20)     6562 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dmissing.c
+-rw-r--r--   0 runner     (501) staff       (20)    15177 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dnotnc4.c
+-rw-r--r--   0 runner     (501) staff       (20)    11901 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/doffsets.c
+-rw-r--r--   0 runner     (501) staff       (20)     2170 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dopaque.c
+-rw-r--r--   0 runner     (501) staff       (20)    32961 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dpathmgr.c
+-rw-r--r--   0 runner     (501) staff       (20)    32946 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/drc.c
+-rw-r--r--   0 runner     (501) staff       (20)     9341 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ds3util.c
+-rw-r--r--   0 runner     (501) staff       (20)     7588 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dstring.c
+-rw-r--r--   0 runner     (501) staff       (20)     5453 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dtype.c
+-rw-r--r--   0 runner     (501) staff       (20)     4527 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dutf8.c
+-rw-r--r--   0 runner     (501) staff       (20)    10862 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dutil.c
+-rw-r--r--   0 runner     (501) staff       (20)    52386 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvar.c
+-rw-r--r--   0 runner     (501) staff       (20)    41839 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarget.c
+-rw-r--r--   0 runner     (501) staff       (20)    22318 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarinq.c
+-rw-r--r--   0 runner     (501) staff       (20)    38016 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarput.c
+-rw-r--r--   0 runner     (501) staff       (20)     5687 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvlen.c
+-rw-r--r--   0 runner     (501) staff       (20)     4039 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nc.c
+-rw-r--r--   0 runner     (501) staff       (20)     4595 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ncbytes.c
+-rw-r--r--   0 runner     (501) staff       (20)   149230 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nchashmap.c
+-rw-r--r--   0 runner     (501) staff       (20)     6328 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclist.c
+-rw-r--r--   0 runner     (501) staff       (20)     6507 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclistmgr.c
+-rw-r--r--   0 runner     (501) staff       (20)     7281 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclog.c
+-rw-r--r--   0 runner     (501) staff       (20)    34144 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ncuri.c
+-rw-r--r--   0 runner     (501) staff       (20)    30569 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc.c
+-rw-r--r--   0 runner     (501) staff       (20)    29211 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc.h
+-rw-r--r--   0 runner     (501) staff       (20)  1621941 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc_data.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.050124 PyPartMC-1.1.4/gitmodules/netcdf-c/liblib/
+-rw-r--r--   0 runner     (501) staff       (20)     4004 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/liblib/nc_initialize.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.085772 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/
+-rw-r--r--   0 runner     (501) staff       (20)    22640 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/attr.m4
+-rw-r--r--   0 runner     (501) staff       (20)    10107 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/dim.c
+-rw-r--r--   0 runner     (501) staff       (20)    20016 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/memio.c
+-rw-r--r--   0 runner     (501) staff       (20)    12218 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/nc3dispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)    42563 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/nc3internal.c
+-rw-r--r--   0 runner     (501) staff       (20)     5804 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncio.c
+-rw-r--r--   0 runner     (501) staff       (20)     4986 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncio.h
+-rw-r--r--   0 runner     (501) staff       (20)    38570 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncx.h
+-rw-r--r--   0 runner     (501) staff       (20)    91027 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncx.m4
+-rw-r--r--   0 runner     (501) staff       (20)    45195 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/posixio.c
+-rw-r--r--   0 runner     (501) staff       (20)    56656 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/putget.m4
+-rw-r--r--   0 runner     (501) staff       (20)    34650 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/v1hpg.c
+-rw-r--r--   0 runner     (501) staff       (20)    17812 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/var.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.089244 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/
+-rw-r--r--   0 runner     (501) staff       (20)     6166 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4cache.c
+-rw-r--r--   0 runner     (501) staff       (20)     1933 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4dispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)    12192 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4grp.c
+-rw-r--r--   0 runner     (501) staff       (20)    60959 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4internal.c
+-rw-r--r--   0 runner     (501) staff       (20)    22718 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4type.c
+-rw-r--r--   0 runner     (501) staff       (20)    62575 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4var.c
+-rw-r--r--   0 runner     (501) staff       (20)    10546 2024-04-02 06:57:45.000000 PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/ncindex.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.089697 PyPartMC-1.1.4/gitmodules/netcdf-fortran/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.089948 PyPartMC-1.1.4/gitmodules/netcdf-fortran/CMakeExtras/
+-rw-r--r--   0 runner     (501) staff       (20)     2443 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     2417 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/COPYRIGHT
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.096472 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/
+-rwxr-xr-x   0 runner     (501) staff       (20)    35483 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    33291 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    17109 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    80960 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    15589 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    56443 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2732 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4.F90
+-rw-r--r--   0 runner     (501) staff       (20)    38904 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1899 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5233 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)    33491 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_func.F90
+-rw-r--r--   0 runner     (501) staff       (20)      789 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16715 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16718 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11047 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1719 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_dims.F90
+-rw-r--r--   0 runner     (501) staff       (20)   124466 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3537 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_externals.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5101 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6806 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23015 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3802 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_variables.F90
+-rw-r--r--   0 runner     (501) staff       (20)      959 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    20393 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_attio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    16094 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_control.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     6572 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_dim.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     8623 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_genatt.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     5086 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_geninq.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    10775 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_genvar.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)     7909 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_lib.c
+-rwxr-xr-x   0 runner     (501) staff       (20)     4428 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_misc.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    58343 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_nc4.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    23742 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_var1io.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    31119 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varaio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    38708 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varmio.F90
+-rwxr-xr-x   0 runner     (501) staff       (20)    37941 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varsio.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2601 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/typeSizes.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.096620 PyPartMC-1.1.4/gitmodules/optional/
+-rw-r--r--   0 runner     (501) staff       (20)     7048 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/optional/COPYING
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.952608 PyPartMC-1.1.4/gitmodules/optional/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.096812 PyPartMC-1.1.4/gitmodules/optional/include/tl/
+-rw-r--r--   0 runner     (501) staff       (20)    73584 2024-04-02 06:57:47.000000 PyPartMC-1.1.4/gitmodules/optional/include/tl/optional.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.097003 PyPartMC-1.1.4/gitmodules/partmc/
+-rw-r--r--   0 runner     (501) staff       (20)    18015 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/COPYING
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.108519 PyPartMC-1.1.4/gitmodules/partmc/src/
+-rw-r--r--   0 runner     (501) staff       (20)    18941 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_binned.F90
+-rw-r--r--   0 runner     (501) staff       (20)    37336 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    17040 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4584 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_info.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9722 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_info_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)    49450 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_mode.F90
+-rw-r--r--   0 runner     (501) staff       (20)    36702 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10615 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_particle_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23922 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_sorted.F90
+-rw-r--r--   0 runner     (501) staff       (20)   124072 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    13932 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_weight.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27073 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/aero_weight_array.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2924 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/bin_average_comp.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3825 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/bin_average_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20694 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/bin_grid.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7275 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/camp_interface.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8917 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/chamber.F90
+-rw-r--r--   0 runner     (501) staff       (20)    19523 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11888 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_additive.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7285 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4941 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown_cont.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5034 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown_free.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4927 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_constant.F90
+-rw-r--r--   0 runner     (501) staff       (20)    11095 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_sedi.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7469 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_zero.F90
+-rw-r--r--   0 runner     (501) staff       (20)    35666 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coagulation.F90
+-rw-r--r--   0 runner     (501) staff       (20)    34136 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/coagulation_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)    30923 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/condense.F90
+-rw-r--r--   0 runner     (501) staff       (20)     9565 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/condense_solver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2913 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/constants.F90
+-rw-r--r--   0 runner     (501) staff       (20)    20205 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4419 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/exact_soln.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3949 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_particles.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6528 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5072 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_time.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4227 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_env.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3867 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_gas.F90
+-rw-r--r--   0 runner     (501) staff       (20)     5692 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_sectional_aero_size.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4858 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/extract_sectional_aero_time.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23458 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/fractal.F90
+-rw-r--r--   0 runner     (501) staff       (20)    16247 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/gas_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)    22073 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/gas_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7566 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/getopt.F90
+-rw-r--r--   0 runner     (501) staff       (20)    15007 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/integer_rmap.F90
+-rw-r--r--   0 runner     (501) staff       (20)    19200 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/integer_rmap2.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8378 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/integer_varray.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18380 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/mosaic.F90
+-rw-r--r--   0 runner     (501) staff       (20)    47083 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/mpi.F90
+-rw-r--r--   0 runner     (501) staff       (20)    27550 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/netcdf.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8579 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/nucleate.F90
+-rw-r--r--   0 runner     (501) staff       (20)     7062 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/numeric_average.F90
+-rw-r--r--   0 runner     (501) staff       (20)    10911 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/numeric_diff.F90
+-rw-r--r--   0 runner     (501) staff       (20)    30038 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/output.F90
+-rw-r--r--   0 runner     (501) staff       (20)    48249 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/partmc.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8459 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)    18343 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4712 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/rand_gsl.c
+-rw-r--r--   0 runner     (501) staff       (20)     2837 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/run_exact.F90
+-rw-r--r--   0 runner     (501) staff       (20)    31148 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/run_part.F90
+-rw-r--r--   0 runner     (501) staff       (20)    12069 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/run_sect.F90
+-rw-r--r--   0 runner     (501) staff       (20)    47571 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/scenario.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1563 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/sort.c
+-rw-r--r--   0 runner     (501) staff       (20)    23797 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/spec_file.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3063 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/spec_line.F90
+-rw-r--r--   0 runner     (501) staff       (20)    23957 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/stats.F90
+-rw-r--r--   0 runner     (501) staff       (20)      482 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/sys.F90
+-rw-r--r--   0 runner     (501) staff       (20)    49504 2024-04-02 06:57:49.000000 PyPartMC-1.1.4/gitmodules/partmc/src/util.F90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.108875 PyPartMC-1.1.4/gitmodules/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    10999 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1684 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.952888 PyPartMC-1.1.4/gitmodules/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.112303 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    23883 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     7069 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    65224 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8458 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.113525 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    28078 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    49007 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5491 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    17971 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    23981 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)    44230 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     1513 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    31685 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)    10728 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     4731 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     4658 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     6923 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner     (501) staff       (20)     8851 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    78946 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9051 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   125304 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    80981 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.113690 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner     (501) staff       (20)     4185 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)    14535 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    27013 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.114221 PyPartMC-1.1.4/gitmodules/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)    10455 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    13460 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     7270 2024-04-02 06:57:51.000000 PyPartMC-1.1.4/gitmodules/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.953274 PyPartMC-1.1.4/gitmodules/pybind11_json/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.953319 PyPartMC-1.1.4/gitmodules/pybind11_json/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.114371 PyPartMC-1.1.4/gitmodules/pybind11_json/include/pybind11_json/
+-rw-r--r--   0 runner     (501) staff       (20)     7219 2024-04-02 06:57:52.000000 PyPartMC-1.1.4/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.114595 PyPartMC-1.1.4/gitmodules/span/
+-rw-r--r--   0 runner     (501) staff       (20)     1338 2024-04-02 06:57:53.000000 PyPartMC-1.1.4/gitmodules/span/LICENSE_1_0.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.953490 PyPartMC-1.1.4/gitmodules/span/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.114807 PyPartMC-1.1.4/gitmodules/span/include/tcb/
+-rw-r--r--   0 runner     (501) staff       (20)    18165 2024-04-02 06:57:53.000000 PyPartMC-1.1.4/gitmodules/span/include/tcb/span.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.114966 PyPartMC-1.1.4/gitmodules/string_view-standalone/
+-rw-r--r--   0 runner     (501) staff       (20)     1077 2024-04-02 06:57:53.000000 PyPartMC-1.1.4/gitmodules/string_view-standalone/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.953655 PyPartMC-1.1.4/gitmodules/string_view-standalone/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.115090 PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.115238 PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    29304 2024-04-02 06:57:53.000000 PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl
+-rw-r--r--   0 runner     (501) staff       (20)    20256 2024-04-02 06:57:53.000000 PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/string_view.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.115884 PyPartMC-1.1.4/gitmodules/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1576 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.116957 PyPartMC-1.1.4/gitmodules/sundials/cmake/
+-rw-r--r--   0 runner     (501) staff       (20)     2962 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsIndexSize.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    10395 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     4883 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsSetupConfig.cmake
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.954380 PyPartMC-1.1.4/gitmodules/sundials/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.118527 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/
+-rw-r--r--   0 runner     (501) staff       (20)     9544 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode.h
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_bandpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_bbdpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     1790 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_diag.h
+-rw-r--r--   0 runner     (501) staff       (20)     2035 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_direct.h
+-rw-r--r--   0 runner     (501) staff       (20)    10422 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_hypamgpre.h
+-rw-r--r--   0 runner     (501) staff       (20)     6515 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_ls.h
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_proj.h
+-rw-r--r--   0 runner     (501) staff       (20)     2873 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_spils.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.120615 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/
+-rw-r--r--   0 runner     (501) staff       (20)     9721 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_cuda.h
+-rw-r--r--   0 runner     (501) staff       (20)     9653 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_hip.h
+-rw-r--r--   0 runner     (501) staff       (20)     8671 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_manyvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     9959 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     1644 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_mpiplusx.h
+-rw-r--r--   0 runner     (501) staff       (20)     9487 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_openmp.h
+-rw-r--r--   0 runner     (501) staff       (20)     9612 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_openmpdev.h
+-rw-r--r--   0 runner     (501) staff       (20)    10795 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_parallel.h
+-rw-r--r--   0 runner     (501) staff       (20)     9697 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_parhyp.h
+-rw-r--r--   0 runner     (501) staff       (20)     9419 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_petsc.h
+-rw-r--r--   0 runner     (501) staff       (20)    11042 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_pthreads.h
+-rw-r--r--   0 runner     (501) staff       (20)     8267 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_raja.h
+-rw-r--r--   0 runner     (501) staff       (20)     8934 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_serial.h
+-rw-r--r--   0 runner     (501) staff       (20)    10053 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_sycl.h
+-rw-r--r--   0 runner     (501) staff       (20)     5824 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_trilinos.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.120940 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/trilinos/
+-rw-r--r--   0 runner     (501) staff       (20)     1819 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    23964 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.124426 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     7791 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     5329 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_config.in
+-rw-r--r--   0 runner     (501) staff       (20)     5520 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8997 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)    13330 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_direct.h
+-rw-r--r--   0 runner     (501) staff       (20)     1690 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_fconfig.in
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_fnvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     1128 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_futils.h
+-rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    10283 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_iterative.h
+-rw-r--r--   0 runner     (501) staff       (20)    10707 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_lapack.h
+-rw-r--r--   0 runner     (501) staff       (20)     9633 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     7839 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_math.h
+-rw-r--r--   0 runner     (501) staff       (20)     5466 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_matrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     4527 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_memory.h
+-rw-r--r--   0 runner     (501) staff       (20)     1399 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_mpi_types.h
+-rw-r--r--   0 runner     (501) staff       (20)     9190 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    12719 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nvector.h
+-rw-r--r--   0 runner     (501) staff       (20)     4744 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     4567 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5165 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_types.h
+-rw-r--r--   0 runner     (501) staff       (20)     1266 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_version.h
+-rw-r--r--   0 runner     (501) staff       (20)     4024 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_xbraid.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.126448 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     2649 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     4768 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h
+-rw-r--r--   0 runner     (501) staff       (20)     2983 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5603 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h
+-rw-r--r--   0 runner     (501) staff       (20)     3142 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h
+-rw-r--r--   0 runner     (501) staff       (20)     3171 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h
+-rw-r--r--   0 runner     (501) staff       (20)     2751 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h
+-rw-r--r--   0 runner     (501) staff       (20)     3052 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h
+-rw-r--r--   0 runner     (501) staff       (20)     4553 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h
+-rw-r--r--   0 runner     (501) staff       (20)     4872 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     5237 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h
+-rw-r--r--   0 runner     (501) staff       (20)     4533 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.127574 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/
+-rw-r--r--   0 runner     (501) staff       (20)     4552 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     5233 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h
+-rw-r--r--   0 runner     (501) staff       (20)     3647 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5083 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h
+-rw-r--r--   0 runner     (501) staff       (20)     5776 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h
+-rw-r--r--   0 runner     (501) staff       (20)     3245 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h
+-rw-r--r--   0 runner     (501) staff       (20)     5136 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.128066 PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     6202 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h
+-rw-r--r--   0 runner     (501) staff       (20)     5449 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h
+-rw-r--r--   0 runner     (501) staff       (20)     4071 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:11.956038 PyPartMC-1.1.4/gitmodules/sundials/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.131795 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/
+-rw-r--r--   0 runner     (501) staff       (20)     1972 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/CHANGES
+-rw-r--r--   0 runner     (501) staff       (20)     3549 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1576 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1166 2024-04-02 06:58:01.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/NOTICE
+-rw-r--r--   0 runner     (501) staff       (20)     2708 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/README.md
+-rw-r--r--   0 runner     (501) staff       (20)   135753 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode.c
+-rw-r--r--   0 runner     (501) staff       (20)    18212 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bandpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2383 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    22668 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bbdpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2621 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    13629 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_diag.c
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_diag_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1956 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_direct.c
+-rw-r--r--   0 runner     (501) staff       (20)    14722 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5554 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_fused_stubs.c
+-rw-r--r--   0 runner     (501) staff       (20)    14959 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_hypamgpre.c
+-rw-r--r--   0 runner     (501) staff       (20)     2766 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    29404 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    28172 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_io.c
+-rw-r--r--   0 runner     (501) staff       (20)    58312 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_ls.c
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_ls_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    12911 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_nls.c
+-rw-r--r--   0 runner     (501) staff       (20)    12603 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_proj.c
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_proj_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_spils.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.134618 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/
+-rw-r--r--   0 runner     (501) staff       (20)     1734 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     4616 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/Makefile.in
+-rw-r--r--   0 runner     (501) staff       (20)     3464 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvband.c
+-rw-r--r--   0 runner     (501) staff       (20)     4950 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c
+-rw-r--r--   0 runner     (501) staff       (20)    22548 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h
+-rw-r--r--   0 runner     (501) staff       (20)     2063 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbp.c
+-rw-r--r--   0 runner     (501) staff       (20)    14934 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbp.h
+-rw-r--r--   0 runner     (501) staff       (20)     2952 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvdense.c
+-rw-r--r--   0 runner     (501) staff       (20)     2046 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvewt.c
+-rw-r--r--   0 runner     (501) staff       (20)     3904 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c
+-rw-r--r--   0 runner     (501) staff       (20)     1370 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c
+-rw-r--r--   0 runner     (501) staff       (20)     1344 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c
+-rw-r--r--   0 runner     (501) staff       (20)     1502 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c
+-rw-r--r--   0 runner     (501) staff       (20)    15564 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvode.c
+-rw-r--r--   0 runner     (501) staff       (20)    49120 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvode.h
+-rw-r--r--   0 runner     (501) staff       (20)     4190 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c
+-rw-r--r--   0 runner     (501) staff       (20)     2399 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvroot.c
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvroot.h
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.135120 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1483 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    43017 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    83166 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.135328 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/
+-rw-r--r--   0 runner     (501) staff       (20)     1562 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.135822 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.136248 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)      979 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    25549 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    40279 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     3740 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fnvector_serial.c
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fnvector_serial.h
+-rw-r--r--   0 runner     (501) staff       (20)    47581 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/nvector_serial.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.138936 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/
+-rw-r--r--   0 runner     (501) staff       (20)     3022 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.140725 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1109 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     7228 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     2922 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    13682 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    19932 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     9392 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     9541 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    11515 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    12797 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)    24749 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    42038 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     6561 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)      957 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     6784 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_band.c
+-rw-r--r--   0 runner     (501) staff       (20)     3712 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_cuda.h
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh
+-rw-r--r--   0 runner     (501) staff       (20)     1403 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_debug.h
+-rw-r--r--   0 runner     (501) staff       (20)     9098 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_dense.c
+-rw-r--r--   0 runner     (501) staff       (20)     6468 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_direct.c
+-rw-r--r--   0 runner     (501) staff       (20)      964 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_futils.c
+-rw-r--r--   0 runner     (501) staff       (20)     2500 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_hip.h
+-rw-r--r--   0 runner     (501) staff       (20)     7260 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8008 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_iterative.c
+-rw-r--r--   0 runner     (501) staff       (20)     5667 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_linearsolver.c
+-rw-r--r--   0 runner     (501) staff       (20)     2956 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_math.c
+-rw-r--r--   0 runner     (501) staff       (20)     4633 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_matrix.c
+-rw-r--r--   0 runner     (501) staff       (20)     4810 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_memory.c
+-rw-r--r--   0 runner     (501) staff       (20)     6479 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c
+-rw-r--r--   0 runner     (501) staff       (20)    20704 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nvector.c
+-rw-r--r--   0 runner     (501) staff       (20)    13469 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c
+-rw-r--r--   0 runner     (501) staff       (20)     3051 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_sycl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_version.c
+-rw-r--r--   0 runner     (501) staff       (20)     6371 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_xbraid.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.140869 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)     1481 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.141568 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/
+-rw-r--r--   0 runner     (501) staff       (20)     1798 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.142281 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     9961 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     7950 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2963 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c
+-rw-r--r--   0 runner     (501) staff       (20)     1892 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h
+-rw-r--r--   0 runner     (501) staff       (20)     7118 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.143004 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/
+-rw-r--r--   0 runner     (501) staff       (20)     1844 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.143513 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     9982 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)     8001 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2978 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c
+-rw-r--r--   0 runner     (501) staff       (20)     1930 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h
+-rw-r--r--   0 runner     (501) staff       (20)     6580 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.144130 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.144577 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1053 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13106 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    13874 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     4522 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c
+-rw-r--r--   0 runner     (501) staff       (20)     3046 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h
+-rw-r--r--   0 runner     (501) staff       (20)    13160 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.144885 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/pcg/
+-rw-r--r--   0 runner     (501) staff       (20)     1709 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    16843 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.145191 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spbcgs/
+-rw-r--r--   0 runner     (501) staff       (20)     1743 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    22722 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.145545 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spfgmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1700 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    25504 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.145851 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spgmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1687 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    26697 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.146143 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/sptfqmr/
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    28426 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.146418 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.146755 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/band/
+-rw-r--r--   0 runner     (501) staff       (20)     1691 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13124 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.147122 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/dense/
+-rw-r--r--   0 runner     (501) staff       (20)     1742 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     8906 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.147419 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/sparse/
+-rw-r--r--   0 runner     (501) staff       (20)     1760 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    34432 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.147618 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/
+-rw-r--r--   0 runner     (501) staff       (20)      842 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.148484 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.148934 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1064 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    12989 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    13798 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2718 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c
+-rw-r--r--   0 runner     (501) staff       (20)     2126 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h
+-rw-r--r--   0 runner     (501) staff       (20)    23849 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.149618 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.150055 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/
+-rw-r--r--   0 runner     (501) staff       (20)     1039 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13234 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c
+-rw-r--r--   0 runner     (501) staff       (20)    14015 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90
+-rw-r--r--   0 runner     (501) staff       (20)     2672 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c
+-rw-r--r--   0 runner     (501) staff       (20)     2051 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h
+-rw-r--r--   0 runner     (501) staff       (20)    16132 2024-04-02 06:58:02.000000 PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.151286 PyPartMC-1.1.4/readme_fortran/
+-rw-r--r--   0 runner     (501) staff       (20)     1437 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/aero_data.dat
+-rw-r--r--   0 runner     (501) staff       (20)      320 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/aero_dist.dat
+-rw-r--r--   0 runner     (501) staff       (20)       37 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/cooking_comp.dat
+-rw-r--r--   0 runner     (501) staff       (20)       56 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/diesel_comp.dat
+-rw-r--r--   0 runner     (501) staff       (20)     1223 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/readme_fortran/main.f90
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-02 06:58:12.163205 PyPartMC-1.1.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     6785 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.158720 PyPartMC-1.1.4/src/
+-rw-r--r--   0 runner     (501) staff       (20)     7750 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8585 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_data.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2474 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_dist.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_dist.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7465 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_mode.F90
+-rw-r--r--   0 runner     (501) staff       (20)     8728 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_mode.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    18162 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_particle.F90
+-rw-r--r--   0 runner     (501) staff       (20)    13629 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_particle.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    22886 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)    17437 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/aero_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4355 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/bin_grid.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/bin_grid.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3337 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/bin_grid.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1104 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/camp_core.F90
+-rw-r--r--   0 runner     (501) staff       (20)      807 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/camp_core.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2152 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/condense.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1073 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/condense.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/condense.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4543 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/env_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3923 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/env_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2832 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/gas_data.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2936 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/gas_data.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3220 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/gas_state.F90
+-rw-r--r--   0 runner     (501) staff       (20)     4102 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/gas_state.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      716 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/json_resource.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10279 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/json_resource.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3808 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/output.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1826 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/output.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/output.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1070 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/photolysis.F90
+-rw-r--r--   0 runner     (501) staff       (20)      815 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/photolysis.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1127 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/pmc_resource.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    27377 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/pypartmc.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      955 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/rand.F90
+-rw-r--r--   0 runner     (501) staff       (20)      699 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/rand.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      705 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/rand.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     9630 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/run_part.F90
+-rw-r--r--   0 runner     (501) staff       (20)     3193 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/run_part.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2687 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/run_part.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5918 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/run_part_opt.F90
+-rw-r--r--   0 runner     (501) staff       (20)     2466 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/run_part_opt.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6950 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/scenario.F90
+-rw-r--r--   0 runner     (501) staff       (20)     1189 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/scenario.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7521 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/scenario.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     9937 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/spec_file_pypartmc.F90
+-rw-r--r--   0 runner     (501) staff       (20)     6894 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/spec_file_pypartmc.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      782 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/sys.F90
+-rw-r--r--   0 runner     (501) staff       (20)      711 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/sys.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1373 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/util.F90
+-rw-r--r--   0 runner     (501) staff       (20)      988 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/util.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      971 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/src/util.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-02 06:58:12.161898 PyPartMC-1.1.4/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      672 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/common.py
+-rw-r--r--   0 runner     (501) staff       (20)      111 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/conftest.py
+-rw-r--r--   0 runner     (501) staff       (20)    14763 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_aero_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     6483 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_aero_dist.py
+-rw-r--r--   0 runner     (501) staff       (20)     8661 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_aero_mode.py
+-rw-r--r--   0 runner     (501) staff       (20)    19981 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_aero_particle.py
+-rw-r--r--   0 runner     (501) staff       (20)    15532 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_aero_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     6061 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_bin_grid.py
+-rw-r--r--   0 runner     (501) staff       (20)     2427 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_condense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1806 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_dtors.py
+-rw-r--r--   0 runner     (501) staff       (20)     3021 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_env_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_gas_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     3743 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_gas_state.py
+-rw-r--r--   0 runner     (501) staff       (20)     2847 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_loss_rate.py
+-rw-r--r--   0 runner     (501) staff       (20)     3762 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_output.py
+-rw-r--r--   0 runner     (501) staff       (20)      986 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_rand.py
+-rw-r--r--   0 runner     (501) staff       (20)     3916 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_run_part.py
+-rw-r--r--   0 runner     (501) staff       (20)     2324 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_run_part_opt.py
+-rw-r--r--   0 runner     (501) staff       (20)    11751 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_scenario.py
+-rw-r--r--   0 runner     (501) staff       (20)     1062 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_units.py
+-rw-r--r--   0 runner     (501) staff       (20)     1624 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_util.py
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2024-04-02 06:57:04.000000 PyPartMC-1.1.4/tests/test_version.py
```

### Comparing `PyPartMC-1.1.3/.github/workflows/conda.yml` & `PyPartMC-1.1.4/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/.github/workflows/pdoc.yml` & `PyPartMC-1.1.4/.github/workflows/pdoc.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/.github/workflows/pylint.yml` & `PyPartMC-1.1.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/.github/workflows/readme_listings.yml` & `PyPartMC-1.1.4/.github/workflows/readme_listings.yml`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,17 @@
   fortran:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: recursive
 
-      - run: sudo apt-get install libnetcdff-dev
+      - run: |
+          sudo apt-get update
+          sudo apt-get install libnetcdff-dev
       - run: |
           cd readme_fortran
           mkdir build
           cd build
           PARTMC_HOME=../../gitmodules/partmc cmake ..
           make
```

### Comparing `PyPartMC-1.1.3/.github/workflows/stale.yml` & `PyPartMC-1.1.4/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/.github/workflows/tests+pypi.yml` & `PyPartMC-1.1.4/.github/workflows/tests+pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -126,18 +126,22 @@
 
       - if: matrix.python-version != 'system'
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - if: matrix.python-version == 'system'
-        run: sudo ln -s `which python3` /usr/local/bin/python
+        run: |
+          sudo ln -s `which python3` /usr/local/bin/python
+          echo PIP_INSTALL_OPTS=--break-system-packages >> $GITHUB_ENV
+
+      - if: matrix.python-version != 'system'
+        run: python -m pip install --upgrade pip==22.1.2
 
-      - run: python -m pip install --upgrade pip==22.1.2
-      - run: pip install "build<1.1" wheel
+      - run: python -m pip install $PIP_INSTALL_OPTS "build<1.1" wheel
       - run: cmake --version
       - run: |
           unset CI
           python -m build 2>&1 | tee build.log
           exit `fgrep -i warning build.log | grep -v "WARNING setuptools_scm" | wc -l`
 
       - if: startsWith(matrix.platform, 'macos-') && matrix.python-version == '3.11'
@@ -179,31 +183,31 @@
         with:
           name: dist
           path: dist
 
       - env:
           SYSTEM_VERSION_COMPAT: 0 
         run: |
-          pip debug --verbose
-          for i in dist/*.whl; do pip install $i[tests]; done;
-          pip show --verbose PyPartMC
+          python -m pip debug --verbose
+          for i in dist/*.whl; do python -m pip install $PIP_INSTALL_OPTS $i[tests]; done;
+          python -m pip show --verbose PyPartMC
 
       ### make sure PyPartMC is not picked up from a local folder
       - run: |
           cd tests
           python -c "import PyPartMC"
-          pytest --durations=10 -v -s -We -p no:unraisableexception .
+          python -m pytest --durations=10 -v -s -We -p no:unraisableexception .
           cd ..
 
       - if: matrix.python-version != '3.7'
         run: |
-          pip install -r gitmodules/devops_tests/requirements.txt
+          python -m pip install $PIP_INSTALL_OPTS -r gitmodules/devops_tests/requirements.txt
           ex -sc 'g/^PyPartMC/d' -cx .binder/requirements.txt
-          pip install -r .binder/requirements.txt
-          GITHUB_TOKEN=${{ secrets.GITHUB_TOKEN }} pytest --durations=10 -v -s -We -p no:unraisableexception gitmodules/devops_tests
+          python -m pip install $PIP_INSTALL_OPTS -r .binder/requirements.txt
+          GITHUB_TOKEN=${{ secrets.GITHUB_TOKEN }} python -m pytest --durations=10 -v -s -We -p no:unraisableexception gitmodules/devops_tests
 
 ### uncomment to gain ssh access in case of failure
 #      - if: ${{ failure() }}
 #        uses: mxschmitt/action-tmate@v3
 #        with:
 #          limit-access-to-actor: true
```

### Comparing `PyPartMC-1.1.3/.gitmodules` & `PyPartMC-1.1.4/.gitmodules`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/.zenodo.json` & `PyPartMC-1.1.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/CITATION.cff` & `PyPartMC-1.1.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/CMakeLists.txt` & `PyPartMC-1.1.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/LICENSE` & `PyPartMC-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/MANIFEST.in` & `PyPartMC-1.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/PKG-INFO` & `PyPartMC-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,21 @@
-Metadata-Version: 2.1
-Name: PyPartMC
-Version: 1.1.3
-Summary: Python interface to PartMC
-Author: PyPartMC team (see https://github.com/open-atmos/PyPartMC/graphs/contributors)
-Author-email: nriemer@illinois.edu
-License: GPL-3.0
-Project-URL: Tracker, https://github.com/open-atmos/PyPartMC/issues
-Project-URL: Documentation, https://open-atmos.github.io/PyPartMC
-Project-URL: Source, https://github.com/open-atmos/PyPartMC/
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-order; extra == "tests"
-Requires-Dist: fastcore!=1.5.8; extra == "tests"
-Requires-Dist: ghapi; extra == "tests"
-
 ![logo](https://raw.githubusercontent.com/wiki/open-atmos/PyPartMC/logo.svg)
 
 # PyPartMC
 
 PyPartMC is a Python interface to [PartMC](https://lagrange.mechse.illinois.edu/partmc/), 
   a particle-resolved Monte-Carlo code for atmospheric aerosol simulation.
 PyPartMC is implemented in C++ and it also constitutes a C++ API to the PartMC Fortran internals.
 The Python API can facilitate using PartMC from other environments - see, e.g., Julia and Matlab examples below.
 
 For an outline of the project, rationale, architecture, and features, refer to: [D'Aquino et al., 2024 (SoftwareX)](https://doi.org/10.1016/j.softx.2023.101613) (please cite if PyPartMC is used in your research).
 For a list of talks and other relevant resources, please see [project Wiki](https://github.com/open-atmos/PyPartMC/wiki/).
 
-[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/)
+[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/) [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
+   
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=UIUC&)](https://atmos.illinois.edu/)
 [![Github Actions Build Status](https://github.com/open-atmos/PyPartMC/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyPartMC/actions)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyPartMC/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7662635.svg)](https://doi.org/10.5281/zenodo.7662635)
 [![PyPI version](https://badge.fury.io/py/PyPartMC.svg)](https://pypi.org/p/PyPartMC)
 
@@ -297,14 +278,20 @@
         spec_file_pypartmc_f --> spec_file_pypartmc_c["SpecFile-C"]
     end
 
     style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
 ```
 
 ## FAQ
+- Q: How to install PyPartMC with MOSAIC enabled?    
+  A: Installation can be done using `pip`, however, `pip` needs to be instructed not to use binary packages available at pypi.org but rather to compile from source (pip will download the source from pip.org), and the path to compiled MOSAIC library needs to be provided at compile-time; the following command should convey it:
+```bash
+MOSAIC_HOME=<<PATH_TO_MOSAIC_LIB>> pip install --force-reinstall --no-binary=PyPartMC PyPartMC
+```
+
 - Q: Why `pip install PyPartMC` triggers compilation on my brand new Apple machine, while it quickly downloads and installs binary packages when executed on older Macs, Windows or Linux?    
   A: We are not yet providing binary wheels on PyPI for Apple-silicon (arm64) machines. Cross-compilation with gfortran is only supported with experimental unofficial builds [and is tricky](https://github.com/iains/gcc-12-branch/issues/23), while Github Actions ARM64 virtual machines are [costly](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions#minute-multipliers).  
 
 - Q: Why some of the constructors expect data to be passed as **lists of single-entry dictionaries** instead of multi-element dictionaries?    
   A: This is intentional and related with PartMC relying on the order of elements within spec-file input; while Python dictionaries preserve ordering (insertion order), JSON format does not, and we intend to make these data structures safe to be [de]serialized using JSON.   
 
 - Q: How to check the version of PartMC that PyPartMC was compiled against?    
@@ -345,15 +332,15 @@
 PyPartMC codebase benefits from Pylint, Black and isort code analysis (which are all part of the CI workflows where we also use pre-commit hooks. The pre-commit hooks can be run locally, and then the resultant changes need to be staged before committing. To set up the hooks locally, install pre-commit via `pip install pre-commit` and set up the git hooks via `pre-commit install` (this needs to be done every time you clone the project). To run all pre-commit hooks, run `pre-commit run --all-files`. The `.pre-commit-config.yaml` file can be modified in case new hooks are to be added or existing ones need to be altered.
 
 ## Credits
 
 #### PyPartMC:
 
 authors: [PyPartMC developers](https://github.com/open-atmos/PyPartMC/graphs/contributors)   
-funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/)   
+funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/), [Polish National Science Centre](https://ncn.gov.pl/en)   
 copyright: [University of Illinois at Urbana-Champaign](https://atmos.illinois.edu/)   
 licence: [GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 #### PartMC:
 authors: [Nicole Riemer](https://www.atmos.uiuc.edu/~nriemer/), [Matthew West](https://lagrange.mechse.illinois.edu/mwest/), [Jeff Curtis](https://publish.illinois.edu/jcurtis2/) et al.   
 licence: [GPL v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) or later
```

### Comparing `PyPartMC-1.1.3/PyPartMC/__init__.py` & `PyPartMC-1.1.4/PyPartMC/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/PyPartMC.egg-info/PKG-INFO` & `PyPartMC-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPartMC
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python interface to PartMC
 Author: PyPartMC team (see https://github.com/open-atmos/PyPartMC/graphs/contributors)
 Author-email: nriemer@illinois.edu
 License: GPL-3.0
 Project-URL: Tracker, https://github.com/open-atmos/PyPartMC/issues
 Project-URL: Documentation, https://open-atmos.github.io/PyPartMC
 Project-URL: Source, https://github.com/open-atmos/PyPartMC/
@@ -26,15 +26,16 @@
   a particle-resolved Monte-Carlo code for atmospheric aerosol simulation.
 PyPartMC is implemented in C++ and it also constitutes a C++ API to the PartMC Fortran internals.
 The Python API can facilitate using PartMC from other environments - see, e.g., Julia and Matlab examples below.
 
 For an outline of the project, rationale, architecture, and features, refer to: [D'Aquino et al., 2024 (SoftwareX)](https://doi.org/10.1016/j.softx.2023.101613) (please cite if PyPartMC is used in your research).
 For a list of talks and other relevant resources, please see [project Wiki](https://github.com/open-atmos/PyPartMC/wiki/).
 
-[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/)
+[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/) [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
+   
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=UIUC&)](https://atmos.illinois.edu/)
 [![Github Actions Build Status](https://github.com/open-atmos/PyPartMC/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyPartMC/actions)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyPartMC/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7662635.svg)](https://doi.org/10.5281/zenodo.7662635)
 [![PyPI version](https://badge.fury.io/py/PyPartMC.svg)](https://pypi.org/p/PyPartMC)
 
@@ -297,14 +298,20 @@
         spec_file_pypartmc_f --> spec_file_pypartmc_c["SpecFile-C"]
     end
 
     style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
 ```
 
 ## FAQ
+- Q: How to install PyPartMC with MOSAIC enabled?    
+  A: Installation can be done using `pip`, however, `pip` needs to be instructed not to use binary packages available at pypi.org but rather to compile from source (pip will download the source from pip.org), and the path to compiled MOSAIC library needs to be provided at compile-time; the following command should convey it:
+```bash
+MOSAIC_HOME=<<PATH_TO_MOSAIC_LIB>> pip install --force-reinstall --no-binary=PyPartMC PyPartMC
+```
+
 - Q: Why `pip install PyPartMC` triggers compilation on my brand new Apple machine, while it quickly downloads and installs binary packages when executed on older Macs, Windows or Linux?    
   A: We are not yet providing binary wheels on PyPI for Apple-silicon (arm64) machines. Cross-compilation with gfortran is only supported with experimental unofficial builds [and is tricky](https://github.com/iains/gcc-12-branch/issues/23), while Github Actions ARM64 virtual machines are [costly](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions#minute-multipliers).  
 
 - Q: Why some of the constructors expect data to be passed as **lists of single-entry dictionaries** instead of multi-element dictionaries?    
   A: This is intentional and related with PartMC relying on the order of elements within spec-file input; while Python dictionaries preserve ordering (insertion order), JSON format does not, and we intend to make these data structures safe to be [de]serialized using JSON.   
 
 - Q: How to check the version of PartMC that PyPartMC was compiled against?    
@@ -345,15 +352,15 @@
 PyPartMC codebase benefits from Pylint, Black and isort code analysis (which are all part of the CI workflows where we also use pre-commit hooks. The pre-commit hooks can be run locally, and then the resultant changes need to be staged before committing. To set up the hooks locally, install pre-commit via `pip install pre-commit` and set up the git hooks via `pre-commit install` (this needs to be done every time you clone the project). To run all pre-commit hooks, run `pre-commit run --all-files`. The `.pre-commit-config.yaml` file can be modified in case new hooks are to be added or existing ones need to be altered.
 
 ## Credits
 
 #### PyPartMC:
 
 authors: [PyPartMC developers](https://github.com/open-atmos/PyPartMC/graphs/contributors)   
-funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/)   
+funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/), [Polish National Science Centre](https://ncn.gov.pl/en)   
 copyright: [University of Illinois at Urbana-Champaign](https://atmos.illinois.edu/)   
 licence: [GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 #### PartMC:
 authors: [Nicole Riemer](https://www.atmos.uiuc.edu/~nriemer/), [Matthew West](https://lagrange.mechse.illinois.edu/mwest/), [Jeff Curtis](https://publish.illinois.edu/jcurtis2/) et al.   
 licence: [GPL v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) or later
```

### Comparing `PyPartMC-1.1.3/PyPartMC.egg-info/SOURCES.txt` & `PyPartMC-1.1.4/PyPartMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/README.md` & `PyPartMC-1.1.4/PyPartMC.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,41 @@
+Metadata-Version: 2.1
+Name: PyPartMC
+Version: 1.1.4
+Summary: Python interface to PartMC
+Author: PyPartMC team (see https://github.com/open-atmos/PyPartMC/graphs/contributors)
+Author-email: nriemer@illinois.edu
+License: GPL-3.0
+Project-URL: Tracker, https://github.com/open-atmos/PyPartMC/issues
+Project-URL: Documentation, https://open-atmos.github.io/PyPartMC
+Project-URL: Source, https://github.com/open-atmos/PyPartMC/
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-order; extra == "tests"
+Requires-Dist: fastcore!=1.5.8; extra == "tests"
+Requires-Dist: ghapi; extra == "tests"
+
 ![logo](https://raw.githubusercontent.com/wiki/open-atmos/PyPartMC/logo.svg)
 
 # PyPartMC
 
 PyPartMC is a Python interface to [PartMC](https://lagrange.mechse.illinois.edu/partmc/), 
   a particle-resolved Monte-Carlo code for atmospheric aerosol simulation.
 PyPartMC is implemented in C++ and it also constitutes a C++ API to the PartMC Fortran internals.
 The Python API can facilitate using PartMC from other environments - see, e.g., Julia and Matlab examples below.
 
 For an outline of the project, rationale, architecture, and features, refer to: [D'Aquino et al., 2024 (SoftwareX)](https://doi.org/10.1016/j.softx.2023.101613) (please cite if PyPartMC is used in your research).
 For a list of talks and other relevant resources, please see [project Wiki](https://github.com/open-atmos/PyPartMC/wiki/).
 
-[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/)
+[![US Funding](https://img.shields.io/static/v1?label=US%20DOE%20Funding%20by&color=267c32&message=ASR&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAQCAMAAAA25D/gAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAASFBMVEVOTXyyIjRDQnNZWINZWITtzdFUU4BVVIFVVYHWiZM9PG/KZnNXVoJaWYT67/FKSXhgX4hgX4lcW4VbWoX03uHQeIN2VXj///9pZChlAAAAAWJLR0QXC9aYjwAAAAd0SU1FB+EICRMGJV+KCCQAAABdSURBVBjThdBJDoAgEETRkkkZBBX0/kd11QTTpH1/STqpAAwWBkobSlkGbt0o5xmEfqxDZJB2Q6XMoBwnVSbTylWp0hi42rmbwTOYPDfR5Kc+07IIUQQvghX9THsBHcES8/SiF0kAAAAldEVYdGRhdGU6Y3JlYXRlADIwMTctMDgtMDlUMTk6MDY6MzcrMDA6MDCX1tBgAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDE3LTA4LTA5VDE5OjA2OjM3KzAwOjAw5oto3AAAAABJRU5ErkJggg==)](https://asr.science.energy.gov/) [![PL Funding](https://img.shields.io/static/v1?label=PL%20Funding%20by&color=d21132&message=NCN&logoWidth=25&logo=image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAANCAYAAACpUE5eAAAABmJLR0QA/wD/AP+gvaeTAAAAKUlEQVQ4jWP8////fwYqAiZqGjZqIHUAy4dJS6lqIOMdEZvRZDPcDQQAb3cIaY1Sbi4AAAAASUVORK5CYII=)](https://www.ncn.gov.pl/?language=en)
+   
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Copyright](https://img.shields.io/static/v1?label=Copyright&color=249fe2&message=UIUC&)](https://atmos.illinois.edu/)
 [![Github Actions Build Status](https://github.com/open-atmos/PyPartMC/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyPartMC/actions)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyPartMC/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7662635.svg)](https://doi.org/10.5281/zenodo.7662635)
 [![PyPI version](https://badge.fury.io/py/PyPartMC.svg)](https://pypi.org/p/PyPartMC)
 
@@ -277,14 +298,20 @@
         spec_file_pypartmc_f --> spec_file_pypartmc_c["SpecFile-C"]
     end
 
     style PartMC fill:#7ae7ff,stroke-width:2px,color:#2B2B2B
 ```
 
 ## FAQ
+- Q: How to install PyPartMC with MOSAIC enabled?    
+  A: Installation can be done using `pip`, however, `pip` needs to be instructed not to use binary packages available at pypi.org but rather to compile from source (pip will download the source from pip.org), and the path to compiled MOSAIC library needs to be provided at compile-time; the following command should convey it:
+```bash
+MOSAIC_HOME=<<PATH_TO_MOSAIC_LIB>> pip install --force-reinstall --no-binary=PyPartMC PyPartMC
+```
+
 - Q: Why `pip install PyPartMC` triggers compilation on my brand new Apple machine, while it quickly downloads and installs binary packages when executed on older Macs, Windows or Linux?    
   A: We are not yet providing binary wheels on PyPI for Apple-silicon (arm64) machines. Cross-compilation with gfortran is only supported with experimental unofficial builds [and is tricky](https://github.com/iains/gcc-12-branch/issues/23), while Github Actions ARM64 virtual machines are [costly](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions#minute-multipliers).  
 
 - Q: Why some of the constructors expect data to be passed as **lists of single-entry dictionaries** instead of multi-element dictionaries?    
   A: This is intentional and related with PartMC relying on the order of elements within spec-file input; while Python dictionaries preserve ordering (insertion order), JSON format does not, and we intend to make these data structures safe to be [de]serialized using JSON.   
 
 - Q: How to check the version of PartMC that PyPartMC was compiled against?    
@@ -325,15 +352,15 @@
 PyPartMC codebase benefits from Pylint, Black and isort code analysis (which are all part of the CI workflows where we also use pre-commit hooks. The pre-commit hooks can be run locally, and then the resultant changes need to be staged before committing. To set up the hooks locally, install pre-commit via `pip install pre-commit` and set up the git hooks via `pre-commit install` (this needs to be done every time you clone the project). To run all pre-commit hooks, run `pre-commit run --all-files`. The `.pre-commit-config.yaml` file can be modified in case new hooks are to be added or existing ones need to be altered.
 
 ## Credits
 
 #### PyPartMC:
 
 authors: [PyPartMC developers](https://github.com/open-atmos/PyPartMC/graphs/contributors)   
-funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/)   
+funding: [US Department of Energy Atmospheric System Research programme](https://asr.science.energy.gov/), [Polish National Science Centre](https://ncn.gov.pl/en)   
 copyright: [University of Illinois at Urbana-Champaign](https://atmos.illinois.edu/)   
 licence: [GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 #### PartMC:
 authors: [Nicole Riemer](https://www.atmos.uiuc.edu/~nriemer/), [Matthew West](https://lagrange.mechse.illinois.edu/mwest/), [Jeff Curtis](https://publish.illinois.edu/jcurtis2/) et al.   
 licence: [GPL v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) or later
```

### Comparing `PyPartMC-1.1.3/examples/cloud_parcel.ipynb` & `PyPartMC-1.1.4/examples/cloud_parcel.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/hello_world.ipynb` & `PyPartMC-1.1.4/examples/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/lognorm_ex.ipynb` & `PyPartMC-1.1.4/examples/lognorm_ex.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/mie_optical.ipynb` & `PyPartMC-1.1.4/examples/mie_optical.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/particle_simulation.ipynb` & `PyPartMC-1.1.4/examples/particle_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/process_simulation_output.ipynb` & `PyPartMC-1.1.4/examples/process_simulation_output.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/terminal_velocities.ipynb` & `PyPartMC-1.1.4/examples/terminal_velocities.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/examples/widgets_playground.ipynb` & `PyPartMC-1.1.4/examples/widgets_playground.ipynb`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Include/amd.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Include/amd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Include/amd_internal.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd.f` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd.f`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_1.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_1.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_2.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_aat.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_aat.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_control.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_control.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_dump.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_dump.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_global.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_global.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_info.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_info.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_order.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_order.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amd_valid.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amd_valid.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/AMD/Source/amdbar.f` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/AMD/Source/amdbar.f`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Include/btf.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Include/btf.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Include/btf_internal.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Include/btf_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_maxtrans.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_order.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_order.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/BTF/Source/btf_strongcomp.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Include/colamd.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Include/colamd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/COLAMD/Source/colamd.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/COLAMD/Source/colamd.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu_internal.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu_internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Include/klu_version.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Include/klu_version.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_analyze.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_analyze_given.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_defaults.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_diagnostics.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_dump.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_dump.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_extract.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_extract.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_factor.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_factor.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_free_numeric.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_free_symbolic.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_kernel.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_memory.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_memory.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_refactor.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_scale.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_scale.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_solve.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_solve.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_sort.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_sort.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/KLU/Source/klu_tsolve.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/LICENSE.txt` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h` & `PyPartMC-1.1.4/gitmodules/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/camp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/COPYING` & `PyPartMC-1.1.4/gitmodules/camp/COPYING`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/Jacobian.c` & `PyPartMC-1.1.4/gitmodules/camp/src/Jacobian.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/Jacobian.h` & `PyPartMC-1.1.4/gitmodules/camp/src/Jacobian.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_solver.c` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_phase_solver.h` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_phase_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_factory.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_solver.c` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_rep_solver.h` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_rep_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_modal_binned_mass.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_single_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_reps/aero_rep_single_particle.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/aero_reps.h` & `PyPartMC-1.1.4/gitmodules/camp/src/aero_reps.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_common.h` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_common.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_core.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_core.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_debug.h` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_debug.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_solver.c` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_solver.h` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_solver_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_solver_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/camp_state.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/camp_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/chem_spec_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/chem_spec_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/constants.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/constants.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.c` & `PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/debug_diff_check.h` & `PyPartMC-1.1.4/gitmodules/camp/src/debug_diff_check.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/env_state.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/mechanism_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/mechanism_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/mpi.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/mpi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/property.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/property.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rand.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rand_gsl.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rand_gsl.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxn_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxn_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxn_factory.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxn_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxn_solver.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxn_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxn_solver.h` & `PyPartMC-1.1.4/gitmodules/camp/src/rxn_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_H2O2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_CMAQ_OH_HNO3.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_HL_phase_transfer.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_SIMPOL_phase_transfer.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_aqueous_equilibrium.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_arrhenius.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_arrhenius.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_arrhenius.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_arrhenius.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_arrhenius.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_condensed_phase_photolysis.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_emission.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_emission.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_emission.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_emission.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_first_order_loss.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_first_order_loss.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_first_order_loss.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_first_order_loss.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_photolysis.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_photolysis.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_photolysis.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_surface.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_surface.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_surface.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_surface.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_ternary_chemical_activation.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_troe.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_troe.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_troe.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_troe.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_no_ro2.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wennberg_tunneling.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wet_deposition.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wet_deposition.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns/rxn_wet_deposition.c` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns/rxn_wet_deposition.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/rxns.h` & `PyPartMC-1.1.4/gitmodules/camp/src/rxns.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/solver_stats.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/solver_stats.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_model_data.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_model_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_model_factory.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_model_factory.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_model_solver.c` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_model_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_model_solver.h` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_model_solver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_PDFiTE.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_PDFiTE.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_UNIFAC.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_UNIFAC.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models/sub_model_ZSR_aerosol_water.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/sub_models.h` & `PyPartMC-1.1.4/gitmodules/camp/src/sub_models.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/time_derivative.c` & `PyPartMC-1.1.4/gitmodules/camp/src/time_derivative.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/time_derivative.h` & `PyPartMC-1.1.4/gitmodules/camp/src/time_derivative.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/util.F90` & `PyPartMC-1.1.4/gitmodules/camp/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/camp/src/util.h` & `PyPartMC-1.1.4/gitmodules/camp/src/util.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/LICENSE.MIT` & `PyPartMC-1.1.4/gitmodules/json/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/adl_serializer.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/adl_serializer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/byte_container_with_subtype.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/from_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/to_chars.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/conversions/to_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/exceptions.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/hash.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/hash.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/binary_reader.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/input_adapters.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/json_sax.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/lexer.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/lexer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/parser.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/parser.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/input/position_t.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/input/position_t.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/internal_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iter_impl.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iteration_proxy.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/iterator_traits.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/iterators/primitive_iterator.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/json_pointer.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/json_pointer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/json_ref.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/json_ref.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/macro_scope.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/macro_scope.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/macro_unscope.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/cpp_future.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/detected.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/detected.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/is_sax.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/meta/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/binary_writer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/output_adapters.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/output/serializer.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/output/serializer.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/string_concat.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/string_concat.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/string_escape.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/string_escape.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/detail/value_t.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/detail/value_t.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/json.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/json_fwd.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/json_fwd.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/ordered_map.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/ordered_map.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp` & `PyPartMC-1.1.4/gitmodules/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/LICENSE` & `PyPartMC-1.1.4/gitmodules/json-fortran/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_file_module.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_file_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_scalar_by_path.inc` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_scalar_by_path.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_vec_by_path.inc` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_vec_by_path.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_get_vec_by_path_alloc.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_initialize_arguments.inc` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_initialize_arguments.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_kinds.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_kinds.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_macros.inc` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_macros.inc`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_module.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_parameters.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_parameters.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_string_utilities.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_string_utilities.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/json_value_module.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/json_value_module.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/introspection/test_iso_10646_support.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_01.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_01.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_02.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_02.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_03.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_03.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_04.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_04.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_05.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_05.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_06.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_06.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_07.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_07.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_08.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_08.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_09.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_09.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_10.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_10.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_11.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_11.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_12.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_12.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_13.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_13.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_14.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_14.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_15.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_15.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_16.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_16.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_17.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_17.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_18.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_18.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_19.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_19.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_20.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_20.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_21.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_21.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_22.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_22.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_23.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_23.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_24.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_24.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_25.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_25.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_26.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_26.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_27.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_27.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_28.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_28.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_29.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_29.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_30.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_30.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_31.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_31.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_32.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_32.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_33.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_33.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_34.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_34.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_35.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_35.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_36.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_36.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_37.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_37.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_38.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_38.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_39.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_39.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_40.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_40.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_41.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_41.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_42.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_42.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_43.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_43.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_44.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_44.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_45.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_45.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_46.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_46.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_47.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_47.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_48.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_48.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/json-fortran/src/tests/jf_test_49.F90` & `PyPartMC-1.1.4/gitmodules/json-fortran/src/tests/jf_test_49.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/netcdf-c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/COPYRIGHT` & `PyPartMC-1.1.4/gitmodules/netcdf-c/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/config.h.cmake.in` & `PyPartMC-1.1.4/gitmodules/netcdf-c/config.h.cmake.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/fbits.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/fbits.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc3dispatch.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc3dispatch.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc3internal.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc3internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc4dispatch.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc4dispatch.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc4internal.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc4internal.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc_logging.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc_logging.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nc_provenance.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nc_provenance.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncauth.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncauth.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncbytes.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncbytes.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncconfigure.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncconfigure.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncdispatch.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncdispatch.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncexternl.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncexternl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nchashmap.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nchashmap.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nchttp.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nchttp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncindex.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncindex.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nclist.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nclist.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/nclog.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/nclog.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncmodel.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncmodel.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncoffsets.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncoffsets.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncpathmgr.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncpathmgr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncrc.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncrc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncs3sdk.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncs3sdk.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncuri.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncuri.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncutf8.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncutf8.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/ncxml.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/ncxml.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_aux.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_aux.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_dispatch.h.in` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_dispatch.h.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_f.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_f.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_filter.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_filter.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_mem.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_mem.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/netcdf_meta.h.in` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/netcdf_meta.h.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/onstack.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/onstack.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/include/rnd.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/include/rnd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/datt.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/datt.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattget.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattget.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattinq.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattinq.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dattput.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dattput.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dauth.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dauth.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/daux.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/daux.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcompound.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcompound.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcopy.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcopy.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dcrc64.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dcrc64.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ddim.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ddim.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ddispatch.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ddispatch.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/denum.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/denum.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/derror.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/derror.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dfile.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dfile.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dfilter.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dfilter.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dgroup.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dgroup.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinfermodel.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinfermodel.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinstance.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinstance.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dinstance_intern.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dinstance_intern.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dmissing.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dmissing.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dnotnc4.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dnotnc4.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/doffsets.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/doffsets.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dopaque.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dopaque.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dpathmgr.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dpathmgr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/drc.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/drc.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ds3util.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ds3util.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dstring.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dstring.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dtype.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dtype.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dutf8.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dutf8.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dutil.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dutil.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvar.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvar.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarget.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarget.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarinq.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarinq.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvarput.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvarput.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/dvlen.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/dvlen.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nc.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nc.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ncbytes.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ncbytes.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nchashmap.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nchashmap.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclist.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclist.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclistmgr.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclistmgr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/nclog.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/nclog.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/ncuri.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/ncuri.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libdispatch/utf8proc_data.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libdispatch/utf8proc_data.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/liblib/nc_initialize.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/liblib/nc_initialize.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/attr.m4` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/attr.m4`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/dim.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/dim.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/memio.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/memio.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/nc3dispatch.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/nc3dispatch.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/nc3internal.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/nc3internal.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncio.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncio.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncio.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncio.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncx.h` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncx.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/ncx.m4` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/ncx.m4`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/posixio.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/posixio.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/putget.m4` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/putget.m4`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/v1hpg.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/v1hpg.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc/var.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc/var.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4cache.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4cache.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4dispatch.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4dispatch.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4grp.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4grp.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4internal.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4internal.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4type.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4type.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/nc4var.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/nc4var.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-c/libsrc4/ncindex.c` & `PyPartMC-1.1.4/gitmodules/netcdf-c/libsrc4/ncindex.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/CMakeExtras/MatchNetCDFFortranTypes.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/COPYRIGHT` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf4_nc_interfaces.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf4_nf_interfaces.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nc_interfaces.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/module_netcdf_nf_interfaces.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_eightbyte.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_externals.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_file.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_file.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_func.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_func.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_overloads.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_variables.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf4_visibility.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_attributes.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_constants.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_constants.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_dims.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_dims.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_expanded.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_externals.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_externals.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_file.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_file.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_overloads.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_text_variables.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_variables.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_variables.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/netcdf_visibility.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_attio.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_attio.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_control.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_control.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_dim.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_dim.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_genatt.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_genatt.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_geninq.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_geninq.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_genvar.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_genvar.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_lib.c` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_lib.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_misc.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_misc.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_nc4.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_nc4.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_nc_noparallel.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_var1io.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_var1io.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varaio.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varaio.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varmio.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varmio.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/nf_varsio.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/nf_varsio.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/netcdf-fortran/fortran/typeSizes.F90` & `PyPartMC-1.1.4/gitmodules/netcdf-fortran/fortran/typeSizes.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/optional/COPYING` & `PyPartMC-1.1.4/gitmodules/optional/COPYING`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/optional/include/tl/optional.hpp` & `PyPartMC-1.1.4/gitmodules/optional/include/tl/optional.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/COPYING` & `PyPartMC-1.1.4/gitmodules/partmc/COPYING`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_binned.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_binned.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_data.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_dist.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_info.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_info.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_info_array.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_info_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_mode.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_mode.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_particle.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_particle_array.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_particle_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_sorted.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_sorted.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_state.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_weight.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_weight.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/aero_weight_array.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/aero_weight_array.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/bin_average_comp.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/bin_average_comp.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/bin_average_size.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/bin_average_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/bin_grid.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/bin_grid.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/camp_interface.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/camp_interface.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/chamber.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/chamber.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_additive.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_additive.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown_cont.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown_cont.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_brown_free.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_brown_free.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_constant.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_constant.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_sedi.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_sedi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coag_kernel_zero.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coag_kernel_zero.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coagulation.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coagulation.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/coagulation_dist.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/coagulation_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/condense.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/condense.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/condense_solver.c` & `PyPartMC-1.1.4/gitmodules/partmc/src/condense_solver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/constants.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/constants.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/env_state.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/exact_soln.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/exact_soln.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_particles.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_particles.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_size.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_aero_time.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_aero_time.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_env.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_env.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_gas.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_gas.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_sectional_aero_size.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_sectional_aero_size.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/extract_sectional_aero_time.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/extract_sectional_aero_time.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/fractal.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/fractal.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/gas_data.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/gas_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/gas_state.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/gas_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/getopt.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/getopt.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/integer_rmap.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/integer_rmap.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/integer_rmap2.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/integer_rmap2.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/integer_varray.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/integer_varray.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/mosaic.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/mosaic.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/mpi.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/mpi.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/netcdf.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/netcdf.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/nucleate.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/nucleate.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/numeric_average.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/numeric_average.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/numeric_diff.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/numeric_diff.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/output.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/output.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/partmc.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/partmc.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/photolysis.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/rand.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/rand_gsl.c` & `PyPartMC-1.1.4/gitmodules/partmc/src/rand_gsl.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/run_exact.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/run_exact.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/run_part.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/run_part.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/run_sect.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/run_sect.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/scenario.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/scenario.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/sort.c` & `PyPartMC-1.1.4/gitmodules/partmc/src/sort.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/spec_file.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/spec_file.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/spec_line.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/spec_line.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/stats.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/stats.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/partmc/src/util.F90` & `PyPartMC-1.1.4/gitmodules/partmc/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/LICENSE` & `PyPartMC-1.1.4/gitmodules/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/attr.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/buffer_info.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/cast.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/chrono.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/complex.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/class.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/common.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/descr.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/init.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/internals.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/detail/typeid.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/eigen.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/embed.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/eval.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/functional.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/gil.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/iostream.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/numpy.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/operators.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/options.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/pybind11.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/pytypes.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl/filesystem.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/include/pybind11/stl_bind.h` & `PyPartMC-1.1.4/gitmodules/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/tools/FindPythonLibsNew.cmake` & `PyPartMC-1.1.4/gitmodules/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/tools/pybind11Common.cmake` & `PyPartMC-1.1.4/gitmodules/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11/tools/pybind11Tools.cmake` & `PyPartMC-1.1.4/gitmodules/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp` & `PyPartMC-1.1.4/gitmodules/pybind11_json/include/pybind11_json/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/span/LICENSE_1_0.txt` & `PyPartMC-1.1.4/gitmodules/span/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/span/include/tcb/span.hpp` & `PyPartMC-1.1.4/gitmodules/span/include/tcb/span.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/string_view-standalone/LICENSE` & `PyPartMC-1.1.4/gitmodules/string_view-standalone/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl` & `PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/detail/string_view.inl`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/string_view-standalone/include/bpstd/string_view.hpp` & `PyPartMC-1.1.4/gitmodules/string_view-standalone/include/bpstd/string_view.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/LICENSE` & `PyPartMC-1.1.4/gitmodules/sundials/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsIndexSize.cmake` & `PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsIndexSize.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake` & `PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsSetupCompilers.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/cmake/SundialsSetupConfig.cmake` & `PyPartMC-1.1.4/gitmodules/sundials/cmake/SundialsSetupConfig.cmake`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_bandpre.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_bandpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_bbdpre.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_bbdpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_diag.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_diag.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_direct.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_direct.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_hypamgpre.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_hypamgpre.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_ls.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_ls.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_proj.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_proj.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/cvode/cvode_spils.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/cvode/cvode_spils.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_cuda.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_cuda.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_hip.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_hip.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_manyvector.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_manyvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_mpimanyvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_mpiplusx.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_mpiplusx.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_openmp.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_openmp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_openmpdev.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_openmpdev.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_parallel.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_parallel.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_parhyp.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_parhyp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_petsc.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_petsc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_pthreads.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_pthreads.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_raja.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_raja.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_serial.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_sycl.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_sycl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/nvector_trilinos.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/nvector_trilinos.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorInterface.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/include/nvector/trilinos/SundialsTpetraVectorKernels.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_band.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_config.in` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_config.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_cuda_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_dense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_direct.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_fconfig.in` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_fconfig.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_fnvector.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_futils.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_futils.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_hip_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_iterative.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_lapack.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_linearsolver.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_math.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_matrix.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_memory.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_memory.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_mpi_types.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_mpi_types.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nvector.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_nvector_senswrapper.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_sycl_policies.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_types.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_version.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sundials/sundials_xbraid.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sundials/sundials_xbraid.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_cusolversp_batchqr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackband.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_lapackdense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_magmadense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_onemkldense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_pcg.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spbcgs.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spfgmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_spgmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_superludist.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunlinsol/sunlinsol_superlumt.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_cusparse.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_magmadense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_onemkldense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_slunrloc.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunmatrix/sunmatrix_sparse.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_newton.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h` & `PyPartMC-1.1.4/gitmodules/sundials/include/sunnonlinsol/sunnonlinsol_petscsnes.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/CHANGES` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/CHANGES`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/LICENSE` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/NOTICE` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/NOTICE`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/README.md` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/README.md`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bandpre.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bandpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bbdpre.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bbdpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_diag.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_diag.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_diag_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_diag_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_direct.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_direct.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_fused_gpu.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_fused_stubs.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_fused_stubs.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_hypamgpre.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_hypamgpre.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_hypamgpre_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_io.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_io.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_ls.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_ls.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_ls_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_ls_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_nls.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_nls.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_proj.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_proj.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_proj_impl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_proj_impl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/cvode_spils.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/cvode_spils.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/Makefile.in` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/Makefile.in`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvband.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvband.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbbd.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbbd.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbp.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbp.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvbp.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvbp.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvdense.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvdense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvewt.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvewt.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvjtimes.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnulllinsol.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnullmatrix.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvnullnonlinsol.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvode.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvode.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvode.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvode.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvpreco.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvroot.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvroot.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvroot.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvroot.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fcmix/fcvsparse.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/fcvode_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/cvode/fmod/fcvode_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fmod/fnvector_serial_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fnvector_serial.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/fnvector_serial.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/nvector/serial/nvector_serial.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/nvector/serial/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_futils_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_linearsolver_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_matrix_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nonlinearsolver_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_nvector_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/fmod/fsundials_types_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_band.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_cuda.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_cuda.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_cuda_kernels.cuh`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_debug.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_debug.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_dense.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_direct.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_futils.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_futils.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_hip.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_hip.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_hip_kernels.hip.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_iterative.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_linearsolver.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_linearsolver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_math.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_math.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_matrix.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_matrix.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_memory.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_memory.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nonlinearsolver.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nvector.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_nvector_senswrapper.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_sycl.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_sycl.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_version.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_version.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sundials/sundials_xbraid.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sundials/sundials_xbraid.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fmod/fsunlinsol_band_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/fsunlinsol_band.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/band/sunlinsol_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fmod/fsunlinsol_dense_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/fsunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/dense/sunlinsol_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fmod/fsunlinsol_klu_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/fsunlinsol_klu.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/klu/sunlinsol_klu.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/pcg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/pcg/sunlinsol_pcg.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spbcgs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spbcgs/sunlinsol_spbcgs.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spfgmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spfgmr/sunlinsol_spfgmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spgmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/spgmr/sunlinsol_spgmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/sptfqmr/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunlinsol/sptfqmr/sunlinsol_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/band/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/band/sunmatrix_band.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/dense/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/dense/sunmatrix_dense.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/sparse/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunmatrix/sparse/sunmatrix_sparse.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fmod/fsunnonlinsol_fixedpoint_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/fsunnonlinsol_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/fixedpoint/sunnonlinsol_fixedpoint.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fmod/fsunnonlinsol_newton_mod.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/fsunnonlinsol_newton.h`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c` & `PyPartMC-1.1.4/gitmodules/sundials/src/sunnonlinsol/newton/sunnonlinsol_newton.c`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/readme_fortran/CMakeLists.txt` & `PyPartMC-1.1.4/readme_fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/readme_fortran/main.f90` & `PyPartMC-1.1.4/readme_fortran/main.f90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/setup.py` & `PyPartMC-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_data.F90` & `PyPartMC-1.1.4/src/aero_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_data.hpp` & `PyPartMC-1.1.4/src/aero_data.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_dist.F90` & `PyPartMC-1.1.4/src/aero_dist.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_dist.hpp` & `PyPartMC-1.1.4/src/aero_dist.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_mode.F90` & `PyPartMC-1.1.4/src/aero_mode.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_mode.hpp` & `PyPartMC-1.1.4/src/aero_mode.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_particle.F90` & `PyPartMC-1.1.4/src/aero_particle.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_particle.hpp` & `PyPartMC-1.1.4/src/aero_particle.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_state.F90` & `PyPartMC-1.1.4/src/aero_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/aero_state.hpp` & `PyPartMC-1.1.4/src/aero_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/bin_grid.F90` & `PyPartMC-1.1.4/src/bin_grid.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/bin_grid.cpp` & `PyPartMC-1.1.4/src/bin_grid.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/bin_grid.hpp` & `PyPartMC-1.1.4/src/bin_grid.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/camp_core.F90` & `PyPartMC-1.1.4/src/camp_core.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/camp_core.hpp` & `PyPartMC-1.1.4/src/camp_core.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/condense.F90` & `PyPartMC-1.1.4/src/condense.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/condense.cpp` & `PyPartMC-1.1.4/src/condense.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/condense.hpp` & `PyPartMC-1.1.4/src/condense.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/env_state.F90` & `PyPartMC-1.1.4/src/env_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/env_state.hpp` & `PyPartMC-1.1.4/src/env_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/gas_data.F90` & `PyPartMC-1.1.4/src/gas_data.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/gas_data.hpp` & `PyPartMC-1.1.4/src/gas_data.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/gas_state.F90` & `PyPartMC-1.1.4/src/gas_state.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/gas_state.hpp` & `PyPartMC-1.1.4/src/gas_state.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/json_resource.cpp` & `PyPartMC-1.1.4/src/json_resource.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/json_resource.hpp` & `PyPartMC-1.1.4/src/json_resource.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/output.F90` & `PyPartMC-1.1.4/src/output.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/output.cpp` & `PyPartMC-1.1.4/src/output.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/output.hpp` & `PyPartMC-1.1.4/src/output.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/photolysis.F90` & `PyPartMC-1.1.4/src/photolysis.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/photolysis.hpp` & `PyPartMC-1.1.4/src/photolysis.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/pmc_resource.hpp` & `PyPartMC-1.1.4/src/pmc_resource.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/pypartmc.cpp` & `PyPartMC-1.1.4/src/pypartmc.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/rand.F90` & `PyPartMC-1.1.4/src/rand.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/rand.cpp` & `PyPartMC-1.1.4/src/rand.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/rand.hpp` & `PyPartMC-1.1.4/src/rand.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/run_part.F90` & `PyPartMC-1.1.4/src/run_part.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/run_part.cpp` & `PyPartMC-1.1.4/src/run_part.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/run_part.hpp` & `PyPartMC-1.1.4/src/run_part.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/run_part_opt.F90` & `PyPartMC-1.1.4/src/run_part_opt.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/run_part_opt.hpp` & `PyPartMC-1.1.4/src/run_part_opt.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/scenario.F90` & `PyPartMC-1.1.4/src/scenario.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/scenario.cpp` & `PyPartMC-1.1.4/src/scenario.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/scenario.hpp` & `PyPartMC-1.1.4/src/scenario.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/spec_file_pypartmc.F90` & `PyPartMC-1.1.4/src/spec_file_pypartmc.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/spec_file_pypartmc.cpp` & `PyPartMC-1.1.4/src/spec_file_pypartmc.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/sys.F90` & `PyPartMC-1.1.4/src/sys.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/sys.cpp` & `PyPartMC-1.1.4/src/sys.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/util.F90` & `PyPartMC-1.1.4/src/util.F90`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/util.cpp` & `PyPartMC-1.1.4/src/util.cpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/src/util.hpp` & `PyPartMC-1.1.4/src/util.hpp`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/common.py` & `PyPartMC-1.1.4/tests/common.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_aero_data.py` & `PyPartMC-1.1.4/tests/test_aero_data.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_aero_dist.py` & `PyPartMC-1.1.4/tests/test_aero_dist.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_aero_mode.py` & `PyPartMC-1.1.4/tests/test_aero_mode.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_aero_particle.py` & `PyPartMC-1.1.4/tests/test_aero_particle.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_aero_state.py` & `PyPartMC-1.1.4/tests/test_aero_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_bin_grid.py` & `PyPartMC-1.1.4/tests/test_bin_grid.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_condense.py` & `PyPartMC-1.1.4/tests/test_condense.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_dtors.py` & `PyPartMC-1.1.4/tests/test_dtors.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_env_state.py` & `PyPartMC-1.1.4/tests/test_env_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_gas_data.py` & `PyPartMC-1.1.4/tests/test_gas_data.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_gas_state.py` & `PyPartMC-1.1.4/tests/test_gas_state.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_loss_rate.py` & `PyPartMC-1.1.4/tests/test_loss_rate.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_output.py` & `PyPartMC-1.1.4/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_rand.py` & `PyPartMC-1.1.4/tests/test_rand.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_run_part.py` & `PyPartMC-1.1.4/tests/test_run_part.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_run_part_opt.py` & `PyPartMC-1.1.4/tests/test_run_part_opt.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_scenario.py` & `PyPartMC-1.1.4/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_units.py` & `PyPartMC-1.1.4/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_util.py` & `PyPartMC-1.1.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPartMC-1.1.3/tests/test_version.py` & `PyPartMC-1.1.4/tests/test_version.py`

 * *Files identical despite different names*

