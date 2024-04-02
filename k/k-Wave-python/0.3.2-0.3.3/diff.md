# Comparing `tmp/k_wave_python-0.3.2.tar.gz` & `tmp/k_wave_python-0.3.3.tar.gz`

## Comparing `k_wave_python-0.3.2.tar` & `k_wave_python-0.3.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.readthedocs.yaml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/CITATION.cff
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/Dockerfile
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/make_docs.sh
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/run_tests.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    11496 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/content/13487435192755641643
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/content/1921099194987439213
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/content/5526710289020645422
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/content/5950811561636507670
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.ruff_cache/content/655415607675938108
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/__init__.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/data.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/enums.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/executor.py
--rw-r--r--   0        0        0    67376 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation.py
--rw-r--r--   0        0        0    23601 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kgrid.py
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kmedium.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/ksensor.py
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/ksource.py
--rw-r--r--   0        0        0    23589 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kspaceFirstOrder2D.py
--rw-r--r--   0        0        0    24275 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kspaceFirstOrder3D.py
--rw-r--r--   0        0        0    17937 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kspaceFirstOrderAS.py
--rw-r--r--   0        0        0    31375 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/ktransducer.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/recorder.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/__init__.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/create_absorption_variables.py
--rw-r--r--   0        0        0    17342 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/create_storage_variables.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/data_cast.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/display_simulation_params.py
--rw-r--r--   0        0        0    11055 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/expand_grid_matrices.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/retract_transducer_grid_size.py
--rw-r--r--   0        0        0    19867 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/save_to_disk_func.py
--rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/scale_source_terms_func.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/kWaveSimulation_helper/set_sound_speed_ref.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/options/__init__.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/options/simulation_execution_options.py
--rw-r--r--   0        0        0    18691 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/options/simulation_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/reconstruction/__init__.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/reconstruction/beamform.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/reconstruction/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/__init__.py
--rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/angular_spectrum.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/angular_spectrum_cw.py
--rw-r--r--   0        0        0    11505 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/atten_comp.py
--rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/checks.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/colormap.py
--rw-r--r--   0        0        0    17014 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/conversion.py
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/data.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/dotdictionary.py
--rw-r--r--   0        0        0    26076 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/filters.py
--rw-r--r--   0        0        0    15464 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/interp.py
--rw-r--r--   0        0        0    16613 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/io.py
--rw-r--r--   0        0        0    35129 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/kwave_array.py
--rw-r--r--   0        0        0   117193 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/mapgen.py
--rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/math.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/matlab.py
--rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/matrix.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/plot.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/pml.py
--rw-r--r--   0        0        0    29134 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/signals.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/tictoc.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/kwave/utils/typing.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/LICENSE
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/docs/README.md
--rw-r--r--   0        0        0    45792 2020-02-02 00:00:00.000000 k_wave_python-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/CITATION.cff
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/Dockerfile
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/make_docs.sh
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/run_tests.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    11496 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/content/13487435192755641643
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/content/1921099194987439213
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/content/5526710289020645422
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/content/5950811561636507670
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.ruff_cache/content/655415607675938108
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/__init__.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/data.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/enums.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/executor.py
+-rw-r--r--   0        0        0    67343 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation.py
+-rw-r--r--   0        0        0    23197 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kgrid.py
+-rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kmedium.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/ksensor.py
+-rw-r--r--   0        0        0    19621 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/ksource.py
+-rw-r--r--   0        0        0    23094 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kspaceFirstOrder2D.py
+-rw-r--r--   0        0        0    23757 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kspaceFirstOrder3D.py
+-rw-r--r--   0        0        0    17380 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kspaceFirstOrderAS.py
+-rw-r--r--   0        0        0    31411 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/ktransducer.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/recorder.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/__init__.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/create_absorption_variables.py
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/create_storage_variables.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/data_cast.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/display_simulation_params.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/expand_grid_matrices.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/retract_transducer_grid_size.py
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/save_to_disk_func.py
+-rw-r--r--   0        0        0    14618 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/scale_source_terms_func.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/kWaveSimulation_helper/set_sound_speed_ref.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/options/__init__.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/options/simulation_execution_options.py
+-rw-r--r--   0        0        0    18531 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/options/simulation_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/reconstruction/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/reconstruction/beamform.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/reconstruction/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/__init__.py
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/angular_spectrum.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/angular_spectrum_cw.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/atten_comp.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/checks.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/colormap.py
+-rw-r--r--   0        0        0    16798 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/conversion.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/data.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/dotdictionary.py
+-rw-r--r--   0        0        0    25854 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/filters.py
+-rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/interp.py
+-rw-r--r--   0        0        0    16622 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/io.py
+-rw-r--r--   0        0        0    35116 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/kwave_array.py
+-rw-r--r--   0        0        0   115943 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/mapgen.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/math.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/matlab.py
+-rw-r--r--   0        0        0    14094 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/matrix.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/plot.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/pml.py
+-rw-r--r--   0        0        0    29001 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/signals.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/tictoc.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/kwave/utils/typing.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/docs/README.md
+-rw-r--r--   0        0        0    45794 2020-02-02 00:00:00.000000 k_wave_python-0.3.3/PKG-INFO
```

### Comparing `k_wave_python-0.3.2/.pre-commit-config.yaml` & `k_wave_python-0.3.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,23 @@
   hooks:
   - id: nb-clean
     name: nb-clean
     entry: nb-clean clean
     language: python
     types_or: [jupyter]
     minimum_pre_commit_version: 2.9.2
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  # Ruff version.
+  rev: v0.2.2
+  hooks:
+    # Run the linter.
+    - id: ruff
+      args: [ --fix ]
+    # Run the formatter.
+    - id: ruff-format
 # - repo: https://github.com/pre-commit/pre-commit-hooks
 #   rev: v4.5.0  # Use the ref you want to point at
 #   hooks:
 #   -   id: trailing-whitespace
 # - repo: https://github.com/nbQA-dev/nbQA
 #   rev: 1.7.1
 #   hooks:
```

### Comparing `k_wave_python-0.3.2/.pytest_cache/v/cache/nodeids` & `k_wave_python-0.3.3/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/.ruff_cache/content/13487435192755641643` & `k_wave_python-0.3.3/.ruff_cache/content/13487435192755641643`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/.ruff_cache/content/1921099194987439213` & `k_wave_python-0.3.3/.ruff_cache/content/1921099194987439213`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/.ruff_cache/content/5950811561636507670` & `k_wave_python-0.3.3/.ruff_cache/content/5950811561636507670`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/kwave/data.py` & `k_wave_python-0.3.3/kwave/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         - It can have 3 elements at max
         - Its elements can be anything
         - The elements do not have to be same type,
                 e.g. this is valid: Array([<scalar>, <List>, <Tuple of Tuples>])
 
     WARNING: The class will be deprecated once we refactor the kWaveGrid class to use the Vector class instead!
     """
+
     data: list
 
     def __post_init__(self):
         assert 1 <= len(self) <= 3
 
     def __len__(self):
         return len(self.data)
```

### Comparing `k_wave_python-0.3.2/kwave/executor.py` & `k_wave_python-0.3.3/kwave/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,63 +5,61 @@
 
 import h5py
 
 from kwave.utils.dotdictionary import dotdict
 
 
 class Executor:
-
     def __init__(self, execution_options, simulation_options):
-
         self.execution_options = execution_options
         self.simulation_options = simulation_options
 
         self._make_binary_executable()
 
     def _make_binary_executable(self):
         self.execution_options.binary_path.chmod(self.execution_options.binary_path.stat().st_mode | stat.S_IEXEC)
 
     def run_simulation(self, input_filename: str, output_filename: str, options: str):
-
-        command = f'{self.execution_options.system_string} ' \
-                  f'{self.execution_options.binary_path} ' \
-                  f'-i {input_filename} ' \
-                  f'-o {output_filename} ' \
-                  f'{options}'
+        command = (
+            f"{self.execution_options.system_string} "
+            f"{self.execution_options.binary_path} "
+            f"-i {input_filename} "
+            f"-o {output_filename} "
+            f"{options}"
+        )
 
         try:
             with subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True) as proc:
                 stdout, stderr = "", ""
                 if self.execution_options.show_sim_log:
                     # Stream stdout in real-time
                     for line in proc.stdout:
-                        print(line, end='')
+                        print(line, end="")
                 else:
-                    stdout, stderr = proc.communicate()  
+                    stdout, stderr = proc.communicate()
 
-                proc.wait() # wait for process to finish before checking return code
+                proc.wait()  # wait for process to finish before checking return code
                 if proc.returncode != 0:
                     raise subprocess.CalledProcessError(proc.returncode, command, stdout, stderr)
 
         except subprocess.CalledProcessError as e:
             # Special handling for MagicMock during testing
             if isinstance(e.returncode, unittest.mock.MagicMock):
-                logging.info('Skipping AssertionError in testing.')
+                logging.info("Skipping AssertionError in testing.")
             else:
                 # This ensures stdout is printed regardless of show_sim_logs value if an error occurs
                 print(e.stdout)
                 raise
 
         sensor_data = self.parse_executable_output(output_filename)
 
         return sensor_data
 
     @staticmethod
     def parse_executable_output(output_filename: str) -> dotdict:
-
         # Load the simulation and pml sizes from the output file
         # with h5py.File(output_filename, 'r') as output_file:
         #     Nx, Ny, Nz = output_file['/Nx'][0].item(), output_file['/Ny'][0].item(), output_file['/Nz'][0].item()
         #     pml_x_size, pml_y_size = output_file['/pml_x_size'][0].item(), output_file['/pml_y_size'][0].item()
         #     pml_z_size = output_file['/pml_z_size'][0].item() if Nz > 1 else 0
 
         # # Set the default index variables for the _all and _final variables
@@ -75,18 +73,18 @@
         # if self.simulation_options.pml_inside:
         #     x1, x2 = 1 + pml_x_size, Nx - pml_x_size
         #     y1, y2 = (1, Ny) if self.simulation_options.simulation_type is SimulationType.AXISYMMETRIC else (
         #         1 + pml_y_size, Ny - pml_y_size)
         #     z1, z2 = 1 + pml_z_size, Nz - pml_z_size if Nz > 1 else (1, Nz)
 
         # Load the C++ data back from disk using h5py
-        with h5py.File(output_filename, 'r') as output_file:
+        with h5py.File(output_filename, "r") as output_file:
             sensor_data = {}
             for key in output_file.keys():
-                sensor_data[key] = output_file[f'/{key}'][0].squeeze()
+                sensor_data[key] = output_file[f"/{key}"][0].squeeze()
         #     if self.simulation_options.cuboid_corners:
         #         sensor_data = [output_file[f'/p/{index}'][()] for index in range(1, len(key['mask']) + 1)]
         #
         # # Combine the sensor data if using a kWaveTransducer as a sensor
         # if isinstance(sensor, kWaveTransducer):
         #     sensor_data['p'] = sensor.combine_sensor_data(sensor_data['p'])
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import logging
 from dataclasses import dataclass
 
 import numpy as np
 
 from kwave.data import Vector
-from kwave.kWaveSimulation_helper import display_simulation_params, set_sound_speed_ref, expand_grid_matrices, \
-    create_storage_variables, create_absorption_variables, scale_source_terms_func
+from kwave.kWaveSimulation_helper import (
+    display_simulation_params,
+    set_sound_speed_ref,
+    expand_grid_matrices,
+    create_storage_variables,
+    create_absorption_variables,
+    scale_source_terms_func,
+)
 from kwave.kgrid import kWaveGrid
 from kwave.kmedium import kWaveMedium
 from kwave.ksensor import kSensor
 from kwave.ksource import kSource
 from kwave.ktransducer import NotATransducer
 from kwave.options.simulation_options import SimulationOptions, SimulationType
 from kwave.recorder import Recorder
@@ -21,21 +27,17 @@
 from kwave.utils.filters import smooth
 from kwave.utils.matlab import matlab_find, matlab_mask
 from kwave.utils.matrix import num_dim2
 
 
 @dataclass
 class kWaveSimulation(object):
-
-    def __init__(self,
-                 kgrid: kWaveGrid,
-                 source: kSource,
-                 sensor: NotATransducer,
-                 medium: kWaveMedium,
-                 simulation_options: SimulationOptions):
+    def __init__(
+        self, kgrid: kWaveGrid, source: kSource, sensor: NotATransducer, medium: kWaveMedium, simulation_options: SimulationOptions
+    ):
         self.precision = None
         self.kgrid = kgrid
         self.medium = medium
         self.source = source
         self.sensor = sensor
         self.options = simulation_options
 
@@ -45,26 +47,19 @@
         # flags which control the characteristics of the sensor
         #: Whether time reversal simulation is enabled
 
         # check if performing time reversal, and replace inputs to explicitly use a
         # source with a dirichlet boundary condition
         if self.sensor.time_reversal_boundary_data is not None:
             # define a new source structure
-            source = {
-                'p_mask': self.sensor.p_mask,
-                'p': np.flip(self.sensor.time_reversal_boundary_data, 2),
-                'p_mode': 'dirichlet'
-            }
+            source = {"p_mask": self.sensor.p_mask, "p": np.flip(self.sensor.time_reversal_boundary_data, 2), "p_mode": "dirichlet"}
 
             # define a new sensor structure
             Nx, Ny, Nz = self.kgrid.Nx, self.kgrid.Ny, self.kgrid.Nz
-            sensor = kSensor(
-                mask=np.ones((Nx, Ny, max(1, Nz))),
-                record=['p_final']
-            )
+            sensor = kSensor(mask=np.ones((Nx, Ny, max(1, Nz))), record=["p_final"])
             # set time reversal flag
             self.userarg_time_rev = True
         else:
             # set time reversal flag
             self.userarg_time_rev = False
 
             #: Whether sensor.mask should be re-ordered.
@@ -84,74 +79,74 @@
             #: If tse sensor is an object of the kWaveTransducer class
             self.transducer_sensor = False
 
             self.record = Recorder()
 
         # transducer source flags
         #: transducer is object of kWaveTransducer class
-        self.transducer_source         = False
+        self.transducer_source = False
 
         #: Apply receive elevation focus on the transducer
         self.transducer_receive_elevation_focus = False
 
         # general
-        self.COLOR_MAP                       = get_color_map()      #: default color map
-        self.ESTIMATE_SIM_TIME_STEPS         = 50                   #: time steps used to estimate simulation time
-        self.HIGHEST_PRIME_FACTOR_WARNING    = 7                    #: largest prime factor before warning
-        self.KSPACE_CFL                      = 0.3                  #: default CFL value used if kgrid.t_array is set to 'auto'
-        self.PSTD_CFL                        = 0.1                  #: default CFL value used if kgrid.t_array is set to 'auto'
+        self.COLOR_MAP = get_color_map()  #: default color map
+        self.ESTIMATE_SIM_TIME_STEPS = 50  #: time steps used to estimate simulation time
+        self.HIGHEST_PRIME_FACTOR_WARNING = 7  #: largest prime factor before warning
+        self.KSPACE_CFL = 0.3  #: default CFL value used if kgrid.t_array is set to 'auto'
+        self.PSTD_CFL = 0.1  #: default CFL value used if kgrid.t_array is set to 'auto'
 
         # source types
-        self.SOURCE_S_MODE_DEF               = 'additive'           #: source mode for stress sources
-        self.SOURCE_P_MODE_DEF               = 'additive'           #: source mode for pressure sources
-        self.SOURCE_U_MODE_DEF               = 'additive'           #: source mode for velocity sources
+        self.SOURCE_S_MODE_DEF = "additive"  #: source mode for stress sources
+        self.SOURCE_P_MODE_DEF = "additive"  #: source mode for pressure sources
+        self.SOURCE_U_MODE_DEF = "additive"  #: source mode for velocity sources
 
         # filenames
-        self.STREAM_TO_DISK_FILENAME         = 'temp_sensor_data.bin'   #: default disk stream filename
-        self.LOG_NAME                        = ['k-Wave-Log-', get_date_string()]  #: default log filename
+        self.STREAM_TO_DISK_FILENAME = "temp_sensor_data.bin"  #: default disk stream filename
+        self.LOG_NAME = ["k-Wave-Log-", get_date_string()]  #: default log filename
 
         self.calling_func_name = None
-        logging.log(logging.INFO, f'  start time: {get_date_string()}')
+        logging.log(logging.INFO, f"  start time: {get_date_string()}")
 
         self.c_ref, self.c_ref_compression, self.c_ref_shear = [None] * 3
         self.transducer_input_signal = None
 
         #: Indexing variable corresponding to the location of all the pressure source elements
         self.p_source_pos_index = None
         #: Indexing variable corresponding to the location of all the velocity source elements
         self.u_source_pos_index = None
         #: Indexing variable corresponding to the location of all the stress source elements
         self.s_source_pos_index = None
 
         #: Delay mask that accounts for the beamforming delays and elevation focussing
         self.delay_mask = None
 
-        self.absorb_nabla1  = None  #: absorbing fractional Laplacian operator
-        self.absorb_tau     = None  #: absorbing fractional Laplacian coefficient
-        self.absorb_nabla2  = None  #: dispersive fractional Laplacian operator
-        self.absorb_eta     = None  #: dispersive fractional Laplacian coefficient
-
-        self.dt             = None  #: Alias to kgrid.dt
-        self.rho0           = None  #: Alias to medium.density
-        self.c0             = None  #: Alias to medium.sound_speed
+        self.absorb_nabla1 = None  #: absorbing fractional Laplacian operator
+        self.absorb_tau = None  #: absorbing fractional Laplacian coefficient
+        self.absorb_nabla2 = None  #: dispersive fractional Laplacian operator
+        self.absorb_eta = None  #: dispersive fractional Laplacian coefficient
+
+        self.dt = None  #: Alias to kgrid.dt
+        self.rho0 = None  #: Alias to medium.density
+        self.c0 = None  #: Alias to medium.sound_speed
         self.index_data_type = None
 
     @property
     def equation_of_state(self):
         """
         Returns:
             Set equation of state variable
         """
         if self.medium.absorbing:
             if self.medium.stokes:
-                return 'stokes'
+                return "stokes"
             else:
-                return 'absorbing'
+                return "absorbing"
         else:
-            return 'loseless'
+            return "loseless"
 
     @property
     def use_sensor(self):
         """
         Returns:
             False if no output of any kind is required
 
@@ -161,16 +156,15 @@
     @property
     def blank_sensor(self):
         """
         Returns
             True if sensor.mask is not defined but _max_all or _final variables are still recorded
 
         """
-        fields = ['p', 'p_max', 'p_min', 'p_rms', 'u', 'u_non_staggered',
-                  'u_split_field', 'u_max', 'u_min', 'u_rms', 'I', 'I_avg']
+        fields = ["p", "p_max", "p_min", "p_rms", "u", "u_non_staggered", "u_split_field", "u_max", "u_min", "u_rms", "I", "I_avg"]
         if not any(self.record.is_set(fields)) and not self.time_rev:
             return False
         return False
 
     @property
     def kelvin_voigt_model(self):
         """
@@ -193,16 +187,15 @@
     def time_rev(self):
         """
         Returns:
             True for time reversal simulaions using sensor.time_reversal_boundary_data
 
         """
         if self.sensor is not None and not isinstance(self.sensor, NotATransducer):
-            if not self.options.simulation_type.is_elastic_simulation() and \
-                    self.sensor.time_reversal_boundary_data is not None:
+            if not self.options.simulation_type.is_elastic_simulation() and self.sensor.time_reversal_boundary_data is not None:
                 return True
         else:
             return self.userarg_time_rev
 
     @property
     def elastic_time_rev(self):
         """
@@ -459,15 +452,15 @@
     def use_w_source_correction_u(self):
         """
         Returns:
             Whether to use the w source correction instead of the k-space source correction for velocity sources
         """
         flag = False
         if not isinstance(self.source, NotATransducer):
-            if any([(getattr(self.source, k) is not None) for k in ['ux', 'uy', 'uz', 'u_mask']]):
+            if any([(getattr(self.source, k) is not None) for k in ["ux", "uy", "uz", "u_mask"]]):
                 if self.source.u_frequency_ref is not None:
                     flag = True
         return flag
 
     def input_checking(self, calling_func_name) -> None:
         """
         Check the input fields for correctness and validness
@@ -495,16 +488,15 @@
         is_elastic_code = opt.simulation_type.is_elastic_simulation()
         self.print_start_status(is_elastic_code=is_elastic_code)
         self.set_index_data_type()
 
         user_medium_density_input = self.check_medium(self.medium, self.kgrid.k, simulation_type=opt.simulation_type)
 
         # select the reference sound speed used in the k-space operator
-        self.c_ref, self.c_ref_compression, self.c_ref_shear \
-            = set_sound_speed_ref(self.medium, opt.simulation_type)
+        self.c_ref, self.c_ref_compression, self.c_ref_shear = set_sound_speed_ref(self.medium, opt.simulation_type)
 
         self.check_source(k_dim, self.kgrid.Nt)
         self.check_sensor(k_dim)
         self.check_kgrid_time()
         self.precision = self.select_precision(opt)
         self.check_input_combinations(opt, user_medium_density_input, k_dim, pml_size, self.kgrid.N)
 
@@ -517,66 +509,65 @@
         self.assign_pseudonyms(self.medium, self.kgrid)
         self.scale_source_terms(opt.scale_source_terms)
         self.create_pml_indices(
             kgrid_dim=self.kgrid.dim,
             kgrid_N=Vector(self.kgrid.N),
             pml_size=pml_size,
             pml_inside=opt.pml_inside,
-            is_axisymmetric=opt.simulation_type.is_axisymmetric()
+            is_axisymmetric=opt.simulation_type.is_axisymmetric(),
         )
 
     @staticmethod
     def check_calling_func_name_and_dim(calling_func_name, kgrid_dim) -> None:
         """
         Check correct function has been called for the dimensionality of kgrid
 
         Args:
             calling_func_name: Name of the script that makes calls to kWaveSimulation
             kgrid_dim: Dimensionality of the kWaveGrid
 
         Returns:
             None
         """
-        assert not calling_func_name.startswith(('pstdElastic', 'kspaceElastic')), \
-            "Elastic simulation is not supported."
+        assert not calling_func_name.startswith(("pstdElastic", "kspaceElastic")), "Elastic simulation is not supported."
 
-        if calling_func_name == 'kspaceFirstOrder1D':
-            assert kgrid_dim == 1, f'kgrid has the wrong dimensionality for {calling_func_name}.'
-        elif calling_func_name in ['kspaceFirstOrder2D', 'pstdElastic2D', 'kspaceElastic2D', 'kspaceFirstOrderAS']:
-            assert kgrid_dim == 2, f'kgrid has the wrong dimensionality for {calling_func_name}.'
-        elif calling_func_name in ['kspaceFirstOrder3D', 'pstdElastic3D', 'kspaceElastic3D']:
-            assert kgrid_dim == 3, f'kgrid has the wrong dimensionality for {calling_func_name}.'
+        if calling_func_name == "kspaceFirstOrder1D":
+            assert kgrid_dim == 1, f"kgrid has the wrong dimensionality for {calling_func_name}."
+        elif calling_func_name in ["kspaceFirstOrder2D", "pstdElastic2D", "kspaceElastic2D", "kspaceFirstOrderAS"]:
+            assert kgrid_dim == 2, f"kgrid has the wrong dimensionality for {calling_func_name}."
+        elif calling_func_name in ["kspaceFirstOrder3D", "pstdElastic3D", "kspaceElastic3D"]:
+            assert kgrid_dim == 3, f"kgrid has the wrong dimensionality for {calling_func_name}."
 
     @staticmethod
     def print_start_status(is_elastic_code: bool) -> None:
         """
         Update command-line status with the start time
 
         Args:
             is_elastic_code: is the simulation elastic
 
         Returns:
             None
         """
         if is_elastic_code:  # pragma: no cover
-            logging.log(logging.INFO, 'Running k-Wave elastic simulation...')
+            logging.log(logging.INFO, "Running k-Wave elastic simulation...")
         else:
-            logging.log(logging.INFO, 'Running k-Wave simulation...')
-        logging.log(logging.INFO, f'  start time: {get_date_string()}')
+            logging.log(logging.INFO, "Running k-Wave simulation...")
+        logging.log(logging.INFO, f"  start time: {get_date_string()}")
 
     def set_index_data_type(self) -> None:
         """
         Pre-calculate the data type needed to store the matrix indices given the
         total number of grid points: indexing variables will be created using this data type to save memory
 
         Returns:
             None
         """
         total_grid_points = self.kgrid.total_grid_points
-        self.index_data_type = get_smallest_possible_type(total_grid_points, 'uint', default='double')
+        self.index_data_type = get_smallest_possible_type(total_grid_points, "uint", default="double")
 
     @staticmethod
     def check_medium(medium, kgrid_k, simulation_type: SimulationType) -> bool:
         """
         Check the properties of the medium structure for correctness and validity
 
         Args:
@@ -590,180 +581,175 @@
         """
 
         # if using the fluid code, allow the density field to be blank if the medium is homogeneous
         if (not simulation_type.is_elastic_simulation()) and medium.density is None and medium.sound_speed.size == 1:
             user_medium_density_input = False
             medium.density = 1
         else:
-            medium.ensure_defined('density')
+            medium.ensure_defined("density")
             user_medium_density_input = True
 
         # check medium absorption inputs for the fluid code
-        is_absorbing = any(medium.is_defined('alpha_coeff', 'alpha_power'))
-        is_stokes = (simulation_type.is_axisymmetric() or medium.alpha_mode == 'stokes')
+        is_absorbing = any(medium.is_defined("alpha_coeff", "alpha_power"))
+        is_stokes = simulation_type.is_axisymmetric() or medium.alpha_mode == "stokes"
         medium.set_absorbing(is_absorbing, is_stokes)
 
         if is_absorbing:
             medium.check_fields(kgrid_k.shape)
         return user_medium_density_input
 
-    def check_sensor(self, kgrid_dim)-> None:
+    def check_sensor(self, kgrid_dim) -> None:
         """
         Check the Sensor properties for correctness and validity
 
         Args:
             k_dim: kWaveGrid dimensionality
 
         Returns:
             None
         """
         # =========================================================================
         # CHECK SENSOR STRUCTURE INPUTS
         # =========================================================================
         # check sensor fields
         if self.sensor is not None:
-
             # check the sensor input is valid
             # TODO FARID move this check as a type checking
-            assert isinstance(self.sensor, (kSensor, NotATransducer)), \
-                'sensor must be defined as an object of the kSensor or kWaveTransducer class.'
+            assert isinstance(
+                self.sensor, (kSensor, NotATransducer)
+            ), "sensor must be defined as an object of the kSensor or kWaveTransducer class."
 
             # check if sensor is a transducer, otherwise check input fields
             if not isinstance(self.sensor, NotATransducer):
                 if kgrid_dim == 2:
-
                     # check for sensor directivity input and set flag
                     directivity = self.sensor.directivity
                     if directivity is not None and self.sensor.directivity.angle is not None:
-
                         # make sure the sensor mask is not blank
-                        assert self.sensor.mask is not None, 'The mask must be defined for the sensor'
+                        assert self.sensor.mask is not None, "The mask must be defined for the sensor"
 
                         # check sensor.directivity.pattern and sensor.mask have the same size
-                        assert directivity.angle.shape == self.sensor.mask.shape, \
-                            'sensor.directivity.angle and sensor.mask must be the same size.'
+                        assert (
+                            directivity.angle.shape == self.sensor.mask.shape
+                        ), "sensor.directivity.angle and sensor.mask must be the same size."
 
                         # check if directivity size input exists, otherwise make it
                         # a constant times kgrid.dx
                         if directivity.size is None:
                             directivity.set_default_size(self.kgrid)
 
                         # find the unique directivity angles
                         # assign the wavenumber vectors
                         directivity.set_unique_angles(self.sensor.mask)
                         directivity.set_wavenumbers(self.kgrid)
 
                 # check for time reversal inputs and set flags
-                if not self.options.simulation_type.is_elastic_simulation() and \
-                        self.sensor.time_reversal_boundary_data is not None:
+                if not self.options.simulation_type.is_elastic_simulation() and self.sensor.time_reversal_boundary_data is not None:
                     self.record.p = False
 
                 # check for sensor.record and set usage flgs - if no flgs are
                 # given, the time history of the acoustic pressure is recorded by
                 # default
                 if self.sensor.record is not None:
-
                     # check for time reversal data
                     if self.time_rev:
-                        logging.log(logging.WARN, 'sensor.record is not used for time reversal reconstructions')
+                        logging.log(logging.WARN, "sensor.record is not used for time reversal reconstructions")
 
                     # check the input is a cell array
-                    assert isinstance(self.sensor.record, list), \
-                        'sensor.record must be given as a list, e.g. ["p", "u"]'
+                    assert isinstance(self.sensor.record, list), 'sensor.record must be given as a list, e.g. ["p", "u"]'
 
                     # check the sensor record flgs
-                    self.record.set_flags_from_list(
-                        self.sensor.record,
-                        self.options.simulation_type.is_elastic_simulation()
-                    )
+                    self.record.set_flags_from_list(self.sensor.record, self.options.simulation_type.is_elastic_simulation())
 
                 # enforce the sensor.mask field unless just recording the max_all
                 # and _final variables
-                fields = ['p', 'p_max', 'p_min', 'p_rms',
-                          'u', 'u_non_staggered', 'u_split_field', 'u_max', 'u_min', 'u_rms', 'I', 'I_avg']
+                fields = ["p", "p_max", "p_min", "p_rms", "u", "u_non_staggered", "u_split_field", "u_max", "u_min", "u_rms", "I", "I_avg"]
                 if any(self.record.is_set(fields)):
                     assert self.sensor.mask is not None
 
                 # check if sensor mask is a binary grid, a set of cuboid corners,
                 # or a set of Cartesian interpolation points
                 if not self.blank_sensor:
-                    if (kgrid_dim == 3 and num_dim2(self.sensor.mask) == 3) or \
-                            (kgrid_dim != 3 and (self.sensor.mask.shape == self.kgrid.k.shape)):
-
+                    if (kgrid_dim == 3 and num_dim2(self.sensor.mask) == 3) or (
+                        kgrid_dim != 3 and (self.sensor.mask.shape == self.kgrid.k.shape)
+                    ):
                         # check the grid is binary
-                        assert self.sensor.mask.sum() == (self.sensor.mask.size - (self.sensor.mask == 0).sum()), \
-                            'sensor.mask must be a binary grid (numeric values must be 0 or 1).'
+                        assert self.sensor.mask.sum() == (
+                            self.sensor.mask.size - (self.sensor.mask == 0).sum()
+                        ), "sensor.mask must be a binary grid (numeric values must be 0 or 1)."
 
                         # check the grid is not empty
-                        assert self.sensor.mask.sum() != 0, \
-                            'sensor.mask must be a binary grid with at least one element set to 1.'
+                        assert self.sensor.mask.sum() != 0, "sensor.mask must be a binary grid with at least one element set to 1."
 
                     elif self.sensor.mask.shape[0] == 2 * kgrid_dim:
-
                         # make sure the points are integers
-                        assert np.all(self.sensor.mask % 1 == 0), \
-                            'sensor.mask cuboid corner indices must be integers.'
+                        assert np.all(self.sensor.mask % 1 == 0), "sensor.mask cuboid corner indices must be integers."
 
                         # store a copy of the cuboid corners
                         self.record.cuboid_corners_list = self.sensor.mask
 
                         # check the list makes sense
-                        if np.any(self.sensor.mask[self.kgrid.dim:, :] - self.sensor.mask[:self.kgrid.dim, :] < 0):
+                        if np.any(self.sensor.mask[self.kgrid.dim :, :] - self.sensor.mask[: self.kgrid.dim, :] < 0):
                             if kgrid_dim == 1:
-                                raise ValueError('sensor.mask cuboid corners must be defined '
-                                                 'as [x1, x2; ...].'' where x2 => x1, etc.')
+                                raise ValueError("sensor.mask cuboid corners must be defined " "as [x1, x2; ...]." " where x2 => x1, etc.")
                             elif kgrid_dim == 2:
-                                raise ValueError('sensor.mask cuboid corners must be defined '
-                                                 'as [x1, y1, x2, y2; ...].'' where x2 => x1, etc.')
+                                raise ValueError(
+                                    "sensor.mask cuboid corners must be defined " "as [x1, y1, x2, y2; ...]." " where x2 => x1, etc."
+                                )
                             elif kgrid_dim == 3:
-                                raise ValueError('sensor.mask cuboid corners must be defined'
-                                                 ' as [x1, y1, z1, x2, y2, z2; ...].'' where x2 => x1, etc.')
+                                raise ValueError(
+                                    "sensor.mask cuboid corners must be defined"
+                                    " as [x1, y1, z1, x2, y2, z2; ...]."
+                                    " where x2 => x1, etc."
+                                )
 
                         # check the list are within bounds
                         if np.any(self.sensor.mask < 1):
-                            raise ValueError('sensor.mask cuboid corners must be within the grid.')
+                            raise ValueError("sensor.mask cuboid corners must be within the grid.")
                         else:
                             if kgrid_dim == 1:
                                 if np.any(self.sensor.mask > self.kgrid.Nx):
-                                    raise ValueError('sensor.mask cuboid corners must be within the grid.')
+                                    raise ValueError("sensor.mask cuboid corners must be within the grid.")
                             elif kgrid_dim == 2:
-                                if np.any(self.sensor.mask[[0, 2], :] > self.kgrid.Nx) or \
-                                        np.any(self.sensor.mask[[1, 3], :] > self.kgrid.Ny):
-                                    raise ValueError('sensor.mask cuboid corners must be within the grid.')
+                                if np.any(self.sensor.mask[[0, 2], :] > self.kgrid.Nx) or np.any(
+                                    self.sensor.mask[[1, 3], :] > self.kgrid.Ny
+                                ):
+                                    raise ValueError("sensor.mask cuboid corners must be within the grid.")
                             elif kgrid_dim == 3:
-                                if np.any(self.sensor.mask[[0, 3], :] > self.kgrid.Nx) or \
-                                        np.any(self.sensor.mask[[1, 4], :] > self.kgrid.Ny) or \
-                                        np.any(self.sensor.mask[[2, 5], :] > self.kgrid.Nz):
-                                    raise ValueError('sensor.mask cuboid corners must be within the grid.')
+                                if (
+                                    np.any(self.sensor.mask[[0, 3], :] > self.kgrid.Nx)
+                                    or np.any(self.sensor.mask[[1, 4], :] > self.kgrid.Ny)
+                                    or np.any(self.sensor.mask[[2, 5], :] > self.kgrid.Nz)
+                                ):
+                                    raise ValueError("sensor.mask cuboid corners must be within the grid.")
 
                         # create a binary mask for display from the list of corners
                         # TODO FARID mask should be option_factory in sensor not here
                         self.sensor.mask = np.zeros_like(self.kgrid.k, dtype=bool)
                         cuboid_corners_list = self.record.cuboid_corners_list
                         for cuboid_index in range(cuboid_corners_list.shape[1]):
                             if self.kgrid.dim == 1:
-                                self.sensor.mask[
-                                    cuboid_corners_list[0, cuboid_index]:cuboid_corners_list[1, cuboid_index]
-                                ] = 1
+                                self.sensor.mask[cuboid_corners_list[0, cuboid_index] : cuboid_corners_list[1, cuboid_index]] = 1
                             if self.kgrid.dim == 2:
                                 self.sensor.mask[
-                                    cuboid_corners_list[0, cuboid_index]:cuboid_corners_list[2, cuboid_index],
-                                    cuboid_corners_list[1, cuboid_index]:cuboid_corners_list[3, cuboid_index]
+                                    cuboid_corners_list[0, cuboid_index] : cuboid_corners_list[2, cuboid_index],
+                                    cuboid_corners_list[1, cuboid_index] : cuboid_corners_list[3, cuboid_index],
                                 ] = 1
                             if self.kgrid.dim == 3:
                                 self.sensor.mask[
-                                    cuboid_corners_list[0, cuboid_index]:cuboid_corners_list[3, cuboid_index],
-                                    cuboid_corners_list[1, cuboid_index]:cuboid_corners_list[4, cuboid_index],
-                                    cuboid_corners_list[2, cuboid_index]:cuboid_corners_list[5, cuboid_index]
+                                    cuboid_corners_list[0, cuboid_index] : cuboid_corners_list[3, cuboid_index],
+                                    cuboid_corners_list[1, cuboid_index] : cuboid_corners_list[4, cuboid_index],
+                                    cuboid_corners_list[2, cuboid_index] : cuboid_corners_list[5, cuboid_index],
                                 ] = 1
                     else:
                         # check the Cartesian sensor mask is the correct size
                         # (1 x N, 2 x N, 3 x N)
-                        assert self.sensor.mask.shape[0] == kgrid_dim and num_dim2(self.sensor.mask) <= 2, \
-                            f'Cartesian sensor.mask for a {kgrid_dim}D simulation must be given as a {kgrid_dim} by N array.'
+                        assert (
+                            self.sensor.mask.shape[0] == kgrid_dim and num_dim2(self.sensor.mask) <= 2
+                        ), f"Cartesian sensor.mask for a {kgrid_dim}D simulation must be given as a {kgrid_dim} by N array."
 
                         # set Cartesian mask flag (this is modified in
                         # createStorageVariables if the interpolation setting is
                         # set to nearest)
                         self.binary_sensor_mask = False
 
                         # extract Cartesian data from sensor mask
@@ -787,16 +773,17 @@
                             self.sensor_z = self.sensor.mask[2, :]
 
                         # compute an equivalent sensor mask using nearest neighbour
                         # interpolation, if flgs.time_rev = false and
                         # cartesian_interp = 'linear' then this is only used for
                         # display, if flgs.time_rev = true or cartesian_interp =
                         # 'nearest' this grid is used as the sensor.mask
-                        self.sensor.mask, self.order_index, self.reorder_index = \
-                            cart2grid(self.kgrid, self.sensor.mask, self.options.simulation_type.is_axisymmetric())
+                        self.sensor.mask, self.order_index, self.reorder_index = cart2grid(
+                            self.kgrid, self.sensor.mask, self.options.simulation_type.is_axisymmetric()
+                        )
 
                         # if in time reversal mode, reorder the p0 input data in
                         # the order of the binary sensor_mask
                         if self.time_rev:
                             raise NotImplementedError
                             """
                             # append the reordering data
@@ -821,15 +808,15 @@
 
                     # get the elevation mask that is used to extract the correct values
                     # from the sensor data buffer for averaging
                     self.transducer_receive_mask = self.sensor.elevation_beamforming_mask
 
         # check for directivity inputs with time reversal
         if kgrid_dim == 2 and self.use_sensor and self.compute_directivity and self.time_rev:
-            logging.log(logging.WARN, 'sensor directivity fields are not used for time reversal.')
+            logging.log(logging.WARN, "sensor directivity fields are not used for time reversal.")
 
     def check_source(self, k_dim, k_Nt) -> None:
         """
         Check the source properties for correctness and validity
 
         Args:
             kgrid_dim: kWaveGrid dimension
@@ -842,23 +829,22 @@
         # CHECK SOURCE STRUCTURE INPUTS
         # =========================================================================
 
         # check source inputs
         if not isinstance(self.source, (kSource, NotATransducer)):
             # allow an invalid or empty source input if computing time reversal,
             # otherwise return error
-            assert self.time_rev, 'source must be defined as an object of the kSource or kWaveTransducer classes.'
+            assert self.time_rev, "source must be defined as an object of the kSource or kWaveTransducer classes."
 
         elif not isinstance(self.source, NotATransducer):
-
             # --------------------------
             # SOURCE IS NOT A TRANSDUCER
             # --------------------------
 
-            '''
+            """
                 check allowable source types
                 
                 Depending on the kgrid dimensionality and the simulation type, 
                     following fields are allowed & might be use:
                 
                 kgrid.dim == 1:
                     non-elastic code:
@@ -869,108 +855,105 @@
                     elastic code:
                         ['p0', 'sxx', 'syy', 'sxy', 's_mask', 's_mode', 'ux', 'uy', 'u_mask', 'u_mode']
                 kgrid.dim == 3:
                     non-elastic code:
                         ['p0', 'p', 'p_mask', 'p_mode', 'p_frequency_ref', 'ux', 'uy', 'uz', 'u_mask', 'u_mode', 'u_frequency_ref']
                     elastic code:
                         ['p0', 'sxx', 'syy', 'szz', 'sxy', 'sxz', 'syz', 's_mask', 's_mode', 'ux', 'uy', 'uz', 'u_mask', 'u_mode']
-            '''
+            """
 
             self.source.validate(self.kgrid)
 
             # check for a time varying pressure source input
             if self.source.p is not None:
-
                 # check the source mode input is valid
                 if self.source.p_mode is None:
                     self.source.p_mode = self.SOURCE_P_MODE_DEF
 
                 if self.source_p > k_Nt:
-                    logging.log(logging.WARN, '  source.p has more time points than kgrid.Nt, remaining time points will not be used.')
+                    logging.log(logging.WARN, "  source.p has more time points than kgrid.Nt, remaining time points will not be used.")
 
                 # create an indexing variable corresponding to the location of all the source elements
                 self.p_source_pos_index = matlab_find(self.source.p_mask)
 
                 # check if the mask is binary or labelled
                 p_unique = np.unique(self.source.p_mask)
 
                 # create a second indexing variable
                 if p_unique.size <= 2 and p_unique.sum() == 1:
                     # set signal index to all elements
-                    self.p_source_sig_index = ':'
+                    self.p_source_sig_index = ":"
                 else:
                     # set signal index to the labels (this allows one input signal
                     # to be used for each source label)
                     self.p_source_sig_index = self.source.p_mask(self.source.p_mask != 0)
 
                 # convert the data type depending on the number of indices
                 self.p_source_pos_index = cast_to_type(self.p_source_pos_index, self.index_data_type)
                 if self.source_p_labelled:
                     self.p_source_sig_index = cast_to_type(self.p_source_sig_index, self.index_data_type)
 
             # check for time varying velocity source input and set source flag
-            if any([(getattr(self.source, k) is not None) for k in ['ux', 'uy', 'uz', 'u_mask']]):
-
+            if any([(getattr(self.source, k) is not None) for k in ["ux", "uy", "uz", "u_mask"]]):
                 # check the source mode input is valid
                 if self.source.u_mode is None:
                     self.source.u_mode = self.SOURCE_U_MODE_DEF
 
                 # create an indexing variable corresponding to the location of all
                 # the source elements
                 self.u_source_pos_index = matlab_find(self.source.u_mask)
 
                 # check if the mask is binary or labelled
                 u_unique = np.unique(self.source.u_mask)
 
                 # create a second indexing variable
                 if u_unique.size <= 2 and u_unique.sum() == 1:
-
                     # set signal index to all elements
-                    self.u_source_sig_index = ':'
+                    self.u_source_sig_index = ":"
                 else:
                     # set signal index to the labels (this allows one input signal
                     # to be used for each source label)
                     self.u_source_sig_index = self.source.u_mask[self.source.u_mask != 0]
 
                 # convert the data type depending on the number of indices
                 self.u_source_pos_index = cast_to_type(self.u_source_pos_index, self.index_data_type)
                 if self.source_u_labelled:
                     self.u_source_sig_index = cast_to_type(self.u_source_sig_index, self.index_data_type)
 
             # check for time varying stress source input and set source flag
-            if any([(getattr(self.source, k) is not None) for k in ['sxx', 'syy', 'szz', 'sxy', 'sxz', 'syz', 's_mask']]):
+            if any([(getattr(self.source, k) is not None) for k in ["sxx", "syy", "szz", "sxy", "sxz", "syz", "s_mask"]]):
                 # create an indexing variable corresponding to the location of all
                 # the source elements
                 raise NotImplementedError
-                's_source_pos_index = find(source.s_mask != 0);'
+                "s_source_pos_index = find(source.s_mask != 0);"
 
                 # check if the mask is binary or labelled
-                's_unique = unique(source.s_mask);'
+                "s_unique = unique(source.s_mask);"
 
                 # create a second indexing variable
-                if eng.eval('numel(s_unique) <= 2 && sum(s_unique) == 1'):  # noqa: F821
+                if eng.eval("numel(s_unique) <= 2 && sum(s_unique) == 1"):  # noqa: F821
                     # set signal index to all elements
-                    eng.workspace['s_source_sig_index'] = ':'  # noqa: F821
+                    eng.workspace["s_source_sig_index"] = ":"  # noqa: F821
 
                 else:
                     # set signal index to the labels (this allows one input signal
                     # to be used for each source label)
                     s_source_sig_index = source.s_mask(source.s_mask != 0)  # noqa
 
-                f's_source_pos_index = {self.index_data_type}(s_source_pos_index);'
+                f"s_source_pos_index = {self.index_data_type}(s_source_pos_index);"
                 if self.source_s_labelled:
-                    f's_source_sig_index = {self.index_data_type}(s_source_sig_index);'
+                    f"s_source_sig_index = {self.index_data_type}(s_source_sig_index);"
 
         else:
             # ----------------------
             # SOURCE IS A TRANSDUCER
             # ----------------------
 
             # if the sensor is a transducer, check that the simulation is in 3D
-            assert k_dim == 3, 'Transducer inputs are only compatible with 3D simulations.'
+            assert k_dim == 3, "Transducer inputs are only compatible with 3D simulations."
 
             # get the input signal - this is appended with zeros if required to
             # account for the beamforming delays (this will throw an error if the
             # input signal is not defined)
             self.transducer_input_signal = self.source.input_signal
 
             # get the delay mask that accounts for the beamforming delays and
@@ -983,15 +966,15 @@
             self.transducer_source = self.transducer_input_signal.size - delay_mask.max()
 
             # get the active elements mask
             active_elements_mask = self.source.active_elements_mask
 
             # get the apodization mask if not set to 'Rectangular' and convert to a
             # linear array
-            if self.source.transmit_apodization == 'Rectangular':
+            if self.source.transmit_apodization == "Rectangular":
                 self.transducer_transmit_apodization = 1
             else:
                 self.transducer_transmit_apodization = self.source.transmit_apodization_mask
                 self.transducer_transmit_apodization = self.transducer_transmit_apodization[active_elements_mask != 0]
 
             # create indexing variable corresponding to the active elements
             # and convert the data type depending on the number of indices
@@ -1000,15 +983,15 @@
             # convert the delay mask to an indexing variable (this doesn't need to
             # be modified if the grid is expanded) which tells each point in the
             # source mask which point in the input_signal should be used
             delay_mask = matlab_mask(delay_mask, active_elements_mask != 0)  # compatibility
 
             # convert the data type depending on the maximum value of the delay
             # mask and the length of the source
-            smallest_type = get_smallest_possible_type(delay_mask.max(), 'uint')
+            smallest_type = get_smallest_possible_type(delay_mask.max(), "uint")
             if smallest_type is not None:
                 delay_mask = delay_mask.astype(smallest_type)
 
             # move forward by 1 as a delay of 0 corresponds to the first point in the input signal
             self.delay_mask = delay_mask + 1
 
             # clean up unused variables
@@ -1019,41 +1002,46 @@
         Check time-related kWaveGrid inputs
 
         Returns:
             None
         """
 
         # check kgrid for t_array existance, and create if not defined
-        if isinstance(self.kgrid.t_array, str) and self.kgrid.t_array == 'auto':
-
+        if isinstance(self.kgrid.t_array, str) and self.kgrid.t_array == "auto":
             # check for time reversal mode
             if self.time_rev:
-                raise ValueError('kgrid.t_array (Nt and dt) must be defined explicitly in time reversal mode.')
+                raise ValueError("kgrid.t_array (Nt and dt) must be defined explicitly in time reversal mode.")
 
             # check for time varying sources
             if (not self.source_p0_elastic) and (
-                    self.source_p or
-                    self.source_ux or self.source_uy or self.source_uz or
-                    self.source_sxx or self.source_syy or self.source_szz or
-                    self.source_sxy or self.source_sxz or self.source_syz):
-                raise ValueError('kgrid.t_array (Nt and dt) must be defined explicitly when using a time-varying source.')
+                self.source_p
+                or self.source_ux
+                or self.source_uy
+                or self.source_uz
+                or self.source_sxx
+                or self.source_syy
+                or self.source_szz
+                or self.source_sxy
+                or self.source_sxz
+                or self.source_syz
+            ):
+                raise ValueError("kgrid.t_array (Nt and dt) must be defined explicitly when using a time-varying source.")
 
             # create the time array using the compressional sound speed
             self.kgrid.makeTime(self.medium.sound_speed, self.KSPACE_CFL)
 
         # check kgrid.t_array for stability given medium properties
         if not self.options.simulation_type.is_elastic_simulation():
-
             # calculate the largest timestep for which the model is stable
 
             dt_stability_limit = check_stability(self.kgrid, self.medium)
 
             # give a warning if the timestep is larger than stability limit allows
             if self.kgrid.dt > dt_stability_limit:
-                logging.log(logging.WARN, '  time step may be too large for a stable simulation.')
+                logging.log(logging.WARN, "  time step may be too large for a stable simulation.")
 
     @staticmethod
     def select_precision(opt: SimulationOptions):
         """
         Select the minimal precision for storing the data
 
         Args:
@@ -1062,28 +1050,28 @@
         Returns:
             Minimal precision for variable allocation
 
         """
         # set storage variable type based on data_cast - this enables the
         # output variables to be directly created in the data_cast format,
         # rather than creating them in double precision and then casting them
-        if opt.data_cast == 'off':
-            precision = 'double'
-        elif opt.data_cast == 'single':
-            precision = 'single'
-        elif opt.data_cast == 'gsingle':
-            precision = 'single'
-        elif opt.data_cast == 'gdouble':
-            precision = 'double'
-        elif opt.data_cast == 'gpuArray':
+        if opt.data_cast == "off":
+            precision = "double"
+        elif opt.data_cast == "single":
+            precision = "single"
+        elif opt.data_cast == "gsingle":
+            precision = "single"
+        elif opt.data_cast == "gdouble":
+            precision = "double"
+        elif opt.data_cast == "gpuArray":
             raise NotImplementedError("gpuArray is not supported in Python-version")
-        elif opt.data_cast == 'kWaveGPUsingle':
-            precision = 'single'
-        elif opt.data_cast == 'kWaveGPUdouble':
-            precision = 'double'
+        elif opt.data_cast == "kWaveGPUsingle":
+            precision = "single"
+        elif opt.data_cast == "kWaveGPUdouble":
+            precision = "double"
         else:
             raise ValueError("'Unknown ''DataCast'' option'")
         return precision
 
     def check_input_combinations(self, opt: SimulationOptions, user_medium_density_input: bool, k_dim, pml_size, kgrid_N) -> None:
         """
         Check the input combinations for correctness and validity
@@ -1099,57 +1087,59 @@
             None
         """
         # =========================================================================
         # CHECK FOR VALID INPUT COMBINATIONS
         # =========================================================================
 
         # enforce density input if velocity sources or output are being used
-        if not user_medium_density_input and (self.source_ux or
-                                              self.source_uy or
-                                              self.source_uz or
-                                              self.record.u or
-                                              self.record.u_max or
-                                              self.record.u_rms):
-            raise ValueError('medium.density must be explicitly defined '
-                             'if velocity inputs or outputs are used, even in homogeneous media.')
+        if not user_medium_density_input and (
+            self.source_ux or self.source_uy or self.source_uz or self.record.u or self.record.u_max or self.record.u_rms
+        ):
+            raise ValueError(
+                "medium.density must be explicitly defined " "if velocity inputs or outputs are used, even in homogeneous media."
+            )
 
         # TODO(walter): move to check medium
         # enforce density input if nonlinear equations are being used
         if not user_medium_density_input and self.medium.is_nonlinear():
-            raise ValueError('medium.density must be explicitly defined if medium.BonA is specified.')
+            raise ValueError("medium.density must be explicitly defined if medium.BonA is specified.")
 
         # check sensor compatability options for flgs.compute_directivity
-        if self.use_sensor and k_dim == 2 and self.compute_directivity and \
-                not self.binary_sensor_mask and opt.cartesian_interp == 'linear':
-            raise ValueError('sensor directivity fields are only compatible '
-                             'with binary sensor masks or ''CartInterp'' set to ''nearest''.')
+        if self.use_sensor and k_dim == 2 and self.compute_directivity and not self.binary_sensor_mask and opt.cartesian_interp == "linear":
+            raise ValueError(
+                "sensor directivity fields are only compatible " "with binary sensor masks or " "CartInterp" " set to " "nearest" "."
+            )
 
         # check for split velocity output
         if self.record.u_split_field and not self.binary_sensor_mask:
-            raise ValueError('The option sensor.record = {''u_split_field''} is only compatible '
-                             'with a binary sensor mask.')
+            raise ValueError("The option sensor.record = {" "u_split_field" "} is only compatible " "with a binary sensor mask.")
 
         # check input options for data streaming *****
         if opt.stream_to_disk:
             if not self.use_sensor or self.time_rev:
                 raise ValueError(
-                    'The optional input ''StreamToDisk'' is currently only compatible '
-                    'with forward simulations using a non-zero sensor mask.')
+                    "The optional input "
+                    "StreamToDisk"
+                    " is currently only compatible "
+                    "with forward simulations using a non-zero sensor mask."
+                )
             elif self.sensor.record is not None and self.sensor.record.ismember(self.record.flags[1:]).any():
-                raise ValueError('The optional input ''StreamToDisk'' is currently only compatible '
-                                 'with sensor.record = {''p''} (the default).')
+                raise ValueError(
+                    "The optional input " "StreamToDisk" " is currently only compatible " "with sensor.record = {" "p" "} (the default)."
+                )
 
         is_axisymmetric = self.options.simulation_type.is_axisymmetric()
         # make sure the PML size is smaller than the grid if PMLInside is true
         if opt.pml_inside and (
-                (k_dim == 1 and ((pml_size.x * 2 > self.kgrid.Nx))) or
-                (k_dim == 2 and not is_axisymmetric and ((pml_size.x * 2 > kgrid_N[0]) or (pml_size.y * 2 > kgrid_N[1]))) or
-                (k_dim == 2 and is_axisymmetric and ((pml_size.x * 2 > kgrid_N[0]) or (pml_size.y > kgrid_N[1]))) or
-                (k_dim == 3 and ((pml_size.x*2 > kgrid_N[0]) or (pml_size.x*2 > kgrid_N[1]) or (pml_size.z * 2 > kgrid_N[2]) ))):
-            raise ValueError('The size of the PML must be smaller than the size of the grid.')
+            (k_dim == 1 and (pml_size.x * 2 > self.kgrid.Nx))
+            or (k_dim == 2 and not is_axisymmetric and ((pml_size.x * 2 > kgrid_N[0]) or (pml_size.y * 2 > kgrid_N[1])))
+            or (k_dim == 2 and is_axisymmetric and ((pml_size.x * 2 > kgrid_N[0]) or (pml_size.y > kgrid_N[1])))
+            or (k_dim == 3 and ((pml_size.x * 2 > kgrid_N[0]) or (pml_size.x * 2 > kgrid_N[1]) or (pml_size.z * 2 > kgrid_N[2])))
+        ):
+            raise ValueError("The size of the PML must be smaller than the size of the grid.")
 
         # make sure the PML is inside if using a non-uniform grid
         if self.nonuniform_grid and not opt.pml_inside:
             raise ValueError("''PMLInside'' must be true for simulations using non-uniform grids.")
 
         # check for compatible input options if saving to disk
         # modified by Farid | disabled temporarily!
@@ -1157,41 +1147,42 @@
         #                   (not self.use_sensor or not self.binary_sensor_mask or self.time_rev):
         #     raise ValueError('The optional input ''SaveToDisk'' is currently only compatible
         #                       with forward simulations using a non-zero binary sensor mask.')
 
         # check the record start time is within range
         record_start_index = self.sensor.record_start_index
         if self.use_sensor and ((record_start_index > self.kgrid.Nt) or (record_start_index < 1)):
-            raise ValueError('sensor.record_start_index must be between 1 and the number of time steps.')
+            raise ValueError("sensor.record_start_index must be between 1 and the number of time steps.")
 
         # ensure 'WSWA' symmetry if using axisymmetric code with 'SaveToDisk'
-        if is_axisymmetric and self.options.radial_symmetry != 'WSWA' and isinstance(self.options.save_to_disk, str):
-
+        if is_axisymmetric and self.options.radial_symmetry != "WSWA" and isinstance(self.options.save_to_disk, str):
             # display a warning only if using WSWS symmetry (not WSWA-FFT)
-            if self.options.radial_symmetry.startswith('WSWS'):
-                logging.log(logging.WARN,  '  Optional input ''RadialSymmetry'' changed to ''WSWA'' for compatability with ''SaveToDisk''.')
+            if self.options.radial_symmetry.startswith("WSWS"):
+                logging.log(
+                    logging.WARN, "  Optional input " "RadialSymmetry" " changed to " "WSWA" " for compatability with " "SaveToDisk" "."
+                )
 
             # update setting
-            self.options.radial_symmetry = 'WSWA'
+            self.options.radial_symmetry = "WSWA"
 
         # ensure p0 smoothing is switched off if p0 is empty
         if not self.source_p0:
             self.options.smooth_p0 = False
 
         # start log if required
         if opt.create_log:
             raise NotImplementedError(f"diary({self.LOG_NAME}.txt');")
 
         # update command line status
         if self.time_rev:
-            logging.log(logging.INFO, '  time reversal mode')
+            logging.log(logging.INFO, "  time reversal mode")
 
         # cleanup unused variables
         for k in list(self.__dict__.keys()):
-            if k.endswith('_DEF'):
+            if k.endswith("_DEF"):
                 delattr(self, k)
 
     def smooth_and_enlarge(self, source, k_dim, kgrid_N, opt: SimulationOptions) -> None:
         """
         Smooth and enlarge grids
 
         Args:
@@ -1209,205 +1200,212 @@
         #   NOTE 1: if p0 has any values at the edge of the domain, the smoothing
         #   may cause part of p0 to wrap to the other side of the domain
         #   NOTE 2: p0 is smoothed before the grid is expanded to ensure that p0 is
         #   exactly zero within the PML
         #   NOTE 3: for the axisymmetric code, p0 is smoothed assuming WS origin
         #   symmetry
         if self.source_p0 and self.options.smooth_p0:
-
             # update command line status
-            logging.log(logging.INFO, '  smoothing p0 distribution...')
+            logging.log(logging.INFO, "  smoothing p0 distribution...")
 
             if self.options.simulation_type.is_axisymmetric():
-                if self.options.radial_symmetry in ['WSWA-FFT', 'WSWA']:
+                if self.options.radial_symmetry in ["WSWA-FFT", "WSWA"]:
                     # create a new kWave grid object with expanded radial grid
                     kgrid_exp = kWaveGrid([kgrid_N.x, kgrid_N.y * 4], [self.kgrid.dx, self.kgrid.dy])
 
                     # mirror p0 in radial dimension using WSWA symmetry
                     self.source.p0 = self.source.p0.astype(float)
                     p0_exp = np.zeros((kgrid_exp.Nx, kgrid_exp.Ny))
-                    p0_exp[:, kgrid_N.y*0 + 0:kgrid_N.y*1] =            self.source.p0
-                    p0_exp[:, kgrid_N.y*1 + 1:kgrid_N.y*2] = -np.fliplr(self.source.p0[:, 1:])
-                    p0_exp[:, kgrid_N.y*2 + 0:kgrid_N.y*3] =           -self.source.p0
-                    p0_exp[:, kgrid_N.y*3 + 1:kgrid_N.y*4] =  np.fliplr(self.source.p0[:, 1:])
+                    p0_exp[:, kgrid_N.y * 0 + 0 : kgrid_N.y * 1] = self.source.p0
+                    p0_exp[:, kgrid_N.y * 1 + 1 : kgrid_N.y * 2] = -np.fliplr(self.source.p0[:, 1:])
+                    p0_exp[:, kgrid_N.y * 2 + 0 : kgrid_N.y * 3] = -self.source.p0
+                    p0_exp[:, kgrid_N.y * 3 + 1 : kgrid_N.y * 4] = np.fliplr(self.source.p0[:, 1:])
 
-                elif self.options.radial_symmetry in ['WSWS-FFT', 'WSWS']:
+                elif self.options.radial_symmetry in ["WSWS-FFT", "WSWS"]:
                     # create a new kWave grid object with expanded radial grid
                     kgrid_exp = kWaveGrid([kgrid_N.x, kgrid_N.y * 2 - 2], [self.kgrid.dx, self.kgrid.dy])
 
                     # mirror p0 in radial dimension using WSWS symmetry
                     p0_exp = np.zeros((kgrid_exp.Nx, kgrid_exp.Ny))
-                    p0_exp[:, 1:kgrid_N.y]              = source.p0
-                    p0_exp[:, kgrid_N.y + 0:kgrid_N.y*2 - 2] = np.fliplr(source.p0[:, 1:-1])
+                    p0_exp[:, 1 : kgrid_N.y] = source.p0
+                    p0_exp[:, kgrid_N.y + 0 : kgrid_N.y * 2 - 2] = np.fliplr(source.p0[:, 1:-1])
 
                 # smooth p0
                 p0_exp = smooth(p0_exp, True)
 
                 # trim back to original size
-                source.p0 = p0_exp[:, 0:self.kgrid.Ny]
+                source.p0 = p0_exp[:, 0 : self.kgrid.Ny]
 
                 # clean up unused variables
                 del kgrid_exp
                 del p0_exp
             else:
                 source.p0 = smooth(source.p0, True)
 
         # expand the computational grid if the PML is set to be outside the input
         # grid defined by the user
         if opt.pml_inside is False:
             expand_results = expand_grid_matrices(
-                self.kgrid, self.medium, self.source, self.sensor, self.options,
-                dotdict({
-                    'p_source_pos_index': self.p_source_pos_index,
-                    'u_source_pos_index': self.u_source_pos_index,
-                    's_source_pos_index': self.s_source_pos_index,
-                }),
-                dotdict({
-                    'axisymmetric': self.options.simulation_type.is_axisymmetric(),
-                    'use_sensor': self.use_sensor,
-                    'blank_sensor': self.blank_sensor,
-                    'cuboid_corners': self.cuboid_corners,
-
-                    'source_p0': self.source_p0,
-                    'source_p': self.source_p,
-
-                    'source_ux': self.source_ux,
-                    'source_uy': self.source_uy,
-                    'source_uz': self.source_uz,
-
-                    'transducer_source': self.transducer_source,
-
-                    'source_sxx': self.source_sxx,
-                    'source_syy': self.source_syy,
-                    'source_szz': self.source_szz,
-                    'source_sxy': self.source_sxy,
-                    'source_sxz': self.source_sxz,
-                    'source_syz': self.source_syz
-                })
+                self.kgrid,
+                self.medium,
+                self.source,
+                self.sensor,
+                self.options,
+                dotdict(
+                    {
+                        "p_source_pos_index": self.p_source_pos_index,
+                        "u_source_pos_index": self.u_source_pos_index,
+                        "s_source_pos_index": self.s_source_pos_index,
+                    }
+                ),
+                dotdict(
+                    {
+                        "axisymmetric": self.options.simulation_type.is_axisymmetric(),
+                        "use_sensor": self.use_sensor,
+                        "blank_sensor": self.blank_sensor,
+                        "cuboid_corners": self.cuboid_corners,
+                        "source_p0": self.source_p0,
+                        "source_p": self.source_p,
+                        "source_ux": self.source_ux,
+                        "source_uy": self.source_uy,
+                        "source_uz": self.source_uz,
+                        "transducer_source": self.transducer_source,
+                        "source_sxx": self.source_sxx,
+                        "source_syy": self.source_syy,
+                        "source_szz": self.source_szz,
+                        "source_sxy": self.source_sxy,
+                        "source_sxz": self.source_sxz,
+                        "source_syz": self.source_syz,
+                    }
+                ),
             )
-            self.kgrid, self.index_data_type, self.p_source_pos_index, \
-                self.u_source_pos_index, self.s_source_pos_index = expand_results
+            self.kgrid, self.index_data_type, self.p_source_pos_index, self.u_source_pos_index, self.s_source_pos_index = expand_results
 
         # get maximum prime factors
         if self.options.simulation_type.is_axisymmetric():
             prime_facs = self.kgrid.highest_prime_factors(self.options.radial_symmetry[:4])
         else:
             prime_facs = self.kgrid.highest_prime_factors()
 
         # give warning for bad dimension sizes
         if prime_facs.max() > self.HIGHEST_PRIME_FACTOR_WARNING:
             prime_facs = prime_facs[prime_facs != 0]
-            logging.log(logging.WARN, f'Highest prime factors in each dimension are {prime_facs}')
-            logging.log(logging.WARN, 'Use dimension sizes with lower prime factors to improve speed')
+            logging.log(logging.WARN, f"Highest prime factors in each dimension are {prime_facs}")
+            logging.log(logging.WARN, "Use dimension sizes with lower prime factors to improve speed")
         del prime_facs
 
         # smooth the sound speed distribution if required
         if opt.smooth_c0 and num_dim2(self.medium.sound_speed) == k_dim and self.medium.sound_speed.size > 1:
-            logging.log(logging.INFO, '  smoothing sound speed distribution...')
+            logging.log(logging.INFO, "  smoothing sound speed distribution...")
             self.medium.sound_speed = smooth(self.medium.sound_speed)
 
         # smooth the ambient density distribution if required
         if opt.smooth_rho0 and num_dim2(self.medium.density) == k_dim and self.medium.density.size > 1:
-            logging.log(logging.INFO, 'smoothing density distribution...')
+            logging.log(logging.INFO, "smoothing density distribution...")
             self.medium.density = smooth(self.medium.density)
 
     def create_sensor_variables(self) -> None:
         """
         Create the sensor related variables
 
         Returns:
             None
         """
         # define the output variables and mask indices if using the sensor
         if self.use_sensor:
             if not self.blank_sensor or isinstance(self.options.save_to_disk, str):
                 if self.cuboid_corners:
-
                     # create empty list of sensor indices
                     self.sensor_mask_index = []
 
                     # loop through the list of cuboid corners, and extract the
                     # sensor mask indices for each cube
                     for cuboid_index in range(self.record.cuboid_corners_list.shape[1]):
-
                         # create empty binary mask
                         temp_mask = np.zeros_like(self.kgrid.k, dtype=bool)
 
                         if self.kgrid.dim == 1:
                             self.sensor.mask[
-                            self.record.cuboid_corners_list[0, cuboid_index]:self.record.cuboid_corners_list[1, cuboid_index]
+                                self.record.cuboid_corners_list[0, cuboid_index] : self.record.cuboid_corners_list[1, cuboid_index]
                             ] = 1
                         if self.kgrid.dim == 2:
                             self.sensor.mask[
-                            self.record.cuboid_corners_list[0, cuboid_index]:self.record.cuboid_corners_list[2, cuboid_index],
-                            self.record.cuboid_corners_list[1, cuboid_index]:self.record.cuboid_corners_list[3, cuboid_index]
+                                self.record.cuboid_corners_list[0, cuboid_index] : self.record.cuboid_corners_list[2, cuboid_index],
+                                self.record.cuboid_corners_list[1, cuboid_index] : self.record.cuboid_corners_list[3, cuboid_index],
                             ] = 1
                         if self.kgrid.dim == 3:
                             self.sensor.mask[
-                            self.record.cuboid_corners_list[0, cuboid_index]:self.record.cuboid_corners_list[3, cuboid_index],
-                            self.record.cuboid_corners_list[1, cuboid_index]:self.record.cuboid_corners_list[4, cuboid_index],
-                            self.record.cuboid_corners_list[2, cuboid_index]:self.record.cuboid_corners_list[5, cuboid_index]
+                                self.record.cuboid_corners_list[0, cuboid_index] : self.record.cuboid_corners_list[3, cuboid_index],
+                                self.record.cuboid_corners_list[1, cuboid_index] : self.record.cuboid_corners_list[4, cuboid_index],
+                                self.record.cuboid_corners_list[2, cuboid_index] : self.record.cuboid_corners_list[5, cuboid_index],
                             ] = 1
 
                         # extract mask indices
                         self.sensor_mask_index.append(matlab_find(temp_mask))
                     self.sensor_mask_index = np.array(self.sensor_mask_index)
 
                     # cleanup unused variables
                     del temp_mask
 
                 else:
                     # create mask indices (this works for both normal sensor and
                     # transducer inputs)
-                    self.sensor_mask_index = np.where(self.sensor.mask.flatten(order='F') != 0)[0] + 1  # +1 due to matlab indexing
+                    self.sensor_mask_index = np.where(self.sensor.mask.flatten(order="F") != 0)[0] + 1  # +1 due to matlab indexing
                     self.sensor_mask_index = np.expand_dims(self.sensor_mask_index, -1)  # compatibility, n => [n, 1]
 
                 # convert the data type depending on the number of indices (this saves
                 # memory)
                 self.sensor_mask_index = cast_to_type(self.sensor_mask_index, self.index_data_type)
 
             else:
                 # set the sensor mask index variable to be empty
                 self.sensor_mask_index = []
 
         # run subscript to create storage variables if not saving to disk
         # TODO (Walter): this case is very broken but save to disk is currently always true!
         if self.use_sensor and not self.options.save_to_disk:
             result = create_storage_variables(
-                self.kgrid, self.sensor, self.options,
-                dotdict({
-                    'binary_sensor_mask': self.binary_sensor_mask,
-                    'time_rev': self.time_rev,
-                    'blank_sensor': self.blank_sensor,
-                    'record_u_split_field': self.record_u_split_field,
-                    'axisymmetric': self.options.simulation_type.is_axisymmetric(),
-                    'reorder_data': self.reorder_data,
-                }),
-                dotdict({
-                    'sensor_x': self.sensor.x,
-                    'sensor_mask_index': self.sensor.mask_index,
-                    'record': self.record,
-                    'sensor_data_buffer_size': self.sensor.data_buffer_size,
-                })
+                self.kgrid,
+                self.sensor,
+                self.options,
+                dotdict(
+                    {
+                        "binary_sensor_mask": self.binary_sensor_mask,
+                        "time_rev": self.time_rev,
+                        "blank_sensor": self.blank_sensor,
+                        "record_u_split_field": self.record_u_split_field,
+                        "axisymmetric": self.options.simulation_type.is_axisymmetric(),
+                        "reorder_data": self.reorder_data,
+                    }
+                ),
+                dotdict(
+                    {
+                        "sensor_x": self.sensor.x,
+                        "sensor_mask_index": self.sensor.mask_index,
+                        "record": self.record,
+                        "sensor_data_buffer_size": self.sensor.data_buffer_size,
+                    }
+                ),
             )
-            self.binary_sensor_mask                 = result.binary_sensor_mask
-            self.reorder_data                       = result.reorder_data
+            self.binary_sensor_mask = result.binary_sensor_mask
+            self.reorder_data = result.reorder_data
             self.transducer_receive_elevation_focus = result.transducer_receive_elevation_focus
 
     def create_absorption_vars(self) -> None:
         """
         Create absorption variables for the fluid code based on
         the expanded and smoothed values of the medium parameters (if not saving to disk)
 
         Returns:
             None
         """
         if not self.options.simulation_type.is_elastic_simulation() and not self.options.save_to_disk:
-            self.absorb_nabla1, self.absorb_nabla2, self.absorb_tau, self.absorb_eta = \
-                create_absorption_variables(self.kgrid, self.medium, self.equation_of_state)
+            self.absorb_nabla1, self.absorb_nabla2, self.absorb_tau, self.absorb_eta = create_absorption_variables(
+                self.kgrid, self.medium, self.equation_of_state
+            )
 
     def assign_pseudonyms(self, medium: kWaveMedium, kgrid: kWaveGrid) -> None:
         """
         Shorten commonly used field names (these act only as pointers provided that the values aren't modified)
         (done after enlarging and smoothing the grids)
 
         Args:
@@ -1445,34 +1443,41 @@
 
         try:
             u_source_pos_index = self.u_source_pos_index
         except AttributeError:
             u_source_pos_index = None
 
         self.transducer_input_signal = scale_source_terms_func(
-            self.c0, self.dt, self.kgrid, self.source,
-            p_source_pos_index, s_source_pos_index, u_source_pos_index, self.transducer_input_signal,
-            dotdict({
-                'nonuniform_grid': self.nonuniform_grid,
-                'source_ux': self.source_ux,
-                'source_uy': self.source_uy,
-                'source_uz': self.source_uz,
-                'transducer_source': self.transducer_source,
-                'source_p': self.source_p,
-                'source_p0': self.source_p0,
-                'use_w_source_correction_p': self.use_w_source_correction_p,
-                'use_w_source_correction_u': self.use_w_source_correction_u,
-
-                'source_sxx': self.source_sxx,
-                'source_syy': self.source_syy,
-                'source_szz': self.source_szz,
-                'source_sxy': self.source_sxy,
-                'source_sxz': self.source_sxz,
-                'source_syz': self.source_syz,
-            })
+            self.c0,
+            self.dt,
+            self.kgrid,
+            self.source,
+            p_source_pos_index,
+            s_source_pos_index,
+            u_source_pos_index,
+            self.transducer_input_signal,
+            dotdict(
+                {
+                    "nonuniform_grid": self.nonuniform_grid,
+                    "source_ux": self.source_ux,
+                    "source_uy": self.source_uy,
+                    "source_uz": self.source_uz,
+                    "transducer_source": self.transducer_source,
+                    "source_p": self.source_p,
+                    "source_p0": self.source_p0,
+                    "use_w_source_correction_p": self.use_w_source_correction_p,
+                    "use_w_source_correction_u": self.use_w_source_correction_u,
+                    "source_sxx": self.source_sxx,
+                    "source_syy": self.source_syy,
+                    "source_szz": self.source_szz,
+                    "source_sxy": self.source_sxy,
+                    "source_sxz": self.source_sxz,
+                    "source_syz": self.source_syz,
+                }
+            ),
         )
 
     def create_pml_indices(self, kgrid_dim, kgrid_N: Vector, pml_size, pml_inside, is_axisymmetric):
         """
         Define index variables to remove the PML from the display if the optional
         input 'PlotPML' is set to false
```

### Comparing `k_wave_python-0.3.2/kwave/kgrid.py` & `k_wave_python-0.3.3/kwave/kgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     of the kWaveGrid class contains the grid coordinates and wavenumber
     matrices used within the simulation and reconstruction functions in
     k-Wave. The grid matrices are indexed as: (x, 1) in 1D; (x, y) in
     2D; and (x, y, z) in 3D. The grid is assumed to be a regularly spaced
     Cartesian grid, with grid spacing given by dx, dy, dz (typically the
     grid spacing in each direction is constant).
     """
+
     # default CFL number
     CFL_DEFAULT = 0.3
 
     # machine precision
     MACHINE_PRECISION = 100 * sys.float_info.epsilon
 
     def __init__(self, N, spacing):
@@ -34,31 +35,31 @@
             spacing: grid point spacing in each direction [m]
         """
         N, spacing = np.atleast_1d(N), np.atleast_1d(spacing)  # if inputs are lists
         assert N.ndim == 1 and spacing.ndim == 1  # ensure no multidimensional lists
         assert (1 <= N.size <= 3) and (1 <= spacing.size <= 3)  # ensure valid dimensionality
         assert N.size == spacing.size, "Size list N and spacing list do not have the same size."
 
-        self.N = N.astype(int)              #: grid size in each dimension [grid points]
-        self.spacing = spacing              #: grid point spacing in each direction [m]
-        self.dim = self.N.size              #: Number of dimensions (1, 2 or 3)
-
-        self.nonuniform = False             #: flag that indicates grid non-uniformity
-        self.dt = 'auto'                    #: size of time step [s]
-        self.Nt = 'auto'                    #: number of time steps [s]
+        self.N = N.astype(int)  #: grid size in each dimension [grid points]
+        self.spacing = spacing  #: grid point spacing in each direction [m]
+        self.dim = self.N.size  #: Number of dimensions (1, 2 or 3)
+
+        self.nonuniform = False  #: flag that indicates grid non-uniformity
+        self.dt = "auto"  #: size of time step [s]
+        self.Nt = "auto"  #: number of time steps [s]
 
         # originally there was [xn_vec, yn_vec, zn_vec]
-        self.n_vec      = FlexibleVector([0] * self.dim)  #: position vectors for the grid points in [0, 1]
+        self.n_vec = FlexibleVector([0] * self.dim)  #: position vectors for the grid points in [0, 1]
         # originally there was [xn_vec_sgx, yn_vec_sgy, zn_vec_sgz]
-        self.n_vec_sg   = FlexibleVector([0] * self.dim)  #: position vectors for the staggered grid points in [0, 1]
+        self.n_vec_sg = FlexibleVector([0] * self.dim)  #: position vectors for the staggered grid points in [0, 1]
 
         # originally there was [dxudxn, dyudyn, dzudzn]
-        self.dudn       = FlexibleVector([0] * self.dim)  #: transformation gradients between uniform and staggered grids
+        self.dudn = FlexibleVector([0] * self.dim)  #: transformation gradients between uniform and staggered grids
         # originally there was [dxudxn_sgx, dyudyn_sgy, dzudzn_sgz]
-        self.dudn_sg    = FlexibleVector([0] * self.dim)  #: transformation gradients between uniform and staggered grids
+        self.dudn_sg = FlexibleVector([0] * self.dim)  #: transformation gradients between uniform and staggered grids
 
         # assign the grid parameters for the x spatial direction
         # originally kx_vec
         self.k_vec = FlexibleVector([self.makeDim(self.Nx, self.dx)])  #: Nx x 1 vector of wavenumber components in the x-direction [rad/m]
 
         if self.dim == 1:
             # define the scalar wavenumber based on the wavenumber components
@@ -92,44 +93,43 @@
     def t_array(self):
         """
         time array [s]
         """
         # TODO (walter): I would change this functionality to return a time array even if Nt or dt are not yet set
         #  (e.g. if they are still 'auto')
 
-        if self.Nt == 'auto' or self.dt == 'auto':
-            return 'auto'
+        if self.Nt == "auto" or self.dt == "auto":
+            return "auto"
         else:
             t_array = np.arange(0, self.Nt) * self.dt
             # TODO: adding this extra dimension seems unnecessary
             # This leads to an extra squeeze when plotting e.g. in example "array as sensor" on lines 110 and 111
             return np.expand_dims(t_array, axis=0)
 
     @t_array.setter
     def t_array(self, t_array):
         # check for 'auto' input
-        if t_array == 'auto':
+        if t_array == "auto":
             # set values to auto
-            self.Nt = 'auto'
-            self.dt = 'auto'
+            self.Nt = "auto"
+            self.dt = "auto"
 
         else:
             # extract property values
             Nt_temp = t_array.size
             dt_temp = t_array[1] - t_array[0]
 
             # check the time array begins at zero
-            assert t_array[0] == 0, 't_array must begin at zero.'
+            assert t_array[0] == 0, "t_array must begin at zero."
 
             # check the time array is evenly spaced
-            assert (t_array[1:] - t_array[0:-1] - dt_temp).max() < self.MACHINE_PRECISION, \
-                't_array must be evenly spaced.'
+            assert (t_array[1:] - t_array[0:-1] - dt_temp).max() < self.MACHINE_PRECISION, "t_array must be evenly spaced."
 
             # check the time steps are increasing
-            assert dt_temp > 0, 't_array must be monotonically increasing.'
+            assert dt_temp > 0, "t_array must be monotonically increasing."
 
             # assign values
             self.Nt = Nt_temp
             self.dt = dt_temp
 
     def setTime(self, Nt, dt) -> None:
         """
@@ -138,20 +138,20 @@
         Args:
             Nt:
             dt:
 
         Returns: None
         """
         # check the value for Nt
-        assert (isinstance(Nt, int) or
-                np.issubdtype(Nt, np.int64) or
-                np.issubdtype(Nt, np.int32)) and Nt > 0, 'Nt must be a positive integer.'
+        assert (
+            isinstance(Nt, int) or np.issubdtype(Nt, np.int64) or np.issubdtype(Nt, np.int32)
+        ) and Nt > 0, "Nt must be a positive integer."
 
         # check the value for dt
-        assert dt > 0, 'dt must be positive.'
+        assert dt > 0, "dt must be positive."
 
         # assign values
         self.Nt = Nt
         self.dt = dt
 
     @property
     def Nx(self):
@@ -437,28 +437,22 @@
             axisymmetric: Axisymmetric code or None
 
         Returns:
             Vector of three elements
         """
         # import statement place here in order to avoid circular dependencies
         if axisymmetric is not None:
-            if axisymmetric == 'WSWA':
-                prime_facs = [largest_prime_factor(self.Nx),
-                              largest_prime_factor(self.Ny * 4),
-                              largest_prime_factor(self.Nz)]
-            elif axisymmetric == 'WSWS':
-                prime_facs = [largest_prime_factor(self.Nx),
-                              largest_prime_factor(self.Ny * 2 - 2),
-                              largest_prime_factor(self.Nz)]
+            if axisymmetric == "WSWA":
+                prime_facs = [largest_prime_factor(self.Nx), largest_prime_factor(self.Ny * 4), largest_prime_factor(self.Nz)]
+            elif axisymmetric == "WSWS":
+                prime_facs = [largest_prime_factor(self.Nx), largest_prime_factor(self.Ny * 2 - 2), largest_prime_factor(self.Nz)]
             else:
-                raise ValueError('Unknown axisymmetric symmetry.')
+                raise ValueError("Unknown axisymmetric symmetry.")
         else:
-            prime_facs = [largest_prime_factor(self.Nx),
-                          largest_prime_factor(self.Ny),
-                          largest_prime_factor(self.Nz)]
+            prime_facs = [largest_prime_factor(self.Nx), largest_prime_factor(self.Ny), largest_prime_factor(self.Nz)]
         return np.array(prime_facs)
 
     # TODO (walter): convert this name to snake case
     def makeTime(self, c, cfl=CFL_DEFAULT, t_end=None):
         """
         Compute Nt and dt based on the cfl number and grid size, where
         the number of time-steps is chosen based on the time it takes to
@@ -584,16 +578,15 @@
             n = np.arange(1, M // 2).T
             kx_vec = 2 * math.pi * n / (M * dx)
         elif dtt_type == DiscreteSine.TYPE_2:
             # whole-wavenumber DTT
             # HAHA / DST-II
             n = np.arange(1, M // 2 + 1).T
             kx_vec = 2 * math.pi * n / (M * dx)
-        elif dtt_type in [DiscreteCosine.TYPE_3, DiscreteCosine.TYPE_4,
-                          DiscreteSine.TYPE_3,   DiscreteSine.TYPE_4]:
+        elif dtt_type in [DiscreteCosine.TYPE_3, DiscreteCosine.TYPE_4, DiscreteSine.TYPE_3, DiscreteSine.TYPE_4]:
             # half-wavenumber DTTs
             # WSWA / DCT-III
             # HSHA / DCT-IV
             # WAWS / DST-III
             # HAHS / DST-IV
             n = np.arange(0, M // 2).T
             kx_vec = 2 * math.pi * (n + 0.5) / (M * dx)
@@ -618,30 +611,30 @@
             dudn_sg:
 
         Returns:
 
         """
 
         # check the dimension to set the nonuniform grid is appropriate
-        assert dim <= self.dim, f'Cannot set nonuniform parameters for dimension {dim} of {self.dim}-dimensional grid.'
+        assert dim <= self.dim, f"Cannot set nonuniform parameters for dimension {dim} of {self.dim}-dimensional grid."
 
         # force non-uniform grid spacing to be column vectors, and the
         # gradients to be in the correct direction for use with bsxfun
-        n_vec            = np.reshape(n_vec,    (-1, 1), order='F')
-        n_vec_sg         = np.reshape(n_vec_sg, (-1, 1), order='F')
+        n_vec = np.reshape(n_vec, (-1, 1), order="F")
+        n_vec_sg = np.reshape(n_vec_sg, (-1, 1), order="F")
 
         if dim == 1:
-            dudn         = np.reshape(dudn,     (-1, 1), order='F')
-            dudn_sg      = np.reshape(dudn_sg,  (-1, 1), order='F')
+            dudn = np.reshape(dudn, (-1, 1), order="F")
+            dudn_sg = np.reshape(dudn_sg, (-1, 1), order="F")
         elif dim == 2:
-            dudn         = np.reshape(dudn,     (1, -1), order='F')
-            dudn_sg      = np.reshape(dudn_sg,  (1, -1), order='F')
+            dudn = np.reshape(dudn, (1, -1), order="F")
+            dudn_sg = np.reshape(dudn_sg, (1, -1), order="F")
         elif dim == 3:
-            dudn         = np.reshape(dudn,     (1, 1, -1), order='F')
-            dudn_sg      = np.reshape(dudn_sg,  (1, 1, -1), order='F')
+            dudn = np.reshape(dudn, (1, 1, -1), order="F")
+            dudn_sg = np.reshape(dudn_sg, (1, 1, -1), order="F")
 
         self.n_vec.assign_dim(self.dim, n_vec)
         self.n_vec_sg.assign_dim(self.dim, n_vec_sg)
 
         self.dudn.assign_dim(self.dim, dudn)
         self.dudn_sg.assign_dim(self.dim, dudn_sg)
 
@@ -667,15 +660,15 @@
             dtt_type:
 
         Returns:
 
         """
         # check dtt_type is a scalar or a vector the same size self.dim
         dtt_type = np.array(dtt_type)
-        assert (dtt_type.size in [1, self.dim]), f'dtt_type must be a scalar, or {self.dim}D vector'
+        assert dtt_type.size in [1, self.dim], f"dtt_type must be a scalar, or {self.dim}D vector"
         if self.dim == 1:
             k, M = self.kx_vec_dtt(dtt_type[0])
             return k, M
         elif self.dim == 2:
             # assign the grid parameters for the x and y spatial directions
             kx_vec_dtt, Mx = self.kx_vec_dtt(dtt_type[0])
             ky_vec_dtt, My = self.ky_vec_dtt(dtt_type[-1])
```

### Comparing `k_wave_python-0.3.2/kwave/kmedium.py` & `k_wave_python-0.3.3/kwave/kmedium.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,76 +6,79 @@
 
 import kwave.utils.checks
 
 
 @dataclass
 class kWaveMedium(object):
     # sound speed distribution within the acoustic medium [m/s] | required to be defined
-    sound_speed                 : np.array
+    sound_speed: np.array
     # reference sound speed used within the k-space operator (phase correction term) [m/s]
-    sound_speed_ref             : np.array = None
+    sound_speed_ref: np.array = None
     # density distribution within the acoustic medium [kg/m^3]
-    density                     : np.array = None
+    density: np.array = None
     # power law absorption coefficient [dB/(MHz^y cm)]
-    alpha_coeff                 : np.array = None
+    alpha_coeff: np.array = None
     # power law absorption exponent
-    alpha_power                 : np.array = None
+    alpha_power: np.array = None
     # optional input to force either the absorption or dispersion terms in the equation of state to be excluded;
     # valid inputs are 'no_absorption' or 'no_dispersion'
-    alpha_mode                  : np.array = None
+    alpha_mode: np.array = None
     # frequency domain filter applied to the absorption and dispersion terms in the equation of state
-    alpha_filter                : np.array = None
+    alpha_filter: np.array = None
     # two element array used to control the sign of absorption and dispersion terms in the equation of state
-    alpha_sign                  : np.array = None
+    alpha_sign: np.array = None
     # parameter of nonlinearity
-    BonA                        : np.array = None
+    BonA: np.array = None
     # is the medium absorbing?
-    absorbing                   : bool     = False
+    absorbing: bool = False
     # is the medium absorbing stokes?
-    stokes                      : bool     = False
+    stokes: bool = False
 
-   #  """
-   #     Note: For heterogeneous medium parameters, medium.sound_speed and
-   #     medium.density must be given in matrix form with the same dimensions as
-   #     kgrid. For homogeneous medium parameters, these can be given as single
-   #     numeric values. If the medium is homogeneous and velocity inputs or
-   #     outputs are not required, it is not necessary to specify medium.density.
-   # """
+    #  """
+    #     Note: For heterogeneous medium parameters, medium.sound_speed and
+    #     medium.density must be given in matrix form with the same dimensions as
+    #     kgrid. For homogeneous medium parameters, these can be given as single
+    #     numeric values. If the medium is homogeneous and velocity inputs or
+    #     outputs are not required, it is not necessary to specify medium.density.
+    # """
 
     def __post_init__(self):
-        self.sound_speed                    = np.atleast_1d(self.sound_speed)
+        self.sound_speed = np.atleast_1d(self.sound_speed)
 
     def check_fields(self, kgrid_shape: np.ndarray) -> None:
         """
         Check whether the given properties are valid
 
         Args:
             kgrid_shape: Shape of the kWaveGrid
 
         Returns:
             None
         """
         # check the absorption mode input is valid
         if self.alpha_mode is not None:
-            assert self.alpha_mode in ['no_absorption', 'no_dispersion', 'stokes'], \
-                "medium.alpha_mode must be set to 'no_absorption', 'no_dispersion', or 'stokes'."
+            assert self.alpha_mode in [
+                "no_absorption",
+                "no_dispersion",
+                "stokes",
+            ], "medium.alpha_mode must be set to 'no_absorption', 'no_dispersion', or 'stokes'."
 
         # check the absorption filter input is valid
         if self.alpha_filter is not None and not (self.alpha_filter.shape == kgrid_shape).all():
-            raise ValueError('medium.alpha_filter must be the same size as the computational grid.')
+            raise ValueError("medium.alpha_filter must be the same size as the computational grid.")
 
         # check the absorption sign input is valid
-        if self.alpha_sign is not None and \
-                (not kwave.utils.checkutils.is_number(self.alpha_sign) or (self.alpha_sign.size != 2)):
-            raise ValueError('medium.alpha_sign must be given as a '
-                             '2 element numerical array controlling absorption and dispersion, respectively.')
+        if self.alpha_sign is not None and (not kwave.utils.checkutils.is_number(self.alpha_sign) or (self.alpha_sign.size != 2)):
+            raise ValueError(
+                "medium.alpha_sign must be given as a " "2 element numerical array controlling absorption and dispersion, respectively."
+            )
 
         # check alpha_coeff is non-negative and real
         if not np.all(np.isreal(self.alpha_coeff)) or np.any(self.alpha_coeff < 0):
-            raise ValueError('medium.alpha_coeff must be non-negative and real.')
+            raise ValueError("medium.alpha_coeff must be non-negative and real.")
 
     def is_defined(self, *fields) -> List[bool]:
         """
         Check if the field(s) are defined or None
 
         Args:
             *fields: String list of the fields
@@ -95,15 +98,15 @@
         Args:
             *fields: String list of the fields
 
         Returns:
             None
         """
         for f in fields:
-            assert getattr(self, f) is not None, f'The field {f} must be not be None'
+            assert getattr(self, f) is not None, f"The field {f} must be not be None"
 
     def is_nonlinear(self) -> bool:
         """
         Check if the medium is nonlinear
 
         Returns:
             whether the fluid simulation is nonlinear
@@ -132,62 +135,61 @@
         """
         Check if the medium properties are set correctly for absorbing simulation without stokes
 
         Returns:
             None
         """
         # enforce both absorption parameters
-        self.ensure_defined('alpha_coeff', 'alpha_power')
+        self.ensure_defined("alpha_coeff", "alpha_power")
 
         # check y is a scalar
-        assert np.isscalar(self.alpha_power), 'medium.alpha_power must be scalar.'
+        assert np.isscalar(self.alpha_power), "medium.alpha_power must be scalar."
 
         # check y is real and within 0 to 3
-        assert np.all(np.isreal(self.alpha_coeff)) and 0 < self.alpha_power < 3, \
-            'medium.alpha_power must be a real number between 0 and 3.'
+        assert np.all(np.isreal(self.alpha_coeff)) and 0 < self.alpha_power < 3, "medium.alpha_power must be a real number between 0 and 3."
 
         # display warning if y is close to 1 and the dispersion term has not been set to zero
-        if self.alpha_mode != 'no_dispersion':
-            assert self.alpha_power != 1, \
-                """The power law dispersion term in the equation of state is not valid for medium.alpha_power = 1.
+        if self.alpha_mode != "no_dispersion":
+            assert self.alpha_power != 1, """The power law dispersion term in the equation of state is not valid for medium.alpha_power = 1.
                 This error can be avoided by choosing a power law exponent close to, but not exactly, 1.
                 If modelling acoustic absorption for medium.alpha_power = 1 is important and modelling dispersion is not
                 critical, this error can also be avoided by setting medium.alpha_mode to 'no_dispersion'"""
 
     def _check_absorbing_with_stokes(self):
         """
         Check if the medium properties are set correctly for absorbing simulation with stokes
 
         Returns:
             None
         """
         # enforce absorption coefficient
-        self.ensure_defined('alpha_coeff')
+        self.ensure_defined("alpha_coeff")
 
         # give warning if y is specified
         if self.alpha_power is not None and (self.alpha_power.size != 1 or self.alpha_power != 2):
-            logging.log(logging.WARN, 'the axisymmetric code and stokes absorption assume alpha_power = 2, user value ignored.')
+            logging.log(logging.WARN, "the axisymmetric code and stokes absorption assume alpha_power = 2, user value ignored.")
 
         # overwrite y value
         self.alpha_power = 2
 
         # don't allow medium.alpha_mode with the axisymmetric code
-        if self.alpha_mode is not None and (self.alpha_mode in ['no_absorption', 'no_dispersion']):
-            raise NotImplementedError('Input option medium.alpha_mode is not supported with the axisymmetric code '
-                                      'or medium.alpha_mode = ''stokes''.')
+        if self.alpha_mode is not None and (self.alpha_mode in ["no_absorption", "no_dispersion"]):
+            raise NotImplementedError(
+                "Input option medium.alpha_mode is not supported with the axisymmetric code " "or medium.alpha_mode = " "stokes" "."
+            )
 
         # don't allow alpha_filter with stokes absorption (no variables are applied in k-space)
-        assert self.alpha_filter is None, \
-            "Input option medium.alpha_filter is not supported with the axisymmetric code " \
-            "or medium.alpha_mode = 'stokes'. "
+        assert self.alpha_filter is None, (
+            "Input option medium.alpha_filter is not supported with the axisymmetric code " "or medium.alpha_mode = 'stokes'. "
+        )
 
     ##########################################
     # Elastic-code related properties - raise error when accessed
     ##########################################
-    _ELASTIC_CODE_ACCESS_ERROR_TEXT_ = 'Elastic simulation and related properties are not supported!'
+    _ELASTIC_CODE_ACCESS_ERROR_TEXT_ = "Elastic simulation and related properties are not supported!"
 
     @property
     def sound_speed_shear(self):  # pragma: no cover
         """
         Shear sound speed (used in elastic simulations | not supported currently!)
         """
         raise NotImplementedError(self._ELASTIC_CODE_ACCESS_ERROR_TEXT_)
```

### Comparing `k_wave_python-0.3.2/kwave/ksensor.py` & `k_wave_python-0.3.3/kwave/ksensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 
 from kwave.utils.matrix import expand_matrix
 
 
 class kSensor(object):
-
     def __init__(self, mask=None, record=None):
         self._mask = mask
         # cell array of the acoustic parameters to record in the form Recorder
         self.record = record
         # record the time series from the beginning by default
         # time index at which the sensor should start recording the data specified by sensor.record
         self._record_start_index = 1
@@ -64,29 +63,29 @@
 @dataclass
 class kSensorDirectivity(object):
     #: matrix of directivity angles (direction of maximum
     #: response) for each sensor element defined in
     #: sensor.mask. The angles are in radians where 0 = max
     #: sensitivity in x direction (up/down) and pi/2 or -pi/2
     #: = max sensitivity in y direction (left/right)
-    angle               : np.ndarray    = None
+    angle: np.ndarray = None
 
     #: string defining the directivity pattern, valid inputs
     #: are 'pressure' (spatial averaging over the sensor
     #: surface equivalent to a sinc function) and 'gradient'
-    pattern             : str           = 'pressure'
+    pattern: str = "pressure"
 
     #: equivalent element size (the larger the element size the more directional the response)
-    size                : float         = None
+    size: float = None
 
     #: list of the unique directivity angles
-    unique_angles       : np.ndarray    = None
+    unique_angles: np.ndarray = None
 
     #: It is precomputed to allow data casting, as kgrid.kx (etc) are computed on the fly.
-    wavenumbers         : np.ndarray    = None
+    wavenumbers: np.ndarray = None
 
     def set_default_size(self, kgrid) -> None:
         """
         Set the element size based on the kGrid
 
         Args:
             kgrid: Instance of `~kwave.kgrid.kWaveGrid` class
```

### Comparing `k_wave_python-0.3.2/kwave/ksource.py` & `k_wave_python-0.3.3/kwave/ksource.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 
 from kwave.kgrid import kWaveGrid
 from kwave.utils.matrix import num_dim2
 
 
 @dataclass
 class kSource(object):
-    _p0             = None
+    _p0 = None
     #: time varying pressure at each of the source positions given by source.p_mask
-    p               = None
+    p = None
     #: binary matrix specifying the positions of the time varying pressure source distribution
-    p_mask          = None
+    p_mask = None
     #: optional input to control whether the input pressure is injected as a mass source or enforced
     # as a dirichlet boundary condition; valid inputs are 'additive' (the default) or 'dirichlet'
-    p_mode          = None
+    p_mode = None
     #: Pressure reference frequency
     p_frequency_ref = None
 
     #: time varying particle velocity in the x-direction at each of the source positions given by source.u_mask
-    ux              = None
+    ux = None
     #: time varying particle velocity in the y-direction at each of the source positions given by source.u_mask
-    uy              = None
+    uy = None
     #: time varying particle velocity in the z-direction at each of the source positions given by source.u_mask
-    uz              = None
+    uz = None
     #: binary matrix specifying the positions of the time varying particle velocity distribution
-    u_mask          = None
+    u_mask = None
     #: optional input to control whether the input velocity is applied as a force source or enforced as a dirichlet
     # boundary condition; valid inputs are 'additive' (the default) or 'dirichlet'
-    u_mode          = None
+    u_mode = None
     #: Velocity reference frequency
     u_frequency_ref = None
 
-    sxx             = None      #: Stress source in x -> x direction
-    syy             = None      #: Stress source in y -> y direction
-    szz             = None      #: Stress source in z -> z direction
-    sxy             = None      #: Stress source in x -> y direction
-    sxz             = None      #: Stress source in x -> z direction
-    syz             = None      #: Stress source in y -> z direction
-    s_mask          = None      #: Stress source mask
-    s_mode          = None      #: Stress source mode
+    sxx = None  #: Stress source in x -> x direction
+    syy = None  #: Stress source in y -> y direction
+    szz = None  #: Stress source in z -> z direction
+    sxy = None  #: Stress source in x -> y direction
+    sxz = None  #: Stress source in x -> z direction
+    syz = None  #: Stress source in y -> z direction
+    s_mask = None  #: Stress source mask
+    s_mode = None  #: Stress source mode
 
     def is_p0_empty(self) -> bool:
         """
         Check if the `p0` field is set and not empty
         """
         return self.p0 is None or len(self.p0) == 0 or (np.sum(self.p0 != 0) == 0)
 
@@ -74,276 +74,283 @@
 
         Returns:
             None
         """
         if self.p0 is not None:
             if self.p0.shape != kgrid.k.shape:
                 # throw an error if p0 is not the correct size
-                raise ValueError('source.p0 must be the same size as the computational grid.')
+                raise ValueError("source.p0 must be the same size as the computational grid.")
 
             # if using the elastic code, reformulate source.p0 in terms of the
             # stress source terms using the fact that source.p = [0.5 0.5] /
             # (2*CFL) is the same as source.p0 = 1
             # if self.elastic_code:
             #     raise NotImplementedError
 
         # check for a time varying pressure source input
         if self.p is not None:
-
             # force p_mask to be given if p is given
             assert self.p_mask is not None
 
             # check mask is the correct size
             # noinspection PyTypeChecker
             if (num_dim2(self.p_mask) != kgrid.dim) or (self.p_mask.shape != kgrid.k.shape):
-                raise ValueError('source.p_mask must be the same size as the computational grid.')
+                raise ValueError("source.p_mask must be the same size as the computational grid.")
 
             # check mask is not empty
-            assert np.sum(self.p_mask) != 0, 'source.p_mask must be a binary grid with at least one element set to 1.'
+            assert np.sum(self.p_mask) != 0, "source.p_mask must be a binary grid with at least one element set to 1."
 
             # don't allow both source.p0 and source.p in the same simulation
             # USERS: please contact us via http://www.k-wave.org/forum if this
             # is a problem
             assert self.p0 is None, "source.p0 and source.p can't be defined in the same simulation."
 
             # check the source mode input is valid
             if self.p_mode is not None:
-                assert self.p_mode in ['additive', 'dirichlet', 'additive-no-correction'], \
-                    "source.p_mode must be set to ''additive'', ''additive-no-correction'', or ''dirichlet''."
+                assert self.p_mode in [
+                    "additive",
+                    "dirichlet",
+                    "additive-no-correction",
+                ], "source.p_mode must be set to ''additive'', ''additive-no-correction'', or ''dirichlet''."
 
             # check if a reference frequency is defined
             if self.p_frequency_ref is not None:
-
                 # check frequency is a scalar, positive number
                 assert np.isscalar(self.p_frequency_ref) and self.p_frequency_ref > 0
 
                 # check frequency is within range
-                assert self.p_frequency_ref <= kgrid.k_max_all * np.min(self.medium.sound_speed / 2 * np.pi), \
-                    'source.p_frequency_ref is higher than the maximum frequency supported by the spatial grid.'
+                assert self.p_frequency_ref <= kgrid.k_max_all * np.min(
+                    self.medium.sound_speed / 2 * np.pi
+                ), "source.p_frequency_ref is higher than the maximum frequency supported by the spatial grid."
 
                 # change source mode to no include k-space correction
-                self.p_mode = 'additive-no-correction'
+                self.p_mode = "additive-no-correction"
 
             if len(self.p[0]) > kgrid.Nt:
-                logging.log(logging.WARN, '  source.p has more time points than kgrid.Nt, remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.p has more time points than kgrid.Nt, remaining time points will not be used.")
 
             # check if the mask is binary or labelled
             p_unique = np.unique(self.p_mask)
 
             # create a second indexing variable
             if p_unique.size <= 2 and p_unique.sum() == 1:
-
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements, or the number
                 # of labelled sources
                 if self.p.shape[0] > 1 and (len(self.p[:, 0]) != self.p_mask.sum()):
-                    raise ValueError('The number of time series in source.p '
-                                     'must match the number of source elements in source.p_mask.')
+                    raise ValueError("The number of time series in source.p " "must match the number of source elements in source.p_mask.")
             else:
-
                 # check the source labels are monotonic, and start from 1
                 if (sum(p_unique[1:] - p_unique[:-1]) != len(p_unique) - 1) or (not any(p_unique == 1)):
                     raise ValueError(
-                        'If using a labelled source.p_mask, '
-                        'the source labels must be monotonically increasing and start from 1.')
+                        "If using a labelled source.p_mask, " "the source labels must be monotonically increasing and start from 1."
+                    )
                 # make sure the correct number of input signals are given
                 if np.size(self.p, 1) != (np.size(p_unique) - 1):
-                    raise ValueError('The number of time series in source.p '
-                                     'must match the number of labelled source elements in source.p_mask.')
+                    raise ValueError(
+                        "The number of time series in source.p " "must match the number of labelled source elements in source.p_mask."
+                    )
 
         # check for time varying velocity source input and set source flag
-        if any([(getattr(self, k) is not None) for k in ['ux', 'uy', 'uz', 'u_mask']]):
-
+        if any([(getattr(self, k) is not None) for k in ["ux", "uy", "uz", "u_mask"]]):
             # force u_mask to be given
             assert self.u_mask is not None
 
             # check mask is the correct size
-            assert num_dim2(self.u_mask) == kgrid.dim and self.u_mask.shape == kgrid.k.shape, \
-                'source.u_mask must be the same size as the computational grid.'
+            assert (
+                num_dim2(self.u_mask) == kgrid.dim and self.u_mask.shape == kgrid.k.shape
+            ), "source.u_mask must be the same size as the computational grid."
 
             # check mask is not empty
-            assert np.array(self.u_mask).sum() != 0, \
-                'source.u_mask must be a binary grid with at least one element set to 1.'
+            assert np.array(self.u_mask).sum() != 0, "source.u_mask must be a binary grid with at least one element set to 1."
 
             # check the source mode input is valid
             if self.u_mode is not None:
-                assert self.u_mode in ['additive', 'dirichlet', 'additive-no-correction'], \
-                    "source.u_mode must be set to ''additive'', ''additive-no-correction'', or ''dirichlet''."
+                assert self.u_mode in [
+                    "additive",
+                    "dirichlet",
+                    "additive-no-correction",
+                ], "source.u_mode must be set to ''additive'', ''additive-no-correction'', or ''dirichlet''."
 
             # check if a reference frequency is defined
             if self.u_frequency_ref is not None:
-
                 # check frequency is a scalar, positive number
                 u_frequency_ref = self.u_frequency_ref
                 assert np.isscalar(u_frequency_ref) and u_frequency_ref > 0
 
                 # check frequency is within range
-                assert self.u_frequency_ref <= (kgrid.k_max_all * np.min(self.medium.sound_speed) / 2 * np.pi), \
-                    "source.u_frequency_ref is higher than the maximum frequency supported by the spatial grid."
+                assert self.u_frequency_ref <= (
+                    kgrid.k_max_all * np.min(self.medium.sound_speed) / 2 * np.pi
+                ), "source.u_frequency_ref is higher than the maximum frequency supported by the spatial grid."
 
                 # change source mode to no include k-space correction
-                self.u_mode = 'additive-no-correction'
+                self.u_mode = "additive-no-correction"
 
             if self.ux is not None:
                 if self.flag_ux > kgrid.Nt:
-                    logging.log(logging.WARN, '  source.ux has more time points than kgrid.Nt, '
-                         'remaining time points will not be used.')
+                    logging.log(logging.WARN, "  source.ux has more time points than kgrid.Nt, " "remaining time points will not be used.")
             if self.uy is not None:
                 if self.flag_uy > kgrid.Nt:
-                    logging.log(logging.WARN, '  source.uy has more time points than kgrid.Nt, '
-                         'remaining time points will not be used.')
+                    logging.log(logging.WARN, "  source.uy has more time points than kgrid.Nt, " "remaining time points will not be used.")
             if self.uz is not None:
                 if self.flag_uz > kgrid.Nt:
-                    logging.log(logging.WARN, '  source.uz has more time points than kgrid.Nt, '
-                         'remaining time points will not be used.')
+                    logging.log(logging.WARN, "  source.uz has more time points than kgrid.Nt, " "remaining time points will not be used.")
 
             # check if the mask is binary or labelled
             u_unique = np.unique(self.u_mask)
 
             # create a second indexing variable
             if u_unique.size <= 2 and u_unique.sum() == 1:
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements
                 ux_size = self.ux[:, 0].size
                 uy_size = self.uy[:, 0].size if (self.uy is not None) else None
                 uz_size = self.uz[:, 0].size if (self.uz is not None) else None
                 u_sum = np.sum(self.u_mask)
-                if (self.flag_ux and (ux_size > 1)) or \
-                        (self.flag_uy and (uy_size > 1)) or \
-                        (self.flag_uz and (uz_size > 1)):
-                    if (self.flag_ux and (ux_size != u_sum)) and \
-                            (self.flag_uy and (uy_size != u_sum)) or \
-                            (self.flag_uz and (uz_size != u_sum)):
-                        raise ValueError('The number of time series in source.ux (etc) '
-                                         'must match the number of source elements in source.u_mask.')
+                if (self.flag_ux and (ux_size > 1)) or (self.flag_uy and (uy_size > 1)) or (self.flag_uz and (uz_size > 1)):
+                    if (
+                        (self.flag_ux and (ux_size != u_sum))
+                        and (self.flag_uy and (uy_size != u_sum))
+                        or (self.flag_uz and (uz_size != u_sum))
+                    ):
+                        raise ValueError(
+                            "The number of time series in source.ux (etc) " "must match the number of source elements in source.u_mask."
+                        )
 
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements
-                if (self.flag_ux and (ux_size > 1)) or \
-                        (self.flag_uy and (uy_size > 1)) or (self.flag_uz and (uz_size > 1)):
-                    if (self.flag_ux and (ux_size != u_sum)) or \
-                            (self.flag_uy and (uy_size != u_sum)) or (self.flag_uz and (uz_size != u_sum)):
-                        raise ValueError('The number of time series in source.ux (etc) '
-                                         'must match the number of source elements in source.u_mask.')
+                if (self.flag_ux and (ux_size > 1)) or (self.flag_uy and (uy_size > 1)) or (self.flag_uz and (uz_size > 1)):
+                    if (
+                        (self.flag_ux and (ux_size != u_sum))
+                        or (self.flag_uy and (uy_size != u_sum))
+                        or (self.flag_uz and (uz_size != u_sum))
+                    ):
+                        raise ValueError(
+                            "The number of time series in source.ux (etc) " "must match the number of source elements in source.u_mask."
+                        )
             else:
                 raise NotImplementedError
 
                 # check the source labels are monotonic, and start from 1
                 # if (sum(u_unique(2:end) - u_unique(1:end-1)) != (numel(u_unique) - 1)) or (~any(u_unique == 1))
-                if eng.eval('(sum(u_unique(2:end) - '
-                            'u_unique(1:end-1)) ~= '
-                            '(numel(u_unique) - 1)) '
-                            '|| '
-                            '(~any(u_unique == 1))'):
-                    raise ValueError('If using a labelled source.u_mask, '
-                                     'the source labels must be monotonically increasing and start from 1.')
+                if eng.eval("(sum(u_unique(2:end) - " "u_unique(1:end-1)) ~= " "(numel(u_unique) - 1)) " "|| " "(~any(u_unique == 1))"):
+                    raise ValueError(
+                        "If using a labelled source.u_mask, " "the source labels must be monotonically increasing and start from 1."
+                    )
 
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements
                 # if (flgs.source_ux and (size(source.ux, 1) != (numel(u_unique) - 1))) or
                 #   (flgs.source_uy and (size(source.uy, 1) != (numel(u_unique) - 1))) or
                 #   (flgs.source_uz and (size(source.uz, 1) != (numel(u_unique) - 1)))
-                if eng.eval('(flgs.source_ux && (size(source.ux, 1) ~= (numel(u_unique) - 1))) '
-                            '|| (flgs.source_uy && (size(source.uy, 1) ~= (numel(u_unique) - 1))) '
-                            '|| '
-                            '(flgs.source_uz && (size(source.uz, 1) ~= (numel(u_unique) - 1)))'):
-                    raise ValueError('The number of time series in source.ux (etc) '
-                                     'must match the number of labelled source elements in source.u_mask.')
+                if eng.eval(
+                    "(flgs.source_ux && (size(source.ux, 1) ~= (numel(u_unique) - 1))) "
+                    "|| (flgs.source_uy && (size(source.uy, 1) ~= (numel(u_unique) - 1))) "
+                    "|| "
+                    "(flgs.source_uz && (size(source.uz, 1) ~= (numel(u_unique) - 1)))"
+                ):
+                    raise ValueError(
+                        "The number of time series in source.ux (etc) "
+                        "must match the number of labelled source elements in source.u_mask."
+                    )
 
         # check for time varying stress source input and set source flag
-        if any([(getattr(self, k) is not None) for k in ['sxx', 'syy', 'szz', 'sxy', 'sxz', 'syz', 's_mask']]):
-
+        if any([(getattr(self, k) is not None) for k in ["sxx", "syy", "szz", "sxy", "sxz", "syz", "s_mask"]]):
             # force s_mask to be given
-            enforce_fields(self, 's_mask')
+            enforce_fields(self, "s_mask")
 
             # check mask is the correct size
             # if (numDim(source.s_mask) != kgrid.dim) or (all(size(source.s_mask) != size(kgrid.k)))
-            if eng.eval('(numDim(source.s_mask) ~= kgrid.dim) || (all(size(source.s_mask) ~= size(kgrid.k)))'):
-                raise ValueError('source.s_mask must be the same size as the computational grid.')
+            if eng.eval("(numDim(source.s_mask) ~= kgrid.dim) || (all(size(source.s_mask) ~= size(kgrid.k)))"):
+                raise ValueError("source.s_mask must be the same size as the computational grid.")
 
             # check mask is not empty
-            assert np.array(eng.getfield(source, 's_mask')) != 0, \
-                "source.s_mask must be a binary grid with at least one element set to 1."
+            assert np.array(eng.getfield(source, "s_mask")) != 0, "source.s_mask must be a binary grid with at least one element set to 1."
 
             # check the source mode input is valid
-            if eng.isfield(source, 's_mode'):
-                assert eng.getfield(source, 's_mode') in ['additive', 'dirichlet'], \
-                    "source.s_mode must be set to ''additive'' or ''dirichlet''."
+            if eng.isfield(source, "s_mode"):
+                assert eng.getfield(source, "s_mode") in [
+                    "additive",
+                    "dirichlet",
+                ], "source.s_mode must be set to ''additive'' or ''dirichlet''."
             else:
-                eng.setfield(source, 's_mode', self.SOURCE_S_MODE_DEF)
+                eng.setfield(source, "s_mode", self.SOURCE_S_MODE_DEF)
 
             # set source flgs to the length of the sources, this allows the
             # inputs to be defined independently and be of any length
             if self.sxx is not None and self_sxx > k_Nt:
-                logging.log(logging.WARN, '  source.sxx has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.sxx has more time points than kgrid.Nt," " remaining time points will not be used.")
             if self.syy is not None and self_syy > k_Nt:
-                logging.log(logging.WARN, '  source.syy has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.syy has more time points than kgrid.Nt," " remaining time points will not be used.")
             if self.szz is not None and self_szz > k_Nt:
-                logging.log(logging.WARN, '  source.szz has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.szz has more time points than kgrid.Nt," " remaining time points will not be used.")
             if self.sxy is not None and self_sxy > k_Nt:
-                logging.log(logging.WARN, '  source.sxy has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.sxy has more time points than kgrid.Nt," " remaining time points will not be used.")
             if self.sxz is not None and self_sxz > k_Nt:
-                logging.log(logging.WARN, '  source.sxz has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.sxz has more time points than kgrid.Nt," " remaining time points will not be used.")
             if self.syz is not None and self_syz > k_Nt:
-                logging.log(logging.WARN, '  source.syz has more time points than kgrid.Nt,'
-                     ' remaining time points will not be used.')
+                logging.log(logging.WARN, "  source.syz has more time points than kgrid.Nt," " remaining time points will not be used.")
 
             # create an indexing variable corresponding to the location of all
             # the source elements
             raise NotImplementedError
 
             # check if the mask is binary or labelled
-            's_unique = unique(source.s_mask);'
+            "s_unique = unique(source.s_mask);"
 
             # create a second indexing variable
-            if eng.eval('numel(s_unique) <= 2 && sum(s_unique) == 1'):
-                s_mask = eng.getfield(source, 's_mask')
+            if eng.eval("numel(s_unique) <= 2 && sum(s_unique) == 1"):
+                s_mask = eng.getfield(source, "s_mask")
                 s_mask_sum = np.array(s_mask).sum()
 
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements
-                if (self.source_sxx and (eng.eval('length(source.sxx(:,1)) > 1))'))) or \
-                        (self.source_syy and (eng.eval('length(source.syy(:,1)) > 1))'))) or \
-                        (self.source_szz and (eng.eval('length(source.szz(:,1)) > 1))'))) or \
-                        (self.source_sxy and (eng.eval('length(source.sxy(:,1)) > 1))'))) or \
-                        (self.source_sxz and (eng.eval('length(source.sxz(:,1)) > 1))'))) or \
-                        (self.source_syz and (eng.eval('length(source.syz(:,1)) > 1))'))):
-                    if (self.source_sxx and (eng.eval('length(source.sxx(:,1))') != s_mask_sum)) or \
-                            (self.source_syy and (eng.eval('length(source.syy(:,1))') != s_mask_sum)) or \
-                            (self.source_szz and (eng.eval('length(source.szz(:,1))') != s_mask_sum)) or \
-                            (self.source_sxy and (eng.eval('length(source.sxy(:,1))') != s_mask_sum)) or \
-                            (self.source_sxz and (eng.eval('length(source.sxz(:,1))') != s_mask_sum)) or \
-                            (self.source_syz and (eng.eval('length(source.syz(:,1))') != s_mask_sum)):
-                        raise ValueError('The number of time series in source.sxx (etc) '
-                                         'must match the number of source elements in source.s_mask.')
+                if (
+                    (self.source_sxx and (eng.eval("length(source.sxx(:,1)) > 1))")))
+                    or (self.source_syy and (eng.eval("length(source.syy(:,1)) > 1))")))
+                    or (self.source_szz and (eng.eval("length(source.szz(:,1)) > 1))")))
+                    or (self.source_sxy and (eng.eval("length(source.sxy(:,1)) > 1))")))
+                    or (self.source_sxz and (eng.eval("length(source.sxz(:,1)) > 1))")))
+                    or (self.source_syz and (eng.eval("length(source.syz(:,1)) > 1))")))
+                ):
+                    if (
+                        (self.source_sxx and (eng.eval("length(source.sxx(:,1))") != s_mask_sum))
+                        or (self.source_syy and (eng.eval("length(source.syy(:,1))") != s_mask_sum))
+                        or (self.source_szz and (eng.eval("length(source.szz(:,1))") != s_mask_sum))
+                        or (self.source_sxy and (eng.eval("length(source.sxy(:,1))") != s_mask_sum))
+                        or (self.source_sxz and (eng.eval("length(source.sxz(:,1))") != s_mask_sum))
+                        or (self.source_syz and (eng.eval("length(source.syz(:,1))") != s_mask_sum))
+                    ):
+                        raise ValueError(
+                            "The number of time series in source.sxx (etc) " "must match the number of source elements in source.s_mask."
+                        )
 
             else:
                 # check the source labels are monotonic, and start from 1
                 # if (sum(s_unique(2:end) - s_unique(1:end-1)) != (numel(s_unique) - 1)) or (~any(s_unique == 1))
-                if eng.eval('(sum(s_unique(2:end) - s_unique(1:end-1)) ~= '
-                            '(numel(s_unique) - 1)) || (~any(s_unique == 1))'):
-                    raise ValueError('If using a labelled source.s_mask, '
-                                     'the source labels must be monotonically increasing and start from 1.')
+                if eng.eval("(sum(s_unique(2:end) - s_unique(1:end-1)) ~= " "(numel(s_unique) - 1)) || (~any(s_unique == 1))"):
+                    raise ValueError(
+                        "If using a labelled source.s_mask, " "the source labels must be monotonically increasing and start from 1."
+                    )
 
-                numel_s_unique = eng.eval('numel(s_unique) - 1;')
+                numel_s_unique = eng.eval("numel(s_unique) - 1;")
                 # if more than one time series is given, check the number of time
                 # series given matches the number of source elements
-                if (self.source_sxx and (eng.eval('size(source.sxx, 1)') != numel_s_unique)) or \
-                        (self.source_syy and (eng.eval('size(source.syy, 1)') != numel_s_unique)) or \
-                        (self.source_szz and (eng.eval('size(source.szz, 1)') != numel_s_unique)) or \
-                        (self.source_sxy and (eng.eval('size(source.sxy, 1)') != numel_s_unique)) or \
-                        (self.source_sxz and (eng.eval('size(source.sxz, 1)') != numel_s_unique)) or \
-                        (self.source_syz and (eng.eval('size(source.syz, 1)') != numel_s_unique)):
-                    raise ValueError('The number of time series in source.sxx (etc) '
-                                     'must match the number of labelled source elements in source.u_mask.')
+                if (
+                    (self.source_sxx and (eng.eval("size(source.sxx, 1)") != numel_s_unique))
+                    or (self.source_syy and (eng.eval("size(source.syy, 1)") != numel_s_unique))
+                    or (self.source_szz and (eng.eval("size(source.szz, 1)") != numel_s_unique))
+                    or (self.source_sxy and (eng.eval("size(source.sxy, 1)") != numel_s_unique))
+                    or (self.source_sxz and (eng.eval("size(source.sxz, 1)") != numel_s_unique))
+                    or (self.source_syz and (eng.eval("size(source.syz, 1)") != numel_s_unique))
+                ):
+                    raise ValueError(
+                        "The number of time series in source.sxx (etc) "
+                        "must match the number of labelled source elements in source.u_mask."
+                    )
 
     @property
     def flag_ux(self):
         """
         Get the length of the sources in X-direction, this allows the
         inputs to be defined independently and be of any length
```

### Comparing `k_wave_python-0.3.2/kwave/kspaceFirstOrder2D.py` & `k_wave_python-0.3.3/kwave/kspaceFirstOrder2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 from kwave.utils.dotdictionary import dotdict
 from kwave.utils.interp import interpolate2d
 from kwave.utils.pml import get_pml
 from kwave.utils.tictoc import TicToc
 
 
 def kspace_first_order_2d_gpu(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: NotATransducer,
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions) -> np.ndarray:
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: NotATransducer,
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
+) -> np.ndarray:
     """
     2D ime-domain simulation of wave propagation on a GPU using C++ CUDA code.
 
     kspaceFirstOrder2DG provides a blind interface to the C++/CUDA
     version of kspaceFirstOrder2D (called kspaceFirstOrder-CUDA) in the
     same way as kspaceFirstOrder3DC. Note, the C++ code does not support
     all input options, and all display options are ignored (only command
@@ -51,38 +52,32 @@
     'BinariesPath'.
 
     This function is essentially a wrapper and directly uses the capabilities
     of kspaceFirstOrder3DC by replacing the binary name with the name of the
     GPU binary.
     """
     execution_options.is_gpu_simulation = True  # force to GPU
-    assert isinstance(kgrid, kWaveGrid), 'kgrid must be a kWaveGrid object'
-    assert isinstance(medium, kWaveMedium), 'medium must be a kWaveMedium object'
-    assert isinstance(simulation_options, SimulationOptions), 'simulation_options must be a SimulationOptions object'
-    assert isinstance(execution_options,
-                      SimulationExecutionOptions), 'execution_options must be a SimulationExecutionOptions object'
+    assert isinstance(kgrid, kWaveGrid), "kgrid must be a kWaveGrid object"
+    assert isinstance(medium, kWaveMedium), "medium must be a kWaveMedium object"
+    assert isinstance(simulation_options, SimulationOptions), "simulation_options must be a SimulationOptions object"
+    assert isinstance(execution_options, SimulationExecutionOptions), "execution_options must be a SimulationExecutionOptions object"
 
     sensor_data = kspaceFirstOrder2D(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options,
-        execution_options=execution_options
+        kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options, execution_options=execution_options
     )  # pass inputs to CPU version
     return sensor_data
 
 
 def kspaceFirstOrder2DC(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     2D time-domain simulation of wave propagation using C++ code.
 
     kspaceFirstOrder2DC provides a blind interface to the C++ version of
     kspaceFirstOrder2D (called kspaceFirstOrder-OMP) in the same way as
     kspaceFirstOrder3DC. Note, the C++ code does not support all input
@@ -126,31 +121,26 @@
 
     Returns:
         Sensor data as a numpy array
     """
     execution_options.is_gpu_simulation = False  # force to CPU
     # generate the input file and save to disk
     sensor_data = kspaceFirstOrder2D(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options,
-        execution_options=execution_options
+        kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options, execution_options=execution_options
     )
     return sensor_data
 
 
 def kspaceFirstOrder2D(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor, None],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor, None],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     2D time-domain simulation of wave propagation.
 
     kspaceFirstOrder2D simulates the time-domain propagation of
     compressional waves through a two-dimensional homogeneous or
     heterogeneous acoustic medium given four input structures: kgrid,
@@ -294,27 +284,21 @@
     """
     # start the timer and store the start time
     TicToc.tic()
 
     # Currently we only support binary execution, meaning all simulations must be saved to disk.
     if not simulation_options.save_to_disk:
         if execution_options.is_gpu_simulation:
-            raise ValueError('GPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True')
+            raise ValueError("GPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True")
         else:
-            raise ValueError('CPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True')
+            raise ValueError("CPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True")
 
-    k_sim = kWaveSimulation(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options
-    )
+    k_sim = kWaveSimulation(kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options)
 
-    k_sim.input_checking('kspaceFirstOrder2D')
+    k_sim.input_checking("kspaceFirstOrder2D")
 
     # =========================================================================
     # CALCULATE MEDIUM PROPERTIES ON STAGGERED GRID
     # =========================================================================
     options = k_sim.options
 
     # interpolate the values of the density at the staggered grid locations
@@ -348,107 +332,114 @@
     Nx, Ny = k_sim.kgrid.Nx, k_sim.kgrid.Ny
     dx, dy = k_sim.kgrid.dx, k_sim.kgrid.dy
     dt = k_sim.kgrid.dt
     pml_x_alpha, pml_y_alpha = options.pml_x_alpha, options.pml_y_alpha
     pml_x_size, pml_y_size = options.pml_x_size, options.pml_y_size
     c_ref = k_sim.c_ref
 
-    k_sim.pml_x     = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, False, 1)
+    k_sim.pml_x = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, False, 1)
     k_sim.pml_x_sgx = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, True and options.use_sg, 1)
-    k_sim.pml_y     = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, False, 2)
+    k_sim.pml_y = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, False, 2)
     k_sim.pml_y_sgy = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, True and options.use_sg, 2)
 
     # define the k-space derivative operators, multiply by the staggered
     # grid shift operators, and then re-order using ifftshift (the option
     # flgs.use_sg exists for debugging)
     kx_vec, ky_vec = k_sim.kgrid.k_vec
     kx_vec, ky_vec = np.array(kx_vec), np.array(ky_vec)
     if options.use_sg:
-        k_sim.ddx_k_shift_pos = np.fft.ifftshift( 1j * kx_vec * np.exp( 1j * kx_vec * dx/2) )[None, :]
-        k_sim.ddx_k_shift_neg = np.fft.ifftshift( 1j * kx_vec * np.exp( -1j * kx_vec * dx/2) )[None, :]
-        k_sim.ddy_k_shift_pos = np.fft.ifftshift( 1j * ky_vec * np.exp( 1j * ky_vec * dy/2) )[None, :]
-        k_sim.ddy_k_shift_neg = np.fft.ifftshift( 1j * ky_vec * np.exp( -1j * ky_vec * dy/2) )[None, :]
+        k_sim.ddx_k_shift_pos = np.fft.ifftshift(1j * kx_vec * np.exp(1j * kx_vec * dx / 2))[None, :]
+        k_sim.ddx_k_shift_neg = np.fft.ifftshift(1j * kx_vec * np.exp(-1j * kx_vec * dx / 2))[None, :]
+        k_sim.ddy_k_shift_pos = np.fft.ifftshift(1j * ky_vec * np.exp(1j * ky_vec * dy / 2))[None, :]
+        k_sim.ddy_k_shift_neg = np.fft.ifftshift(1j * ky_vec * np.exp(-1j * ky_vec * dy / 2))[None, :]
     else:
-        k_sim.ddx_k_shift_pos = np.fft.ifftshift( 1j * kx_vec )[None, :]
-        k_sim.ddx_k_shift_neg = np.fft.ifftshift( 1j * kx_vec )[None, :]
-        k_sim.ddy_k_shift_pos = np.fft.ifftshift( 1j * ky_vec )[None, :]
-        k_sim.ddy_k_shift_neg = np.fft.ifftshift( 1j * ky_vec )[None, :]
+        k_sim.ddx_k_shift_pos = np.fft.ifftshift(1j * kx_vec)[None, :]
+        k_sim.ddx_k_shift_neg = np.fft.ifftshift(1j * kx_vec)[None, :]
+        k_sim.ddy_k_shift_pos = np.fft.ifftshift(1j * ky_vec)[None, :]
+        k_sim.ddy_k_shift_neg = np.fft.ifftshift(1j * ky_vec)[None, :]
 
     # force the derivative and shift operators to be in the correct direction for use with BSXFUN
     k_sim.ddy_k_shift_pos = k_sim.ddy_k_shift_pos.T
     k_sim.ddy_k_shift_neg = k_sim.ddy_k_shift_neg.T
 
     # create k-space operators (the option flgs.use_kspace exists for debugging)
     if options.use_kspace:
         k = k_sim.kgrid.k
         k_sim.kappa = np.fft.ifftshift(np.sinc(c_ref * k * dt / 2))
-        if (k_sim.source_p and k_sim.source.p_mode == 'additive') or \
-                ((k_sim.source_ux or k_sim.source_uy or k_sim.source_uz) and k_sim.source.u_mode == 'additive'):
+        if (k_sim.source_p and k_sim.source.p_mode == "additive") or (
+            (k_sim.source_ux or k_sim.source_uy or k_sim.source_uz) and k_sim.source.u_mode == "additive"
+        ):
             k_sim.source_kappa = np.fft.ifftshift(np.cos(c_ref * k * dt / 2))
     else:
-        k_sim.kappa          = 1
-        k_sim.source_kappa   = 1
+        k_sim.kappa = 1
+        k_sim.source_kappa = 1
 
     # =========================================================================
     # SAVE DATA TO DISK FOR RUNNING SIMULATION EXTERNAL TO MATLAB
     # =========================================================================
 
     # save to disk option for saving the input matrices to disk for running
     # simulations using k-Wave++
     if options.save_to_disk:
         # store the pml size for resizing transducer object below
         retract_size = [[options.pml_x_size, options.pml_y_size, options.pml_z_size]]
 
         # run subscript to save files to disk
-        save_to_disk_func(k_sim.kgrid, k_sim.medium, k_sim.source, k_sim.options, execution_options.auto_chunking,
-                          dotdict({
-                              'ddx_k_shift_pos': k_sim.ddx_k_shift_pos,
-                              'ddx_k_shift_neg': k_sim.ddx_k_shift_neg,
-                              'dt': k_sim.dt,
-                              'c0': k_sim.c0,
-                              'c_ref': k_sim.c_ref,
-                              'rho0': k_sim.rho0,
-                              'rho0_sgx': k_sim.rho0_sgx,
-                              'rho0_sgy': k_sim.rho0_sgy,
-                              'rho0_sgz': k_sim.rho0_sgz,
-                              'p_source_pos_index': k_sim.p_source_pos_index,
-                              'u_source_pos_index': k_sim.u_source_pos_index,
-                              's_source_pos_index': k_sim.s_source_pos_index,
-                              'transducer_input_signal': k_sim.transducer_input_signal,
-                              'delay_mask': k_sim.delay_mask,
-                              'sensor_mask_index': k_sim.sensor_mask_index,
-                              'record': k_sim.record,
-                          }),
-                          dotdict({
-                            'source_p': k_sim.source_p,
-                            'source_p0': k_sim.source_p0,
-
-                            'source_ux': k_sim.source_ux,
-                            'source_uy': k_sim.source_uy,
-                            'source_uz': k_sim.source_uz,
-
-                            'source_sxx': k_sim.source_sxx,
-                            'source_syy': k_sim.source_syy,
-                            'source_szz': k_sim.source_szz,
-                            'source_sxy': k_sim.source_sxy,
-                            'source_sxz': k_sim.source_sxz,
-                            'source_syz': k_sim.source_syz,
-
-                            'transducer_source': k_sim.transducer_source,
-                            'nonuniform_grid': k_sim.nonuniform_grid,
-                            'elastic_code': k_sim.options.simulation_type.is_elastic_simulation(),
-                            'axisymmetric': k_sim.options.simulation_type.is_axisymmetric(),
-                            'cuboid_corners': k_sim.cuboid_corners,
-                        }))
+        save_to_disk_func(
+            k_sim.kgrid,
+            k_sim.medium,
+            k_sim.source,
+            k_sim.options,
+            execution_options.auto_chunking,
+            dotdict(
+                {
+                    "ddx_k_shift_pos": k_sim.ddx_k_shift_pos,
+                    "ddx_k_shift_neg": k_sim.ddx_k_shift_neg,
+                    "dt": k_sim.dt,
+                    "c0": k_sim.c0,
+                    "c_ref": k_sim.c_ref,
+                    "rho0": k_sim.rho0,
+                    "rho0_sgx": k_sim.rho0_sgx,
+                    "rho0_sgy": k_sim.rho0_sgy,
+                    "rho0_sgz": k_sim.rho0_sgz,
+                    "p_source_pos_index": k_sim.p_source_pos_index,
+                    "u_source_pos_index": k_sim.u_source_pos_index,
+                    "s_source_pos_index": k_sim.s_source_pos_index,
+                    "transducer_input_signal": k_sim.transducer_input_signal,
+                    "delay_mask": k_sim.delay_mask,
+                    "sensor_mask_index": k_sim.sensor_mask_index,
+                    "record": k_sim.record,
+                }
+            ),
+            dotdict(
+                {
+                    "source_p": k_sim.source_p,
+                    "source_p0": k_sim.source_p0,
+                    "source_ux": k_sim.source_ux,
+                    "source_uy": k_sim.source_uy,
+                    "source_uz": k_sim.source_uz,
+                    "source_sxx": k_sim.source_sxx,
+                    "source_syy": k_sim.source_syy,
+                    "source_szz": k_sim.source_szz,
+                    "source_sxy": k_sim.source_sxy,
+                    "source_sxz": k_sim.source_sxz,
+                    "source_syz": k_sim.source_syz,
+                    "transducer_source": k_sim.transducer_source,
+                    "nonuniform_grid": k_sim.nonuniform_grid,
+                    "elastic_code": k_sim.options.simulation_type.is_elastic_simulation(),
+                    "axisymmetric": k_sim.options.simulation_type.is_axisymmetric(),
+                    "cuboid_corners": k_sim.cuboid_corners,
+                }
+            ),
+        )
 
         # run subscript to resize the transducer object if the grid has been expanded
         retract_transducer_grid_size(k_sim.source, k_sim.sensor, retract_size, k_sim.options.pml_inside)
 
         # exit matlab computation if required
         if options.save_to_disk_exit:
             return
 
         executor = Executor(simulation_options=simulation_options, execution_options=execution_options)
         executor_options = execution_options.get_options_string(sensor=k_sim.sensor)
-        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename,
-                                              options=executor_options)
+        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename, options=executor_options)
         return sensor_data
```

### Comparing `k_wave_python-0.3.2/kwave/kspaceFirstOrder3D.py` & `k_wave_python-0.3.3/kwave/kspaceFirstOrder3D.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 from kwave.utils.dotdictionary import dotdict
 from kwave.utils.interp import interpolate3d
 from kwave.utils.pml import get_pml
 from kwave.utils.tictoc import TicToc
 
 
 def kspaceFirstOrder3DG(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     3D time-domain simulation of wave propagation on a GPU using C++ CUDA code.
 
     kspaceFirstOrder3DG provides a blind interface to the C++/CUDA
     version of kspaceFirstOrder3D (called kspaceFirstOrder-CUDA) in the
     same way as kspaceFirstOrder3DC. Note, the C++ code does not support
@@ -59,33 +59,28 @@
     Args:
         **kwargs:
 
     Returns:
 
     """
     execution_options.is_gpu_simulation = True
-    assert execution_options.is_gpu_simulation, 'kspaceFirstOrder2DG can only be used for GPU simulations'
+    assert execution_options.is_gpu_simulation, "kspaceFirstOrder2DG can only be used for GPU simulations"
     sensor_data = kspaceFirstOrder3D(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options,
-        execution_options=execution_options
+        kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options, execution_options=execution_options
     )  # pass inputs to CPU version
     return sensor_data
 
 
 def kspaceFirstOrder3DC(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     3D time-domain simulation of wave propagation using C++ code.
 
     kspaceFirstOrder3DC provides a blind interface to the C++ version of
     kspaceFirstOrder3D (called kspaceFirstOrder-OMP). Note, the C++ code
     does not support all input options, and all display options are
@@ -119,31 +114,26 @@
 
     Returns:
 
     """
     execution_options.is_gpu_simulation = False
     # generate the input file and save to disk
     sensor_data = kspaceFirstOrder3D(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options,
-        execution_options=execution_options
+        kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options, execution_options=execution_options
     )
     return sensor_data
 
 
 def kspaceFirstOrder3D(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     3D time-domain simulation of wave propagation.
 
     kspaceFirstOrder3D simulates the time-domain propagation of
     compressional waves through a three-dimensional homogeneous or
     heterogeneous acoustic medium given four input structures: kgrid,
@@ -297,26 +287,20 @@
     """
     # start the timer and store the start time
     TicToc.tic()
 
     # Currently we only support binary execution, meaning all simulations must be saved to disk.
     if not simulation_options.save_to_disk:
         if execution_options.is_gpu_simulation:
-            raise ValueError('GPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True')
+            raise ValueError("GPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True")
         else:
-            raise ValueError('CPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True')
+            raise ValueError("CPU simulation requires saving to disk. Please set SimulationOptions.save_to_disk=True")
 
-    k_sim = kWaveSimulation(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options
-    )
-    k_sim.input_checking('kspaceFirstOrder3D')
+    k_sim = kWaveSimulation(kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options)
+    k_sim.input_checking("kspaceFirstOrder3D")
 
     # =========================================================================
     # CALCULATE MEDIUM PROPERTIES ON STAGGERED GRID
     # =========================================================================
     options = k_sim.options
 
     # TODO(walter): this could all be moved inside of ksim
@@ -355,40 +339,40 @@
     Nx, Ny, Nz = k_sim.kgrid.Nx, k_sim.kgrid.Ny, k_sim.kgrid.Nz
     dx, dy, dz = k_sim.kgrid.dx, k_sim.kgrid.dy, k_sim.kgrid.dz
     dt = k_sim.kgrid.dt
     pml_x_alpha, pml_y_alpha, pml_z_alpha = options.pml_x_alpha, options.pml_y_alpha, options.pml_z_alpha
     pml_x_size, pml_y_size, pml_z_size = options.pml_x_size, options.pml_y_size, options.pml_z_size
     c_ref = k_sim.c_ref
 
-    k_sim.pml_x     = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, False, 1)
+    k_sim.pml_x = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, False, 1)
     k_sim.pml_x_sgx = get_pml(Nx, dx, dt, c_ref, pml_x_size, pml_x_alpha, True and options.use_sg, 1)
-    k_sim.pml_y     = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, False, 2)
+    k_sim.pml_y = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, False, 2)
     k_sim.pml_y_sgy = get_pml(Ny, dy, dt, c_ref, pml_y_size, pml_y_alpha, True and options.use_sg, 2)
-    k_sim.pml_z     = get_pml(Nz, dz, dt, c_ref, pml_z_size, pml_z_alpha, False, 3)
+    k_sim.pml_z = get_pml(Nz, dz, dt, c_ref, pml_z_size, pml_z_alpha, False, 3)
     k_sim.pml_z_sgz = get_pml(Nz, dz, dt, c_ref, pml_z_size, pml_z_alpha, True and options.use_sg, 3)
 
     # define the k-space derivative operators, multiply by the staggered
     # grid shift operators, and then re-order using ifftshift (the option
     # flgs.use_sg exists for debugging)
     kx_vec, ky_vec, kz_vec = k_sim.kgrid.k_vec
     kx_vec, ky_vec, kz_vec = np.array(kx_vec), np.array(ky_vec), np.array(kz_vec)
     if options.use_sg:
-        k_sim.ddx_k_shift_pos = np.fft.ifftshift( 1j * kx_vec * np.exp( 1j * kx_vec * dx/2) ).T
-        k_sim.ddx_k_shift_neg = np.fft.ifftshift( 1j * kx_vec * np.exp( -1j * kx_vec * dx/2) ).T
-        k_sim.ddy_k_shift_pos = np.fft.ifftshift( 1j * ky_vec * np.exp( 1j * ky_vec * dy/2) ).T
-        k_sim.ddy_k_shift_neg = np.fft.ifftshift( 1j * ky_vec * np.exp( -1j * ky_vec * dy/2) ).T
-        k_sim.ddz_k_shift_pos = np.fft.ifftshift( 1j * kz_vec * np.exp( 1j * kz_vec * dz/2) ).T
-        k_sim.ddz_k_shift_neg = np.fft.ifftshift( 1j * kz_vec * np.exp( -1j * kz_vec * dz/2) ).T
+        k_sim.ddx_k_shift_pos = np.fft.ifftshift(1j * kx_vec * np.exp(1j * kx_vec * dx / 2)).T
+        k_sim.ddx_k_shift_neg = np.fft.ifftshift(1j * kx_vec * np.exp(-1j * kx_vec * dx / 2)).T
+        k_sim.ddy_k_shift_pos = np.fft.ifftshift(1j * ky_vec * np.exp(1j * ky_vec * dy / 2)).T
+        k_sim.ddy_k_shift_neg = np.fft.ifftshift(1j * ky_vec * np.exp(-1j * ky_vec * dy / 2)).T
+        k_sim.ddz_k_shift_pos = np.fft.ifftshift(1j * kz_vec * np.exp(1j * kz_vec * dz / 2)).T
+        k_sim.ddz_k_shift_neg = np.fft.ifftshift(1j * kz_vec * np.exp(-1j * kz_vec * dz / 2)).T
     else:
-        k_sim.ddx_k_shift_pos = np.fft.ifftshift( 1j * kx_vec ).T
-        k_sim.ddx_k_shift_neg = np.fft.ifftshift( 1j * kx_vec ).T
-        k_sim.ddy_k_shift_pos = np.fft.ifftshift( 1j * ky_vec ).T
-        k_sim.ddy_k_shift_neg = np.fft.ifftshift( 1j * ky_vec ).T
-        k_sim.ddz_k_shift_pos = np.fft.ifftshift( 1j * kz_vec ).T
-        k_sim.ddz_k_shift_neg = np.fft.ifftshift( 1j * kz_vec ).T
+        k_sim.ddx_k_shift_pos = np.fft.ifftshift(1j * kx_vec).T
+        k_sim.ddx_k_shift_neg = np.fft.ifftshift(1j * kx_vec).T
+        k_sim.ddy_k_shift_pos = np.fft.ifftshift(1j * ky_vec).T
+        k_sim.ddy_k_shift_neg = np.fft.ifftshift(1j * ky_vec).T
+        k_sim.ddz_k_shift_pos = np.fft.ifftshift(1j * kz_vec).T
+        k_sim.ddz_k_shift_neg = np.fft.ifftshift(1j * kz_vec).T
 
     # force the derivative and shift operators to be in the correct direction for use with BSXFUN
     k_sim.ddy_k_shift_pos = k_sim.ddy_k_shift_pos.T
     k_sim.ddy_k_shift_neg = k_sim.ddy_k_shift_neg.T
 
     ddz_k_shift_pos = k_sim.ddz_k_shift_pos  # N x 1
     ddz_k_shift_pos = np.expand_dims(ddz_k_shift_pos, axis=-1).transpose((1, 2, 0))
@@ -398,78 +382,85 @@
     ddz_k_shift_neg = np.expand_dims(ddz_k_shift_neg, axis=-1).transpose((1, 2, 0))
     k_sim.ddz_k_shift_neg = ddz_k_shift_neg
 
     # create k-space operators (the option flgs.use_kspace exists for debugging)
     if options.use_kspace:
         k = k_sim.kgrid.k
         k_sim.kappa = np.fft.ifftshift(np.sinc(c_ref * k * dt / 2))
-        if (k_sim.source_p and k_sim.source.p_mode == 'additive') or \
-                ((k_sim.source_ux or k_sim.source_uy or k_sim.source_uz) and k_sim.source.u_mode == 'additive'):
+        if (k_sim.source_p and k_sim.source.p_mode == "additive") or (
+            (k_sim.source_ux or k_sim.source_uy or k_sim.source_uz) and k_sim.source.u_mode == "additive"
+        ):
             k_sim.source_kappa = np.fft.ifftshift(np.cos(c_ref * k * dt / 2))
     else:
-        k_sim.kappa          = 1
-        k_sim.source_kappa   = 1
+        k_sim.kappa = 1
+        k_sim.source_kappa = 1
 
     # =========================================================================
     # SAVE DATA TO DISK FOR RUNNING SIMULATION EXTERNAL TO MATLAB
     # =========================================================================
 
     # save to disk option for saving the input matrices to disk for running
     # simulations using k-Wave++
     if options.save_to_disk:
         # store the pml size for resizing transducer object below
         retract_size = [[options.pml_x_size, options.pml_y_size, options.pml_z_size]]
 
         # run subscript to save files to disk
-        save_to_disk_func(k_sim.kgrid, k_sim.medium, k_sim.source, k_sim.options, execution_options.auto_chunking,
-                          dotdict({
-                              'ddx_k_shift_pos': k_sim.ddx_k_shift_pos,
-                              'ddx_k_shift_neg': k_sim.ddx_k_shift_neg,
-                              'dt': k_sim.dt,
-                              'c0': k_sim.c0,
-                              'c_ref': k_sim.c_ref,
-                              'rho0': k_sim.rho0,
-                              'rho0_sgx': k_sim.rho0_sgx,
-                              'rho0_sgy': k_sim.rho0_sgy,
-                              'rho0_sgz': k_sim.rho0_sgz,
-                              'p_source_pos_index': k_sim.p_source_pos_index,
-                              'u_source_pos_index': k_sim.u_source_pos_index,
-                              's_source_pos_index': k_sim.s_source_pos_index,
-                              'transducer_input_signal': k_sim.transducer_input_signal,
-                              'delay_mask': k_sim.delay_mask,
-                              'sensor_mask_index': k_sim.sensor_mask_index,
-                              'record': k_sim.record,
-                          }),
-                          dotdict({
-                              'source_p': k_sim.source_p,
-                              'source_p0': k_sim.source_p0,
-
-                              'source_ux': k_sim.source_ux,
-                              'source_uy': k_sim.source_uy,
-                              'source_uz': k_sim.source_uz,
-
-                              'source_sxx': k_sim.source_sxx,
-                              'source_syy': k_sim.source_syy,
-                              'source_szz': k_sim.source_szz,
-                              'source_sxy': k_sim.source_sxy,
-                              'source_sxz': k_sim.source_sxz,
-                              'source_syz': k_sim.source_syz,
-
-                              'transducer_source': k_sim.transducer_source,
-                              'nonuniform_grid': k_sim.nonuniform_grid,
-                              'elastic_code': k_sim.options.simulation_type.is_elastic_simulation(),
-                              'axisymmetric': k_sim.options.simulation_type.is_axisymmetric(),
-                              'cuboid_corners': k_sim.cuboid_corners,
-                          }))
+        save_to_disk_func(
+            k_sim.kgrid,
+            k_sim.medium,
+            k_sim.source,
+            k_sim.options,
+            execution_options.auto_chunking,
+            dotdict(
+                {
+                    "ddx_k_shift_pos": k_sim.ddx_k_shift_pos,
+                    "ddx_k_shift_neg": k_sim.ddx_k_shift_neg,
+                    "dt": k_sim.dt,
+                    "c0": k_sim.c0,
+                    "c_ref": k_sim.c_ref,
+                    "rho0": k_sim.rho0,
+                    "rho0_sgx": k_sim.rho0_sgx,
+                    "rho0_sgy": k_sim.rho0_sgy,
+                    "rho0_sgz": k_sim.rho0_sgz,
+                    "p_source_pos_index": k_sim.p_source_pos_index,
+                    "u_source_pos_index": k_sim.u_source_pos_index,
+                    "s_source_pos_index": k_sim.s_source_pos_index,
+                    "transducer_input_signal": k_sim.transducer_input_signal,
+                    "delay_mask": k_sim.delay_mask,
+                    "sensor_mask_index": k_sim.sensor_mask_index,
+                    "record": k_sim.record,
+                }
+            ),
+            dotdict(
+                {
+                    "source_p": k_sim.source_p,
+                    "source_p0": k_sim.source_p0,
+                    "source_ux": k_sim.source_ux,
+                    "source_uy": k_sim.source_uy,
+                    "source_uz": k_sim.source_uz,
+                    "source_sxx": k_sim.source_sxx,
+                    "source_syy": k_sim.source_syy,
+                    "source_szz": k_sim.source_szz,
+                    "source_sxy": k_sim.source_sxy,
+                    "source_sxz": k_sim.source_sxz,
+                    "source_syz": k_sim.source_syz,
+                    "transducer_source": k_sim.transducer_source,
+                    "nonuniform_grid": k_sim.nonuniform_grid,
+                    "elastic_code": k_sim.options.simulation_type.is_elastic_simulation(),
+                    "axisymmetric": k_sim.options.simulation_type.is_axisymmetric(),
+                    "cuboid_corners": k_sim.cuboid_corners,
+                }
+            ),
+        )
 
         # run subscript to resize the transducer object if the grid has been expanded
         retract_transducer_grid_size(k_sim.source, k_sim.sensor, retract_size, k_sim.options.pml_inside)
 
         # exit matlab computation if required
         if options.save_to_disk_exit:
             return
 
         executor = Executor(simulation_options=simulation_options, execution_options=execution_options)
         executor_options = execution_options.get_options_string(sensor=k_sim.sensor)
-        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename,
-                                              options=executor_options)
+        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename, options=executor_options)
         return sensor_data
```

### Comparing `k_wave_python-0.3.2/kwave/kspaceFirstOrderAS.py` & `k_wave_python-0.3.3/kwave/kspaceFirstOrderAS.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 from kwave.utils.math import sinc
 from kwave.utils.matrix import num_dim2
 from kwave.utils.pml import get_pml
 from kwave.utils.tictoc import TicToc
 
 
 def kspaceFirstOrderASC(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     Axisymmetric time-domain simulation of wave propagation using C++ code.
 
     kspaceFirstOrderASC provides a blind interface to the C++ version of
     kspaceFirstOrderAS (called kspaceFirstOrder-OMP) in the same way as
     kspaceFirstOrder3DC. Note, the C++ code does not support all input
@@ -73,31 +73,26 @@
     Args:
         **kwargs:
 
     Returns:
     """
     # generate the input file and save to disk
     sensor_data = kspaceFirstOrderAS(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options,
-        execution_options=execution_options
+        kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options, execution_options=execution_options
     )
     return sensor_data
 
 
 def kspaceFirstOrderAS(
-        kgrid: kWaveGrid,
-        source: kSource,
-        sensor: Union[NotATransducer, kSensor],
-        medium: kWaveMedium,
-        simulation_options: SimulationOptions,
-        execution_options: SimulationExecutionOptions
+    kgrid: kWaveGrid,
+    source: kSource,
+    sensor: Union[NotATransducer, kSensor],
+    medium: kWaveMedium,
+    simulation_options: SimulationOptions,
+    execution_options: SimulationExecutionOptions,
 ):
     """
     Axisymmetric time-domain simulation of wave propagation.
 
     kspaceFirstOrderAS simulates the time-domain propagation of
     compressional waves through an axisymmetric homogeneous or
     heterogeneous acoustic medium. The code is functionally very similar
@@ -157,26 +152,22 @@
     Returns:
 
     """
     # start the timer and store the start time
     TicToc.tic()
 
     if simulation_options.simulation_type is not SimulationType.AXISYMMETRIC:
-        logging.log(logging.WARN,  "simulation type is not set to axisymmetric while using kSapceFirstOrderAS. "
-              "Setting simulation type to axisymmetric.")
+        logging.log(
+            logging.WARN,
+            "simulation type is not set to axisymmetric while using kSapceFirstOrderAS. " "Setting simulation type to axisymmetric.",
+        )
         simulation_options.simulation_type = SimulationType.AXISYMMETRIC
 
-    k_sim = kWaveSimulation(
-        kgrid=kgrid,
-        source=source,
-        sensor=sensor,
-        medium=medium,
-        simulation_options=simulation_options
-    )
-    k_sim.input_checking('kspaceFirstOrderAS')
+    k_sim = kWaveSimulation(kgrid=kgrid, source=source, sensor=sensor, medium=medium, simulation_options=simulation_options)
+    k_sim.input_checking("kspaceFirstOrderAS")
 
     # =========================================================================
     # CALCULATE MEDIUM PROPERTIES ON STAGGERED GRID
     # =========================================================================
     options = k_sim.options
 
     # interpolate the values of the density at the staggered grid locations
@@ -231,65 +222,67 @@
     #    - there is no explicit grid shift (this is done by choosing DTTs
     #      with the appropriate symmetry)
     #    - ifftshift isn't required as the wavenumbers start from DC
     # when using FFTs:
     #    - the grid is expanded, and the fields replicated in the radial
     #      dimension to give the required symmetry
     #    - the derivative and shift operators are defined as normal
-    if options.radial_symmetry in ['WSWA-FFT', 'WSWS-FFT']:
+    if options.radial_symmetry in ["WSWA-FFT", "WSWS-FFT"]:
         # create a new kWave grid object with expanded radial grid
-        if options.radial_symmetry == 'WSWA-FFT':
+        if options.radial_symmetry == "WSWA-FFT":
             # extend grid by a factor of x4 to account for
             # symmetries in WSWA
             kgrid_exp = kWaveGrid([Nx, Ny * 4], [dx, dy])
-        elif options.radial_symmetry == 'WSWS-FFT':
+        elif options.radial_symmetry == "WSWS-FFT":
             # extend grid by a factor of x2 - 2 to account for
             # symmetries in WSWS
             kgrid_exp = kWaveGrid([Nx, Ny * 2 - 2], [dx, dy])
         # define operators, rotating y-direction for use with bsxfun
         k_sim.ddy_k = ifftshift(1j * k_sim.kgrid.k_vec.y).T
         k_sim.y_shift_pos = ifftshift(np.exp(1j * kgrid_exp.k_vec.y * kgrid_exp.dy / 2)).T
         k_sim.y_shift_neg = ifftshift(np.exp(-1j * kgrid_exp.k_vec.y * kgrid_exp.dy / 2)).T
 
         # define the k-space operator
         if options.use_kspace:
             k_sim.kappa = ifftshift(sinc(c_ref * kgrid_exp.k * dt / 2))
-            if (k_sim.source_p and (k_sim.source.p_mode == 'additive')) or (
-                    (k_sim.source_ux or k_sim.source_uy) and (k_sim.source.u_mode == 'additive')):
+            if (k_sim.source_p and (k_sim.source.p_mode == "additive")) or (
+                (k_sim.source_ux or k_sim.source_uy) and (k_sim.source.u_mode == "additive")
+            ):
                 k_sim.source_kappa = ifftshift(np.cos(c_ref * kgrid_exp.k * dt / 2))
         else:
             k_sim.kappa = 1
             k_sim.source_kappa = 1
-    elif options.radial_symmetry in ['WSWA', 'WSWS']:
-        if options.radial_symmetry == 'WSWA':
+    elif options.radial_symmetry in ["WSWA", "WSWS"]:
+        if options.radial_symmetry == "WSWA":
             # get the wavenumbers and implied length for the DTTs
             ky_vec, M = k_sim.kgrid.ky_vec_dtt(DiscreteCosine.TYPE_3)
 
             # define the derivative operators
             k_sim.ddy_k_wswa = -ky_vec.T
             k_sim.ddy_k_hahs = ky_vec.T
-        elif options.radial_symmetry == 'WSWS':
+        elif options.radial_symmetry == "WSWS":
             # get the wavenumbers and implied length for the DTTs
             ky_vec, M = k_sim.kgrid.ky_vec_dtt(DiscreteCosine.TYPE_1)
 
             # define the derivative operators
             k_sim.ddy_k_wsws = -ky_vec[1:].T
             k_sim.ddy_k_haha = ky_vec[1:].T
 
         # define the k-space operator
         if options.use_kspace:
             # define scalar wavenumber
-            k_dtt = np.sqrt(np.tile(ifftshift(k_sim.kgrid.k_vec.x) ** 2, [1, k_sim.kgrid.Ny]) + np.tile((ky_vec.T) ** 2,
-                                                                                                        [k_sim.kgrid.Nx,
-                                                                                                         1]))
+            k_dtt = np.sqrt(
+                np.tile(ifftshift(k_sim.kgrid.k_vec.x) ** 2, [1, k_sim.kgrid.Ny]) + np.tile((ky_vec.T) ** 2, [k_sim.kgrid.Nx, 1])
+            )
 
             # define k-space operators
             k_sim.kappa = sinc(c_ref * k_dtt * k_sim.kgrid.dt / 2)
-            if (k_sim.source_p and (k_sim.source.p_mode == 'additive')) or (
-                    (k_sim.source_ux or k_sim.source_uy) and (k_sim.source.u_mode == 'additive')):
+            if (k_sim.source_p and (k_sim.source.p_mode == "additive")) or (
+                (k_sim.source_ux or k_sim.source_uy) and (k_sim.source.u_mode == "additive")
+            ):
                 k_sim.source_kappa = np.cos(c_ref * k_dtt * k_sim.kgrid.dt / 2)
 
             # cleanup unused variables
             del k_dtt
 
         else:
             k_sim.kappa = 1
@@ -297,73 +290,79 @@
 
     # define staggered and non-staggered grid axial distance
     k_sim.y_vec = (k_sim.kgrid.y_vec - k_sim.kgrid.y_vec[0]).T
     k_sim.y_vec_sg = (k_sim.kgrid.y_vec - k_sim.kgrid.y_vec[0] + k_sim.kgrid.dy / 2).T
 
     # option to run simulations without the spatial staggered grid is not
     # supported for the axisymmetric code
-    assert options.use_sg, 'Optional input ''UseSG'' is not supported for axisymmetric simulations.'
+    assert options.use_sg, "Optional input " "UseSG" " is not supported for axisymmetric simulations."
 
     # =========================================================================
     # SAVE DATA TO DISK FOR RUNNING SIMULATION EXTERNAL TO MATLAB
     # =========================================================================
 
     # save to disk option for saving the input matrices to disk for running
     # simulations using k-Wave++
     if options.save_to_disk:
         # store the pml size for resizing transducer object below
         retract_size = [[options.pml_x_size, options.pml_y_size, options.pml_z_size]]
 
         # run subscript to save files to disk
-        save_to_disk_func(k_sim.kgrid, k_sim.medium, k_sim.source, k_sim.options, execution_options.auto_chunking,
-                          dotdict({
-                              'ddx_k_shift_pos': k_sim.ddx_k_shift_pos,
-                              'ddx_k_shift_neg': k_sim.ddx_k_shift_neg,
-                              'dt': k_sim.dt,
-                              'c0': k_sim.c0,
-                              'c_ref': k_sim.c_ref,
-                              'rho0': k_sim.rho0,
-                              'rho0_sgx': k_sim.rho0_sgx,
-                              'rho0_sgy': k_sim.rho0_sgy,
-                              'rho0_sgz': k_sim.rho0_sgz,
-                              'p_source_pos_index': k_sim.p_source_pos_index,
-                              'u_source_pos_index': k_sim.u_source_pos_index,
-                              's_source_pos_index': k_sim.s_source_pos_index,
-                              'transducer_input_signal': k_sim.transducer_input_signal,
-                              'delay_mask': k_sim.delay_mask,
-                              'sensor_mask_index': k_sim.sensor_mask_index,
-                              'record': k_sim.record,
-                          }),
-                          dotdict({
-                              'source_p': k_sim.source_p,
-                              'source_p0': k_sim.source_p0,
-
-                              'source_ux': k_sim.source_ux,
-                              'source_uy': k_sim.source_uy,
-                              'source_uz': k_sim.source_uz,
-
-                              'source_sxx': k_sim.source_sxx,
-                              'source_syy': k_sim.source_syy,
-                              'source_szz': k_sim.source_szz,
-                              'source_sxy': k_sim.source_sxy,
-                              'source_sxz': k_sim.source_sxz,
-                              'source_syz': k_sim.source_syz,
-
-                              'transducer_source': k_sim.transducer_source,
-                              'nonuniform_grid': k_sim.nonuniform_grid,
-                              'elastic_code': k_sim.options.simulation_type.is_elastic_simulation(),
-                              'axisymmetric': k_sim.options.simulation_type.is_axisymmetric(),
-                              'cuboid_corners': k_sim.cuboid_corners,
-                          }))
+        save_to_disk_func(
+            k_sim.kgrid,
+            k_sim.medium,
+            k_sim.source,
+            k_sim.options,
+            execution_options.auto_chunking,
+            dotdict(
+                {
+                    "ddx_k_shift_pos": k_sim.ddx_k_shift_pos,
+                    "ddx_k_shift_neg": k_sim.ddx_k_shift_neg,
+                    "dt": k_sim.dt,
+                    "c0": k_sim.c0,
+                    "c_ref": k_sim.c_ref,
+                    "rho0": k_sim.rho0,
+                    "rho0_sgx": k_sim.rho0_sgx,
+                    "rho0_sgy": k_sim.rho0_sgy,
+                    "rho0_sgz": k_sim.rho0_sgz,
+                    "p_source_pos_index": k_sim.p_source_pos_index,
+                    "u_source_pos_index": k_sim.u_source_pos_index,
+                    "s_source_pos_index": k_sim.s_source_pos_index,
+                    "transducer_input_signal": k_sim.transducer_input_signal,
+                    "delay_mask": k_sim.delay_mask,
+                    "sensor_mask_index": k_sim.sensor_mask_index,
+                    "record": k_sim.record,
+                }
+            ),
+            dotdict(
+                {
+                    "source_p": k_sim.source_p,
+                    "source_p0": k_sim.source_p0,
+                    "source_ux": k_sim.source_ux,
+                    "source_uy": k_sim.source_uy,
+                    "source_uz": k_sim.source_uz,
+                    "source_sxx": k_sim.source_sxx,
+                    "source_syy": k_sim.source_syy,
+                    "source_szz": k_sim.source_szz,
+                    "source_sxy": k_sim.source_sxy,
+                    "source_sxz": k_sim.source_sxz,
+                    "source_syz": k_sim.source_syz,
+                    "transducer_source": k_sim.transducer_source,
+                    "nonuniform_grid": k_sim.nonuniform_grid,
+                    "elastic_code": k_sim.options.simulation_type.is_elastic_simulation(),
+                    "axisymmetric": k_sim.options.simulation_type.is_axisymmetric(),
+                    "cuboid_corners": k_sim.cuboid_corners,
+                }
+            ),
+        )
 
         # run subscript to resize the transducer object if the grid has been expanded
         retract_transducer_grid_size(k_sim.source, k_sim.sensor, retract_size, k_sim.options.pml_inside)
 
         # exit matlab computation if required
         if options.save_to_disk_exit:
             return
 
         executor = Executor(simulation_options=simulation_options, execution_options=execution_options)
         executor_options = execution_options.get_options_string(sensor=k_sim.sensor)
-        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename,
-                                              options=executor_options)
+        sensor_data = executor.run_simulation(k_sim.options.input_filename, k_sim.options.output_filename, options=executor_options)
         return sensor_data
```

### Comparing `k_wave_python-0.3.2/kwave/ktransducer.py` & `k_wave_python-0.3.3/kwave/ktransducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,66 +12,66 @@
 
 # force value to be a positive integer
 def make_pos_int(val):
     return np.abs(val).astype(int)
 
 
 class kWaveTransducerSimple(object):
-
     def __init__(
-            self,
-            kgrid: kWaveGrid,
-            number_elements=128,
-            element_width=1,
-            element_length=20,
-            element_spacing=0,
-            position=None,
-            radius=float('inf')
+        self,
+        kgrid: kWaveGrid,
+        number_elements=128,
+        element_width=1,
+        element_length=20,
+        element_spacing=0,
+        position=None,
+        radius=float("inf"),
     ):
         """
         Args:
             kgrid: kWaveGrid object
             number_elements: the total number of transducer elements
             element_width: the width of each element in grid points
             element_length: the length of each element in grid points
             element_spacing: the spacing (kerf width) between the transducer elements in grid points
             position: the position of the corner of the transducer in the grid
             radius: the radius of curvature of the transducer [m]
 
         """
 
         # allocate the grid size and spacing
-        self.stored_grid_size = [kgrid.Nx, kgrid.Ny, kgrid.Nz]    # size of the grid in which the transducer is defined
-        self.grid_spacing = [kgrid.dx, kgrid.dy, kgrid.dz]        # corresponding grid spacing
+        self.stored_grid_size = [kgrid.Nx, kgrid.Ny, kgrid.Nz]  # size of the grid in which the transducer is defined
+        self.grid_spacing = [kgrid.dx, kgrid.dy, kgrid.dz]  # corresponding grid spacing
 
         self.number_elements = make_pos_int(number_elements)
         self.element_width = make_pos_int(element_width)
         self.element_length = make_pos_int(element_length)
         self.element_spacing = make_pos_int(element_spacing)
 
         if position is None:
             position = [1, 1, 1]
         self.position = make_pos_int(position)
 
-        assert np.isinf(radius), 'Only a value of transducer.radius = inf is currently supported'
+        assert np.isinf(radius), "Only a value of transducer.radius = inf is currently supported"
         self.radius = radius
 
         # check the transducer fits into the grid
         if np.sum(self.position == 0):
-            raise ValueError('The defined transducer must be positioned within the grid')
-        elif (self.position[1] + self.number_elements * self.element_width + (
-                self.number_elements - 1) * self.element_spacing) > self.stored_grid_size[1]:
-            raise ValueError('The defined transducer is too large or positioned outside the grid in the y-direction')
+            raise ValueError("The defined transducer must be positioned within the grid")
+        elif (
+            self.position[1] + self.number_elements * self.element_width + (self.number_elements - 1) * self.element_spacing
+        ) > self.stored_grid_size[1]:
+            raise ValueError("The defined transducer is too large or positioned outside the grid in the y-direction")
         elif (self.position[2] + self.element_length) > self.stored_grid_size[2]:
             logging.log(logging.INFO, self.position[2])
             logging.log(logging.INFO, self.element_length)
             logging.log(logging.INFO, self.stored_grid_size[2])
-            raise ValueError('The defined transducer is too large or positioned outside the grid in the z-direction')
+            raise ValueError("The defined transducer is too large or positioned outside the grid in the z-direction")
         elif self.position[0] > self.stored_grid_size[0]:
-            raise ValueError('The defined transducer is positioned outside the grid in the x-direction')
+            raise ValueError("The defined transducer is positioned outside the grid in the x-direction")
 
     @property
     def element_pitch(self):
         return (self.element_spacing + self.element_width) * self.grid_spacing[1]
 
     @property
     def transducer_width(self):
@@ -83,118 +83,119 @@
             the overall length of the transducer
 
         """
         return self.number_elements * self.element_width + (self.number_elements - 1) * self.element_spacing
 
 
 class NotATransducer(kSensor):
-
     def __init__(
-            self,
-            transducer: kWaveTransducerSimple,
-            kgrid: kWaveGrid,
-            active_elements=None,
-            focus_distance=float('inf'),
-            elevation_focus_distance=float('inf'),
-            receive_apodization='Rectangular',
-            transmit_apodization='Rectangular',
-            sound_speed=1540,
-            input_signal=None,
-            steering_angle_max=None,
-            steering_angle=None
+        self,
+        transducer: kWaveTransducerSimple,
+        kgrid: kWaveGrid,
+        active_elements=None,
+        focus_distance=float("inf"),
+        elevation_focus_distance=float("inf"),
+        receive_apodization="Rectangular",
+        transmit_apodization="Rectangular",
+        sound_speed=1540,
+        input_signal=None,
+        steering_angle_max=None,
+        steering_angle=None,
     ):
         """
         'time_reversal_boundary_data' and 'record' fields should not be defined
         for the objects of this class
 
         Args:
             kgrid: kWaveGrid object
             active_elements: the transducer elements that are currently active elements
             elevation_focus_distance: the focus depth in the elevation direction [m]
             receive_apodization: transmit apodization
             transmit_apodization: receive apodization
             sound_speed: sound speed used to calculate beamforming delays [m/s]
             focus_distance: focus distance used to calculate beamforming delays [m]
             input_signal:
-            steering_angle_max:
-            steering_angle:
+            steering_angle_max: max steering angle [deg]
+            steering_angle: steering angle [deg]
 
         """
 
         super().__init__()
         assert isinstance(transducer, kWaveTransducerSimple)
         self.transducer = transducer
         # time index to start recording if transducer is used as a sensor
         self.record_start_index = 1
         # stored value of appended_zeros (accessed using get and set methods).
         # This is used to set the number of zeros that are appended and prepended to the input signal.
-        self.stored_appended_zeros = 'auto'
+        self.stored_appended_zeros = "auto"
         # stored value of the minimum beamforming delay.
         # This is used to offset the delay mask so that all the delays are >= 0
-        self.stored_beamforming_delays_offset = 'auto'
+        self.stored_beamforming_delays_offset = "auto"
         # stored value of the steering_angle_max (accessed using get and set methods).
         # This can be set by the user and is used to derive the two parameters above.
-        self.stored_steering_angle_max = 'auto'
+        self.stored_steering_angle_max = "auto"
         # stored value of the steering_angle (accessed using get and set methods)
         self.stored_steering_angle = 0
 
         ####################################
         # if the sensor is a transducer, check that the simulation is in 3D
-        assert kgrid.dim == 3, 'Transducer inputs are only compatible with 3D simulations.'
+        assert kgrid.dim == 3, "Transducer inputs are only compatible with 3D simulations."
 
         ####################################
 
         # allocate the temporal spacing
         if is_number(kgrid.dt):
             self.dt = kgrid.dt
         elif kgrid.t_array is not None:
             self.dt = kgrid.t_array[1] - kgrid.t_array[0]
         else:
-            raise ValueError('kgrid.dt or kgrid.t_array must be explicitly defined')
+            raise ValueError("kgrid.dt or kgrid.t_array must be explicitly defined")
 
         if active_elements is None:
             active_elements = np.ones((transducer.number_elements, 1))
         self.active_elements = active_elements
 
         self.elevation_focus_distance = elevation_focus_distance
 
         # check the length of the input
-        assert not is_number(receive_apodization) or len(receive_apodization) == self.number_active_elements, \
-            'The length of the receive apodization input must match the number of active elements'
+        assert (
+            not is_number(receive_apodization) or len(receive_apodization) == self.number_active_elements
+        ), "The length of the receive apodization input must match the number of active elements"
         self.receive_apodization = receive_apodization
 
         # check the length of the input
-        assert not is_number(transmit_apodization) or len(transmit_apodization) == self.number_active_elements, \
-            'The length of the transmit apodization input must match the number of active elements'
+        assert (
+            not is_number(transmit_apodization) or len(transmit_apodization) == self.number_active_elements
+        ), "The length of the transmit apodization input must match the number of active elements"
         self.transmit_apodization = transmit_apodization
 
         # check to see the sound_speed is positive
-        assert sound_speed > 0, 'transducer.sound_speed must be greater than 0'
+        assert sound_speed > 0, "transducer.sound_speed must be greater than 0"
         self.sound_speed = sound_speed
 
         self.focus_distance = focus_distance
 
         if input_signal is not None:
             input_signal = np.squeeze(input_signal)
-            assert input_signal.ndim == 1, 'transducer.input_signal must be a one-dimensional array'
+            assert input_signal.ndim == 1, "transducer.input_signal must be a one-dimensional array"
             self.stored_input_signal = np.atleast_2d(input_signal).T  # force the input signal to be a column vector
 
         if steering_angle_max is not None:
             # set the maximum steering angle using the set method (this avoids having to duplicate error checking)
             self.steering_angle_max = steering_angle_max
 
         if steering_angle is not None:
             # set the maximum steering angle using the set method (this
             # avoids having to duplicate error checking)
             self.steering_angle = steering_angle
 
         # assign the data type for the transducer matrix based on the
         # number of different elements (uint8 supports 255 numbers so
         # most of the time this data type will be used)
-        mask_type = get_smallest_possible_type(transducer.number_elements, 'uint')
+        mask_type = get_smallest_possible_type(transducer.number_elements, "uint")
 
         # create an empty transducer mask (the grid points within
         # element 'n' are all given the value 'n')
         assert transducer.stored_grid_size is not None
         self.indexed_mask = np.zeros(transducer.stored_grid_size, dtype=mask_type)
 
         # create a second empty mask used for the elevation beamforming
@@ -215,25 +216,32 @@
 
             element_pos_x = element_pos_x - 1
             element_pos_y = element_pos_y - 1
             element_pos_z = element_pos_z - 1
 
             # assign the grid points within the current element the
             # index of the element
-            self.indexed_mask[element_pos_x, element_pos_y:element_pos_y + transducer.element_width,
-            element_pos_z:element_pos_z + transducer.element_length] = element_index + 1
+            self.indexed_mask[
+                element_pos_x,
+                element_pos_y : element_pos_y + transducer.element_width,
+                element_pos_z : element_pos_z + transducer.element_length,
+            ] = element_index + 1
 
             # assign the individual grid points an index corresponding
             # to their order across the element
-            self.indexed_element_voxel_mask[element_pos_x, element_pos_y:element_pos_y + transducer.element_width,
-            element_pos_z:element_pos_z + transducer.element_length] = element_voxel_index
+            self.indexed_element_voxel_mask[
+                element_pos_x,
+                element_pos_y : element_pos_y + transducer.element_width,
+                element_pos_z : element_pos_z + transducer.element_length,
+            ] = element_voxel_index
 
         # double check the transducer fits within the desired grid size
-        assert (np.array(self.indexed_mask.shape) == transducer.stored_grid_size).all(), \
-            'Desired transducer is larger than the input grid_size'
+        assert (
+            np.array(self.indexed_mask.shape) == transducer.stored_grid_size
+        ).all(), "Desired transducer is larger than the input grid_size"
 
         self.sxx = self.syy = self.szz = self.sxy = self.sxz = self.syz = None
         self.u_mode = self.p_mode = None
         self.ux = self.uy = self.uz = None
 
     @staticmethod
     def isfield(_):
@@ -254,26 +262,31 @@
         element_pitch = self.transducer.element_pitch
 
         # create indexing variable
         element_index = np.arange(-(self.number_active_elements - 1) / 2, (self.number_active_elements + 1) / 2)
 
         # check for focus depth
         if np.isinf(self.focus_distance):
-
             # calculate time delays for a steered beam
-            delay_times = element_pitch * element_index * \
-                          np.sin(self.steering_angle * np.pi / 180) / self.sound_speed  # [s]
+            delay_times = element_pitch * element_index * np.sin(self.steering_angle * np.pi / 180) / self.sound_speed  # [s]
 
         else:
-
             # calculate time delays for a steered and focussed beam
-            delay_times = self.focus_distance / self.sound_speed * (
-                    1 - np.sqrt(1 + (element_index * element_pitch / self.focus_distance) ** 2
-                                - 2 * (element_index * element_pitch / self.focus_distance) * np.sin(
-                self.steering_angle * np.pi / 180)))  # [s]
+            delay_times = (
+                self.focus_distance
+                / self.sound_speed
+                * (
+                    1
+                    - np.sqrt(
+                        1
+                        + (element_index * element_pitch / self.focus_distance) ** 2
+                        - 2 * (element_index * element_pitch / self.focus_distance) * np.sin(self.steering_angle * np.pi / 180)
+                    )
+                )
+            )  # [s]
 
         # convert the delays to be in units of time points
         delay_times = (delay_times / self.dt).round().astype(int)
         return delay_times
 
     @property
     def beamforming_delays_offset(self):
@@ -326,38 +339,39 @@
     # set the stored value of the steering angle
     @steering_angle.setter
     def steering_angle(self, steering_angle):
         # force to be scalar
         steering_angle = float(steering_angle)
 
         # check if the steering angle is between -90 and 90
-        assert -90 < steering_angle < 90, 'Input for steering_angle must be betweeb -90 and 90 degrees.'
+        assert -90 < steering_angle < 90, "Input for steering_angle must be betweeb -90 and 90 degrees."
 
         # check if the steering angle is less than the maximum steering angle
-        if self.stored_steering_angle_max != 'auto' and (abs(steering_angle) > self.stored_steering_angle_max):
-            raise ValueError('Input for steering_angle cannot be greater than steering_angle_max.')
+        if self.stored_steering_angle_max != "auto" and (abs(steering_angle) > self.stored_steering_angle_max):
+            raise ValueError("Input for steering_angle cannot be greater than steering_angle_max.")
 
         # update the stored value
         self.stored_steering_angle = steering_angle
 
     @property
     def steering_angle_max(self):
         return self.stored_steering_angle_max
 
     @steering_angle_max.setter
     def steering_angle_max(self, steering_angle_max):
         # force input to be scalar and positive
         steering_angle_max = float(steering_angle_max)
 
         # check the steering angle is within range
-        assert -90 < steering_angle_max < 90, 'Input for steering_angle_max must be between -90 and 90.'
+        assert -90 < steering_angle_max < 90, "Input for steering_angle_max must be between -90 and 90."
 
         # check the maximum steering angle is greater than the current steering angle
-        assert self.stored_steering_angle_max == 'auto' or abs(self.stored_steering_angle) <= steering_angle_max, \
-            'Input for steering_angle_max cannot be less than the current steering_angle.'
+        assert (
+            self.stored_steering_angle_max == "auto" or abs(self.stored_steering_angle) <= steering_angle_max
+        ), "Input for steering_angle_max cannot be less than the current steering_angle."
 
         # overwrite the stored value
         self.stored_steering_angle_max = steering_angle_max
 
         # store a copy of the current value for the steering angle
         current_steering_angle = self.stored_steering_angle
 
@@ -381,15 +395,15 @@
             min_delay = min_delay + min(self.elevation_beamforming_delays)
 
         # set the beamforming offset to the difference between the
         # maximum and minimum delay
         self.stored_appended_zeros = max_delay - min_delay
 
         # set the minimum beamforming delay (converting to a positive number)
-        self.stored_beamforming_delays_offset = - min_delay
+        self.stored_beamforming_delays_offset = -min_delay
 
         # reset the previous value of the steering angle
         self.stored_steering_angle = current_steering_angle
 
     @property
     def elevation_beamforming_mask(self):  # nr
         # get elevation beamforming mask
@@ -412,26 +426,25 @@
         return np.fliplr(mask)
 
     @property
     def input_signal(self):
         signal = self.stored_input_signal
 
         # check the signal is not empty
-        assert signal is not None, 'Transducer input signal is not defined'
+        assert signal is not None, "Transducer input signal is not defined"
 
         # automatically prepend and append zeros if the beamforming
         # delay offset is set
 
         # check if the beamforming delay offset is set. If so, use this
         # number to prepend and append this number of zeros to the
         # input signal. Otherwise, calculate how many zeros are needed
         # and prepend and append these.
         stored_appended_zeros = self.stored_appended_zeros
-        if stored_appended_zeros != 'auto':
-
+        if stored_appended_zeros != "auto":
             # use the current value of the beamforming offset to add
             # zeros to the input signal
             signal = np.vstack([np.zeros((stored_appended_zeros, 1)), signal, np.zeros((stored_appended_zeros, 1))])
 
         else:
             # get the current delay beam forming
             delay_mask = self.delay_mask()
@@ -444,25 +457,23 @@
 
             # count the number of trailing zeros in the input signal
             trailing_zeros = matlab_find(np.flipud(signal))[0, 0] - 1
 
             # check the number of leading zeros is sufficient given the
             # maximum delay
             if leading_zeros < delay_max + 1:
-
-                logging.log(logging.INFO, f'  prepending transducer.input_signal with {delay_max - leading_zeros + 1} leading zeros')
+                logging.log(logging.INFO, f"  prepending transducer.input_signal with {delay_max - leading_zeros + 1} leading zeros")
 
                 # prepend extra leading zeros
                 signal = np.vstack([np.zeros((delay_max - leading_zeros + 1, 1)), signal])
 
             # check the number of leading zeros is sufficient given the
             # maximum delay
             if trailing_zeros < delay_max + 1:
-
-                logging.log(logging.INFO, f'  appending transducer.input_signal with {delay_max - trailing_zeros + 1} trailing zeros')
+                logging.log(logging.INFO, f"  appending transducer.input_signal with {delay_max - trailing_zeros + 1} trailing zeros")
 
                 # append extra trailing zeros
                 signal = np.vstack([signal, np.zeros((delay_max - trailing_zeros + 1, 1))])
 
         return signal
 
     @property
@@ -527,17 +538,15 @@
         self.indexed_mask = expand_matrix(self.indexed_mask, expand_size, 0)
 
     def retract_grid(self, retract_size):
         indexed_mask = self.indexed_mask
         retract_size = np.array(retract_size[0]).astype(np.int_)
 
         self.indexed_mask = indexed_mask[
-            retract_size[0]:-retract_size[0],
-            retract_size[1]:-retract_size[1],
-            retract_size[2]:-retract_size[2]
+            retract_size[0] : -retract_size[0], retract_size[1] : -retract_size[1], retract_size[2] : -retract_size[2]
         ]
 
     @property
     def transmit_apodization_mask(self):
         """
         convert the transmit wave apodization into the form of a element mask,
         where the apodization values are placed at the grid points
@@ -553,36 +562,36 @@
 
         # create an empty mask;
         mask = np.zeros(self.transducer.stored_grid_size)
 
         # assign the apodization values to every grid point in the transducer
         mask_index = self.indexed_active_elements_mask
         mask_index = mask_index[mask_index != 0]
-        mask[self.active_elements_mask == 1] = apodization[mask_index - 1, 0]   # -1 for conversion
+        mask[self.active_elements_mask == 1] = apodization[mask_index - 1, 0]  # -1 for conversion
         return mask
 
     def get_transmit_apodization(self):
         """
         Returns:
             return the transmit apodization, converting strings of window
             type to actual numbers using getWin
 
         """
 
         # check if a user defined apodization is given and whether this
         # is still the correct size (in case the number of active
         # elements has changed)
         if is_number(self.transmit_apodization):
-            assert self.transmit_apodization.size == self.number_active_elements, \
-                'The length of the transmit apodization input must match the number of active elements'
+            assert (
+                self.transmit_apodization.size == self.number_active_elements
+            ), "The length of the transmit apodization input must match the number of active elements"
 
             # assign apodization
             apodization = self.transmit_apodization
         else:
-
             # if the number of active elements is greater than 1,
             # create apodization using getWin, otherwise, assign 1
             if self.number_active_elements > 1:
                 apodization, _ = get_win(int(self.number_active_elements), type_=self.transmit_apodization)
             else:
                 apodization = 1
         apodization = np.array(apodization)
@@ -602,68 +611,60 @@
         if indexed_active_elements_mask_copy is None:
             return mask
 
         active_elements_index = matlab_find(indexed_active_elements_mask_copy)
 
         # calculate azimuth focus delay times provided they are not all zero
         if (not np.isinf(self.focus_distance) or (self.steering_angle != 0)) and (mode is None or mode != 2):
-
             # get the element beamforming delays and reverse
             delay_times = -self.beamforming_delays
 
             # add delay times
             # mask[active_elements_index] = delay_times[indexed_active_elements_mask_copy[active_elements_index]]
             mask[unflatten_matlab_mask(mask, active_elements_index, diff=-1)] = matlab_mask(
-                delay_times,
-                matlab_mask(indexed_active_elements_mask_copy, active_elements_index, diff=-1),
-                diff=-1
+                delay_times, matlab_mask(indexed_active_elements_mask_copy, active_elements_index, diff=-1), diff=-1
             ).squeeze()
 
         # calculate elevation focus time delays provided each element is longer than one grid point
-        if not np.isinf(self.elevation_focus_distance) and \
-                (self.transducer.element_length > 1) and (mode is None or mode != 3):
-
+        if not np.isinf(self.elevation_focus_distance) and (self.transducer.element_length > 1) and (mode is None or mode != 3):
             # get elevation beamforming delays
             elevation_delay_times = self.elevation_beamforming_delays
 
             # get current mask
             element_voxel_mask = self.indexed_element_voxel_mask
 
             # add delay times
             mask[unflatten_matlab_mask(mask, active_elements_index - 1)] += matlab_mask(
-                elevation_delay_times,
-                matlab_mask(element_voxel_mask, active_elements_index - 1) - 1
+                elevation_delay_times, matlab_mask(element_voxel_mask, active_elements_index - 1) - 1
             )[:, 0]  # -1s compatibility
 
         # shift delay times (these should all be >= 0, where a value of 0 means no delay)
-        if self.stored_appended_zeros == 'auto':
-            mask[unflatten_matlab_mask(mask, active_elements_index - 1)] -= \
-                mask[unflatten_matlab_mask(mask, active_elements_index - 1)].min()  # -1s compatibility
+        if self.stored_appended_zeros == "auto":
+            mask[unflatten_matlab_mask(mask, active_elements_index - 1)] -= mask[
+                unflatten_matlab_mask(mask, active_elements_index - 1)
+            ].min()  # -1s compatibility
         else:
-            mask[unflatten_matlab_mask(mask, active_elements_index - 1)] += \
-                self.stored_beamforming_delays_offset  # -1s compatibility
+            mask[unflatten_matlab_mask(mask, active_elements_index - 1)] += self.stored_beamforming_delays_offset  # -1s compatibility
         return mask.astype(np.uint8)
 
     @property
     def elevation_beamforming_delays(self):
         """
         Calculate the elevation beamforming delays based on the focus setting
 
         """
         if not np.isinf(self.elevation_focus_distance):
             # create indexing variable
 
             element_index = np.arange(-(self.transducer.element_length - 1) / 2, (self.transducer.element_length + 1) / 2)
 
             # calculate time delays for a focussed beam
-            delay_times = self.elevation_focus_distance - \
-                          np.sqrt(
-                              (element_index * self.transducer.grid_spacing[2]) ** 2
-                              + self.elevation_focus_distance ** 2
-                          )
+            delay_times = self.elevation_focus_distance - np.sqrt(
+                (element_index * self.transducer.grid_spacing[2]) ** 2 + self.elevation_focus_distance**2
+            )
             delay_times /= self.sound_speed
 
             # convert the delays to be in units of time points and then reverse
             delay_times = -np.round(delay_times / self.dt).astype(np.int32)
 
         else:
             # create an empty array
@@ -672,16 +673,17 @@
 
     def get_receive_apodization(self):
         """
         Get the current receive apodization setting.
         """
         # Example implementation, adjust based on actual logic
         if is_number(self.receive_apodization):
-            assert self.receive_apodization.size == self.number_active_elements, \
-                'The length of the receive apodization input must match the number of active elements'
+            assert (
+                self.receive_apodization.size == self.number_active_elements
+            ), "The length of the receive apodization input must match the number of active elements"
             return self.receive_apodization
         else:
             if self.number_active_elements > 1:
                 apodization, _ = get_win(int(self.number_active_elements), type_=self.receive_apodization)
             else:
                 apodization = 1
         return np.array(apodization)
@@ -696,63 +698,66 @@
         # Get the current beamforming weights and reverse
         delays = -self.beamforming_delays
 
         # Offset the received sensor_data by the beamforming delays and apply receive apodization
         for element_index in range(self.number_active_elements):
             if delays[element_index] > 0:
                 # Shift element data forwards
-                sensor_data[element_index, :] = np.pad(sensor_data[element_index, delays[element_index]:],
-                                                       (0, delays[element_index]),
-                                                       'constant') * apodization[element_index]
+                sensor_data[element_index, :] = (
+                    np.pad(sensor_data[element_index, delays[element_index] :], (0, delays[element_index]), "constant")
+                    * apodization[element_index]
+                )
             elif delays[element_index] < 0:
                 # Shift element data backwards
-                sensor_data[element_index, :] = np.pad(sensor_data[element_index, :sensor_data.shape[1] + delays[element_index]],
-                                                       (-delays[element_index], 0),
-                                                       'constant') * apodization[element_index]
+                sensor_data[element_index, :] = (
+                    np.pad(
+                        sensor_data[element_index, : sensor_data.shape[1] + delays[element_index]], (-delays[element_index], 0), "constant"
+                    )
+                    * apodization[element_index]
+                )
 
         # Form the line summing across the elements
         line = np.sum(sensor_data, axis=0)
         return line
 
-
     def combine_sensor_data(self, sensor_data):
         # check the data is the correct size
         if sensor_data.shape[0] != (self.number_active_elements * self.transducer.element_width * self.transducer.element_length):
-            raise ValueError('The number of time series in the input sensor_data must '
-                             'match the number of grid points in the active tranducer elements.')
+            raise ValueError(
+                "The number of time series in the input sensor_data must "
+                "match the number of grid points in the active tranducer elements."
+            )
 
         # get index of which element each time series belongs to
         # Tricky things going on here
         ind = self.indexed_active_elements_mask[0].T[self.indexed_active_elements_mask[0].T > 0]
 
         # create empty output
         sensor_data_sum = np.zeros((int(self.number_active_elements), sensor_data.shape[1]))
 
         # check if an elevation focus is set
         if np.isinf(self.elevation_focus_distance):
-
             raise NotImplementedError
 
             # # loop over time series and sum
             # for ii = 1:length(ind)
             #     sensor_data_sum(ind(ii), :) = sensor_data_sum(ind(ii), :) + sensor_data(ii, :);
             # end
 
         else:
-
             # get the elevation delay for each grid point of each
             # active transducer element (this is given in units of grid
             # points)
             dm = self.delay_mask(2)
             # dm = dm[self.active_elements_mask != 0]
             dm = dm[0].T[self.active_elements_mask[0].T != 0]
             dm = dm.astype(np.int32)
 
             # loop over time series, shift and sum
             for ii in range(len(ind)):
                 # FARID: something nasty can be here
                 end = -dm[ii] if dm[ii] != 0 else sensor_data_sum.shape[-1]
-                sensor_data_sum[ind[ii]-1, 0:end] = sensor_data_sum[ind[ii]-1, 0:end] + sensor_data[ii, dm[ii]:]
+                sensor_data_sum[ind[ii] - 1, 0:end] = sensor_data_sum[ind[ii] - 1, 0:end] + sensor_data[ii, dm[ii] :]
 
         # divide by number of time series in each element
         sensor_data_sum = sensor_data_sum * (1 / (self.transducer.element_width * self.transducer.element_length))
         return sensor_data_sum
```

### Comparing `k_wave_python-0.3.2/kwave/recorder.py` & `k_wave_python-0.3.3/kwave/recorder.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 
 from kwave.data import Vector
 from kwave.kgrid import kWaveGrid
 
 
 @dataclass
 class Recorder(object):
-
     def __init__(self):
         # flags which control which parameters are recorded
-        self.p                  = True     #: time-varying acoustic pressure
-        self.p_max              = False    #: maximum pressure over simulation
-        self.p_min              = False    #: minimum pressure over simulation
-        self.p_rms              = False    #: root-mean-squared pressure over simulation
-        self.p_max_all          = False    #: maximum pressure over simulation at all grid points
-        self.p_min_all          = False    #: minimum pressure over simulation at all grid points
-        self.p_final            = False    #: final pressure field at all grid points
-        self.u                  = False    #: time-varying particle velocity
-        self.u_split_field      = False    #: compressional and shear components of time-varying particle velocity
-        self.u_non_staggered    = False    #: time-varying particle velocity on non-staggered grid
-        self.u_max              = False    #: maximum particle velocity over simulation
-        self.u_min              = False    #: minimum particle velocity over simulation
-        self.u_rms              = False    #: root-mean-squared particle velocity over simulation
-        self.u_max_all          = False    #: maximum particle velocity over simulation at all grid points
-        self.u_min_all          = False    #: minimum particle velocity over simulation at all grid points
-        self.u_final            = False    #: final particle velocity field at all grid points
-        self.I                  = False    #: time-varying acoustic intensity
-        self.I_avg              = False    #: time-averaged acoustic intensity
+        self.p = True  #: time-varying acoustic pressure
+        self.p_max = False  #: maximum pressure over simulation
+        self.p_min = False  #: minimum pressure over simulation
+        self.p_rms = False  #: root-mean-squared pressure over simulation
+        self.p_max_all = False  #: maximum pressure over simulation at all grid points
+        self.p_min_all = False  #: minimum pressure over simulation at all grid points
+        self.p_final = False  #: final pressure field at all grid points
+        self.u = False  #: time-varying particle velocity
+        self.u_split_field = False  #: compressional and shear components of time-varying particle velocity
+        self.u_non_staggered = False  #: time-varying particle velocity on non-staggered grid
+        self.u_max = False  #: maximum particle velocity over simulation
+        self.u_min = False  #: minimum particle velocity over simulation
+        self.u_rms = False  #: root-mean-squared particle velocity over simulation
+        self.u_max_all = False  #: maximum particle velocity over simulation at all grid points
+        self.u_min_all = False  #: minimum particle velocity over simulation at all grid points
+        self.u_final = False  #: final particle velocity field at all grid points
+        self.I = False  #: time-varying acoustic intensity
+        self.I_avg = False  #: time-averaged acoustic intensity
 
         self.cuboid_corners_list = None
 
         self.x1_inside, self.x2_inside = None, None
         self.y1_inside, self.y2_inside = None, None
         self.z1_inside, self.z2_inside = None, None
 
@@ -45,24 +44,24 @@
 
         Returns:
             None
         """
         # check the contents of the cell array are valid inputs
         allowed_flags = self.get_allowed_flags(is_elastic_code)
         for record_element in flags_list:
-            assert record_element in allowed_flags, f'{record_element} is not a valid input for sensor.record'
+            assert record_element in allowed_flags, f"{record_element} is not a valid input for sensor.record"
 
-            if record_element == 'p':  # custom logic for 'p'
+            if record_element == "p":  # custom logic for 'p'
                 continue
             else:
                 setattr(self, record_element, True)
 
         # set self.record_p to false if a user input for sensor.record
         # is given and 'p' is not set (default is true)
-        self.p = ('p' in flags_list)
+        self.p = "p" in flags_list
 
     def set_index_variables(self, kgrid: kWaveGrid, pml_size: Vector, is_pml_inside: bool, is_axisymmetric: bool) -> None:
         """
         Assign the index variables
 
         Args:
             kgrid: kWaveGrid instance
@@ -104,19 +103,35 @@
 
         Args:
             is_elastic_code: Whether the simulation is axisymmetric
 
         Returns:
             List of allowed flags for a given simulation type
         """
-        allowed_flags = ['p', 'p_max', 'p_min', 'p_rms', 'p_max_all', 'p_min_all', 'p_final',
-                         'u', 'u_max', 'u_min', 'u_rms', 'u_max_all', 'u_min_all', 'u_final',
-                         'u_non_staggered', 'I', 'I_avg']
+        allowed_flags = [
+            "p",
+            "p_max",
+            "p_min",
+            "p_rms",
+            "p_max_all",
+            "p_min_all",
+            "p_final",
+            "u",
+            "u_max",
+            "u_min",
+            "u_rms",
+            "u_max_all",
+            "u_min_all",
+            "u_final",
+            "u_non_staggered",
+            "I",
+            "I_avg",
+        ]
         if is_elastic_code:  # pragma: no cover
-            allowed_flags += ['u_split_field']
+            allowed_flags += ["u_split_field"]
         return allowed_flags
 
     def is_set(self, attrs: List[str]) -> List[bool]:
         """
         Check if the attributes are set
 
         Args:
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/__init__.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/create_absorption_variables.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/create_absorption_variables.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from kwave.kgrid import kWaveGrid
 from kwave.kmedium import kWaveMedium
 from kwave.utils.conversion import db2neper
 
 
 def create_absorption_variables(kgrid: kWaveGrid, medium: kWaveMedium, equation_of_state):
     # define the lossy derivative operators and proportionality coefficients
-    if equation_of_state == 'absorbing':
+    if equation_of_state == "absorbing":
         return create_absorbing_medium_variables(kgrid.k, medium)
-    elif equation_of_state == 'stokes':
+    elif equation_of_state == "stokes":
         return create_stokes_medium_variables(medium)
     else:
         raise NotImplementedError
 
 
 def create_absorbing_medium_variables(kgrid_k, medium: kWaveMedium):
     # convert the absorption coefficient to nepers.(rad/s)^-y.m^-1
@@ -37,27 +37,27 @@
     # compute the absorbing coefficient
     absorb_tau = compute_absorbing_coeff(medium)
     return None, None, absorb_tau, None
 
 
 def get_absorbtion(kgrid_k, medium):
     # compute the absorbing fractional Laplacian operator and coefficient
-    if medium.alpha_mode == 'no_absorption':
+    if medium.alpha_mode == "no_absorption":
         return 0, 0
 
-    nabla1 = kgrid_k**(medium.alpha_power - 2)
+    nabla1 = kgrid_k ** (medium.alpha_power - 2)
     nabla1[np.isinf(nabla1)] = 0
     nabla1 = np.fft.ifftshift(nabla1)
     tau = compute_absorbing_coeff(medium)
     return nabla1, tau
 
 
 def get_dispersion(kgrid_k, medium):
     # compute the dispersive fractional Laplacian operator and coefficient
-    if medium.alpha_mode == 'no_dispersion':
+    if medium.alpha_mode == "no_dispersion":
         return 0, 0
     nabla2 = kgrid_k ** (medium.alpha_power - 1)
     nabla2[np.isinf(nabla2)] = 0
     nabla2 = np.fft.ifftshift(nabla2)
     eta = compute_dispersive_coeff(medium)
     return nabla2, eta
 
@@ -70,15 +70,15 @@
     # with absorption compensation)
     if medium.alpha_sign is not None:
         tau = np.sign(medium.alpha_sign[0]) * tau
     return tau
 
 
 def compute_dispersive_coeff(medium):
-    eta = 2 * medium.alpha_coeff * medium.sound_speed**(medium.alpha_power) * math.tan(math.pi * medium.alpha_power / 2)
+    eta = 2 * medium.alpha_coeff * medium.sound_speed ** (medium.alpha_power) * math.tan(math.pi * medium.alpha_power / 2)
 
     # modify the sign of the absorption operator if alpha_sign is defined
     # (this is used for time-reversal photoacoustic image reconstruction
     # with absorption compensation)
     if medium.alpha_sign is not None:
         eta = np.sign(medium.alpha_sign[1]) * eta
     return eta
@@ -88,15 +88,15 @@
     # pre-filter the absorption parameters if alpha_filter is defined (this
     # is used for time-reversal photoacoustic image reconstruction
     # with absorption compensation)
     if medium.alpha_filter is None:
         return nabla1, nabla2
 
     # update command line status
-    logging.log(logging.INFO, '  filtering absorption variables...')
+    logging.log(logging.INFO, "  filtering absorption variables...")
 
     # frequency shift the absorption parameters
     nabla1 = np.fft.fftshift(nabla1)
     nabla2 = np.fft.fftshift(nabla2)
 
     # apply the filter
     nabla1 = nabla1 * medium.alpha_filter
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/create_storage_variables.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/create_storage_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,74 +7,78 @@
 from kwave.options.simulation_options import SimulationOptions
 from kwave.utils.dotdictionary import dotdict
 
 
 # Note from Farid: This function/file is very suspicious. I'm pretty sure that the implementation is not correct.
 # Full test-coverage is required for bug-fixes!
 
-def create_storage_variables(
-        kgrid: kWaveGrid, sensor, opt: SimulationOptions,
-        values: dotdict, flags: dotdict
-):
+
+def create_storage_variables(kgrid: kWaveGrid, sensor, opt: SimulationOptions, values: dotdict, flags: dotdict):
     # =========================================================================
     # PREPARE DATA MASKS AND STORAGE VARIABLES
     # =========================================================================
 
     record = None  # self.record  # ???
 
     set_flags(flags, values.sensor_x, sensor.mask, opt.cartesian_interp)
 
     # preallocate output variables
     if flags.time_rev:
         return flags
 
-    num_sensor_points = get_num_of_sensor_points(flags.blank_sensor, flags.binary_sensor_mask, kgrid.k,
-                                                 values.sensor_mask_index, values.sensor_x)
-
-    num_recorded_time_points, stream_data_index = \
-        get_num_recorded_time_points(kgrid.dim, kgrid.Nt, opt.stream_to_disk, sensor.record_start_index)
+    num_sensor_points = get_num_of_sensor_points(
+        flags.blank_sensor, flags.binary_sensor_mask, kgrid.k, values.sensor_mask_index, values.sensor_x
+    )
+
+    num_recorded_time_points, stream_data_index = get_num_recorded_time_points(
+        kgrid.dim, kgrid.Nt, opt.stream_to_disk, sensor.record_start_index
+    )
 
     create_shift_operators(record, values.record, kgrid, opt.use_sg)
 
     create_normalized_wavenumber_vectors(record, kgrid, flags.record_u_split_field)
 
     pml_size = [opt.pml_x_size, opt.pml_y_size, opt.pml_z_size]
-    pml_size = Vector(pml_size[:kgrid.dim])
+    pml_size = Vector(pml_size[: kgrid.dim])
     all_vars_size = calculate_all_vars_size(kgrid, opt.pml_inside, pml_size)
 
-    sensor_data = create_sensor_variables(values.record, kgrid, num_sensor_points, num_recorded_time_points,
-                                          all_vars_size)
+    sensor_data = create_sensor_variables(values.record, kgrid, num_sensor_points, num_recorded_time_points, all_vars_size)
 
-    create_transducer_buffer(values.transducer_sensor, values.transducer_receive_elevation_focus, sensor,
-                             num_sensor_points, num_recorded_time_points, values.sensor_data_buffer_size,
-                             flags, sensor_data)
+    create_transducer_buffer(
+        values.transducer_sensor,
+        values.transducer_receive_elevation_focus,
+        sensor,
+        num_sensor_points,
+        num_recorded_time_points,
+        values.sensor_data_buffer_size,
+        flags,
+        sensor_data,
+    )
 
     compute_triangulation_points(flags, kgrid, record)
 
     return flags
 
 
 def set_flags(flags, sensor_x, sensor_mask, is_cartesian_interp):
     # check sensor mask based on the Cartesian interpolation setting
-    if not flags.binary_sensor_mask and is_cartesian_interp == 'nearest':
-
+    if not flags.binary_sensor_mask and is_cartesian_interp == "nearest":
         # extract the data using the binary sensor mask created in
         # inputChecking, but switch on Cartesian reorder flag so that the
         # final data is returned in the correct order (not in time
         # reversal mode).
         flags.binary_sensor_mask = True
         if not flags.time_rev:
             flags.reorder_data = True
 
         # check if any duplicate points have been discarded in the
         # conversion from a Cartesian to binary mask
         num_discarded_points = len(sensor_x) - sensor_mask.sum()
         if num_discarded_points != 0:
-            logging.log(logging.WARN,  
-                f'  {num_discarded_points} duplicated sensor points discarded (nearest neighbour interpolation)')
+            logging.log(logging.WARN, f"  {num_discarded_points} duplicated sensor points discarded (nearest neighbour interpolation)")
 
 
 def get_num_of_sensor_points(is_blank_sensor, is_binary_sensor_mask, kgrid_k, sensor_mask_index, sensor_x):
     """
     Returns the number of sensor points for a given set of sensor parameters.
 
     Args:
@@ -109,15 +113,14 @@
         stream_to_disk:
         record_start_index:
 
     Returns:
 
     """
     if kgrid_dim == 3 and stream_to_disk:
-
         # set the number of points
         num_recorded_time_points = stream_to_disk
 
         # initialise the file index variable
         stream_data_index = 1
 
     else:
@@ -127,15 +130,15 @@
     return num_recorded_time_points, stream_data_index
 
 
 def create_shift_operators(record: dotdict, record_old: dotdict, kgrid: kWaveGrid, is_use_sg):
     # create shift operators used for calculating the components of the
     # particle velocity field on the non-staggered grids (these are used
     # for both binary and cartesian sensor masks)
-    if (record_old.u_non_staggered or record_old.u_split_field or record_old.I or record_old.I_avg):
+    if record_old.u_non_staggered or record_old.u_split_field or record_old.I or record_old.I_avg:
         if is_use_sg:
             if kgrid.dim == 1:
                 record.x_shift_neg = ifftshift(np.exp(-1j * kgrid.k_vec.x * kgrid.dx / 2))
             elif kgrid.dim == 2:
                 record.x_shift_neg = ifftshift(np.exp(-1j * kgrid.k_vec.x * kgrid.dx / 2))
                 record.y_shift_neg = ifftshift(np.exp(-1j * kgrid.k_vec.y * kgrid.dy / 2)).T
             elif kgrid.dim == 3:
@@ -223,15 +226,14 @@
         elif kgrid.dim == 3:
             sensor_data.ux = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uy = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uz = np.zeros([num_sensor_points, num_recorded_time_points])
 
     # maximum particle velocity
     if record_old.u_max:
-
         # pre-allocate the velocity fields based on the number of
         # dimensions in the simulation
         if kgrid.dim == 1:
             sensor_data.ux_max = np.zeros([num_sensor_points, 1])
         if kgrid.dim == 2:
             sensor_data.ux_max = np.zeros([num_sensor_points, 1])
             sensor_data.uy_max = np.zeros([num_sensor_points, 1])
@@ -267,59 +269,55 @@
         if kgrid.dim == 3:
             sensor_data.ux_rms = np.zeros([num_sensor_points, 1])
             sensor_data.uy_rms = np.zeros([num_sensor_points, 1])
             sensor_data.uz_rms = np.zeros([num_sensor_points, 1])
 
     # maximum particle velocity over all grid points
     if record_old.u_max_all:
-
         # pre-allocate the velocity fields based on the number of dimensions in the simulation
         if kgrid.dim == 1:
             sensor_data.ux_max_all = np.zeros(all_vars_size)
         if kgrid.dim == 2:
             sensor_data.ux_max_all = np.zeros(all_vars_size)
             sensor_data.uy_max_all = np.zeros(all_vars_size)
         if kgrid.dim == 3:
             sensor_data.ux_max_all = np.zeros(all_vars_size)
             sensor_data.uy_max_all = np.zeros(all_vars_size)
             sensor_data.uz_max_all = np.zeros(all_vars_size)
 
     # minimum particle velocity over all grid points
     if record_old.u_min_all:
-
         # pre-allocate the velocity fields based on the number of dimensions in the simulation
         if kgrid.dim == 1:
             sensor_data.ux_min_all = np.zeros(all_vars_size)
         if kgrid.dim == 2:
             sensor_data.ux_min_all = np.zeros(all_vars_size)
             sensor_data.uy_min_all = np.zeros(all_vars_size)
         if kgrid.dim == 3:
             sensor_data.ux_min_all = np.zeros(all_vars_size)
             sensor_data.uy_min_all = np.zeros(all_vars_size)
             sensor_data.uz_min_all = np.zeros(all_vars_size)
 
     # time history of the acoustic particle velocity on the
     # non-staggered grid points
     if record_old.u_non_staggered or record_old.I or record_old.I_avg:
-
         # pre-allocate the velocity fields based on the number of dimensions in the simulation
         if kgrid.dim == 1:
             sensor_data.ux_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
         if kgrid.dim == 2:
             sensor_data.ux_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uy_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
         if kgrid.dim == 3:
             sensor_data.ux_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uy_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uz_non_staggered = np.zeros([num_sensor_points, num_recorded_time_points])
 
     # time history of the acoustic particle velocity split into
     # compressional and shear components
     if record_old.u_split_field:
-
         # pre-allocate the velocity fields based on the number of dimensions in the simulation
         if kgrid.dim == 2:
             sensor_data.ux_split_p = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.ux_split_s = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uy_split_p = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uy_split_s = np.zeros([num_sensor_points, num_recorded_time_points])
         if kgrid.dim == 3:
@@ -329,20 +327,27 @@
             sensor_data.uy_split_s = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uz_split_p = np.zeros([num_sensor_points, num_recorded_time_points])
             sensor_data.uz_split_s = np.zeros([num_sensor_points, num_recorded_time_points])
 
     return sensor_data
 
 
-def create_transducer_buffer(is_transducer_sensor, is_transducer_receive_elevation_focus, sensor,
-                             num_sensor_points, num_recorded_time_points, sensor_data_buffer_size, flags, sensor_data):
+def create_transducer_buffer(
+    is_transducer_sensor,
+    is_transducer_receive_elevation_focus,
+    sensor,
+    num_sensor_points,
+    num_recorded_time_points,
+    sensor_data_buffer_size,
+    flags,
+    sensor_data,
+):
     # object of the kWaveTransducer class is being used as a sensor
     if is_transducer_sensor:
         if is_transducer_receive_elevation_focus:
-
             # if there is elevation focusing, a buffer is
             # needed to store a short time history at each
             # sensor point before averaging
             # ???
             sensor_data_buffer_size = sensor.elevation_beamforming_delays.max() + 1
             if sensor_data_buffer_size > 1:
                 sensor_data_buffer = np.zeros([num_sensor_points, sensor_data_buffer_size])  # noqa: F841
@@ -357,23 +362,21 @@
 
 def compute_triangulation_points(flags, kgrid, record):
     # precomputate the triangulation points if a Cartesian sensor mask
     # is used with linear interpolation (tri and bc are the Delaunay
     # triangulation and Barycentric coordinates)
     if not flags.binary_sensor_mask:
         if kgrid.dim == 1:
-
             # assign pseudonym for Cartesain grid points in 1D (this
             # is later used for data casting)
             record.grid_x = kgrid.x_vec
 
         else:
-
             # update command line status
-            logging.log(logging.INFO, '  calculating Delaunay triangulation...')
+            logging.log(logging.INFO, "  calculating Delaunay triangulation...")
 
             # compute triangulation
             if kgrid.dim == 2:
                 if flags.axisymmetric:
                     record.tri, record.bc = gridDataFast2D(kgrid.x, kgrid.y - kgrid.y_vec.min(), sensor_x, sensor_y)
                 else:
                     record.tri, record.bc = gridDataFast2D(kgrid.x, kgrid.y, sensor_x, sensor_y)
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/data_cast.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/data_cast.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,180 +9,206 @@
 
 def dataCast(data_cast, medium: kWaveMedium, kgrid: kWaveGrid, opt: SimulationOptions, values: dotdict, flags: dotdict):
     # NOTE from Farid: this method is not used now.
     # Therefore, there still exists 'self' calls at the end.
     # Originally, self was referring to the kWaveSimulation class
 
     # update command line status
-    logging.log(logging.INFO, f'  casting variables to {data_cast} type...')
+    logging.log(logging.INFO, f"  casting variables to {data_cast} type...")
 
     # create list of variable names used in all dimensions
     if flags.elastic_code:  # pragma: no cover
-        cast_variables = ['dt', 'mu', 'lambda']
+        cast_variables = ["dt", "mu", "lambda"]
     else:
-        cast_variables = ['dt', 'kappa', 'c0', 'rho0']
+        cast_variables = ["dt", "kappa", "c0", "rho0"]
 
     # create a separate list for indexing variables
     cast_index_variables = []
 
     # add variables specific to simulations in certain dimensions
     if kgrid.dim == 1:
         # variables used in the fluid code
-        cast_variables = cast_variables + ['ddx_k', 'shift_pos', 'shift_neg','pml_x', 'pml_x_sgx', 'rho0_sgx_inv']
+        cast_variables = cast_variables + ["ddx_k", "shift_pos", "shift_neg", "pml_x", "pml_x_sgx", "rho0_sgx_inv"]
 
     elif kgrid.dim == 2:
         # variables used in both fluid and elastic codes
-        cast_variables = cast_variables + ['ddx_k_shift_pos', 'ddx_k_shift_neg', 'pml_x', 'pml_y',
-                                           'pml_x_sgx', 'pml_y_sgy', 'rho0_sgx_inv', 'rho0_sgy_inv']
+        cast_variables = cast_variables + [
+            "ddx_k_shift_pos",
+            "ddx_k_shift_neg",
+            "pml_x",
+            "pml_y",
+            "pml_x_sgx",
+            "pml_y_sgy",
+            "rho0_sgx_inv",
+            "rho0_sgy_inv",
+        ]
 
         # y-dimension shift and derivative variables (these differ between the fluid/elastic code and the axisymmetric code)
         if flags.axisymmetric:
-
             # y-axis variables
-            cast_variables = cast_variables + ['y_vec', 'y_vec_sg']
+            cast_variables = cast_variables + ["y_vec", "y_vec_sg"]
 
             # derivative and shift variables
-            if opt.radial_symmetry in ['WSWA-FFT','WSWS-FFT','WS-FFT']:
-                cast_variables = cast_variables + ['ddy_k', 'y_shift_pos', 'y_shift_neg']
+            if opt.radial_symmetry in ["WSWA-FFT", "WSWS-FFT", "WS-FFT"]:
+                cast_variables = cast_variables + ["ddy_k", "y_shift_pos", "y_shift_neg"]
 
-            elif opt.radial_symmetry == 'WSWA':
-                cast_variables = cast_variables + ['ddy_k_wswa', 'ddy_k_hahs']
+            elif opt.radial_symmetry == "WSWA":
+                cast_variables = cast_variables + ["ddy_k_wswa", "ddy_k_hahs"]
 
-            elif opt.radial_symmetry == 'WSWS':
-                cast_variables = cast_variables + ['ddy_k_wsws', 'ddy_k_haha']
+            elif opt.radial_symmetry == "WSWS":
+                cast_variables = cast_variables + ["ddy_k_wsws", "ddy_k_haha"]
 
         else:
             # derivative and shift variables in the regular code
-            cast_variables = cast_variables + ['ddy_k_shift_pos', 'ddy_k_shift_neg']
+            cast_variables = cast_variables + ["ddy_k_shift_pos", "ddy_k_shift_neg"]
 
         # extra variables only used in elastic code
         if flags.elastic_code:  # pragma: no cover
-
             # variables used in both lossless and lossy case
-            cast_variables = cast_variables +  ['mu_sgxy', 'mpml_x', 'mpml_y', 'mpml_x_sgx', 'mpml_y_sgy']
+            cast_variables = cast_variables + ["mu_sgxy", "mpml_x", "mpml_y", "mpml_x_sgx", "mpml_y_sgy"]
 
             # extra variables only used in the lossy case
             if flags.kelvin_voigt_model:
-                cast_variables = cast_variables + ['chi', 'eta', 'eta_sgxy']
+                cast_variables = cast_variables + ["chi", "eta", "eta_sgxy"]
 
     elif kgrid.dim == 3:
         # variables used in both fluid and elastic codes
-        cast_variables = cast_variables + ['ddx_k_shift_pos', 'ddy_k_shift_pos', 'ddz_k_shift_pos',
-                                           'ddx_k_shift_neg', 'ddy_k_shift_neg', 'ddz_k_shift_neg',
-                                           'pml_x', 'pml_y', 'pml_z',
-                                           'pml_x_sgx', 'pml_y_sgy', 'pml_z_sgz',
-                                           'rho0_sgx_inv', 'rho0_sgy_inv', 'rho0_sgz_inv']
+        cast_variables = cast_variables + [
+            "ddx_k_shift_pos",
+            "ddy_k_shift_pos",
+            "ddz_k_shift_pos",
+            "ddx_k_shift_neg",
+            "ddy_k_shift_neg",
+            "ddz_k_shift_neg",
+            "pml_x",
+            "pml_y",
+            "pml_z",
+            "pml_x_sgx",
+            "pml_y_sgy",
+            "pml_z_sgz",
+            "rho0_sgx_inv",
+            "rho0_sgy_inv",
+            "rho0_sgz_inv",
+        ]
 
         # extra variables only used in elastic code
         if flags.elastic_code:  # pragma: no cover
             # variables used in both lossless and lossy case
-            cast_variables = cast_variables + ['mu_sgxy', 'mu_sgxz', 'mu_sgyz',
-                                               'mpml_x', 'mpml_y', 'mpml_z',
-                                               'mpml_x_sgx', 'mpml_y_sgy', 'mpml_z_sgz']
+            cast_variables = cast_variables + [
+                "mu_sgxy",
+                "mu_sgxz",
+                "mu_sgyz",
+                "mpml_x",
+                "mpml_y",
+                "mpml_z",
+                "mpml_x_sgx",
+                "mpml_y_sgy",
+                "mpml_z_sgz",
+            ]
 
             # extra variables only used in the lossy case
             if flags.kelvin_voigt_model:
-                cast_variables = cast_variables + ['chi', 'eta', 'eta_sgxy', 'eta_sgxz', 'eta_sgyz']
+                cast_variables = cast_variables + ["chi", "eta", "eta_sgxy", "eta_sgxz", "eta_sgyz"]
 
     # add sensor mask variables
     if flags.use_sensor:
-        cast_index_variables += ['sensor_mask_index']
+        cast_index_variables += ["sensor_mask_index"]
         if flags.binary_sensor_mask and (values.record.u_non_staggered or values.record.I or values.record.I_avg):
             if kgrid.dim == 1:
-                cast_index_variables += ['record.x_shift_neg']
+                cast_index_variables += ["record.x_shift_neg"]
             elif kgrid.dim == 2:
-                cast_index_variables += ['record.x_shift_neg', 'record.y_shift_neg']
+                cast_index_variables += ["record.x_shift_neg", "record.y_shift_neg"]
             elif kgrid.dim == 3:
-                cast_index_variables += ['record.x_shift_neg', 'record.y_shift_neg', 'record.z_shift_neg']
+                cast_index_variables += ["record.x_shift_neg", "record.y_shift_neg", "record.z_shift_neg"]
 
     # additional variables only used if the medium is absorbing
-    if values.equation_of_state == 'absorbing':
-        cast_variables += ['absorb_nabla1', 'absorb_nabla2', 'absorb_eta', 'absorb_tau']
+    if values.equation_of_state == "absorbing":
+        cast_variables += ["absorb_nabla1", "absorb_nabla2", "absorb_eta", "absorb_tau"]
 
     # additional variables only used if the propagation is nonlinear
     if medium.is_nonlinear():
-        cast_variables += ['medium.BonA']
+        cast_variables += ["medium.BonA"]
 
     # additional variables only used if there is an initial pressure source
     if flags.source_p0:
-        cast_variables += ['source.p0']
+        cast_variables += ["source.p0"]
 
     # additional variables only used if there is a time varying pressure source term
     if flags.source_p:
-        cast_variables += ['source.p']
-        cast_index_variables += ['p_source_pos_index']
+        cast_variables += ["source.p"]
+        cast_index_variables += ["p_source_pos_index"]
         if flags.source_p_labelled:
-            cast_index_variables += ['p_source_sig_index']
+            cast_index_variables += ["p_source_sig_index"]
 
     # additional variables only used if there is a time varying velocity source term
     if flags.source_ux or flags.source_uy or flags.source_uz:
-        cast_index_variables += ['u_source_pos_index']
+        cast_index_variables += ["u_source_pos_index"]
         if self.source_u_labelled:  # noqa: F821
-            cast_index_variables += ['u_source_sig_index']
+            cast_index_variables += ["u_source_sig_index"]
 
     if flags.source_ux:
-        cast_variables += ['source.ux']
+        cast_variables += ["source.ux"]
     if flags.source_uy:
-        cast_variables += ['source.uy']
+        cast_variables += ["source.uy"]
     if flags.source_uz:
-        cast_variables += ['source.uz']
+        cast_variables += ["source.uz"]
 
     # additional variables only used if there is a time varying stress source term
     if flags.source_sxx or flags.source_syy or flags.source_szz or flags.source_sxy or flags.source_sxz or flags.source_syz:
-        cast_index_variables += ['s_source_pos_index']
+        cast_index_variables += ["s_source_pos_index"]
         if flags.source_s_labelled:
-            cast_index_variables += ['s_source_sig_index']
+            cast_index_variables += ["s_source_sig_index"]
 
     if flags.source_sxx:
-        cast_variables += ['source.sxx']
+        cast_variables += ["source.sxx"]
     if flags.source_syy:
-        cast_variables += ['source.syy']
+        cast_variables += ["source.syy"]
     if flags.source_szz:
-        cast_variables += ['source.szz']
+        cast_variables += ["source.szz"]
     if flags.source_sxy:
-        cast_variables += ['source.sxy']
+        cast_variables += ["source.sxy"]
     if flags.source_sxz:
-        cast_variables += ['source.sxz']
+        cast_variables += ["source.sxz"]
     if flags.source_syz:
-        cast_variables += ['source.syz']
+        cast_variables += ["source.syz"]
 
     # addition variables only used if there is a transducer source
     if flags.transducer_source:
-        cast_variables += ['transducer_input_signal']
-        cast_index_variables += ['u_source_pos_index', 'delay_mask', 'self.transducer_source', 'transducer_transmit_apodization']
+        cast_variables += ["transducer_input_signal"]
+        cast_index_variables += ["u_source_pos_index", "delay_mask", "self.transducer_source", "transducer_transmit_apodization"]
 
     # addition variables only used if there is a transducer sensor with an elevation focus
     if flags.transducer_sensor and flags.transducer_receive_elevation_focus:
-        cast_index_variables += ['sensor_data_buffer', 'transducer_receive_mask']
+        cast_index_variables += ["sensor_data_buffer", "transducer_receive_mask"]
 
     # additional variables only used with nonuniform grids
     if flags.nonuniform_grid:
         if kgrid.dim == 1:
-            cast_index_variables += ['kgrid.dxudxn']
+            cast_index_variables += ["kgrid.dxudxn"]
         elif kgrid.dim == 2:
-            cast_index_variables += ['kgrid.dxudxn', 'kgrid.dyudyn']
+            cast_index_variables += ["kgrid.dxudxn", "kgrid.dyudyn"]
         elif kgrid.dim == 3:
-            cast_index_variables += ['kgrid.dxudxn', 'kgrid.dyudyn', 'kgrid.dzudzn']
+            cast_index_variables += ["kgrid.dxudxn", "kgrid.dyudyn", "kgrid.dzudzn"]
 
     # additional variables only used for Cartesian sensor masks with linear interpolation
     if flags.use_sensor and not flags.binary_sensor_mask and not flags.time_rev:
         if kgrid.dim == 1:
-            cast_variables += ['record.grid_x', 'record.sensor_x']
+            cast_variables += ["record.grid_x", "record.sensor_x"]
         else:
-            cast_variables += ['record.tri', 'record.bc']
+            cast_variables += ["record.tri", "record.bc"]
 
     # additional variables only used in 2D if sensor directivity is defined
     if flags.compute_directivity:
-        cast_variables += ['sensor.directivity_angle', 'sensor.directivity_unique_angles', 'sensor.directivity_wavenumbers']
+        cast_variables += ["sensor.directivity_angle", "sensor.directivity_unique_angles", "sensor.directivity_wavenumbers"]
 
     # cast variables
     for cast_var in cast_variables:
-        if '.' in cast_var:
-            part1, part2 = cast_var.split('.')
+        if "." in cast_var:
+            part1, part2 = cast_var.split(".")
             subdict = getattr(self, part1)  # noqa: F821
             subdict[part2] = cast_to_type(subdict[part2], data_cast)
         else:
             setattr(self, cast_var, cast_to_type(getattr(self, cast_var), data_cast))  # noqa: F821
 
     # cast index variables only if casting to the GPU
-    if data_cast.startswith('kWaveGPU'):
+    if data_cast.startswith("kWaveGPU"):
         raise NotImplementedError
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/display_simulation_params.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/display_simulation_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def display_simulation_params(kgrid: kWaveGrid, medium: kWaveMedium, elastic_code: bool):
     dt = kgrid.dt
     t_array_end = kgrid.t_array[0][-1]
     Nt = int(kgrid.Nt)
     k_size = kgrid.size
 
     # display time step information
-    logging.log(logging.INFO, '  dt: ', f'{scale_SI(dt)[0]}s, t_end: {scale_SI(t_array_end)[0]}s, time steps:', Nt)
+    logging.log(logging.INFO, "  dt: ", f"{scale_SI(dt)[0]}s, t_end: {scale_SI(t_array_end)[0]}s, time steps:", Nt)
 
     c_min, c_min_comp, c_min_shear = get_min_sound_speed(medium, elastic_code)
 
     # get suitable scaling factor
     _, scale, _, _ = scale_SI(np.min(k_size[k_size != 0]))
 
     print_grid_size(kgrid, scale)
@@ -35,54 +35,63 @@
         c_min_shear = np.min(medium.sound_speed_shear[medium.sound_speed_shear != 0])
         return None, c_min_comp, c_min_shear
 
 
 def print_grid_size(kgrid, scale):
     k_size = kgrid.size
 
-    grid_size_pts       = [int(kgrid.Nx)]
+    grid_size_pts = [int(kgrid.Nx)]
     if kgrid.dim >= 2:
         grid_size_pts.append(int(kgrid.Ny))
     if kgrid.dim == 3:
         grid_size_pts.append(int(kgrid.Nz))
 
     if kgrid.dim == 1:
-        grid_size_scale     = [scale_SI(k_size[0])[0]]
+        grid_size_scale = [scale_SI(k_size[0])[0]]
     elif kgrid.dim == 2:
-        grid_size_scale     = [k_size[0] * scale, k_size[1] * scale]
+        grid_size_scale = [k_size[0] * scale, k_size[1] * scale]
     elif kgrid.dim == 3:
-        grid_size_scale     = [round(k_size[0]*scale, 4), round(k_size[1]*scale, 4), round(k_size[2]*scale, 4)]
+        grid_size_scale = [round(k_size[0] * scale, 4), round(k_size[1] * scale, 4), round(k_size[2] * scale, 4)]
     else:
         raise NotImplementedError
 
-    grid_size_str   = ' by '.join(map(str, grid_size_pts))
-    grid_scale_str  = ' by '.join(map(str, grid_size_scale))
+    grid_size_str = " by ".join(map(str, grid_size_pts))
+    grid_scale_str = " by ".join(map(str, grid_size_scale))
 
     # display grid size
-    logging.log(logging.INFO, f'  input grid size: {grid_size_str} grid points ({grid_scale_str} m)')
+    logging.log(logging.INFO, f"  input grid size: {grid_size_str} grid points ({grid_scale_str} m)")
 
 
 def print_max_supported_freq(kgrid, c_min):
     # display the grid size and maximum supported frequency
     k_max, k_max_all = kgrid.k_max, kgrid.k_max_all
 
     if kgrid.dim == 1:
         # display maximum supported frequency
-        logging.log(logging.INFO, '  maximum supported frequency: ', scale_SI(k_max_all * c_min / (2*np.pi))[0], 'Hz')
+        logging.log(logging.INFO, "  maximum supported frequency: ", scale_SI(k_max_all * c_min / (2 * np.pi))[0], "Hz")
 
     elif kgrid.dim == 2:
         # display maximum supported frequency
         if k_max.x == k_max.y:
-            logging.log(logging.INFO, '  maximum supported frequency: ', scale_SI(k_max_all * c_min / (2*np.pi))[0], 'Hz')
+            logging.log(logging.INFO, "  maximum supported frequency: ", scale_SI(k_max_all * c_min / (2 * np.pi))[0], "Hz")
         else:
-            logging.log(logging.INFO, '  maximum supported frequency: ', scale_SI(k_max.x * c_min / (2*np.pi))[0],
-                  'Hz by ', scale_SI(k_max.y * c_min / (2*np.pi))[0], 'Hz')
+            logging.log(
+                logging.INFO,
+                "  maximum supported frequency: ",
+                scale_SI(k_max.x * c_min / (2 * np.pi))[0],
+                "Hz by ",
+                scale_SI(k_max.y * c_min / (2 * np.pi))[0],
+                "Hz",
+            )
 
     elif kgrid.dim == 3:
         # display maximum supported frequency
         if k_max.x == k_max.z and k_max.x == k_max.y:
-            logging.log(logging.INFO, '  maximum supported frequency: ', f'{scale_SI(k_max_all * c_min / (2*np.pi))[0]}Hz')
+            logging.log(logging.INFO, "  maximum supported frequency: ", f"{scale_SI(k_max_all * c_min / (2*np.pi))[0]}Hz")
         else:
-            logging.log(logging.INFO, '  maximum supported frequency: ',
-                  f'{scale_SI(k_max.x * c_min / (2*np.pi))[0]}Hz by '
-                  f'{scale_SI(k_max.y * c_min / (2*np.pi))[0]}Hz by '
-                  f'{scale_SI(k_max.z * c_min / (2*np.pi))[0]}Hz')
+            logging.log(
+                logging.INFO,
+                "  maximum supported frequency: ",
+                f"{scale_SI(k_max.x * c_min / (2*np.pi))[0]}Hz by "
+                f"{scale_SI(k_max.y * c_min / (2*np.pi))[0]}Hz by "
+                f"{scale_SI(k_max.z * c_min / (2*np.pi))[0]}Hz",
+            )
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/expand_grid_matrices.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/expand_grid_matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,57 +8,54 @@
 from kwave.data import Vector
 from kwave.utils.data import get_smallest_possible_type
 from kwave.utils.dotdictionary import dotdict
 from kwave.utils.matlab import matlab_find
 from kwave.utils.matrix import expand_matrix
 
 
-def expand_grid_matrices(
-        kgrid: kWaveGrid, medium: kWaveMedium, source, sensor, opt: SimulationOptions,
-        values: dotdict, flags: dotdict):
+def expand_grid_matrices(kgrid: kWaveGrid, medium: kWaveMedium, source, sensor, opt: SimulationOptions, values: dotdict, flags: dotdict):
     # update command line status
-    logging.log(logging.INFO, '  expanding computational grid...')
+    logging.log(logging.INFO, "  expanding computational grid...")
 
     #####################
     # Grab values
     #####################
 
     # retaining the values for kgrid time array
     pml_size = [opt.pml_x_size, opt.pml_y_size, opt.pml_z_size]
-    pml_size = Vector(pml_size[:kgrid.dim])
+    pml_size = Vector(pml_size[: kgrid.dim])
 
     p_source_pos_index = values.p_source_pos_index
     u_source_pos_index = values.u_source_pos_index
     s_source_pos_index = values.s_source_pos_index
 
-    is_source_sensor_same = (isinstance(sensor, NotATransducer) and sensor == source)
+    is_source_sensor_same = isinstance(sensor, NotATransducer) and sensor == source
 
     #####################
     # Expand Structures
     #####################
 
     # expand the computational grid, replacing the original grid
     kgrid = expand_kgrid(kgrid, flags.axisymmetric, pml_size)
 
     expand_size = calculate_expand_size(kgrid, flags.axisymmetric, pml_size)
 
     # update the data type in case adding the PML requires additional index precision
     total_grid_points = kgrid.total_grid_points
-    index_data_type = get_smallest_possible_type(total_grid_points, 'uint', default='double')
+    index_data_type = get_smallest_possible_type(total_grid_points, "uint", default="double")
 
     expand_sensor(sensor, expand_size, flags.use_sensor, flags.blank_sensor)
 
     # TODO why it is not self.record ? "self"
     record = expand_cuboid_corner_list(flags.cuboid_corners, kgrid, pml_size)  # noqa: F841
 
     expand_medium(medium, expand_size)
 
     p_source_pos_index, u_source_pos_index, s_source_pos_index = expand_source(
-        source, is_source_sensor_same, flags, expand_size, index_data_type,
-        p_source_pos_index, u_source_pos_index, s_source_pos_index
+        source, is_source_sensor_same, flags, expand_size, index_data_type, p_source_pos_index, u_source_pos_index, s_source_pos_index
     )
 
     expand_directivity_angle(kgrid, sensor, expand_size, flags.use_sensor, flags.compute_directivity)
 
     print_grid_size(kgrid)
 
     return kgrid, index_data_type, p_source_pos_index, u_source_pos_index, s_source_pos_index
@@ -66,22 +63,22 @@
 
 def expand_kgrid(kgrid, is_axisymmetric, pml_size):
     Nt_temp, dt_temp = kgrid.Nt, kgrid.dt
 
     pml_size = pml_size.squeeze()
 
     if kgrid.dim == 1:
-        new_size            = kgrid.N + 2 * pml_size
+        new_size = kgrid.N + 2 * pml_size
     elif kgrid.dim == 2:
         if is_axisymmetric:
-            new_size        = [kgrid.Nx + 2 * pml_size[0], kgrid.Ny + pml_size[1]]
+            new_size = [kgrid.Nx + 2 * pml_size[0], kgrid.Ny + pml_size[1]]
         else:
-            new_size        = kgrid.N + 2 * pml_size
+            new_size = kgrid.N + 2 * pml_size
     elif kgrid.dim == 3:
-        new_size            = kgrid.N + 2 * pml_size
+        new_size = kgrid.N + 2 * pml_size
     else:
         raise NotImplementedError
 
     kgrid = kWaveGrid(new_size, kgrid.spacing)
     # re-assign original time array
     kgrid.setTime(Nt_temp, dt_temp)
 
@@ -113,63 +110,74 @@
 
     # enlarge the grid of density by exting the edge values into the expanded grid
     medium.density = np.atleast_1d(medium.density)
     if medium.density.size > 1:
         medium.density = expand_matrix(medium.density, expand_size)
 
     # for key in ['alpha_coeff', 'alpha_coeff_compression', 'alpha_coeff_shear', 'BonA']:
-    for key in ['alpha_coeff', 'BonA']:
+    for key in ["alpha_coeff", "BonA"]:
         # enlarge the grid of medium[key] if given
         attr = getattr(medium, key)
         if attr is not None and np.atleast_1d(attr).size > 1:
             attr = expand_matrix(np.atleast_1d(attr), expand_size)
             setattr(medium, key, attr)
 
     # enlarge the absorption filter mask if given
     if medium.alpha_filter is not None:
         medium.alpha_filter = expand_matrix(medium.alpha_filter, expand_size, 0)
 
 
 def expand_source(
-        source, is_source_sensor_same, flags, expand_size, index_data_type,
-        p_source_pos_index, u_source_pos_index, s_source_pos_index):
-
-    p_source_pos_index = expand_pressure_sources(source, expand_size, flags.source_p0, flags.source_p,
-                                                 index_data_type, p_source_pos_index)
+    source, is_source_sensor_same, flags, expand_size, index_data_type, p_source_pos_index, u_source_pos_index, s_source_pos_index
+):
+    p_source_pos_index = expand_pressure_sources(source, expand_size, flags.source_p0, flags.source_p, index_data_type, p_source_pos_index)
 
     u_source_pos_index = expand_velocity_sources(
-        source, expand_size, is_source_sensor_same, index_data_type, u_source_pos_index,
-        flags.source_ux, flags.source_uy, flags.source_uz, flags.transducer_source
+        source,
+        expand_size,
+        is_source_sensor_same,
+        index_data_type,
+        u_source_pos_index,
+        flags.source_ux,
+        flags.source_uy,
+        flags.source_uz,
+        flags.transducer_source,
     )
 
     s_source_pos_index = expand_stress_sources(source, expand_size, flags, index_data_type, s_source_pos_index)
 
     return p_source_pos_index, u_source_pos_index, s_source_pos_index
 
 
 def expand_pressure_sources(source, expand_size, is_source_p0, is_source_p, index_data_type, p_source_pos_index):
     # enlarge the initial pressure if given
     if is_source_p0:
         source.p0 = expand_matrix(source.p0, expand_size, 0)
 
     # enlarge the pressure source mask if given
     if is_source_p:
-
         # enlarge the pressure source mask
         source.p_mask = expand_matrix(source.p_mask, expand_size, 0)
 
         # create an indexing variable corresponding to the source elements
         # and convert the data type deping on the number of indices
         p_source_pos_index = matlab_find(source.p_mask).astype(index_data_type)
     return p_source_pos_index
 
 
 def expand_velocity_sources(
-        source, expand_size, is_source_sensor_same, index_data_type, u_source_pos_index,
-        is_source_ux, is_source_uy, is_source_uz, is_transducer_source
+    source,
+    expand_size,
+    is_source_sensor_same,
+    index_data_type,
+    u_source_pos_index,
+    is_source_ux,
+    is_source_uy,
+    is_source_uz,
+    is_transducer_source,
 ):
     """
         enlarge the velocity source mask if given
     Args:
         source:
         expand_size:
         is_source_sensor_same:
@@ -180,31 +188,27 @@
         is_source_uz:
         is_transducer_source:
 
     Returns:
 
     """
     if is_source_ux or is_source_uy or is_source_uz or is_transducer_source:
-
         # update the source indexing variable
         if isinstance(source, NotATransducer):
-
             # check if the sensor is also the same transducer, if so, don't expand the grid again
             if not is_source_sensor_same:
-
                 # expand the transducer mask
                 source.expand_grid(expand_size)
 
             # get the new active elements mask
             active_elements_mask = source.active_elements_mask
 
             # update the indexing variable corresponding to the active elements
             u_source_pos_index = matlab_find(active_elements_mask)
         else:
-
             # enlarge the velocity source mask
             source.u_mask = expand_matrix(source.u_mask, expand_size, 0)
 
             # create an indexing variable corresponding to the source elements
             u_source_pos_index = matlab_find(source.u_mask)
 
         # convert the data type deping on the number of indices
@@ -253,19 +257,19 @@
         kgrid:
 
     Returns:
 
     """
     k_Nx, k_Ny, k_Nz = kgrid.Nx, kgrid.Ny, kgrid.Nz
     if kgrid.dim == 1:
-        logging.log(logging.INFO, '  computational grid size:', int(k_Nx), 'grid points')
+        logging.log(logging.INFO, "  computational grid size:", int(k_Nx), "grid points")
     elif kgrid.dim == 2:
-        logging.log(logging.INFO, '  computational grid size:', int(k_Nx), 'by', int(k_Ny), 'grid points')
+        logging.log(logging.INFO, "  computational grid size:", int(k_Nx), "by", int(k_Ny), "grid points")
     elif kgrid.dim == 3:
-        logging.log(logging.INFO, '  computational grid size:', int(k_Nx), 'by', int(k_Ny), 'by', int(k_Nz), 'grid points')
+        logging.log(logging.INFO, "  computational grid size:", int(k_Nx), "by", int(k_Ny), "by", int(k_Nz), "grid points")
 
 
 def expand_cuboid_corner_list(is_cuboid_list, kgrid, pml_size: Vector):
     """
         add the PML size to cuboid corner indices if using a cuboid sensor mask
     Args:
         is_cuboid_list:
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/retract_transducer_grid_size.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/retract_transducer_grid_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 def retract_transducer_grid_size(source, sensor, retract_size, pml_inside: bool):
     # resize the transducer object if the grid has been expanded
     is_source_kwave_transducer = isinstance(source, NotATransducer)
     is_sensor_kwave_transducer = isinstance(sensor, NotATransducer)
     retract_size = np.array(retract_size)
 
     if not pml_inside and (is_source_kwave_transducer or is_sensor_kwave_transducer):
-
         # check if the sensor is a transducer
         if is_sensor_kwave_transducer:
             # retract the transducer mask
             sensor.retract_grid(retract_size)
 
         # check if the source is a transducer, and if so, and different
         # transducer to the sensor
         if is_source_kwave_transducer and not (is_sensor_kwave_transducer and sensor == source):
-
             # retract the transducer mask
             source.retract_grid(retract_size)
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/save_to_disk_func.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/save_to_disk_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 from kwave.utils.dotdictionary import dotdict
 from kwave.utils.io import write_attributes, write_matrix
 from kwave.utils.matrix import num_dim2
 from kwave.utils.tictoc import TicToc
 
 
 def save_to_disk_func(
-        kgrid: kWaveGrid, medium: kWaveMedium, source,
-        opt: SimulationOptions, auto_chunk: bool,
-        values: dotdict, flags: dotdict):
+    kgrid: kWaveGrid, medium: kWaveMedium, source, opt: SimulationOptions, auto_chunk: bool, values: dotdict, flags: dotdict
+):
     # update command line status
-    logging.log(logging.INFO, '  precomputation completed in ', scale_time(TicToc.toc()))
+    logging.log(logging.INFO, "  precomputation completed in ", scale_time(TicToc.toc()))
     TicToc.tic()
-    logging.log(logging.INFO, '  saving input files to disk...')
+    logging.log(logging.INFO, "  saving input files to disk...")
 
     # check for a binary sensor mask or cuboid corners
     # modified by Farid | disabled temporarily!
     # assert self.binary_sensor_mask or self.cuboid_corners, \
     #     "Optional input ''save_to_disk'' only supported for sensor masks defined as a binary matrix
     #           or the opposing corners of a rectangle (2D) or cuboid (3D)."
 
@@ -41,121 +40,125 @@
 
     # overwrite z-values for 2D simulations
     if kgrid.dim == 2:
         integer_variables.Nz = 1
         integer_variables.pml_z_size = 0
 
     grab_medium_props(integer_variables, float_variables, medium, flags.elastic_code)
-    grab_source_props(integer_variables, float_variables, source,
-                      values.u_source_pos_index, values.s_source_pos_index, values.p_source_pos_index,
-                      values.transducer_input_signal, values.delay_mask)
+    grab_source_props(
+        integer_variables,
+        float_variables,
+        source,
+        values.u_source_pos_index,
+        values.s_source_pos_index,
+        values.p_source_pos_index,
+        values.transducer_input_signal,
+        values.delay_mask,
+    )
 
     grab_sensor_props(integer_variables, kgrid.dim, values.sensor_mask_index, values.record.cuboid_corners_list)
     grab_nonuniform_grid_props(float_variables, kgrid, flags.nonuniform_grid)
 
     # =========================================================================
     # DATACAST AND SAVING
     # =========================================================================
 
     remove_z_dimension(float_variables, kgrid.dim)
-    save_file(opt.input_filename, integer_variables, float_variables, opt.hdf_compression_level, 
-              auto_chunk=auto_chunk)
+    save_file(opt.input_filename, integer_variables, float_variables, opt.hdf_compression_level, auto_chunk=auto_chunk)
 
     # update command line status
-    logging.log(logging.INFO, '  completed in ', scale_time(TicToc.toc()))
+    logging.log(logging.INFO, "  completed in ", scale_time(TicToc.toc()))
 
 
 def grab_integer_variables(integer_variables, kgrid, flags, medium):
     # integer variables used within the time loop for all codes
 
-    variables = dotdict({
-        'Nx': kgrid.Nx,
-        'Ny': kgrid.Ny,
-        'Nz': kgrid.Nz,
-        'Nt': kgrid.Nt,
-        'p_source_flag': flags.source_p,
-        'p0_source_flag': flags.source_p0,
-
-        'ux_source_flag': flags.source_ux,
-        'uy_source_flag': flags.source_uy,
-        'uz_source_flag': flags.source_uz,
-
-        'sxx_source_flag': flags.source_sxx,
-        'syy_source_flag': flags.source_syy,
-        'szz_source_flag': flags.source_szz,
-
-        'sxy_source_flag': flags.source_sxy,
-        'sxz_source_flag': flags.source_sxz,
-        'syz_source_flag': flags.source_syz,
-
-        'transducer_source_flag': flags.transducer_source,
-        'nonuniform_grid_flag': flags.nonuniform_grid,
-        'nonlinear_flag': medium.is_nonlinear(),
-        'absorbing_flag': None,
-        'elastic_flag': flags.elastic_code,
-        'axisymmetric_flag': flags.axisymmetric,
-
-        # create pseudonyms for the sensor flgs
-        #   0: binary mask indices
-        #   1: cuboid corners
-        'sensor_mask_type': flags.cuboid_corners
-    })
+    variables = dotdict(
+        {
+            "Nx": kgrid.Nx,
+            "Ny": kgrid.Ny,
+            "Nz": kgrid.Nz,
+            "Nt": kgrid.Nt,
+            "p_source_flag": flags.source_p,
+            "p0_source_flag": flags.source_p0,
+            "ux_source_flag": flags.source_ux,
+            "uy_source_flag": flags.source_uy,
+            "uz_source_flag": flags.source_uz,
+            "sxx_source_flag": flags.source_sxx,
+            "syy_source_flag": flags.source_syy,
+            "szz_source_flag": flags.source_szz,
+            "sxy_source_flag": flags.source_sxy,
+            "sxz_source_flag": flags.source_sxz,
+            "syz_source_flag": flags.source_syz,
+            "transducer_source_flag": flags.transducer_source,
+            "nonuniform_grid_flag": flags.nonuniform_grid,
+            "nonlinear_flag": medium.is_nonlinear(),
+            "absorbing_flag": None,
+            "elastic_flag": flags.elastic_code,
+            "axisymmetric_flag": flags.axisymmetric,
+            # create pseudonyms for the sensor flgs
+            #   0: binary mask indices
+            #   1: cuboid corners
+            "sensor_mask_type": flags.cuboid_corners,
+        }
+    )
     integer_variables.update(variables)
 
 
 def grab_pml_size(integer_variables, opt):
     # additional integer variables not used within time loop but stored directly to output file
-    integer_variables['pml_x_size'] = opt.pml_x_size
-    integer_variables['pml_y_size'] = opt.pml_y_size
-    integer_variables['pml_z_size'] = opt.pml_z_size
+    integer_variables["pml_x_size"] = opt.pml_x_size
+    integer_variables["pml_y_size"] = opt.pml_y_size
+    integer_variables["pml_z_size"] = opt.pml_z_size
 
 
 def grab_float_variables(float_variables: dotdict, kgrid, opt, values, is_elastic_code, is_axisymmetric):
     # single precision variables not used within time loop but stored directly
     # to the output file for all files
-    variables = dotdict({
-        'dx': kgrid.dx,
-        'dy': kgrid.dy,
-        'dz': kgrid.dz,
-
-        'pml_x_alpha': opt.pml_x_alpha,
-        'pml_y_alpha': opt.pml_y_alpha,
-        'pml_z_alpha': opt.pml_z_alpha
-    })
+    variables = dotdict(
+        {
+            "dx": kgrid.dx,
+            "dy": kgrid.dy,
+            "dz": kgrid.dz,
+            "pml_x_alpha": opt.pml_x_alpha,
+            "pml_y_alpha": opt.pml_y_alpha,
+            "pml_z_alpha": opt.pml_z_alpha,
+        }
+    )
     float_variables.update(variables)
 
     if is_elastic_code:  # pragma: no cover
         grab_elastic_code_variables(float_variables, kgrid, values)
     elif is_axisymmetric:
         grab_axisymmetric_variables(float_variables, values)
     else:
         # single precision variables used within the time loop
-        float_variables['dt'] = values.dt
-        float_variables['c0'] = values.c0
-        float_variables['c_ref'] = values.c_ref
-        float_variables['rho0'] = values.rho0
-        float_variables['rho0_sgx'] = values.rho0_sgx
-        float_variables['rho0_sgy'] = values.rho0_sgy
-        float_variables['rho0_sgz'] = values.rho0_sgz
+        float_variables["dt"] = values.dt
+        float_variables["c0"] = values.c0
+        float_variables["c_ref"] = values.c_ref
+        float_variables["rho0"] = values.rho0
+        float_variables["rho0_sgx"] = values.rho0_sgx
+        float_variables["rho0_sgy"] = values.rho0_sgy
+        float_variables["rho0_sgz"] = values.rho0_sgz
 
 
 def grab_elastic_code_variables(float_variables, kgrid, values):  # pragma: no cover
     # single precision variables used within the time loop
-    float_variables['dt'] = None
-    float_variables['c_ref'] = None
-    float_variables['lambda'] = None
-    float_variables['mu'] = None
-
-    float_variables['rho0_sgx'] = None
-    float_variables['rho0_sgy'] = None
-    float_variables['rho0_sgz'] = None
-
-    float_variables['mu_sgxy'] = None
-    float_variables['mu_sgxz'] = None
-    float_variables['mu_sgyz'] = None
+    float_variables["dt"] = None
+    float_variables["c_ref"] = None
+    float_variables["lambda"] = None
+    float_variables["mu"] = None
+
+    float_variables["rho0_sgx"] = None
+    float_variables["rho0_sgy"] = None
+    float_variables["rho0_sgz"] = None
+
+    float_variables["mu_sgxy"] = None
+    float_variables["mu_sgxz"] = None
+    float_variables["mu_sgyz"] = None
 
     # create shift variables used for calculating u_non_staggered and I outputs
     x_shift_neg = np.fft.ifftshift(np.exp(-1j * kgrid.k_vec.x * kgrid.dx / 2))
     y_shift_neg = np.fft.ifftshift(np.exp(-1j * kgrid.k_vec.y * kgrid.dy / 2)).T
     z_shift_neg = np.transpose(np.fft.ifftshift(np.exp(-1j * kgrid.k_vec.z * kgrid.dz / 2)), (1, 2, 0))
 
     # create reduced variables for use with real-to-complex FFT
@@ -163,88 +166,95 @@
     Nx_r = kgrid.Nx // 2 + 1
     Ny_r = kgrid.Ny // 2 + 1
     Nz_r = Nz // 2 + 1
 
     ddx_k_shift_pos = values.ddx_k_shift_pos
     ddx_k_shift_neg = values.ddx_k_shift_neg
 
-    float_variables['ddx_k_shift_pos_r'] = ddx_k_shift_pos[:Nx_r]
-    float_variables['ddy_k_shift_pos'] = None
-    float_variables['ddz_k_shift_pos'] = None
-
-    float_variables['ddx_k_shift_neg_r'] = ddx_k_shift_neg[:Nx_r]
-    float_variables['ddy_k_shift_neg'] = None
-    float_variables['ddz_k_shift_neg'] = None
-
-    float_variables['x_shift_neg_r'] = x_shift_neg[:Nx_r]
-    float_variables['y_shift_neg_r'] = y_shift_neg[:Ny_r]
-    float_variables['z_shift_neg_r'] = z_shift_neg[:Nz_r]
+    float_variables["ddx_k_shift_pos_r"] = ddx_k_shift_pos[:Nx_r]
+    float_variables["ddy_k_shift_pos"] = None
+    float_variables["ddz_k_shift_pos"] = None
+
+    float_variables["ddx_k_shift_neg_r"] = ddx_k_shift_neg[:Nx_r]
+    float_variables["ddy_k_shift_neg"] = None
+    float_variables["ddz_k_shift_neg"] = None
+
+    float_variables["x_shift_neg_r"] = x_shift_neg[:Nx_r]
+    float_variables["y_shift_neg_r"] = y_shift_neg[:Ny_r]
+    float_variables["z_shift_neg_r"] = z_shift_neg[:Nz_r]
 
     del x_shift_neg
 
-    float_variables['pml_x'] = None
-    float_variables['pml_y'] = None
-    float_variables['pml_z'] = None
-
-    float_variables['pml_x_sgx'] = None
-    float_variables['pml_y_sgy'] = None
-    float_variables['pml_z_sgz'] = None
-
-    float_variables['mpml_x_sgx'] = None
-    float_variables['mpml_y_sgy'] = None
-    float_variables['mpml_z_sgz'] = None
-
-    float_variables['mpml_x'] = None
-    float_variables['mpml_y'] = None
-    float_variables['mpml_z'] = None
+    float_variables["pml_x"] = None
+    float_variables["pml_y"] = None
+    float_variables["pml_z"] = None
+
+    float_variables["pml_x_sgx"] = None
+    float_variables["pml_y_sgy"] = None
+    float_variables["pml_z_sgz"] = None
+
+    float_variables["mpml_x_sgx"] = None
+    float_variables["mpml_y_sgy"] = None
+    float_variables["mpml_z_sgz"] = None
+
+    float_variables["mpml_x"] = None
+    float_variables["mpml_y"] = None
+    float_variables["mpml_z"] = None
 
 
 def grab_axisymmetric_variables(float_variables, values):
     # single precision variables used within the time loop
-    float_variables['dt'] = values.dt
-    float_variables['c0'] = values.c0
-    float_variables['c_ref'] = values.c_ref
-    float_variables['rho0'] = values.rho0
-    float_variables['rho0_sgx'] = values.rho0_sgx
-    float_variables['rho0_sgy'] = values.rho0_sgy
+    float_variables["dt"] = values.dt
+    float_variables["c0"] = values.c0
+    float_variables["c_ref"] = values.c_ref
+    float_variables["rho0"] = values.rho0
+    float_variables["rho0_sgx"] = values.rho0_sgx
+    float_variables["rho0_sgy"] = values.rho0_sgy
 
 
 def grab_medium_props(integer_variables, float_variables, medium, is_elastic_code):
     # =========================================================================
     # VARIABLES USED IN NONLINEAR SIMULATIONS
     # =========================================================================
     if medium.is_nonlinear():
-        float_variables['BonA'] = medium.BonA
+        float_variables["BonA"] = medium.BonA
 
     # =========================================================================
     # VARIABLES USED IN ABSORBING SIMULATIONS
     # =========================================================================
 
     # set absorbing flag
     if medium.absorbing:
         integer_variables.absorbing_flag = 2 if medium.stokes else 1
     else:
         integer_variables.absorbing_flag = 0
 
     if medium.absorbing:
         if is_elastic_code:  # pragma: no cover
             # add to the variable list
-            float_variables['chi'] = None
-            float_variables['eta'] = None
-            float_variables['eta_sgxy'] = None
-            float_variables['eta_sgxz'] = None
-            float_variables['eta_sgyz'] = None
+            float_variables["chi"] = None
+            float_variables["eta"] = None
+            float_variables["eta_sgxy"] = None
+            float_variables["eta_sgxz"] = None
+            float_variables["eta_sgyz"] = None
         else:
-            float_variables['alpha_coeff'] = medium.alpha_coeff
-            float_variables['alpha_power'] = medium.alpha_power
+            float_variables["alpha_coeff"] = medium.alpha_coeff
+            float_variables["alpha_power"] = medium.alpha_power
 
 
-def grab_source_props(integer_variables, float_variables, source,
-                      u_source_pos_index, s_source_pos_index, p_source_pos_index,
-                      transducer_input_signal, delay_mask):
+def grab_source_props(
+    integer_variables,
+    float_variables,
+    source,
+    u_source_pos_index,
+    s_source_pos_index,
+    p_source_pos_index,
+    transducer_input_signal,
+    delay_mask,
+):
     # =========================================================================
     # SOURCE VARIABLES
     # =========================================================================
     # source modes and indicies
     # - these are only defined if the source flgs are > 0
     # - the source mode describes whether the source will be added or replaced
     # - the source indicies describe which grid points act as the source
@@ -254,37 +264,43 @@
     grab_stress_source_props(integer_variables, source, s_source_pos_index)
     grab_pressure_source_props(integer_variables, source, p_source_pos_index, u_source_pos_index)
     grab_time_varying_source_props(integer_variables, float_variables, source, transducer_input_signal, delay_mask)
 
 
 def grab_velocity_source_props(integer_variables, source, u_source_pos_index):
     # velocity source
-    if any(integer_variables.get(k) for k in ['ux_source_flag', 'uy_source_flag', 'uz_source_flag']):
-        integer_variables['u_source_mode'] = {
-            'dirichlet': 0,
-            'additive-no-correction': 1,
-            'additive': 2,
+    if any(integer_variables.get(k) for k in ["ux_source_flag", "uy_source_flag", "uz_source_flag"]):
+        integer_variables["u_source_mode"] = {
+            "dirichlet": 0,
+            "additive-no-correction": 1,
+            "additive": 2,
         }[source.u_mode]
 
         if integer_variables.ux_source_flag:
             u_source_many = num_dim2(source.ux) > 1
         elif integer_variables.uy_source_flag:
             u_source_many = num_dim2(source.uy) > 1
         elif integer_variables.uz_source_flag:
             u_source_many = num_dim2(source.uz) > 1
-        integer_variables['u_source_many'] = u_source_many
+        integer_variables["u_source_many"] = u_source_many
 
         integer_variables.u_source_index = u_source_pos_index
 
 
 def grab_stress_source_props(integer_variables, source, s_source_pos_index):
     # stress source
-    if integer_variables.sxx_source_flag or integer_variables.syy_source_flag or integer_variables.szz_source_flag \
-            or integer_variables.sxy_source_flag or integer_variables.sxz_source_flag or integer_variables.syz_source_flag:
-        integer_variables.s_source_mode = source.s_mode != 'dirichlet'
+    if (
+        integer_variables.sxx_source_flag
+        or integer_variables.syy_source_flag
+        or integer_variables.szz_source_flag
+        or integer_variables.sxy_source_flag
+        or integer_variables.sxz_source_flag
+        or integer_variables.syz_source_flag
+    ):
+        integer_variables.s_source_mode = source.s_mode != "dirichlet"
         if integer_variables.sxx_source_flag:
             s_source_many = num_dim2(source.sxx) > 1
         elif integer_variables.syy_source_flag:
             s_source_many = num_dim2(source.syy) > 1
         elif integer_variables.szz_source_flag:
             s_source_many = num_dim2(source.szz) > 1
         elif integer_variables.sxy_source_flag:
@@ -297,17 +313,17 @@
         integer_variables.s_source_index = s_source_pos_index
 
 
 def grab_pressure_source_props(integer_variables, source, p_source_pos_index, u_source_pos_index):
     # pressure source
     if integer_variables.p_source_flag:
         integer_variables.p_source_mode = {
-            'dirichlet': 0,
-            'additive-no-correction': 1,
-            'additive': 2,
+            "dirichlet": 0,
+            "additive-no-correction": 1,
+            "additive": 2,
         }[source.p_mode]
         integer_variables.p_source_many = num_dim2(source.p) > 1
         integer_variables.p_source_index = p_source_pos_index
 
     # transducer source
     if integer_variables.transducer_source_flag:
         integer_variables.u_source_index = u_source_pos_index
@@ -365,29 +381,28 @@
     # =========================================================================
 
     if integer_variables.sensor_mask_type == 0:
         # mask is defined as a list of grid indices
         integer_variables.sensor_mask_index = sensor_mask_index
 
     elif integer_variables.sensor_mask_type == 1:
-
         cuboid_corners_list = cuboid_corners_list
         # mask is defined as a list of cuboid corners
         if kgrid_dim == 2:
             sensor_mask_corners = np.ones((6, cuboid_corners_list.shape[1]))
             sensor_mask_corners[0, :] = cuboid_corners_list[0, :]
             sensor_mask_corners[1, :] = cuboid_corners_list[1, :]
             sensor_mask_corners[3, :] = cuboid_corners_list[2, :]
             sensor_mask_corners[4, :] = cuboid_corners_list[3, :]
         else:
             sensor_mask_corners = cuboid_corners_list
         integer_variables.sensor_mask_corners = sensor_mask_corners
 
     else:
-        raise NotImplementedError('unknown option for sensor_mask_type')
+        raise NotImplementedError("unknown option for sensor_mask_type")
 
 
 def grab_nonuniform_grid_props(float_variables, kgrid, is_nonuniform_grid):
     # =========================================================================
     # VARIABLES USED FOR NONUNIFORM GRIDS
     # =========================================================================
 
@@ -396,73 +411,73 @@
     # - these are applied using the bsxfun formulation
     if not is_nonuniform_grid:
         return
 
     dxudxn = kgrid.dudn.x
     if np.array(dxudxn).size == 1:
         dxudxn = np.ones((kgrid.Nx, 1))
-    float_variables['dxudxn'] = dxudxn
+    float_variables["dxudxn"] = dxudxn
 
     dyudyn = kgrid.dudn.y
     if np.array(dyudyn).size == 1:
         dyudyn = np.ones((1, kgrid.Ny))
-    float_variables['dyudyn'] = dyudyn
+    float_variables["dyudyn"] = dyudyn
 
     dzudzn = kgrid.dudn.z
     if np.array(dzudzn).size == 1:
         dzudzn = np.ones((1, 1, kgrid.Nz))
-    float_variables['dzudzn'] = dzudzn
+    float_variables["dzudzn"] = dzudzn
 
     dxudxn_sgx = kgrid.dudn_sg.x
     if np.array(dxudxn).size == 1:
         dxudxn_sgx = np.ones((kgrid.Nx, 1))
-    float_variables['dxudxn_sgx'] = dxudxn_sgx
+    float_variables["dxudxn_sgx"] = dxudxn_sgx
 
     dyudyn_sgy = kgrid.dudn_sg.y
     if np.array(dyudyn).size == 1:
         dyudyn_sgy = np.ones((1, kgrid.Ny))
-    float_variables['dyudyn_sgy'] = dyudyn_sgy
+    float_variables["dyudyn_sgy"] = dyudyn_sgy
 
     dzudzn_sgz = kgrid.dudn_sg.z
     if np.array(dzudzn).size == 1:
         dzudzn_sgz = np.ones((1, 1, kgrid.Nz))
-    float_variables['dzudzn_sgz'] = dzudzn_sgz
+    float_variables["dzudzn_sgz"] = dzudzn_sgz
 
 
 def remove_z_dimension(float_variables, kgrid_dim):
     # remove z-dimension variables for saving 2D files
     if kgrid_dim == 2:
         for k in list(float_variables.keys()):
-            if 'z' in k:
+            if "z" in k:
                 del float_variables[k]
 
 
 def enforce_filename_standards(filepath):
     # check for HDF5 filename extension
     filename_ext = os.path.splitext(filepath)[1]
 
     # use .h5 as default if no extension is given
     if len(filename_ext) == 0:
-        filename_ext = '.h5'
-        filepath = filepath + '.h5'
+        filename_ext = ".h5"
+        filepath = filepath + ".h5"
     return filepath, filename_ext
 
 
 def save_file(filepath, integer_variables, float_variables, hdf_compression_level, auto_chunk):
     filepath, filename_ext = enforce_filename_standards(filepath)
 
     # save file
-    if filename_ext == '.h5':
+    if filename_ext == ".h5":
         save_h5_file(filepath, integer_variables, float_variables, hdf_compression_level, auto_chunk)
 
-    elif filename_ext == '.mat':
+    elif filename_ext == ".mat":
         save_mat_file(filepath, integer_variables, float_variables)
     else:
         # throw error for unknown filetype
-        raise NotImplementedError('unknown file extension for ''save_to_disk'' filename')
+        raise NotImplementedError("unknown file extension for " "save_to_disk" " filename")
 
 
 def save_h5_file(filepath, integer_variables, float_variables, hdf_compression_level, auto_chunk):
     # ----------------
     # SAVE HDF5 FILE
     # ----------------
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/scale_source_terms_func.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/scale_source_terms_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 from kwave.kgrid import kWaveGrid
 from kwave.ksource import kSource
 from kwave.utils.dotdictionary import dotdict
 
 
 def scale_source_terms_func(
-        c0, dt, kgrid: kWaveGrid, source,
-        p_source_pos_index, s_source_pos_index, u_source_pos_index,
-        transducer_input_signal,
-        flags: dotdict):
+    c0, dt, kgrid: kWaveGrid, source, p_source_pos_index, s_source_pos_index, u_source_pos_index, transducer_input_signal, flags: dotdict
+):
     """
     Subscript for the first-order k-Wave simulation functions to scale source terms to the correct units.
     Args:
     Returns:
 
     """
-    dx, dy, dz  = kgrid.dx, kgrid.dy, kgrid.dz,
+    dx, dy, dz = (
+        kgrid.dx,
+        kgrid.dy,
+        kgrid.dz,
+    )
 
     # get the dimension size
     N = kgrid.dim
 
     if not check_conditions(flags.nonuniform_grid, flags.source_uy, flags.source_uz, flags.transducer_source):
         return
 
@@ -48,27 +50,26 @@
     apply_velocity_source_corrections(flags.use_w_source_correction_u, flags.source_ux, flags.source_uy, flags.source_uz, source, dt)
 
     scale_velocity_sources(flags, source, kgrid, c0, dt, dx, dy, dz, u_source_pos_index)
 
     # =========================================================================
     # TRANSDUCER SOURCE
     # =========================================================================
-    transducer_input_signal = scale_transducer_source(flags.transducer_source, transducer_input_signal,
-                                                      c0, dt, dx, u_source_pos_index)
+    transducer_input_signal = scale_transducer_source(flags.transducer_source, transducer_input_signal, c0, dt, dx, u_source_pos_index)
     return transducer_input_signal
 
 
 def check_conditions(is_nonuniform_grid, is_source_uy, is_source_uz, is_transducer_source):
     """
     check for non-uniform grid and give error for source terms that haven't yet been implemented
     Returns:
 
     """
     if is_nonuniform_grid and (is_source_uy or is_source_uz or is_transducer_source):
-        logging.log(logging.WARN, 'source scaling not implemented for non-uniform grids with given source condition')
+        logging.log(logging.WARN, "source scaling not implemented for non-uniform grids with given source condition")
         return False
     return True
 
 
 def apply_pressure_source_correction(is_source_p, use_w_source_correction_p, source, dt):
     """
     apply k-space source correction expressed as a function of w
@@ -104,36 +105,36 @@
 
     Returns:
 
     """
     if not is_source_p:
         return
 
-    if source.p_mode == 'dirichlet':
+    if source.p_mode == "dirichlet":
         source.p = scale_pressure_source_dirichlet(source.p, c0, N, p_source_pos_index)
     else:
         if is_nonuniform_grid:
             source.p = scale_pressure_source_nonuniform_grid(source.p, kgrid, c0, N, dt, p_source_pos_index)
 
         else:
             source.p = scale_pressure_source_uniform_grid(source.p, c0, N, dx, dt, p_source_pos_index)
 
 
 def scale_pressure_source_dirichlet(source_p, c0, N, p_source_pos_index):
     if c0.size == 1:
         # compute the scale parameter based on the homogeneous
         # sound speed
-        source_p = source_p / (N * (c0 ** 2))
+        source_p = source_p / (N * (c0**2))
 
     else:
         # compute the scale parameter seperately for each source
         # position based on the sound speed at that position
         ind = range(source_p[:, 0].size)
-        mask = p_source_pos_index.flatten('F')[ind]
-        scale = 1.0 / (N * np.expand_dims(c0.ravel(order='F')[mask.ravel(order='F')] ** 2, axis=-1) )
+        mask = p_source_pos_index.flatten("F")[ind]
+        scale = 1.0 / (N * np.expand_dims(c0.ravel(order="F")[mask.ravel(order="F")] ** 2, axis=-1))
         source_p[ind, :] *= scale
 
     return source_p
 
 
 def scale_pressure_source_nonuniform_grid(source_p, kgrid, c0, N, dt, p_source_pos_index):
     x = kgrid.x
@@ -148,49 +149,48 @@
     # compute averaged grid point seperation map, the interior
     # points are calculated using the average distance to all
     # connected grid points (the edge values are not calculated
     # assuming there are no source points in the PML)
     if kgrid.dim == 1:
         grid_point_sep[1:-1] = x_size * (xn[2:, 0] - xn[0:-2, 0]) / 2
     elif kgrid.dim == 2:
-        grid_point_sep[1:-1, 1:-1] = x_size * (xn[2:, 1:-1] - xn[0:-2, 1:- 1]) / 4 + \
-                                     y_size * (yn[1:-1, 2:] - yn[1:-1, 0:-2]) / 4
+        grid_point_sep[1:-1, 1:-1] = x_size * (xn[2:, 1:-1] - xn[0:-2, 1:-1]) / 4 + y_size * (yn[1:-1, 2:] - yn[1:-1, 0:-2]) / 4
     elif kgrid.dim == 3:
-        grid_point_sep[1:-1, 1:-1, 1:-1] = x_size * (xn[2:, 1:-1, 1:-1] - xn[0:-2, 1:-1, 1:-1]) / 6 + \
-                                           y_size * (yn[1:-1, 2:, 1:-1] - yn[1:-1, 0:-2, 1:- 1]) / 6 + \
-                                           z_size * (zn[1:-1, 1:-1, 2:] - zn[1:-1, 1:-1, 0:-2]) / 6
+        grid_point_sep[1:-1, 1:-1, 1:-1] = (
+            x_size * (xn[2:, 1:-1, 1:-1] - xn[0:-2, 1:-1, 1:-1]) / 6
+            + y_size * (yn[1:-1, 2:, 1:-1] - yn[1:-1, 0:-2, 1:-1]) / 6
+            + z_size * (zn[1:-1, 1:-1, 2:] - zn[1:-1, 1:-1, 0:-2]) / 6
+        )
 
     # compute and apply scale parameter
     for p_index in range(source_p.size[0]):
         if c0.size == 1:
-
             # compute the scale parameter based on the homogeneous sound speed
-            source_p[p_index, :] = source_p[p_index, :] * \
-                                   (2 * dt / (N * c0 * grid_point_sep[p_source_pos_index[p_index]]))
+            source_p[p_index, :] = source_p[p_index, :] * (2 * dt / (N * c0 * grid_point_sep[p_source_pos_index[p_index]]))
 
         else:
-
             # compute the scale parameter based on the sound speed at that position
-            source_p[p_index, :] = source_p[p_index, :] * (2 * dt / (N * c0[p_source_pos_index[p_index]] *
-                                                                     grid_point_sep[p_source_pos_index[p_index]]))
+            source_p[p_index, :] = source_p[p_index, :] * (
+                2 * dt / (N * c0[p_source_pos_index[p_index]] * grid_point_sep[p_source_pos_index[p_index]])
+            )
     return source_p
 
 
 def scale_pressure_source_uniform_grid(source_p, c0, N, dx, dt, p_source_pos_index):
     if c0.size == 1:
         # compute the scale parameter based on the homogeneous
         # sound speed
         source_p = source_p * (2 * dt / (N * c0 * dx))
 
     else:
         # compute the scale parameter seperately for each source
         # position based on the sound speed at that position
         ind = range(source_p[:, 0].size)
-        mask = p_source_pos_index.flatten('F')[ind]
-        scale = (2.0 * dt) / (N * np.expand_dims(c0.ravel(order='F')[mask.ravel(order='F')], axis=-1) * dx)
+        mask = p_source_pos_index.flatten("F")[ind]
+        scale = (2.0 * dt) / (N * np.expand_dims(c0.ravel(order="F")[mask.ravel(order="F")], axis=-1) * dx)
         source_p[ind, :] *= scale
     return source_p
 
 
 def scale_stress_sources(source, c0, flags, dt, dx, N, s_source_pos_index):
     """
     scale the stress source by 1/N to divide amoungst the split field
@@ -215,35 +215,32 @@
     source.sxy = scale_stress_source(source, c0, flags.source_sxy, True, source.sxy, dt, N, dx, s_source_pos_index)
     source.sxz = scale_stress_source(source, c0, flags.source_sxz, True, source.sxz, dt, N, dx, s_source_pos_index)
     source.syz = scale_stress_source(source, c0, flags.source_syz, True, source.syz, dt, N, dx, s_source_pos_index)
 
 
 def scale_stress_source(source, c0, is_source_exists, is_p0_exists, source_val, dt, N, dx, s_source_pos_index):
     if is_source_exists:
-        if source.s_mode == 'dirichlet' or is_p0_exists:
+        if source.s_mode == "dirichlet" or is_p0_exists:
             source_val = source_val / N
         else:
             if c0.size == 1:
-
                 # compute the scale parameter based on the homogeneous sound
                 # speed
                 source_val = source_val * (2 * dt * c0 / (N * dx))
 
             else:
-
                 # compute the scale parameter seperately for each source
                 # position based on the sound speed at that position
                 s_index = range(source_val.size[0])
                 source_val[s_index, :] = source_val[s_index, :] * (2 * dt * c0[s_source_pos_index[s_index]] / (N * dx))
     return source_val
 
 
 def apply_velocity_source_corrections(
-        use_w_source_correction_u: bool, is_ux_exists: bool, is_uy_exists: bool, is_uz_exists: bool,
-        source: kSource, dt: float
+    use_w_source_correction_u: bool, is_ux_exists: bool, is_uy_exists: bool, is_uz_exists: bool, source: kSource, dt: float
 ):
     """
     apply k-space source correction expressed as a function of w
     Args:
         use_w_source_correction_u:
         is_ux_exists:
         is_uy_exists:
@@ -264,40 +261,38 @@
         source.uy = apply_source_correction(source.uy, source.u_frequency_ref, dt)
 
     if is_uz_exists:
         source.uz = apply_source_correction(source.uz, source.u_frequency_ref, dt)
 
 
 def apply_source_correction(source_val, frequency_ref, dt):
-    return source_val * math.cos(2 * math.pi * frequency_ref * dt/2)
+    return source_val * math.cos(2 * math.pi * frequency_ref * dt / 2)
 
 
 def scale_velocity_sources(flags, source, kgrid, c0, dt, dx, dy, dz, u_source_pos_index):
-    source.ux = scale_velocity_source_x(flags.source_ux,
-                                        source.u_mode,
-                                        source.ux,
-                                        kgrid, c0, dt, dx, u_source_pos_index, flags.nonuniform_grid)
+    source.ux = scale_velocity_source_x(
+        flags.source_ux, source.u_mode, source.ux, kgrid, c0, dt, dx, u_source_pos_index, flags.nonuniform_grid
+    )
     source.uy = scale_velocity_source(flags.source_uy, source.u_mode, source.uy, c0, dt, u_source_pos_index, dy)
     source.uz = scale_velocity_source(flags.source_uz, source.u_mode, source.uz, c0, dt, u_source_pos_index, dz)
 
 
 def scale_velocity_source_x(is_source_ux, source_u_mode, source_val, kgrid, c0, dt, dx, u_source_pos_index, is_nonuniform_grid):
     """
     if source.u_mode is not set to 'dirichlet', scale the x-direction
     velocity source terms by 2*dt*c0/dx to account for the time step and
     convert to units of [m/s^2]
     Returns:
 
     """
-    if not is_source_ux or source_u_mode == 'dirichlet':
+    if not is_source_ux or source_u_mode == "dirichlet":
         return
 
     if is_nonuniform_grid:
-        source_val = scale_velocity_source_nonuniform(is_source_ux, source_u_mode, kgrid, source_val,
-                                                      c0, dt, u_source_pos_index)
+        source_val = scale_velocity_source_nonuniform(is_source_ux, source_u_mode, kgrid, source_val, c0, dt, u_source_pos_index)
     else:
         source_val = scale_velocity_source(is_source_ux, source_u_mode, source_val, c0, dt, u_source_pos_index, dx)
     return source_val
 
 
 def scale_velocity_source(is_source, source_u_mode, source_val, c0, dt, u_source_pos_index, d_direction):
     """
@@ -312,15 +307,15 @@
         dt:
         u_source_pos_index:
         d_direction:
 
     Returns:
 
     """
-    if not is_source or source_u_mode == 'dirichlet':
+    if not is_source or source_u_mode == "dirichlet":
         return source_val
 
     if c0.size == 1:
         # compute the scale parameter based on the homogeneous sound speed
         source_val = source_val * (2 * c0 * dt / d_direction)
     else:
         # compute the scale parameter seperately for each source position
@@ -343,39 +338,39 @@
         c0:
         dt:
         u_source_pos_index:
 
     Returns:
 
     """
-    if not is_source or source_u_mode == 'dirichlet':
+    if not is_source or source_u_mode == "dirichlet":
         return source_val
 
     # create empty matrix
     x = kgrid.x
     xn = kgrid.xn
     x_size = kgrid.size[0]
     grid_point_sep = np.zeros_like(x)
 
     # compute averaged grid point seperation map, the interior
     # points are calculated using the average distance to all
     # connected grid points (the edge values are not calculated
     # assuming there are no source points in the PML)
-    grid_point_sep[1:- 1, :, :] = x_size * (xn[2:, :, :] - xn[1:- 2, :, :]) / 2
+    grid_point_sep[1:-1, :, :] = x_size * (xn[2:, :, :] - xn[1:-2, :, :]) / 2
 
     # compute and apply scale parameter
     for u_index in range(source_val.size[0]):
         if c0.size == 1:
             # compute the scale parameter based on the homogeneous sound speed
             source_val[u_index, :] = source_val[u_index, :] * (2 * c0 * dt / (grid_point_sep[u_source_pos_index[u_index]]))
         else:
             # compute the scale parameter based on the sound speed at that position
-            source_val[u_index, :] = source_val[u_index, :] * \
-                                     (2 * c0[u_source_pos_index[u_index]] *
-                                      dt / (grid_point_sep[u_source_pos_index[u_index]]))
+            source_val[u_index, :] = source_val[u_index, :] * (
+                2 * c0[u_source_pos_index[u_index]] * dt / (grid_point_sep[u_source_pos_index[u_index]])
+            )
     return source_val
 
 
 def scale_transducer_source(is_transducer_source, transducer_input_signal, c0, dt, dx, u_source_pos_index):
     """
     scale the transducer source term by 2*dt*c0/dx to account for the time
     step and convert to units of [m/s^2]
@@ -392,9 +387,9 @@
     """
     if is_transducer_source:
         if c0.size == 1:
             transducer_input_signal = transducer_input_signal * (2 * c0 * dt / dx)
         else:
             # compute the scale parameter based on the average sound speed at the
             # transducer positions (only one input signal is used to drive the transducer)
-            transducer_input_signal = transducer_input_signal * (2 * (np.mean(c0.flatten(order='F')[u_source_pos_index - 1])) * dt / dx)
+            transducer_input_signal = transducer_input_signal * (2 * (np.mean(c0.flatten(order="F")[u_source_pos_index - 1])) * dt / dx)
     return transducer_input_signal
```

### Comparing `k_wave_python-0.3.2/kwave/kWaveSimulation_helper/set_sound_speed_ref.py` & `k_wave_python-0.3.3/kwave/kWaveSimulation_helper/set_sound_speed_ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,63 +32,59 @@
     Args:
         medium:
 
     Returns:
 
     """
     c_ref = _get_sound_speed_ref(medium.sound_speed_ref, medium.sound_speed)
-    logging.log(logging.INFO, '  reference sound speed: ', c_ref, 'm/s')
+    logging.log(logging.INFO, "  reference sound speed: ", c_ref, "m/s")
     return c_ref, None, None
 
 
 def get_pstd_elastic_sound_speed_ref(medium: kWaveMedium):  # pragma: no cover
     """
     in the pstd elastic case, the reference sound speed is only used to
     calculate the PML absorption, so just use the compressional wave speed
     Args:
         medium:
 
     Returns:
 
     """
     c_ref = _get_sound_speed_ref(medium.sound_speed_ref, medium.sound_speed_compression)
-    logging.log(logging.INFO, '  reference sound speed: ', c_ref, 'm/s')
+    logging.log(logging.INFO, "  reference sound speed: ", c_ref, "m/s")
     return c_ref, None, None
 
 
 def get_kspace_elastic_sound_speed_ref(medium: kWaveMedium):  # pragma: no cover
     """
     in the k-space elastic case, there are two reference sound speeds for
     the compressional and shear waves, so compute them seperately
     Args:
         medium:
 
     Returns:
 
     """
     c_ref_compression = _get_sound_speed_ref(medium.sound_speed_ref_compression, medium.sound_speed_compression)
-    logging.log(logging.INFO, '  reference sound speed (compression): ', c_ref_compression, 'm/s')
+    logging.log(logging.INFO, "  reference sound speed (compression): ", c_ref_compression, "m/s")
 
     c_ref_shear = _get_sound_speed_ref(medium.sound_speed_ref_shear, medium.sound_speed_shear)
-    logging.log(logging.INFO, '  reference sound speed (shear): ', c_ref_shear, 'm/s')
+    logging.log(logging.INFO, "  reference sound speed (shear): ", c_ref_shear, "m/s")
 
     return None, c_ref_compression, c_ref_shear
 
 
 def _get_sound_speed_ref(reference, speed):
-    reductions = {
-        'min': np.min,
-        'max': np.max,
-        'mean': np.mean
-    }
+    reductions = {"min": np.min, "max": np.max, "mean": np.mean}
 
     if reference is not None:
         # if reference is defined, check whether it is a scalar or 'reduction'
         if np.isscalar(reference):
             c_ref = reference
         else:
             c_ref = reductions[reference](speed)
     else:
-        c_ref = reductions['max'](speed)
+        c_ref = reductions["max"](speed)
 
-    logging.log(logging.INFO, '  reference sound speed: ', c_ref, 'm/s')
+    logging.log(logging.INFO, "  reference sound speed: ", c_ref, "m/s")
     return float(c_ref)
```

### Comparing `k_wave_python-0.3.2/kwave/options/simulation_execution_options.py` & `k_wave_python-0.3.3/kwave/options/simulation_execution_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 @dataclass
 class SimulationExecutionOptions:
     # Are we going to run the simulation on the GPU?
     # Affects binary name and the way the simulation is run
     is_gpu_simulation: bool = False
 
     # user defined location for the binary
-    binary_path: Optional[str] = os.getenv('KWAVE_BINARY_PATH')
+    binary_path: Optional[str] = os.getenv("KWAVE_BINARY_PATH")
     # user defined location for the binary
     binary_name: Optional[str] = None
     # user defined number of threads
-    kwave_function_name: Optional[str] = 'kspaceFirstOrder3D'
+    kwave_function_name: Optional[str] = "kspaceFirstOrder3D"
     # Whether to delete the input and output files after the simulation
     delete_data: bool = True
     # GPU device flag
     device_num: Optional[int] = None
     # number of threads
-    num_threads: Union[int, str] = 'all'
+    num_threads: Union[int, str] = "all"
 
     # user defined thread binding option
     thread_binding: Optional[bool] = None
 
     # user input for system string
     system_call: Optional[str] = None
     verbose_level: int = 0
@@ -41,115 +41,115 @@
     show_sim_log: bool = True
 
     def __post_init__(self):
         self.validate()
 
         if self.binary_name is None:
             if self.is_gpu_simulation:
-                self.binary_name = 'kspaceFirstOrder-CUDA' if is_unix() else 'kspaceFirstOrder-CUDA.exe'
+                self.binary_name = "kspaceFirstOrder-CUDA" if is_unix() else "kspaceFirstOrder-CUDA.exe"
             else:
-                self.binary_name = 'kspaceFirstOrder-OMP' if is_unix() else 'kspaceFirstOrder-OMP.exe'
+                self.binary_name = "kspaceFirstOrder-OMP" if is_unix() else "kspaceFirstOrder-OMP.exe"
 
-        self._is_linux = sys.platform.startswith('linux')
-        self._is_windows = sys.platform.startswith(('win', 'cygwin'))
-        self._is_darwin = sys.platform.startswith('darwin')
+        self._is_linux = sys.platform.startswith("linux")
+        self._is_windows = sys.platform.startswith(("win", "cygwin"))
+        self._is_darwin = sys.platform.startswith("darwin")
 
         if self._is_linux:
-            binary_folder = 'linux'
+            binary_folder = "linux"
         elif self._is_windows:
-            binary_folder = 'windows'
+            binary_folder = "windows"
         elif self._is_darwin:
-            raise NotImplementedError('k-wave-python is currently unsupported on MacOS.')
+            raise NotImplementedError("k-wave-python is currently unsupported on MacOS.")
 
         path_to_kwave = Path(__file__).parent.parent.resolve()
-        self.binary_path = path_to_kwave / 'bin' / binary_folder / self.binary_name
+        self.binary_path = path_to_kwave / "bin" / binary_folder / self.binary_name
 
     def validate(self):
         if isinstance(self.num_threads, int):
-            assert self.num_threads > 0 and self.num_threads != float('inf')
+            assert self.num_threads > 0 and self.num_threads != float("inf")
         else:
-            assert self.num_threads == 'all'
+            assert self.num_threads == "all"
             self.num_threads = None
 
         assert isinstance(self.verbose_level, int) and 0 <= self.verbose_level <= 2
 
     def get_options_string(self, sensor: kSensor) -> str:
         options_dict = {}
         if self.device_num:
-            options_dict['-g'] = self.device_num
+            options_dict["-g"] = self.device_num
 
         if self.num_threads:
-            options_dict['-t'] = self.num_threads
+            options_dict["-t"] = self.num_threads
 
         if self.verbose_level:
-            options_dict['--verbose'] = self.verbose_level
+            options_dict["--verbose"] = self.verbose_level
 
-        options_string = ''
+        options_string = ""
         for flag, value in options_dict.items():
-            options_string += f' {flag} {str(value)}'
+            options_string += f" {flag} {str(value)}"
 
         # check if sensor.record is given
         if sensor.record is not None:
             record = sensor.record
 
             # set the options string to record the required output fields
             record_options_map = {
-                'p': 'p_raw',
-                'p_max': 'p_max',
-                'p_min': 'p_min',
-                'p_rms': 'p_rms',
-                'p_max_all': 'p_max_all',
-                'p_min_all': 'p_min_all',
-                'p_final': 'p_final',
-                'u': 'u_raw',
-                'u_max': 'u_max',
-                'u_min': 'u_min',
-                'u_rms': 'u_rms',
-                'u_max_all': 'u_max_all',
-                'u_min_all': 'u_min_all',
-                'u_final': 'u_final'
+                "p": "p_raw",
+                "p_max": "p_max",
+                "p_min": "p_min",
+                "p_rms": "p_rms",
+                "p_max_all": "p_max_all",
+                "p_min_all": "p_min_all",
+                "p_final": "p_final",
+                "u": "u_raw",
+                "u_max": "u_max",
+                "u_min": "u_min",
+                "u_rms": "u_rms",
+                "u_max_all": "u_max_all",
+                "u_min_all": "u_min_all",
+                "u_final": "u_final",
             }
             for k, v in record_options_map.items():
                 if k in record:
-                    options_string = options_string + f' --{v}'
+                    options_string = options_string + f" --{v}"
 
-            if 'u_non_staggered' in record or 'I_avg' in record or 'I' in record:
-                options_string = options_string + ' --u_non_staggered_raw'
+            if "u_non_staggered" in record or "I_avg" in record or "I" in record:
+                options_string = options_string + " --u_non_staggered_raw"
 
-            if ('I_avg' in record or 'I' in record) and ('p' not in record):
-                options_string = options_string + ' --p_raw'
+            if ("I_avg" in record or "I" in record) and ("p" not in record):
+                options_string = options_string + " --p_raw"
         else:
             # if sensor.record is not given, record the raw time series of p
-            options_string = options_string + ' --p_raw'
+            options_string = options_string + " --p_raw"
 
         # check if sensor.record_start_imdex is given
         if sensor.record_start_index is not None:
-            options_string = options_string + ' -s ' + str(sensor.record_start_index)
+            options_string = options_string + " -s " + str(sensor.record_start_index)
         return options_string
 
     @property
     def system_string(self):
         # set OS string for setting environment variables
         if is_unix():
-            env_set_str = ''
-            sys_sep_str = ' '
+            env_set_str = ""
+            sys_sep_str = " "
         else:
-            env_set_str = 'set '
-            sys_sep_str = ' & '
+            env_set_str = "set "
+            sys_sep_str = " & "
 
         # set system string to define domain for thread migration
-        system_string = env_set_str + 'OMP_PLACES=cores' + sys_sep_str
+        system_string = env_set_str + "OMP_PLACES=cores" + sys_sep_str
 
         if self.thread_binding is not None:
             # read the parameters and update the system options
             if self.thread_binding:
-                system_string = system_string + ' ' + env_set_str + 'OMP_PROC_BIND=SPREAD' + sys_sep_str
+                system_string = system_string + " " + env_set_str + "OMP_PROC_BIND=SPREAD" + sys_sep_str
             else:
-                system_string = system_string + ' ' + env_set_str + 'OMP_PROC_BIND=CLOSE' + sys_sep_str
+                system_string = system_string + " " + env_set_str + "OMP_PROC_BIND=CLOSE" + sys_sep_str
         else:
             # set to round-robin over places
-            system_string = system_string + ' ' + env_set_str + 'OMP_PROC_BIND=SPREAD' + sys_sep_str
+            system_string = system_string + " " + env_set_str + "OMP_PROC_BIND=SPREAD" + sys_sep_str
 
         if self.system_call:
-            system_string = system_string + ' ' + self.system_call + sys_sep_str
+            system_string = system_string + " " + self.system_call + sys_sep_str
 
         return system_string
```

### Comparing `k_wave_python-0.3.2/kwave/options/simulation_options.py` & `k_wave_python-0.3.3/kwave/options/simulation_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     Rules from the original matlab code:
         AXISYMMETRIC => if the calling function name started with 'kspaceFirstOrderAS'
                             or if the userarg_axisymmetric is set to true
         ELASTIC => if the calling function name started with 'pstdElastic' or 'kspaceElastic'
         ELASTIC_WITH_KSPACE_CORRECTION => if the calling function name started with 'kspaceElastic'
     """
+
     FLUID = 1
     AXISYMMETRIC = 2
     ELASTIC = 3
     ELASTIC_WITH_KSPACE_CORRECTION = 4
 
     def is_elastic_simulation(self):
         return self in [SimulationType.ELASTIC, SimulationType.ELASTIC_WITH_KSPACE_CORRECTION]
@@ -77,18 +78,18 @@
         multi_axial_PML_ratio: MPML settings
         pml_x_alpha: PML Alpha for x-axis
         pml_y_alpha: PML Alpha for y-axis
         pml_z_alpha: PML Alpha for z-axis
         pml_x_size: PML Size for x-axis
         pml_y_size: PML Size for y-axis
         pml_z_size: PML Size for z-axis
-        """
+    """
 
     simulation_type: SimulationType = SimulationType.FLUID
-    cart_interp: str = 'linear'
+    cart_interp: str = "linear"
     pml_inside: bool = True
     pml_alpha: float = 2.0
     save_to_disk: bool = False
     save_to_disk_exit: bool = False
     scale_source_terms: bool = True
     smooth_c0: bool = False
     smooth_rho0: bool = False
@@ -97,75 +98,84 @@
     use_sg: bool = True
     use_fd: Optional[int] = None
     pml_auto: bool = False
     create_log: bool = False
     use_finite_difference: bool = False
     stream_to_disk: bool = False
     data_recast: Optional[bool] = False
-    cartesian_interp: str = 'linear'
+    cartesian_interp: str = "linear"
     hdf_compression_level: Optional[int] = None
-    data_cast: str = 'off'
+    data_cast: str = "off"
     pml_search_range: List[int] = field(default_factory=lambda: [10, 40])
-    radial_symmetry: str = 'WSWA-FFT'
+    radial_symmetry: str = "WSWA-FFT"
     multi_axial_PML_ratio: float = 0.1
     data_path: Optional[str] = field(default_factory=lambda: gettempdir())
     output_filename: Optional[str] = field(default_factory=lambda: f"{get_date_string()}_kwave_input.h5")
     input_filename: Optional[str] = field(default_factory=lambda: f"{get_date_string()}_kwave_output.h5")
     pml_x_alpha: Optional[float] = None
     pml_y_alpha: Optional[float] = None
     pml_z_alpha: Optional[float] = None
     pml_size: Optional[List[int]] = None
     pml_x_size: Optional[int] = None
     pml_y_size: Optional[int] = None
     pml_z_size: Optional[int] = None
 
     def __post_init__(self):
-        assert self.cartesian_interp in ['linear', 'nearest'], \
-            "Optional input ''cartesian_interp'' must be set to ''linear'' or ''nearest''."
+        assert self.cartesian_interp in [
+            "linear",
+            "nearest",
+        ], "Optional input ''cartesian_interp'' must be set to ''linear'' or ''nearest''."
 
         assert isinstance(self.data_cast, str), "Optional input ''data_cast'' must be a string."
 
-        assert self.data_cast in ['off', 'double', 'single'], \
-            "Invalid input for ''data_cast''."
+        assert self.data_cast in ["off", "double", "single"], "Invalid input for ''data_cast''."
 
-        if self.data_cast == 'double':
-            self.data_cast = 'off'
+        if self.data_cast == "double":
+            self.data_cast = "off"
 
         # load the HDF5 literals (for the default compression level)
         h5_literals = get_h5_literals()
         self.hdf_compression_level = h5_literals.HDF_COMPRESSION_LEVEL
         # check value is an integer between 0 and 9
-        assert isinstance(self.hdf_compression_level, int) and 0 <= self.hdf_compression_level <= 9, \
-            "Optional input ''hdf_compression_level'' must be an integer between 0 and 9."
-
-        assert np.isscalar(self.multi_axial_PML_ratio) and self.multi_axial_PML_ratio >= 0, \
-            "Optional input ''multi_axial_PML_ratio'' must be a single positive value."
-
-        assert np.isscalar(self.stream_to_disk) or isinstance(self.stream_to_disk, bool), \
-            "Optional input ''stream_to_disk'' must be a single scalar or Boolean value."
-
-        boolean_inputs = {"use_sg": self.use_sg,
-                          "data_recast": self.data_recast,
-                          "save_to_disk_exit": self.save_to_disk_exit,
-                          "use_kspace": self.use_kspace,
-                          "save_to_disk": self.save_to_disk,
-                          "pml_inside": self.pml_inside,
-                          "create_log": self.create_log,
-                          "scale_source_terms": self.scale_source_terms}
+        assert (
+            isinstance(self.hdf_compression_level, int) and 0 <= self.hdf_compression_level <= 9
+        ), "Optional input ''hdf_compression_level'' must be an integer between 0 and 9."
+
+        assert (
+            np.isscalar(self.multi_axial_PML_ratio) and self.multi_axial_PML_ratio >= 0
+        ), "Optional input ''multi_axial_PML_ratio'' must be a single positive value."
+
+        assert np.isscalar(self.stream_to_disk) or isinstance(
+            self.stream_to_disk, bool
+        ), "Optional input ''stream_to_disk'' must be a single scalar or Boolean value."
+
+        boolean_inputs = {
+            "use_sg": self.use_sg,
+            "data_recast": self.data_recast,
+            "save_to_disk_exit": self.save_to_disk_exit,
+            "use_kspace": self.use_kspace,
+            "save_to_disk": self.save_to_disk,
+            "pml_inside": self.pml_inside,
+            "create_log": self.create_log,
+            "scale_source_terms": self.scale_source_terms,
+        }
 
         for key, val in boolean_inputs.items():
             assert isinstance(val, bool), f"Optional input ''{key}'' must be Boolean."
 
-        assert self.radial_symmetry in ['WSWA', 'WSWS', 'WSWA-FFT', 'WSWS-FFT'], \
-            "Optional input ''RadialSymmetry'' must be set to ''WSWA'', ''WSWS'', ''WSWA-FFT'', ''WSWS-FFT''."
+        assert self.radial_symmetry in [
+            "WSWA",
+            "WSWS",
+            "WSWA-FFT",
+            "WSWS-FFT",
+        ], "Optional input ''RadialSymmetry'' must be set to ''WSWA'', ''WSWS'', ''WSWA-FFT'', ''WSWS-FFT''."
 
         # automatically assign the PML size to give small prime factors
         if self.pml_auto and self.pml_inside:
-            raise NotImplementedError(
-                "''pml_size'' set to ''auto'' is only supported with ''pml_inside'' set to false.")
+            raise NotImplementedError("''pml_size'' set to ''auto'' is only supported with ''pml_inside'' set to false.")
 
         if self.pml_size is not None:
             # TODO(walter): remove auto option in exchange for pml_auto=True
             if isinstance(self.pml_size, int):
                 self.pml_size = np.array([self.pml_size])
             if not isinstance(self.pml_size, (list, np.ndarray)):
                 raise ValueError("Optional input ''PMLSize'' must be a integer array of 1, 2 or 3 dimensions.")
@@ -175,16 +185,17 @@
         self.pml_y_alpha = self.pml_alpha if self.pml_y_alpha is None else self.pml_y_alpha
         self.pml_z_alpha = self.pml_alpha if self.pml_z_alpha is None else self.pml_z_alpha
 
         # add pathname to input and output filenames
         self.input_filename = os.path.join(self.data_path, self.input_filename)
         self.output_filename = os.path.join(self.data_path, self.output_filename)
 
-        assert self.use_fd is None or (np.issubdtype(self.use_fd, np.number) and self.use_fd in [2, 4]), \
-            "Optional input ''UseFD'' can only be set to 2, 4."
+        assert self.use_fd is None or (
+            np.issubdtype(self.use_fd, np.number) and self.use_fd in [2, 4]
+        ), "Optional input ''UseFD'' can only be set to 2, 4."
 
     @staticmethod
     def option_factory(kgrid: "kWaveGrid", options: SimulationOptions):
         """
         Initialize the Simulation Options
 
         Args:
@@ -244,40 +255,34 @@
         """
 
         STREAM_TO_DISK_STEPS_DEF = 200  # number of steps before streaming to disk
 
         if options.pml_size is not None and not isinstance(options.pml_size, bool):
             if len(options.pml_size) > kgrid.dim:
                 if kgrid.dim > 1:
-                    raise ValueError(
-                        f"Optional input ''pml_size'' must be a 1 or {kgrid.dim} element numerical array.")
+                    raise ValueError(f"Optional input ''pml_size'' must be a 1 or {kgrid.dim} element numerical array.")
                 else:
                     raise ValueError("Optional input ''pml_size'' must be a single numerical value.")
 
         if kgrid.dim == 1:
-            options.pml_x_alpha = 2
             options.pml_x_size = options.pml_size if options.pml_size else 20
             options.plot_scale = [-1.1, 1.1]
         elif kgrid.dim == 2:
-            options.pml_x_alpha = 2
-            options.pml_y_alpha = options.pml_x_alpha
-            if options.pml_size is None:
-                options.pml_x_size = 20
-                options.pml_y_size = 20
+            if options.pml_size is not None:
+                if len(options.pml_size) == kgrid.dim:
+                    options.pml_x_size, options.pml_y_size = np.asarray(options.pml_size, dtype=int).ravel()
+                else:
+                    options.pml_x_size, options.pml_y_size = (options.pml_size[0], options.pml_size[0])
             else:
-                options.pml_x_size = options.pml_size[0]
-                options.pml_y_size = options.pml_x_size
+                options.pml_x_size, options.pml_y_size = (20, 20)
             options.plot_scale = [-1, 1]
         elif kgrid.dim == 3:
-            if options.pml_size is not None and len(options.pml_size) == kgrid.dim:
-                options.pml_x_size, options.pml_y_size, options.pml_z_size = options.pml_size.ravel()
+            if (options.pml_size is not None) and (len(options.pml_size) == kgrid.dim):
+                options.pml_x_size, options.pml_y_size, options.pml_z_size = np.asarray(options.pml_size).ravel()
             else:
-                options.pml_x_alpha = 2
-                options.pml_y_alpha = options.pml_x_alpha
-                options.pml_z_alpha = options.pml_x_alpha
                 if options.pml_size is None:
                     options.pml_x_size = 10
                     options.pml_y_size = 10
                     options.pml_z_size = 10
                 else:
                     options.pml_x_size = options.pml_size[0]
                     options.pml_y_size = options.pml_x_size
@@ -286,16 +291,15 @@
 
         # replace defaults with user defined values if provided and check inputs
         if (val := options.pml_alpha) is not None and not isinstance(options.pml_alpha, str):
             # check input is correct size
             val = np.atleast_1d(val)
             if val.size > kgrid.dim:
                 if kgrid.dim > 1:
-                    raise ValueError(
-                        f"Optional input ''pml_alpha'' must be a 1 or {kgrid.dim} element numerical array.")
+                    raise ValueError(f"Optional input ''pml_alpha'' must be a 1 or {kgrid.dim} element numerical array.")
                 else:
                     raise ValueError("Optional input ''pml_alpha'' must be a single numerical value.")
 
             # assign input based on number of dimensions
             if kgrid.dim == 1:
                 options.pml_x_alpha = val
             elif kgrid.dim == 2:
@@ -306,27 +310,27 @@
                 options.pml_y_alpha = val[len(val) // 2]
                 options.pml_z_alpha = val[-1]
 
         if options.save_to_disk_exit:
             assert kgrid.dim != 1, "Optional input ''save_to_disk'' is not compatible with 1D simulations."
 
         if options.stream_to_disk:
-            assert not options.simulation_type.is_elastic_simulation() and kgrid.dim == 3, \
-                "Optional input ''stream_to_disk'' is currently only compatible with 3D fluid simulations."
+            assert (
+                not options.simulation_type.is_elastic_simulation() and kgrid.dim == 3
+            ), "Optional input ''stream_to_disk'' is currently only compatible with 3D fluid simulations."
             # if given as a Boolean, replace with the default number of time steps
             if isinstance(options.stream_to_disk, bool) and options.stream_to_disk:
                 options.stream_to_disk = STREAM_TO_DISK_STEPS_DEF
 
         if options.save_to_disk or options.save_to_disk_exit:
             assert kgrid.dim != 1, "Optional input ''save_to_disk'' is not compatible with 1D simulations."
 
         if options.use_fd:
             # input only supported in 1D fluid code
-            assert kgrid.dim == 1 and not options.simulation_type.is_elastic_simulation(), \
-                "Optional input ''use_fd'' only supported in 1D."
+            assert kgrid.dim == 1 and not options.simulation_type.is_elastic_simulation(), "Optional input ''use_fd'' only supported in 1D."
         # get optimal pml size
         if options.simulation_type.is_axisymmetric() or options.pml_auto:
             if options.simulation_type.is_axisymmetric():
                 pml_size_temp = get_optimal_pml_size(kgrid, options.pml_search_range, options.radial_symmetry[:4])
             else:
                 pml_size_temp = get_optimal_pml_size(kgrid, options.pml_search_range)
```

### Comparing `k_wave_python-0.3.2/kwave/reconstruction/beamform.py` & `k_wave_python-0.3.3/kwave/reconstruction/beamform.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
          sound_speed:       scalar sound speed
 
     Returns:
          input_signal_mat:  matrix of time series following the source points
     """
 
     assert not isinstance(kgrid.t_array, str), "kgrid.t_array must be a numeric array."
-    
+
     if isinstance(sound_speed, int):
         sound_speed = float(sound_speed)
 
     assert isinstance(sound_speed, float), "sound_speed must be a scalar."
 
     positions = [kgrid.x.flatten(), kgrid.y.flatten(), kgrid.z.flatten()]
 
@@ -57,53 +57,49 @@
 
     signal_mat = np.zeros((rel_delay.size, input_signal.size + max_delay))
 
     # for src_idx, delay in enumerate(rel_delay):
     #     signal_mat[src_idx, delay:max_delay - delay] = input_signal
     # signal_mat[rel_delay, delay:max_delay - delay] = input_signal
 
-    logging.log(logging.WARN, f'{PendingDeprecationWarning.__name__}: '
-                'This method is not fully migrated, might be depricated and is untested.')
+    logging.log(
+        logging.WARN, f"{PendingDeprecationWarning.__name__}: " "This method is not fully migrated, might be depricated and is untested."
+    )
 
     return signal_mat
 
 
 def scan_conversion(
-        scan_lines: np.ndarray,
-        steering_angles,
-        image_size: Tuple[float, float],
-        c0,
-        dt,
-        resolution: Optional[Tuple[int, int]]
+    scan_lines: np.ndarray, steering_angles, image_size: Tuple[float, float], c0, dt, resolution: Optional[Tuple[int, int]]
 ) -> np.ndarray:
     if resolution is None:
         resolution = (256, 256)  # in pixels
 
     x_resolution, y_resolution = resolution
 
     # assign the inputs
     x, y = image_size
 
     # start the timer
     TicToc.tic()
 
     # update command line status
-    logging.log(logging.INFO, 'Computing ultrasound scan conversion...')
+    logging.log(logging.INFO, "Computing ultrasound scan conversion...")
 
     # extract a_line parameters
     Nt = scan_lines.shape[1]
 
     # calculate radius variable based on the sound speed in the medium and the
     # round trip distance
     r = c0 * np.arange(1, Nt + 1) * dt / 2  # [m]
 
     # create regular Cartesian grid to remap to
     pos_vec_y_new = np.linspace(0, 1, y_resolution) * y - y / 2
     pos_vec_x_new = np.linspace(0, 1, x_resolution) * x
-    [pos_mat_x_new, pos_mat_y_new] = np.array(np.meshgrid(pos_vec_x_new, pos_vec_y_new, indexing='ij'))
+    [pos_mat_x_new, pos_mat_y_new] = np.array(np.meshgrid(pos_vec_x_new, pos_vec_y_new, indexing="ij"))
 
     # convert new points to polar coordinates
     [th_cart, r_cart] = cart2pol(pos_mat_x_new, pos_mat_y_new)
 
     # TODO: move this import statement at the top of the file
     # Not possible now due to cyclic dependencies
     from kwave.utils.interp import interpolate2d_with_queries
@@ -114,29 +110,23 @@
     # and reshape the values to the desired size
     # These three steps can be accomplished in one step in Matlab
     # However, we don't want to add custom logic to the `interpolate2D_with_queries` method.
 
     # Modifications -start
     queries = np.array([r_cart.flatten(), th_cart.flatten()]).T
 
-    b_mode = interpolate2d_with_queries(
-        [r, 2 * np.pi * steering_angles / 360],
-        scan_lines.T,
-        queries,
-        method='linear',
-        copy_nans=False
-    )
+    b_mode = interpolate2d_with_queries([r, 2 * np.pi * steering_angles / 360], scan_lines.T, queries, method="linear", copy_nans=False)
     image_size_points = (len(pos_vec_x_new), len(pos_vec_y_new))
     b_mode = b_mode.reshape(image_size_points)
     # Modifications -end
 
     b_mode[np.isnan(b_mode)] = 0
 
     # update command line status
-    logging.log(logging.INFO, f'  completed in {scale_time(TicToc.toc())}')
+    logging.log(logging.INFO, f"  completed in {scale_time(TicToc.toc())}")
 
     return b_mode
 
 
 def envelope_detection(signal):
     """
     envelopeDetection applies the Hilbert transform to extract the
```

### Comparing `k_wave_python-0.3.2/kwave/reconstruction/tools.py` & `k_wave_python-0.3.3/kwave/reconstruction/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 import numpy as np
 
 
 def log_compression(signal, cf, normalize=False):
     """
-    Log compress an input signal.
+     Log compress an input signal.
 
-    Args:
-        signal: signal to be log compressed
-        cf: compression factor
-        normalize (bool): when true, signal is normalized before compression
+     Args:
+         signal: signal to be log compressed
+         cf: compression factor
+         normalize (bool): when true, signal is normalized before compression
 
-   Returns: signal: log-compressed signal
+    Returns: signal: log-compressed signal
     """
     if normalize:
         ms = np.max(signal, axis=-1)
         if np.ndim(signal) == 2:
             ms = ms[:, np.newaxis]
         signal = ms * (np.log10(1 + cf * signal / ms) / np.log10(1 + cf))
     else:
         signal = np.log10(1 + cf * signal) / np.log10(1 + cf)
     return signal
 
+
 def db(x):
     return 20 * np.log10(np.abs(x))
 
+
 def apodize(distance, aperture, window):
     """
     Function that assigns different apodization to a set of pixels and elements
 
     """
 
-
-    if window == 'none':
+    if window == "none":
         apod = np.ones(np.size(distance))
-    elif window == 'boxcar':
+    elif window == "boxcar":
         apod = np.double(distance <= aperture / 2.0)
-    elif window == 'hanning':
+    elif window == "hanning":
         apod = np.double(distance <= aperture / 2) * (0.5 + 0.5 * np.cos(2 * np.pi * distance / aperture))
-    elif window == 'hamming':
+    elif window == "hamming":
         apod = np.double(distance <= aperture) / 2 * (0.53836 + 0.46164 * np.cos(2 * np.pi * distance / aperture))
-    elif window == 'tukey25':
+    elif window == "tukey25":
         roll = 0.25
-        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (
-                    distance < (aperture / 2)) * 0.5 * (1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2)))
-    elif window == 'tukey50':
+        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (distance < (aperture / 2)) * 0.5 * (
+            1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2))
+        )
+    elif window == "tukey50":
         roll = 0.5
-        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (
-                    distance < (aperture / 2)) * 0.5 * (1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2)))
-    elif window == 'tukey75':
+        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (distance < (aperture / 2)) * 0.5 * (
+            1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2))
+        )
+    elif window == "tukey75":
         roll = 0.75
-        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (
-                    distance < (aperture / 2)) * 0.5 * (1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2)))
+        apod = (distance < (aperture / 2 * (1 - roll))) + (distance > (aperture / 2 * (1 - roll))) * (distance < (aperture / 2)) * 0.5 * (
+            1 + np.cos(2 * np.pi / roll * (distance / aperture - roll / 2 - 1 / 2))
+        )
     else:
-        raise ValueError('Unknown window type. Known types are: boxcar, hamming, hanning, tukey25, tukey50, tukey75.')
+        raise ValueError("Unknown window type. Known types are: boxcar, hamming, hanning, tukey25, tukey50, tukey75.")
 
     return apod
 
 
 def make_time_vector(num_samples, sampling_freq, time_offset):
-    return np.linspace(start=0, num=num_samples,
-                       stop=num_samples / sampling_freq) + time_offset
+    return np.linspace(start=0, num=num_samples, stop=num_samples / sampling_freq) + time_offset
```

### Comparing `k_wave_python-0.3.2/kwave/utils/angular_spectrum.py` & `k_wave_python-0.3.3/kwave/utils/angular_spectrum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
 import time
 
 import numpy as np
 from matplotlib import pyplot as plt
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Dict, Union
-from nptyping import NDArray, Float, Shape
+from jaxtyping import Float
 
 from kwave.utils.conversion import db2neper
 from kwave.utils.data import scale_SI, scale_time
 from kwave.utils.filters import next_pow2
 from kwave.utils.matrix import expand_matrix
 from kwave.utils.tictoc import TicToc
 
 
-@beartype
+@typechecker
 def angular_spectrum(
-        input_plane: NDArray[Shape["Dim1, Dim2, Dim3"], Float], 
-        dx: float, 
-        dt: float, 
-        z_pos: float, 
-        medium: Union[Dict, int],
-        angular_restriction: bool=True,
-        grid_expansion: int=0,
-        fft_length: str='auto',
-        data_cast: str='off',
-        data_recast: bool=False,
-        reverse_proj: bool=False,
-        absorbing: bool=False,
-        plot_updates: bool=False,
-        loops_for_time_est: int=5,
-        record_time_series: bool=False
+    input_plane: Float[np.ndarray, "Dim1 Dim2 Dim3"],
+    dx: float,
+    dt: float,
+    z_pos: float,
+    medium: Union[Dict, int],
+    angular_restriction: bool = True,
+    grid_expansion: int = 0,
+    fft_length: str = "auto",
+    data_cast: str = "off",
+    data_recast: bool = False,
+    reverse_proj: bool = False,
+    absorbing: bool = False,
+    plot_updates: bool = False,
+    loops_for_time_est: int = 5,
+    record_time_series: bool = False,
 ):
     """
     Projects a 2D input plane (given as a 3D matrix of
     time series at each spatial position) using the angular spectrum
     method. The time series are decomposed into spectral components and
     then each frequency is propagated using the spectral propagator with
     angular restriction described in reference [1].
@@ -89,121 +89,119 @@
             spectrum approach for simulations of near-field pressures.
             The Journal of the Acoustical Society of America, 123(1), 68-76.
     """
     TicToc.tic()
     # check list of valid inputs
     if not isinstance(data_cast, str):
         raise ValueError("Optional input 'data_cast' must be a string.")
-    elif data_cast not in ['off', 'double', 'single', 'gpuArray-single', 'gpuArray-double']:
+    elif data_cast not in ["off", "double", "single", "gpuArray-single", "gpuArray-double"]:
         raise ValueError("Invalid input for 'data_cast'.")
 
     # replace double with off
-    if data_cast == 'double':
-        data_cast = 'off'
+    if data_cast == "double":
+        data_cast = "off"
 
     # create empty string to hold extra cast variable for use
     # with the parallel computing toolbox
-    data_cast_prepend = ''
+    data_cast_prepend = ""
 
     # replace PCT options with gpuArray
-    if data_cast == 'gpuArray-single':
-        data_cast = 'gpuArray'
-        data_cast_prepend = 'single'
-    elif data_cast == 'gpuArray-double':
-        data_cast = 'gpuArray'
+    if data_cast == "gpuArray-single":
+        data_cast = "gpuArray"
+        data_cast_prepend = "single"
+    elif data_cast == "gpuArray-double":
+        data_cast = "gpuArray"
 
-    if data_cast == 'gpuArray':
-        raise NotImplementedError('processing with GPU is not supported in the Python implementation of the kWave')
+    if data_cast == "gpuArray":
+        raise NotImplementedError("processing with GPU is not supported in the Python implementation of the kWave")
 
     # check for structured medium input
     if isinstance(medium, dict):
-
         # force the sound speed to be defined
-        if 'sound_speed' not in medium:
+        if "sound_speed" not in medium:
             raise ValueError("medium.sound_speed must be defined when specifying medium properties using a dictionary.")
 
         # assign the sound speed
-        c0 = medium['sound_speed']
+        c0 = medium["sound_speed"]
 
         # assign the absorption
-        if 'alpha_coeff' in medium or 'alpha_power' in medium:
-
+        if "alpha_coeff" in medium or "alpha_power" in medium:
             # enforce both absorption parameters
-            if 'alpha_coeff' not in medium or 'alpha_power' not in medium:
-                raise ValueError(
-                    "Both medium.alpha_coeff and medium.alpha_power must be defined for an absorbing medium.")
+            if "alpha_coeff" not in medium or "alpha_power" not in medium:
+                raise ValueError("Both medium.alpha_coeff and medium.alpha_power must be defined for an absorbing medium.")
 
             # assign flag
             absorbing = True
 
     else:
         # assign the sound speed
         c0 = medium
 
     # check time step is sufficient
     if (c0 * dt / dx) > 1:
         raise ValueError(
-            "Maximum supported frequency in temporal sampling is lower than maximum supported frequency in spatial sample (CFL > 1).")
+            "Maximum supported frequency in temporal sampling is lower than maximum supported frequency in spatial sample (CFL > 1)."
+        )
 
     # get grid size
     Nx, Ny, Nt = input_plane.shape
     z_pos = np.atleast_1d(z_pos)
     Nz = len(z_pos)
 
     # turn off plotting if only one value of z_pos
     if z_pos.size == 1:
         plot_updates = False
 
     # get scale factor for grid size
     scale, scale, prefix, _ = scale_SI(min(Nx * dx, Ny * dx))
 
     # update command line status
-    logging.log(logging.INFO, 'Running angular spectrum projection...')
+    logging.log(logging.INFO, "Running angular spectrum projection...")
     logging.log(logging.INFO, f"  start time: {TicToc.start_time}")
     logging.log(logging.INFO, f"  input plane size: {Nx} by {Ny} grid points ({scale * Nx * dx} by {scale * Ny * dx} {prefix}m)")
     logging.log(logging.INFO, f"  grid expansion: {grid_expansion} grid points")
 
     # reverse time signals if stepping backwards
     if reverse_proj:
         input_plane = np.flip(input_plane, 2)
 
     # expand input
     if grid_expansion > 0:
         input_plane = expand_matrix(input_plane, [grid_expansion, grid_expansion, 0], 0)
         Nx, Ny, Nt = input_plane.shape
 
     # get FFT size
-    if isinstance(fft_length, str) and fft_length == 'auto':
+    if isinstance(fft_length, str) and fft_length == "auto":
         fft_length = int(2 ** (next_pow2(max([Nx, Ny])) + 1))
 
     # update command line status
     logging.log(logging.INFO, f"  FFT size: {fft_length} points")
     logging.log(logging.INFO, f"  maximum supported frequency: {scale_SI(c0 / (2 * dx))}Hz")
     logging.log(logging.INFO, f"  input signal length: {Nt} time points ({scale_SI(Nt * dt)}s)")
 
     # create wavenumber vector
     N = fft_length
     if N % 2 == 0:
         k_vec = np.arange(-N // 2, N // 2) * 2 * np.pi / (N * dx)
     else:
-        k_vec = np.arange(-(N - 1) // 2, (N-1) // 2 + 1) * 2 * np.pi / (N * dx)
+        k_vec = np.arange(-(N - 1) // 2, (N - 1) // 2 + 1) * 2 * np.pi / (N * dx)
 
     # force middle value
     # force middle value to be zero in case 1/Nx is a recurring
     # number and the series doesn't give exactly zero
     k_vec[N // 2] = 0
 
     # shift wavenumbers to be in the correct order for FFTW
     k_vec = np.fft.ifftshift(k_vec)
 
     # create wavenumber grids
-    ky, kx = np.meshgrid(k_vec, k_vec, indexing='ij')
+    ky, kx = np.meshgrid(k_vec, k_vec, indexing="ij")
 
     # precompute term for angular restriction
-    sqrt_kx2_ky2 = np.sqrt(kx ** 2 + ky ** 2)
+    sqrt_kx2_ky2 = np.sqrt(kx**2 + ky**2)
 
     # preallocate maximum pressure output
     pressure_max = np.zeros((Nx, Ny, Nz))
 
     # preallocate time series output
     if record_time_series:
         pressure_time = np.zeros((Nx, Ny, Nt, Nz))
@@ -221,93 +219,87 @@
 
     # Compute frequencies to propagate
     f_vec_prop = f_vec[f_vec < (c0 / (2 * dx))]
 
     # Preallocate loop variable
     pressure_time_step = np.zeros((Nx, Ny, len(f_vec)), dtype=np.complex128)
 
-    if data_cast != 'off':
-        logging.log(logging.INFO, f'  casting variables to {data_cast} type...')
+    if data_cast != "off":
+        logging.log(logging.INFO, f"  casting variables to {data_cast} type...")
 
         # List of variables to cast
-        cast_variables = ['kx', 'ky', 'z_pos', 'input_plane_w_fft', 'pressure_max', 'pressure_time_step']
+        cast_variables = ["kx", "ky", "z_pos", "input_plane_w_fft", "pressure_max", "pressure_time_step"]
 
         # Additional variable if storing snapshots
         if record_time_series:
-            cast_variables.append('pressure_time')
+            cast_variables.append("pressure_time")
 
         # Additional variables used if absorbing
         if absorbing:
-            cast_variables.append('k')
+            cast_variables.append("k")
 
         # Additional variables used for angular restriction
         if angular_restriction:
-            cast_variables.extend(['sqrt_kx2_ky2', 'fft_length', 'dx'])
+            cast_variables.extend(["sqrt_kx2_ky2", "fft_length", "dx"])
 
         # Loop through, and change data type
         for var_name in cast_variables:
-            exec(f'{var_name} = {data_cast}({data_cast_prepend}({var_name}))')
+            exec(f"{var_name} = {data_cast}({data_cast_prepend}({var_name}))")
 
     # Open figure window
     if plot_updates:
         sim_fig = plt.figure()
         plt.show()
 
     # Update command line status
-    logging.log(logging.INFO, f'  precomputation completed in {scale_time(TicToc.toc())}')
-    logging.log(logging.INFO, '  starting z-step loop...')
+    logging.log(logging.INFO, f"  precomputation completed in {scale_time(TicToc.toc())}")
+    logging.log(logging.INFO, "  starting z-step loop...")
 
     # Loop over z-positions
     for z_index in range(Nz):
-
         # Get current z value
         z = z_pos[z_index]
 
         # If set to zero, just store the input plane
         if z == 0:
-
             # Store maximum pressure
             pressure_max[:, :, z_index] = np.max(input_plane, axis=2)
 
             # Store time series data if required
             if record_time_series:
                 pressure_time[:, :, :, z_index] = input_plane
 
         else:
-
             # Loop over frequencies
             for f_index in range(len(f_vec_prop)):
-
                 # Compute wavenumber at driving frequency
                 k = 2 * np.pi * f_vec[f_index] / c0
 
                 # Compute wavenumber grid
-                kz = np.sqrt(k ** 2 - ((kx ** 2) + (ky ** 2)).astype(complex))
+                kz = np.sqrt(k**2 - ((kx**2) + (ky**2)).astype(complex))
 
                 # Compute spectral propagator (Eq. 6)
                 H = np.conj(np.exp(1j * z * kz))
 
                 # Account for attenuation (Eq. 11)
                 if absorbing:
-
                     # Convert attenuation to Np/m
-                    alpha_Np = db2neper(medium.alpha_coeff, medium.alpha_power) * (
-                                2 * np.pi * f_vec[f_index]) ** medium.alpha_power
+                    alpha_Np = db2neper(medium.alpha_coeff, medium.alpha_power) * (2 * np.pi * f_vec[f_index]) ** medium.alpha_power
 
                     # Apply attenuation to propagator
                     if alpha_Np != 0:
                         H = H * np.exp(-alpha_Np * z * k / kz)
 
                 # Apply angular restriction
                 if angular_restriction:
                     # Size of computational domain [m]
                     D = (fft_length - 1) * dx
 
                     # Compute angular threshold (Eq. 10)
-                    kc = k * np.sqrt(0.5 * D ** 2 / (0.5 * D ** 2 + z ** 2))
+                    kc = k * np.sqrt(0.5 * D**2 / (0.5 * D**2 + z**2))
 
                     # Apply threshold to propagator
                     H[sqrt_kx2_ky2 > kc] = 0
 
                 # Compute forward Fourier transform of input plane
                 input_plane_xy_fft = np.fft.fft2(input_plane_w_fft[:, :, f_index], s=(fft_length, fft_length))
 
@@ -339,18 +331,18 @@
             # Store time series data if required
             if record_time_series:
                 pressure_time[:, :, :, z_index] = pressure_time_step_exp
 
             # Update command line status
             if z_index == loops_for_time_est:
                 est_sim_time = scale_time(TicToc.toc() * Nz / z_index)
-                logging.log(logging.INFO, f'  estimated simulation time {est_sim_time}  ...')
+                logging.log(logging.INFO, f"  estimated simulation time {est_sim_time}  ...")
 
     # update command line status
-    logging.log(logging.INFO, f'  simulation completed in {time.perf_counter() - TicToc.start_time}')
+    logging.log(logging.INFO, f"  simulation completed in {time.perf_counter() - TicToc.start_time}")
 
     # == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == =
     # POST PROCESSING
     # == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == =
 
     # Measure total computation time
     total_computation_time = TicToc.toc()
@@ -358,25 +350,25 @@
     # Close plot
     if plot_updates:
         plt.close(sim_fig)
 
     # Trim grid expansion
     if grid_expansion > 0:
         pressure_max = pressure_max[
-                       grid_expansion: -grid_expansion,
-                       grid_expansion: -grid_expansion,
-                       :,
-                       ]
+            grid_expansion:-grid_expansion,
+            grid_expansion:-grid_expansion,
+            :,
+        ]
         if record_time_series:
             pressure_time = pressure_time[
-                            grid_expansion: -grid_expansion,
-                            grid_expansion: -grid_expansion,
-                            :,
-                            :,
-                            ]
+                grid_expansion:-grid_expansion,
+                grid_expansion:-grid_expansion,
+                :,
+                :,
+            ]
 
     # Reverse time signals and grid if stepping backwards
     if reverse_proj:
         pressure_max = np.flip(pressure_max, axis=2)
         if record_time_series:
             pressure_time = np.flip(pressure_time, axis=2)
```

### Comparing `k_wave_python-0.3.2/kwave/utils/angular_spectrum_cw.py` & `k_wave_python-0.3.3/kwave/utils/angular_spectrum_cw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import logging
 import time
 
 import numpy as np
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Dict, Union
-from nptyping import NDArray, Float, Shape
+from jaxtyping import Float
 
 from kwave.utils.conversion import db2neper
 from kwave.utils.data import scale_SI, scale_time
 from kwave.utils.filters import next_pow2
 from kwave.utils.matrix import expand_matrix
 from kwave.utils.tictoc import TicToc
 
 
-@beartype
+@typechecker
 def angular_spectrum_cw(
-        input_plane: NDArray[Shape["Dim1, Dim2"], Float], 
-        dx: float, 
-        z_pos: float, 
-        f0: int, 
-        medium: Union[Dict, int],
-        angular_restriction: bool=True,
-        grid_expansion: int=0,
-        fft_length: str='auto',
-        data_cast: str='off',
-        data_recast: bool=False,
-        reverse_proj: bool=False,
-        absorbing: bool=False,
-        loops_for_time_est: int=5,
+    input_plane: Float[np.ndarray, "Dim1 Dim2"],
+    dx: float,
+    z_pos: float,
+    f0: int,
+    medium: Union[Dict, int],
+    angular_restriction: bool = True,
+    grid_expansion: int = 0,
+    fft_length: str = "auto",
+    data_cast: str = "off",
+    data_recast: bool = False,
+    reverse_proj: bool = False,
+    absorbing: bool = False,
+    loops_for_time_est: int = 5,
 ):
     """
     Projects a 2D input plane (given as a 3D matrix of
     time series at each spatial position) using the angular spectrum
     method. The time series are decomposed into spectral components and
     then each frequency is propagated using the spectral propagator with
     angular restriction described in reference [1].
@@ -76,64 +76,57 @@
             spectrum approach for simulations of near-field pressures.
             The Journal of the Acoustical Society of America, 123(1), 68-76.
     """
     TicToc.tic()
     # check list of valid inputs
     if not isinstance(data_cast, str):
         raise ValueError("Optional input 'data_cast' must be a string.")
-    elif data_cast not in ['off', 'double', 'single', 'gpuArray-single', 'gpuArray-double']:
+    elif data_cast not in ["off", "double", "single", "gpuArray-single", "gpuArray-double"]:
         raise ValueError("Invalid input for 'data_cast'.")
 
     # replace double with off
-    if data_cast == 'double':
-        data_cast = 'off'
+    if data_cast == "double":
+        data_cast = "off"
 
     # create empty string to hold extra cast variable for use
     # with the parallel computing toolbox
-    data_cast_prepend = ''
+    data_cast_prepend = ""
 
     # replace PCT options with gpuArray
-    if data_cast == 'gpuArray-single':
-        data_cast = 'gpuArray'
-        data_cast_prepend = 'single'
-    elif data_cast == 'gpuArray-double':
-        data_cast = 'gpuArray'
+    if data_cast == "gpuArray-single":
+        data_cast = "gpuArray"
+        data_cast_prepend = "single"
+    elif data_cast == "gpuArray-double":
+        data_cast = "gpuArray"
 
-    if data_cast == 'gpuArray':
-        raise NotImplementedError('processing with GPU is not supported in the Python implementation of the kWave')
+    if data_cast == "gpuArray":
+        raise NotImplementedError("processing with GPU is not supported in the Python implementation of the kWave")
 
     # check for structured medium input
     if isinstance(medium, dict):
-
         # force the sound speed to be defined
-        if 'sound_speed' not in medium:
+        if "sound_speed" not in medium:
             raise ValueError("medium.sound_speed must be defined when specifying medium properties using a dictionary.")
 
         # assign the sound speed
-        c0 = medium['sound_speed']
+        c0 = medium["sound_speed"]
 
         # assign the absorption
-        if 'alpha_coeff' in medium or 'alpha_power' in medium:
-
+        if "alpha_coeff" in medium or "alpha_power" in medium:
             # enforce both absorption parameters
-            if 'alpha_coeff' not in medium or 'alpha_power' not in medium:
-                raise ValueError(
-                    "Both medium.alpha_coeff and medium.alpha_power must be defined for an absorbing medium.")
+            if "alpha_coeff" not in medium or "alpha_power" not in medium:
+                raise ValueError("Both medium.alpha_coeff and medium.alpha_power must be defined for an absorbing medium.")
 
             # convert attenuation to Np/m
-            alpha_Np = db2neper(
-                alpha=medium['alpha_coeff'],
-                y=medium['alpha_power']
-            ) * (2 * np.pi * f0) ** medium['alpha_power']
+            alpha_Np = db2neper(alpha=medium["alpha_coeff"], y=medium["alpha_power"]) * (2 * np.pi * f0) ** medium["alpha_power"]
 
             # check for zero absorption and assign flag
             if alpha_Np != 0:
                 absorbing = True
     else:
-
         # assign the sound speed
         c0 = medium
 
     # check for maximum supported frequency
     if dx > (c0 / (2 * f0)):
         raise ValueError(f"Input frequency is higher than maximum supported frequency of {scale_SI(c0 / (2 * dx))}Hz.")
 
@@ -142,156 +135,153 @@
     z_pos = np.atleast_1d(z_pos)
     Nz = len(z_pos)
 
     # get scale factor for grid size
     _, scale, prefix, _ = scale_SI(min(Nx * dx, Ny * dx))
 
     # update command line status
-    logging.log(logging.INFO, 'Running CW angular spectrum projection...')
+    logging.log(logging.INFO, "Running CW angular spectrum projection...")
     logging.log(logging.INFO, f"  start time: {TicToc.start_time}")
     logging.log(logging.INFO, f"  input plane size: {Nx} by {Ny} grid points ({scale * Nx * dx} by {scale * Ny * dx} {prefix}m)")
     logging.log(logging.INFO, f"  grid expansion: {grid_expansion} grid points")
 
     # apply phase conjugation if stepping backwards
     if reverse_proj:
         input_plane = np.conj(input_plane)
 
     # expand input
     if grid_expansion > 0:
         input_plane = expand_matrix(input_plane, [grid_expansion, grid_expansion], 0)
         Nx, Ny = input_plane.shape
 
     # get FFT size
-    if isinstance(fft_length, str) and fft_length == 'auto':
+    if isinstance(fft_length, str) and fft_length == "auto":
         fft_length = int(2 ** (next_pow2(max([Nx, Ny])) + 1))
 
     # update command line status
     logging.log(logging.INFO, f"  FFT size: {fft_length} points")
     logging.log(logging.INFO, f"  maximum supported frequency: {scale_SI(c0 / (2 * dx))}Hz")
 
     # create wavenumber vector
     N = fft_length
     if N % 2 == 0:
         k_vec = np.arange(-N // 2, N // 2) * 2 * np.pi / (N * dx)
     else:
-        k_vec = np.arange(-(N - 1) // 2, (N-1) // 2 + 1) * 2 * np.pi / (N * dx)
+        k_vec = np.arange(-(N - 1) // 2, (N - 1) // 2 + 1) * 2 * np.pi / (N * dx)
 
     # force middle value
     # force middle value to be zero in case 1/Nx is a recurring
     # number and the series doesn't give exactly zero
     k_vec[N // 2] = 0
 
     # shift wavenumbers to be in the correct order for FFTW
     k_vec = np.fft.ifftshift(k_vec)
 
     # compute wavenumber at driving frequency
     k = 2 * np.pi * f0 / c0
 
     # create wavenumber grids
-    ky, kx = np.meshgrid(k_vec, k_vec, indexing='ij')
+    ky, kx = np.meshgrid(k_vec, k_vec, indexing="ij")
     kz = np.sqrt(k**2 - (kx**2 + ky**2).astype(complex))
 
     # precompute term for angular restriction
-    sqrt_kx2_ky2 = np.sqrt(kx ** 2 + ky ** 2)
+    sqrt_kx2_ky2 = np.sqrt(kx**2 + ky**2)
 
     # preallocate maximum pressure output
     pressure = np.zeros((Nx, Ny, Nz), dtype=np.complex128)
     pressure[:, :, 0] = input_plane
 
     # compute forward Fourier transform of input plane
     input_plane_fft = np.fft.fft2(input_plane, (fft_length, fft_length))
 
     # =========================================================================
     # DATA CASTING
     # =========================================================================
 
-    if data_cast != 'off':
-        logging.log(logging.INFO, f'  casting variables to {data_cast} type...')
+    if data_cast != "off":
+        logging.log(logging.INFO, f"  casting variables to {data_cast} type...")
 
         # List of variables to cast
-        cast_variables = ['kz', 'z_pos', 'input_plane_fft', 'pressure']
+        cast_variables = ["kz", "z_pos", "input_plane_fft", "pressure"]
 
         # Additional variables used if absorbing
         if absorbing:
-            cast_variables.extend(['alpha_Np', 'k'])
+            cast_variables.extend(["alpha_Np", "k"])
 
         # Additional variables used for angular restriction
         if angular_restriction:
-            cast_variables.extend(['sqrt_kx2_ky2', 'fft_length', 'dx'])
+            cast_variables.extend(["sqrt_kx2_ky2", "fft_length", "dx"])
 
         # Loop through, and change data type
         for var_name in cast_variables:
-            exec(f'{var_name} = {data_cast}({data_cast_prepend}({var_name}))')
+            exec(f"{var_name} = {data_cast}({data_cast_prepend}({var_name}))")
 
     # =========================================================================
     # Z-LOOP
     # =========================================================================
 
     # Update command line status
-    logging.log(logging.INFO, f'  precomputation completed in {scale_time(TicToc.toc())}')
-    logging.log(logging.INFO, '  starting z-step loop...')
+    logging.log(logging.INFO, f"  precomputation completed in {scale_time(TicToc.toc())}")
+    logging.log(logging.INFO, "  starting z-step loop...")
 
     # Loop over z-positions
     for z_index in range(Nz):
-
         # Get current z value
         z = z_pos[z_index]
 
         # If set to zero, just store the input plane
         if z == 0:
-
             # Store input data
             pressure[:, :, z_index] = input_plane
 
         else:
-
             # compute spectral propagator (Eq. 6)
             H = np.conj(np.exp(1j * z * kz))
 
             # account for attenuation (Eq. 11)
             if absorbing:
                 H = H * np.exp(-alpha_Np * z * k / kz)
 
             # apply angular restriction
             if angular_restriction:
                 # size of computational domain [m]
                 D = (fft_length - 1) * dx
 
                 # compute angular threshold (Eq. 10)
-                kc = k * np.sqrt(0.5 * D ** 2 / (0.5 * D ** 2 + z ** 2))
+                kc = k * np.sqrt(0.5 * D**2 / (0.5 * D**2 + z**2))
 
                 # apply threshold to propagator
                 H[sqrt_kx2_ky2 > kc] = 0
 
             # compute projected field and store
             pressure_step = np.fft.ifft2(input_plane_fft * H, (fft_length, fft_length))
             pressure[:, :, z_index] = pressure_step[:Nx, :Ny]
 
         # Update command line status
         if z_index == loops_for_time_est:
             est_sim_time = scale_time(TicToc.toc() * Nz / z_index)
-            logging.log(logging.INFO, f'  estimated simulation time {est_sim_time}  ...')
+            logging.log(logging.INFO, f"  estimated simulation time {est_sim_time}  ...")
 
     # update command line status
-    logging.log(logging.INFO, f'  simulation completed in {time.perf_counter() - TicToc.start_time}')
+    logging.log(logging.INFO, f"  simulation completed in {time.perf_counter() - TicToc.start_time}")
 
     # == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == =
     # POST PROCESSING
     # == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == == =
 
     # Measure total computation time
     total_computation_time = TicToc.toc()
 
     # Trim grid expansion
     if grid_expansion > 0:
         pressure = pressure[
-                       grid_expansion: -grid_expansion,
-                       grid_expansion: -grid_expansion,
-                       :,
-                       ]
+            grid_expansion:-grid_expansion,
+            grid_expansion:-grid_expansion,
+            :,
+        ]
 
     # Reverse time signals and grid if stepping backwards
     if reverse_proj:
         np.flip(np.conj(pressure), axis=2)
 
     # Cast output back to double precision
     if data_recast:
```

### Comparing `k_wave_python-0.3.2/kwave/utils/atten_comp.py` & `k_wave_python-0.3.3/kwave/utils/atten_comp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 import logging
 import numpy as np
 from matplotlib import pyplot as plt
-from beartype import beartype
-from nptyping import NDArray, Float, Shape
+from beartype import beartype as typechecker
+from jaxtyping import Float
 
 from kwave.utils.conversion import db2neper
 from kwave.utils.math import find_closest
 
 
 # =========================================================================
 # FITTING FUNCTION
 # =========================================================================
 
-@beartype
-def constlinfit(x: float, y: float, a: float, b: float, neg_penalty: float=10):
+
+@typechecker
+def constlinfit(x: float, y: float, a: float, b: float, neg_penalty: float = 10):
     error = a * x + b - y
     error[error < 0] = error[error < 0] * neg_penalty
     return sum(abs(error))
 
 
-@beartype
+@typechecker
 def atten_comp(
-        signal: NDArray[Shape["SensorIndex, TimeIndex"], Float], 
-        dt: float, 
-        c: int, 
-        alpha_0: float, 
-        y: float,
-        display_updates: bool=False,
-        distribution: str='Rihaczek',
-        energy_cutoff: float=0.98,
-        freq_multiplier: float=2,
-        filter_cutoff: str='auto',
-        fit_type: str='spline',
-        noise_cutoff: float=0.03,
-        num_splines: int=40,
-        plot_tfd: bool=False,
-        plot_range: str='auto',
-        t0: int=1,
-        taper_ratio: float=0.5,
+    signal: Float[np.ndarray, "SensorIndex TimeIndex"],
+    dt: float,
+    c: int,
+    alpha_0: float,
+    y: float,
+    display_updates: bool = False,
+    distribution: str = "Rihaczek",
+    energy_cutoff: float = 0.98,
+    freq_multiplier: float = 2,
+    filter_cutoff: str = "auto",
+    fit_type: str = "spline",
+    noise_cutoff: float = 0.03,
+    num_splines: int = 40,
+    plot_tfd: bool = False,
+    plot_range: str = "auto",
+    t0: int = 1,
+    taper_ratio: float = 0.5,
 ):
     """
 
-    Args:
-        signal: time series to compensate, indexed as (sensor_index, time_index)
-        dt: time step [s]
-        c: sound speed [m/s]
-        alpha_0: power law absorption prefactor [dB/(MHz^y cm)]
-        y: power law absorption exponent [0 < y < 3, y != 1]
-        display_updates: Boolean controlling whether command line updates
-%       and compute time are printed to the command line
-        distribution: default TF distribution
-        energy_cutoff: cutoff frequency as a [%] of total energy
-        freq_multiplier: used to increase the cutoff_f for a smoother filter
-        filter_cutoff: automatically compute cutoff based on TFD
-        fit_type: default fit type used for smooth distribution
-        noise_cutoff: [%] of signal max, used to threshold the signals
-        num_splines: used for fit_type = 'spline'
-        plot_tfd: plot TFD and cutoff
-        plot_range: plot range
-        t0: index of laser pulse
-        taper_ratio: taper ratio used for Tukey Window
+        Args:
+            signal: time series to compensate, indexed as (sensor_index, time_index)
+            dt: time step [s]
+            c: sound speed [m/s]
+            alpha_0: power law absorption prefactor [dB/(MHz^y cm)]
+            y: power law absorption exponent [0 < y < 3, y != 1]
+            display_updates: Boolean controlling whether command line updates
+    %       and compute time are printed to the command line
+            distribution: default TF distribution
+            energy_cutoff: cutoff frequency as a [%] of total energy
+            freq_multiplier: used to increase the cutoff_f for a smoother filter
+            filter_cutoff: automatically compute cutoff based on TFD
+            fit_type: default fit type used for smooth distribution
+            noise_cutoff: [%] of signal max, used to threshold the signals
+            num_splines: used for fit_type = 'spline'
+            plot_tfd: plot TFD and cutoff
+            plot_range: plot range
+            t0: index of laser pulse
+            taper_ratio: taper ratio used for Tukey Window
 
-    Returns:
+        Returns:
 
     """
     # dynamic range used in TFD plot [dB]
     # multiplier used to scale the auto-plot range
     PLOT_RANGE_MULT = 1.5
 
     # rotate input signal from (sensor_index, time_index) to (time_index,
@@ -79,77 +80,68 @@
         raise ValueError("A power exponent [y] of 1 is not valid.")
 
     # convert absorption coefficient to nepers
     alpha_0 = db2neper(alpha_0, y)
 
     # update command line status
     if display_updates:
-        logging.log(logging.INFO, 'Applying time variant filter...')
+        logging.log(logging.INFO, "Applying time variant filter...")
 
     # check FitType input
-    if fit_type == 'mav':
-
+    if fit_type == "mav":
         # define settings for moving average based on the
         # length of the input signals
         mav_terms = int(round(N * 1e-2))
         mav_terms = mav_terms + (mav_terms % 2)
 
-    elif fit_type not in ['linear', 'spline']:
-
+    elif fit_type not in ["linear", "spline"]:
         # throw error for unknown input
-        raise ValueError('Optional input ''FitType'' must be set to ''spline'', ''mav'', or ''linear''.')
+        raise ValueError("Optional input " "FitType" " must be set to " "spline" ", " "mav" ", or " "linear" ".")
 
     # =========================================================================
     # COMPUTE AVERAGE TIME FREQUENCY DISTRIBUTION (TFD) OF INPUT
     # =========================================================================
 
     # sample frequency
     Fs = 1 / dt
 
     # create time and frequency axes
     t_array = dt * np.arange(N)
 
     # compute the double-sided frequency axis
-    if N %  2 == 0:
-
+    if N % 2 == 0:
         # N is even
-        f_array = np.arange(-N/2, N/2) * Fs / N
+        f_array = np.arange(-N / 2, N / 2) * Fs / N
 
     else:
-
         # N is odd
         f_array = np.arange(-(N - 1) / 2, (N - 1) / 2) * Fs / N
 
     # compute the TFD if required
-    if filter_cutoff == 'auto' or plot_tfd:
-
+    if filter_cutoff == "auto" or plot_tfd:
         # update display
         if display_updates:
             if num_signals > 1:
-                logging.log(logging.INFO, '  calculating average time-frequency spectrum...')
+                logging.log(logging.INFO, "  calculating average time-frequency spectrum...")
             else:
-                logging.log(logging.INFO, '  calculating time-frequency spectrum...')
+                logging.log(logging.INFO, "  calculating time-frequency spectrum...")
 
         # compute the TFD of the input signal
 
-        if distribution == 'Rihaczek':
+        if distribution == "Rihaczek":
             tfd = np.outer(np.conj(np.fft.fft(signal[:, 0])), signal[:, 0])
             if num_signals > 1:
                 for index in range(1, num_signals):
                     tfd += np.outer(np.conj(np.fft.fft(signal[:, index])), signal[:, index])
             inc = 2 * np.pi / N
-            tfd *= np.exp(
-                np.outer(
-                    -1j * np.arange(0, 2 * np.pi * (1 - 1 / N) + inc, inc),
-                    np.arange(N)
-                )
-            )
+            tfd *= np.exp(np.outer(-1j * np.arange(0, 2 * np.pi * (1 - 1 / N) + inc, inc), np.arange(N)))
             tfd = np.fft.fftshift(tfd, 0) / (N * num_signals)
-        elif distribution == 'Wigner':
-            def qwigner2(x: NDArray[Shape["Dim1"], Float], Fs: float):
+        elif distribution == "Wigner":
+
+            def qwigner2(x: Float[np.ndarray, "Dim1"], Fs: float):
                 raise NotImplementedError
 
             tfd = qwigner2(signal[:, 0], Fs)
             if num_signals > 1:
                 for index in range(1, num_signals):
                     tfd += qwigner2(signal[:, index], Fs)
             tfd /= num_signals
@@ -162,19 +154,19 @@
     if plot_tfd:
         raise NotImplementedError
 
     # =========================================================================
     # FIND CUTOFF FREQUENCIES
     # =========================================================================
 
-    @beartype
-    def findClosest(arr: NDArray[Shape["Dim1"], Float], value: float):
+    @typechecker
+    def findClosest(arr: Float[np.ndarray, "Dim1"], value: float):
         return (np.abs(arr - value)).argmin()
 
-    if filter_cutoff == 'auto':  # noqa: F821
+    if filter_cutoff == "auto":  # noqa: F821
         # update display
         if display_updates:
             logging.log(logging.INFO, "finding filter thresholds... ")
 
         f_array_hs = f_array[f_array >= 0]
         tfd_hs = 2 * tfd[f_array >= 0, :]
 
@@ -191,37 +183,37 @@
             assert len(closes_idx) == 1
             cutoff_index[tw_index] = closes_idx[0]
 
         cutoff_freq_array = f_array_hs[cutoff_index] * freq_multiplier
 
         if plot_tfd:
             plt.hold(True)
-            plt.plot((np.arange(N) * dt * 1e6, cutoff_freq_array * 1e-6, 'y-'))
-            plt.plot((np.arange(N) * dt * 1e6, -cutoff_freq_array * 1e-6, 'y-'))
+            plt.plot((np.arange(N) * dt * 1e6, cutoff_freq_array * 1e-6, "y-"))
+            plt.plot((np.arange(N) * dt * 1e6, -cutoff_freq_array * 1e-6, "y-"))
             plt.draw()
 
-        if fit_type == 'linear':
+        if fit_type == "linear":
             neg_penalty = 10
             x0 = np.array([-f_array_hs[-1] / N, f_array_hs[int(len(f_array_hs) / 2)]])
             opt_vals = opt.fmin(constlinfit, x0, args=(1, N, cutoff_freq_array, neg_penalty))  # noqa: F821
             x = np.array(list(range(1, N + 1)))
             cutoff_freq_array = opt_vals[0] * x + opt_vals[1]
 
-        elif fit_type == 'spline':
-            pp = splinefit(list(range(1, N + 1)), cutoff_freq_array, num_splines, 'r')  # noqa: F821
+        elif fit_type == "spline":
+            pp = splinefit(list(range(1, N + 1)), cutoff_freq_array, num_splines, "r")  # noqa: F821
             cutoff_freq_array = ppval(pp, list(range(1, N + 1)))  # noqa: F821
 
-        elif fit_type == 'mav':
-            cutoff_freq_array = np.convolve(cutoff_freq_array, np.ones(mav_terms) / mav_terms, mode='same')
+        elif fit_type == "mav":
+            cutoff_freq_array = np.convolve(cutoff_freq_array, np.ones(mav_terms) / mav_terms, mode="same")
             cutoff_freq_array = np.roll(cutoff_freq_array, int(-(mav_terms // 2)))
 
-        elif fit_type == 'off':
+        elif fit_type == "off":
             pass
         else:
-            raise ValueError('unknown fit_type setting')
+            raise ValueError("unknown fit_type setting")
 
     else:
         assert not isinstance(filter_cutoff, str)
         # set manual values
         cutoff_freq_array = (filter_cutoff[1] - filter_cutoff[0]) / (N - 1) * np.arange(1, N + 1) + filter_cutoff[0]
 
     # Constrain values outside frequency range
@@ -229,21 +221,21 @@
 
     # Constrain negative values
     cutoff_freq_array = np.maximum(cutoff_freq_array, 0)
 
     # Plot final threshold
     if plot_tfd:
         # Plot
-        plt.plot(t_array * 1e6, cutoff_freq_array * 1e-6, 'w--', label='cutoff_frequency')
-        plt.plot(t_array * 1e6, -cutoff_freq_array * 1e-6, 'w--', label='cutoff_frequency')
+        plt.plot(t_array * 1e6, cutoff_freq_array * 1e-6, "w--", label="cutoff_frequency")
+        plt.plot(t_array * 1e6, -cutoff_freq_array * 1e-6, "w--", label="cutoff_frequency")
 
         # Set the plot range
         if isinstance(plot_range, (int, float)):
             plt.ylim(plot_range)
-        elif plot_range == 'auto' and (PLOT_RANGE_MULT * np.amax(cutoff_freq_array) < f_array[-1]):
+        elif plot_range == "auto" and (PLOT_RANGE_MULT * np.amax(cutoff_freq_array) < f_array[-1]):
             plt.ylim(PLOT_RANGE_MULT * np.amax(cutoff_freq_array) * [-1, 1] * 1e-6)
         plt.show()
 
     # =========================================================================
     # CREATE FILTER
     # =========================================================================
 
@@ -254,44 +246,43 @@
     # relative to the start of the signals
     dist_vec = c * dt * (np.arange(N) - t0)
     dist_vec[dist_vec < 0] = 0
 
     # Check if f_array and dist_vec are valid
     assert f_array is not None and len(f_array) > 0, "f_array must have non-zero length."
     assert dist_vec is not None and len(dist_vec) > 0, "dist_vec must have non-zero length."
-    
+
     # Create the time variant filter
     f_mat, dist_mat = np.meshgrid(f_array, dist_vec)
 
-    assert y != 1, "A power exponent [y] of 1 is not valid." # this is a duplicate assertion to attempt to remove a warning
+    assert y != 1, "A power exponent [y] of 1 is not valid."  # this is a duplicate assertion to attempt to remove a warning
 
     # Add conditionals or use np.where to manage zero and NaN
     part_1 = (2 * np.pi * np.abs(f_mat)) ** y
     part_2 = 1j * np.tan(np.pi * y / 2)
-    part_3 = (2 * np.pi * f_mat)
+    part_3 = 2 * np.pi * f_mat
     part_4 = (2 * np.pi * np.abs(f_mat)) ** (y - 1)
-    
+
     tv_filter = alpha_0 * dist_mat * (part_1 - part_2 * part_3 * part_4)
 
     # convert cutoff frequency to a window size
     N_win_array = np.floor((cutoff_freq_array / f_array[-1]) * N) - 1
     N_win_array[np.fmod(N_win_array, 2) == 1] = N_win_array[np.fmod(N_win_array, 2) == 1] + 1
 
     # loop through each time/distance and create a row of the filter
     for t_index in range(N):
-
         # get the filter cutoff freq
         cutoff_freq = cutoff_freq_array[t_index]
         N_win = int(N_win_array[t_index])
 
         if cutoff_freq != 0:
             # create window
             win = np.zeros(N)
             win_pos = int(np.ceil((N - N_win) / 2)) + 1
-            win[win_pos: win_pos + N_win] = np.tukey(N_win, taper_ratio)
+            win[win_pos : win_pos + N_win] = np.tukey(N_win, taper_ratio)
 
             # window row of tv_filter
             tv_filter[t_index, :] *= win
         else:
             tv_filter[t_index, :] = 0
 
     # take exponential
```

### Comparing `k_wave_python-0.3.2/kwave/utils/checks.py` & `k_wave_python-0.3.3/kwave/utils/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     Raises:
         AssertionError: If any of the specified fields are not in the dictionary.
 
     """
 
     for f in fields:
-        assert f in dictionary.keys(), [f'The field {f} must be defined in the given dictionary']
+        assert f in dictionary.keys(), [f"The field {f} must be defined in the given dictionary"]
 
 
 def enforce_fields_obj(obj, *fields):
     """
     Enforces that certain fields are not None in the given object.
 
     Args:
@@ -41,15 +41,15 @@
 
     Raises:
         AssertionError: If any of the given fields are None in the given object.
 
     """
 
     for f in fields:
-        assert getattr(obj, f) is not None, f'The field {f} must be not None in the given object'
+        assert getattr(obj, f) is not None, f"The field {f} must be not None in the given object"
 
 
 def check_field_names(dictionary, *fields):
     """
     This method checks if the keys of the given dictionary are valid fields.
 
     Args:
@@ -58,15 +58,15 @@
 
     Raises:
         AssertionError: If any of the keys in the dictionary are not in the list of valid fields.
 
     """
 
     for k in dictionary.keys():
-        assert k in fields, f'The field {k} is not a valid field for the given dictionary'
+        assert k in fields, f"The field {k} is not a valid field for the given dictionary"
 
 
 def check_str_eq(value, target: str) -> bool:
     """
     This method checks whether the given value is a string and is equal to the target string.
     It is useful to avoid FutureWarnings when value is not a string.
 
@@ -127,15 +127,15 @@
     """
     Check whether the current platform is a Unix-like system.
 
     Returns:
         True if the current platform is a Unix-like system, False otherwise.
 
     """
-    return platform.system() in ['Linux', 'Darwin']
+    return platform.system() in ["Linux", "Darwin"]
 
 
 def check_stability(kgrid: "kWaveGrid", medium: "kWaveMedium") -> float:
     """
     Calculates the maximum time step for which the k-space
     propagation models are stable.
 
@@ -170,93 +170,85 @@
     FIXED_POINT_ACCURACY = 1e-12
 
     # find the maximum wavenumber
     kmax = kgrid.k.max()
 
     # calculate the reference sound speed for the fluid code, using the
     # maximum by default which ensures the model is unconditionally stable
-    reductions = {
-        'min': np.min,
-        'max': np.max,
-        'mean': np.mean
-    }
+    reductions = {"min": np.min, "max": np.max, "mean": np.mean}
 
     if medium.sound_speed_ref is not None:
         ss_ref = medium.sound_speed_ref
         if np.isscalar(ss_ref):
             c_ref = ss_ref
         else:
             try:
                 c_ref = reductions[ss_ref](medium.sound_speed)
             except KeyError:
-                raise NotImplementedError('Unknown input for medium.sound_speed_ref.')
+                raise NotImplementedError("Unknown input for medium.sound_speed_ref.")
     else:
-        c_ref = reductions['max'](medium.sound_speed)
+        c_ref = reductions["max"](medium.sound_speed)
 
     # calculate the timesteps required for stability
     if medium.alpha_coeff is None or np.all(medium.alpha_coeff == 0):
-
         # =====================================================================
         # NON-ABSORBING CASE
         # =====================================================================
 
         medium.sound_speed = np.atleast_1d(medium.sound_speed)
         if c_ref >= medium.sound_speed.max():
             # set the timestep to Inf when the model is unconditionally stable
-            dt_stability_limit = float('inf')
+            dt_stability_limit = float("inf")
 
         else:
             # set the timestep required for stability when c_ref~=max(medium.sound_speed(:))
             dt_stability_limit = 2 / (c_ref * kmax) * np.asin(c_ref / medium.sound_speed.max())
 
     else:
-
         # =====================================================================
         # ABSORBING CASE
         # =====================================================================
 
         # convert the absorption coefficient to nepers.(rad/s)^-y.m^-1
         medium.alpha_coeff = db2neper(medium.alpha_coeff, medium.alpha_power)
 
         # calculate the absorption constant
-        if medium.alpha_mode == 'no_absorption':
+        if medium.alpha_mode == "no_absorption":
             absorb_tau = -2 * medium.alpha_coeff * medium.sound_speed ** (medium.alpha_power - 1)
         else:
             absorb_tau = np.array([0])
 
         # calculate the dispersion constant
-        if medium.alpha_mode == 'no_dispersion':
-            absorb_eta = 2 * medium.alpha_coeff * medium.sound_speed ** medium.alpha_power * np.tan(
-                np.pi * medium.alpha_power / 2)
+        if medium.alpha_mode == "no_dispersion":
+            absorb_eta = 2 * medium.alpha_coeff * medium.sound_speed**medium.alpha_power * np.tan(np.pi * medium.alpha_power / 2)
         else:
             absorb_eta = np.array([0])
 
         # estimate the timestep required for stability in the absorbing case by
         # assuming the k-space correction factor, kappa = 1 (note that
         # absorb_tau and absorb_eta are negative quantities)
         medium.sound_speed = np.atleast_1d(medium.sound_speed)
 
         temp1 = medium.sound_speed.max() * absorb_tau.min() * kmax ** (medium.alpha_power - 1)
         temp2 = 1 - absorb_eta.min() * kmax ** (medium.alpha_power - 1)
-        dt_estimate = (temp1 + np.sqrt(temp1 ** 2 + 4 * temp2)) / (temp2 * kmax * medium.sound_speed.max())
+        dt_estimate = (temp1 + np.sqrt(temp1**2 + 4 * temp2)) / (temp2 * kmax * medium.sound_speed.max())
 
         # use a fixed point iteration to find the correct timestep, assuming
         # now that kappa = kappa(dt), using the previous estimate as a starting
         # point
 
         # first define the function to iterate
         def kappa(dt):
             return sinc(c_ref * kmax * dt / 2)
 
         def temp3(dt):
             return medium.sound_speed.max() * absorb_tau.min() * kappa(dt) * kmax ** (medium.alpha_power - 1)
 
         def func_to_solve(dt):
-            return (temp3(dt) + np.sqrt((temp3(dt)) ** 2 + 4 * temp2)) / (
-                    temp2 * kmax * kappa(dt) * medium.sound_speed.max())
+            return (temp3(dt) + np.sqrt((temp3(dt)) ** 2 + 4 * temp2)) / (temp2 * kmax * kappa(dt) * medium.sound_speed.max())
 
         # run the fixed point iteration
         dt_stability_limit = dt_estimate
         dt_old = 0
         while abs(dt_stability_limit - dt_old) > FIXED_POINT_ACCURACY:
             dt_old = dt_stability_limit
             dt_stability_limit = func_to_solve(dt_stability_limit)
@@ -279,24 +271,21 @@
         max_number: integer specifying the upper bound of values to test
 
     """
 
     # compute the factors and maximum prime factors for each number in the range
     factors = {}
     for n in range(min_number, max_number):
-        factors[n] = {
-            'factors': primefactors(n),
-            'max_prime_factor': max(primefactors(n))
-        }
+        factors[n] = {"factors": primefactors(n), "max_prime_factor": max(primefactors(n))}
 
     # print the numbers that match each maximum prime factor
     for factor in [2, 3, 5, 7]:
-        logging.log(logging.INFO, f'Numbers with a maximum prime factor of {factor}:')
+        logging.log(logging.INFO, f"Numbers with a maximum prime factor of {factor}:")
         for n in range(min_number, max_number):
-            if factors[n]['max_prime_factor'] == factor:
+            if factors[n]["max_prime_factor"] == factor:
                 logging.log(logging.INFO, n)
 
 
 def check_divisible(number: float, divider: float) -> bool:
     """
     Checks whether number is divisible by divider without any remainder
     Why do we need such a function? -> Because due to floating point precision we
```

### Comparing `k_wave_python-0.3.2/kwave/utils/colormap.py` & `k_wave_python-0.3.3/kwave/utils/colormap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 
 import numpy as np
-from beartype import beartype
-from nptyping import NDArray, Float, Shape
+from beartype import beartype as typechecker
+from jaxtyping import Float
 from matplotlib.colors import ListedColormap
 
 
-@beartype
+@typechecker
 def get_color_map(num_colors: Optional[int] = None) -> ListedColormap:
     """
     Returns the default color map used for display and visualisation across
     the k-Wave Toolbox. Zero values are displayed as white, positive values
     are displayed as yellow through red to black, and negative values are
     displayed as light to dark blue-greys. If no value for `num_colors` is
     provided, `cm` will have 256 colors.
@@ -34,53 +34,53 @@
     neg = neg[neg_pad:, :]
     pos = np.flipud(hot(num_colors // 2))
 
     colors = np.vstack([neg, pos])
     return ListedColormap(colors)
 
 
-@beartype
-def hot(m: int) -> NDArray[Shape["N, 3"], Float]:
+@typechecker
+def hot(m: int) -> Float[np.ndarray, "N 3"]:
     """
     Generate a hot colormap of length m.
     The colormap consists of a progression from black to red, yellow, and white.
 
     Args:
         m: The length of the colormap.
 
     Returns:
         An m-by-3 array containing the hot colormap.
 
     """
 
     n = int(np.fix(3 / 8 * m))
 
-    r = np.concatenate([np.arange(1, n + 1) / n, np.ones(m-n)])
-    g = np.concatenate([np.zeros(n), np.arange(1, n + 1) / n, np.ones(m-2*n)])
-    b = np.concatenate([np.zeros(2*n), np.arange(1, m-2*n + 1)/(m-2*n)])
+    r = np.concatenate([np.arange(1, n + 1) / n, np.ones(m - n)])
+    g = np.concatenate([np.zeros(n), np.arange(1, n + 1) / n, np.ones(m - 2 * n)])
+    b = np.concatenate([np.zeros(2 * n), np.arange(1, m - 2 * n + 1) / (m - 2 * n)])
 
     return np.hstack([r[:, None], g[:, None], b[:, None]])
 
 
-@beartype
-def bone(m: int) -> NDArray[Shape["N, 3"], Float]:
+@typechecker
+def bone(m: int) -> Float[np.ndarray, "N 3"]:
     """
     Returns an m-by-3 matrix containing a "bone" colormap.
 
     Args:
         m: The number of rows in the colormap.
 
     Returns:
         An m-by-3 matrix containing the colormap.
     """
     return (7 * gray(m) + np.fliplr(hot(m))) / 8
 
 
-@beartype
-def gray(m: int) -> NDArray[Shape["N, 3"], Float]:
+@typechecker
+def gray(m: int) -> Float[np.ndarray, "N 3"]:
     """
     Returns an M-by-3 matrix containing a grayscale colormap.
 
     Args:
         m: The length of the colormap.
 
     Returns:
```

### Comparing `k_wave_python-0.3.2/kwave/utils/conversion.py` & `k_wave_python-0.3.3/kwave/utils/conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import math
 from typing import Any
 
 import numpy as np
 from numpy import ndarray
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Tuple, Union
-from nptyping import NDArray, Float, Shape
+from jaxtyping import Real, Float, Num
 
 from kwave.kgrid import kWaveGrid
 from kwave.utils.matlab import matlab_mask
 from kwave.utils.matrix import sort_rows
 
 import kwave.utils.typing as kt
 
 
-@beartype
-def db2neper(alpha: Union[NDArray, kt.NUMERIC], y: kt.NUMERIC = 1) -> Union[NDArray, kt.NUMERIC]:
+@typechecker
+def db2neper(alpha: Real[kt.ArrayLike, "..."], y: Real[kt.ScalarLike, ""] = 1) -> Real[kt.ArrayLike, "..."]:
     """
     Convert decibels to nepers.
 
     Args:
         alpha: Attenuation in dB / (MHz ^ y cm).
         y: Power law exponent (default=1).
 
@@ -30,16 +30,16 @@
     """
 
     # calculate conversion
     alpha = 100 * alpha * (1e-6 / (2 * math.pi)) ** y / (20 * np.log10(np.exp(1)))
     return alpha
 
 
-@beartype
-def neper2db(alpha: Union[NDArray, kt.NUMERIC], y: kt.NUMERIC = 1) -> Union[NDArray, kt.NUMERIC]:
+@typechecker
+def neper2db(alpha: Real[kt.ArrayLike, "..."], y: Real[kt.ScalarLike, ""] = 1) -> Real[kt.ArrayLike, "..."]:
     """
     Converts an attenuation coefficient in units of Nepers / ((rad / s) ^ y m) to units of dB / (MHz ^ y cm).
 
     Args:
         alpha: Attenuation in Nepers / ((rad / s) ^ y m)
         y: Power law exponent (default=1)
 
@@ -49,61 +49,58 @@
     """
 
     # calculate conversion
     alpha = 20 * math.log10(math.exp(1)) * alpha * (2 * math.pi * 1e6) ** y / 100
     return alpha
 
 
-@beartype
-def cast_to_type(data: Union[NDArray, kt.NUMERIC], matlab_type: str) -> Any:
+@typechecker
+def cast_to_type(data: Real[kt.ArrayLike, "..."], matlab_type: str) -> Any:
     """
 
     Args:
         data: The data to cast.
         matlab_type: The type to cast to.
 
     Returns:
         The cast data.
 
     """
     if not isinstance(data, np.ndarray):
         data = np.array(data)
     type_map = {
-        'single': np.float32,
-        'double': np.float64,
-        'uint64': np.uint64,
-        'uint32': np.uint32,
-        'uint16': np.uint16,
+        "single": np.float32,
+        "double": np.float64,
+        "uint64": np.uint64,
+        "uint32": np.uint32,
+        "uint16": np.uint16,
     }
     return data.astype(type_map[matlab_type])
 
 
-@beartype
-def cart2pol(
-    x: Union[kt.NUMERIC, NDArray], 
-    y: Union[kt.NUMERIC, NDArray]
-) -> Tuple[Union[kt.NUMERIC, NDArray], Union[kt.NUMERIC, NDArray]]:
+@typechecker
+def cart2pol(x: Real[kt.ArrayLike, "..."], y: Real[kt.ArrayLike, "..."]) -> Tuple[Real[kt.ArrayLike, "..."], Real[kt.ArrayLike, "..."]]:
     """
     Convert from cartesian to polar coordinates.
 
     Args:
         x: The x-coordinate of the point.
         y: The y-coordinate of the point.
 
     Returns:
         A tuple containing the polar coordinates of the point.
 
     """
 
-    rho = np.sqrt(x ** 2 + y ** 2)
+    rho = np.sqrt(x**2 + y**2)
     phi = np.arctan2(y, x)
     return phi, rho
 
 
-@beartype
+@typechecker
 def grid2cart(input_kgrid: kWaveGrid, grid_selection: ndarray) -> Tuple[ndarray, ndarray]:
     """
     Returns the Cartesian coordinates of the non-zero points of a binary grid.
 
     Args:
         input_kgrid: k-Wave grid object returned by kWaveGrid
         grid_selection: binary grid with the same dimensions as the k-Wave grid kgrid
@@ -129,17 +126,16 @@
     if 0 <= input_kgrid.dim > 3:
         raise ValueError("kGrid with unsupported size passed.")
 
     order_index = np.argwhere(grid_data.squeeze() != 0)
     return cart_data.squeeze(), order_index
 
 
-@beartype
-def freq2wavenumber(n: int, k_max: float, filter_cutoff: float, c: float, k_dim: Union[int, Tuple[int]]) -> Tuple[
-    int, float]:
+@typechecker
+def freq2wavenumber(n: int, k_max: float, filter_cutoff: float, c: float, k_dim: Union[int, Tuple[int]]) -> Tuple[int, float]:
     """
     Convert the given frequency and maximum wavenumber to a wavenumber cutoff and filter size.
 
     Args:
         n: The size of the grid.
         k_max: The maximum wavenumber.
         filter_cutoff: The frequency to convert to a wavenumber cutoff.
@@ -160,22 +156,20 @@
     if filter_size > n:
         # set the alpha_filter size to be the same as the grid size
         filter_size = n
         filter_cutoff = k_max * c / (2 * np.pi)
     return filter_size, filter_cutoff
 
 
-@beartype
-def cart2grid(kgrid: kWaveGrid, 
-              cart_data: Union[
-                  NDArray[Shape["1, NumPoints"], Float],
-                  NDArray[Shape["2, NumPoints"], Float],
-                  NDArray[Shape["3, NumPoints"], Float],
-              ], 
-              axisymmetric: bool=False) -> Tuple:
+@typechecker
+def cart2grid(
+    kgrid: kWaveGrid,
+    cart_data: Union[Float[ndarray, "1 NumPoints"], Float[ndarray, "2 NumPoints"], Float[ndarray, "3 NumPoints"]],
+    axisymmetric: bool = False,
+) -> Tuple:
     """
     Interpolates the set of Cartesian points defined by
     cart_data onto a binary matrix defined by the kWaveGrid object
     kgrid using nearest neighbour interpolation. An error is returned if
     the Cartesian points are outside the computational domain defined by
     kgrid.
 
@@ -187,15 +181,15 @@
     Returns:
         A binary grid
 
     """
 
     # check for axisymmetric input
     if axisymmetric and kgrid.dim != 2:
-        raise AssertionError('Axisymmetric flag only supported in 2D.')
+        raise AssertionError("Axisymmetric flag only supported in 2D.")
 
     # detect whether the inputs are for one, two, or three dimensions
     if kgrid.dim == 1:
         # one-dimensional
         data_x = cart_data[0, :]
 
         # scale position values to grid centered pixel coordinates using
@@ -203,15 +197,15 @@
         data_x = np.round(data_x / kgrid.dx).astype(int)
 
         # shift pixel coordinates to coincide with matrix indexing
         data_x = data_x + np.floor(kgrid.Nx // 2).astype(int)
 
         # check if the points all lie within the grid
         if data_x.max() > kgrid.Nx or data_x.min() < 1:
-            raise AssertionError('Cartesian points must lie within the grid defined by kgrid.')
+            raise AssertionError("Cartesian points must lie within the grid defined by kgrid.")
 
         # create empty grid
         grid_data = np.zeros((kgrid.Nx, 1))
 
         # create index variable
         point_index = np.arange(1, data_x.size + 1)
 
@@ -238,31 +232,28 @@
         if not axisymmetric:
             data_y = data_y + np.floor(kgrid.Ny // 2).astype(int)
         else:
             data_y = data_y
 
         # check if the points all lie within the grid
         if data_x.max() >= kgrid.Nx or data_y.max() >= kgrid.Ny or data_x.min() < 0 or data_y.min() < 0:
-            raise AssertionError('Cartesian points must lie within the grid defined by kgrid.')
+            raise AssertionError("Cartesian points must lie within the grid defined by kgrid.")
 
         # create empty grid
         grid_data = -1 * np.ones((kgrid.Nx, kgrid.Ny))
 
         # map values
         for data_index in range(data_x.size):
             grid_data[data_x[data_index], data_y[data_index]] = int(data_index)
 
         # extract reordering index
-        reorder_index = grid_data.flatten(order='F')[
-            grid_data.flatten(order='F') != -1
-            ]
+        reorder_index = grid_data.flatten(order="F")[grid_data.flatten(order="F") != -1]
         reorder_index = reorder_index[:, None] + 1  # [N] => [N, 1]
 
     elif kgrid.dim == 3:
-
         # three dimensional
         data_x = cart_data[0, :]
         data_y = cart_data[1, :]
         data_z = cart_data[2, :]
 
         # scale position values to grid centered pixel coordinates using
         # nearest neighbour interpolation
@@ -272,35 +263,38 @@
 
         # shift pixel coordinates to coincide with matrix indexing
         data_x = data_x + np.floor(kgrid.Nx // 2).astype(int)
         data_y = data_y + np.floor(kgrid.Ny // 2).astype(int)
         data_z = data_z + np.floor(kgrid.Nz // 2).astype(int)
 
         # check if the points all lie within the grid
-        assert 0 <= data_x.min() and 0 <= data_y.min() and 0 <= data_z.min() and \
-               data_x.max() < kgrid.Nx and data_y.max() < kgrid.Ny and data_z.max() < kgrid.Nz, \
-            "Cartesian points must lie within the grid defined by kgrid."
+        assert (
+            0 <= data_x.min()
+            and 0 <= data_y.min()
+            and 0 <= data_z.min()
+            and data_x.max() < kgrid.Nx
+            and data_y.max() < kgrid.Ny
+            and data_z.max() < kgrid.Nz
+        ), "Cartesian points must lie within the grid defined by kgrid."
 
         # create empty grid
         grid_data = -1 * np.ones((kgrid.Nx, kgrid.Ny, kgrid.Nz), dtype=int)
 
         # create index variable
         point_index = np.arange(1, data_x.size + 1)
 
         # map values
         for data_index in range(data_x.size):
             grid_data[data_x[data_index], data_y[data_index], data_z[data_index]] = point_index[data_index]
 
         # extract reordering index
-        reorder_index = grid_data.flatten(order='F')[
-            grid_data.flatten(order='F') != -1
-            ]
+        reorder_index = grid_data.flatten(order="F")[grid_data.flatten(order="F") != -1]
         reorder_index = reorder_index[:, None, None]  # [N] => [N, 1, 1]
     else:
-        raise ValueError('Input cart_data must be a 1, 2, or 3 dimensional matrix.')
+        raise ValueError("Input cart_data must be a 1, 2, or 3 dimensional matrix.")
 
     # compute the reverse ordering index (i.e., what is the index of each point
     # in the reordering vector)
     order_index = np.ones((reorder_index.size, 2), dtype=int)
     order_index[:, 0] = np.squeeze(reorder_index)
     order_index[:, 1] = np.arange(1, reorder_index.size + 1)
     order_index = sort_rows(order_index, 0)
@@ -314,22 +308,22 @@
         grid_data[grid_data != -1] = 1
         grid_data[grid_data == -1] = 0
 
     # check if any Cartesian points have been mapped to the same grid point,
     # thereby reducing the total number of points
     num_discarded_points = cart_data.shape[1] - np.sum(grid_data)
     if num_discarded_points != 0:
-        logging.log(logging.INFO, f'  cart2grid: {num_discarded_points} Cartesian points mapped to overlapping grid points')
+        logging.log(logging.INFO, f"  cart2grid: {num_discarded_points} Cartesian points mapped to overlapping grid points")
     return grid_data.astype(int), order_index, reorder_index
 
 
-@beartype
+@typechecker
 def hounsfield2soundspeed(
-    ct_data:  Union[NDArray[Shape["Dim1, Dim2"], Float], NDArray[Shape["Dim1, Dim2, Dim3"], Float]]
-) -> Union[NDArray[Shape["Dim1, Dim2"], Float], NDArray[Shape["Dim1, Dim2, Dim3"], Float]]:
+    ct_data: Union[Float[ndarray, "Dim1 Dim2"], Float[ndarray, "Dim1 Dim2 Dim3"]],
+) -> Union[Float[ndarray, "Dim1 Dim2"], Float[ndarray, "Dim1 Dim2 Dim3"]]:
     """
     Calculates the sound speed of a medium given a CT (computed tomography) of the medium.
     For soft tissue, the approximate sound speed can also be returned using the empirical relationship
     given by Mast [1].
 
     Args:
         ct_data: matrix of Hounsfield values.
@@ -344,19 +338,18 @@
     # calculate corresponding sound speed values if required using soft tissue relationship
     # TODO confirm that this linear relationship is correct
     sound_speed = (hounsfield2density(ct_data) + 349) / 0.893
 
     return sound_speed
 
 
-@beartype
+@typechecker
 def hounsfield2density(
-    ct_data: Union[NDArray[Shape["Dim1, Dim2"], Float], NDArray[Shape["Dim1, Dim2, Dim3"], Float]], 
-    plot_fitting: bool = False
-) ->  Union[NDArray[Shape["Dim1, Dim2"], Float], NDArray[Shape["Dim1, Dim2, Dim3"], Float]]:
+    ct_data: Union[Float[ndarray, "Dim1 Dim2"], Float[ndarray, "Dim1 Dim2 Dim3"]], plot_fitting: bool = False
+) -> Union[Float[ndarray, "Dim1 Dim2"], Float[ndarray, "Dim1 Dim2 Dim3"]]:
     """
     Convert Hounsfield units in CT data to density values [kg / m ^ 3] based on experimental data.
 
     Args:
         ct_data: The CT data in Hounsfield units.
         plot_fitting (bool, optional): Whether to plot the fitting curve (default: False).
 
@@ -370,16 +363,15 @@
 
     # apply conversion in several parts using linear fits to the data
     # Part 1: Less than 930 Hounsfield Units
     density[ct_data < 930] = np.polyval([1.025793065681423, -5.680404011488714], ct_data[ct_data < 930])
 
     # Part 2: Between 930 and 1098(soft tissue region)
     index_selection = np.logical_and(930 <= ct_data, ct_data <= 1098)
-    density[index_selection] = np.polyval([0.9082709691264, 103.6151457847139],
-                                          ct_data[index_selection])
+    density[index_selection] = np.polyval([0.9082709691264, 103.6151457847139], ct_data[index_selection])
 
     # Part 3: Between 1098 and 1260(between soft tissue and bone)
     index_selection = np.logical_and(1098 < ct_data, ct_data < 1260)
     density[index_selection] = np.polyval([0.5108369316599, 539.9977189228704], ct_data[index_selection])
 
     # Part 4: Greater than 1260(bone region)
     density[ct_data >= 1260] = np.polyval([0.6625370912451, 348.8555178455294], ct_data[ct_data >= 1260])
@@ -390,21 +382,21 @@
     return density
 
 
 tol = None
 subs0 = None
 
 
-@beartype
+@typechecker
 def tol_star(
-    tolerance: kt.NUMERIC, 
-    kgrid: kWaveGrid, 
-    point: Union[NDArray[Shape["1"], Float], NDArray[Shape["2"], Float], NDArray[Shape["3"], Float]], 
-    debug
-) -> Tuple[NDArray, NDArray, NDArray, NDArray]:
+    tolerance: kt.NUMERIC,
+    kgrid: kWaveGrid,
+    point: Union[Float[ndarray, "1"], Float[ndarray, "2"], Float[ndarray, "3"]],
+    debug,
+) -> Tuple[ndarray, ndarray, ndarray, ndarray]:
     global tol, subs0
 
     ongrid_threshold = kgrid.dx * 1e-3
 
     kgrid_dim = kgrid.dim
     if tol is None or tolerance != tol or len(subs0) != kgrid_dim:
         tol = tolerance
@@ -412,17 +404,17 @@
         decay_subs = int(np.ceil(1 / (np.pi * tol)))
 
         lin_ind = np.arange(-decay_subs, decay_subs + 1)
 
         if kgrid_dim == 1:
             is0 = lin_ind
         elif kgrid_dim == 2:
-            is0, js0 = np.meshgrid(lin_ind, lin_ind, indexing='ij')
+            is0, js0 = np.meshgrid(lin_ind, lin_ind, indexing="ij")
         elif kgrid_dim == 3:
-            is0, js0, ks0 = np.meshgrid(lin_ind, lin_ind, lin_ind, indexing='ij')
+            is0, js0, ks0 = np.meshgrid(lin_ind, lin_ind, lin_ind, indexing="ij")
 
         if kgrid_dim == 1:
             subs0 = [is0]
         elif kgrid_dim == 2:
             instar = np.abs(is0 * js0) <= decay_subs
             is0 = matlab_mask(is0, instar)
             js0 = matlab_mask(js0, instar)
@@ -488,16 +480,15 @@
         lin_ind = is_
     elif kgrid_dim == 2:
         lin_ind = kgrid.Nx * (js - 1) + is_
     elif kgrid_dim == 3:
         lin_ind = kgrid.Nx * kgrid.Ny * (ks - 1) + kgrid.Nx * (js - 1) + is_
 
     # TODO: in current form linear indexing matches MATLAB, but might break in 0 indexed python
-    return lin_ind, np.array(is_) - 1, np.array(js) - 1, np.array(
-        ks) - 1  # -1 for mapping from Matlab indexing to Python indexing
+    return lin_ind, np.array(is_) - 1, np.array(js) - 1, np.array(ks) - 1  # -1 for mapping from Matlab indexing to Python indexing
 
 
-@beartype
-def find_closest(array: NDArray, value: kt.NUMERIC_WITH_COMPLEX):
+@typechecker
+def find_closest(array: ndarray, value: Num[kt.ScalarLike, ""]):
     array = np.asarray(array)
     idx = (np.abs(array - value)).argmin()
     return array[idx], idx
```

### Comparing `k_wave_python-0.3.2/kwave/utils/data.py` & `k_wave_python-0.3.3/kwave/utils/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from datetime import datetime
 from math import floor
 from beartype.typing import Tuple, Union, Optional
-from beartype import beartype
-from nptyping import NDArray
+from beartype import beartype as typechecker
 
 import numpy as np
 from kwave.data import Vector
 
 from kwave.utils.typing import NUMERIC_WITH_COMPLEX
 
 
-@beartype
+@typechecker
 def get_smallest_possible_type(
-    max_array_val: Union[NUMERIC_WITH_COMPLEX, Vector], 
-    target_type_group: str, 
-    default: Optional[str]=None
+    max_array_val: Union[NUMERIC_WITH_COMPLEX, Vector], target_type_group: str, default: Optional[str] = None
 ) -> Union[str, None]:
     """
     Returns the smallest possible type for the given array.
     Args:
         max_array_val: The maximum value in the array.
         target_type_group: The type group to search for the smallest possible type.
         default: The default type to return if no type is found.
 
     Returns:
         The smallest possible type for the given array.
 
     """
 
-    types = {'uint', 'int'}
+    types = {"uint", "int"}
     assert target_type_group in types
 
     for bit_count in [8, 16, 32]:
-        type_ = f'{target_type_group}{bit_count}'
+        type_ = f"{target_type_group}{bit_count}"
         if max_array_val < intmax(type_):
             return type_
 
     type_ = default
     return type_
 
 
-@beartype
+@typechecker
 def intmax(dtype: str) -> int:
     """
     Returns the maximum value for the given integer type.
 
     Args:
         dtype: The integer type.
 
@@ -52,15 +49,15 @@
         The maximum value for the given integer type.
 
     """
 
     return np.iinfo(getattr(np, dtype)).max
 
 
-@beartype
+@typechecker
 def scale_time(seconds: Union[int, float]) -> str:
     """
     Converts an integer number of seconds into hours, minutes,
     and seconds, and returns a string with this information.
 
     Args:
         seconds: number of seconds
@@ -88,38 +85,38 @@
     seconds = seconds - hours * 60 * 60
     minutes = floor(seconds / 60)
     seconds = seconds - minutes * 60
 
     # write out as a string, to keep the output manageable, only the largest
     # three units are written
     if years > 0:
-        time = f'{years} years, {weeks} weeks, and {days} days'
+        time = f"{years} years, {weeks} weeks, and {days} days"
     elif weeks > 0:
-        time = f'{weeks} weeks, {days} days, and {hours} hours'
+        time = f"{weeks} weeks, {days} days, and {hours} hours"
     elif days > 0:
-        time = f'{days} days, {hours} hours, and {minutes} min'
+        time = f"{days} days, {hours} hours, and {minutes} min"
     elif hours > 0:
         seconds = np.round(seconds, 4)
         if np.abs(seconds - int(seconds)) < 1e-4:
             seconds = int(seconds)
-        time = f'{hours}hours {minutes}min {seconds}s'
+        time = f"{hours}hours {minutes}min {seconds}s"
     elif minutes > 0:
         seconds = np.round(seconds, 4)
         if np.abs(seconds - int(seconds)) < 1e-4:
             seconds = int(seconds)
-        time = f'{minutes}min {seconds}s'
+        time = f"{minutes}min {seconds}s"
     else:
         precision = 10  # manually tuned number
         seconds = round(seconds, precision)
-        time = f'{seconds}s'
+        time = f"{seconds}s"
     return time
 
 
-@beartype
-def scale_SI(x: Union[float, NDArray]) -> Tuple[str, Union[int, float], str, str]:
+@typechecker
+def scale_SI(x: Union[float, np.ndarray]) -> Tuple[str, Union[int, float], str, str]:
     """
     Scale a number to the nearest SI unit prefix.
 
     Args:
         x: The number to scale.
 
     Returns:
@@ -134,81 +131,78 @@
     if x < 0:
         x = -x
         negative = True
     else:
         negative = False
 
     if x == 0:
-
         # if x is zero, don't scale
         x_sc = x
-        prefix = ''
-        prefix_fullname = ''
+        prefix = ""
+        prefix_fullname = ""
         scale = 1
 
     elif x < 1:
-
         # update index and input
         x_sc = x * 1e3
         sym_index = 1
 
         # find scaling parameter
         while x_sc < 1 and sym_index < 8:
             x_sc = x_sc * 1e3
             sym_index = sym_index + 1
 
         # define SI unit scalings
         units = {
-            1: ('m', 'milli', 1e3),
-            2: ('u', 'micro', 1e6),
-            3: ('n', 'nano', 1e9),
-            4: ('p', 'pico', 1e12),
-            5: ('f', 'femto', 1e15),
-            6: ('a', 'atto', 1e18),
-            7: ('z', 'zepto', 1e21),
-            8: ('y', 'yocto', 1e24),
+            1: ("m", "milli", 1e3),
+            2: ("u", "micro", 1e6),
+            3: ("n", "nano", 1e9),
+            4: ("p", "pico", 1e12),
+            5: ("f", "femto", 1e15),
+            6: ("a", "atto", 1e18),
+            7: ("z", "zepto", 1e21),
+            8: ("y", "yocto", 1e24),
         }
         prefix, prefix_fullname, scale = units[sym_index]
 
     elif x >= 1000:
-
         # update index and input
         x_sc = x * 1e-3
         sym_index = 1
 
         # find scaling parameter
         while x_sc >= 1000 and sym_index < 8:
             x_sc = x_sc * 1e-3
             sym_index = sym_index + 1
 
         # define SI unit scalings
         units = {
-            1: ('k', 'kilo', 1e-3),
-            2: ('M', 'mega', 1e-6),
-            3: ('G', 'giga', 1e-9),
-            4: ('T', 'tera', 1e-12),
-            5: ('P', 'peta', 1e-15),
-            6: ('E', 'exa', 1e-18),
-            7: ('Z', 'zetta', 1e-21),
-            8: ('Y', 'yotta', 1e-24)
+            1: ("k", "kilo", 1e-3),
+            2: ("M", "mega", 1e-6),
+            3: ("G", "giga", 1e-9),
+            4: ("T", "tera", 1e-12),
+            5: ("P", "peta", 1e-15),
+            6: ("E", "exa", 1e-18),
+            7: ("Z", "zetta", 1e-21),
+            8: ("Y", "yotta", 1e-24),
         }
         prefix, prefix_fullname, scale = units[sym_index]
 
     else:
         # if x is between 1 and 1000, don't scale
         x_sc = x
-        prefix = ''
-        prefix_fullname = ''
+        prefix = ""
+        prefix_fullname = ""
         scale = 1
 
     # form scaling into a string
     round_decimals = 6  # TODO this needs to be tuned
     x_sc = x_sc.round(round_decimals)
-    if (x_sc - int(x_sc)) < (0.1 ** round_decimals):
+    if (x_sc - int(x_sc)) < (0.1**round_decimals):
         # avoid values like X.0, instead have only X
         x_sc = int(x_sc)
-    x_sc = f'-{x_sc}{prefix}' if negative else f'{x_sc}{prefix}'
+    x_sc = f"-{x_sc}{prefix}" if negative else f"{x_sc}{prefix}"
     return x_sc, scale, prefix, prefix_fullname
 
 
 def get_date_string() -> str:
     return datetime.now().strftime("%d-%b-%Y-%H-%M-%S")
```

### Comparing `k_wave_python-0.3.2/kwave/utils/dotdictionary.py` & `k_wave_python-0.3.3/kwave/utils/dotdictionary.py`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/kwave/utils/filters.py` & `k_wave_python-0.3.3/kwave/utils/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,47 +26,46 @@
         fft_len: The length of the FFT.
         dim: The number of dimensions of `func_fft`.
 
     Returns:
         The corrected FFT of the function.
     """
     if fft_len % 2:
-
         # odd FFT length switch dim case
         if dim == 0:
             func_fft[1:, :] = func_fft[1:, :] * 2
         elif dim == 1:
             func_fft[:, 1:] = func_fft[:, 1:] * 2
         elif dim == 2:
             func_fft[:, :, 1:] = func_fft[:, :, 1:] * 2
         elif dim == 3:
             func_fft[:, :, :, 1:] = func_fft[:, :, :, 1:] * 2
     else:
-
         # even FFT length
         if dim == 0:
-            func_fft[1: -1] = func_fft[1: -1] * 2
+            func_fft[1:-1] = func_fft[1:-1] * 2
         elif dim == 1:
-            func_fft[:, 1: -1] = func_fft[:, 1: -1] * 2
+            func_fft[:, 1:-1] = func_fft[:, 1:-1] * 2
         elif dim == 2:
-            func_fft[:, :, 1: -1] = func_fft[:, :, 1: -1] * 2
+            func_fft[:, :, 1:-1] = func_fft[:, :, 1:-1] * 2
         elif dim == 3:
-            func_fft[:, :, :, 1: -1] = func_fft[:, :, :, 1: -1] * 2
+            func_fft[:, :, :, 1:-1] = func_fft[:, :, :, 1:-1] * 2
 
     return func_fft
 
 
 def spect(
-        func: np.ndarray,
-        Fs: float,
-        dim: Optional[Union[int, str]] = 'auto',
-        fft_len: Optional[int] = 0,
-        power_two: Optional[bool] = False,
-        unwrap_phase: Optional[bool] = False,
-        window: Optional[str] = 'Rectangular') -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    func: np.ndarray,
+    Fs: float,
+    dim: Optional[Union[int, str]] = "auto",
+    fft_len: Optional[int] = 0,
+    power_two: Optional[bool] = False,
+    unwrap_phase: Optional[bool] = False,
+    window: Optional[str] = "Rectangular",
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Calculates the spectrum of a signal.
 
     Args:
         func: The signal to analyse.
         Fs: The sampling frequency in Hz.
         dim: The dimension over which the spectrum is calculated. Defaults to 'auto'.
@@ -87,22 +86,22 @@
     """
 
     # check the size of the input
     sz = func.shape
 
     # check input isn't scalar
     if np.size(func) == 1:
-        raise ValueError('Input signal cannot be scalar.')
+        raise ValueError("Input signal cannot be scalar.")
 
     # check input doesn't have more than 4 dimensions
     if len(sz) > 4:
-        raise ValueError('Input signal must have 1, 2, 3, or 4 dimensions.')
+        raise ValueError("Input signal must have 1, 2, 3, or 4 dimensions.")
 
     # automatically set dimension to first non - singleton dimension
-    if dim == 'auto':
+    if dim == "auto":
         dim_index = 0
         while dim_index <= len(sz):
             if sz[dim_index] > 1:
                 dim = dim_index
                 break
             dim_index = dim_index + 1
 
@@ -134,19 +133,19 @@
 
     # reduce to a single sided spectrum where the number of unique points for
     # even numbered FFT lengths is given by N / 2 + 1, and for odd(N + 1) / 2
     num_unique_pts = int(np.ceil((fft_len + 1) / 2))
     if dim == 0:
         func_fft = func_fft[0:num_unique_pts]
     elif dim == 1:
-        func_fft = func_fft[:, 0: num_unique_pts]
+        func_fft = func_fft[:, 0:num_unique_pts]
     elif dim == 2:
-        func_fft = func_fft[:, :, 0: num_unique_pts]
+        func_fft = func_fft[:, :, 0:num_unique_pts]
     elif dim == 3:
-        func_fft = func_fft[:, :, :, 0: num_unique_pts]
+        func_fft = func_fft[:, :, :, 0:num_unique_pts]
 
     func_fft = single_sided_correction(func_fft, fft_len, dim)
 
     # create the frequency axis variable
     f = np.arange(0, func_fft.shape[dim]) * Fs / fft_len
 
     # calculate the amplitude spectrum
@@ -158,17 +157,17 @@
     # unwrap the phase spectrum if required
     if unwrap_phase:
         func_ps = scipy.unwrap(func_ps, [], dim)
 
     return f, func_as, func_ps
 
 
-def extract_amp_phase(data: np.ndarray, Fs: float, source_freq: float, dim: Tuple[str, int] = 'auto',
-                      fft_padding: int = 3,
-                      window: str = 'Hanning') -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+def extract_amp_phase(
+    data: np.ndarray, Fs: float, source_freq: float, dim: Tuple[str, int] = "auto", fft_padding: int = 3, window: str = "Hanning"
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Extract the amplitude and phase information at a specified frequency from a vector or matrix of time series data.
 
     The amplitude and phase are extracted from the frequency spectrum, which is calculated using a windowed and zero
     padded FFT. The values are extracted at the frequency closest to source_freq. By default, the time dimension is set
     to the highest non-singleton dimension.
 
@@ -182,15 +181,15 @@
 
     Returns:
         A tuple of the amplitude, phase and frequency of the extracted signal.
 
     """
 
     # check for the dim input
-    if dim == 'auto':
+    if dim == "auto":
         dim = num_dim(data)
         if dim == 2 and data.shape[1] == 1:
             dim = 1
 
     # create 1D window and reshape to be oriented in the time dimension of the
     # input data
     win, coherent_gain = get_win(data.shape[dim], window)
@@ -224,15 +223,15 @@
     elif dim == 2:
         amp = func_as[:, :, f_index]
         phase = func_ps[:, :, f_index]
     elif dim == 3:
         amp = func_as[:, :, :, f_index]
         phase = func_ps[:, :, :, f_index]
     else:
-        raise ValueError('dim must be 0, 1, 2, or 3')
+        raise ValueError("dim must be 0, 1, 2, or 3")
 
     return amp.squeeze(), phase.squeeze(), f[f_index]
 
 
 def brenner_sharpness(im):
     num_dim = im.ndim
     if num_dim == 2:
@@ -260,16 +259,19 @@
     elif num_dim == 3:
         # define the 3D sobel gradient operator
         sobel3D = np.zeros((3, 3, 3))
         sobel3D[:, :, 0] = np.array([[1, 2, 1], [2, 4, 2], [1, 2, 1]])
         sobel3D[:, :, 2] = -sobel3D[:, :, 0]
 
         # compute metric
-        s = (convolve(im, sobel3D) ** 2 + convolve(im, np.transpose(sobel3D, (2, 0, 1))) ** 2 +
-             convolve(im, np.transpose(sobel3D, (1, 2, 0))) ** 2).sum()
+        s = (
+            convolve(im, sobel3D) ** 2
+            + convolve(im, np.transpose(sobel3D, (2, 0, 1))) ** 2
+            + convolve(im, np.transpose(sobel3D, (1, 2, 0))) ** 2
+        ).sum()
     return s
 
     # TODO: get this passing the tests
     # NOTE: Walter thinks this is the proper way to do this, but it doesn't match the MATLAB version
     # num_dim = im.ndim
     # if num_dim == 2:
     #     # compute metric
@@ -285,17 +287,15 @@
     #     sz = sobel(im, axis=2, mode='constant')
     #     s = (sx ** 2) + (sy ** 2) + (sz ** 2)
     #     s = np.sum(s)
     # else:
     #     raise ValueError("Invalid number of dimensions in im")
 
 
-def sharpness(
-        im: np.ndarray,
-        mode: Optional[str] = "Brenner") -> float:
+def sharpness(im: np.ndarray, mode: Optional[str] = "Brenner") -> float:
     """
     Returns a scalar metric related to the sharpness of a 2D or 3D image matrix.
 
     Args:
         im: The image matrix.
         metric: The metric to use. Defaults to "Brenner".
 
@@ -316,16 +316,15 @@
     if mode == "Brenner":
         metric = brenner_sharpness(im)
     elif mode == "Tenenbaum":
         metric = tenenbaum_sharpness(im)
     elif mode == "NormVariance":
         metric = norm_var(im)
     else:
-        raise ValueError(
-            "Unrecognized sharpness metric passed. Valid values are ['Brenner', 'Tanenbaum', 'NormVariance']")
+        raise ValueError("Unrecognized sharpness metric passed. Valid values are ['Brenner', 'Tanenbaum', 'NormVariance']")
 
     return metric
 
 
 def fwhm(f, x):
     """
     fwhm calculates the Full Width at Half Maximum (FWHM) of a positive
@@ -348,29 +347,27 @@
 
     def lin_interp(x, y, i, half):
         return x[i] + (x[i + 1] - x[i]) * ((half - y[i]) / (y[i + 1] - y[i]))
 
     def half_max_x(x, y):
         half = max(y) / 2.0
         signs = np.sign(np.add(y, -half))
-        zero_crossings = (signs[0:-2] != signs[1:-1])
+        zero_crossings = signs[0:-2] != signs[1:-1]
         zero_crossings_i = np.where(zero_crossings)[0]
-        return [lin_interp(x, y, zero_crossings_i[0], half),
-                lin_interp(x, y, zero_crossings_i[1], half)]
+        return [lin_interp(x, y, zero_crossings_i[0], half), lin_interp(x, y, zero_crossings_i[1], half)]
 
     hmx = half_max_x(x, f)
     fwhm_val = hmx[1] - hmx[0]
 
     return fwhm_val, tuple(hmx)
 
 
-def gaussian_filter(signal: Union[np.ndarray, List[float]],
-                    Fs: float,
-                    frequency: float,
-                    bandwidth: float) -> Union[np.ndarray, List[float]]:
+def gaussian_filter(
+    signal: Union[np.ndarray, List[float]], Fs: float, frequency: float, bandwidth: float
+) -> Union[np.ndarray, List[float]]:
     """
     Applies a frequency domain Gaussian filter with the
     specified center frequency and percentage bandwidth to the input
     signal. If the input signal is given as a matrix, the filter is
     applied to each matrix row.
 
     Args:
@@ -395,33 +392,33 @@
     magnitude = 1
 
     # create double-sided Gaussain filter
     gfilter = np.fmax(gaussian(f, magnitude, mean, variance), gaussian(f, magnitude, -mean, variance))
 
     # add dimensions to filter to be broadcastable to signal shape
     if len(signal.shape) == 2:
-        gfilter = gfilter[np.newaxis,:]
+        gfilter = gfilter[np.newaxis, :]
 
     # apply filter
     signal = np.real(ifft(ifftshift(gfilter * fftshift(fft(signal)))))
 
     return signal
 
 
 def filter_time_series(
-        kgrid: "kWaveGrid",
-        medium: "kWaveMedium",
-        signal: np.ndarray,
-        ppw: Optional[int] = 3,
-        rppw: Optional[int] = 0,
-        stop_band_atten: Optional[int] = 60,
-        transition_width: Optional[float] = 0.1,
-        zerophase: Optional[bool] = False,
-        plot_spectrums: Optional[bool] = False,
-        plot_signals: Optional[bool] = False,
+    kgrid: "kWaveGrid",
+    medium: "kWaveMedium",
+    signal: np.ndarray,
+    ppw: Optional[int] = 3,
+    rppw: Optional[int] = 0,
+    stop_band_atten: Optional[int] = 60,
+    transition_width: Optional[float] = 0.1,
+    zerophase: Optional[bool] = False,
+    plot_spectrums: Optional[bool] = False,
+    plot_signals: Optional[bool] = False,
 ) -> np.ndarray:
     """
     Filters a time-domain signal using the Kaiser windowing method.
 
     The filter is designed to attenuate high-frequency noise in the signal while preserving
     the signal's important features. The filter design parameters can be adjusted to trade off
     between the amount of noise reduction and the amount of signal distortion.
@@ -467,60 +464,64 @@
         m, n = signal.shape
         if n == 1:
             signal = signal.T
             rotate_signal = True
         else:
             rotate_signal = False
     else:
-        raise TypeError('Input signal must be a vector.')
+        raise TypeError("Input signal must be a vector.")
 
     # update the command line status
-    logging.log(logging.INFO, 'Filtering input signal...')
+    logging.log(logging.INFO, "Filtering input signal...")
 
     # extract the time step
-    assert not isinstance(kgrid.t_array, str) or kgrid.t_array != 'auto', 'kgrid.t_array must be explicitly defined.'
+    assert not isinstance(kgrid.t_array, str) or kgrid.t_array != "auto", "kgrid.t_array must be explicitly defined."
 
     # compute the sampling frequency
     Fs = 1 / kgrid.dt
 
     # extract the minium sound speed
     if medium.sound_speed is not None:
-
         # for the fluid code, use medium.sound_speed
         c0 = medium.sound_speed.min()
 
-    elif all(medium.is_defined('sound_speed_compression', 'sound_speed_shear')):  # pragma: no cover
-
+    elif all(medium.is_defined("sound_speed_compression", "sound_speed_shear")):  # pragma: no cover
         # for the elastic code, combine the shear and compression sound speeds and remove zeros values
         ss = np.hstack([medium.sound_speed_compression, medium.sound_speed_shear])
         ss[ss == 0] = np.nan
         c0 = np.nanmin(ss)
 
         # cleanup unused variables
         del ss
 
     else:
         raise ValueError(
-            'The input fields medium.sound_speed or medium.sound_speed_compression and medium.sound_speed_shear must '
-            'be defined.')
+            "The input fields medium.sound_speed or medium.sound_speed_compression and medium.sound_speed_shear must " "be defined."
+        )
 
     # extract the maximum supported frequency (two points per wavelength)
     f_max = kgrid.k_max_all * c0 / (2 * np.pi)
 
     # calculate the filter cut-off frequency
     filter_cutoff_f = 2 * f_max / ppw
 
     # calculate the wavelength of the filter cut-off frequency as a number of time steps
-    filter_wavelength = ((2 * np.pi / filter_cutoff_f) / kgrid.dt)
+    filter_wavelength = (2 * np.pi / filter_cutoff_f) / kgrid.dt
 
     # filter the signal if required
     if ppw != 0:
-        filtered_signal = apply_filter(signal, Fs, float(filter_cutoff_f), 'LowPass',
-                                       zero_phase=zerophase, stop_band_atten=float(stop_band_atten),
-                                       transition_width=transition_width)
+        filtered_signal = apply_filter(
+            signal,
+            Fs,
+            float(filter_cutoff_f),
+            "LowPass",
+            zero_phase=zerophase,
+            stop_band_atten=float(stop_band_atten),
+            transition_width=transition_width,
+        )
 
     # add a start-up ramp if required
     if rppw != 0:
         # calculate the length of the ramp in time steps
         ramp_length = round(rppw * filter_wavelength / (2 * ppw))
 
         # create the ramp
@@ -530,37 +531,38 @@
         filtered_signal[1:ramp_length] = filtered_signal[1:ramp_length] * ramp
 
     # restore the original vector orientation if modified
     if rotate_signal:
         filtered_signal = filtered_signal.T
 
     # update the command line status
-    logging.log(logging.INFO, f'  maximum frequency supported by kgrid: {scale_SI(f_max)}Hz (2 PPW)')
+    logging.log(logging.INFO, f"  maximum frequency supported by kgrid: {scale_SI(f_max)}Hz (2 PPW)")
     if ppw != 0:
-        logging.log(logging.INFO, f'  filter cutoff frequency: {scale_SI(filter_cutoff_f)}Hz ({ppw} PPW)')
+        logging.log(logging.INFO, f"  filter cutoff frequency: {scale_SI(filter_cutoff_f)}Hz ({ppw} PPW)")
     if rppw != 0:
-        logging.log(logging.INFO, 
-            f'  ramp frequency: {scale_SI(2 * np.pi / (2 * ramp_length * kgrid.dt))}Hz (ramp_points_per_wavelength PPW)')
-    logging.log(logging.INFO, '  computation complete.')
+        logging.log(
+            logging.INFO, f"  ramp frequency: {scale_SI(2 * np.pi / (2 * ramp_length * kgrid.dt))}Hz (ramp_points_per_wavelength PPW)"
+        )
+    logging.log(logging.INFO, "  computation complete.")
 
     # plot signals if required
     if plot_signals or plot_spectrums:
         raise NotImplementedError
 
     return filtered_signal
 
 
 def apply_filter(
-        signal: np.ndarray,
-        Fs: float,
-        cutoff_f: float,
-        filter_type: str,
-        zero_phase: Optional[bool] = False,
-        transition_width: Optional[float] = 0.1,
-        stop_band_atten: Optional[int] = 60,
+    signal: np.ndarray,
+    Fs: float,
+    cutoff_f: float,
+    filter_type: str,
+    zero_phase: Optional[bool] = False,
+    transition_width: Optional[float] = 0.1,
+    stop_band_atten: Optional[int] = 60,
 ) -> np.ndarray:
     """
     Filters an input signal using a FIR filter with Kaiser window coefficients based on the specified cut-off frequency and filter type.
     Both causal and zero phase filters can be applied.
 
     Args:
         signal: The input signal.
@@ -573,34 +575,41 @@
 
     Returns:
         The filtered signal.
 
     """
 
     # for a bandpass filter, use applyFilter recursively
-    if filter_type == 'BandPass':
+    if filter_type == "BandPass":
         assert isinstance(cutoff_f, list), "List of two frequencies required as for filter type 'BandPass'"
         assert len(cutoff_f) == 2, "List of two frequencies required as for filter type 'BandPass'"
 
         # apply the low pass filter
-        func_filt_lp = apply_filter(signal, Fs, cutoff_f[1], 'LowPass', stop_band_atten=stop_band_atten,
-                                    transition_width=transition_width, zero_phase=zero_phase)
+        func_filt_lp = apply_filter(
+            signal, Fs, cutoff_f[1], "LowPass", stop_band_atten=stop_band_atten, transition_width=transition_width, zero_phase=zero_phase
+        )
 
         # apply the high pass filter
-        filtered_signal = apply_filter(func_filt_lp, Fs, cutoff_f[0], 'HighPass', stop_band_atten=stop_band_atten,
-                                       transition_width=transition_width, zero_phase=zero_phase)
+        filtered_signal = apply_filter(
+            func_filt_lp,
+            Fs,
+            cutoff_f[0],
+            "HighPass",
+            stop_band_atten=stop_band_atten,
+            transition_width=transition_width,
+            zero_phase=zero_phase,
+        )
 
     else:
-
         # check filter type
-        if filter_type == 'LowPass':
+        if filter_type == "LowPass":
             high_pass = False
-        elif filter_type == 'HighPass':
+        elif filter_type == "HighPass":
             high_pass = True
-            cutoff_f = (Fs / 2 - cutoff_f)
+            cutoff_f = Fs / 2 - cutoff_f
         else:
             raise ValueError(f'Unknown filter type {filter_type}. Options are "LowPass, HighPass, BandPass"')
 
         # make sure input is the correct way around
         m, n = signal.shape
         if m > n:
             signal = signal.T
@@ -616,28 +625,26 @@
         # construct impulse response of ideal bandpass filter h(n), a sinc function
         fc = cutoff_f / Fs  # normalised cut-off
         n = np.arange(-N / 2, N / 2)
         h = 2 * fc * sinc(2 * np.pi * fc * n)
 
         # if no window is given, use a Kaiser window
         # TODO: there is no window argument
-        if 'w' not in locals():
-
+        if "w" not in locals():
             # compute Kaiser window parameter beta
             if stop_band_atten > 50:
                 beta = 0.1102 * (stop_band_atten - 8.7)
             elif stop_band_atten >= 21:
                 beta = 0.5842 * (stop_band_atten - 21) ** 0.4 + 0.07886 * (stop_band_atten - 21)
             else:
                 beta = 0
 
             # construct the Kaiser smoothing window w(n)
             m = np.arange(0, N)
-            w = np.real(scipy.special.iv(0, np.pi * beta * np.sqrt(1 - (2 * m / N - 1) ** 2))) / np.real(
-                scipy.special.iv(0, np.pi * beta))
+            w = np.real(scipy.special.iv(0, np.pi * beta * np.sqrt(1 - (2 * m / N - 1) ** 2))) / np.real(scipy.special.iv(0, np.pi * beta))
 
         # window the ideal impulse response with Kaiser window to obtain the FIR filter coefficients hw(n)
         hw = w * h
 
         # modify to make a high_pass filter
         if high_pass:
             hw = (-1 * np.ones((1, len(hw))) ** (np.arange(1, len(hw) + 1))) * hw
@@ -653,33 +660,30 @@
 
         # remove the part of the signal corresponding to the added zeros
         filtered_signal = filtered_signal[N:]
 
     return filtered_signal[np.newaxis]
 
 
-def smooth(
-        a: np.ndarray,
-        restore_max: Optional[bool] = False,
-        window_type: Optional[str] = 'Blackman') -> np.ndarray:
+def smooth(a: np.ndarray, restore_max: Optional[bool] = False, window_type: Optional[str] = "Blackman") -> np.ndarray:
     """
     Smooths a matrix.
 
     Args:
         a: The spatial distribution to smooth.
         restore_max: Boolean controlling whether the maximum value is restored after smoothing. Defaults to False.
         window_type: Shape of the smoothing window. Any valid inputs to get_win are supported. Defaults to 'Blackman'.
 
     Returns:
         a_sm: The smoothed matrix.
 
     """
 
     DEF_USE_ROTATION = True
-    
+
     if a.dtype == bool:
         a = a.astype(int)
 
     assert is_number(a) and np.all(~np.isinf(a))
     assert isinstance(restore_max, bool)
     assert isinstance(window_type, str)
 
@@ -694,16 +698,16 @@
     # even grid sizes to ensure the DC component of the window has a value of
     # unity
     window_symmetry = (np.array(grid_size) % 2).astype(bool)
 
     # get the window, taking the absolute value to discard machine precision
     # negative values
     from .signals import get_win
-    win, _ = get_win(grid_size, type_=window_type,
-                     rotation=DEF_USE_ROTATION, symmetric=window_symmetry)
+
+    win, _ = get_win(grid_size, type_=window_type, rotation=DEF_USE_ROTATION, symmetric=window_symmetry)
     win = np.abs(win)
 
     # rotate window if input mat is (1, N)
     if a.shape[0] == 1:  # is row?
         win = win.T
 
     # apply the filter
```

### Comparing `k_wave_python-0.3.2/kwave/utils/interp.py` & `k_wave_python-0.3.3/kwave/utils/interp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import numpy as np
 from numpy.fft import fft, fftshift
 from scipy.interpolate import interpn
 from scipy.signal import resample
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Union, List, Tuple, Optional
 
 from .conversion import grid2cart
 from .data import scale_time
 from .matrix import sort_rows
 from .tictoc import TicToc
 
@@ -26,15 +26,15 @@
     Args:
         grid_points: List of 1D or 3D Numpy arrays
         grid_values: A 3D Numpy array which holds values at grid_points
         interp_locs: List of 1D or 3D Numpy arrays
 
     """
 
-    assert len(grid_points) == 3, 'interpolate3D supports only 3D interpolation'
+    assert len(grid_points) == 3, "interpolate3D supports only 3D interpolation"
     assert len(grid_points) == len(interp_locs)
 
     def unpack_and_make_1D(pts):
         pts_x, pts_y, pts_z = pts
         if pts_x.ndim == 3:
             pts_x = pts_x[:, 0, 0]
         if pts_y.ndim == 3:
@@ -43,29 +43,30 @@
             pts_z = pts_z[0, 0, :]
         return pts_x, pts_y, pts_z
 
     g_x, g_y, g_z = unpack_and_make_1D(grid_points)
     q_x, q_y, q_z = unpack_and_make_1D(interp_locs)
 
     # 'ij' indexing is crucial for Matlab compatibility
-    queries = np.array(np.meshgrid(q_x, q_y, q_z, indexing='ij'))
+    queries = np.array(np.meshgrid(q_x, q_y, q_z, indexing="ij"))
     # Queries are just a list of 3D points
     queries = queries.reshape(3, -1).T
 
     # Out of bound points will get NaN values
-    result = interpn((g_x, g_y, g_z), grid_values, queries, method='linear', bounds_error=False, fill_value=np.nan)
+    result = interpn((g_x, g_y, g_z), grid_values, queries, method="linear", bounds_error=False, fill_value=np.nan)
     # Go back from list of interpolated values to 3D volume
     result = result.reshape((g_x.size, g_y.size, g_z.size))
     # set values outside of the interpolation range to original values
     result[np.isnan(result)] = grid_values[np.isnan(result)]
     return result
 
 
-def interpolate2d(grid_points: List[np.ndarray], grid_values: np.ndarray, interp_locs: List[np.ndarray],
-                  method='linear', copy_nans=True) -> np.ndarray:
+def interpolate2d(
+    grid_points: List[np.ndarray], grid_values: np.ndarray, interp_locs: List[np.ndarray], method="linear", copy_nans=True
+) -> np.ndarray:
     """
     Interpolates input grid values at the given locations
     Added by Farid
 
     Matlab version of this function assumes unstructured grid. Interpolating such grid in Python using
     SciPy is very expensive. Thankfully, working with structured grid is fine for our purposes.
     We still support 3D arguments for backward compatibility even though they are mapped to 1D grid.
@@ -75,30 +76,30 @@
         copy_nans:
         grid_points: List of 1D or 3D Numpy arrays
         grid_values: A 3D Numpy array which holds values at grid_points
         interp_locs: List of 1D or 3D Numpy arrays
 
     """
 
-    assert len(grid_points) == 2, 'interpolate2D supports only 2D interpolation'
+    assert len(grid_points) == 2, "interpolate2D supports only 2D interpolation"
     assert len(grid_points) == len(interp_locs)
 
     def unpack_and_make_1D(pts):
         pts_x, pts_y = pts
         if pts_x.ndim == 2:
             pts_x = pts_x[:, 0]
         if pts_y.ndim == 2:
             pts_y = pts_y[0, :]
         return pts_x, pts_y
 
     g_x, g_y = unpack_and_make_1D(grid_points)
     q_x, q_y = unpack_and_make_1D(interp_locs)
 
     # 'ij' indexing is crucial for Matlab compatibility
-    queries = np.array(np.meshgrid(q_x, q_y, indexing='ij'))
+    queries = np.array(np.meshgrid(q_x, q_y, indexing="ij"))
     # Queries are just a list of 3D points
     queries = queries.reshape(2, -1).T
 
     # Out of bound points will get NaN values
     result = interpn((g_x, g_y), grid_values, queries, method=method, bounds_error=False, fill_value=np.nan)
     # Go back from list of interpolated values to 3D volume
     result = result.reshape((q_x.size, q_y.size))
@@ -106,19 +107,15 @@
         assert result.shape == grid_values.shape
         # set values outside of the interpolation range to original values
         result[np.isnan(result)] = grid_values[np.isnan(result)]
     return result
 
 
 def interpolate2d_with_queries(
-        grid_points: List[np.ndarray],
-        grid_values: np.ndarray,
-        queries: np.ndarray,
-        method='linear',
-        copy_nans=True
+    grid_points: List[np.ndarray], grid_values: np.ndarray, queries: np.ndarray, method="linear", copy_nans=True
 ) -> np.ndarray:
     """
     Interpolates input grid values at the given locations
     Added by Farid
 
     Simplified version of `interpolate2D_coords`.
     Expects `interp_locs` to be [N, 2] coordinates of the interpolation locations.
@@ -128,15 +125,15 @@
     Args:
         copy_nans:
         grid_points: List of 1D or 3D Numpy arrays
         grid_values: A 3D Numpy array which holds values at grid_points
         queries: Numpy array with shape [N, 2]
 
     """
-    assert len(grid_points) == 2, 'interpolate2D supports only 2D interpolation'
+    assert len(grid_points) == 2, "interpolate2D supports only 2D interpolation"
 
     g_x, g_y = grid_points
 
     assert g_x.ndim == 1  # is a list
     assert g_y.ndim == 1  # is a list
     assert queries.ndim == 2 and queries.shape[1] == 2
 
@@ -146,18 +143,18 @@
         assert result.shape == grid_values.shape
         # set values outside the interpolation range to original values
         result[np.isnan(result)] = grid_values[np.isnan(result)]
     return result
 
 
 def get_bli(
-        func: np.ndarray,
-        dx: Optional[float] = 1,
-        up_sampling_factor: Optional[int] = 20,
-        plot: Optional[bool] = False,
+    func: np.ndarray,
+    dx: Optional[float] = 1,
+    up_sampling_factor: Optional[int] = 20,
+    plot: Optional[bool] = False,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Calculates the band-limited interpolant of a 1D input function.
 
     Args:
         func: The 1D input function.
         dx: Spatial sampling in meters. Defaults to 1.
@@ -179,111 +176,111 @@
         k_min = -np.pi / dx + dk / 2
         k_max = np.pi / dx - dk / 2
     else:
         # even
         k_min = -np.pi / dx
         k_max = np.pi / dx - dk
 
-    k = np.arange(start=k_min, stop=k_max + dk, step=dk, )
+    k = np.arange(
+        start=k_min,
+        stop=k_max + dk,
+        step=dk,
+    )
     x_fine = np.arange(start=0, stop=((nx - 1) * dx) + dx / up_sampling_factor, step=dx / up_sampling_factor)
 
     func_k = fftshift(fft(func)) / nx
 
     bli = np.real(np.sum(np.matmul(func_k[np.newaxis], np.exp(1j * np.outer(k, x_fine))), axis=0))
     if plot:
         raise NotImplementedError
     return bli, x_fine
 
 
-def interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask, interp='nearest'):
+def interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask, interp="nearest"):
     """
-     Takes a matrix of time-series data recorded over a set
-     of Cartesian sensor points given by cart_sensor_mask and computes the
-     equivalent time-series at each sensor position on the binary sensor
-     mask binary_sensor_mask using interpolation. The properties of
-     binary_sensor_mask are defined by the k-Wave grid object kgrid.
-     Two and three-dimensional data are supported.
-
-     Usage:
-         binary_sensor_data = interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask)
-         binary_sensor_data = interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask, interp)
-
-     Args:
-         kgrid:                k-Wave grid object returned by kWaveGrid
-         cart_sensor_data:     original sensor data measured over
-                              cart_sensor_mask indexed as
-                              cart_sensor_data(sensor position, time)
-         cart_sensor_mask:     Cartesian sensor mask over which
-                              cart_sensor_data is measured
-         binary_sensor_mask:   binary sensor mask at which equivalent
-                              time-series are computed via interpolation
-
-         interp:               (optional) interpolation mode used to compute the
-                              time-series, both 'nearest' and 'linear'
-                              (two-point) modes are supported
-                              (default = 'nearest')
+    Takes a matrix of time-series data recorded over a set
+    of Cartesian sensor points given by cart_sensor_mask and computes the
+    equivalent time-series at each sensor position on the binary sensor
+    mask binary_sensor_mask using interpolation. The properties of
+    binary_sensor_mask are defined by the k-Wave grid object kgrid.
+    Two and three-dimensional data are supported.
+
+    Usage:
+        binary_sensor_data = interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask)
+        binary_sensor_data = interp_cart_data(kgrid, cart_sensor_data, cart_sensor_mask, binary_sensor_mask, interp)
 
-     Returns:
-         array of time-series corresponding to the sensor positions given by binary_sensor_mask
+    Args:
+        kgrid:                k-Wave grid object returned by kWaveGrid
+        cart_sensor_data:     original sensor data measured over
+                             cart_sensor_mask indexed as
+                             cart_sensor_data(sensor position, time)
+        cart_sensor_mask:     Cartesian sensor mask over which
+                             cart_sensor_data is measured
+        binary_sensor_mask:   binary sensor mask at which equivalent
+                             time-series are computed via interpolation
+
+        interp:               (optional) interpolation mode used to compute the
+                             time-series, both 'nearest' and 'linear'
+                             (two-point) modes are supported
+                             (default = 'nearest')
+
+    Returns:
+        array of time-series corresponding to the sensor positions given by binary_sensor_mask
 
     """
 
     # make timer
     timer = TicToc()
     # start the clock
     timer.tic()
 
     # extract the number of data points
     num_cart_data_points, num_time_points = cart_sensor_data.shape
     num_binary_sensor_points = np.sum(binary_sensor_mask.flatten())
 
     # update command line status
-    logging.log(logging.INFO, 'Interpolating Cartesian sensor data...')
-    logging.log(logging.INFO, f'  interpolation mode: {interp}')
-    logging.log(logging.INFO, f'  number of Cartesian sensor points:  {num_cart_data_points}')
-    logging.log(logging.INFO, f'  number of binary sensor points: {num_binary_sensor_points}')
+    logging.log(logging.INFO, "Interpolating Cartesian sensor data...")
+    logging.log(logging.INFO, f"  interpolation mode: {interp}")
+    logging.log(logging.INFO, f"  number of Cartesian sensor points:  {num_cart_data_points}")
+    logging.log(logging.INFO, f"  number of binary sensor points: {num_binary_sensor_points}")
 
     binary_sensor_data = np.zeros((num_binary_sensor_points, num_time_points))
 
     # Check dimensionality of data passed
     if kgrid.dim not in [2, 3]:
-        raise ValueError('Data must be two- or three-dimensional.')
+        raise ValueError("Data must be two- or three-dimensional.")
 
     cart_bsm, _ = grid2cart(kgrid, binary_sensor_mask)
 
     # nearest neighbour interpolation of the data points
     for point_index in range(num_binary_sensor_points):
-
         # find the measured data point that is closest
         dist = np.linalg.norm(cart_bsm[:, point_index] - cart_sensor_mask.T, ord=2, axis=1)
-        if interp == 'nearest':
-
+        if interp == "nearest":
             dist_min_index = np.argmin(dist)
 
             # assign value
             binary_sensor_data[point_index, :] = cart_sensor_data[dist_min_index, :]
 
-        elif interp == 'linear':
+        elif interp == "linear":
             # raise NotImplementedError
             # append the distance information onto the data set
             cart_sensor_data_ro = cart_sensor_data
             np.append(cart_sensor_data_ro, dist[:, None], axis=1)
             new_col_pos = -1
 
             # reorder the data set based on distance information
             cart_sensor_data_ro = sort_rows(cart_sensor_data_ro, new_col_pos)
 
             # linearly interpolate between the two closest points
-            perc = cart_sensor_data_ro[2, new_col_pos] / (
-                    cart_sensor_data_ro[1, new_col_pos] + cart_sensor_data_ro[2, new_col_pos])
-            binary_sensor_data[point_index, :] = perc * cart_sensor_data_ro[1, :] + \
-                                                 (1 - perc) * cart_sensor_data_ro[2, :]
+            perc = cart_sensor_data_ro[2, new_col_pos] / (cart_sensor_data_ro[1, new_col_pos] + cart_sensor_data_ro[2, new_col_pos])
+            binary_sensor_data[point_index, :] = perc * cart_sensor_data_ro[1, :] + (1 - perc) * cart_sensor_data_ro[2, :]
 
         else:
-            raise ValueError('Unknown interpolation option.')
+            raise ValueError("Unknown interpolation option.")
 
         # elif interp == 'linear':
         #
         #         # dist = np.sqrt((cart_bsm[0, point_index] - cart_sensor_mask[0, :])**2 +
         #                                                   (cart_bsm[1, point_index] - cart_sensor_mask[1, :])**2)
         #         # dist = np.linalg.norm(cart_bsm[:, point_index] - cart_sensor_mask.T, axis=1)
         #         # append the distance information onto the data set
@@ -300,61 +297,55 @@
         #         binary_sensor_data[point_index, :] = perc * cart_sensor_data_ro[1, :new_col_pos - 1] +
         #                                                       (1 - perc) * cart_sensor_data_ro[1, :new_col_pos - 1]
         #
         # else:
         #     raise ValueError('Unknown interpolation option.')
 
     # update command line status
-    logging.log(logging.INFO, f'  computation completed in {scale_time(timer.toc())}')
+    logging.log(logging.INFO, f"  computation completed in {scale_time(timer.toc())}")
     return binary_sensor_data
 
 
 def interpftn(x, sz: tuple, win=None):
     """
-     Resamples an N-D matrix to the size given in sz using Fourier interpolation.
+    Resamples an N-D matrix to the size given in sz using Fourier interpolation.
 
 
-     Args:
-         x:           matrix to interpolate
-         sz:          list or tupple of new size
-         win:         (optional) name of windowing function to use
+    Args:
+        x:           matrix to interpolate
+        sz:          list or tupple of new size
+        win:         (optional) name of windowing function to use
 
-     Returns:
-         Resampled matrix
+    Returns:
+        Resampled matrix
 
-     Examples:
-         >>> y = interpftn(x, sz)
-         >>> y = interpftn(x, sz, win)
+    Examples:
+        >>> y = interpftn(x, sz)
+        >>> y = interpftn(x, sz, win)
 
     """
 
     # extract the size of the input matrix
     x_sz = x.shape
 
     # check enough coefficients have been given
     if sum([x != 1 for x in x_sz]) != len(sz):
-        raise ValueError('The number of scaling coefficients must equal the number of dimensions in x.')
+        raise ValueError("The number of scaling coefficients must equal the number of dimensions in x.")
 
     # interpolate for each matrix dimension (dimensions with no interpolation required are skipped)
     y = x
     for p_idx, p in enumerate(sz):
         if p != x_sz[p_idx]:
             y = resample(y, p, axis=p_idx, window=win)
 
     return y
 
 
-@beartype
-def get_delta_bli(
-    Nx: int, 
-    dx: float, 
-    x: np.ndarray, 
-    x0: Union[int, float], 
-    include_imag: bool = False
-) -> np.ndarray:
+@typechecker
+def get_delta_bli(Nx: int, dx: float, x: np.ndarray, x0: Union[int, float], include_imag: bool = False) -> np.ndarray:
     """
     Exact BLI of an arbitrarily positioned delta function.
 
     Calculates the exact Band-Limited Interpolation (BLI) of an arbitrarily positioned delta function.
     For grid dimensions with an evenly-sampled periodicity, a small Nyquist frequency sinusoid is added.
     This sinusoid is invisible on grid samples and has zero amplitude when the delta function lies on a grid node.
     It is important when the evaluation points aren't grid nodes, and when the delta function is off-grid.
@@ -374,15 +365,15 @@
     """
 
     # ignore imaginary component of even function by default
     if include_imag is None:
         include_imag = False
 
     # check whether the grid has even or odd samples per period
-    is_even = (Nx % 2 == 0)
+    is_even = Nx % 2 == 0
 
     # compute BLI
     if is_even:
         # compute periodic sinc function
         f = np.sin(np.pi * (x - x0) / dx) / (Nx * np.tan(np.pi * (x - x0) / (Nx * dx)))
 
         # correct indeterminate points
```

### Comparing `k_wave_python-0.3.2/kwave/utils/io.py` & `k_wave_python-0.3.3/kwave/utils/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import platform
 import socket
 from datetime import datetime
 from typing import Optional
 
 import cv2
@@ -12,51 +11,48 @@
 import kwave
 from .conversion import cast_to_type
 from .data import get_date_string
 from .dotdictionary import dotdict
 
 
 def get_h5_literals():
-    literals = dotdict({
-        # data type
-        'DATA_TYPE_ATT_NAME': 'data_type',
-        'MATRIX_DATA_TYPE_MATLAB': 'single',
-        'MATRIX_DATA_TYPE_C': 'float',
-        'INTEGER_DATA_TYPE_MATLAB': 'uint64',
-        'INTEGER_DATA_TYPE_C': 'long',
-
-        # real / complex
-        'DOMAIN_TYPE_ATT_NAME': 'domain_type',
-        'DOMAIN_TYPE_REAL': 'real',
-        'DOMAIN_TYPE_COMPLEX': 'complex',
-
-        # file descriptors
-        'FILE_MAJOR_VER_ATT_NAME': 'major_version',
-        'FILE_MINOR_VER_ATT_NAME': 'minor_version',
-        'FILE_DESCR_ATT_NAME': 'file_description',
-        'FILE_CREATION_DATE_ATT_NAME': 'creation_date',
-        'CREATED_BY_ATT_NAME': 'created_by',
-
-        # file type
-        'FILE_TYPE_ATT_NAME': 'file_type',
-        'HDF_INPUT_FILE': 'input',
-        'HDF_OUTPUT_FILE': 'output',
-        'HDF_CHECKPOINT_FILE': 'checkpoint',
-
-        # file version information
-        'HDF_FILE_MAJOR_VERSION': '1',
-        'HDF_FILE_MINOR_VERSION': '2',
-
-        # compression level
-        'HDF_COMPRESSION_LEVEL': 0
-    })
+    literals = dotdict(
+        {
+            # data type
+            "DATA_TYPE_ATT_NAME": "data_type",
+            "MATRIX_DATA_TYPE_MATLAB": "single",
+            "MATRIX_DATA_TYPE_C": "float",
+            "INTEGER_DATA_TYPE_MATLAB": "uint64",
+            "INTEGER_DATA_TYPE_C": "long",
+            # real / complex
+            "DOMAIN_TYPE_ATT_NAME": "domain_type",
+            "DOMAIN_TYPE_REAL": "real",
+            "DOMAIN_TYPE_COMPLEX": "complex",
+            # file descriptors
+            "FILE_MAJOR_VER_ATT_NAME": "major_version",
+            "FILE_MINOR_VER_ATT_NAME": "minor_version",
+            "FILE_DESCR_ATT_NAME": "file_description",
+            "FILE_CREATION_DATE_ATT_NAME": "creation_date",
+            "CREATED_BY_ATT_NAME": "created_by",
+            # file type
+            "FILE_TYPE_ATT_NAME": "file_type",
+            "HDF_INPUT_FILE": "input",
+            "HDF_OUTPUT_FILE": "output",
+            "HDF_CHECKPOINT_FILE": "checkpoint",
+            # file version information
+            "HDF_FILE_MAJOR_VERSION": "1",
+            "HDF_FILE_MINOR_VERSION": "2",
+            # compression level
+            "HDF_COMPRESSION_LEVEL": 0,
+        }
+    )
     return literals
 
 
-def write_matrix(filename, matrix: np.ndarray, matrix_name: str, compression_level:int =None, auto_chunk: bool =True):
+def write_matrix(filename, matrix: np.ndarray, matrix_name: str, compression_level: int = None, auto_chunk: bool = True):
     # get literals
     h5_literals = get_h5_literals()
 
     assert isinstance(auto_chunk, bool), "auto_chunk must be a boolean."
 
     if compression_level is None:
         compression_level = h5_literals.HDF_COMPRESSION_LEVEL
@@ -83,81 +79,76 @@
         # set chunk size to Nx * Ny
         chunk_size = [Nx, Ny, 1]
     elif dims == 2:
         # set chunk size to Nx
         chunk_size = [Nx, 1, 1]
     elif dims <= 1:
         # check that the matrix size is greater than 1 MB
-        one_mb = (1024 ** 2) / 8
+        one_mb = (1024**2) / 8
         if matrix.size > one_mb:
             # set chunk size to 1 MB
             if Nx > Ny:
                 chunk_size = [one_mb, 1, 1]
             elif Ny > Nz:
                 chunk_size = [1, one_mb, 1]
             else:
                 chunk_size = [1, 1, one_mb]
         else:
-
             # set no compression
             compression_level = 0
 
             # set chunk size to grid size
             if matrix.size == 1:
                 chunk_size = (1, 1, 1)
             elif Nx > Ny:
                 chunk_size = (Nx, 1, 1)
             elif Ny > Nz:
                 chunk_size = (1, Ny, 1)
             else:
                 chunk_size = (1, 1, Nz)
     else:
         # throw error for unknown matrix size
-        raise ValueError('Input matrix must have 1, 2 or 3 dimensions.')
+        raise ValueError("Input matrix must have 1, 2 or 3 dimensions.")
 
     # check the format of the matrix is either single precision (float in C++)
     # or uint64 (unsigned long in C++)
     if matrix.dtype == np.float32:
         # set data type flags
         data_type_matlab = h5_literals.MATRIX_DATA_TYPE_MATLAB
         data_type_c = h5_literals.MATRIX_DATA_TYPE_C
     elif matrix.dtype == np.uint64:
-
         # set data type flags
         data_type_matlab = h5_literals.INTEGER_DATA_TYPE_MATLAB
         data_type_c = h5_literals.INTEGER_DATA_TYPE_C
 
     else:
         # throw error for unknown data type
-        raise ValueError('Input matrix must be of type ''single'' or ''uint64''.')
+        raise ValueError("Input matrix must be of type " "single" " or " "uint64" ".")
 
     # check if the input matrix is real or complex, if complex, rearrange the
     # data in the C++ format
     if np.isreal(matrix).all():
-
         # set file tag
-        domain_type = 'real'  # DOMAIN_TYPE_REAL
+        domain_type = "real"  # DOMAIN_TYPE_REAL
 
     elif dims == 3:
-
         # set file tag
         domain_type = h5_literals.DOMAIN_TYPE_COMPLEX
 
         # rearrange the data so the real and imaginary parts are stored in the
         # same matrix
         matrix = np.concatenate(matrix.real, matrix.imag, axis=0)
         matrix = matrix.reshape((Nx, 2, Ny, Nz))
         matrix = np.transpose(matrix, (1, 0, 2, 3))
         matrix = matrix.reshape((2 * Nx, Ny, Nz))
 
         # update the size of Nx
         Nx = 2 * Nx
 
     elif dims <= 1:
-
         # set file tag
         domain_type = h5_literals.DOMAIN_TYPE_COMPLEX
 
         # rearrange the data so the real and imaginary parts are stored in the
         # same matrix
         nelems = matrix.size
         matrix = matrix.reshape((nelems, 1))
@@ -174,34 +165,30 @@
         if Nx == 1 and Ny == 1 and Nz == 1:
             Nx = 2 * Nx
 
         # put in correct dimension
         matrix = matrix.reshape((Nx, Ny, Nz))
 
     else:
-        raise NotImplementedError('Currently there is no support for saving 2D complex matrices.')
+        raise NotImplementedError("Currently there is no support for saving 2D complex matrices.")
 
     # allocate a holder for the new matrix within the file
-    opts = {
-        'dtype': data_type_matlab,
-        'chunks': auto_chunk if auto_chunk is True else tuple(chunk_size)
-    }
-    
+    opts = {"dtype": data_type_matlab, "chunks": auto_chunk if auto_chunk is True else tuple(chunk_size)}
+
     if compression_level != 0:
         # use compression
-        opts['compression'] = compression_level
+        opts["compression"] = compression_level
 
     # write the matrix into the file
     with h5py.File(filename, "a") as f:
-        f.create_dataset(f'/{matrix_name}', [Nx, Ny, Nz], data=matrix, **opts)
+        f.create_dataset(f"/{matrix_name}", [Nx, Ny, Nz], data=matrix, **opts)
 
         # set attributes for the matrix (used by k-Wave++)
-        assign_str_attr(f[f'/{matrix_name}'].attrs, h5_literals.DOMAIN_TYPE_ATT_NAME, domain_type)
-        assign_str_attr(f[f'/{matrix_name}'].attrs, h5_literals.DATA_TYPE_ATT_NAME, data_type_c)
-
+        assign_str_attr(f[f"/{matrix_name}"].attrs, h5_literals.DOMAIN_TYPE_ATT_NAME, domain_type)
+        assign_str_attr(f[f"/{matrix_name}"].attrs, h5_literals.DATA_TYPE_ATT_NAME, data_type_c)
 
 
 def write_attributes(filename: str, file_description: Optional[str] = None) -> None:
     """
     Write attributes to a HDF5 file.
 
     This function writes attributes to a HDF5 file using a deprecated legacy method if legacy is set to True, or a new
@@ -209,47 +196,47 @@
     file_description is not provided, a default file description will be used.
 
     Args:
         filename: The name of the HDF5 file.
         file_description: The description of the file. If not provided, a default description
             will be used.
 
-    Raises:
-        DeprecationWarning: If legacy is set to True, a DeprecationWarning will be raised.
-
     """
 
-    logging.log(logging.WARN, f'{DeprecationWarning.__name__}: Attributes will soon be typed when saved and not saved ')
     # get literals
     h5_literals = get_h5_literals()
 
     # get computer infor
-    comp_info = dotdict({
-        'date': datetime.now().strftime("%d-%b-%Y"),
-        'computer_name': socket.gethostname(),
-        'operating_system_type': platform.system(),
-        'operating_system': platform.system() + " " + platform.release() + " " + platform.version(),
-        'user_name': os.environ.get('USERNAME'),
-        'matlab_version': 'N/A',
-        'kwave_version': '1.3',
-        'kwave_path': 'N/A',
-    })
+    comp_info = dotdict(
+        {
+            "date": datetime.now().strftime("%d-%b-%Y"),
+            "computer_name": socket.gethostname(),
+            "operating_system_type": platform.system(),
+            "operating_system": platform.system() + " " + platform.release() + " " + platform.version(),
+            "user_name": os.environ.get("USERNAME"),
+            "matlab_version": "N/A",
+            "kwave_version": "1.3",
+            "kwave_path": "N/A",
+        }
+    )
 
     # set file description if not provided by user
     if file_description is None:
-        file_description = f'Input data created by {comp_info.user_name} running MATLAB ' \
-                           f'{comp_info.matlab_version} on {comp_info.operating_system_type}'
+        file_description = (
+            f"Input data created by {comp_info.user_name} running MATLAB "
+            f"{comp_info.matlab_version} on {comp_info.operating_system_type}"
+        )
 
     # set additional file attributes
     with h5py.File(filename, "a") as f:
         # create a dictionary of attributes
         attributes = {
             h5_literals.FILE_MAJOR_VER_ATT_NAME: h5_literals.HDF_FILE_MAJOR_VERSION,
             h5_literals.FILE_MINOR_VER_ATT_NAME: h5_literals.HDF_FILE_MINOR_VERSION,
-            h5_literals.CREATED_BY_ATT_NAME: f'k-Wave {kwave.VERSION}',
+            h5_literals.CREATED_BY_ATT_NAME: f"k-Wave {kwave.VERSION}",
             h5_literals.FILE_DESCR_ATT_NAME: file_description,
             h5_literals.FILE_TYPE_ATT_NAME: h5_literals.HDF_INPUT_FILE,
             h5_literals.FILE_CREATION_DATE_ATT_NAME: get_date_string(),
         }
         # loop through the attributes dictionary and assign each attribute to the file
         for key, value in attributes.items():
             assign_str_attr(f.attrs, key, value)
@@ -296,101 +283,108 @@
     Args:
         filename:
 
     """
 
     # h5_literals = get_h5_literals()
 
-    with h5py.File(filename, 'r') as hf:
+    with h5py.File(filename, "r") as hf:
         names = hf.keys()
 
         v_list = [
-            ('ux_source', 'u_source_many'),
-            ('uy_source', 'u_source_many'),
-            ('uz_source', 'u_source_many'),
-
-            ('sxx_source', 's_source_many'),
-            ('syy_source', 's_source_many'),
-            ('szz_source', 's_source_many'),
-            ('sxy_source', 's_source_many'),
-            ('sxz_source', 's_source_many'),
-            ('syz_source', 's_source_many'),
-
-            ('p_source', 'p_source_many')
+            ("ux_source", "u_source_many"),
+            ("uy_source", "u_source_many"),
+            ("uz_source", "u_source_many"),
+            ("sxx_source", "s_source_many"),
+            ("syy_source", "s_source_many"),
+            ("szz_source", "s_source_many"),
+            ("sxy_source", "s_source_many"),
+            ("sxz_source", "s_source_many"),
+            ("syz_source", "s_source_many"),
+            ("p_source", "p_source_many"),
         ]
         variable_list = {}
         for prefix, many_flag_key in v_list:
-            inp_name = f'{prefix}_input'
-            flag_name = f'{prefix}_flag'
+            inp_name = f"{prefix}_input"
+            flag_name = f"{prefix}_flag"
             if inp_name in names:
                 variable_list[flag_name] = hf[inp_name].shape[1]
 
                 variable_list[many_flag_key] = hf[inp_name].shape[0] != 1
             else:
                 variable_list[flag_name] = 0
 
         # --------------------
         # u source
         # --------------------
 
         # write u_source mode if not already in file (1 is Additive, 0 is Dirichlet)
-        if any(variable_list[flag] for flag in ['ux_source_flag', 'uy_source_flag', 'uz_source_flag']) \
-                and 'u_source_mode' not in names:
-            variable_list['u_source_mode'] = 1
+        if any(variable_list[flag] for flag in ["ux_source_flag", "uy_source_flag", "uz_source_flag"]) and "u_source_mode" not in names:
+            variable_list["u_source_mode"] = 1
 
         # --------------------
         # s source
         # --------------------
 
         # write s_source mode if not already in file (1 is Additive, 0 is Dirichlet)
-        if any(variable_list[flag] for flag in ['sxx_source_flag', 'syy_source_flag', 'szz_source_flag',
-                                                'sxy_source_flag', 'sxz_source_flag', 'syz_source_flag']) \
-                and 's_source_mode' not in names:
-            variable_list['s_source_mode'] = 1
+        if (
+            any(
+                variable_list[flag]
+                for flag in [
+                    "sxx_source_flag",
+                    "syy_source_flag",
+                    "szz_source_flag",
+                    "sxy_source_flag",
+                    "sxz_source_flag",
+                    "syz_source_flag",
+                ]
+            )
+            and "s_source_mode" not in names
+        ):
+            variable_list["s_source_mode"] = 1
 
         # --------------------
         # p source
         # --------------------
 
         # write p_source mode if not already in file (1 is Additive, 0 is Dirichlet)
-        if any(variable_list[flag] for flag in ['p_source_flag']) \
-                and 'p_source_mode' not in names:
-            variable_list['p_source_mode'] = 1
+        if any(variable_list[flag] for flag in ["p_source_flag"]) and "p_source_mode" not in names:
+            variable_list["p_source_mode"] = 1
 
         # check for p0_source_input and set p0_source_flag
-        variable_list['p0_source_flag'] = 'p0_source_input' in names
+        variable_list["p0_source_flag"] = "p0_source_input" in names
 
         # --------------------
         # additional flags
         # --------------------
         # check for transducer_source_input and set transducer_source_flag
-        variable_list['transducer_source_flag'] = 'transducer_source_input' in names
+        variable_list["transducer_source_flag"] = "transducer_source_input" in names
 
         # check for BonA and set nonlinear flag
-        variable_list['nonlinear_flag'] = 'BonA' in names
+        variable_list["nonlinear_flag"] = "BonA" in names
 
         # check for alpha_coeff and set absorbing flag
-        variable_list['absorbing_flag'] = 'alpha_coeff' in names
+        variable_list["absorbing_flag"] = "alpha_coeff" in names
 
         # check for lambda and set elastic flag
-        variable_list['elastic_flag'] = 'lambda' in names
+        variable_list["elastic_flag"] = "lambda" in names
 
         # set axisymmetric grid flag to false
-        variable_list['axisymmetric_flag'] = 0
+        variable_list["axisymmetric_flag"] = 0
 
         # set nonuniform grid flag to false
-        variable_list['nonuniform_grid_flag'] = 0
+        variable_list["nonuniform_grid_flag"] = 0
 
         # check for sensor_mask_index and sensor_mask_corners
-        if 'sensor_mask_index' in names:
-            variable_list['sensor_mask_type'] = 0
-        elif 'sensor_mask_corners' in names:
-            variable_list['sensor_mask_type'] = 1
+        if "sensor_mask_index" in names:
+            variable_list["sensor_mask_type"] = 0
+        elif "sensor_mask_corners" in names:
+            variable_list["sensor_mask_type"] = 1
         else:
-            raise ValueError('Either sensor_mask_index or sensor_mask_corners must be defined in the input file')
+            raise ValueError("Either sensor_mask_index or sensor_mask_corners must be defined in the input file")
 
     # --------------------
     # write flags to file
     # --------------------
 
     # change all the index variables to be in 64-bit unsigned integers (long in C++) and write to file
     for key, value in variable_list.items():
@@ -398,51 +392,51 @@
         value = np.array(value, dtype=np.uint64)
         write_matrix(filename, value, key)
         del value
 
 
 def write_grid(filename, grid_size, grid_spacing, pml_size, pml_alpha, Nt, dt, c_ref):
     """
-     Creates and writes the wavenumber grids and PML variables
-     required by the k-Wave C++ code to the HDF5 file specified by the
-     user.
-
-         List of parameters that are written:
-             Nx
-             Ny
-             Nz
-             Nt
-             dt
-             dx
-             dy
-             dz
-             c_ref
-             pml_x_alpha
-             pml_y_alpha
-             pml_z_alpha
-             pml_x_size
-             pml_y_size
-             pml_z_size
+    Creates and writes the wavenumber grids and PML variables
+    required by the k-Wave C++ code to the HDF5 file specified by the
+    user.
+
+        List of parameters that are written:
+            Nx
+            Ny
+            Nz
+            Nt
+            dt
+            dx
+            dy
+            dz
+            c_ref
+            pml_x_alpha
+            pml_y_alpha
+            pml_z_alpha
+            pml_x_size
+            pml_y_size
+            pml_z_size
 
     """
 
     h5_literals = get_h5_literals()
 
     # =========================================================================
     # STORE FLOATS
     # =========================================================================
     variable_list = {
-        'dt': dt,
-        'dx': grid_spacing[0],
-        'dy': grid_spacing[1],
-        'dz': grid_spacing[2],
-        'pml_x_alpha': pml_alpha[0],
-        'pml_y_alpha': pml_alpha[1],
-        'pml_z_alpha': pml_alpha[2],
-        'c_ref': c_ref
+        "dt": dt,
+        "dx": grid_spacing[0],
+        "dy": grid_spacing[1],
+        "dz": grid_spacing[2],
+        "pml_x_alpha": pml_alpha[0],
+        "pml_y_alpha": pml_alpha[1],
+        "pml_z_alpha": pml_alpha[2],
+        "c_ref": c_ref,
     }
 
     # change float variables to be in single precision (float in C++), then add to HDF5 file
     for key, value in variable_list.items():
         # cast matrix to single precision
         value = cast_to_type(value, h5_literals.MATRIX_DATA_TYPE_MATLAB)
         write_matrix(filename, value, key)
@@ -450,21 +444,21 @@
 
     # =========================================================================
     # STORE INTEGERS
     # =========================================================================
 
     # integer variables
     variable_list = {
-        'Nx': grid_size[0],
-        'Ny': grid_size[1],
-        'Nz': grid_size[2],
-        'Nt': Nt,
-        'pml_x_size': pml_size[0],
-        'pml_y_size': pml_size[1],
-        'pml_z_size': pml_size[2]
+        "Nx": grid_size[0],
+        "Ny": grid_size[1],
+        "Nz": grid_size[2],
+        "Nt": Nt,
+        "pml_x_size": pml_size[0],
+        "pml_y_size": pml_size[1],
+        "pml_z_size": pml_size[2],
     }
 
     # change all the index variables to be in 64-bit unsigned integers (long in C++)
     for key, value in variable_list.items():
         # cast matrix to 64-bit unsigned integer
         value = cast_to_type(value, h5_literals.INTEGER_DATA_TYPE_MATLAB)
         write_matrix(filename, value, key)
@@ -477,15 +471,15 @@
 
     Args:
         attrs: HDF5 attribute object
         attr_name: name of attribute
         attr_val: value of attribute
 
     """
-    attrs.create(attr_name, attr_val, None, dtype=f'<S{len(attr_val)}')
+    attrs.create(attr_name, attr_val, None, dtype=f"<S{len(attr_val)}")
 
 
 def load_image(path, is_gray):
     if is_gray:
         img = cv2.imread(path, cv2.IMREAD_GRAYSCALE)
     else:
         img = cv2.imread(path, cv2.IMREAD_COLOR)
```

### Comparing `k_wave_python-0.3.2/kwave/utils/kwave_array.py` & `k_wave_python-0.3.3/kwave/utils/kwave_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 import time
 from dataclasses import dataclass
 from math import ceil
-from typing import Iterable, Optional
+from typing import Optional
 
 import numpy as np
 from numpy import arcsin, pi, cos, size, array
 from numpy.linalg import linalg
 
-import kwave
+from kwave.data import Vector
 from kwave.kgrid import kWaveGrid
 from kwave.utils.conversion import tol_star
 from kwave.utils.interp import get_delta_bli
-from kwave.utils.mapgen import trim_cart_points, make_cart_rect, make_cart_arc, make_cart_bowl, make_cart_disc, \
-    make_cart_spherical_segment
+from kwave.utils.mapgen import trim_cart_points, make_cart_rect, make_cart_arc, make_cart_bowl, make_cart_disc, make_cart_spherical_segment
 from kwave.utils.math import sinc, get_affine_matrix
 from kwave.utils.matlab import matlab_assign, matlab_mask, matlab_find
 
 
 @dataclass
 class Element:
     group_id: int
@@ -33,15 +32,15 @@
     inner_diameter: Optional[float] = None
     outer_diameter: Optional[float] = None
     diameter: Optional[float] = None
 
     radius_of_curvature: Optional[float] = None
     position: Optional[np.ndarray] = None
     focus_position: Optional[np.ndarray] = None
-    
+
     # custom element
     integration_points: Optional[np.ndarray] = None
 
     length: Optional[float] = None
     width: Optional[float] = None
     orientation: Optional[np.ndarray] = None
 
@@ -82,23 +81,24 @@
                 self.end_point = [self.end_point]
             self.end_point = np.array(self.end_point, dtype=float)
 
         self.measure = round(float(self.measure), 8)
 
 
 class kWaveArray(object):
-
-    def __init__(self,
-                 axisymmetric: bool = False,
-                 bli_tolerance: float = 0.05,
-                 bli_type: str = 'sinc',
-                 single_precision: bool = False,
-                 upsampling_rate: int = 10):
+    def __init__(
+        self,
+        axisymmetric: bool = False,
+        bli_tolerance: float = 0.05,
+        bli_type: str = "sinc",
+        single_precision: bool = False,
+        upsampling_rate: int = 10,
+    ):
         assert 0 <= bli_tolerance <= 1
-        assert bli_type in ['exact', 'sinc']
+        assert bli_type in ["exact", "sinc"]
 
         self.axisymmetric = axisymmetric
         self.bli_tolerance = bli_tolerance
         self.bli_type = bli_type
         self.single_precision = single_precision
         self.upsampling_rate = upsampling_rate
 
@@ -109,15 +109,14 @@
         self.array_transformation = []
 
         self.use_spiral_disc_points = 0
         self.num_arc_plot_points = 100
         self.element_plot_colour = np.array([0, 158, 194], dtype=float) / 255
 
     def add_annular_array(self, position, radius, diameters, focus_pos):
-
         assert isinstance(position, (list, tuple)), "'position' must be list or tuple"
         assert isinstance(radius, (int, float)), "'radius' must be an integer or float"
         assert isinstance(diameters, (list, tuple)), "'diameters' must be list or tuple"
         assert isinstance(focus_pos, (list, tuple)), "'focus_pos' must be list or tuple"
         assert len(position) == 3, "'position' must have 3 elements"
         assert len(focus_pos) == 3, "'focus_pos' must have 3 elements"
         assert all(len(i) == 2 for i in diameters), "'diameters' must be a list of lists, each with 2 elements"
@@ -134,34 +133,33 @@
 
         for el_ind in range(annular_array_num_el):
             self.number_elements += 1
 
             varphi_min = arcsin(diameters[el_ind][0] / (2 * radius))
             varphi_max = arcsin(diameters[el_ind][1] / (2 * radius))
 
-            area = 2 * pi * radius ** 2 * (1 - cos(varphi_max)) - 2 * pi * radius ** 2 * (1 - cos(varphi_min))
+            area = 2 * pi * radius**2 * (1 - cos(varphi_max)) - 2 * pi * radius**2 * (1 - cos(varphi_min))
 
             element = Element(
                 group_id=self.number_groups,
-                group_type='annular_array',
+                group_type="annular_array",
                 element_number=el_ind + 1,
-                type='annulus',
+                type="annulus",
                 dim=2,
                 position=array(position),
                 radius_of_curvature=radius,
                 inner_diameter=diameters[el_ind][0],
                 outer_diameter=diameters[el_ind][1],
                 focus_position=array(focus_pos),
                 active=True,
-                measure=area
+                measure=area,
             )
             self.elements.append(element)
 
     def add_annular_element(self, position, radius, diameters, focus_pos):
-
         assert isinstance(position, (list, tuple)), "'position' must be list or tuple"
         assert isinstance(radius, (int, float)), "'radius' must be an integer or float"
         assert isinstance(diameters, (list, tuple)), "'diameters' must be list or tuple"
         assert isinstance(focus_pos, (list, tuple)), "'focus_pos' must be list or tuple"
         assert len(position) == 3, "'position' must have 3 elements"
         assert len(focus_pos) == 3, "'focus_pos' must have 3 elements"
         assert len(diameters) == 2, "'diameters' must have 2 elements"
@@ -173,31 +171,32 @@
             raise ValueError(f"3D annular array cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
 
         varphi_min = arcsin(diameters[0] / (2 * radius))
         varphi_max = arcsin(diameters[1] / (2 * radius))
 
-        area = 2 * pi * radius ** 2 * (1 - cos(varphi_max)) - 2 * pi * radius ** 2 * (1 - cos(varphi_min))
+        area = 2 * pi * radius**2 * (1 - cos(varphi_max)) - 2 * pi * radius**2 * (1 - cos(varphi_min))
 
-        self.elements.append(Element(
-            group_id=0,
-            type='annulus',
-            dim=2,
-            position=array(position),
-            radius_of_curvature=radius,
-            inner_diameter=diameters[0],
-            outer_diameter=diameters[1],
-            focus_position=array(focus_pos),
-            active=True,
-            measure=area
-        ))
+        self.elements.append(
+            Element(
+                group_id=0,
+                type="annulus",
+                dim=2,
+                position=array(position),
+                radius_of_curvature=radius,
+                inner_diameter=diameters[0],
+                outer_diameter=diameters[1],
+                focus_position=array(focus_pos),
+                active=True,
+                measure=area,
+            )
+        )
 
     def add_bowl_element(self, position, radius, diameter, focus_pos):
-
         assert isinstance(position, (list, tuple)), "'position' must be list or tuple"
         assert isinstance(radius, (int, float)), "'radius' must be an integer or float"
         assert isinstance(diameter, (int, float)), "'diameter' must be an integer or float"
         assert isinstance(focus_pos, (list, tuple)), "'focus_pos' must be list or tuple"
         assert len(position) == 3, "'position' must have 3 elements"
         assert len(focus_pos) == 3, "'focus_pos' must have 3 elements"
 
@@ -207,110 +206,102 @@
         if self.dim != 3:
             raise ValueError(f"3D bowl element cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
 
         varphi_max = arcsin(diameter / (2 * radius))
 
-        area = 2 * pi * radius ** 2 * (1 - cos(varphi_max))
+        area = 2 * pi * radius**2 * (1 - cos(varphi_max))
+
+        self.elements.append(
+            Element(
+                group_id=0,
+                type="bowl",
+                dim=2,
+                position=array(position),
+                radius_of_curvature=radius,
+                diameter=diameter,
+                focus_position=array(focus_pos),
+                active=True,
+                measure=area,
+            )
+        )
 
-        self.elements.append(Element(
-            group_id=0,
-            type='bowl',
-            dim=2,
-            position=array(position),
-            radius_of_curvature=radius,
-            diameter=diameter,
-            focus_position=array(focus_pos),
-            active=True,
-            measure=area
-        ))
-        
     def add_custom_element(self, integration_points, measure, element_dim, label):
-        
         assert isinstance(integration_points, (np.ndarray)), "'integration_points' must be a numpy array"
         assert isinstance(measure, (int, float)), "'measure' must be an integer or float"
         assert isinstance(element_dim, (int)) and element_dim in [1, 2, 3], "'element_dim' must be an integer and either 1, 2 or 3"
         assert isinstance(label, (str)), "'label' must be a string"
-        
+
         # check the dimensionality of the integration points
         input_dim = integration_points.shape[0]
         if (input_dim < 1) or (input_dim > 3):
             raise ValueError("Input integration_points must be a 1 x N (in 1D), 2 x N (in 2D), or 3 x N (in 3D) array.")
 
         # check if this is the first element, and set the dimension
         if self.number_elements == 0:
             self.dim = input_dim
-        
+
         # check that the element is being added to an array with the
         # correct dimensions
         if self.dim != input_dim:
             raise ValueError(f"{input_dim}D custom element cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
-        
+
         self.elements.append(
             Element(
-                group_id=0,
-                type='custom',
-                dim=element_dim,
-                label=label,
-                integration_points=integration_points,
-                active=True,
-                measure=measure
+                group_id=0, type="custom", dim=element_dim, label=label, integration_points=integration_points, active=True, measure=measure
             )
         )
-        
-        
-    def add_rect_element(self, position, Lx, Ly, theta):
 
+    def add_rect_element(self, position, Lx, Ly, theta):
         assert isinstance(position, (list, tuple)), "'position' must be a list or tuple"
         assert isinstance(Lx, (int, float)), "'Lx' must be an integer or float"
         assert isinstance(Ly, (int, float)), "'Ly' must be an integer or float"
 
         coord_dim = len(position)
 
         if coord_dim not in [2, 3]:
-            raise ValueError(
-                "Input position for rectangular element must be specified as a 2 (2D) or 3 (3D) element array.")
+            raise ValueError("Input position for rectangular element must be specified as a 2 (2D) or 3 (3D) element array.")
 
         if coord_dim == 3:
-            assert isinstance(theta, (kwave.data.Vector, list, tuple)) and len(
-                theta) == 3, "'theta' must be a list or tuple of length 3"
+            assert isinstance(theta, (Vector, list, tuple)) and len(theta) == 3, "'theta' must be a list or tuple of length 3"
         else:
             assert isinstance(theta, (int, float)), "'theta' must be an integer or float"
 
         if self.number_elements == 0:
             self.dim = coord_dim
 
         if self.dim != coord_dim:
             raise ValueError(f"{coord_dim}D rectangular element cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
 
         area = Lx * Ly
 
-        self.elements.append(Element(
-            group_id=0,
-            type='rect',
-            dim=2,
-            position=array(position),
-            length=Lx,
-            width=Ly,
-            orientation=array(theta) if coord_dim == 3 else theta,
-            active=True,
-            measure=area
-        ))
+        self.elements.append(
+            Element(
+                group_id=0,
+                type="rect",
+                dim=2,
+                position=array(position),
+                length=Lx,
+                width=Ly,
+                orientation=array(theta) if coord_dim == 3 else theta,
+                active=True,
+                measure=area,
+            )
+        )
 
     def add_arc_element(self, position, radius, diameter, focus_pos):
-
-        assert isinstance(position, Iterable), "'position' must be list, tuple or Vector"
+        assert isinstance(position, (list, tuple, Vector)), "'position' must be list, tuple or Vector"
         assert isinstance(radius, (int, float)), "'radius' must be an integer or float"
         assert isinstance(diameter, (int, float)), "'diameter' must be an integer or float"
-        assert isinstance(focus_pos, Iterable), "'focus_pos' must be list, tuple or Vector"
+        assert isinstance(focus_pos, (list, tuple, Vector)), "'focus_pos' must be list, tuple or Vector"
         assert len(position) == 2, "'position' must have 2 elements"
         assert len(focus_pos) == 2, "'focus_pos' must have 2 elements"
 
         if self.number_elements == 0:
             self.dim = 2
 
         if self.dim != 2:
@@ -318,74 +309,74 @@
 
         self.number_elements += 1
 
         varphi_max = arcsin(diameter / (2 * radius))
 
         length = 2 * radius * varphi_max
 
-        self.elements.append(Element(
-            group_id=0,
-            type='arc',
-            dim=1,
-            position=array(position),
-            radius_of_curvature=radius,
-            diameter=diameter,
-            focus_position=array(focus_pos),
-            active=True,
-            measure=length
-        ))
+        self.elements.append(
+            Element(
+                group_id=0,
+                type="arc",
+                dim=1,
+                position=array(position),
+                radius_of_curvature=radius,
+                diameter=diameter,
+                focus_position=array(focus_pos),
+                active=True,
+                measure=length,
+            )
+        )
 
     def add_disc_element(self, position, diameter, focus_pos=None):
-
         assert isinstance(position, (list, tuple)), "'position' must be a list or tuple"
         assert isinstance(diameter, (int, float)), "'diameter' must be an integer or float"
 
         coord_dim = len(position)
 
         if coord_dim not in [2, 3]:
             raise ValueError("Input position for disc element must be specified as a 2 (2D) or 3 (3D) element array.")
 
         if coord_dim == 3:
-            assert isinstance(focus_pos, (list, tuple)) and len(
-                focus_pos) == 3, "'focus_pos' must be a list or tuple of length 3"
+            assert isinstance(focus_pos, (list, tuple)) and len(focus_pos) == 3, "'focus_pos' must be a list or tuple of length 3"
         else:
             focus_pos = []
 
         if self.number_elements == 0:
             self.dim = coord_dim
 
         if self.dim != coord_dim:
             raise ValueError(f"{coord_dim}D disc element cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
 
         area = pi * (diameter / 2) ** 2
 
-        self.elements.append(Element(
-            group_id=0,
-            type='disc',
-            dim=2,
-            position=array(position),
-            diameter=diameter,
-            focus_position=array(focus_pos),
-            active=True,
-            measure=area
-        ))
+        self.elements.append(
+            Element(
+                group_id=0,
+                type="disc",
+                dim=2,
+                position=array(position),
+                diameter=diameter,
+                focus_position=array(focus_pos),
+                active=True,
+                measure=area,
+            )
+        )
 
     def remove_element(self, element_num):
-
         if element_num > self.number_elements:
             raise ValueError(f"Cannot remove element {element_num} from array with {self.number_elements} elements.")
 
         self.elements.pop(element_num)
 
         self.number_elements -= 1
 
     def add_line_element(self, start_point, end_point):
-
         assert isinstance(start_point, (list, tuple)), "'start_point' must be a list or tuple"
         assert isinstance(end_point, (list, tuple)), "'end_point' must be a list or tuple"
 
         input_dim = len(start_point)
 
         if input_dim not in [1, 2, 3]:
             raise ValueError("Input start_point must have 1 (in 1D), 2 (in 2D), or 3 (in 3D) elements.")
@@ -399,38 +390,41 @@
         if self.dim != input_dim:
             raise ValueError(f"{input_dim}D line element cannot be added to an array with {self.dim}D elements.")
 
         self.number_elements += 1
 
         line_length = linalg.norm(array(end_point) - array(start_point))
 
-        self.elements.append(Element(
-            group_id=0,
-            type='line',
-            dim=1,
-            start_point=array(start_point),
-            end_point=array(end_point),
-            active=True,
-            measure=line_length
-        ))
+        self.elements.append(
+            Element(
+                group_id=0, type="line", dim=1, start_point=array(start_point), end_point=array(end_point), active=True, measure=line_length
+            )
+        )
 
     def get_element_grid_weights(self, kgrid, element_num):
         return self.get_off_grid_points(kgrid, element_num, False)
 
     def get_element_binary_mask(self, kgrid, element_num):
         return self.get_off_grid_points(kgrid, element_num, True)
 
     def get_array_grid_weights(self, kgrid):
         self.check_for_elements()
 
-        grid_weights = np.zeros((kgrid.Nx, kgrid.Ny, max(kgrid.Nz, 1)))
+        if kgrid.Nz >= 1:
+            grid_weights = np.zeros((kgrid.Nx, kgrid.Ny, kgrid.Nz))
+        else:
+            grid_weights = np.zeros((kgrid.Nx, kgrid.Ny))
+
+        assert len(grid_weights.shape) == self.dim, "Grid weights shape must match kArray dimensions."
 
         for ind in range(self.number_elements):
             grid_weights += self.get_off_grid_points(kgrid, ind, False)
 
+        assert len(grid_weights.shape) == self.dim, "Grid weights shape must match kArray dimensions."
+
         return grid_weights
 
     def get_array_binary_mask(self, kgrid):
         self.check_for_elements()
 
         mask = np.zeros((kgrid.Nx, kgrid.Ny, max(kgrid.Nz, 1)), dtype=bool)
 
@@ -438,129 +432,138 @@
             grid_weights = self.get_off_grid_points(kgrid, ind, True)
             mask = np.bitwise_or(np.squeeze(mask), grid_weights)
 
         return mask
 
     def check_for_elements(self):
         if self.number_elements == 0:
-            raise ValueError('Cannot call method on an array with zero elements.')
+            raise ValueError("Cannot call method on an array with zero elements.")
 
     def affine(self, vec):
-
         if len(self.array_transformation) == 0:
             return vec
 
         # check vector is the correct length
         if self.dim != len(vec):
-            raise ValueError('Input vector length must match the number of dimensions')
+            raise ValueError("Input vector length must match the number of dimensions")
 
         # apply transformation
         vec = np.append(vec, [1])
         vec = np.matmul(self.array_transformation, vec)
         return vec[:-1]
 
     def get_off_grid_points(self, kgrid, element_num, mask_only):
-
         # check the array has elements
         self.check_for_elements()
 
         # check inputs
         assert isinstance(kgrid, kWaveGrid)
         assert 0 <= element_num <= self.number_elements - 1
 
         # compute measure (length/area/volume) in grid squares (assuming dx = dy = dz)
         m_grid = self.elements[element_num].measure / (kgrid.dx) ** (self.elements[element_num].dim)
 
         # get number of integration points
-        if self.elements[element_num].type == 'custom':
+        if self.elements[element_num].type == "custom":
             # assign number of integration points directly
             m_integration = self.elements[element_num].integration_points.shape[1]
         else:
             # compute the number of integration points using the upsampling rate
             m_integration = ceil(m_grid * self.upsampling_rate)
 
         # compute integration points covering element
-        if self.elements[element_num].type == 'annulus':
+        if self.elements[element_num].type == "annulus":
             # compute points using make_cart_spherical_segment
             integration_points = make_cart_spherical_segment(
                 self.affine(self.elements[element_num].position),
                 self.elements[element_num].radius_of_curvature,
                 self.elements[element_num].inner_diameter,
                 self.elements[element_num].outer_diameter,
                 self.affine(self.elements[element_num].focus_position),
-                m_integration)
+                m_integration,
+            )
 
-        elif self.elements[element_num].type == 'arc':
+        elif self.elements[element_num].type == "arc":
             # compute points using make_cart_arc
             integration_points = make_cart_arc(
                 self.affine(self.elements[element_num].position),
                 self.elements[element_num].radius_of_curvature,
                 self.elements[element_num].diameter,
                 self.affine(self.elements[element_num].focus_position),
-                m_integration)
+                m_integration,
+            )
 
-        elif self.elements[element_num].type == 'bowl':
+        elif self.elements[element_num].type == "bowl":
             # compute points using make_cart_bowl
             integration_points = make_cart_bowl(
                 self.affine(self.elements[element_num].position),
                 self.elements[element_num].radius_of_curvature,
                 self.elements[element_num].diameter,
                 self.affine(self.elements[element_num].focus_position),
-                m_integration)
+                m_integration,
+            )
 
-        elif self.elements[element_num].type == 'custom':
+        elif self.elements[element_num].type == "custom":
             # directly assign integration points
             integration_points = self.elements[element_num].integration_points
 
-        elif self.elements[element_num].type == 'disc':
+        elif self.elements[element_num].type == "disc":
             # compute points using make_cart_disc
             integration_points = make_cart_disc(
                 self.affine(self.elements[element_num].position),
                 self.elements[element_num].diameter / 2,
                 self.affine(self.elements[element_num].focus_position),
                 m_integration,
                 False,
-                self.use_spiral_disc_points)
+                self.use_spiral_disc_points,
+            )
 
-        elif self.elements[element_num].type == 'rect':
+        elif self.elements[element_num].type == "rect":
             # compute points using make_cart_rect
             integration_points = make_cart_rect(
                 self.affine(self.elements[element_num].position),
                 self.elements[element_num].length,
                 self.elements[element_num].width,
                 self.elements[element_num].orientation,
-                m_integration)
+                m_integration,
+            )
 
-        elif self.elements[element_num].type == 'line':
+        elif self.elements[element_num].type == "line":
             # get distance between points in each dimension
             d = (self.elements[element_num].end_point - self.elements[element_num].start_point) / m_integration
 
             # compute a set of uniformly spaced Cartesian points
             # covering the line using linspace, where the end
             # points are offset by half the point spacing
             if self.dim == 1:
-                integration_points = np.linspace(self.elements[element_num].start_point + d[0] / 2,
-                                                 self.elements[element_num].end_point - d[0] / 2, m_integration)
+                integration_points = np.linspace(
+                    self.elements[element_num].start_point + d[0] / 2, self.elements[element_num].end_point - d[0] / 2, m_integration
+                )
             elif self.dim == 2:
-                px = np.linspace(self.elements[element_num].start_point[0] + d[0] / 2,
-                                 self.elements[element_num].end_point[0] - d[0] / 2, m_integration)
-                py = np.linspace(self.elements[element_num].start_point[1] + d[1] / 2,
-                                 self.elements[element_num].end_point[1] - d[1] / 2, m_integration)
+                px = np.linspace(
+                    self.elements[element_num].start_point[0] + d[0] / 2, self.elements[element_num].end_point[0] - d[0] / 2, m_integration
+                )
+                py = np.linspace(
+                    self.elements[element_num].start_point[1] + d[1] / 2, self.elements[element_num].end_point[1] - d[1] / 2, m_integration
+                )
                 integration_points = np.array([px, py])
             elif self.dim == 3:
-                px = np.linspace(self.elements[element_num].start_point[0] + d[0] / 2,
-                                 self.elements[element_num].end_point[0] - d[0] / 2, m_integration)
-                py = np.linspace(self.elements[element_num].start_point[1] + d[1] / 2,
-                                 self.elements[element_num].end_point[1] - d[1] / 2, m_integration)
-                pz = np.linspace(self.elements[element_num].start_point[2] + d[2] / 2,
-                                 self.elements[element_num].end_point[2] - d[2] / 2, m_integration)
+                px = np.linspace(
+                    self.elements[element_num].start_point[0] + d[0] / 2, self.elements[element_num].end_point[0] - d[0] / 2, m_integration
+                )
+                py = np.linspace(
+                    self.elements[element_num].start_point[1] + d[1] / 2, self.elements[element_num].end_point[1] - d[1] / 2, m_integration
+                )
+                pz = np.linspace(
+                    self.elements[element_num].start_point[2] + d[2] / 2, self.elements[element_num].end_point[2] - d[2] / 2, m_integration
+                )
                 integration_points = np.array([px, py, pz])
 
         else:
-            raise ValueError(f'{self.elements[element_num].type} is not a valid array element type.')
+            raise ValueError(f"{self.elements[element_num].type} is not a valid array element type.")
 
         # recompute actual number of points
         m_integration = integration_points.shape[1]
 
         # compute scaling factor
         scale = m_grid / m_integration
 
@@ -568,33 +571,41 @@
             # create new expanded grid
             kgrid_expanded = kWaveGrid(kgrid.Nx, kgrid.dx, 2 * kgrid.Ny, kgrid.dy)
 
             # remove integration points which are outside grid
             integration_points = trim_cart_points(kgrid_expanded, integration_points)
 
             # calculate grid weights from BLIs centered on the integration points
-            grid_weights = off_grid_points(kgrid_expanded, integration_points, scale,
-                                           bli_tolerance=self.bli_tolerance,
-                                           bli_type=self.bli_type,
-                                           mask_only=mask_only,
-                                           single_precision=self.single_precision)
+            grid_weights = off_grid_points(
+                kgrid_expanded,
+                integration_points,
+                scale,
+                bli_tolerance=self.bli_tolerance,
+                bli_type=self.bli_type,
+                mask_only=mask_only,
+                single_precision=self.single_precision,
+            )
 
             # keep points in the positive y domain
-            grid_weights = grid_weights[:, kgrid.Ny + 1:]
+            grid_weights = grid_weights[:, kgrid.Ny + 1 :]
 
         else:
             # remove integration points which are outside grid
             integration_points = trim_cart_points(kgrid, integration_points)
 
             # calculate grid weights from BLIs centered on the integration points
-            grid_weights = off_grid_points(kgrid, integration_points, scale,
-                                           bli_tolerance=self.bli_tolerance,
-                                           bli_type=self.bli_type,
-                                           mask_only=mask_only,
-                                           single_precision=self.single_precision)
+            grid_weights = off_grid_points(
+                kgrid,
+                integration_points,
+                scale,
+                bli_tolerance=self.bli_tolerance,
+                bli_type=self.bli_type,
+                mask_only=mask_only,
+                single_precision=self.single_precision,
+            )
 
         return grid_weights
 
     def get_distributed_source_signal(self, kgrid, source_signal):
         start_time = time.time()
 
         self.check_for_elements()
@@ -602,118 +613,107 @@
         mask = self.get_array_binary_mask(kgrid)
         mask_ind = matlab_find(mask).squeeze(axis=-1)
         num_source_points = np.sum(mask)
 
         Nt = np.shape(source_signal)[1]
 
         if self.single_precision:
-            data_type = 'float32'
+            data_type = "float32"
             sz_bytes = num_source_points * Nt * 4
         else:
-            data_type = 'float64'
+            data_type = "float64"
             sz_bytes = num_source_points * Nt * 8
 
         sz_ind = 1
         while sz_bytes > 1024:
             sz_bytes = sz_bytes / 1024
             sz_ind += 1
 
-        prefixes = ['', 'K', 'M', 'G', 'T']
+        prefixes = ["", "K", "M", "G", "T"]
         sz_bytes = np.round(sz_bytes, 2)  # TODO: should round to significant to map matlab functionality
-        logging.log(logging.INFO, f'approximate size of source matrix: {str(sz_bytes)} {prefixes[sz_ind]} B ( {data_type} precision)')
+        logging.log(logging.INFO, f"approximate size of source matrix: {str(sz_bytes)} {prefixes[sz_ind]} B ( {data_type} precision)")
 
         source_signal = source_signal.astype(data_type)
 
         distributed_source_signal = np.zeros((num_source_points, Nt), dtype=data_type)
 
         for ind in range(self.number_elements):
             source_weights = self.get_element_grid_weights(kgrid, ind)
 
-            element_mask_ind = matlab_find(np.array(source_weights), val=0, mode='neq').squeeze(axis=-1)
+            element_mask_ind = matlab_find(np.array(source_weights), val=0, mode="neq").squeeze(axis=-1)
 
             local_ind = np.isin(mask_ind, element_mask_ind)
 
-            distributed_source_signal[local_ind] += (
-                    matlab_mask(source_weights, element_mask_ind - 1) * source_signal[ind, :][None, :]
-            )
+            distributed_source_signal[local_ind] += matlab_mask(source_weights, element_mask_ind - 1) * source_signal[ind, :][None, :]
 
         end_time = time.time()
-        logging.log(logging.INFO, f'total computation time : {end_time - start_time:.2f} s')
+        logging.log(logging.INFO, f"total computation time : {end_time - start_time:.2f} s")
 
         return distributed_source_signal
 
     def combine_sensor_data(self, kgrid, sensor_data):
-
         self.check_for_elements()
 
         mask = self.get_array_binary_mask(kgrid)
         mask_ind = matlab_find(mask).squeeze(axis=-1)
 
         Nt = np.shape(sensor_data)[1]
         # TODO (Walter): this assertion does not work when "auto" is set
         # assert kgrid.Nt == Nt, 'sensor_data must have the same number of time steps as kgrid'
 
         combined_sensor_data = np.zeros((self.number_elements, Nt))
 
         for element_num in range(self.number_elements):
             source_weights = self.get_element_grid_weights(kgrid, element_num)
 
-            element_mask_ind = matlab_find(np.array(source_weights), val=0, mode='neq').squeeze(axis=-1)
+            element_mask_ind = matlab_find(np.array(source_weights), val=0, mode="neq").squeeze(axis=-1)
 
             local_ind = np.isin(mask_ind, element_mask_ind)
 
-            combined_sensor_data[element_num, :] = np.sum(sensor_data[local_ind] * matlab_mask(source_weights, element_mask_ind - 1),
-                                                          axis=0)
+            combined_sensor_data[element_num, :] = np.sum(
+                sensor_data[local_ind] * matlab_mask(source_weights, element_mask_ind - 1), axis=0
+            )
 
             m_grid = self.elements[element_num].measure / (kgrid.dx) ** (self.elements[element_num].dim)
 
             combined_sensor_data[element_num, :] = combined_sensor_data[element_num, :] / m_grid
 
         return combined_sensor_data
 
     def set_array_position(self, translation, rotation):
-
         # get affine matrix and store
         self.array_transformation = get_affine_matrix(translation, rotation)
 
     def set_affine_transform(self, affine_transform):
-
         # check array has elements
         if self.number_elements == 0:
-            raise ValueError('Array must have at least one element before a transformation can be defined.')
+            raise ValueError("Array must have at least one element before a transformation can be defined.")
 
         # check the input is the correct size
         sx, sy = affine_transform.shape
         if (self.dim == 2 and (sx != 3 or sy != 3)) or (self.dim == 3 and (sx != 4 or sy != 4)):
-            raise ValueError('Affine transform must be a 3x3 matrix for arrays in 2D, and 4x4 for arrays in 3D.')
+            raise ValueError("Affine transform must be a 3x3 matrix for arrays in 2D, and 4x4 for arrays in 3D.")
 
             # assign the transform
         self.array_transformation = affine_transform
 
     def get_element_positions(self):
-
         # initialise output
         element_pos = np.zeros((self.dim, self.number_elements))
 
         # loop through the elements and assign transformed position
         for i, element in enumerate(self.elements):
             element_pos[:, i] = self.affine(element.position)
 
         return element_pos
 
 
-def off_grid_points(kgrid, points,
-                    scale=1,
-                    bli_tolerance=0.1,
-                    bli_type='sinc',
-                    mask_only=False,
-                    single_precision=False,
-                    debug=False,
-                    display_wait_bar=False):
-
+def off_grid_points(
+    kgrid, points, scale=1, bli_tolerance=0.1, bli_type="sinc", mask_only=False, single_precision=False, debug=False, display_wait_bar=False
+):
     wait_bar_update_freq = 100
 
     # check dimensions of points input
     if points.shape[0] != kgrid.dim:
         raise ValueError("Input points must be given as matrix with dimensions num_dims x num_points.")
 
     # get the number of off-grid points
@@ -725,25 +725,25 @@
     elif np.size(scale) != num_points:
         raise ValueError("Input scale must be scalar or the same length as points.")
     if not isinstance(debug, bool):
         raise ValueError("Optional input 'Debug' must be Boolean.")
 
     if not (isinstance(bli_tolerance, (int, float)) and 0 < bli_tolerance < 1):
         raise ValueError("bli_tolerance should be a real scalar value between 0 and 1.")
-    if bli_type not in ['sinc', 'exact']:
+    if bli_type not in ["sinc", "exact"]:
         raise ValueError("Optional input 'bli_type' must be either 'sinc' or 'exact'.")
     if not isinstance(mask_only, bool):
         raise ValueError("Optional input 'mask_only' must be Boolean.")
     if not isinstance(single_precision, bool):
         raise ValueError("Optional input 'single_precision' must be Boolean.")
     if not isinstance(display_wait_bar, bool):
         raise ValueError("Optional input 'display_wait_bar' must be Boolean.")
 
     # reassign bli_tolerance if bli_type is 'exact'
-    if bli_type == 'exact':
+    if bli_type == "exact":
         bli_tolerance = 0
 
     # extract grid vectors (to avoid recomputing them below)
     x_vec = kgrid.x_vec
     y_vec = kgrid.y_vec
     z_vec = kgrid.z_vec
 
@@ -778,14 +778,15 @@
         mask = np.zeros((kgrid.Nx, kgrid.Ny), dtype=mask_type)
     elif kgrid.dim == 3:
         mask = np.zeros((kgrid.Nx, kgrid.Ny, kgrid.Nz), dtype=mask_type)
 
     # display wait bar
     if display_wait_bar:
         import tqdm
+
         tqdm.tqdm(total=100, desc="Computing off-grid source mask...")
 
     # add to the overall mask using contributions from each source point
     for point_ind in range(num_points):
         # extract a single point
         point = points[:, point_ind]
 
@@ -796,41 +797,40 @@
 
         if bli_tolerance == 0:
             if mask_only:
                 mask = np.ones(mask.shape, dtype=bool)
                 return mask
             else:
                 if kgrid.dim == 1:
-                    if bli_type == 'sinc':
+                    if bli_type == "sinc":
                         mask = mask + scale[point_ind] * sinc(pi_on_dx * (x_vec - point[0]))
-                    elif bli_type == 'exact':
+                    elif bli_type == "exact":
                         mask = mask + scale[point_ind] * get_delta_bli(kgrid.Nx, kgrid.dx, x_vec, point[0])
 
                 elif kgrid.dim == 2:
-                    if bli_type == 'sinc':
+                    if bli_type == "sinc":
                         mask_t_x = sinc(pi_on_dx * (x_vec - point[0]))
                         mask_t_y = sinc(pi_on_dy * (y_vec - point[1]))
-                    elif bli_type == 'exact':
+                    elif bli_type == "exact":
                         mask_t_x = get_delta_bli(kgrid.Nx, kgrid.dx, x_vec, point[0])
                         mask_t_y = get_delta_bli(kgrid.Ny, kgrid.dy, y_vec, point[1])
 
                     mask = mask + scale[point_ind] * (mask_t_x @ mask_t_y.T)
 
                 elif kgrid.dim == 3:
-                    if bli_type == 'sinc':
+                    if bli_type == "sinc":
                         mask_t_x = sinc(pi_on_dx * (x_vec - point[0]))
                         mask_t_y = sinc(pi_on_dy * (y_vec - point[1]))
                         mask_t_z = sinc(pi_on_dz * (z_vec - point[2]))
-                    elif bli_type == 'exact':
+                    elif bli_type == "exact":
                         mask_t_x = get_delta_bli(kgrid.Nx, kgrid.dx, x_vec, point[0])
                         mask_t_y = get_delta_bli(kgrid.Ny, kgrid.dy, y_vec, point[1])
                         mask_t_z = get_delta_bli(kgrid.Nz, kgrid.dz, z_vec, point[2])
 
-                    mask = mask + scale[point_ind] * np.reshape(np.kron(mask_t_y @ mask_t_z.T, mask_t_x),
-                                                                [kgrid.Nx, kgrid.Ny, kgrid.Nz])
+                    mask = mask + scale[point_ind] * np.reshape(np.kron(mask_t_y @ mask_t_z.T, mask_t_x), [kgrid.Nx, kgrid.Ny, kgrid.Nz])
 
         else:
             # create an array of neighbouring grid points for BLI evaluation
             if kgrid.dim == 1:
                 ind, is_, _, _ = tol_star(bli_tolerance, kgrid, point, debug)
                 xs = x_vec[is_]
                 xyz = xs
@@ -867,15 +867,13 @@
 
                 # apply scaling for non-uniform grid
                 if kgrid.nonuniform:
                     current_mask_t = mask_t * BLIscale
 
                 updated_mask_value = matlab_mask(mask, ind - 1).squeeze(axis=-1) + scale[point_ind] * current_mask_t
                 # add this contribution to the overall source mask
-                mask = matlab_assign(mask,
-                                     ind - 1,
-                                     updated_mask_value)
+                mask = matlab_assign(mask, ind - 1, updated_mask_value)
 
         # update the waitbar
         if display_wait_bar and (point_ind % wait_bar_update_freq == 0):
             tqdm.update(wait_bar_update_freq)
     return mask
```

### Comparing `k_wave_python-0.3.2/kwave/utils/mapgen.py` & `k_wave_python-0.3.3/kwave/utils/mapgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from math import floor
 import warnings
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 from scipy import optimize
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Union, List, Tuple, cast, Optional
-from nptyping import NDArray, Float, Shape, Complex, Int, Number
+from jaxtyping import Float, Complex, Int, Real, Integer
 
 from .conversion import db2neper, neper2db
 from .data import scale_SI
 from .math import cosd, sind, Rz, Ry, Rx, compute_linear_transform
 from .matlab import matlab_assign, matlab_find, ind2sub, sub2ind
 from .matrix import max_nd
 from .tictoc import TicToc
@@ -23,16 +23,17 @@
 
 # GLOBALS
 # define literals (ref: http://www.wolframalpha.com/input/?i=golden+angle)
 GOLDEN_ANGLE = 2.39996322972865332223155550663361385312499901105811504
 PACKING_NUMBER = 7  # 2*pi
 
 
-def make_cart_disc(disc_pos: np.ndarray, radius: float, focus_pos: np.ndarray, num_points: int, plot_disc: bool = False,
-                   use_spiral: bool = False) -> np.ndarray:
+def make_cart_disc(
+    disc_pos: np.ndarray, radius: float, focus_pos: np.ndarray, num_points: int, plot_disc: bool = False, use_spiral: bool = False
+) -> np.ndarray:
     """
     Create evenly distributed Cartesian points covering a disc.
 
     Args:
         disc_pos:       Cartesian position of the center of the disc given as a
                         two (2D) or three (3D) element tuple [m].
         radius:         Radius of the disc [m].
@@ -43,40 +44,38 @@
         use_spiral:     Boolean controlling whether the Cartesian points are chosen using a spiral sampling pattern.
                         Concentric sampling is used by default.
 
     Returns:
         disc: 2 x num_points or 3 x num_points array of Cartesian coordinates.
     """
 
-
     # check input values
     if radius <= 0:
         raise ValueError("The radius must be positive.")
 
     def make_spiral_circle_points(num_points: int, radius: float) -> np.ndarray:
         # compute spiral parameters
         theta = lambda t: GOLDEN_ANGLE * t
-        C = np.pi * radius ** 2 / (num_points - 1)
+        C = np.pi * radius**2 / (num_points - 1)
         r = lambda t: np.sqrt(C * t / np.pi)
 
         # compute canonical spiral points
         t = np.linspace(0, num_points - 1, num_points)
         p0 = np.multiply(np.vstack((np.cos(theta(t)), np.sin(theta(t)))), r(t))
         return p0
 
     def make_concentric_circle_points(num_points: int, radius: float) -> Tuple[np.ndarray, int]:
-
-        assert num_points >= 1, "The number of points must be greater or equal to 1." 
+        assert num_points >= 1, "The number of points must be greater or equal to 1."
 
         num_radial = int(np.ceil(np.sqrt(num_points / np.pi)))
-       
+
         try:
             d_radial = radius / (num_radial - 1)
         except ZeroDivisionError:
-            d_radial = float('inf')
+            d_radial = float("inf")
 
         r = np.arange(num_radial) * (radius - d_radial / 2) / (num_radial - 1)
 
         # recompute the number of points that will be created below
         num_points = 1
         for k in range(2, num_radial + 1):
             num_theta = round((k - 1) * PACKING_NUMBER)
@@ -92,15 +91,14 @@
             p = r[k - 1] * np.vstack((np.cos(thetas), np.sin(thetas)))
             i_right = i_left + num_theta
             points[:, i_left:i_right] = p
             i_left = i_right
         return points, num_points
 
     if use_spiral:
-
         p0 = make_spiral_circle_points(num_points, radius)
 
     else:
         # otherwise use concentric circles (note that the num_points is increased
         # to ensure a full set of concentric rings)
 
         p0, num_points = make_concentric_circle_points(num_points, radius)
@@ -127,15 +125,15 @@
     if plot_disc:
         # select suitable axis scaling factor
         _, scale, prefix, unit = scale_SI(np.max(disc))
 
         # create the figure
         if len(disc_pos) == 2:
             plt.figure()
-            plt.plot(disc[1, :] * scale, disc[0, :] * scale, '.')
+            plt.plot(disc[1, :] * scale, disc[0, :] * scale, ".")
             plt.gca().invert_yaxis()
             plt.xlabel(f"y-position [{prefix}m]")
             plt.ylabel(f"x-position [{prefix}m]")
             plt.axis("equal")
         else:
             fig = plt.figure()
             ax = fig.add_subplot(111, projection="3d")
@@ -146,23 +144,18 @@
             ax.axis("equal")
             ax.grid(True)
             ax.box(True)
 
     return np.squeeze(disc)
 
 
-@beartype
+@typechecker
 def make_cart_bowl(
-    bowl_pos: np.ndarray, 
-    radius: float, 
-    diameter: float, 
-    focus_pos: np.ndarray, 
-    num_points: int,
-    plot_bowl: Optional[bool] = False
-) -> NDArray[Shape["3, NumPoints"], Float]:
+    bowl_pos: np.ndarray, radius: float, diameter: float, focus_pos: np.ndarray, num_points: int, plot_bowl: Optional[bool] = False
+) -> Float[np.ndarray, "3 NumPoints"]:
     """
     Create evenly distributed Cartesian points covering a bowl.
 
     Args:
         bowl_pos:       Cartesian position of the centre of the rear surface of
                         the bowl given as a three element vector [bx, by, bz] [m].
         radius:         Radius of curvature of the bowl [m].
@@ -203,17 +196,15 @@
     # compute spiral parameters
     theta = lambda t: GOLDEN_ANGLE * t
     C = 2 * np.pi * (1 - np.cos(varphi_max)) / (num_points - 1)
     varphi = lambda t: np.arccos(1 - C * t / (2 * np.pi))
 
     # compute canonical spiral points
     t = np.linspace(0, num_points - 1, num_points)
-    p0 = np.array([np.cos(theta(t)) * np.sin(varphi(t)),
-                   np.sin(theta(t)) * np.sin(varphi(t)),
-                   np.cos(varphi(t))])
+    p0 = np.array([np.cos(theta(t)) * np.sin(varphi(t)), np.sin(theta(t)) * np.sin(varphi(t)), np.cos(varphi(t))])
     p0 = radius * p0
 
     # linearly transform the canonical spiral points to give bowl in correct orientation
     R, b = compute_linear_transform(bowl_pos, focus_pos, radius)
 
     if b.ndim == 1:
         b = np.expand_dims(b, axis=-1)  # expand dims for broadcasting
@@ -223,27 +214,27 @@
     # plot results
     if plot_bowl is True:
         # select suitable axis scaling factor
         _, scale, prefix, unit = scale_SI(np.max(bowl))
 
         # create the figure
         fig = plt.figure()
-        ax = fig.add_subplot(111, projection='3d')
+        ax = fig.add_subplot(111, projection="3d")
         ax.scatter(bowl[0, :] * scale, bowl[1, :] * scale, bowl[2, :] * scale)
-        ax.set_xlabel('[' + prefix + unit + ']')
-        ax.set_ylabel('[' + prefix + unit + ']')
-        ax.set_zlabel('[' + prefix + unit + ']')
+        ax.set_xlabel("[" + prefix + unit + "]")
+        ax.set_ylabel("[" + prefix + unit + "]")
+        ax.set_zlabel("[" + prefix + unit + "]")
         ax.set_box_aspect([1, 1, 1])
         plt.grid(True)
         plt.show()
 
     return bowl
 
 
-def get_spaced_points(start: float, stop: float, n: int = 100, spacing: str = 'linear') -> np.ndarray:
+def get_spaced_points(start: float, stop: float, n: int = 100, spacing: str = "linear") -> np.ndarray:
     """
     Generate a row vector of either logarithmically or linearly spaced points between `start` and `stop`.
 
     When `spacing` is set to 'linear', the function is identical to the inbuilt `np.linspace` function.
     When `spacing` is set to 'log', the function is similar to the inbuilt `np.logspace` function, except
     that `start` and `stop` define the start and end numbers, not decades. For logarithmically spaced
     points, `start` must be > 0. If `n` < 2, `stop` is returned.
@@ -259,26 +250,25 @@
 
     Raises:
         ValueError: if `stop` <= `start` or `spacing` is not 'linear' or 'log'
 
     """
 
     if stop <= start:
-        raise ValueError('`stop` must be larger than `start`.')
+        raise ValueError("`stop` must be larger than `start`.")
 
-    if spacing == 'linear':
+    if spacing == "linear":
         return np.linspace(start, stop, num=n)
-    elif spacing == 'log':
+    elif spacing == "log":
         return np.geomspace(start, stop, num=n)
     else:
         raise ValueError(f"`spacing` {spacing} is not a valid argument. Choose from 'linear' or 'log'.")
 
 
-def fit_power_law_params(a0: float, y: float, c0: float, f_min: float, f_max: float, plot_fit: bool = False) -> Tuple[
-    float, float]:
+def fit_power_law_params(a0: float, y: float, c0: float, f_min: float, f_max: float, plot_fit: bool = False) -> Tuple[float, float]:
     """
     Calculate absorption parameters that fit a power law over a given frequency range.
 
     This function calculates the absorption parameters that should be defined in the simulation functions
     to achieve the desired power law absorption behavior defined by `a0` and `y`. This takes into account
     the actual absorption behavior exhibited by the fractional Laplacian wave equation.
 
@@ -305,23 +295,23 @@
 
     # define frequency axis
     f = get_spaced_points(f_min, f_max, 200)
     w = 2 * np.pi * f
     # convert user defined a0 to Nepers/((rad/s)^y m)
     a0_np = db2neper(a0, y)
 
-    desired_absorption = a0_np * w ** y
+    desired_absorption = a0_np * w**y
 
     def abs_func(trial_vals):
         """Second-order absorption error"""
         a0_np_trial, y_trial = trial_vals
 
-        actual_absorption = a0_np_trial * w ** y_trial / (1 - (y_trial + 1) *
-                                                          a0_np_trial * c0 * np.tan(np.pi * y_trial / 2) * w ** (
-                                                                  y_trial - 1))
+        actual_absorption = (
+            a0_np_trial * w**y_trial / (1 - (y_trial + 1) * a0_np_trial * c0 * np.tan(np.pi * y_trial / 2) * w ** (y_trial - 1))
+        )
 
         absorption_error = np.sqrt(np.sum((desired_absorption - actual_absorption) ** 2))
 
         return absorption_error
 
     a0_np_fit, y_fit = optimize.fmin(abs_func, [a0_np, y])
 
@@ -381,35 +371,44 @@
     Returns:
         abs:  absorption [dB / cm]
 
     Examples:
         >>> abs = waterAbsorption(f, T)
 
     References:
-        [1] J. M. M. Pinkerton (1949) "The Absorption of Ultrasonic Waves in Liquids and its 
-                                        Relation to Molecular Constitution," 
+        [1] J. M. M. Pinkerton (1949) "The Absorption of Ultrasonic Waves in Liquids and its
+                                        Relation to Molecular Constitution,"
         Proceedings of the Physical Society. Section B, 2, 129-141
 
     """
 
     NEPER2DB = 8.686
     # check temperature is within range
-    if not np.all([np.all(temp>=0.0), np.all(temp<=60.0)]):
+    if not np.all([np.all(temp >= 0.0), np.all(temp <= 60.0)]):
         raise Warning("Temperature outside range of experimental data")
 
     # conversion factor between Nepers and dB NEPER2DB = 8.686;
     # coefficients for 7th order polynomial fit
-    a = [56.723531840522710, -2.899633796917384, 0.099253401567561, -0.002067402501557, 2.189417428917596e-005,
-         -6.210860973978427e-008, -6.402634551821596e-010, 3.869387679459408e-012]
+    a = [
+        56.723531840522710,
+        -2.899633796917384,
+        0.099253401567561,
+        -0.002067402501557,
+        2.189417428917596e-005,
+        -6.210860973978427e-008,
+        -6.402634551821596e-010,
+        3.869387679459408e-012,
+    ]
 
     # compute absorption
-    a_on_fsqr = (a[0] + a[1] * temp + a[2] * temp ** 2 + a[3] * temp ** 3 + a[4] * temp ** 4 + a[5] * temp ** 5 + a[
-        6] * temp ** 6 + a[7] * temp ** 7) * 1e-17
+    a_on_fsqr = (
+        a[0] + a[1] * temp + a[2] * temp**2 + a[3] * temp**3 + a[4] * temp**4 + a[5] * temp**5 + a[6] * temp**6 + a[7] * temp**7
+    ) * 1e-17
 
-    abs = NEPER2DB * 1e12 * f ** 2 * a_on_fsqr
+    abs = NEPER2DB * 1e12 * f**2 * a_on_fsqr
     return abs
 
 
 def water_sound_speed(temp: Union[float, kt.NP_DOMAIN]) -> Union[float, kt.NP_DOMAIN]:
     """
     Calculate the sound speed in distilled water with temperature according to Marczak (1997)
 
@@ -425,15 +424,15 @@
     References:
         [1] R. Marczak (1997). "The sound velocity in water as a function of temperature".
         Journal of Research of the National Institute of Standards and Technology, 102(6), 561-567.
 
     """
 
     # check limits
-    if not np.all([np.all(temp>=0.0), np.all(temp<=95.0)]):
+    if not np.all([np.all(temp >= 0.0), np.all(temp <= 95.0)]):
         raise ValueError("`temp` must be between 0 and 95.")
 
     # find value
     p = [2.787860e-9, -1.398845e-6, 3.287156e-4, -5.779136e-2, 5.038813, 1.402385e3]
     c = np.polyval(p, temp)
     return c
 
@@ -457,19 +456,19 @@
     References:
         [1] F. E. Jones and G. L. Harris (1992) "ITS-90 Density of Water Formulation for Volumetric Standards Calibration,"
         Journal of Research of the National Institute of Standards and Technology, 97(3), 335-340.
 
     """
 
     # check limits
-    if not np.all([np.all(np.asarray(temp)>=5.0), np.all(np.asarray(temp)<=40.0)]):
+    if not np.all([np.all(np.asarray(temp) >= 5.0), np.all(np.asarray(temp) <= 40.0)]):
         raise ValueError("`temp` must be between 5 and 40.")
 
     # calculate density of air-saturated water
-    density = 999.84847 + 6.337563e-2 * temp - 8.523829e-3 * temp ** 2 + 6.943248e-5 * temp ** 3 - 3.821216e-7 * temp ** 4
+    density = 999.84847 + 6.337563e-2 * temp - 8.523829e-3 * temp**2 + 6.943248e-5 * temp**3 - 3.821216e-7 * temp**4
     return density
 
 
 def water_non_linearity(temp: Union[float, kt.NP_DOMAIN]) -> Union[float, kt.NP_DOMAIN]:
     """
      Calculates the parameter of nonlinearity B/A at a
      given temperature using a fourth-order polynomial fitted to the data
@@ -481,36 +480,32 @@
     Returns:
         BonA: parameter of nonlinearity
 
     Examples:
          >>> BonA = waterNonlinearity(T)
 
      References:
-         [1] R. T. Beyer (1960) "Parameter of nonlinearity in fluids," 
+         [1] R. T. Beyer (1960) "Parameter of nonlinearity in fluids,"
          J. Acoust. Soc. Am., 32(6), 719-721.
 
     """
 
     # check limits
-    if not np.all([np.all(temp>=0.0), np.all(temp<=100.0)]):
+    if not np.all([np.all(temp >= 0.0), np.all(temp <= 100.0)]):
         raise ValueError("`temp` must be between 0 and 100.")
 
     # find value
     p = [-4.587913769504693e-08, 1.047843302423604e-05, -9.355518377254833e-04, 5.380874771364909e-2, 4.186533937275504]
     BonA = np.polyval(p, temp)
     return BonA
 
 
-@beartype
+@typechecker
 def make_ball(
-        grid_size: Vector, 
-        ball_center: Vector, 
-        radius: int, 
-        plot_ball: bool = False,
-        binary: bool = False
+    grid_size: Vector, ball_center: Vector, radius: int, plot_ball: bool = False, binary: bool = False
 ) -> Union[kt.NP_ARRAY_INT_3D, kt.NP_ARRAY_BOOL_3D]:
     """
     Creates a binary map of a filled ball within a 3D grid.
 
     Args:
         grid_size: size of the 3D grid in [grid points].
         ball_center: centre of the ball in [grid points]
@@ -553,21 +548,18 @@
     # plot results
     if plot_ball:
         raise NotImplementedError
         # voxelPlot(double(ball))
     return ball
 
 
-@beartype
+@typechecker
 def make_cart_sphere(
-    radius: Union[float, int], 
-    num_points: int, 
-    center_pos: Vector = Vector([0, 0, 0]),
-    plot_sphere: bool = False
-) -> NDArray[Shape["3, NumPoints"], Float]:
+    radius: Union[float, int], num_points: int, center_pos: Vector = Vector([0, 0, 0]), plot_sphere: bool = False
+) -> Float[np.ndarray, "3 NumPoints"]:
     """
     Cart_sphere creates a set of points in Cartesian coordinates defining a sphere.
 
     Args:
         radius: the radius of the sphere.
         num_points: the number of points to be generated.
         center_pos: the coordinates of the center of the sphere. Defaults to (0, 0, 0).
@@ -578,15 +570,15 @@
 
     """
     # generate angle functions using the Golden Section Spiral method
     inc = np.pi * (3 - np.sqrt(5))
     off = 2 / num_points
     k = np.arange(0, num_points)
     y = k * off - 1 + (off / 2)
-    r = np.sqrt(1 - (y ** 2))
+    r = np.sqrt(1 - (y**2))
     phi = k * inc
 
     if num_points <= 0:
         raise ValueError("num_points must be greater than 0")
 
     # create the sphere
     sphere = radius * np.concatenate([np.cos(phi) * r[np.newaxis, :], y[np.newaxis, :], np.sin(phi) * r[np.newaxis, :]])
@@ -597,34 +589,30 @@
     # plot results
     if plot_sphere:
         # select suitable axis scaling factor
         [x_sc, scale, prefix, _] = scale_SI(np.max(sphere))
 
         # create the figure
         plt.figure()
-        plt.style.use('seaborn-poster')
-        ax = plt.axes(projection='3d')
-        ax.plot3D(sphere[0, :] * scale, sphere[1, :] * scale, sphere[2, :] * scale, '.')
+        plt.style.use("seaborn-poster")
+        ax = plt.axes(projection="3d")
+        ax.plot3D(sphere[0, :] * scale, sphere[1, :] * scale, sphere[2, :] * scale, ".")
         ax.set_xlabel(f"[{prefix} m]")
         ax.set_ylabel(f"[{prefix} m]")
         ax.set_zlabel(f"[{prefix} m]")
-        ax.axis('auto')
+        ax.axis("auto")
         ax.grid()
         plt.show()
 
     return sphere.squeeze()
 
 
 def make_cart_circle(
-    radius: float, 
-    num_points: int, 
-    center_pos: Vector = Vector([0, 0]),
-    arc_angle: float = 2 * np.pi, 
-    plot_circle: bool = False
-) -> NDArray[Shape["2, NumPoints"], Float]:
+    radius: float, num_points: int, center_pos: Vector = Vector([0, 0]), arc_angle: float = 2 * np.pi, plot_circle: bool = False
+) -> Float[np.ndarray, "2 NumPoints"]:
     """
     Create a set of points in cartesian coordinates defining a circle or arc.
 
     This function creates a set of points in cartesian coordinates defining a circle or arc.
 
     Args:
         radius: radius of the circle or arc
@@ -658,30 +646,25 @@
     # plot results
     if plot_circle:
         # select suitable axis scaling factor
         [_, scale, prefix, _] = scale_SI(np.max(abs(circle)))
 
         # create the figure
         plt.figure()
-        plt.plot(circle[1, :] * scale, circle[0, :] * scale, 'b.')
+        plt.plot(circle[1, :] * scale, circle[0, :] * scale, "b.")
         plt.xlabel([f"y-position [{prefix} m]"])
         plt.ylabel([f"x-position [{prefix} m]"])
-        plt.axis('equal')
+        plt.axis("equal")
         plt.show()
 
     return np.squeeze(circle)
 
 
-@beartype
-def make_disc(
-    grid_size: Vector, 
-    center: Vector, 
-    radius, 
-    plot_disc=False
-) -> kt.NP_ARRAY_BOOL_2D:
+@typechecker
+def make_disc(grid_size: Vector, center: Vector, radius, plot_disc=False) -> kt.NP_ARRAY_BOOL_2D:
     """
     Create a binary map of a filled disc within a 2D grid.
 
     This function creates a binary map of a filled disc within a two-dimensional grid. The disc position is denoted by 1's
     in the matrix with 0's elsewhere. A single grid point is taken as the disc centre, so the total diameter of the disc
     will always be an odd number of grid points. If used within a k-Wave grid where dx != dy, the disc will appear oval
     shaped. If part of the disc overlaps the grid edge, the rest of the disc will wrap to the grid edge on the opposite
@@ -694,30 +677,30 @@
         plot_disc: If set to True, the disc will be plotted using Matplotlib.
 
     Returns:
         A binary map of the disc in the 2D grid.
 
     """
 
-    assert len(grid_size) == 2, 'Grid size must be 2D.'
-    assert len(center) == 2, 'Center must be 2D.'
+    assert len(grid_size) == 2, "Grid size must be 2D."
+    assert len(center) == 2, "Center must be 2D."
 
     # define literals
     MAGNITUDE = 1
 
     # force integer values
     grid_size = grid_size.round().astype(int)
     center = center.round().astype(int)
 
     # check for zero values
     center.x = center.x if center.x != 0 else np.floor(grid_size.x / 2).astype(int) + 1
     center.y = center.y if center.y != 0 else np.floor(grid_size.y / 2).astype(int) + 1
 
     # check the inputs
-    assert np.all(0 < center) and np.all(center <= grid_size), 'Disc center must be within grid.'
+    assert np.all(0 < center) and np.all(center <= grid_size), "Disc center must be within grid."
 
     # create empty matrix
     disc = np.zeros(grid_size, dtype=bool)
 
     # define np.pixel map
     r = make_pixel_map(grid_size, shift=[0, 0])
 
@@ -730,21 +713,17 @@
 
     # create the figure
     if plot_disc:
         raise NotImplementedError
     return disc
 
 
-@beartype
+@typechecker
 def make_circle(
-        grid_size: Vector, 
-        center: Vector, 
-        radius: Union[int, Int, Float], 
-        arc_angle: Optional[float] = None,
-        plot_circle: bool = False
+    grid_size: Vector, center: Vector, radius: Real[kt.ScalarLike, ""], arc_angle: Optional[float] = None, plot_circle: bool = False
 ) -> kt.NP_ARRAY_INT_2D:
     """
     Create a binary map of a circle within a 2D grid.
 
     This function creates a binary map of a circle (or arc) using the midpoint circle algorithm within a two-dimensional grid.
     The circle position is denoted by 1's in the matrix with 0's elsewhere. A single grid point is taken as the circle
     centre, so the total diameter will always be an odd number of grid points. The centre of the circle and the radius
@@ -800,52 +779,49 @@
     # draw the remaining cardinal points
     px = [cx, cx + y, cx - y]
     py = [cy + y, cy, cy]
     for point_index, (px_i, py_i) in enumerate(zip(px, py)):
         # check whether the point is within the arc made by arc_angle, and lies
         # within the grid
         if (np.arctan2(px_i - cx, py_i - cy) + np.pi) <= arc_angle:
-            if (px_i >= 1) and (px_i <= grid_size.x) and (py_i >= 1) and (
-                    py_i <= grid_size.y):
+            if (px_i >= 1) and (px_i <= grid_size.x) and (py_i >= 1) and (py_i <= grid_size.y):
                 circle[px_i - 1, py_i - 1] = MAGNITUDE
 
     # loop through the remaining points using the midpoint circle algorithm
     while x < (y - 1):
-
         x = x + 1
         if d < 0:
             d = d + x + x + 1
         else:
             y = y - 1
             a = x - y + 1
             d = d + a + a
 
         # setup point indices (break coding standard for readability)
         px = [x + cx, y + cx, y + cx, x + cx, -x + cx, -y + cx, -y + cx, -x + cx]
         py = [y + cy, x + cy, -x + cy, -y + cy, -y + cy, -x + cy, x + cy, y + cy]
 
         # loop through each point
         for point_index, (px_i, py_i) in enumerate(zip(px, py)):
-
             # check whether the point is within the arc made by arc_angle, and
             # lies within the grid
             if (np.arctan2(px_i - cx, py_i - cy) + np.pi) <= arc_angle:
                 if (px_i >= 1) and (px_i <= grid_size.x) and (py_i >= 1) and (py_i <= grid_size.y):
                     circle[px_i - 1, py_i - 1] = MAGNITUDE
 
     if plot_circle:
-        plt.imshow(circle, cmap='gray_r')
-        plt.ylabel('x-position [grid points]')
-        plt.xlabel('y-position [grid points]')
+        plt.imshow(circle, cmap="gray_r")
+        plt.ylabel("x-position [grid points]")
+        plt.xlabel("y-position [grid points]")
         plt.show()
 
     return circle
 
 
-def make_pixel_map(grid_size: Vector, shift=None, origin_size='single') -> np.ndarray:
+def make_pixel_map(grid_size: Vector, shift=None, origin_size="single") -> np.ndarray:
     """
     Generates a matrix with values of the distance of each pixel from the center of a grid.
 
     This function generates a matrix populated with values of how far each pixel in a grid is from the center. The center
     can be a single pixel or a double pixel, and the optional input parameter 'OriginSize' controls this. For grids where
     the dimension size and center pixel size are not both odd or even, the optional input parameter 'Shift' can be used to
     control the location of the center point.
@@ -876,15 +852,15 @@
          x x x x      x x 0 0 x        x x x x x
                       x x x x x        x x x x x
 
          By default, a single pixel centre is used which is shifted towards
          the final row and column.
 
     """
-    assert len(grid_size) == 2 or len(grid_size) == 3, 'Grid size must be a 2 or 3 element vector.'
+    assert len(grid_size) == 2 or len(grid_size) == 3, "Grid size must be a 2 or 3 element vector."
 
     # define defaults
     shift_def = 1
 
     Nx = grid_size[0]
     Ny = grid_size[1]
     Nz = None
@@ -893,40 +869,41 @@
 
     # detect whether the inputs are for two or three dimensions
     map_dimension = 2 if Nz is None else 3
     if shift is None:
         shift = [shift_def] * map_dimension
 
     # catch input errors
-    assert origin_size in ['single', 'double'], 'Unknown setting for optional input Center.'
+    assert origin_size in ["single", "double"], "Unknown setting for optional input Center."
 
-    assert len(shift) == map_dimension, \
-        f'Optional input Shift must have {map_dimension} elements for {map_dimension} dimensional input parameters.'
+    assert (
+        len(shift) == map_dimension
+    ), f"Optional input Shift must have {map_dimension} elements for {map_dimension} dimensional input parameters."
 
     if map_dimension == 2:
         # create the maps for each dimension
         nx = create_pixel_dim(Nx, origin_size, shift[0])
         ny = create_pixel_dim(Ny, origin_size, shift[1])
 
         # create plaid grids
-        r_x, r_y = np.meshgrid(nx, ny, indexing='ij')
+        r_x, r_y = np.meshgrid(nx, ny, indexing="ij")
 
         # extract the pixel radius
-        r = np.sqrt(r_x ** 2 + r_y ** 2)
+        r = np.sqrt(r_x**2 + r_y**2)
     if map_dimension == 3:
         # create the maps for each dimension
         nx = create_pixel_dim(Nx, origin_size, shift[0])
         ny = create_pixel_dim(Ny, origin_size, shift[1])
         nz = create_pixel_dim(Nz, origin_size, shift[2])
 
         # create plaid grids
-        r_x, r_y, r_z = np.meshgrid(nx, ny, nz, indexing='ij')
+        r_x, r_y, r_z = np.meshgrid(nx, ny, nz, indexing="ij")
 
         # extract the pixel radius
-        r = np.sqrt(r_x ** 2 + r_y ** 2 + r_z ** 2)
+        r = np.sqrt(r_x**2 + r_y**2 + r_z**2)
     return r
 
 
 def create_pixel_dim(Nx: int, origin_size: float, shift: float) -> Tuple[np.ndarray, float]:
     """
     Create an array of pixel dimensions and a pixel size.
 
@@ -940,57 +917,53 @@
 
     """
 
     # Nested function to create the pixel radius variable
 
     # grid dimension has an even number of points
     if Nx % 2 == 0:
-
         # pixel numbering has a single centre point
-        if origin_size == 'single':
-
+        if origin_size == "single":
             # centre point is shifted towards the final pixel
             if shift == 1:
                 nx = np.arange(-Nx / 2, Nx / 2 - 1 + 1, 1)
 
             # centre point is shifted towards the first pixel
             else:
                 nx = np.arange(-Nx / 2 + 1, Nx / 2 + 1, 1)
 
         # pixel numbering has a double centre point
         else:
             nx = np.hstack([np.arange(-Nx / 2 + 1, 0 + 1, 1), np.arange(0, -Nx / 2 - 1 + 1, 1)])
 
     # grid dimension has an odd number of points
     else:
-
         # pixel numbering has a single centre point
-        if origin_size == 'single':
+        if origin_size == "single":
             nx = np.arange(-(Nx - 1) / 2, (Nx - 1) / 2 + 1, 1)
 
         # pixel numbering has a double centre point
         else:
-
             # centre point is shifted towards the final pixel
             if shift == 1:
                 nx = np.hstack([np.arange(-(Nx - 1) / 2, 0 + 1, 1), np.arange(0, (Nx - 1) / 2 - 1 + 1, 1)])
 
             # centre point is shifted towards the first pixel
             else:
                 nx = np.hstack([np.arange(-(Nx - 1) / 2 + 1, 0 + 1, 1), np.arange(0, (Nx - 1) / 2 + 1, 1)])
     return nx
 
 
-@beartype
+@typechecker
 def make_line(
-        grid_size: Vector,
-        startpoint: Union[Tuple[Int, Int], NDArray[Shape['2'], Int]],
-        endpoint: Optional[Union[Tuple[Int, Int], NDArray[Shape['2'], Int]]] = None,
-        angle: Optional[float] = None,
-        length: Optional[int] = None
+    grid_size: Vector,
+    startpoint: Union[Tuple[Int[kt.ScalarLike, ""], Int[kt.ScalarLike, ""]], Int[np.ndarray, "2"]],
+    endpoint: Optional[Union[Tuple[Int[kt.ScalarLike, ""], Int[kt.ScalarLike, ""]], Int[np.ndarray, "2"]]] = None,
+    angle: Optional[Float[kt.ScalarLike, ""]] = None,
+    length: Optional[Int[kt.ScalarLike, ""]] = None,
 ) -> kt.NP_ARRAY_BOOL_2D:
     """
     Generate a line shape with a given start and end point, angle, or length.
 
     Args:
         grid_size: The size of the grid in pixels.
         startpoint: The start point of the line, given as a tuple of x and y coordinates.
@@ -1001,85 +974,81 @@
         length: The length of the line in pixels.
                 If not specified, the line is drawn from the start point to the end point.
 
     Returns:
         line: A 2D array of the same size as the input parameters,
                 with a value of 1 for pixels that are part of the line and 0 for pixels that are not.
     """
-    assert len(grid_size) == 2, 'Grid size must be a 2-element vector.'
+    assert len(grid_size) == 2, "Grid size must be a 2-element vector."
 
     startpoint = np.array(startpoint, dtype=int)
     if endpoint is not None:
         endpoint = np.array(endpoint, dtype=int)
 
     if len(startpoint) != 2:
-        raise ValueError('startpoint should be a two-element vector.')
+        raise ValueError("startpoint should be a two-element vector.")
 
     if np.any(startpoint < 1) or startpoint[0] > grid_size.x or startpoint[1] > grid_size.y:
-        ValueError('The starting point must lie within the grid, between [1 1] and [grid_size.x grid_size.y].')
+        ValueError("The starting point must lie within the grid, between [1 1] and [grid_size.x grid_size.y].")
 
     # =========================================================================
     # LINE BETWEEN TWO POINTS OR ANGLED LINE?
     # =========================================================================
 
     if endpoint is not None:
-        linetype = 'AtoB'
+        linetype = "AtoB"
         a, b = startpoint, endpoint
 
         # Addition => Fix Matlab2Python indexing
         a -= 1
         b -= 1
     else:
-        linetype = 'angled'
+        linetype = "angled"
         angle, linelength = angle, length
 
     # =========================================================================
     # MORE INPUT CHECKING
     # =========================================================================
 
-    if linetype == 'AtoB':
-
+    if linetype == "AtoB":
         # a and b must be different points
         if np.all(a == b):
-            raise ValueError('The first and last points cannot be the same.')
+            raise ValueError("The first and last points cannot be the same.")
 
         # end point must be a two-element row vector
         if len(b) != 2:
-            raise ValueError('endpoint should be a two-element vector.')
+            raise ValueError("endpoint should be a two-element vector.")
 
         # a and b must be within the grid
         xx = np.array([a[0], b[0]], dtype=int)
         yy = np.array([a[1], b[1]], dtype=int)
         if np.any(a < 0) or np.any(b < 0) or np.any(xx > grid_size.x - 1) or np.any(yy > grid_size.y - 1):
-            raise ValueError('Both the start and end points must lie within the grid.')
-
-    if linetype == 'angled':
+            raise ValueError("Both the start and end points must lie within the grid.")
 
+    if linetype == "angled":
         # angle must lie between -np.pi and np.pi
         angle = angle % (2 * np.pi)
         if angle > np.pi:
             angle = angle - (2 * np.pi)
         elif angle < -np.pi:
             angle = angle + (2 * np.pi)
 
     # =========================================================================
     # CALCULATE A LINE FROM A TO B
     # =========================================================================
 
-    if linetype == 'AtoB':
-
+    if linetype == "AtoB":
         # define an empty grid to hold the line
         line = np.zeros(grid_size, dtype=bool)
 
         # find the equation of the line
         m = (b[1] - a[1]) / (b[0] - a[0])  # gradient of the line
         c = a[1] - m * a[0]  # where the line crosses the y axis
 
         if abs(m) < 1:
-
             # start at the end with the smallest value of x
             if a[0] < b[0]:
                 x, y = a
                 x_end = b[0]
             else:
                 x, y = b
                 x_end = a[0]
@@ -1101,15 +1070,14 @@
                 x = poss_x[index[0] - 1]
                 y = poss_y[index[0] - 1]
 
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
         elif not np.isinf(abs(m)):
-
             # start at the end with the smallest value of y
             if a[1] < b[1]:
                 x = a[0]
                 y = a[1]
                 y_end = b[1]
             else:
                 x = b[0]
@@ -1133,15 +1101,14 @@
                 x = poss_x[index[0] - 1]
                 y = poss_y[index[0] - 1]
 
                 # add the point to the line
                 line[x, y] = 1
 
         else:  # m = +-Inf
-
             # start at the end with the smallest value of y
             if a[1] < b[1]:
                 x = a[0]
                 y = a[1]
                 y_end = b[1]
             else:
                 x = b[0]
@@ -1158,53 +1125,48 @@
                 # add the point to the line
                 line[x, y] = 1
 
     # =========================================================================
     # CALCULATE AN ANGLED LINE
     # =========================================================================
 
-    elif linetype == 'angled':
-
+    elif linetype == "angled":
         # define an empty grid to hold the line
         line = np.zeros(grid_size, dtype=bool)
 
         # start at the atart
         x, y = startpoint
 
         # fill in the first point
         line[x - 1, y - 1] = 1
 
         # initialise the current length of the line
         line_length = 0
 
         if abs(angle) == np.pi:
-
             while line_length < linelength:
-
                 # next point
                 y = y + 1
 
                 # stop the points incrementing at the edges
                 if y > grid_size.y:
                     break
 
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif (angle < np.pi) and (angle > np.pi / 2):
-
             # define the equation of the line
             m = -np.tan(angle - np.pi / 2)  # gradient of the line
             c = y - m * x  # where the line crosses the y axis
 
             while line_length < linelength:
-
                 # next points to try are
                 poss_x = np.array([x - 1, x - 1, x])
                 poss_y = np.array([y, y + 1, y + 1])
 
                 # find the point closest to the line
                 true_y = m * poss_x + c
                 diff = (poss_y - true_y) ** 2
@@ -1221,38 +1183,34 @@
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif angle == np.pi / 2:
-
             while line_length < linelength:
-
                 # next point
                 x = x - 1
 
                 # stop the points incrementing at the edges
                 if x < 1:
                     break
 
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif (angle < np.pi / 2) and (angle > 0):
-
             # define the equation of the line
             m = np.tan(np.pi / 2 - angle)  # gradient of the line
             c = y - m * x  # where the line crosses the y axis
 
             while line_length < linelength:
-
                 # next points to try are
                 poss_x = np.array([x - 1, x - 1, x])
                 poss_y = np.array([y, y - 1, y - 1])
 
                 # find the point closest to the line
                 true_y = m * poss_x + c
                 diff = (poss_y - true_y) ** 2
@@ -1269,38 +1227,34 @@
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif angle == 0:
-
             while line_length < linelength:
-
                 # next point
                 y = y - 1
 
                 # stop the points incrementing at the edges
                 if y < 1:
                     break
 
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif (angle < 0) and (angle > -np.pi / 2):
-
             # define the equation of the line
             m = -np.tan(np.pi / 2 + angle)  # gradient of the line
             c = y - m * x  # where the line crosses the y axis
 
             while line_length < linelength:
-
                 # next points to try are
                 poss_x = np.array([x + 1, x + 1, x])
                 poss_y = np.array([y, y - 1, y - 1])
 
                 # find the point closest to the line
                 true_y = m * poss_x + c
                 diff = (poss_y - true_y) ** 2
@@ -1317,38 +1271,34 @@
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif angle == -np.pi / 2:
-
             while line_length < linelength:
-
                 # next point
                 x = x + 1
 
                 # stop the points incrementing at the edges
                 if x > grid_size.x:
                     break
 
                 # add the point to the line
                 line[x - 1, y - 1] = 1
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
         elif (angle < -np.pi / 2) and (angle > -np.pi):
-
             # define the equation of the line
             m = np.tan(-angle - np.pi / 2)  # gradient of the line
             c = y - m * x  # where the line crosses the y axis
 
             while line_length < linelength:
-
                 # next points to try are
                 poss_x = np.array([x + 1, x + 1, x])
                 poss_y = np.array([y, y + 1, y + 1])
 
                 # find the point closest to the line
                 true_y = m * poss_x + c
                 diff = (poss_y - true_y) ** 2
@@ -1367,82 +1317,77 @@
 
                 # calculate the current length of the line
                 line_length = np.sqrt((x - startpoint[0]) ** 2 + (y - startpoint[1]) ** 2)
 
     return line
 
 
-@beartype
+@typechecker
 def make_arc(
-        grid_size: Vector, 
-        arc_pos: np.ndarray, 
-        radius: Union[int, float], 
-        diameter: Union[Int, int], 
-        focus_pos: Vector
+    grid_size: Vector, arc_pos: np.ndarray, radius: Real[kt.ScalarLike, ""], diameter: Int[kt.ScalarLike, ""], focus_pos: Vector
 ) -> Union[kt.NP_ARRAY_INT_2D, kt.NP_ARRAY_BOOL_2D]:
     """
     Generates an arc shape with a given radius, diameter, and focus position.
 
     Args:
         grid_size: The size of the grid, given as a 1D array with the number of pixels in each dimension.
         arc_pos: The position of the arc, given as a 1D array with the coordinates in each dimension.
         radius: The radius of the arc.
         diameter: The diameter of the arc.
         focus_pos: The position of the focus, given as a 1D array with the coordinates in each dimension.
 
     Returns:
         np.ndarray: A 2D array with the arc shape.
     """
-    assert len(grid_size) == 2, 'The grid size must be a 2D vector.'
-    assert len(arc_pos) == 2, 'The arc position must be a 2D vector.'
-    assert len(focus_pos) == 2, 'The focus position must be a 2D vector.'
+    assert len(grid_size) == 2, "The grid size must be a 2D vector."
+    assert len(arc_pos) == 2, "The arc position must be a 2D vector."
+    assert len(focus_pos) == 2, "The focus position must be a 2D vector."
 
     # force integer input values
     grid_size = grid_size.round().astype(int)
     arc_pos = arc_pos.round().astype(int)
     diameter = int(round(diameter))
     focus_pos = focus_pos.round().astype(int)
 
     try:
         radius = int(radius)
     except OverflowError:
         radius = float(radius)
 
     # check the input ranges
     if np.any(grid_size < 1):
-        raise ValueError('The grid size must be positive.')
+        raise ValueError("The grid size must be positive.")
     if radius <= 0:
-        raise ValueError('The radius must be positive.')
+        raise ValueError("The radius must be positive.")
 
     if diameter <= 0:
-        raise ValueError('The diameter must be positive.')
+        raise ValueError("The diameter must be positive.")
 
     if np.any(arc_pos < 1) or np.any(arc_pos > grid_size):
-        raise ValueError('The centre of the arc must be within the grid.')
+        raise ValueError("The centre of the arc must be within the grid.")
 
     if diameter > 2 * radius:
-        raise ValueError('The diameter of the arc must be less than twice the radius of curvature.')
+        raise ValueError("The diameter of the arc must be less than twice the radius of curvature.")
 
     if diameter % 2 != 1:
-        raise ValueError('The diameter must be an odd number of grid points.')
+        raise ValueError("The diameter must be an odd number of grid points.")
 
     if np.all(arc_pos == focus_pos):
-        raise ValueError('The focus_pos must be different to the arc_pos.')
+        raise ValueError("The focus_pos must be different to the arc_pos.")
 
     # assign variable names to vector components
     Nx, Ny = grid_size
     ax, ay = arc_pos
     fx, fy = focus_pos
 
     # =========================================================================
     # CREATE ARC
     # =========================================================================
 
     if not np.isinf(radius):
-
         # find half the arc angle
         half_arc_angle = np.arcsin(diameter / 2 / radius)
 
         # find centre of circle on which the arc lies
         distance_cf = np.sqrt((ax - fx) ** 2 + (ay - fy) ** 2)
         cx = round(radius / distance_cf * (fx - ax) + ax)
         cy = round(radius / distance_cf * (fy - ay) + ay)
@@ -1454,19 +1399,18 @@
         # form vector from the geometric arc centre to the arc midpoint
         v1 = arc_pos - c
 
         # calculate length of vector
         l1 = np.sqrt(sum((arc_pos - c) ** 2))
 
         # extract all points that form part of the arc
-        arc_ind = matlab_find(arc, mode='eq', val=1)
+        arc_ind = matlab_find(arc, mode="eq", val=1)
 
         # loop through the arc points
         for arc_ind_i in arc_ind:
-
             # extract the indices of the current point
             x_ind, y_ind = ind2sub([Nx, Ny], arc_ind_i)
             p = np.array([x_ind, y_ind])
 
             # form vector from the geometric arc centre to the current point
             v2 = p - c
 
@@ -1478,22 +1422,21 @@
             theta = np.arccos(sum(v1 * v2 / (l1 * l2)))
 
             # if the angle is greater than the half angle of the arc, remove
             # it from the arc
             if theta > half_arc_angle:
                 arc = matlab_assign(arc, arc_ind_i - 1, 0)
     else:
-
         # calculate arc direction angle, then rotate by 90 degrees
         ang = np.arctan((fx - ax) / (fy - ay)) + np.pi / 2
 
         # draw lines to create arc with infinite radius
         arc = np.logical_or(
             make_line(grid_size, arc_pos, endpoint=None, angle=ang, length=(diameter - 1) // 2),
-            make_line(grid_size, arc_pos, endpoint=None, angle=(ang + np.pi), length=(diameter - 1) // 2)
+            make_line(grid_size, arc_pos, endpoint=None, angle=(ang + np.pi), length=(diameter - 1) // 2),
         )
     return arc
 
 
 def make_pixel_map_point(grid_size: Vector, centre_pos: np.ndarray) -> np.ndarray:
     """
     Generates a map of the distance of each pixel from a given centre position.
@@ -1509,52 +1452,51 @@
         ValueError: If `grid_size` and `centre_pos` do not have the same number of dimensions.
     """
     # check for number of dimensions
     num_dim = len(grid_size)
 
     # check that centre_pos has the same dimensions
     if len(grid_size) != len(centre_pos):
-        raise ValueError('The inputs centre_pos and grid_size must have the same number of dimensions.')
+        raise ValueError("The inputs centre_pos and grid_size must have the same number of dimensions.")
 
     if num_dim == 2:
         # assign inputs and force to be integers
         Nx, Ny = grid_size.astype(int)
         cx, cy = centre_pos.astype(int)
 
         # generate index vectors in each dimension
         nx = np.arange(0, Nx) - cx + 1
         ny = np.arange(0, Ny) - cy + 1
 
         # combine index matrices
         pixel_map = np.zeros((Nx, Ny))
-        pixel_map += (nx ** 2)[:, None]
-        pixel_map += (ny ** 2)[None, :]
+        pixel_map += (nx**2)[:, None]
+        pixel_map += (ny**2)[None, :]
         pixel_map = np.sqrt(pixel_map)
 
     elif num_dim == 3:
-
         # assign inputs and force to be integers
         Nx, Ny, Nz = grid_size.astype(int)
         cx, cy, cz = centre_pos.astype(int)
 
         # generate index vectors in each dimension
         nx = np.arange(0, Nx) - cx + 1
         ny = np.arange(0, Ny) - cy + 1
         nz = np.arange(0, Nz) - cz + 1
 
         # combine index matrices
         pixel_map = np.zeros((Nx, Ny, Nz))
-        pixel_map += (nx ** 2)[:, None, None]
-        pixel_map += (ny ** 2)[None, :, None]
-        pixel_map += (nz ** 2)[None, None, :]
+        pixel_map += (nx**2)[:, None, None]
+        pixel_map += (ny**2)[None, :, None]
+        pixel_map += (nz**2)[None, None, :]
         pixel_map = np.sqrt(pixel_map)
 
     else:
         # throw error
-        raise ValueError('Grid size must be 2 or 3D.')
+        raise ValueError("Grid size must be 2 or 3D.")
 
     return pixel_map
 
 
 def make_pixel_map_plane(grid_size: Vector, normal: np.ndarray, point: np.ndarray) -> np.ndarray:
     """
     Generates a pixel map of a plane with given normal vector and point.
@@ -1567,15 +1509,15 @@
     Returns:
         pixel_map: A 2D array with the distance of each pixel from the given plane.
 
     Raises:
         ValueError: If the normal vector is zero.
     """  # error checking
     if np.all(normal == 0):
-        raise ValueError('Normal vector should not be zero.')
+        raise ValueError("Normal vector should not be zero.")
 
     # check for number of dimensions
     num_dim = len(grid_size)
 
     if num_dim == 2:
         # assign inputs and force to be integers
         Nx = round(grid_size[0])
@@ -1584,50 +1526,47 @@
         # create coordinate meshes
         [px, py] = np.meshgrid(Nx, Ny)
         [pointx, pointy] = np.meshgrid(np.ones((1, Nx)) * point[0], np.ones(1, Ny) * point[1])
         [nx, ny] = np.meshgrid(np.ones((1, Nx)) * normal[0], np.ones(1, Ny) * normal[2])
 
         # calculate distance according to Eq. (6) at
         # http://mathworld.wolfram.com/Point-PlaneDistance.html
-        pixel_map = np.abs((px - pointx) * nx + (py - pointy) * ny) / np.sqrt(sum(normal ** 2))
+        pixel_map = np.abs((px - pointx) * nx + (py - pointy) * ny) / np.sqrt(sum(normal**2))
 
     elif num_dim == 3:
-
         # assign inputs and force to be integers
         Nx = np.round(grid_size[0])
         Ny = np.round(grid_size[1])
         Nz = np.round(grid_size[2])
 
         # create coordinate meshes
-        px, py, pz = np.meshgrid(np.arange(1, Nx + 1), np.arange(1, Ny + 1), np.arange(1, Nz + 1), indexing='ij')
-        pointx, pointy, pointz = np.meshgrid(np.ones(Nx) * point[0], np.ones(Ny) * point[1], np.ones(Nz) * point[2],
-                                             indexing='ij')
-        nx, ny, nz = np.meshgrid(np.ones(Nx) * normal[0], np.ones(Ny) * normal[1], np.ones(Nz) * normal[2],
-                                 indexing='ij')
+        px, py, pz = np.meshgrid(np.arange(1, Nx + 1), np.arange(1, Ny + 1), np.arange(1, Nz + 1), indexing="ij")
+        pointx, pointy, pointz = np.meshgrid(np.ones(Nx) * point[0], np.ones(Ny) * point[1], np.ones(Nz) * point[2], indexing="ij")
+        nx, ny, nz = np.meshgrid(np.ones(Nx) * normal[0], np.ones(Ny) * normal[1], np.ones(Nz) * normal[2], indexing="ij")
 
         # calculate distance according to Eq. (6) at
         # http://mathworld.wolfram.com/Point-PlaneDistance.html
-        pixel_map = np.abs((px - pointx) * nx + (py - pointy) * ny + (pz - pointz) * nz) / np.sqrt(sum(normal ** 2))
+        pixel_map = np.abs((px - pointx) * nx + (py - pointy) * ny + (pz - pointz) * nz) / np.sqrt(sum(normal**2))
 
     else:
         # throw error
-        raise ValueError('Grid size must be 2 or 3D.')
+        raise ValueError("Grid size must be 2 or 3D.")
 
     return pixel_map
 
 
-@beartype
+@typechecker
 def make_bowl(
-    grid_size: Vector, 
-    bowl_pos: Vector, 
-    radius: Union[int, float], 
-    diameter: Union[Number, int, float],
-    focus_pos: Vector, 
-    binary: bool = False, 
-    remove_overlap: bool = False
+    grid_size: Vector,
+    bowl_pos: Vector,
+    radius: Union[int, float],
+    diameter: Real[kt.ScalarLike, ""],
+    focus_pos: Vector,
+    binary: bool = False,
+    remove_overlap: bool = False,
 ) -> Union[kt.NP_ARRAY_BOOL_3D, kt.NP_ARRAY_INT_3D]:
     """
     Generate a matrix representing a bowl-shaped object in 3D space.
 
     This function generates a 3D matrix representing a bowl-shaped object with the specified radius and diameter. The position
     of the bowl and the focus point can be specified, as well as whether to return a binary matrix or a matrix with
     continuous values. The optional parameter 'remove_overlap' can be used to remove any overlap with the surrounding grid.
@@ -1643,17 +1582,17 @@
 
     Returns:
         matrix: 3D matrix representing the bowl-shaped object
 
     Raises:
         ValueError: if any of the input arguments are outside the valid range
     """
-    assert len(grid_size) == 3, 'Grid size must be 3D.'
-    assert len(bowl_pos) == 3, 'Bowl position must be 3D.'
-    assert len(focus_pos) == 3, 'Focus position must be 3D.'
+    assert len(grid_size) == 3, "Grid size must be 3D."
+    assert len(bowl_pos) == 3, "Bowl position must be 3D."
+    assert len(focus_pos) == 3, "Focus position must be 3D."
 
     # =========================================================================
     # DEFINE LITERALS
     # =========================================================================
 
     # threshold used to find the closest point to the radius
     THRESHOLD = 0.5
@@ -1671,27 +1610,27 @@
     bowl_pos = np.round(bowl_pos).astype(int)
     focus_pos = np.round(focus_pos).astype(int)
     diameter = np.round(diameter)
     radius = np.round(radius)
 
     # check the input ranges
     if np.any(grid_size < 1):
-        raise ValueError('The grid size must be positive.')
+        raise ValueError("The grid size must be positive.")
     if np.any(bowl_pos < 1) or np.any(bowl_pos > grid_size):
-        raise ValueError('The centre of the bowl must be within the grid.')
+        raise ValueError("The centre of the bowl must be within the grid.")
     if radius <= 0:
-        raise ValueError('The radius must be positive.')
+        raise ValueError("The radius must be positive.")
     if diameter <= 0:
-        raise ValueError('The diameter must be positive.')
+        raise ValueError("The diameter must be positive.")
     if diameter > (2 * radius):
-        raise ValueError('The diameter of the bowl must be less than twice the radius of curvature.')
+        raise ValueError("The diameter of the bowl must be less than twice the radius of curvature.")
     if diameter % 2 == 0:
-        raise ValueError('The diameter must be an odd number of grid points.')
+        raise ValueError("The diameter must be an odd number of grid points.")
     if np.all(bowl_pos == focus_pos):
-        raise ValueError('The focus_pos must be different to the bowl_pos.')
+        raise ValueError("The focus_pos must be different to the bowl_pos.")
 
     # =========================================================================
     # BOUND THE GRID TO SPEED UP CALCULATION
     # =========================================================================
 
     # create bounding box slightly larger than bowl diameter * sqrt(2)
     Nx = np.round(np.sqrt(2) * diameter).astype(int) + BOUNDING_BOX_EXP
@@ -1718,15 +1657,14 @@
         bowl_sm = np.zeros((Nx, Ny, Nz))
 
     # =========================================================================
     # CREATE DISTANCE MATRIX
     # =========================================================================
 
     if not np.isinf(radius):
-
         # find half the arc angle
         half_arc_angle = np.arcsin(diameter / (2 * radius))
 
         # find centre of sphere on which the bowl lies
         distance_cf = np.sqrt((bx - fx) ** 2 + (by - fy) ** 2 + (bz - fz) ** 2)
         cx = round(radius / distance_cf * (fx - bx) + bx)
         cy = round(radius / distance_cf * (fy - by) + by)
@@ -1736,15 +1674,14 @@
         # generate matrix with distance from the centre
         pixel_map = make_pixel_map_point(grid_size_sm, c)
 
         # set search radius to bowl radius
         search_radius = radius
 
     else:
-
         # generate matrix with distance from the centre
         pixel_map = make_pixel_map_plane(grid_size_sm, bowl_pos_sm - focus_pos_sm, bowl_pos_sm)
 
         # set search radius to 0 (the disc is flat)
         search_radius = 0
 
     # calculate distance from search radius
@@ -1763,16 +1700,16 @@
     # extract the linear index in the y-z plane of the values that lie on the
     # bowl surface
     yz_ind_forw = matlab_find(value_forw < THRESHOLD)
     yz_ind_back = matlab_find(value_back < THRESHOLD)
 
     # use these subscripts to extract the x-index of the grid points that lie
     # on the bowl surface
-    x_ind_forw = index_forw.flatten(order='F')[yz_ind_forw - 1] + 1
-    x_ind_back = index_back.flatten(order='F')[yz_ind_back - 1] + 1
+    x_ind_forw = index_forw.flatten(order="F")[yz_ind_forw - 1] + 1
+    x_ind_back = index_back.flatten(order="F")[yz_ind_back - 1] + 1
 
     # convert the linear index to equivalent subscript values
     y_ind_forw, z_ind_forw = ind2sub([Ny, Nz], yz_ind_forw)
     y_ind_back, z_ind_back = ind2sub([Ny, Nz], yz_ind_back)
 
     # combine x-y-z indices into a linear index
     linear_index_forw = sub2ind([Nx, Ny, Nz], x_ind_forw - 1, y_ind_forw - 1, z_ind_forw - 1) + 1
@@ -1801,16 +1738,16 @@
     # extract the linear index in the y-z plane of the values that lie on the
     # bowl surface
     zx_ind_forw = matlab_find(value_forw < THRESHOLD)
     zx_ind_back = matlab_find(value_back < THRESHOLD)
 
     # use these subscripts to extract the y-index of the grid points that lie
     # on the bowl surface
-    y_ind_forw = index_forw.flatten(order='F')[zx_ind_forw - 1] + 1
-    y_ind_back = index_back.flatten(order='F')[zx_ind_back - 1] + 1
+    y_ind_forw = index_forw.flatten(order="F")[zx_ind_forw - 1] + 1
+    y_ind_back = index_back.flatten(order="F")[zx_ind_back - 1] + 1
 
     # convert the linear index to equivalent subscript values
     z_ind_forw, x_ind_forw = ind2sub([Nz, Nx], zx_ind_forw)
     z_ind_back, x_ind_back = ind2sub([Nz, Nx], zx_ind_back)
 
     # combine x-y-z indices into a linear index
     linear_index_forw = sub2ind([Nx, Ny, Nz], x_ind_forw - 1, y_ind_forw - 1, z_ind_forw - 1) + 1
@@ -1839,16 +1776,16 @@
     # extract the linear index in the y-z plane of the values that lie on the
     # bowl surface
     xy_ind_forw = matlab_find(value_forw < THRESHOLD)
     xy_ind_back = matlab_find(value_back < THRESHOLD)
 
     # use these subscripts to extract the z-index of the grid points that lie
     # on the bowl surface
-    z_ind_forw = index_forw.flatten(order='F')[xy_ind_forw - 1] + 1
-    z_ind_back = index_back.flatten(order='F')[xy_ind_back - 1] + 1
+    z_ind_forw = index_forw.flatten(order="F")[xy_ind_forw - 1] + 1
+    z_ind_back = index_back.flatten(order="F")[xy_ind_back - 1] + 1
 
     # convert the linear index to equivalent subscript values
     x_ind_forw, y_ind_forw = ind2sub([Nx, Ny], xy_ind_forw)
     x_ind_back, y_ind_back = ind2sub([Nx, Ny], xy_ind_back)
 
     # combine x-y-z indices into a linear index
     linear_index_forw = sub2ind([Nx, Ny, Nz], x_ind_forw - 1, y_ind_forw - 1, z_ind_forw - 1) + 1
@@ -1860,25 +1797,23 @@
 
     # =========================================================================
     # RESTRICT SPHERE TO BOWL
     # =========================================================================
 
     # remove grid points within the sphere that do not form part of the bowl
     if not np.isinf(radius):
-
         # form vector from the geometric bowl centre to the back of the bowl
         v1 = bowl_pos_sm - c
 
         # calculate length of vector
         l1 = np.sqrt(sum((bowl_pos_sm - c) ** 2))
 
         # loop through the non-zero elements in the bowl matrix
         bowl_ind = matlab_find(bowl_sm == 1)[:, 0]
         for bowl_ind_i in bowl_ind:
-
             # extract the indices of the current point
             x_ind, y_ind, z_ind = ind2sub([Nx, Ny, Nz], bowl_ind_i)
             p = np.array([x_ind, y_ind, z_ind])
 
             # form vector from the geometric bowl centre to the current point
             # on the bowl
             v2 = p - c
@@ -1895,27 +1830,25 @@
 
             # if the angle is greater than the half angle of the bowl, remove
             # it from the bowl
             if theta > half_arc_angle:
                 bowl_sm = matlab_assign(bowl_sm, bowl_ind_i - 1, 0)
 
     else:
-
         # form a distance map from the centre of the disc
         pixelMapPoint = make_pixel_map_point(grid_size_sm, bowl_pos_sm)
 
         # set all points in the disc greater than the diameter to zero
         bowl_sm[pixelMapPoint > (diameter / 2)] = 0
 
     # =========================================================================
     # REMOVE OVERLAPPED POINTS
     # =========================================================================
 
     if remove_overlap:
-
         # define the shapes that capture the overlapped points, along with the
         # corresponding mask of which point to delete
         overlap_shapes = []
         overlap_delete = []
 
         shape = np.zeros((3, 3, 3))
         shape[0, 0, :] = 1
@@ -2030,69 +1963,55 @@
         # set loop flag
         points_remaining = True
 
         # initialise deleted point counter
         deleted_points = 0
 
         # set list of possible permutations
-        perm_list = [
-            [0, 1, 2],
-            [0, 2, 1],
-            [1, 2, 0],
-            [1, 0, 2],
-            [2, 0, 1],
-            [2, 1, 0]
-        ]
+        perm_list = [[0, 1, 2], [0, 2, 1], [1, 2, 0], [1, 0, 2], [2, 0, 1], [2, 1, 0]]
 
         while points_remaining:
-
             # get linear index of non-zero bowl elements
             index_mat = matlab_find(bowl_sm > 0)[:, 0]
 
             # set Boolean delete variable
             delete_point = False
 
             # loop through all points on the bowl, and find the all the points with
             # more than 8 neighbours
             index = 0
             for index, index_mat_i in enumerate(index_mat):
-
                 # extract subscripts for current point
                 cx, cy, cz = ind2sub([Nx, Ny, Nz], index_mat_i)
 
                 # ignore edge points
                 if (cx > 1) and (cx < Nx) and (cy > 1) and (cy < Ny) and (cz > 1) and (cz < Nz):
-
                     # extract local region around current point
-                    region = bowl_sm[cx - 1:cx + 1, cy - 1:cy + 1, cz - 1:cz + 1]  # FARID might not work
+                    region = bowl_sm[cx - 1 : cx + 1, cy - 1 : cy + 1, cz - 1 : cz + 1]  # FARID might not work
 
                     # if there's more than 8 neighbours, check the point for
                     # deletion
                     if (region.sum() - 1) > 8:
-
                         # loop through the different shapes
                         for shape_index in range(len(overlap_shapes)):
-
                             # check every permutation of the shape, and apply the
                             # deletion mask if the pattern matches
 
                             # loop through possible shape permutations
                             for ind1 in range(len(perm_list)):
-
                                 # get shape and delete mask
                                 overlap_s = overlap_shapes[shape_index]
                                 overlap_d = overlap_delete[shape_index]
 
                                 # permute
                                 overlap_s = np.transpose(overlap_s, perm_list[ind1])
                                 overlap_d = np.transpose(overlap_d, perm_list[ind1])
 
                                 # loop through possible shape reflections
                                 for ind2 in range(1, 8):
-
                                     # flipfunc the shape
                                     if ind2 == 2:
                                         overlap_s = np.flip(overlap_s, axis=0)
                                         overlap_d = np.flip(overlap_d, axis=0)
                                     elif ind2 == 3:
                                         overlap_s = np.flip(overlap_s, axis=1)
                                         overlap_d = np.flip(overlap_d, axis=1)
@@ -2107,15 +2026,14 @@
                                         overlap_d = np.flip(np.flip(overlap_d, axis=0), axis=2)
                                     elif ind2 == 7:
                                         overlap_s = np.flip(np.flip(overlap_s, axis=1), axis=2)
                                         overlap_d = np.flip(np.flip(overlap_d, axis=1), axis=2)
 
                                     # rotate the shape 4 x 90 degrees
                                     for ind3 in range(4):
-
                                         # check if the shape matches
                                         if np.all(overlap_s == region):
                                             delete_point = True
 
                                         # break from loop if a match is found
                                         if delete_point:
                                             break
@@ -2131,33 +2049,32 @@
                                 # break from loop if a match is found
                                 if delete_point:
                                     break
 
                             # remove point from bowl if required, and update
                             # counter
                             if delete_point:
-                                bowl_sm[cx - 1:cx + 1, cy - 1:cy + 1, cz - 1:cz + 1] = bowl_sm[cx - 1:cx + 1,
-                                                                                       cy - 1:cy + 1,
-                                                                                       cz - 1:cz + 1] * np.bitwise_not(
-                                    overlap_d).astype(float)  # Farid won't work probably
+                                bowl_sm[cx - 1 : cx + 1, cy - 1 : cy + 1, cz - 1 : cz + 1] = bowl_sm[
+                                    cx - 1 : cx + 1, cy - 1 : cy + 1, cz - 1 : cz + 1
+                                ] * np.bitwise_not(overlap_d).astype(float)  # Farid won't work probably
                                 deleted_points = deleted_points + 1
                                 break
 
                 # break from loop if a match is found
                 if delete_point:
                     break
 
             # break from while loop if the outer for loop has completed
             # without deleting a point
             if index == (len(index_mat) - 1):
                 points_remaining = False
 
         # display status
         if deleted_points:
-            logging.log(logging.INFO, '{deleted_points} overlapped points removed from bowl')
+            logging.log(logging.INFO, "{deleted_points} overlapped points removed from bowl")
 
     # =========================================================================
     # PLACE BOWL WITHIN LARGER GRID
     # =========================================================================
 
     # preallocate storage variable
     if binary:
@@ -2171,21 +2088,21 @@
     y1 = bowl_pos[1] - by
     y2 = y1 + Ny
     z1 = bowl_pos[2] - bz
     z2 = z1 + Nz
 
     # truncate bounding box if it falls outside the grid
     if x1 < 0:
-        bowl_sm = bowl_sm[abs(x1):, :, :]
+        bowl_sm = bowl_sm[abs(x1) :, :, :]
         x1 = 0
     if y1 < 0:
-        bowl_sm = bowl_sm[:, abs(y1):, :]
+        bowl_sm = bowl_sm[:, abs(y1) :, :]
         y1 = 0
     if z1 < 0:
-        bowl_sm = bowl_sm[:, :, abs(z1):]
+        bowl_sm = bowl_sm[:, :, abs(z1) :]
         z1 = 0
     if x2 >= grid_size[0]:
         to_delete = x2 - grid_size[0]
         bowl_sm = bowl_sm[:-to_delete, :, :]
         x2 = grid_size[0]
     if y2 >= grid_size[1]:
         to_delete = y2 - grid_size[1]
@@ -2199,21 +2116,21 @@
     # place bowl into grid
     bowl[x1:x2, y1:y2, z1:z2] = bowl_sm
 
     return bowl
 
 
 def make_multi_bowl(
-    grid_size: Vector, 
-    bowl_pos: List[Tuple[int, int]], 
-    radius: int, 
+    grid_size: Vector,
+    bowl_pos: List[Tuple[int, int]],
+    radius: int,
     diameter: int,
     focus_pos: Tuple[int, int],
     binary: bool = False,
-    remove_overlap: bool = False
+    remove_overlap: bool = False,
 ) -> Tuple[np.ndarray, List[np.ndarray]]:
     """
     Generates a multi-bowl mask for an image given the size of the grid, the positions of the bowls,
     the radius of each bowl, the diameter of the bowls, and the position of the focus.
 
     Args:
         grid_size: The size of the grid (assumed to be square).
@@ -2227,21 +2144,21 @@
     Returns:
         bowls:
         bowls_labeled:
     """
 
     # check inputs
     if bowl_pos.shape[-1] != 3:
-        raise ValueError('bowl_pos should contain 3 columns, with [bx, by, bz] in each row.')
+        raise ValueError("bowl_pos should contain 3 columns, with [bx, by, bz] in each row.")
 
     if len(radius) != 1 and len(radius) != bowl_pos.shape[0]:
-        raise ValueError('The number of rows in bowl_pos and radius does not match.')
+        raise ValueError("The number of rows in bowl_pos and radius does not match.")
 
     if len(diameter) != 1 and len(diameter) != bowl_pos.shape[0]:
-        raise ValueError('The number of rows in bowl_pos and diameter does not match.')
+        raise ValueError("The number of rows in bowl_pos and diameter does not match.")
 
     # force integer grid size values
     grid_size = np.round(grid_size).astype(int)
     bowl_pos = np.round(bowl_pos).astype(int)
     focus_pos = np.round(focus_pos).astype(int)
     diameter = np.round(diameter)
     radius = np.round(radius)
@@ -2256,21 +2173,20 @@
     else:
         bowls = np.zeros(grid_size)
 
     bowls_labelled = np.zeros(grid_size)
 
     # loop for calling make_bowl
     for bowl_index in range(bowl_pos.shape[0]):
-
         # update command line status
         if bowl_index == 1:
             TicToc.tic()
         else:
             TicToc.toc(reset=True)
-        logging.log(logging.INFO, f'Creating bowl {bowl_index} of {bowl_pos.shape[0]} ... ')
+        logging.log(logging.INFO, f"Creating bowl {bowl_index} of {bowl_pos.shape[0]} ... ")
 
         # get parameters for current bowl
         if bowl_pos.shape[0] > 1:
             bowl_pos_k = bowl_pos[bowl_index]
         else:
             bowl_pos_k = bowl_pos
         bowl_pos_k = Vector(bowl_pos_k)
@@ -2288,46 +2204,39 @@
         if focus_pos.shape[0] > 1:
             focus_pos_k = focus_pos[bowl_index]
         else:
             focus_pos_k = focus_pos
         focus_pos_k = Vector(focus_pos_k)
 
         # create new bowl
-        new_bowl = make_bowl(
-            grid_size, bowl_pos_k, radius_k, diameter_k, focus_pos_k,
-            remove_overlap=remove_overlap, binary=binary
-        )
+        new_bowl = make_bowl(grid_size, bowl_pos_k, radius_k, diameter_k, focus_pos_k, remove_overlap=remove_overlap, binary=binary)
 
         # add bowl to bowl matrix
         bowls = bowls + new_bowl
 
         # add new bowl to labelling matrix
         bowls_labelled[new_bowl == 1] = bowl_index
 
     TicToc.toc()
 
     # check if any of the bowls are overlapping
     max_nd_val, _ = max_nd(bowls)
     if max_nd_val > 1:
         # display warning
-        logging.log(logging.WARN,  f'{max_nd_val - 1} bowls are overlapping')
+        logging.log(logging.WARN, f"{max_nd_val - 1} bowls are overlapping")
 
         # force the output to be binary
         bowls[bowls != 0] = 1
 
     return bowls, bowls_labelled
 
 
-@beartype
+@typechecker
 def make_multi_arc(
-    grid_size: Vector,
-    arc_pos: np.ndarray,
-    radius: Union[int, np.ndarray],
-    diameter: Union[int, np.ndarray], 
-    focus_pos: np.ndarray
+    grid_size: Vector, arc_pos: np.ndarray, radius: Union[int, np.ndarray], diameter: Union[int, np.ndarray], focus_pos: np.ndarray
 ) -> Tuple[kt.NP_ARRAY_FLOAT_2D, kt.NP_ARRAY_FLOAT_2D]:
     """
     Generates a multi-arc mask for an image given the size of the grid,
     the positions and properties of the arcs, and the position of the focus.
 
     Args:
         grid_size: The size of the grid (assumed to be square).
@@ -2342,21 +2251,21 @@
 
     Raises:
         ValueError: If the shape of arc_pos is not (N, 2), if the number of rows in arc_pos and radius do not match,
                     or if the number of rows in arc_pos and diameter do not match.
     """
     # check inputs
     if arc_pos.shape[-1] != 2:
-        raise ValueError('arc_pos should contain 2 columns, with [ax, ay] in each row.')
+        raise ValueError("arc_pos should contain 2 columns, with [ax, ay] in each row.")
 
     if len(radius) != 1 and len(radius) != arc_pos.shape[0]:
-        raise ValueError('The number of rows in arc_pos and radius does not match.')
+        raise ValueError("The number of rows in arc_pos and radius does not match.")
 
     if len(diameter) != 1 and len(diameter) != arc_pos.shape[0]:
-        raise ValueError('The number of rows in arc_pos and diameter does not match.')
+        raise ValueError("The number of rows in arc_pos and diameter does not match.")
 
     # force integer grid size values
     grid_size = grid_size.round().astype(int)
     arc_pos = arc_pos.round().astype(int)
     diameter = diameter.round()
     focus_pos = focus_pos.round().astype(int)
     radius = radius.round()
@@ -2367,15 +2276,14 @@
 
     # create empty matrix
     arcs = np.zeros(grid_size)
     arcs_labelled = np.zeros(grid_size)
 
     # loop for calling make_arc
     for k in range(arc_pos.shape[0]):
-
         # get parameters for current arc
         if arc_pos.shape[0] > 1:
             arc_pos_k = arc_pos[k]
         else:
             arc_pos_k = arc_pos
 
         if len(radius) > 1:
@@ -2402,43 +2310,40 @@
         # add new arc to labelling matrix
         arcs_labelled[new_arc == 1] = k
 
     # check if any of the arcs are overlapping
     max_nd_val, _ = max_nd(arcs)
     if max_nd_val > 1:
         # display warning
-        logging.log(logging.WARN,  f'{max_nd_val - 1} arcs are overlapping')
+        logging.log(logging.WARN, f"{max_nd_val - 1} arcs are overlapping")
 
         # force the output to be binary
         arcs[arcs != 0] = 1
 
     return arcs, arcs_labelled
 
 
-@beartype
+@typechecker
 def make_sphere(
-    grid_size: Vector, 
-    radius: Union[float, int], 
-    plot_sphere: bool = False,
-    binary: bool = False
+    grid_size: Vector, radius: Union[float, int], plot_sphere: bool = False, binary: bool = False
 ) -> Union[kt.NP_ARRAY_INT_3D, kt.NP_ARRAY_BOOL_3D]:
     """
     Generates a sphere mask for a 3D grid given the dimensions of the grid, the radius of the sphere,
         and optional flags to plot the sphere and/or return a binary mask.
 
     Args:
         grid_size: The size of the grid (assumed to be cubic).
         radius: The radius of the sphere.
         plot_sphere: Whether to plot the sphere (default: False).
         binary: Whether to return a binary mask (default: False).
 
     Returns:
         sphere: The sphere mask as a NumPy array.
     """
-    assert len(grid_size) == 3, 'grid_size must be a 3D vector'
+    assert len(grid_size) == 3, "grid_size must be a 3D vector"
 
     # enforce a centered sphere
     center = np.floor(grid_size / 2).astype(int) + 1
 
     # preallocate the storage variable
     if binary:
         sphere = np.zeros(grid_size, dtype=bool)
@@ -2448,15 +2353,14 @@
     # create a guide circle from which the individal radii can be extracted
     guide_circle = make_circle(np.flip(grid_size[:2]), np.flip(center[:2]), radius)
 
     # step through the guide circle points and create partially filled discs
     centerpoints = np.arange(center.x - radius, center.x + 1)
     reflection_offset = np.arange(len(centerpoints), 1, -1)
     for centerpoint_index in range(len(centerpoints)):
-
         # extract the current row from the guide circle
         row_data = guide_circle[:, centerpoints[centerpoint_index] - 1]
 
         # add an index to the grid points in the current row
         row_index = row_data * np.arange(1, len(row_data) + 1)
 
         # calculate the radius
@@ -2470,15 +2374,14 @@
             circle_fill = np.zeros(grid_size[1:], dtype=bool)
         else:
             circle_fill = np.zeros(grid_size[1:])
 
         # fill in the circle line by line
         fill_centerpoints = np.arange(center.z - swept_radius, center.z + swept_radius + 1).astype(int)
         for fill_centerpoints_i in fill_centerpoints:
-
             # extract the first row
             row_data = circle[:, fill_centerpoints_i - 1]
 
             # add an index to the grid points in the current row
             row_index = row_data * np.arange(1, len(row_data) + 1)
 
             # calculate the diameter
@@ -2486,16 +2389,15 @@
             stop_index = row_index.max()
 
             # count how many points on the line
             num_points = sum(row_data)
 
             # fill in the line
             if start_index != stop_index and (stop_index - start_index) >= num_points:
-                circle_fill[(start_index + num_points // 2) - 1:stop_index - (num_points // 2),
-                fill_centerpoints_i - 1] = 1
+                circle_fill[(start_index + num_points // 2) - 1 : stop_index - (num_points // 2), fill_centerpoints_i - 1] = 1
 
         # remove points from the filled circle that existed in the previous
         # layer
         if centerpoint_index == 0:
             sphere[centerpoints[centerpoint_index] - 1, :, :] = circle + circle_fill
             prev_circle = circle + circle_fill
         else:
@@ -2503,31 +2405,29 @@
             circle_fill = circle_fill - prev_circle
             circle_fill[circle_fill < 0] = 0
             sphere[centerpoints[centerpoint_index] - 1, :, :] = circle + circle_fill
             prev_circle = prev_circle_alt
 
         # create the other half of the sphere at the same time
         if centerpoint_index != len(centerpoints) - 1:
-            sphere[center.x + reflection_offset[centerpoint_index] - 2, :, :] = sphere[
-                                                                                centerpoints[centerpoint_index] - 1, :,
-                                                                                :]
+            sphere[center.x + reflection_offset[centerpoint_index] - 2, :, :] = sphere[centerpoints[centerpoint_index] - 1, :, :]
 
     # plot results
     if plot_sphere:
         raise NotImplementedError
     return sphere
 
 
-@beartype
+@typechecker
 def make_spherical_section(
-    radius: Union[float, int], 
-    height: Union[float, int], 
-    width: Optional[Union[float, int]] = None, 
+    radius: Real[kt.ScalarLike, ""],
+    height: Real[kt.ScalarLike, ""],
+    width: Optional[Real[kt.ScalarLike, ""]] = None,
     plot_section: bool = False,
-    binary: bool = False
+    binary: bool = False,
 ) -> Tuple:
     """
     Generates a spherical section mask given the radius and height of the section and
         optional parameters to specify the width and/or plot and return a binary mask.
 
     Args:
         radius: The radius of the spherical section.
@@ -2546,19 +2446,19 @@
     """
     use_spherical_sections = True
 
     # force inputs to be integers
     radius = int(radius)
     height = int(height)
 
-    use_width = (width is not None)
+    use_width = width is not None
     if use_width:
         width = int(width)
         if width % 2 == 0:
-            raise ValueError('Input width must be an odd number.')
+            raise ValueError("Input width must be an odd number.")
 
     # calculate minimum grid dimensions to fit entire sphere
     Nx = 2 * radius + 1
 
     # create sphere
     ss = make_sphere(Vector([Nx] * 3), radius, False, binary)
 
@@ -2576,18 +2476,17 @@
 
     # truncate transducer grid based on length (removes empty rows and columns)
     offset = int((Nx - length) / 2)
     ss = ss[:, offset:-offset, offset:-offset]
 
     # also truncate to given width if defined by user
     if use_width:
-
         # check the value is appropriate
         if width > length:
-            raise ValueError('Input for width must be less than or equal to transducer length.')
+            raise ValueError("Input for width must be less than or equal to transducer length.")
 
         # calculate offset
         offset = int((length - width) / 2)
 
         # truncate transducer grid
         ss = ss[:, offset:-offset, :]
 
@@ -2598,85 +2497,81 @@
     mx, mx_ind = np.max(ss, axis=0), ss.argmax(axis=0) + 1
     mask = np.squeeze(mx != 0)
     mx_ind = np.squeeze(mx_ind) * mask
 
     # double check there there is only one value of spherical section in
     # each matrix column
     if mx.sum() != ss.sum():
-        raise ValueError(
-            'mean neighbour distance cannot be calculated uniquely due to overlapping points in the x-direction')
+        raise ValueError("mean neighbour distance cannot be calculated uniquely due to overlapping points in the x-direction")
 
     # calculate average distance to grid point neighbours in the flat case
     x_dist = np.tile([1, 0, 1], [3, 1])
     y_dist = x_dist.T
-    flat_dist = np.sqrt(x_dist ** 2 + y_dist ** 2)
+    flat_dist = np.sqrt(x_dist**2 + y_dist**2)
     flat_dist = np.mean(flat_dist)
 
     # compute distance map
     dist_map = np.zeros(mx_ind.shape)
     sz = mx_ind.shape
     for m in range(sz[0]):
         for n in range(sz[1]):
-
             # clear map
             local_heights = np.zeros((3, 3))
 
             # extract the height (x-distance) of the 8 neighbouring grid
             # points
             if m == 0 and n == 0:
-                local_heights[1:3, 1:3] = mx_ind[m:m + 2, n:n + 2]
+                local_heights[1:3, 1:3] = mx_ind[m : m + 2, n : n + 2]
             elif m == (sz[0] - 1) and n == (sz[1] - 1):
-                local_heights[0:2, 0:2] = mx_ind[m - 1:m + 1, n - 1:n + 1]
+                local_heights[0:2, 0:2] = mx_ind[m - 1 : m + 1, n - 1 : n + 1]
             elif m == 0 and n == (sz[1] - 1):
-                local_heights[1:3, 0:2] = mx_ind[m:m + 2, n - 1:n + 1]
+                local_heights[1:3, 0:2] = mx_ind[m : m + 2, n - 1 : n + 1]
             elif m == (sz[0] - 1) and n == 0:
-                local_heights[0:2, 1:3] = mx_ind[m - 1:m + 1, n:n + 2]
+                local_heights[0:2, 1:3] = mx_ind[m - 1 : m + 1, n : n + 2]
             elif m == 0:
-                local_heights[1:3, :] = mx_ind[m:m + 2, n - 1:n + 2]
+                local_heights[1:3, :] = mx_ind[m : m + 2, n - 1 : n + 2]
             elif m == (sz[0] - 1):
-                local_heights[0:2, :] = mx_ind[m - 1:m + 1, n - 1:n + 2]
+                local_heights[0:2, :] = mx_ind[m - 1 : m + 1, n - 1 : n + 2]
             elif n == 0:
-                local_heights[:, 1:3] = mx_ind[m - 1:m + 2, n:n + 2]
+                local_heights[:, 1:3] = mx_ind[m - 1 : m + 2, n : n + 2]
             elif n == (sz[1] - 1):
-                local_heights[:, 0:2] = mx_ind[m - 1:m + 2, n - 1:n + 1]
+                local_heights[:, 0:2] = mx_ind[m - 1 : m + 2, n - 1 : n + 1]
             else:
-                local_heights = mx_ind[m - 1:m + 2, n - 1:n + 2]
+                local_heights = mx_ind[m - 1 : m + 2, n - 1 : n + 2]
 
             # compute average variation from center
             local_heights_var = abs(local_heights - local_heights[1, 1])
 
             # threshold no neighbours
             local_heights_var[local_heights == 0] = 0
 
             # calculate total distance from centre
-            dist = np.sqrt(x_dist ** 2 + y_dist ** 2 + local_heights_var ** 2)
+            dist = np.sqrt(x_dist**2 + y_dist**2 + local_heights_var**2)
 
             # average and store as a ratio
             dist_map[m, n] = 1 + (np.mean(dist) - flat_dist) / flat_dist
 
     # threshold out the non-transducer grid points
     dist_map[mask != 1] = 0
 
     # plot if required
     if plot_section:
         raise NotImplementedError
 
     return ss, dist_map
 
 
-@beartype
+@typechecker
 def make_cart_rect(
-    rect_pos, 
-    Lx: Union[float, int], 
-    Ly: Union[float, int], 
-    theta: Optional[Union[
-        int, float, List, 
-        kt.NP_ARRAY_INT_1D, kt.NP_ARRAY_FLOAT_1D]]=None, 
-    num_points: int=0, 
-    plot_rect: bool=False
+    rect_pos,
+    Lx: Real[kt.ScalarLike, ""],
+    Ly: Real[kt.ScalarLike, ""],
+    theta: Optional[Union[Real[kt.ScalarLike, ""], List, Integer[np.ndarray, "..."], Float[np.ndarray, "..."]]] = None,
+    num_points: int = 0,
+    plot_rect: bool = False,
 ) -> Union[kt.NP_ARRAY_FLOAT_2D, kt.NP_ARRAY_FLOAT_3D]:
     """
     Create evenly distributed Cartesian points covering a rectangle.
 
     Args:
     rect_pos : List. Cartesian position of the centre of the rectangle.
     Lx : Float. Height of the rectangle (along the x-coordinate before rotation).
@@ -2699,36 +2594,33 @@
     # Distance between points in each dimension
     d_x = 2 / npts_x
     d_y = 2 / npts_y
 
     # Compute canonical rectangle points ([-1, 1] x [-1, 1], z=0 plane)
     p_x = np.linspace(-1 + d_x / 2, 1 - d_x / 2, npts_x)
     p_y = np.linspace(-1 + d_y / 2, 1 - d_y / 2, npts_y)
-    P_x, P_y = np.meshgrid(p_x, p_y, indexing='ij')
+    P_x, P_y = np.meshgrid(p_x, p_y, indexing="ij")
     p0 = np.stack((P_x.flatten(), P_y.flatten()), axis=0)
 
     # Add z-dimension points if in 3D
     if len(rect_pos) == 3:
         p0 = np.vstack((p0, np.zeros(num_points)))
 
     # Transform the canonical rectangle points to give the specified rectangle
     if len(rect_pos) == 2:
-
         # Scaling transformation
         S = np.array([[Lx, 0], [0, Ly]]) / 2
 
         # Rotation
         if theta is None:
             R = np.eye(2)
         else:
-            R = np.array([[cosd(theta), -sind(theta)],
-                          [sind(theta), cosd(theta)]])
+            R = np.array([[cosd(theta), -sind(theta)], [sind(theta), cosd(theta)]])
 
     else:
-
         # Scaling transformation
         S = np.array([[Lx, 0, 0], [0, Ly, 0], [0, 0, 2]]) / 2
 
         # Rotation
         if theta is None:
             # No rotation
             R = np.eye(3)
@@ -2744,33 +2636,25 @@
 
     # Shift the rectangle to the appropriate centre
     rect = p0 + np.expand_dims(np.array(rect_pos), axis=1)
 
     return rect
 
 
-@beartype
+@typechecker
 def focused_bowl_oneil(
-    radius: kt.NUMERIC, 
-    diameter: kt.NUMERIC, 
-    velocity: kt.NUMERIC, 
-    frequency: kt.NUMERIC, 
+    radius: kt.NUMERIC,
+    diameter: kt.NUMERIC,
+    velocity: kt.NUMERIC,
+    frequency: kt.NUMERIC,
     sound_speed: kt.NUMERIC,
-    density: kt.NUMERIC, 
-    axial_positions: Optional[
-        Union[kt.NP_ARRAY_FLOAT_1D, float, List]
-    ] = None,
-    lateral_positions: Optional[
-        Union[kt.NP_ARRAY_FLOAT_1D, float, List]
-    ] = None
-) -> Tuple[
-    Optional[kt.NP_ARRAY_FLOAT_1D], 
-    Optional[kt.NP_ARRAY_FLOAT_1D], 
-    Optional[kt.NP_ARRAY_COMPLEX_1D]
-]:
+    density: kt.NUMERIC,
+    axial_positions: Optional[Union[kt.NP_ARRAY_FLOAT_1D, float, List]] = None,
+    lateral_positions: Optional[Union[kt.NP_ARRAY_FLOAT_1D, float, List]] = None,
+) -> Tuple[Optional[kt.NP_ARRAY_FLOAT_1D], Optional[kt.NP_ARRAY_FLOAT_1D], Optional[kt.NP_ARRAY_COMPLEX_1D]]:
     """
     Calculates O'Neil's solution for the axial and lateral pressure amplitude generated by a focused bowl transducer.
 
     Args:
         radius: The radius of the transducer.
         diameter: The diameter of the transducer.
         velocity: The normal surface velocity of the transducer.
@@ -2807,19 +2691,16 @@
 
     References:
         O'Neil, H. (1949). Theory of focusing radiators. J. Acoust. Soc. Am., 21(5), 516-526.
     """
 
     float_eps = np.finfo(float).eps
 
-    # @beartype  => could not figure out what's wrong with type annotation here, revisit in the future
-    def calculate_axial_pressure() -> Tuple[
-                                        NDArray[Shape["N"], Float], 
-                                        NDArray[Shape["N"], Complex]
-                                    ]:
+    # @typechecker  => could not figure out what's wrong with type annotation here, revisit in the future
+    def calculate_axial_pressure() -> Tuple[Float[np.ndarray, "N"], Complex[np.ndarray, "N"]]:
         # calculate distances
         B = np.sqrt((axial_positions - h) ** 2 + (diameter / 2) ** 2)
         d = B - axial_positions
         E = 2 / (1 - axial_positions / radius)
         M = (B + axial_positions) / 2
 
         # compute pressure
@@ -2831,52 +2712,54 @@
         # calculate magnitude of the on - axis pressure  (Eq. 3.0)
         axial_pressure = density * sound_speed * velocity * np.abs(P)
         # calculate complex magnitude of the on - axis pressure assuming t = 0 (Eq. 3.0)
         complex_axial_pressure = density * sound_speed * velocity * P * 1j * np.exp(-1j * k * M)
 
         return axial_pressure, complex_axial_pressure
 
-    @beartype
-    def calculate_lateral_pressure() -> NDArray[Shape["N"], Float]:
+    @typechecker
+    def calculate_lateral_pressure() -> Float[np.ndarray, "N"]:
         # calculate magnitude of the lateral pressure at the geometric focus
         Z = k * lateral_positions * diameter / (2 * radius)
         # TODO: this should work
         # assert np.all(Z) > 0, 'Z must be greater than 0'
-        lateral_pressure = 2. * density * sound_speed * velocity * k * h * scipy.special.jv(1, Z) / Z
+        lateral_pressure = 2.0 * density * sound_speed * velocity * k * h * scipy.special.jv(1, Z) / Z
 
         # replace origin with limit
         lateral_pressure[lateral_positions == 0] = density * sound_speed * velocity * k * h
         return lateral_pressure
 
     # wave number
     k = 2 * np.pi * frequency / sound_speed
 
     # height of rim
-    h = radius - np.sqrt(radius ** 2 - (diameter / 2) ** 2)
+    h = radius - np.sqrt(radius**2 - (diameter / 2) ** 2)
 
     p_axial = None
     p_lateral = None
     p_axial_complex = None
 
     if lateral_positions is not None:
         p_lateral = calculate_lateral_pressure()
     if axial_positions is not None:
         p_axial, p_axial_complex = calculate_axial_pressure()
     return p_axial, p_lateral, p_axial_complex
 
 
-@beartype
-def focused_annulus_oneil(radius: float,
-                          diameter: Union[NDArray[Shape["NumElements, 2"], Float], NDArray[Shape["2, NumElements"], Float]],
-                          amplitude: NDArray[Shape["NumElements"], Float],
-                          phase: NDArray[Shape["NumElements"], Float],
-                          frequency: kt.NUMERIC,
-                          sound_speed: kt.NUMERIC,
-                          density: kt.NUMERIC,
-                          axial_positions: Union[kt.NP_ARRAY_FLOAT_1D, float, list]) -> Union[kt.NP_ARRAY_FLOAT_1D, float]:
+@typechecker
+def focused_annulus_oneil(
+    radius: float,
+    diameter: Union[Float[np.ndarray, "NumElements 2"], Float[np.ndarray, "2 NumElements"]],
+    amplitude: Float[np.ndarray, "NumElements"],
+    phase: Float[np.ndarray, "NumElements"],
+    frequency: kt.NUMERIC,
+    sound_speed: kt.NUMERIC,
+    density: kt.NUMERIC,
+    axial_positions: Union[kt.NP_ARRAY_FLOAT_1D, float, list],
+) -> Union[kt.NP_ARRAY_FLOAT_1D, float]:
     """Compute axial pressure for focused annulus transducer using O'Neil's solution
 
     focused_annulus_oneil calculates the axial pressure for a focused
     annular transducer using O'Neil's solution (O'Neil, H. Theory of
     focusing radiators. J. Acoust. Soc. Am., 21(5), 516-526, 1949). The
     annuluar elements are uniformly driven by a continuous wave sinusoid
     at a given frequency and normal surface velocity.
@@ -2919,79 +2802,77 @@
 
     References:
         O'Neil, H. (1949). Theory of focusing radiators. J. Acoust. Soc. Am., 21(5), 516-526.
 
     See also focused_bowl_oneil.
     """
 
-    if (not np.greater_equal(diameter, np.zeros_like(diameter)).all() or not np.isreal(diameter).all() 
-        or not np.isfinite(diameter).all()): 
+    if not np.greater_equal(diameter, np.zeros_like(diameter)).all() or not np.isreal(diameter).all() or not np.isfinite(diameter).all():
         raise ValueError("wrong values in diameter object")
 
-    if not np.all(np.isfinite(amplitude)): 
+    if not np.all(np.isfinite(amplitude)):
         raise ValueError("amplitude contains an np.inf")
     if not np.all(np.isfinite(frequency)):
-         raise ValueError("frequency contains an np.inf")
+        raise ValueError("frequency contains an np.inf")
 
     # set the number of elements in annular array
     num_elements: int = np.size(amplitude)
 
-    if ((radius <= 0.0) or not np.isreal(radius) or not np.isfinite(radius)): 
+    if (radius <= 0.0) or not np.isreal(radius) or not np.isfinite(radius):
         raise ValueError("radius is incorrect")
 
-    if (((phase < -np.pi).any() or (phase > np.pi).any()) or not np.isreal(phase).any()
-        or not np.isfinite(phase).all()):
+    if ((phase < -np.pi).any() or (phase > np.pi).any()) or not np.isreal(phase).any() or not np.isfinite(phase).all():
         raise ValueError("phase is incorrect")
 
-    if (np.shape(diameter)[0] != 2):
+    if np.shape(diameter)[0] != 2:
         diameter = np.transpose(diameter)
 
     # pre-allocate output
     p_axial = np.zeros(np.shape(axial_positions))
 
     # loop over elements and sum fields
     for ind in range(num_elements):
-
         # get complex pressure for bowls with inner and outer aperature diameter
-        if (diameter[0, ind] == 0):
+        if diameter[0, ind] == 0:
             p_el_inner = 0.0 + 0.0j
         else:
-            _, _, p_el_inner = focused_bowl_oneil(radius, diameter[0, ind], amplitude[ind], frequency,
-                                                  sound_speed, density, axial_positions=axial_positions)
+            _, _, p_el_inner = focused_bowl_oneil(
+                radius, diameter[0, ind], amplitude[ind], frequency, sound_speed, density, axial_positions=axial_positions
+            )
 
-        _, _, p_el_outer = focused_bowl_oneil(radius, diameter[1, ind], amplitude[ind], frequency,
-                                              sound_speed, density, axial_positions=axial_positions)
+        _, _, p_el_outer = focused_bowl_oneil(
+            radius, diameter[1, ind], amplitude[ind], frequency, sound_speed, density, axial_positions=axial_positions
+        )
 
         # pressure for annular element
         p_el = p_el_outer - p_el_inner
 
         # account for phase
         p_el = np.abs(p_el) * np.exp(1.0j * (np.angle(p_el) + phase[ind]))
 
         # add to complete response
         p_axial = p_axial + p_el
 
     # take magnitude of complete response
     return np.abs(p_axial)
 
 
-
 def ndgrid(*args):
-    return np.array(np.meshgrid(*args, indexing='ij'))
+    return np.array(np.meshgrid(*args, indexing="ij"))
 
 
 def trim_cart_points(kgrid, points: np.ndarray):
     """
-        trim_cart_points filters a dim x num_points array of Cartesian points
-        so that only those within the bounds of a given kgrid remain.
-        :param kgrid: Object of the kWaveGrid class defining the Cartesian
-                      and k-space grid fields.
-        :param points: dim x num_points array of Cartesian coordinates to trim [m].
-        :return: dim x num_points array of Cartesian coordinates that lie within the grid defined by kgrid [m].
-        """
+    trim_cart_points filters a dim x num_points array of Cartesian points
+    so that only those within the bounds of a given kgrid remain.
+    :param kgrid: Object of the kWaveGrid class defining the Cartesian
+                  and k-space grid fields.
+    :param points: dim x num_points array of Cartesian coordinates to trim [m].
+    :return: dim x num_points array of Cartesian coordinates that lie within the grid defined by kgrid [m].
+    """
 
     # find indices for points within the simulation domain
     ind_x = (points[0, :] >= kgrid.x_vec[0]) & (points[0, :] <= kgrid.x_vec[-1])
 
     if kgrid.dim > 1:
         ind_y = (points[1, :] >= kgrid.y_vec[0]) & (points[1, :] <= kgrid.y_vec[-1])
 
@@ -3008,23 +2889,23 @@
 
     # output only valid points
     points = points[:, ind]
 
     return points
 
 
-@beartype
+@typechecker
 def make_cart_arc(
-    arc_pos: Vector, 
-    radius: Union[float, int], 
-    diameter: int, 
-    focus_pos: Vector, 
+    arc_pos: Float[np.ndarray, "2"],
+    radius: Union[float, int],
+    diameter: Union[float, int],
+    focus_pos: Float[np.ndarray, "2"],
     num_points: int,
-    plot_arc: bool = False
-) -> NDArray[Shape["2, NumPoints"], Float]:
+    plot_arc: bool = False,
+) -> Float[np.ndarray, "2 NumPoints"]:
     """
     make_cart_arc creates a 2 x num_points array of the Cartesian
     coordinates of points evenly distributed over an arc. The midpoint of
     the arc is set by arc_pos. The orientation of the arc is set by
     focus_pos, which corresponds to any point on the axis of the arc
     (note, this must not be equal to arc_pos). It is assumed that the arc
     angle is equal to or less than pi radians. If the radius is set to
@@ -3079,29 +2960,25 @@
     # Plot results
     if plot_arc:
         # Select suitable axis scaling factor
         _, scale, prefix, _ = scale_SI(np.max(np.abs(arc)))
 
         # Create the figure
         plt.figure()
-        plt.plot(arc[1, :] * scale, arc[0, :] * scale, 'b.')
+        plt.plot(arc[1, :] * scale, arc[0, :] * scale, "b.")
         plt.gca().invert_yaxis()
         plt.xlabel(f"y-position [{prefix}m]")
         plt.ylabel(f"x-position [{prefix}m]")
         plt.axis("equal")
         plt.show()
 
     return arc
 
 
-def compute_linear_transform2D(
-    arc_pos: Vector, 
-    radius: float, 
-    focus_pos: Vector
-) -> Tuple[np.ndarray, np.ndarray]:
+def compute_linear_transform2D(arc_pos: Vector, radius: float, focus_pos: Vector) -> Tuple[np.ndarray, np.ndarray]:
     """
 
     Compute a rotation matrix to transform the computed arc points to the orientation
     specified by the arc and focus positions
 
     Args:
         arc_pos:
@@ -3131,25 +3008,25 @@
     # Compute an offset for the arc, where arc_centre = move from arc_pos
     # towards focus by radius
     b = arc_pos.reshape(-1, 1) + radius * beam_vec.reshape(-1, 1)
 
     return R, b
 
 
-@beartype
+@typechecker
 def make_cart_spherical_segment(
-    bowl_pos: NDArray[Shape["3"], Float], 
-    radius: Union[float, int], 
-    inner_diameter: Union[float, int], 
+    bowl_pos: Float[np.ndarray, "3"],
+    radius: Union[float, int],
+    inner_diameter: Union[float, int],
     outer_diameter: Union[float, int],
-    focus_pos: NDArray[Shape["3"], Float], 
-    num_points: int, 
+    focus_pos: Float[np.ndarray, "3"],
+    num_points: int,
     plot_bowl: Optional[bool] = False,
-    num_points_inner: int = 0
-) -> NDArray[Shape["3, NumPoints"], Float]:
+    num_points_inner: int = 0,
+) -> Float[np.ndarray, "3 NumPoints"]:
     """
     Create evenly distributed Cartesian points covering a spherical segment.
 
     Args:
         bowl_pos:           Cartesian position of the centre of the rear surface
                             of the underlying bowl on which the spherical segment lies given as a
                             three element vector [bx, by, bz] [m].
@@ -3202,17 +3079,15 @@
     else:
         C = (1 - np.cos(varphi_max)) / (num_points - 1)
         varphi = lambda t: np.arccos(1 - C * t)
         t_start = int(np.ceil((1 - np.cos(varphi_min)) / C))
         t = np.linspace(t_start, num_points - 1, num_points)
 
     # compute canonical spiral points
-    p0 = np.array([np.cos(theta(t)) * np.sin(varphi(t)),
-                   np.sin(theta(t)) * np.sin(varphi(t)),
-                   np.cos(varphi(t))])
+    p0 = np.array([np.cos(theta(t)) * np.sin(varphi(t)), np.sin(theta(t)) * np.sin(varphi(t)), np.cos(varphi(t))])
     p0 = radius * p0
 
     # linearly transform the canonical spiral points to give bowl in correct orientation
     R, b = compute_linear_transform(bowl_pos, focus_pos, radius)
     if np.shape(b) == (3,):
         b = np.expand_dims(b, axis=1)  # expand dims for broadcasting
 
@@ -3220,17 +3095,17 @@
 
     # plot results
     if plot_bowl is True:
         _, scale, prefix, unit = scale_SI(np.max(segment))
 
         # create the figure
         fig = plt.figure()
-        ax = fig.add_subplot(111, projection='3d')
+        ax = fig.add_subplot(111, projection="3d")
         ax.scatter(segment[0] * scale, segment[1] * scale, segment[2] * scale)
-        ax.set_xlabel('[' + prefix + 'm]')
-        ax.set_ylabel('[' + prefix + 'm]')
-        ax.set_zlabel('[' + prefix + 'm]')
+        ax.set_xlabel("[" + prefix + "m]")
+        ax.set_ylabel("[" + prefix + "m]")
+        ax.set_zlabel("[" + prefix + "m]")
         ax.set_box_aspect([1, 1, 1])
         plt.grid(True)
         plt.show()
 
     return segment
```

### Comparing `k_wave_python-0.3.2/kwave/utils/math.py` & `k_wave_python-0.3.3/kwave/utils/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,25 +38,21 @@
 
     Returns:
         A list of prime numbers less than n.
 
     """
 
     sieve = bytearray([True]) * (n // 2 + 1)
-    for i in range(1, int(n ** 0.5) // 2 + 1):
+    for i in range(1, int(n**0.5) // 2 + 1):
         if sieve[i]:
-            sieve[2 * i * (i + 1)::2 * i + 1] = bytearray((n // 2 - 2 * i * (i + 1)) // (2 * i + 1) + 1)
+            sieve[2 * i * (i + 1) :: 2 * i + 1] = bytearray((n // 2 - 2 * i * (i + 1)) // (2 * i + 1) + 1)
     return [2, *compress(range(3, n, 2), sieve[1:])]
 
 
-def fourier_shift(
-        data: np.ndarray,
-        shift: float,
-        shift_dim: Optional[int] = None
-) -> np.ndarray:
+def fourier_shift(data: np.ndarray, shift: float, shift_dim: Optional[int] = None) -> np.ndarray:
     """
     Shifts an array along one of its dimensions using Fourier interpolation.
 
     Args:
         data: The input array.
         shift: The amount of shift to apply.
         shift_dim: The dimension along which to shift the array. Default is the last dimension.
@@ -90,15 +86,15 @@
 
     # put the wavenumber vector in the correct orientation for use with bsxfun
     reshape_dims_to = [1] * data.ndim
     if 0 <= shift_dim <= 3:
         reshape_dims_to[shift_dim] = -1
         k_vec = np.reshape(k_vec, reshape_dims_to)
     else:
-        raise ValueError('Input dim must be 0, 1, 2 or 3.')
+        raise ValueError("Input dim must be 0, 1, 2 or 3.")
 
     # shift the input using a Fourier interpolant
     part_1 = ifftshift(np.exp(1j * k_vec * shift))
     part_2 = fft(data, axis=shift_dim)
     part_1_times_2 = part_1 * part_2
     result = ifft(part_1_times_2, axis=shift_dim).real
     return result
@@ -184,21 +180,20 @@
     Returns:
         A list of prime factors of n.
 
     """
 
     factors = []
     while n % 2 == 0:
-        factors.append(2),
+        (factors.append(2),)
         n = n / 2
 
     # n became odd
     for i in range(3, int(math.sqrt(n)) + 1, 2):
-
-        while (n % i == 0):
+        while n % i == 0:
             factors.append(i)
             n = n / i
 
     if n > 2:
         factors.append(n)
 
     return factors
@@ -247,18 +242,18 @@
 
     mu = np.mean(im)
     s = np.sum((im - mu) ** 2) / mu
     return s
 
 
 def gaussian(
-        x: Union[int, float, np.ndarray],
-        magnitude: Optional[Union[int, float]] = None,
-        mean: Optional[float] = 0,
-        variance: Optional[float] = 1,
+    x: Union[int, float, np.ndarray],
+    magnitude: Optional[Union[int, float]] = None,
+    mean: Optional[float] = 0,
+    variance: Optional[float] = 1,
 ) -> Union[int, float, np.ndarray]:
     """
     Returns a Gaussian distribution f(x) with the specified magnitude, mean, and variance. If these values are not specified,
     the magnitude is normalised and values of variance = 1 and mean = 0 are used. For example running:
 
         import matplotlib.pyplot as plt
         x = np.arange(-3, 0.05, 3)
@@ -278,15 +273,15 @@
         A Gaussian distribution.
 
     """
 
     if magnitude is None:
         magnitude = (2 * math.pi * variance) ** -0.5
 
-    gauss_distr = magnitude * np.exp(-(x - mean) ** 2 / (2 * variance))
+    gauss_distr = magnitude * np.exp(-((x - mean) ** 2) / (2 * variance))
 
     return gauss_distr
     # return magnitude * norm.pdf(x, loc=mean, scale=variance)
     """ # Former impl. form Farid
         if magnitude is None:
         magnitude = np.sqrt(2 * np.pi * variance)
     return magnitude * np.exp(-(x - mean) ** 2 / (2 * variance))
@@ -296,14 +291,15 @@
 def cosd(angle_in_degrees):
     # Note:
     #   Using numpy.radians instead math.radians
     #   does not yield the same results as matlab
     angle_in_radians = math.radians(angle_in_degrees)
     return math.cos(angle_in_radians)
 
+
 def sind(angle_in_degrees):
     # Note:
     #   Using numpy.radians instead math.radians
     #   does not yield the same results as matlab
     angle_in_radians = math.radians(angle_in_degrees)
     return math.sin(angle_in_radians)
 
@@ -314,116 +310,94 @@
 
     Args:
     theta : float. Angle of rotation (in degrees)
 
     Returns:
     np.array. 3D rotation matrix
     """
-    R = np.array([[1, 0, 0],
-                  [0, cosd(theta), -sind(theta)],
-                  [0, sind(theta), cosd(theta)]])
+    R = np.array([[1, 0, 0], [0, cosd(theta), -sind(theta)], [0, sind(theta), cosd(theta)]])
     return R
 
+
 def Ry(theta):
     """
     3D rotation matrix for rotation about y-axis
 
     Args:
     theta : float. Angle of rotation (in degrees)
 
     Returns:
     np.array. 3D rotation matrix
     """
-    R = np.array([[cosd(theta), 0, sind(theta)],
-                  [0, 1, 0],
-                  [-sind(theta), 0, cosd(theta)]])
+    R = np.array([[cosd(theta), 0, sind(theta)], [0, 1, 0], [-sind(theta), 0, cosd(theta)]])
     return R
 
+
 def Rz(theta):
     """
     3D rotation matrix for rotation about z-axis
 
     Args:
     theta : float. Angle of rotation (in degrees)
 
     Returns:
     np.array. 3D rotation matrix
     """
-    R = np.array([[cosd(theta), -sind(theta), 0],
-                  [sind(theta), cosd(theta), 0],
-                  [0, 0, 1]])
+    R = np.array([[cosd(theta), -sind(theta), 0], [sind(theta), cosd(theta), 0], [0, 0, 1]])
     return R
 
 
 def get_affine_matrix(translation: Vector, rotation: Union[int, float, np.ndarray, Vector]):
     # Check dimensions
     if len(translation) == 2 and isinstance(rotation, (int, float)):
-
         # Assign the inputs
         dx = translation[0]
         dy = translation[1]
         th = rotation
 
         # Build affine matrix (counter-clockwise)
-        affine = np.array([
-            [cosd(th), -sind(th), dx],
-            [sind(th), cosd(th), dy],
-            [0, 0, 1]
-        ])
+        affine = np.array([[cosd(th), -sind(th), dx], [sind(th), cosd(th), dy], [0, 0, 1]])
 
     elif len(translation) == 3 and isinstance(rotation, (np.ndarray, Vector)) and len(rotation) == 3:
-
         # Assign the inputs
         dx, dy, dz = translation
         x_th, y_th, z_th = rotation
 
         # Build the rotation matrices
-        x_th_matrix = np.array([
-            [1, 0, 0],
-            [0, cosd(x_th), -sind(x_th)],
-            [0, sind(x_th), cosd(x_th)]
-        ])
-
-        y_th_matrix = np.array([
-            [cosd(y_th), 0, sind(y_th)],
-            [0, 1, 0],
-            [-sind(y_th), 0, cosd(y_th)]
-        ])
-
-        z_th_matrix = np.array([
-            [cosd(z_th), -sind(z_th), 0],
-            [sind(z_th), cosd(z_th), 0],
-            [0, 0, 1]
-        ])
+        x_th_matrix = np.array([[1, 0, 0], [0, cosd(x_th), -sind(x_th)], [0, sind(x_th), cosd(x_th)]])
+
+        y_th_matrix = np.array([[cosd(y_th), 0, sind(y_th)], [0, 1, 0], [-sind(y_th), 0, cosd(y_th)]])
+
+        z_th_matrix = np.array([[cosd(z_th), -sind(z_th), 0], [sind(z_th), cosd(z_th), 0], [0, 0, 1]])
 
         # Build affine matrix
         affine = np.zeros((4, 4))
         affine[0:3, 0:3] = np.dot(z_th_matrix, np.dot(y_th_matrix, x_th_matrix))
         affine[:, 3] = [dx, dy, dz, 1]
 
     else:
-        raise ValueError('Incorrect size for translation and rotation inputs.')
+        raise ValueError("Incorrect size for translation and rotation inputs.")
 
     return affine
 
 
 def compute_linear_transform(pos1, pos2, offset=None):
     # Compute vector pointing from pos1 to pos2
     beam_vec = pos2 - pos1
 
     magnitude = np.linalg.norm(beam_vec)
-    
+
     # TODO: it seems matlab behaviour is to return nans when positions are the same.
     #       we should open an issue and change our behaviour once matlab is fixed.
     # if magnitude == 0:
     #     # "pos1 and pos2 are the same"
     #     return np.eye(3), 0 if offset is None else offset
 
     # Normalise to give unit beam vector
-    beam_vec = beam_vec /  magnitude
+    beam_vec = beam_vec / magnitude
 
     # Canonical normalised beam_vec (canonical pos1 is [0, 0, 1])
     beam_vec0 = np.array([0, 0, -1])
 
     # Find the rotation matrix for the bowl
     u = np.cross(beam_vec0, beam_vec)
```

### Comparing `k_wave_python-0.3.2/kwave/utils/matlab.py` & `k_wave_python-0.3.3/kwave/utils/matlab.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,35 +28,35 @@
     if np.isclose(quotient, closest_int, rtol=rtol, atol=atol).all():
         return np.zeros_like(x)
 
     remainder = x - np.fix(quotient) * y
 
     return remainder
 
-def matlab_assign(matrix: np.ndarray, indices: Union[int, np.ndarray],
-                  values: Union[int, float, np.ndarray]) -> np.ndarray:
+
+def matlab_assign(matrix: np.ndarray, indices: Union[int, np.ndarray], values: Union[int, float, np.ndarray]) -> np.ndarray:
     """
     Assigns values to elements of a matrix using subscript indices.
 
     Args:
         matrix: The matrix to which values will be assigned.
         indices: The subscript indices of the elements to be assigned. Can be a single integer or a NumPy array.
         values: The values to be assigned. Can be a single integer, float, or a NumPy array.
 
     Returns:
         The modified matrix.
 
     """
     original_shape = matrix.shape
-    matrix = np.ravel(matrix, order='F')
+    matrix = np.ravel(matrix, order="F")
     matrix[indices] = values
-    return matrix.reshape(original_shape, order='F')
+    return matrix.reshape(original_shape, order="F")
 
 
-def matlab_find(arr: Union[List[int], np.ndarray], val: int = 0, mode: str = 'neq') -> np.ndarray:
+def matlab_find(arr: Union[List[int], np.ndarray], val: int = 0, mode: str = "neq") -> np.ndarray:
     """
     Finds the indices of elements in an array that satisfy a given condition.
 
     Args:
         arr: The array to search. Can be a list or a NumPy array.
         val: The value to compare against. Default is 0.
         mode: The comparison mode. Can be either 'neq' (not equal) or 'eq' (equal). Default is 'neq'.
@@ -64,18 +64,18 @@
     Returns:
         A NumPy array of indices.
 
     """
 
     if not isinstance(arr, np.ndarray):
         arr = np.array(arr)
-    if mode == 'neq':
-        arr = np.where(arr.flatten(order='F') != val)[0] + 1  # +1 due to matlab indexing
+    if mode == "neq":
+        arr = np.where(arr.flatten(order="F") != val)[0] + 1  # +1 due to matlab indexing
     else:  # 'eq'
-        arr = np.where(arr.flatten(order='F') == val)[0] + 1  # +1 due to matlab indexing
+        arr = np.where(arr.flatten(order="F") == val)[0] + 1  # +1 due to matlab indexing
     return np.expand_dims(arr, -1)  # compatibility, n => [n, 1]
 
 
 def matlab_mask(arr: np.ndarray, mask: np.ndarray, diff: Optional[int] = None) -> np.ndarray:
     """
     Applies a mask to an array and returns the masked elements.
 
@@ -86,38 +86,37 @@
 
     Returns:
         A NumPy array containing the masked elements.
 
     """
 
     if diff is None:
-        return np.expand_dims(arr.ravel(order='F')[mask.ravel(order='F')], axis=-1)  # compatibility, n => [n, 1]
+        return np.expand_dims(arr.ravel(order="F")[mask.ravel(order="F")], axis=-1)  # compatibility, n => [n, 1]
     else:
-        return np.expand_dims(arr.ravel(order='F')[mask.ravel(order='F') + diff], axis=-1)  # compatibility, n => [n, 1]
+        return np.expand_dims(arr.ravel(order="F")[mask.ravel(order="F") + diff], axis=-1)  # compatibility, n => [n, 1]
 
 
-def unflatten_matlab_mask(arr: np.ndarray, mask: np.ndarray, diff: Optional[int] = None) -> Tuple[
-    Union[int, np.ndarray], ...]:
+def unflatten_matlab_mask(arr: np.ndarray, mask: np.ndarray, diff: Optional[int] = None) -> Tuple[Union[int, np.ndarray], ...]:
     """
     Converts a mask array to a tuple of subscript indices for an n-dimensional array.
 
     Args:
         arr: The n-dimensional array for which the mask was created.
         mask: The mask array, which can be of any dimensions.
         diff: An optional integer to add to the mask indices before converting them to subscript indices.
 
     Returns:
         A tuple of integers or NumPy arrays representing the corresponding subscript indices.
 
     """
 
     if diff is None:
-        return np.unravel_index(mask.ravel(order='F'), arr.shape, order='F')
+        return np.unravel_index(mask.ravel(order="F"), arr.shape, order="F")
     else:
-        return np.unravel_index(mask.ravel(order='F') + diff, arr.shape, order='F')
+        return np.unravel_index(mask.ravel(order="F") + diff, arr.shape, order="F")
 
 
 def ind2sub(array_shape: Tuple[int, ...], ind: int) -> Tuple[int, ...]:
     """
     Converts a linear index to a tuple of subscript indices for an n-dimensional array.
 
     Args:
@@ -125,15 +124,15 @@
         ind: The linear index to be converted.
 
     Returns:
         A tuple of integers representing the corresponding subscript indices.
 
     """
 
-    indices = np.unravel_index(ind - 1, array_shape, order='F')
+    indices = np.unravel_index(ind - 1, array_shape, order="F")
     indices = (np.squeeze(index) + 1 for index in indices)
     return indices
 
 
 def sub2ind(array_shape: Tuple[int, int, int], x: np.ndarray, y: np.ndarray, z: np.ndarray) -> np.ndarray:
     """
     Convert 3D subscript indices to a linear index.
@@ -151,10 +150,10 @@
         A 1D numpy array containing the linear indices.
 
     """
 
     results = []
     x, y, z = np.squeeze(x), np.squeeze(y), np.squeeze(z)
     for x_i, y_i, z_i in zip(x, y, z):
-        index = np.ravel_multi_index((x_i, y_i, z_i), dims=array_shape, order='F')
+        index = np.ravel_multi_index((x_i, y_i, z_i), dims=array_shape, order="F")
         results.append(index)
     return np.array(results)
```

### Comparing `k_wave_python-0.3.2/kwave/utils/matrix.py` & `k_wave_python-0.3.3/kwave/utils/matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import logging
 
 import numpy as np
 from scipy.interpolate import interpn, interp1d
-from beartype import beartype
-from beartype.typing import Union, List, Tuple, Any, Optional
-from nptyping import NDArray, Number, Shape, Int
-
-from kwave.utils.typing import INT, NUMERIC
+from beartype import beartype as typechecker
+from beartype.typing import Union, List, Tuple, Optional
+from jaxtyping import Int, Num, Shaped, Real, Bool
+import kwave.utils.typing as kt
 
 from .data import scale_time
 from .tictoc import TicToc
 
 
-
-
-
-@beartype
-def trim_zeros(data: NDArray[Any, Number]) -> Tuple[NDArray[Any, Number], List[Tuple[INT, INT]]]:
+@typechecker
+def trim_zeros(data: Num[np.ndarray, "..."]) -> Tuple[Num[np.ndarray, "..."], List[Tuple[Int[kt.ScalarLike, ""], Int[kt.ScalarLike, ""]]]]:
     """
     Create a tight bounding box by removing zeros.
 
-    Args: 
+    Args:
         data: Matrix to trim.
 
     Returns:
         Tuple containing the trimmed matrix and indices used to trim the matrix.
 
     Raises:
         ValueError: If the input data is not 1D, 2D, or 3D.
@@ -60,15 +56,14 @@
     collapse = {2: [1, 0], 3: [(1, 2), (0, 2), (0, 1)]}
 
     # preallocate output to store indices
     ind = []
 
     # loop through dimensions
     for dim_index in range(data.ndim):
-
         # collapse to 1D vector
         if data.ndim == 1:
             summed_values = data
         else:
             summed_values = np.sum(np.abs(data), axis=collapse[data.ndim][dim_index])
 
         # find the first and last non-empty values
@@ -90,19 +85,20 @@
             elif dim_index == 2:
                 data = data[..., ind_first:ind_last]
                 ind.append((ind_first, ind_last))
 
     return data, ind
 
 
-@beartype
+@typechecker
 def expand_matrix(
-    matrix: NDArray[Any, Any], 
-    exp_coeff: Union[NDArray[Shape["*"], Int], List[int]],   # noqa: F722
-    edge_val: Optional[NUMERIC]=None):
+    matrix: Union[Num[np.ndarray, "..."], Bool[np.ndarray, "..."]],
+    exp_coeff: Union[Shaped[kt.ArrayLike, "dim"], List],
+    edge_val: Optional[Real[kt.ScalarLike, ""]] = None,
+):
     """
     Enlarge a matrix by extending the edge values.
 
     expandMatrix enlarges an input matrix by extension of the values at
     the outer faces of the matrix (endpoints in 1D, outer edges in 2D,
     outer surfaces in 3D). Alternatively, if an input for edge_val is
     given, all expanded matrix elements will have this value. The values
@@ -127,43 +123,43 @@
 
     """
 
     opts = {}
     matrix = np.squeeze(matrix)
 
     if edge_val is None:
-        opts['mode'] = 'edge'
+        opts["mode"] = "edge"
     else:
-        opts['mode'] = 'constant'
-        opts['constant_values'] = edge_val
+        opts["mode"] = "constant"
+        opts["constant_values"] = edge_val
 
     exp_coeff = np.array(exp_coeff).astype(int).squeeze()
     n_coeff = exp_coeff.size
     assert n_coeff > 0
 
     if n_coeff == 1:
-        opts['pad_width'] = exp_coeff
+        opts["pad_width"] = exp_coeff
     elif len(matrix.shape) == 1:
         assert n_coeff <= 2
-        opts['pad_width'] = exp_coeff
+        opts["pad_width"] = exp_coeff
     elif len(matrix.shape) == 2:
         if n_coeff == 2:
-            opts['pad_width'] = exp_coeff
+            opts["pad_width"] = exp_coeff
         if n_coeff == 4:
-            opts['pad_width'] = [(exp_coeff[0], exp_coeff[1]), (exp_coeff[2], exp_coeff[3])]
+            opts["pad_width"] = [(exp_coeff[0], exp_coeff[1]), (exp_coeff[2], exp_coeff[3])]
     elif len(matrix.shape) == 3:
         if n_coeff == 3:
-            opts['pad_width'] = np.tile(np.expand_dims(exp_coeff, axis=-1), [1, 2])
+            opts["pad_width"] = np.tile(np.expand_dims(exp_coeff, axis=-1), [1, 2])
         if n_coeff == 6:
-            opts['pad_width'] = [(exp_coeff[0], exp_coeff[1]), (exp_coeff[2], exp_coeff[3]), (exp_coeff[4], exp_coeff[5])]
+            opts["pad_width"] = [(exp_coeff[0], exp_coeff[1]), (exp_coeff[2], exp_coeff[3]), (exp_coeff[4], exp_coeff[5])]
 
     return np.pad(matrix, **opts)
 
 
-def resize(mat: np.ndarray, new_size: Union[int, List[int]], interp_mode: str = 'linear') -> np.ndarray:
+def resize(mat: np.ndarray, new_size: Union[int, List[int]], interp_mode: str = "linear") -> np.ndarray:
     """
     Resizes a matrix of spatial samples to a desired resolution or spatial sampling frequency
     via interpolation.
 
     Parameters:
         mat: Matrix to be resized (i.e., resampled).
         new_size: Desired output resolution.
@@ -172,18 +168,17 @@
     Returns:
         Resized matrix.
     """
     # start the timer
     TicToc.tic()
 
     # update command line status
-    logging.log(logging.INFO, 'Resizing matrix...')
+    logging.log(logging.INFO, "Resizing matrix...")
     # check inputs
-    assert num_dim2(mat) == len(new_size), \
-        'Resolution input must have the same number of elements as data dimensions.'
+    assert num_dim2(mat) == len(new_size), "Resolution input must have the same number of elements as data dimensions."
 
     mat = mat.squeeze()
 
     axis = []
     for dim in range(len(mat.shape)):
         dim_size = mat.shape[dim]
         axis.append(np.linspace(0, 1, dim_size))
@@ -199,17 +194,17 @@
     new_points = xi
     mat_rs = np.squeeze(interpn(points, mat, new_points, method=interp_mode))
     # TODO: fix this hack.
     if dim + 1 == 3:
         mat_rs = mat_rs.reshape([new_size[1], new_size[0], new_size[2]])
         mat_rs = np.transpose(mat_rs, (1, 0, 2))
     else:
-        mat_rs = mat_rs.reshape(new_size, order='F')
+        mat_rs = mat_rs.reshape(new_size, order="F")
     # update command line status
-    logging.log(logging.INFO, f'  completed in {scale_time(TicToc.toc())}')
+    logging.log(logging.INFO, f"  completed in {scale_time(TicToc.toc())}")
     assert mat_rs.shape == tuple(new_size), "Resized matrix does not match requested size."
     return mat_rs
 
 
 def gradient_fd(f, dx=None, dim=None, deriv_order=None, accuracy_order=None) -> List[np.ndarray]:
     """
     Calculate the gradient of an n-dimensional input matrix using the finite-difference method.
@@ -237,17 +232,17 @@
         A list of ndarrays (or a single ndarray if there is only one dimension)
         corresponding to the derivatives of f with respect to each dimension.
         Each derivative has the same shape as f.
 
     """
 
     if deriv_order:
-        logging.log(logging.WARN, f'{DeprecationWarning.__name__}: deriv_order is no longer a supported argument.')
+        logging.log(logging.WARN, f"{DeprecationWarning.__name__}: deriv_order is no longer a supported argument.")
     if accuracy_order:
-        logging.log(logging.WARN, f'{DeprecationWarning.__name__}: accuracy_order is no longer a supported argument.')
+        logging.log(logging.WARN, f"{DeprecationWarning.__name__}: accuracy_order is no longer a supported argument.")
 
     if dim is not None and dx is not None:
         return np.gradient(f, dx, axis=dim)
     elif dim is not None:
         return np.gradient(f, axis=dim)
     elif dx is not None:
         return np.gradient(f, dx)
@@ -349,38 +344,38 @@
 
     """
 
     # Start timer
     TicToc.tic()
 
     # Update command line status
-    logging.log(logging.INFO, 'Revolving 2D matrix to form a 3D matrix...')
+    logging.log(logging.INFO, "Revolving 2D matrix to form a 3D matrix...")
 
     # Get size of matrix
     m, n = mat2d.shape
 
     # Create the reference axis for the 2D image
     r_axis_one_sided = np.arange(0, n)
     r_axis_two_sided = np.arange(-(n - 1), n)
 
     # Compute the distance from every pixel in the z-y cross-section of the 3D
     # matrix to the rotation axis
     z, y = np.meshgrid(r_axis_two_sided, r_axis_two_sided)
-    r = np.sqrt(y ** 2 + z ** 2)
+    r = np.sqrt(y**2 + z**2)
 
     # Create empty image matrix
     mat3D = np.zeros((m, 2 * n - 1, 2 * n - 1))
 
     # Loop through each cross-section and create 3D matrix
     for x_index in range(m):
-        interp = interp1d(x=r_axis_one_sided, y=mat2d[x_index, :], kind='linear', bounds_error=False, fill_value=0)
+        interp = interp1d(x=r_axis_one_sided, y=mat2d[x_index, :], kind="linear", bounds_error=False, fill_value=0)
         mat3D[x_index, :, :] = interp(r)
 
     # Update command line status
-    logging.log(logging.INFO, f'  completed in {scale_time(TicToc.toc())}s')
+    logging.log(logging.INFO, f"  completed in {scale_time(TicToc.toc())}s")
     return mat3D
 
 
 def sort_rows(arr: np.ndarray, index: int) -> np.ndarray:
     """
     Sort the rows of a 2D numpy array by the values in a specific column.
```

### Comparing `k_wave_python-0.3.2/kwave/utils/plot.py` & `k_wave_python-0.3.3/kwave/utils/plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,29 +13,29 @@
         transparency (float): Value between 0 and 1 specifying transparency where 1 gives no transparency (default = 0.8).
 
     Returns:
         None
     """
     # Check input matrix is 3D and single or double precision
     if len(mat.shape) != 3 or not np.issubdtype(mat.dtype, np.floating):
-        raise ValueError('Input must be a 3D matrix in single or double precision.')
+        raise ValueError("Input must be a 3D matrix in single or double precision.")
 
     # Normalize the matrix
     mat = mat / np.max(mat)
 
     # Create 3D figure
     fig = plt.figure()
-    ax = fig.add_subplot(111, projection='3d')
+    ax = fig.add_subplot(111, projection="3d")
     ax.voxels(mat, facecolors=color, alpha=transparency, edgecolors=(0.5, 0.5, 0.5, 0.5))
 
     # Set the axes properties and labels
     ax.view_init(elev=35, azim=-35)  # Adjust viewing angles here
-    ax.set_xlabel('x [voxels]')
-    ax.set_ylabel('y [voxels]')
-    ax.set_zlabel('z [voxels]')
+    ax.set_xlabel("x [voxels]")
+    ax.set_ylabel("y [voxels]")
+    ax.set_zlabel("z [voxels]")
 
     if not axis_tight:
         sz = mat.shape
         ax.set_xlim([0.5, sz[2] + 0.5])
         ax.set_ylim([0.5, sz[1] + 0.5])
         ax.set_zlim([0.5, sz[0] + 0.5])
```

### Comparing `k_wave_python-0.3.2/kwave/utils/pml.py` & `k_wave_python-0.3.3/kwave/utils/pml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 
 from kwave.utils.math import largest_prime_factor
 
 
-def get_pml(Nx: int, dx: float, dt: float, c: float, pml_size: int, pml_alpha: float,
-            staggered: bool, dimension: int, axisymmetric: bool = False) -> np.ndarray:
+def get_pml(
+    Nx: int, dx: float, dt: float, c: float, pml_size: int, pml_alpha: float, staggered: bool, dimension: int, axisymmetric: bool = False
+) -> np.ndarray:
     """
     Returns a 1D perfectly matched layer variable based on the given size and absorption coefficient.
 
     This function calculates a 1D perfectly matched layer (PML) variable based on the specified size and absorption coefficient.
     It uses the given parameters to create an absorption profile, which is then exponentiated and reshaped in the desired direction.
     If the axisymmetric argument is set to True, the axial side of the radial PML will not be added.
 
@@ -41,15 +42,15 @@
 
     # exponentiate and add the components of the pml to the total function
     pml_left = np.exp(-pml_left * dt / 2)
     pml_right = np.exp(-pml_right * dt / 2)
     pml = np.ones((1, Nx))
     if not axisymmetric:
         pml[:, :pml_size] = pml_left
-    pml[:, Nx - pml_size:] = pml_right
+    pml[:, Nx - pml_size :] = pml_right
 
     # reshape the pml vector to be in the desired direction
     if dimension == 1:
         pml = pml.T
     elif dimension == 3:
         pml = np.reshape(pml, (1, 1, Nx))
     return pml
@@ -83,66 +84,68 @@
 
     Returns:
          PML size that gives the overall grid with the smallest prime factors.
 
     """
     # check if grid size is given as kgrid, and extract grid size
     from kwave.kgrid import kWaveGrid
+
     if isinstance(grid_size, kWaveGrid):
         grid_size = grid_size.N
 
     # assign grid size
     grid_dim = len(grid_size)
 
     # check grid size is 1, 2, or 3
-    assert 1 <= grid_dim <= 3, 'Grid dimensions must be given as a 1, 2, or 3 element vector.'
+    assert 1 <= grid_dim <= 3, "Grid dimensions must be given as a 1, 2, or 3 element vector."
 
     # check for pml_range input
     if pml_range is None:
         pml_range = [10, 40]
 
     # force integer
     pml_range = np.round(pml_range).astype(int)
 
     # check for positive values
-    assert np.all(pml_range >= 0), 'Optional input pml_range must be positive.'
+    assert np.all(pml_range >= 0), "Optional input pml_range must be positive."
 
     # check for correct length
-    assert len(pml_range) == 2, 'Optional input pml_range must be a two element vector.'
+    assert len(pml_range) == 2, "Optional input pml_range must be a two element vector."
 
     # check for monotonic
-    assert pml_range[1] > pml_range[0], 'The second value for pml_range must be greater than the first.'
+    assert pml_range[1] > pml_range[0], "The second value for pml_range must be greater than the first."
 
     # check for axisymmetric input
     if axisymmetric is None:
         axisymmetric = False
 
     # check for correct string
-    assert not isinstance(axisymmetric, str) or axisymmetric.startswith(('WSWA', 'WSWS')), \
-        "Optional input axisymmetric must be set to ''WSWA'' or ''WSWS''."
+    assert not isinstance(axisymmetric, str) or axisymmetric.startswith(
+        ("WSWA", "WSWS")
+    ), "Optional input axisymmetric must be set to ''WSWA'' or ''WSWS''."
 
     # check for correct dimensions
     if isinstance(axisymmetric, str) and grid_dim != 2:
-        raise ValueError('Optional input axisymmetric is only valid for 2D grid sizes.')
+        raise ValueError("Optional input axisymmetric is only valid for 2D grid sizes.")
 
     # create array of PML values to search
     pml_size = np.arange(pml_range[0], pml_range[1] + 1)
 
     # extract the largest prime factor for each dimension for each pml size
     facs = np.zeros((grid_dim, len(pml_size)))
     for dim in range(0, grid_dim):
         for index in range(0, len(pml_size)):
             if isinstance(axisymmetric, str) and dim == 2:
-                if axisymmetric == 'WSWA':
+                if axisymmetric == "WSWA":
                     facs[dim, index] = largest_prime_factor((grid_size[dim] + pml_size[index]) * 4)
-                if axisymmetric == 'WSWS':
+                if axisymmetric == "WSWS":
                     facs[dim, index] = largest_prime_factor((grid_size[dim] + pml_size[index]) * 2 - 2)
             else:
                 facs[dim, index] = largest_prime_factor(grid_size[dim] + 2 * pml_size[index])
 
     # get best dimension size
     ind_opt = np.argmin(facs, 1)
 
     # assign output
     pml_sz = pml_size[ind_opt]
 
-    return pml_sz
+    return pml_sz
```

### Comparing `k_wave_python-0.3.2/kwave/utils/signals.py` & `k_wave_python-0.3.3/kwave/utils/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import logging
 from math import floor
 
 import numpy as np
 import scipy
 from numpy.fft import ifftshift, fft, ifft
 
-from beartype import beartype
+from beartype import beartype as typechecker
 from beartype.typing import Union, List, Optional, Tuple
-from nptyping import NDArray, Shape, Int, Bool
+from jaxtyping import Int, Bool
 
 from .conversion import freq2wavenumber
 from .data import scale_SI
 from .mapgen import ndgrid
 from .math import sinc, gaussian
 from .matlab import matlab_mask, unflatten_matlab_mask, rem
 from .matrix import broadcast_axis, num_dim
 
+import kwave.utils.typing as kt
+
 
 def add_noise(signal: np.ndarray, snr: float, mode="rms"):
     """
     Add Gaussian noise to a signal.
 
     Args:
         signal:      input signal
@@ -27,67 +29,69 @@
         mode:        'rms' (default) or 'peak'
 
     Returns:
         Signal with augmented with noise. This behaviour differs from the k-Wave MATLAB implementation in that the SNR is nor returned.
 
     """
     if mode == "rms":
-        reference = np.sqrt(np.mean(signal ** 2))
+        reference = np.sqrt(np.mean(signal**2))
     elif mode == "peak":
         reference = np.max(signal)
     else:
         raise ValueError(f"Unknown parameter '{mode}' for input mode.")
 
     # calculate the standard deviation of the Gaussian noise
     std_dev = reference / (10 ** (snr / 20))
 
     # calculate noise
     noise = std_dev * np.random.randn(*signal.shape)
 
     # check the snr
-    noise_rms = np.sqrt(np.mean(noise ** 2))
-    snr = 20. * np.log10(reference / noise_rms)
+    noise_rms = np.sqrt(np.mean(noise**2))
+    snr = 20.0 * np.log10(reference / noise_rms)
 
     # add noise to the recorded sensor data
     signal = signal + noise
 
     return signal
 
 
-@beartype
-def get_win(N: Union[int, NDArray, Tuple[int, int], Tuple[int, int, int], List[Union[int, Int]]],
-            # TODO: replace and refactor for scipy.signal.get_window
-            # https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.get_window.html#scipy.signal.get_window
-            type_: str,  # TODO change this to enum in the future
-            plot_win: bool = False,
-            param: Optional[float] = None,
-            rotation: bool = False,
-            symmetric: Union[bool, NDArray[Shape["N"], Bool]] = True,
-            square: bool = False):
-    """
-
-   A frequency domain windowing function of specified type and dimensions.
+@typechecker
+def get_win(
+    N: Union[int, np.ndarray, Tuple[int, int], Tuple[int, int, int], List[Int[kt.ScalarLike, ""]]],
+    # TODO: replace and refactor for scipy.signal.get_window
+    # https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.get_window.html#scipy.signal.get_window
+    type_: str,  # TODO change this to enum in the future
+    plot_win: bool = False,
+    param: Optional[float] = None,
+    rotation: bool = False,
+    symmetric: Union[bool, Bool[np.ndarray, "N"]] = True,
+    square: bool = False,
+):
+    """
+
+    A frequency domain windowing function of specified type and dimensions.
+
+     Args:
+         N: Number of samples, [Nx] for 1D, [Nx, Ny] for 2D, [Nx, Ny, Nz] for 3D.
+         type_: Window type. Supported values: 'Bartlett', 'Bartlett-Hanning', 'Blackman', 'Blackman-Harris',
+                                               'Blackman-Nuttall', 'Cosine', 'Flattop', 'Gaussian', 'HalfBand',
+                                               'Hamming', 'Hanning', 'Kaiser', 'Lanczos', 'Nuttall',
+                                               'Rectangular', 'Triangular', 'Tukey'.
+         plot_win: Boolean to display the window (default = False).
+         param: Control parameter for Tukey, Blackman, Gaussian, and Kaiser windows: taper ratio (Tukey),
+                                      alpha (Blackman, Kaiser), standard deviation (Gaussian)
+                                      (default = 0.5, 0.16, 3 respectively).
+         rotation: Boolean to create windows via rotation or outer product (default = False).
+         symmetric: Boolean to make the window symmetrical (default = True).
+                    Can also be a vector defining the symmetry in each matrix dimension.
+         square: Boolean to force the window to be square (default = False).
 
-    Args:
-        N: Number of samples, [Nx] for 1D, [Nx, Ny] for 2D, [Nx, Ny, Nz] for 3D.
-        type_: Window type. Supported values: 'Bartlett', 'Bartlett-Hanning', 'Blackman', 'Blackman-Harris',
-                                              'Blackman-Nuttall', 'Cosine', 'Flattop', 'Gaussian', 'HalfBand',
-                                              'Hamming', 'Hanning', 'Kaiser', 'Lanczos', 'Nuttall',
-                                              'Rectangular', 'Triangular', 'Tukey'.
-        plot_win: Boolean to display the window (default = False).
-        param: Control parameter for Tukey, Blackman, Gaussian, and Kaiser windows: taper ratio (Tukey),
-                                     alpha (Blackman, Kaiser), standard deviation (Gaussian)
-                                     (default = 0.5, 0.16, 3 respectively).
-        rotation: Boolean to create windows via rotation or outer product (default = False).
-        symmetric: Boolean to make the window symmetrical (default = True).
-                   Can also be a vector defining the symmetry in each matrix dimension.
-        square: Boolean to force the window to be square (default = False).
-
-    Returns:
-        A tuple of (win, cg) where win is the window and cg is the coherent gain of the window.
+     Returns:
+         A tuple of (win, cg) where win is the window and cg is the coherent gain of the window.
     """
 
     def cosine_series(n: int, N: int, coeffs: List[float]) -> np.ndarray:
         """
 
         Sub-function to calculate a summed filter cosine series.
 
@@ -111,28 +115,28 @@
     N = N if np.size(N) > 1 else int(N)
 
     # Check if symmetric is either `bool` or `list of bools`
     # assert isinstance(symmetric, int) or isinstance(symmetric, list)
     symmetric = np.array(symmetric, dtype=bool)
 
     # Set default value for `param` if type is one of the special ones
-    assert not plot_win, NotImplementedError('Plotting is not implemented.')
-    if type_ == 'Tukey':
+    assert not plot_win, NotImplementedError("Plotting is not implemented.")
+    if type_ == "Tukey":
         if param is None:
             param = 0.5
         param = np.clip(param, a_min=0, a_max=1)
-    elif type_ == 'Blackman':
+    elif type_ == "Blackman":
         if param is None:
             param = 0.16
         param = np.clip(param, a_min=0, a_max=1)
-    elif type_ == 'Gaussian':
+    elif type_ == "Gaussian":
         if param is None:
             param = 0.5
         param = np.clip(param, a_min=0, a_max=0.5)
-    elif type_ == 'Kaiser':
+    elif type_ == "Kaiser":
         if param is None:
             param = 3
         param = np.clip(param, a_min=0, a_max=100)
 
     # if a non-symmetrical window is required, enlarge the window size (note,
     # this expands each dimension individually if symmetric is a vector)
     N = N + 1 * (1 - symmetric.astype(int))
@@ -148,94 +152,95 @@
     if N.size == 1:
         # TODO: what should this behaviour be if N is a list of ints? make windows of multiple lengths?
         n = np.arange(0, N)
 
         # TODO: find failure cases in test suite when N is zero.
         # assert np.all(N) > 1, 'Signal length N must be greater than 1'
 
-        if type_ == 'Bartlett':
+        if type_ == "Bartlett":
             win = (2 / (N - 1) * ((N - 1) / 2 - abs(n - (N - 1) / 2))).T
-        elif type_ == 'Bartlett-Hanning':
+        elif type_ == "Bartlett-Hanning":
             win = (0.62 - 0.48 * abs(n / (N - 1) - 1 / 2) - 0.38 * np.cos(2 * np.pi * n / (N - 1))).T
-        elif type_ == 'Blackman':
+        elif type_ == "Blackman":
             win = cosine_series(n, N, [(1 - param) / 2, 0.5, param / 2])
-        elif type_ == 'Blackman-Harris':
+        elif type_ == "Blackman-Harris":
             win = cosine_series(n, N, [0.35875, 0.48829, 0.14128, 0.01168])
-        elif type_ == 'Blackman-Nuttall':
+        elif type_ == "Blackman-Nuttall":
             win = cosine_series(n, N, [0.3635819, 0.4891775, 0.1365995, 0.0106411])
-        elif type_ == 'Cosine':
+        elif type_ == "Cosine":
             win = (np.cos(np.pi * n / (N - 1) - np.pi / 2)).T
-        elif type_ == 'Flattop':
+        elif type_ == "Flattop":
             win = cosine_series(n, N, [0.21557895, 0.41663158, 0.277263158, 0.083578947, 0.006947368])
-        elif type_ == 'Gaussian':
+        elif type_ == "Gaussian":
             win = (np.exp(-0.5 * ((n - (N - 1) / 2) / (param * (N - 1) / 2)) ** 2)).T
-        elif type_ == 'HalfBand':
+        elif type_ == "HalfBand":
             win = np.ones(N)
             # why not to just round? => because rounding 0.5 introduces unexpected behaviour
             # round(0.5) should be 1 but it is 0
             ramp_length = round(N / 4 + 1e-8)
-            ramp = 1 / 2 + 9 / 16 * np.cos(np.pi * np.arange(1, ramp_length + 1) / (2 * ramp_length)) - 1 / 16 * np.cos(
-                3 * np.pi * np.arange(1, ramp_length + 1) / (2 * ramp_length))
+            ramp = (
+                1 / 2
+                + 9 / 16 * np.cos(np.pi * np.arange(1, ramp_length + 1) / (2 * ramp_length))
+                - 1 / 16 * np.cos(3 * np.pi * np.arange(1, ramp_length + 1) / (2 * ramp_length))
+            )
             if ramp_length > 0:
                 win[0:ramp_length] = np.flip(ramp)
                 win[-ramp_length:] = ramp
-        elif type_ == 'Hamming':
+        elif type_ == "Hamming":
             win = (0.54 - 0.46 * np.cos(2 * np.pi * n / (N - 1))).T
-        elif type_ == 'Hanning':
+        elif type_ == "Hanning":
             win = (0.5 - 0.5 * np.cos(2 * np.pi * n / (N - 1))).T
-        elif type_ == 'Kaiser':
+        elif type_ == "Kaiser":
             part_1 = scipy.special.iv(0, np.pi * param * np.sqrt(1 - (2 * n / (N - 1) - 1) ** 2))
             part_2 = scipy.special.iv(0, np.pi * param)
             win = part_1 / part_2
-        elif type_ == 'Lanczos':
+        elif type_ == "Lanczos":
             win = 2 * np.pi * n / (N - 1) - np.pi
             win = sinc(win + 1e-12).T
-        elif type_ == 'Nuttall':
+        elif type_ == "Nuttall":
             win = cosine_series(n, N, [0.3635819, 0.4891775, 0.1365995, 0.0106411])
-        elif type_ == 'Rectangular':
+        elif type_ == "Rectangular":
             win = np.ones(N)
-        elif type_ == 'Triangular':
+        elif type_ == "Triangular":
             win = (2 / N * (N / 2 - abs(n - (N - 1) / 2))).T
-        elif type_ == 'Tukey':
+        elif type_ == "Tukey":
             win = np.ones((N, 1))
             index = np.arange(0, (N - 1) * param / 2 + 1e-8)
             param = param * N
-            win[0: len(index)] = 0.5 * (1 + np.cos(2 * np.pi / param * (index - param / 2)))[:, None]
-            win[np.arange(-1, -len(index) - 1, -1)] = win[0:len(index)]
+            win[0 : len(index)] = 0.5 * (1 + np.cos(2 * np.pi / param * (index - param / 2)))[:, None]
+            win[np.arange(-1, -len(index) - 1, -1)] = win[0 : len(index)]
             win = win.squeeze(axis=-1)
         else:
-            raise ValueError(f'Unknown window type: {type_}')
+            raise ValueError(f"Unknown window type: {type_}")
 
         # trim the window if required
         if not symmetric:
             N -= 1
         win = win[0:N]
         win = np.expand_dims(win, axis=-1)
 
         # calculate the coherent gain
         cg = win.sum() / N
     elif N.size == 2:
-
         # create the 2D window
         if rotation:
-
             # create the window in one dimension using getWin recursively
             L = max(N)
             win_lin, _ = get_win(int(L), type_, param=param)
             win_lin = np.squeeze(win_lin)
 
             # create the reference axis
             radius = (L - 1) / 2
             ll = np.linspace(-radius, radius, L)
 
             # create the 2D window using rotation
             xx = np.linspace(-radius, radius, N[0])
             yy = np.linspace(-radius, radius, N[1])
             [x, y] = ndgrid(xx, yy)
-            r = np.sqrt(x ** 2 + y ** 2)
+            r = np.sqrt(x**2 + y**2)
             r[r > radius] = radius
             interp_func = scipy.interpolate.interp1d(ll, win_lin)
             win = interp_func(r)
             win[r <= radius] = interp_func(r[r <= radius])
 
         else:
             # create the window in each dimension using getWin recursively
@@ -243,87 +248,84 @@
             win_y, _ = get_win(int(N[1]), type_, param=param)
 
             # create the 2D window using the outer product
             win = (win_y * win_x.T).T
 
         # trim the window if required
         N = N - 1 * (1 - np.array(symmetric).astype(int))
-        win = win[0:N[0], 0:N[1]]
+        win = win[0 : N[0], 0 : N[1]]
 
         # calculate the coherent gain
         cg = win.sum() / np.prod(N)
     elif N.size == 3:
         # create the 3D window
         if rotation:
-
             # create the window in one dimension using getWin recursively
             L = N.max()
             win_lin, _ = get_win(int(L), type_, param=param)
 
             # create the reference axis
             radius = (L - 1) / 2
             ll = np.linspace(-radius, radius, L)
 
             # create the 3D window using rotation
             xx = np.linspace(-radius, radius, N[0])
             yy = np.linspace(-radius, radius, N[1])
             zz = np.linspace(-radius, radius, N[2])
             [x, y, z] = ndgrid(xx, yy, zz)
-            r = np.sqrt(x ** 2 + y ** 2 + z ** 2)
+            r = np.sqrt(x**2 + y**2 + z**2)
             r[r > radius] = radius
 
             win_lin = np.squeeze(win_lin)
             interp_func = scipy.interpolate.interp1d(ll, win_lin)
             win = interp_func(r)
             win[r <= radius] = interp_func(r[r <= radius])
 
         else:
-
             # create the window in each dimension using getWin recursively
             win_x, _ = get_win(int(N[0]), type_, param=param)
             win_y, _ = get_win(int(N[1]), type_, param=param)
             win_z, _ = get_win(int(N[2]), type_, param=param)
 
             # create the 2D window using the outer product
-            win_2D = (win_x * win_z.T)
+            win_2D = win_x * win_z.T
 
             # create the 3D window
             win = np.zeros((N[0], N[1], N[2]))
             for index in range(0, N[1]):
                 win[:, index, :] = win_2D[:, :] * win_y[index]
 
         # trim the window if required
         N = N - 1 * (1 - np.array(symmetric).astype(int))
-        win = win[0:N[0], 0:N[1], 0:N[2]]
+        win = win[0 : N[0], 0 : N[1], 0 : N[2]]
 
         # calculate the coherent gain
         cg = win.sum() / np.prod(N)
     else:
-        raise ValueError('Invalid input for N, only 1-, 2-, and 3-D windows are supported.')
+        raise ValueError("Invalid input for N, only 1-, 2-, and 3-D windows are supported.")
 
     # enlarge the window if required
     if square and (N.size != 1):
         L = N[0]
         win_sq = win
         win = np.zeros(N_orig)
         if N.size == 2:
             index1 = round((N[0] - L) / 2)
             index2 = round((N[1] - L) / 2)
-            win[index1:(index1 + L), index2:(index2 + L)] = win_sq
+            win[index1 : (index1 + L), index2 : (index2 + L)] = win_sq
         elif N.size == 3:
             index1 = floor((N_orig[0] - L) / 2)
             index2 = floor((N_orig[1] - L) / 2)
             index3 = floor((N_orig[2] - L) / 2)
-            win[index1:index1 + L, index2:index2 + L, index3:index3 + L] = win_sq
+            win[index1 : index1 + L, index2 : index2 + L, index3 : index3 + L] = win_sq
 
     return win, cg
 
 
-def tone_burst(sample_freq, signal_freq, num_cycles, envelope='Gaussian', plot_signal=False, signal_length=0,
-               signal_offset=0):
+def tone_burst(sample_freq, signal_freq, num_cycles, envelope="Gaussian", plot_signal=False, signal_length=0, signal_offset=0):
     """
     Create an enveloped single frequency tone burst.
 
     Args:
         sample_freq: sampling frequency in Hz
         signal_freq: frequency of the tone burst signal in Hz
         num_cycles: number of sinusoidal oscillations
@@ -338,43 +340,42 @@
                         If an array is given, a matrix of tone bursts is created where each row corresponds to
                         a tone burst for each value of the 'SignalOffset'.
 
     Returns:
         created tone burst
 
     """
-    assert isinstance(signal_offset, int) or isinstance(signal_offset,
-                                                        np.ndarray), "signal_offset must be integer or array of integers"
+    assert isinstance(signal_offset, int) or isinstance(signal_offset, np.ndarray), "signal_offset must be integer or array of integers"
     assert isinstance(signal_length, int), "signal_length must be integer"
 
     # calculate the temporal spacing
     dt = 1 / sample_freq  # [s]
 
     # create the tone burst
     tone_length = num_cycles / signal_freq  # [s]
-    # We want to include the endpoint but only if it's divisible by the step-size. 
+    # We want to include the endpoint but only if it's divisible by the step-size.
     # Modulo operator is not stable, so multiple conditions included.
     # if ( (tone_length % dt) < 1e-18 or (np.abs(tone_length % dt - dt) < 1e-18) ):
-    if (rem(tone_length, dt) < 1e-18):
+    if rem(tone_length, dt) < 1e-18:
         tone_t = np.linspace(0, tone_length, int(tone_length / dt) + 1)
     else:
         tone_t = np.arange(0, tone_length, dt)
 
     tone_burst = np.sin(2 * np.pi * signal_freq * tone_t)
     tone_index = np.round(signal_offset)
 
     # check for ring up and ring down input
     if isinstance(envelope, list) or isinstance(envelope, np.ndarray):  # and envelope.size == 2:
-
         # assign the inputs
         num_ring_up_cycles, num_ring_down_cycles = envelope
 
         # check signal is long enough for ring up and down
-        assert num_cycles >= (num_ring_up_cycles + num_ring_down_cycles), \
-            'Input num_cycles must be longer than num_ring_up_cycles + num_ring_down_cycles.'
+        assert num_cycles >= (
+            num_ring_up_cycles + num_ring_down_cycles
+        ), "Input num_cycles must be longer than num_ring_up_cycles + num_ring_down_cycles."
 
         # get period
         period = 1 / signal_freq
 
         # create x-axis for ramp between 0 and pi
         up_ramp_length_points = round(num_ring_up_cycles * period / dt)
         down_ramp_length_points = round(num_ring_down_cycles * period / dt)
@@ -386,33 +387,32 @@
         down_ramp = (np.cos(down_ramp_axis) + 1) * 0.5
 
         # apply the ramps
         tone_burst[0:up_ramp_length_points] = tone_burst[0:up_ramp_length_points] * up_ramp
         tone_burst[-down_ramp_length_points:] = tone_burst[-down_ramp_length_points:] * down_ramp
 
     else:
-
         # create the envelope
-        if envelope == 'Gaussian':
+        if envelope == "Gaussian":
             x_lim = 3
             window_x = np.arange(-x_lim, x_lim + 1e-8, 2 * x_lim / (len(tone_burst) - 1))
             window = gaussian(window_x, 1, 0, 1)
-        elif envelope == 'Rectangular':
+        elif envelope == "Rectangular":
             window = np.ones_like(tone_burst)
-        elif envelope == 'RingUpDown':
+        elif envelope == "RingUpDown":
             raise NotImplementedError("RingUpDown not yet implemented")
         else:
-            raise ValueError(f'Unknown envelope {envelope}.')
+            raise ValueError(f"Unknown envelope {envelope}.")
 
         # apply the envelope
         tone_burst = tone_burst * window
 
         # force the ends to be zero by applying a second window
-        if envelope == 'Gaussian':
-            tone_burst = tone_burst * np.squeeze(get_win(len(tone_burst), type_='Tukey', param=0.05)[0])
+        if envelope == "Gaussian":
+            tone_burst = tone_burst * np.squeeze(get_win(len(tone_burst), type_="Tukey", param=0.05)[0])
 
     # calculate the expected FWHM in the frequency domain
     # t_var = tone_length/(2*x_lim)
     # w_var = 1/(4*pi^2*t_var)
     # fw = 2 * sqrt(2 * log(2) * w_var)
 
     # Convert tone_index and signal_offset to numpy arrays
@@ -425,18 +425,18 @@
     signal = np.zeros((tone_index.size, signal_length))
 
     # Add the tone burst to the signal array
     # Add the tone burst to the signal array
     tone_index = np.atleast_1d(tone_index)
 
     if tone_index.size == 1:
-        signal[:, int(tone_index):int(tone_index) + len(tone_burst)] = tone_burst.T
+        signal[:, int(tone_index) : int(tone_index) + len(tone_burst)] = tone_burst.T
     else:
         for offset, tone_idx in enumerate(tone_index):
-            signal[offset, int(tone_idx):int(tone_idx) + len(tone_burst)] = tone_burst.T
+            signal[offset, int(tone_idx) : int(tone_idx) + len(tone_burst)] = tone_burst.T
     # plot the signal if required
     if plot_signal:
         raise NotImplementedError
 
     return signal
 
 
@@ -453,32 +453,32 @@
         np.ndarray of the reordered sensor data.
 
     Raises:
         ValueError: If the simulation is not 2D or the sensor is not defined as a binary mask.
     """
     # check simulation is 2D
     if kgrid.dim != 2:
-        raise ValueError('The simulation must be 2D.')
+        raise ValueError("The simulation must be 2D.")
 
     # check sensor.mask is a binary mask
     if sensor.mask.dtype != bool and set(np.unique(sensor.mask).tolist()) != {0, 1}:
-        raise ValueError('The sensor must be defined as a binary mask.')
+        raise ValueError("The sensor must be defined as a binary mask.")
 
     # find the coordinates of the sensor points
     x_sensor = matlab_mask(kgrid.x, sensor.mask == 1)
     x_sensor = np.squeeze(x_sensor)
     y_sensor = matlab_mask(kgrid.y, sensor.mask == 1)
     y_sensor = np.squeeze(y_sensor)
 
     # find the angle of each sensor point (from the centre)
     angle = np.arctan2(-x_sensor, -y_sensor)
     angle[angle < 0] = 2 * np.pi + angle[angle < 0]
 
     # sort the sensor points in order of increasing angle
-    indices_new = np.argsort(angle, kind='stable')
+    indices_new = np.argsort(angle, kind="stable")
 
     # reorder the measure time series so that adjacent time series correspond
     # to adjacent sensor points.
     reordered_sensor_data = sensor_data[indices_new]
     return reordered_sensor_data
 
 
@@ -521,50 +521,51 @@
 
     Returns:
         alpha_filter
 
     """
 
     dim = num_dim(kgrid.k)
-    logging.log(logging.INFO, f'    taper ratio: {taper_ratio}')
+    logging.log(logging.INFO, f"    taper ratio: {taper_ratio}")
     # extract the maximum sound speed
     c = max(medium.sound_speed)
 
     assert len(filter_cutoff) == dim, f"Input filter_cutoff must have {dim} elements for a {dim}D grid"
 
     # parse cutoff freqs
     filter_size = []
     for idx, freq in enumerate(filter_cutoff):
-        if freq == 'max':
+        if freq == "max":
             filter_cutoff[idx] = calc_max_freq(kgrid.k_max[idx], c)
             filter_size_local = kgrid.N[idx]
         else:
-            filter_size_local, filter_cutoff[idx] = freq2wavenumber(kgrid.N[idx], kgrid.k_max[idx], filter_cutoff[idx],
-                                                                    c, kgrid.k[idx])
+            filter_size_local, filter_cutoff[idx] = freq2wavenumber(kgrid.N[idx], kgrid.k_max[idx], filter_cutoff[idx], c, kgrid.k[idx])
         filter_size.append(filter_size_local)
 
     # create the alpha_filter
-    filter_sec, _ = get_win(filter_size, 'Tukey', param=taper_ratio, rotation=True)
+    filter_sec, _ = get_win(filter_size, "Tukey", param=taper_ratio, rotation=True)
 
     # enlarge the alpha_filter to the size of the grid
     alpha_filter = np.zeros(kgrid.N)
     indexes = [round((kgrid.N[idx] - filter_size[idx]) / 2) for idx in range(len(filter_size))]
 
     if dim == 1:
-        alpha_filter[indexes[0]: indexes[0] + filter_size[0]] = np.squeeze(filter_sec)
+        alpha_filter[indexes[0] : indexes[0] + filter_size[0]] = np.squeeze(filter_sec)
     elif dim == 2:
-        alpha_filter[indexes[0]: indexes[0] + filter_size[0], indexes[1]: indexes[1] + filter_size[1]] = filter_sec
+        alpha_filter[indexes[0] : indexes[0] + filter_size[0], indexes[1] : indexes[1] + filter_size[1]] = filter_sec
     elif dim == 3:
-        alpha_filter[indexes[0]: indexes[0] + filter_size[0], indexes[1]: indexes[1] + filter_size[1],
-        indexes[2]:indexes[2] + filter_size[2]] = filter_sec
+        alpha_filter[
+            indexes[0] : indexes[0] + filter_size[0], indexes[1] : indexes[1] + filter_size[1], indexes[2] : indexes[2] + filter_size[2]
+        ] = filter_sec
 
     def dim_string(cutoff_vals):
         return "".join([(str(scale_SI(co)[0]) + " Hz by ") for co in cutoff_vals])
+
     # update the command line status
-    logging.log(logging.INFO, '  filter cutoff: ' + dim_string(filter_cutoff)[:-4] + '.')
+    logging.log(logging.INFO, "  filter cutoff: " + dim_string(filter_cutoff)[:-4] + ".")
 
     return alpha_filter
 
 
 def get_wave_number(Nx, dx, dim):
     if Nx % 2 == 0:
         # even
@@ -573,16 +574,15 @@
         nx = np.arange(start=-(Nx - 1) / 2, stop=(Nx - 1) / 2 + 1) / Nx
 
     kx = ifftshift((2 * np.pi / dx) * nx)
 
     return kx
 
 
-def gradient_spect(f: np.ndarray, dn: List[float], dim: Optional[Union[int, List[int]]] = None,
-                   deriv_order: int = 1) -> np.ndarray:
+def gradient_spect(f: np.ndarray, dn: List[float], dim: Optional[Union[int, List[int]]] = None, deriv_order: int = 1) -> np.ndarray:
     """
     gradient_spect calculates the gradient of an n-dimensional input matrix using the Fourier collocation spectral method.
     The gradient for singleton dimensions is returned as 0.
 
     Args:
         f: A numpy ndarray representing the input matrix.
         dn: A list of floats representing the grid spacings in each dimension.
@@ -595,15 +595,14 @@
     """
 
     # get size of the input function
     sz = f.shape
 
     # check if input is 1D or user defined input dimension is given
     if dim or len(sz) == 1:
-
         # check if a single dn value is given, if not, extract the required value
         if not (isinstance(dn, int) or isinstance(dn, float)):
             dn = dn[dim]
 
         # get the grid size along the specified dimension, or the longest dimension if 1D
         if max(sz) == np.prod(sz):
             dim = np.argmax(sz)
@@ -617,16 +616,15 @@
         # calculate derivative and assign output
         grads = np.real(ifft((1j * kx) ** deriv_order * fft(f, axis=dim), axis=dim))
     else:
         # logging.log(logging.WARN, "This implementation is not tested.")
         # get the wave number
         # kx = get_wave_number(sz(dim), dn[dim], dim)
 
-        assert len(dn) == len(sz), ValueError(
-            f"{len(sz)} values for dn must be specified for a {len(sz)}-dimensional input matrix.")
+        assert len(dn) == len(sz), ValueError(f"{len(sz)} values for dn must be specified for a {len(sz)}-dimensional input matrix.")
 
         grads = []
         # calculate the gradient for each non-singleton dimension
         for dim in range(num_dim(f)):
             # get the wave number
             kx = get_wave_number(sz[dim], dn[dim], dim)
             # calculate derivative and assign output
@@ -645,24 +643,23 @@
         unmasked_sensor_data = np.zeros((kgrid.Nx, kgrid.Ny))
     elif kgrid.k == 3:
         unmasked_sensor_data = np.zeros((kgrid.Nx, kgrid.Ny, kgrid.Nz))
     else:
         raise NotImplementedError
 
     # reorder input data
-    flat_sensor_mask = (sensor.mask != 0).flatten('F')
+    flat_sensor_mask = (sensor.mask != 0).flatten("F")
     assignment_mask = unflatten_matlab_mask(unmasked_sensor_data, np.where(flat_sensor_mask)[0])
     # unmasked_sensor_data.flatten('F')[flat_sensor_mask] = sensor_data.flatten()
     unmasked_sensor_data[assignment_mask] = sensor_data.flatten()
     # unmasked_sensor_data[unflatten_matlab_mask(unmasked_sensor_data, sensor.mask != 0)] = sensor_data
     return unmasked_sensor_data
 
 
-def create_cw_signals(t_array: np.ndarray, freq: float, amp: np.ndarray, phase: np.ndarray,
-                      ramp_length: int = 4) -> np.ndarray:
+def create_cw_signals(t_array: np.ndarray, freq: float, amp: np.ndarray, phase: np.ndarray, ramp_length: int = 4) -> np.ndarray:
     """
     Generate a series of continuous wave (CW) signals based on the 1D or 2D input matrices `amp` and `phase`, where each signal
     is given by:
 
         amp[i, j] .* sin(2 * pi * freq * t_array + phase[i, j]);
 
     To avoid startup transients, a cosine tapered up-ramp is applied to the beginning of the signal. By default, the length
@@ -706,16 +703,15 @@
     # create input signals
     cw_signal = np.zeros((N1, N2, len(t_array)))
 
     # create signal
     for index1 in range(N1):
         for index2 in range(N2):
             if amp.ndim > 1:
-                cw_signal[index1, index2, :] = amp[index1, index2] * np.sin(
-                    2 * np.pi * freq * t_array + phase[index1, index2])
+                cw_signal[index1, index2, :] = amp[index1, index2] * np.sin(2 * np.pi * freq * t_array + phase[index1, index2])
             else:
                 cw_signal[index1, index2, :] = amp[index1] * np.sin(2 * np.pi * freq * t_array + phase[index1])
 
     # apply ramp to avoid startup transients
     if ramp_length != 0:
         # get period and time step (assuming dt is constant)
         period = 1 / freq
```

### Comparing `k_wave_python-0.3.2/kwave/utils/tictoc.py` & `k_wave_python-0.3.3/kwave/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/LICENSE` & `k_wave_python-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k_wave_python-0.3.2/pyproject.toml` & `k_wave_python-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,36 +26,36 @@
 dependencies = [
     "h5py==3.10.0",
     "scipy==1.12.0",
     "opencv-python==4.9.0.80",
     "deepdiff==6.7.1",
     "matplotlib==3.8.3",
     "numpy>=1.22.2,<1.27.0",
-    "nptyping==2.5.0",
-    "beartype==0.16.4"
+    "beartype==0.17.2",
+    "jaxtyping==0.2.28"
 ]
 
 [project.urls]
 Homepage = "http://www.k-wave.org/"
 Documentation = "https://waltersimson.com/k-wave-python/"
 Repository = "https://github.com/waltsims/k-wave-python"
 Bug-tracker = "https://github.com/waltsims/k-wave-python/issues"
 
 [project.optional-dependencies]
 test = ["pytest",
-        "coverage==7.4.3",
+        "coverage==7.4.4",
         "phantominator",
         "requests==2.31.0"]
-example = ["gdown==4.6.0"]
+example = ["gdown==5.1.0"]
 docs = ["m2r2==0.3.2",
     "sphinx-copybutton==0.5.2",
     "sphinx-tabs==3.4.4",
     "sphinx-toolbox==3.5.0",
     "furo==2024.1.29"]
-dev = ["pre-commit==3.6.2"]
+dev = ["pre-commit==3.7.0"]
 
 [tool.hatch.version]
 path = "kwave/__init__.py"
 
 [tool.hatch.metadata]
 
 # can be removed as soon as uff is published and no longer a direct reference
@@ -88,18 +88,17 @@
     # omit anything in a .local directory anywhere
     "tests/*",
     ]
 
 [tool.ruff]
 # Allow lines to be as long as 140 characters.
 line-length = 140
-# Ruff and nptyping.Shape do not play well together.
-# See the open issue: https://github.com/astral-sh/ruff/issues/6014
-ignore = ["F821"]
-[tool.ruff.per-file-ignores]
+# F821 needed to avoid false-positives in nested functions, F722 due to jaxtyping 
+lint.ignore = ["F821", "F722"]
+[tool.ruff.lint.per-file-ignores]
 # ksource.py contains a lot of non-ported Matlab code that is not usable.
 "kwave/ksource.py" = ["F821"]
 # create_storage_variables.py references a few functions that are not ported yet.
 "kwave/kWaveSimulation_helper/create_storage_variables.py" = ["F821"]
 "kwave/kWaveSimulation_helper/__init__.py" = ["F401"]
 "kwave/options/__init__.py" = ["F401"]
 # Fix in the future => E731: Do not assign a `lambda` expression, use a `def`
```

### Comparing `k_wave_python-0.3.2/docs/README.md` & `k_wave_python-0.3.3/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ![](_static/example_bmode.png)
 
 After installation, run the B-mode reconstruction example in the `examples` directory of the repository:
 
 ```bash
 git clone https://github.com/waltsims/k-wave-python
 cd k-wave-python
-git checkout v0.3.2
+git checkout v0.3.3
 pip install '.[example]' 
 python3 examples/us_bmode_linear_transducer/us_bmode_linear_transducer.py
 ```
 
 This example file steps through the process of:
  1. Generating a simulation medium
  2. Configuring a transducer
```

### Comparing `k_wave_python-0.3.2/PKG-INFO` & `k_wave_python-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-Wave-python
-Version: 0.3.2
+Version: 0.3.3
 Summary: Acoustics toolbox for time domain acoustic and ultrasound simulations in complex and tissue-realistic media.
 Project-URL: Homepage, http://www.k-wave.org/
 Project-URL: Documentation, https://waltersimson.com/k-wave-python/
 Project-URL: Repository, https://github.com/waltsims/k-wave-python
 Project-URL: Bug-tracker, https://github.com/waltsims/k-wave-python/issues
 Author-email: Farid Yagubbayli <farid.yagubbayli@tum.de>, Walter Simson <walter.simson@tum.de>
 Maintainer-email: Walter Simson <walter.simson@tum.de>, Farid Yagubbayli <farid.yagubbayli@tum.de>, David Sinden <david.sinden@mevis.fraunhofer.de>
@@ -683,34 +683,34 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Requires-Dist: beartype==0.16.4
+Requires-Dist: beartype==0.17.2
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: h5py==3.10.0
+Requires-Dist: jaxtyping==0.2.28
 Requires-Dist: matplotlib==3.8.3
-Requires-Dist: nptyping==2.5.0
 Requires-Dist: numpy<1.27.0,>=1.22.2
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: scipy==1.12.0
 Provides-Extra: dev
-Requires-Dist: pre-commit==3.6.2; extra == 'dev'
+Requires-Dist: pre-commit==3.7.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == 'docs'
 Requires-Dist: m2r2==0.3.2; extra == 'docs'
 Requires-Dist: sphinx-copybutton==0.5.2; extra == 'docs'
 Requires-Dist: sphinx-tabs==3.4.4; extra == 'docs'
 Requires-Dist: sphinx-toolbox==3.5.0; extra == 'docs'
 Provides-Extra: example
-Requires-Dist: gdown==4.6.0; extra == 'example'
+Requires-Dist: gdown==5.1.0; extra == 'example'
 Provides-Extra: test
-Requires-Dist: coverage==7.4.3; extra == 'test'
+Requires-Dist: coverage==7.4.4; extra == 'test'
 Requires-Dist: phantominator; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: requests==2.31.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # k-Wave-python
 [![Documentation Status](https://readthedocs.org/projects/k-wave-python/badge/?version=latest)](https://k-wave-python.readthedocs.io/en/latest/?badge=latest)
@@ -743,15 +743,15 @@
 ![](_static/example_bmode.png)
 
 After installation, run the B-mode reconstruction example in the `examples` directory of the repository:
 
 ```bash
 git clone https://github.com/waltsims/k-wave-python
 cd k-wave-python
-git checkout v0.3.2
+git checkout v0.3.3
 pip install '.[example]' 
 python3 examples/us_bmode_linear_transducer/us_bmode_linear_transducer.py
 ```
 
 This example file steps through the process of:
  1. Generating a simulation medium
  2. Configuring a transducer
```

