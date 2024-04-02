# Comparing `tmp/power-grid-model-1.7.8a1374103622511.tar.gz` & `tmp/power-grid-model-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.7.8a1374103622511.tar", last modified: Tue Mar  5 14:31:44 2024, max compression
+gzip compressed data, was "power-grid-model-1.7.9.tar", last modified: Fri Mar  8 08:51:41 2024, max compression
```

## Comparing `power-grid-model-1.7.8a1374103622511.tar` & `power-grid-model-1.7.9.tar`

### file list

```diff
@@ -1,739 +1,740 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.627035 power-grid-model-1.7.8a1374103622511/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-03-05 14:31:44.627035 power-grid-model-1.7.8a1374103622511/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-05 14:31:16.000000 power-grid-model-1.7.8a1374103622511/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.523034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.523034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.511034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.527034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.527034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_handler.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.527034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/gen_getters.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42450 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22831 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.527034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)    32013 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/deserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/serializer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.527034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/
--rw-r--r--   0 runner    (1001) docker     (127)    39409 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/input.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/output.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/update.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/batch_parameter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.531034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/calculation_info.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/component_list.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/counting_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/grouped_index_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/typing.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.531034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21377 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/index_mapping.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.535035 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/calculation_info.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/math_state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22754 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/topology.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.535035 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/common_solver_functions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30274 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/measured_values.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21670 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16021 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    33282 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.535035 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.535035 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.539034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset.h
--rw-r--r--   0 runner    (1001) docker     (127)    56706 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/serialization.h
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.539034 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    95362 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/forward_declarations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/serialization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 14:31:44.627035 power-grid-model-1.7.8a1374103622511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.515035 power-grid-model-1.7.8a1374103622511/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.543034 power-grid-model-1.7.8a1374103622511/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.543034 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/buffer_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    25316 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.547034 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    36789 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34111 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.627035 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-03-05 14:31:44.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45321 2024-03-05 14:31:44.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 14:31:44.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-05 14:31:44.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 14:31:44.000000 power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.523034 power-grid-model-1.7.8a1374103622511/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.547034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.547034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.547034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.551035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.551035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.555034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.555034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.555034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.559034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.559034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.559034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.563034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.563034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.515035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.515035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.563034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.567034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.567034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.567034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.567034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.571035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.571035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.571035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.575034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.575034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.575034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.575034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.579034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.579034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.579034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.583034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.583034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.583034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.587034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.587034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.587034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.591035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.591035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.591035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.591035 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (127)    23855 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.595034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.595034 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    31157 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.519034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.599034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   276262 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.599034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   276200 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.599034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    67667 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.603034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    67517 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.603034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   268377 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.603034 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   268495 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.607035 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   276137 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.607035 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)   276326 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.523034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.607035 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.607035 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.611034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.611034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.611034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.611034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.615034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.615034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.615034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.615034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.619034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.619034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32128 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    13306 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.619034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.623034 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/params.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/params.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.623034 power-grid-model-1.7.8a1374103622511/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.623034 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.523034 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.623034 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:31:44.627035 power-grid-model-1.7.8a1374103622511/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19891 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-03-05 14:31:14.000000 power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.038503 power-grid-model-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-03-08 08:51:41.034503 power-grid-model-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-08 08:51:16.000000 power-grid-model-1.7.9/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.922502 power-grid-model-1.7.9/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.922502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.910502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.922502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.926502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_handler.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.926502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/gen_getters.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42720 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.926502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)    32034 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/deserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/serializer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.926502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/
+-rw-r--r--   0 runner    (1001) docker     (127)    40333 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/batch_parameter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.930503 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/calculation_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/component_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/counting_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/grouped_index_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16247 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/typing.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.930503 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21419 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/index_mapping.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.934502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/calculation_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/math_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22570 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    67238 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.934502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/common_solver_functions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30320 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/measured_values.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33030 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16021 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33282 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.934502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.934502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.938502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56706 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/serialization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.938502 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    95362 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/forward_declarations.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/serialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 08:51:41.038503 power-grid-model-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.910502 power-grid-model-1.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.942503 power-grid-model-1.7.9/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.942503 power-grid-model-1.7.9/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/buffer_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/power_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25316 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.946503 power-grid-model-1.7.9/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36789 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34111 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.034503 power-grid-model-1.7.9/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-03-08 08:51:40.000000 power-grid-model-1.7.9/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45408 2024-03-08 08:51:40.000000 power-grid-model-1.7.9/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 08:51:40.000000 power-grid-model-1.7.9/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-08 08:51:40.000000 power-grid-model-1.7.9/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-08 08:51:40.000000 power-grid-model-1.7.9/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.946503 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.946503 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.950502 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.950502 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.950502 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.954502 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.954502 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.958503 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.958503 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.958503 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.962503 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.962503 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.962503 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.914502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.914502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.914502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.962503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.966503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.966503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.966503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.970503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.970503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.970503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.974503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.974503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.914502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.974503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.978503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.978503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.978503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.982503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.982503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.982503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.986503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.986503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.986503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.990503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.990503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.990503 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.994503 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.994503 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/single-transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.994503 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)    23855 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.998503 power-grid-model-1.7.9/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.998503 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    31157 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.002503 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   276262 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.002503 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   276200 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.002503 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    67667 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.006503 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    67517 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.006503 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   268377 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.010503 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   268495 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.010503 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   276137 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.014503 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)   276326 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.918502 power-grid-model-1.7.9/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.014503 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.014503 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.014503 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.018503 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.018503 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.018503 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.018503 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.022503 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.022503 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.022503 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.026503 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.026503 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32128 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    13306 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.026503 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.030503 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.030503 power-grid-model-1.7.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.030503 power-grid-model-1.7.9/tests/unit/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:40.922502 power-grid-model-1.7.9/tests/unit/deprecated/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.034503 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/deprecated/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:51:41.034503 power-grid-model-1.7.9/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19891 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-03-08 08:51:14.000000 power-grid-model-1.7.9/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.7.8a1374103622511/LICENSE` & `power-grid-model-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/PKG-INFO` & `power-grid-model-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.7.8a1374103622511
+Version: 1.7.9
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Contributors to the Power Grid Model project <powergridmodel@lfenergy.org>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.7.8a1374103622511/README.md` & `power-grid-model-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 //
 // SPDX-License-Identifier: MPL-2.0
 
 #pragma once
 
 // define dataset classes with void pointers
 
+#include "dataset_fwd.hpp"
+
 #include "../common/common.hpp"
 
 #include <cassert>
 #include <map>
 
 namespace power_grid_model {
 
@@ -21,16 +23,27 @@
 // the dataset can also be a batch of sets with different length per batch
 //     the indptr is an integer array, for i-th sets,
 //          the set data is in the range [ indptr[i], indptr[i + 1] )
 // the dataset can also be a batch of sets with the same length per batch
 //     the indptr is a nullptr, for i-th sets,
 //          the set data is in the range [ i * elements_per_scenario, (i + 1) * elements_per_scenario )
 
-template <bool is_const> class DataPointer {
-    template <class T> using ptr_t = std::conditional_t<is_const, T const*, T*>;
+template <dataset_type_tag T> constexpr bool is_const_dataset_v = std::same_as<T, const_dataset_t>;
+
+static_assert(dataset_type_tag<const_dataset_t>);
+static_assert(dataset_type_tag<mutable_dataset_t>);
+static_assert(is_const_dataset_v<const_dataset_t>);
+static_assert(!is_const_dataset_v<mutable_dataset_t>);
+
+template <dataset_type_tag dataset_type_> class DataPointer {
+  public:
+    using dataset_type = dataset_type_;
+
+  private:
+    template <class T> using ptr_t = std::conditional_t<is_const_dataset_v<dataset_type>, T const*, T*>;
 
   public:
     DataPointer() : ptr_{nullptr}, indptr_{nullptr}, batch_size_{}, elements_per_scenario_{} {}
 
     // single batch dataset
     DataPointer(ptr_t<void> ptr, Idx single_length)
         : ptr_{ptr}, indptr_{nullptr}, batch_size_{1}, elements_per_scenario_{single_length} {}
@@ -81,27 +94,27 @@
         if (indptr_ != nullptr) {
             return (indptr_[batch_size_] == 0);
         }
         return batch_size_ == 0 || elements_per_scenario_ == 0;
     }
 
     // conversion to const iterator
-    explicit operator DataPointer<true>() const
-        requires(!is_const)
+    explicit operator DataPointer<const_dataset_t>() const
+        requires(!is_const_dataset_v<dataset_type>)
     {
-        return DataPointer<true>{ptr_, indptr_, batch_size_, elements_per_scenario_};
+        return DataPointer<const_dataset_t>{ptr_, indptr_, batch_size_, elements_per_scenario_};
     }
 
   private:
     ptr_t<void> ptr_;
     Idx const* indptr_;
     Idx batch_size_;            // number of batches
     Idx elements_per_scenario_; // number of data points per batch, -1 for variable batches
 };
 
-using MutableDataPointer = DataPointer<false>;
-using ConstDataPointer = DataPointer<true>;
+using MutableDataPointer = DataPointer<mutable_dataset_t>;
+using ConstDataPointer = DataPointer<const_dataset_t>;
 
 using Dataset = std::map<std::string, MutableDataPointer>;
 using ConstDataset = std::map<std::string, ConstDataPointer>;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_handler.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_handler.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -13,34 +13,52 @@
 #include "meta_data_gen.hpp"
 
 #include <span>
 #include <string_view>
 
 namespace power_grid_model::meta_data {
 
+template <dataset_handler_tag T>
+constexpr bool is_data_mutable_v = std::same_as<T, mutable_dataset_t> || std::same_as<T, writable_dataset_t>;
+template <dataset_handler_tag T> constexpr bool is_indptr_mutable_v = std::same_as<T, writable_dataset_t>;
+
+static_assert(dataset_handler_tag<const_dataset_t>);
+static_assert(dataset_handler_tag<mutable_dataset_t>);
+static_assert(dataset_handler_tag<writable_dataset_t>);
+static_assert(!is_data_mutable_v<const_dataset_t>);
+static_assert(is_data_mutable_v<mutable_dataset_t>);
+static_assert(is_data_mutable_v<writable_dataset_t>);
+static_assert(!is_indptr_mutable_v<const_dataset_t>);
+static_assert(!is_indptr_mutable_v<mutable_dataset_t>);
+static_assert(is_indptr_mutable_v<writable_dataset_t>);
+
 struct ComponentInfo {
     MetaComponent const* component;
     // for non-uniform component, this is -1, we use indptr to describe the elements per scenario
     Idx elements_per_scenario;
     Idx total_elements;
 };
 
 struct DatasetInfo {
     bool is_batch;
     Idx batch_size; // for single dataset, the batch size is one
     MetaDataset const* dataset;
     std::vector<ComponentInfo> component_info;
 };
 
-template <bool data_mutable, bool indptr_mutable>
-    requires(data_mutable || !indptr_mutable)
-class DatasetHandler {
+template <dataset_handler_tag dataset_handler_type_> class DatasetHandler {
+    struct immutable_t {};
+    struct mutable_t {};
+
   public:
-    using Data = std::conditional_t<data_mutable, void, void const>;
-    using Indptr = std::conditional_t<indptr_mutable, Idx, Idx const>;
+    using dataset_handler_type = dataset_handler_type_;
+
+    using Data = std::conditional_t<is_data_mutable_v<dataset_handler_type>, void, void const>;
+    using Indptr = std::conditional_t<is_indptr_mutable_v<dataset_handler_type>, Idx, Idx const>;
+
     struct Buffer {
         Data* data;
         // for uniform buffer, indptr is empty
         std::span<Indptr> indptr;
     };
 
     DatasetHandler(bool is_batch, Idx batch_size, std::string_view dataset)
@@ -50,45 +68,43 @@
                         .component_info = {}} {
         if (!dataset_info_.is_batch && (dataset_info_.batch_size != 1)) {
             throw DatasetError{"For non-batch dataset, batch size should be one!\n"};
         }
     }
 
     // implicit conversion constructor to const
-    template <bool indptr_mutable_other>
-    DatasetHandler(DatasetHandler<true, indptr_mutable_other> const& other)
-        requires(!data_mutable)
-        : dataset_info_{other.get_description()} {
+    template <dataset_handler_tag other_dataset_handler_type>
+        requires(is_data_mutable_v<other_dataset_handler_type> && !is_data_mutable_v<dataset_handler_type>)
+    DatasetHandler(DatasetHandler<other_dataset_handler_type> const& other) : dataset_info_{other.get_description()} {
         for (Idx i{}; i != other.n_components(); ++i) {
             auto const& buffer = other.get_buffer(i);
             buffers_.push_back(Buffer{.data = buffer.data, .indptr = buffer.indptr});
         }
     }
 
-    template <bool dataset_const>
-    std::map<std::string, DataPointer<dataset_const>> export_dataset(Idx scenario = -1) const
-        requires(dataset_const || data_mutable)
-    {
+    template <dataset_type_tag dataset_type>
+        requires(is_const_dataset_v<dataset_type> || is_data_mutable_v<dataset_handler_type>)
+    std::map<std::string, DataPointer<dataset_type>> export_dataset(Idx scenario = -1) const {
         if (!is_batch() && scenario > 0) {
             throw DatasetError{"Cannot export a single dataset with multiple scenarios!\n"};
         }
-        std::map<std::string, DataPointer<dataset_const>> dataset;
+        std::map<std::string, DataPointer<dataset_type>> dataset;
         for (Idx i{}; i != n_components(); ++i) {
             ComponentInfo const& component = get_component_info(i);
             Buffer const& buffer = get_buffer(i);
             if (scenario < 0) {
-                dataset[component.component->name] = DataPointer<dataset_const>{
+                dataset[component.component->name] = DataPointer<dataset_type>{
                     buffer.data, buffer.indptr.data(), batch_size(), component.elements_per_scenario};
             } else {
                 if (component.elements_per_scenario < 0) {
-                    dataset[component.component->name] = DataPointer<dataset_const>{
+                    dataset[component.component->name] = DataPointer<dataset_type>{
                         component.component->advance_ptr(buffer.data, buffer.indptr[scenario]),
                         buffer.indptr[scenario + 1] - buffer.indptr[scenario]};
                 } else {
-                    dataset[component.component->name] = DataPointer<dataset_const>{
+                    dataset[component.component->name] = DataPointer<dataset_type>{
                         component.component->advance_ptr(buffer.data, component.elements_per_scenario * scenario),
                         component.elements_per_scenario};
                 }
             }
         }
         return dataset;
     }
@@ -117,39 +133,39 @@
     }
 
     ComponentInfo const& get_component_info(std::string_view component) const {
         return dataset_info_.component_info[find_component(component, true)];
     }
 
     void add_component_info(std::string_view component, Idx elements_per_scenario, Idx total_elements)
-        requires indptr_mutable
+        requires is_indptr_mutable_v<dataset_handler_type>
     {
         add_component_info_impl(component, elements_per_scenario, total_elements);
     }
 
     void add_buffer(std::string_view component, Idx elements_per_scenario, Idx total_elements, Indptr* indptr,
                     Data* data)
-        requires(!indptr_mutable)
+        requires(!is_indptr_mutable_v<dataset_handler_type>)
     {
-        check_non_uniform_integrity<true>(elements_per_scenario, total_elements, indptr);
+        check_non_uniform_integrity<immutable_t>(elements_per_scenario, total_elements, indptr);
         add_component_info_impl(component, elements_per_scenario, total_elements);
         buffers_.back().data = data;
         if (indptr) {
             buffers_.back().indptr = {indptr, static_cast<size_t>(batch_size() + 1)};
         } else {
             buffers_.back().indptr = {};
         }
     }
 
     void set_buffer(std::string_view component, Indptr* indptr, Data* data)
-        requires indptr_mutable
+        requires is_indptr_mutable_v<dataset_handler_type>
     {
         Idx const idx = find_component(component, true);
         ComponentInfo const& info = dataset_info_.component_info[idx];
-        check_non_uniform_integrity<false>(info.elements_per_scenario, info.total_elements, indptr);
+        check_non_uniform_integrity<mutable_t>(info.elements_per_scenario, info.total_elements, indptr);
         buffers_[idx].data = data;
         if (indptr) {
             buffers_[idx].indptr = {indptr, static_cast<size_t>(batch_size() + 1)};
         } else {
             buffers_[idx].indptr = {};
         }
     }
@@ -161,21 +177,22 @@
     void check_uniform_integrity(Idx elements_per_scenario, Idx total_elements) {
         if ((elements_per_scenario >= 0) && (elements_per_scenario * batch_size() != total_elements)) {
             throw DatasetError{
                 "For a uniform buffer, total_elements should be equal to elements_per_scenario * batch_size !\n"};
         }
     }
 
-    template <bool check_indptr_content>
+    template <typename check_indptr_content>
+        requires std::same_as<check_indptr_content, mutable_t> || std::same_as<check_indptr_content, immutable_t>
     void check_non_uniform_integrity(Idx elements_per_scenario, Idx total_elements, Indptr* indptr) {
         if (elements_per_scenario < 0) {
             if (!indptr) {
                 throw DatasetError{"For a non-uniform buffer, indptr should be supplied !\n"};
             }
-            if constexpr (check_indptr_content) {
+            if constexpr (std::same_as<check_indptr_content, immutable_t>) {
                 if (indptr[0] != 0 || indptr[batch_size()] != total_elements) {
                     throw DatasetError{
                         "For a non-uniform buffer, indptr should begin with 0 and end with total_elements !\n"};
                 }
             }
         } else {
             if (indptr) {
@@ -191,12 +208,12 @@
         check_uniform_integrity(elements_per_scenario, total_elements);
         dataset_info_.component_info.push_back(
             {&dataset_info_.dataset->get_component(component), elements_per_scenario, total_elements});
         buffers_.push_back(Buffer{});
     }
 };
 
-using ConstDatasetHandler = DatasetHandler<false, false>;
-using MutableDatasetHandler = DatasetHandler<true, false>;
-using WritableDatasetHandler = DatasetHandler<true, true>;
+using ConstDatasetHandler = DatasetHandler<const_dataset_t>;
+using MutableDatasetHandler = DatasetHandler<mutable_dataset_t>;
+using WritableDatasetHandler = DatasetHandler<writable_dataset_t>;
 
 } // namespace power_grid_model::meta_data
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,18 @@
     operator BaseInput const&() const { return reinterpret_cast<BaseInput const&>(*this); }
 
     // implicit conversions to ApplianceInput
     operator ApplianceInput&() { return reinterpret_cast<ApplianceInput&>(*this); }
     operator ApplianceInput const&() const { return reinterpret_cast<ApplianceInput const&>(*this); }
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct LoadGenInput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     ID node;  // node ID to which this appliance is connected
     IntS status;  // whether the appliance is connected
     LoadGenType type;  // type of the load_gen
     RealValue<sym> p_specified;  // specified active/reactive power
     RealValue<sym> q_specified;  // specified active/reactive power
 
@@ -248,16 +250,16 @@
     operator ApplianceInput const&() const { return reinterpret_cast<ApplianceInput const&>(*this); }
 
     // implicit conversions to GenericLoadGenInput
     operator GenericLoadGenInput&() { return reinterpret_cast<GenericLoadGenInput&>(*this); }
     operator GenericLoadGenInput const&() const { return reinterpret_cast<GenericLoadGenInput const&>(*this); }
 };
 
-using SymLoadGenInput = LoadGenInput<true>;
-using AsymLoadGenInput = LoadGenInput<false>;
+using SymLoadGenInput = LoadGenInput<symmetric_t>;
+using AsymLoadGenInput = LoadGenInput<asymmetric_t>;
 
 struct ShuntInput {
     ID id;  // ID of the object
     ID node;  // node ID to which this appliance is connected
     IntS status;  // whether the appliance is connected
     double g1;  // positive sequence admittance
     double b1;  // positive sequence admittance
@@ -302,16 +304,18 @@
     operator BaseInput const&() const { return reinterpret_cast<BaseInput const&>(*this); }
 
     // implicit conversions to SensorInput
     operator SensorInput&() { return reinterpret_cast<SensorInput&>(*this); }
     operator SensorInput const&() const { return reinterpret_cast<SensorInput const&>(*this); }
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct VoltageSensorInput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     ID measured_object;  // ID of the measured object
     double u_sigma;  // sigma of error margin of voltage measurement
     RealValue<sym> u_measured;  // measured voltage magnitude and angle
     RealValue<sym> u_angle_measured;  // measured voltage magnitude and angle
 
     // implicit conversions to BaseInput
@@ -323,16 +327,16 @@
     operator SensorInput const&() const { return reinterpret_cast<SensorInput const&>(*this); }
 
     // implicit conversions to GenericVoltageSensorInput
     operator GenericVoltageSensorInput&() { return reinterpret_cast<GenericVoltageSensorInput&>(*this); }
     operator GenericVoltageSensorInput const&() const { return reinterpret_cast<GenericVoltageSensorInput const&>(*this); }
 };
 
-using SymVoltageSensorInput = VoltageSensorInput<true>;
-using AsymVoltageSensorInput = VoltageSensorInput<false>;
+using SymVoltageSensorInput = VoltageSensorInput<symmetric_t>;
+using AsymVoltageSensorInput = VoltageSensorInput<asymmetric_t>;
 
 struct GenericPowerSensorInput {
     ID id;  // ID of the object
     ID measured_object;  // ID of the measured object
     MeasuredTerminalType measured_terminal_type;  // type of measured terminal
     double power_sigma;  // sigma of error margin of apparent power measurement
 
@@ -341,16 +345,18 @@
     operator BaseInput const&() const { return reinterpret_cast<BaseInput const&>(*this); }
 
     // implicit conversions to SensorInput
     operator SensorInput&() { return reinterpret_cast<SensorInput&>(*this); }
     operator SensorInput const&() const { return reinterpret_cast<SensorInput const&>(*this); }
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct PowerSensorInput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     ID measured_object;  // ID of the measured object
     MeasuredTerminalType measured_terminal_type;  // type of measured terminal
     double power_sigma;  // sigma of error margin of apparent power measurement
     RealValue<sym> p_measured;  // measured active/reactive power
     RealValue<sym> q_measured;  // measured active/reactive power
     RealValue<sym> p_sigma;  // sigma of error margin of active/reactive power measurement
@@ -365,16 +371,16 @@
     operator SensorInput const&() const { return reinterpret_cast<SensorInput const&>(*this); }
 
     // implicit conversions to GenericPowerSensorInput
     operator GenericPowerSensorInput&() { return reinterpret_cast<GenericPowerSensorInput&>(*this); }
     operator GenericPowerSensorInput const&() const { return reinterpret_cast<GenericPowerSensorInput const&>(*this); }
 };
 
-using SymPowerSensorInput = PowerSensorInput<true>;
-using AsymPowerSensorInput = PowerSensorInput<false>;
+using SymPowerSensorInput = PowerSensorInput<symmetric_t>;
+using AsymPowerSensorInput = PowerSensorInput<asymmetric_t>;
 
 struct FaultInput {
     ID id;  // ID of the object
     IntS status;  // whether the appliance is connected
     FaultType fault_type;  // type of the fault
     FaultPhase fault_phase;  // phase(s) of the fault
     ID fault_object;  // ID of the faulty object
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 template <> struct ctype_t<int32_t> {
     static constexpr CType value = CType::c_int32;
 };
 template <> struct ctype_t<int8_t> {
     static constexpr CType value = CType::c_int8;
 };
 
-template <> struct ctype_t<RealValue<false>> {
+template <> struct ctype_t<RealValue<asymmetric_t>> {
     static constexpr CType value = CType::c_double3;
 };
 template <class T>
     requires std::is_enum_v<T>
 struct ctype_t<T> : ctype_t<std::underlying_type_t<T>> {};
 template <class T> constexpr CType ctype_v = ctype_t<T>::value;
 
@@ -58,29 +58,29 @@
 template <class Functor, class... Args> decltype(auto) ctype_func_selector(CType ctype, Functor f, Args&&... args) {
     using enum CType;
 
     switch (ctype) {
     case c_double:
         return f.template operator()<double>(std::forward<Args>(args)...);
     case c_double3:
-        return f.template operator()<RealValue<false>>(std::forward<Args>(args)...);
+        return f.template operator()<RealValue<asymmetric_t>>(std::forward<Args>(args)...);
     case c_int8:
         return f.template operator()<int8_t>(std::forward<Args>(args)...);
     case c_int32:
         return f.template operator()<int32_t>(std::forward<Args>(args)...);
     default:
         throw MissingCaseForEnumError{"CType selector", ctype};
     }
 }
 
 // set nan
 inline void set_nan(double& x) { x = nan; }
 inline void set_nan(IntS& x) { x = na_IntS; }
 inline void set_nan(ID& x) { x = na_IntID; }
-inline void set_nan(RealValue<false>& x) { x = RealValue<false>{nan}; }
+inline void set_nan(RealValue<asymmetric_t>& x) { x = RealValue<asymmetric_t>{nan}; }
 template <class Enum>
     requires std::same_as<std::underlying_type_t<Enum>, IntS>
 inline void set_nan(Enum& x) {
     x = static_cast<Enum>(na_IntS);
 }
 
 using RawDataPtr = void*;            // raw mutable data ptr
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 template <class T> struct input_getter_s {
     using type = typename T::InputType;
 };
 template <class T> struct update_getter_s {
     using type = typename T::UpdateType;
 };
 template <class T> struct sym_output_getter_s {
-    using type = typename T::template OutputType<true>;
+    using type = typename T::template OutputType<symmetric_t>;
 };
 template <class T> struct asym_output_getter_s {
-    using type = typename T::template OutputType<false>;
+    using type = typename T::template OutputType<asymmetric_t>;
 };
 template <class T> struct sc_output_getter_s {
     using type = typename T::ShortCircuitOutputType;
 };
 
 // generate meta data
 constexpr MetaData meta_data = get_meta_data<AllComponents, // all components list
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/gen_getters.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/gen_getters.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     (reinterpret_cast<StructType const*>(buffer_ptr) + pos)->*member_ptr;
             },
         .compare_value = [](RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol, double rtol, Idx pos) -> bool {
             ValueType const& x = (reinterpret_cast<StructType const*>(ptr_x) + pos)->*member_ptr;
             ValueType const& y = (reinterpret_cast<StructType const*>(ptr_y) + pos)->*member_ptr;
             if constexpr (std::same_as<ValueType, double>) {
                 return std::abs(y - x) < (std::abs(x) * rtol + atol);
-            } else if constexpr (std::same_as<ValueType, RealValue<false>>) {
+            } else if constexpr (std::same_as<ValueType, RealValue<asymmetric_t>>) {
                 return (abs(y - x) < (abs(x) * rtol + atol)).all();
             } else {
                 return x == y;
             }
         },
     };
 };
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -227,16 +227,18 @@
             meta_data_gen::get_meta_attribute<GenericLoadGenInput, &GenericLoadGenInput::id, offsetof(GenericLoadGenInput, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<GenericLoadGenInput, &GenericLoadGenInput::node, offsetof(GenericLoadGenInput, node), []{ return "node"; }>::value,
             meta_data_gen::get_meta_attribute<GenericLoadGenInput, &GenericLoadGenInput::status, offsetof(GenericLoadGenInput, status), []{ return "status"; }>::value,
             meta_data_gen::get_meta_attribute<GenericLoadGenInput, &GenericLoadGenInput::type, offsetof(GenericLoadGenInput, type), []{ return "type"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<LoadGenInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<LoadGenInput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 6> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<LoadGenInput<sym>, &LoadGenInput<sym>::id, offsetof(LoadGenInput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenInput<sym>, &LoadGenInput<sym>::node, offsetof(LoadGenInput<sym>, node), []{ return "node"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenInput<sym>, &LoadGenInput<sym>::status, offsetof(LoadGenInput<sym>, status), []{ return "status"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenInput<sym>, &LoadGenInput<sym>::type, offsetof(LoadGenInput<sym>, type), []{ return "type"; }>::value,
@@ -283,16 +285,18 @@
             
             meta_data_gen::get_meta_attribute<GenericVoltageSensorInput, &GenericVoltageSensorInput::id, offsetof(GenericVoltageSensorInput, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<GenericVoltageSensorInput, &GenericVoltageSensorInput::measured_object, offsetof(GenericVoltageSensorInput, measured_object), []{ return "measured_object"; }>::value,
             meta_data_gen::get_meta_attribute<GenericVoltageSensorInput, &GenericVoltageSensorInput::u_sigma, offsetof(GenericVoltageSensorInput, u_sigma), []{ return "u_sigma"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<VoltageSensorInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<VoltageSensorInput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 5> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<VoltageSensorInput<sym>, &VoltageSensorInput<sym>::id, offsetof(VoltageSensorInput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorInput<sym>, &VoltageSensorInput<sym>::measured_object, offsetof(VoltageSensorInput<sym>, measured_object), []{ return "measured_object"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorInput<sym>, &VoltageSensorInput<sym>::u_sigma, offsetof(VoltageSensorInput<sym>, u_sigma), []{ return "u_sigma"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorInput<sym>, &VoltageSensorInput<sym>::u_measured, offsetof(VoltageSensorInput<sym>, u_measured), []{ return "u_measured"; }>::value,
@@ -308,16 +312,18 @@
             meta_data_gen::get_meta_attribute<GenericPowerSensorInput, &GenericPowerSensorInput::id, offsetof(GenericPowerSensorInput, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<GenericPowerSensorInput, &GenericPowerSensorInput::measured_object, offsetof(GenericPowerSensorInput, measured_object), []{ return "measured_object"; }>::value,
             meta_data_gen::get_meta_attribute<GenericPowerSensorInput, &GenericPowerSensorInput::measured_terminal_type, offsetof(GenericPowerSensorInput, measured_terminal_type), []{ return "measured_terminal_type"; }>::value,
             meta_data_gen::get_meta_attribute<GenericPowerSensorInput, &GenericPowerSensorInput::power_sigma, offsetof(GenericPowerSensorInput, power_sigma), []{ return "power_sigma"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<PowerSensorInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<PowerSensorInput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 8> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<PowerSensorInput<sym>, &PowerSensorInput<sym>::id, offsetof(PowerSensorInput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorInput<sym>, &PowerSensorInput<sym>::measured_object, offsetof(PowerSensorInput<sym>, measured_object), []{ return "measured_object"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorInput<sym>, &PowerSensorInput<sym>::measured_terminal_type, offsetof(PowerSensorInput<sym>, measured_terminal_type), []{ return "measured_terminal_type"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorInput<sym>, &PowerSensorInput<sym>::power_sigma, offsetof(PowerSensorInput<sym>, power_sigma), []{ return "power_sigma"; }>::value,
@@ -575,16 +581,18 @@
         set_nan(comp.node);
         set_nan(comp.status);
         set_nan(comp.type);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<LoadGenInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<LoadGenInput<sym_type>> {
+    using sym = sym_type;
+
     LoadGenInput<sym> operator() () const {
         LoadGenInput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.node);
         set_nan(comp.status);
@@ -639,16 +647,18 @@
         set_nan(comp.id);
         set_nan(comp.measured_object);
         set_nan(comp.u_sigma);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<VoltageSensorInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<VoltageSensorInput<sym_type>> {
+    using sym = sym_type;
+
     VoltageSensorInput<sym> operator() () const {
         VoltageSensorInput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.measured_object);
         set_nan(comp.u_sigma);
@@ -668,16 +678,18 @@
         set_nan(comp.measured_object);
         set_nan(comp.measured_terminal_type);
         set_nan(comp.power_sigma);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<PowerSensorInput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<PowerSensorInput<sym_type>> {
+    using sym = sym_type;
+
     PowerSensorInput<sym> operator() () const {
         PowerSensorInput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.measured_object);
         set_nan(comp.measured_terminal_type);
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -27,31 +27,35 @@
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<BaseOutput, &BaseOutput::id, offsetof(BaseOutput, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<BaseOutput, &BaseOutput::energized, offsetof(BaseOutput, energized), []{ return "energized"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<NodeOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<NodeOutput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 7> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::id, offsetof(NodeOutput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::energized, offsetof(NodeOutput<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::u_pu, offsetof(NodeOutput<sym>, u_pu), []{ return "u_pu"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::u, offsetof(NodeOutput<sym>, u), []{ return "u"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::u_angle, offsetof(NodeOutput<sym>, u_angle), []{ return "u_angle"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::p, offsetof(NodeOutput<sym>, p), []{ return "p"; }>::value,
             meta_data_gen::get_meta_attribute<NodeOutput<sym>, &NodeOutput<sym>::q, offsetof(NodeOutput<sym>, q), []{ return "q"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<BranchOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<BranchOutput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 11> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::id, offsetof(BranchOutput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::energized, offsetof(BranchOutput<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::loading, offsetof(BranchOutput<sym>, loading), []{ return "loading"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::p_from, offsetof(BranchOutput<sym>, p_from), []{ return "p_from"; }>::value,
@@ -61,16 +65,18 @@
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::p_to, offsetof(BranchOutput<sym>, p_to), []{ return "p_to"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::q_to, offsetof(BranchOutput<sym>, q_to), []{ return "q_to"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::i_to, offsetof(BranchOutput<sym>, i_to), []{ return "i_to"; }>::value,
             meta_data_gen::get_meta_attribute<BranchOutput<sym>, &BranchOutput<sym>::s_to, offsetof(BranchOutput<sym>, s_to), []{ return "s_to"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<Branch3Output<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<Branch3Output<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 15> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::id, offsetof(Branch3Output<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::energized, offsetof(Branch3Output<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::loading, offsetof(Branch3Output<sym>, loading), []{ return "loading"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::p_1, offsetof(Branch3Output<sym>, p_1), []{ return "p_1"; }>::value,
@@ -84,43 +90,49 @@
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::p_3, offsetof(Branch3Output<sym>, p_3), []{ return "p_3"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::q_3, offsetof(Branch3Output<sym>, q_3), []{ return "q_3"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::i_3, offsetof(Branch3Output<sym>, i_3), []{ return "i_3"; }>::value,
             meta_data_gen::get_meta_attribute<Branch3Output<sym>, &Branch3Output<sym>::s_3, offsetof(Branch3Output<sym>, s_3), []{ return "s_3"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<ApplianceOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<ApplianceOutput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 7> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::id, offsetof(ApplianceOutput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::energized, offsetof(ApplianceOutput<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::p, offsetof(ApplianceOutput<sym>, p), []{ return "p"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::q, offsetof(ApplianceOutput<sym>, q), []{ return "q"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::i, offsetof(ApplianceOutput<sym>, i), []{ return "i"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::s, offsetof(ApplianceOutput<sym>, s), []{ return "s"; }>::value,
             meta_data_gen::get_meta_attribute<ApplianceOutput<sym>, &ApplianceOutput<sym>::pf, offsetof(ApplianceOutput<sym>, pf), []{ return "pf"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<VoltageSensorOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<VoltageSensorOutput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 4> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<VoltageSensorOutput<sym>, &VoltageSensorOutput<sym>::id, offsetof(VoltageSensorOutput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorOutput<sym>, &VoltageSensorOutput<sym>::energized, offsetof(VoltageSensorOutput<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorOutput<sym>, &VoltageSensorOutput<sym>::u_residual, offsetof(VoltageSensorOutput<sym>, u_residual), []{ return "u_residual"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorOutput<sym>, &VoltageSensorOutput<sym>::u_angle_residual, offsetof(VoltageSensorOutput<sym>, u_angle_residual), []{ return "u_angle_residual"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<PowerSensorOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<PowerSensorOutput<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 4> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<PowerSensorOutput<sym>, &PowerSensorOutput<sym>::id, offsetof(PowerSensorOutput<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorOutput<sym>, &PowerSensorOutput<sym>::energized, offsetof(PowerSensorOutput<sym>, energized), []{ return "energized"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorOutput<sym>, &PowerSensorOutput<sym>::p_residual, offsetof(PowerSensorOutput<sym>, p_residual), []{ return "p_residual"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorOutput<sym>, &PowerSensorOutput<sym>::q_residual, offsetof(PowerSensorOutput<sym>, q_residual), []{ return "q_residual"; }>::value,
@@ -226,16 +238,18 @@
         
         set_nan(comp.id);
         set_nan(comp.energized);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<NodeOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<NodeOutput<sym_type>> {
+    using sym = sym_type;
+
     NodeOutput<sym> operator() () const {
         NodeOutput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.u_pu);
@@ -243,16 +257,18 @@
         set_nan(comp.u_angle);
         set_nan(comp.p);
         set_nan(comp.q);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<BranchOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<BranchOutput<sym_type>> {
+    using sym = sym_type;
+
     BranchOutput<sym> operator() () const {
         BranchOutput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.loading);
@@ -264,16 +280,18 @@
         set_nan(comp.q_to);
         set_nan(comp.i_to);
         set_nan(comp.s_to);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<Branch3Output<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<Branch3Output<sym_type>> {
+    using sym = sym_type;
+
     Branch3Output<sym> operator() () const {
         Branch3Output<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.loading);
@@ -289,16 +307,18 @@
         set_nan(comp.q_3);
         set_nan(comp.i_3);
         set_nan(comp.s_3);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<ApplianceOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<ApplianceOutput<sym_type>> {
+    using sym = sym_type;
+
     ApplianceOutput<sym> operator() () const {
         ApplianceOutput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.p);
@@ -306,30 +326,34 @@
         set_nan(comp.i);
         set_nan(comp.s);
         set_nan(comp.pf);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<VoltageSensorOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<VoltageSensorOutput<sym_type>> {
+    using sym = sym_type;
+
     VoltageSensorOutput<sym> operator() () const {
         VoltageSensorOutput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.u_residual);
         set_nan(comp.u_angle_residual);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<PowerSensorOutput<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<PowerSensorOutput<sym_type>> {
+    using sym = sym_type;
+
     PowerSensorOutput<sym> operator() () const {
         PowerSensorOutput<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.energized);
         set_nan(comp.p_residual);
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,18 @@
             meta_data_gen::get_meta_attribute<ThreeWindingTransformerUpdate, &ThreeWindingTransformerUpdate::status_1, offsetof(ThreeWindingTransformerUpdate, status_1), []{ return "status_1"; }>::value,
             meta_data_gen::get_meta_attribute<ThreeWindingTransformerUpdate, &ThreeWindingTransformerUpdate::status_2, offsetof(ThreeWindingTransformerUpdate, status_2), []{ return "status_2"; }>::value,
             meta_data_gen::get_meta_attribute<ThreeWindingTransformerUpdate, &ThreeWindingTransformerUpdate::status_3, offsetof(ThreeWindingTransformerUpdate, status_3), []{ return "status_3"; }>::value,
             meta_data_gen::get_meta_attribute<ThreeWindingTransformerUpdate, &ThreeWindingTransformerUpdate::tap_pos, offsetof(ThreeWindingTransformerUpdate, tap_pos), []{ return "tap_pos"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<LoadGenUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<LoadGenUpdate<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 4> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<LoadGenUpdate<sym>, &LoadGenUpdate<sym>::id, offsetof(LoadGenUpdate<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenUpdate<sym>, &LoadGenUpdate<sym>::status, offsetof(LoadGenUpdate<sym>, status), []{ return "status"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenUpdate<sym>, &LoadGenUpdate<sym>::p_specified, offsetof(LoadGenUpdate<sym>, p_specified), []{ return "p_specified"; }>::value,
             meta_data_gen::get_meta_attribute<LoadGenUpdate<sym>, &LoadGenUpdate<sym>::q_specified, offsetof(LoadGenUpdate<sym>, q_specified), []{ return "q_specified"; }>::value,
@@ -122,28 +124,32 @@
             meta_data_gen::get_meta_attribute<ShuntUpdate, &ShuntUpdate::g1, offsetof(ShuntUpdate, g1), []{ return "g1"; }>::value,
             meta_data_gen::get_meta_attribute<ShuntUpdate, &ShuntUpdate::b1, offsetof(ShuntUpdate, b1), []{ return "b1"; }>::value,
             meta_data_gen::get_meta_attribute<ShuntUpdate, &ShuntUpdate::g0, offsetof(ShuntUpdate, g0), []{ return "g0"; }>::value,
             meta_data_gen::get_meta_attribute<ShuntUpdate, &ShuntUpdate::b0, offsetof(ShuntUpdate, b0), []{ return "b0"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<VoltageSensorUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<VoltageSensorUpdate<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 4> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<VoltageSensorUpdate<sym>, &VoltageSensorUpdate<sym>::id, offsetof(VoltageSensorUpdate<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorUpdate<sym>, &VoltageSensorUpdate<sym>::u_sigma, offsetof(VoltageSensorUpdate<sym>, u_sigma), []{ return "u_sigma"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorUpdate<sym>, &VoltageSensorUpdate<sym>::u_measured, offsetof(VoltageSensorUpdate<sym>, u_measured), []{ return "u_measured"; }>::value,
             meta_data_gen::get_meta_attribute<VoltageSensorUpdate<sym>, &VoltageSensorUpdate<sym>::u_angle_measured, offsetof(VoltageSensorUpdate<sym>, u_angle_measured), []{ return "u_angle_measured"; }>::value,
     };
 };
 
-template <bool sym>
-struct get_attributes_list<PowerSensorUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_attributes_list<PowerSensorUpdate<sym_type>> {
+    using sym = sym_type;
+
     static constexpr std::array<MetaAttribute, 6> value{
             // all attributes including base class
             
             meta_data_gen::get_meta_attribute<PowerSensorUpdate<sym>, &PowerSensorUpdate<sym>::id, offsetof(PowerSensorUpdate<sym>, id), []{ return "id"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorUpdate<sym>, &PowerSensorUpdate<sym>::power_sigma, offsetof(PowerSensorUpdate<sym>, power_sigma), []{ return "power_sigma"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorUpdate<sym>, &PowerSensorUpdate<sym>::p_measured, offsetof(PowerSensorUpdate<sym>, p_measured), []{ return "p_measured"; }>::value,
             meta_data_gen::get_meta_attribute<PowerSensorUpdate<sym>, &PowerSensorUpdate<sym>::q_measured, offsetof(PowerSensorUpdate<sym>, q_measured), []{ return "q_measured"; }>::value,
@@ -246,16 +252,18 @@
         set_nan(comp.status_2);
         set_nan(comp.status_3);
         set_nan(comp.tap_pos);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<LoadGenUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<LoadGenUpdate<sym_type>> {
+    using sym = sym_type;
+
     LoadGenUpdate<sym> operator() () const {
         LoadGenUpdate<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.status);
         set_nan(comp.p_specified);
@@ -290,30 +298,34 @@
         set_nan(comp.b1);
         set_nan(comp.g0);
         set_nan(comp.b0);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<VoltageSensorUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<VoltageSensorUpdate<sym_type>> {
+    using sym = sym_type;
+
     VoltageSensorUpdate<sym> operator() () const {
         VoltageSensorUpdate<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.u_sigma);
         set_nan(comp.u_measured);
         set_nan(comp.u_angle_measured);
         return comp;
     }
 };
 
-template <bool sym>
-struct get_component_nan<PowerSensorUpdate<sym>> {
+template <symmetry_tag sym_type>
+struct get_component_nan<PowerSensorUpdate<sym_type>> {
+    using sym = sym_type;
+
     PowerSensorUpdate<sym> operator() () const {
         PowerSensorUpdate<sym> comp;
         // all attributes including base class
         
         set_nan(comp.id);
         set_nan(comp.power_sigma);
         set_nan(comp.p_measured);
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -16,34 +16,38 @@
 namespace power_grid_model {
 
 struct BaseOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct NodeOutput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     RealValue<sym> u_pu;  // voltage magnitude and angle
     RealValue<sym> u;  // voltage magnitude and angle
     RealValue<sym> u_angle;  // voltage magnitude and angle
     RealValue<sym> p;  // node injection
     RealValue<sym> q;  // node injection
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymNodeOutput = NodeOutput<true>;
-using AsymNodeOutput = NodeOutput<false>;
+using SymNodeOutput = NodeOutput<symmetric_t>;
+using AsymNodeOutput = NodeOutput<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct BranchOutput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     double loading;  // loading of the branch
     RealValue<sym> p_from;  // power flow at from-side
     RealValue<sym> q_from;  // power flow at from-side
     RealValue<sym> i_from;  // power flow at from-side
     RealValue<sym> s_from;  // power flow at from-side
@@ -53,19 +57,21 @@
     RealValue<sym> s_to;  // power flow at to-side
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymBranchOutput = BranchOutput<true>;
-using AsymBranchOutput = BranchOutput<false>;
+using SymBranchOutput = BranchOutput<symmetric_t>;
+using AsymBranchOutput = BranchOutput<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct Branch3Output {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     double loading;  // loading of the branch
     RealValue<sym> p_1;  // power flow at side 1
     RealValue<sym> q_1;  // power flow at side 1
     RealValue<sym> i_1;  // power flow at side 1
     RealValue<sym> s_1;  // power flow at side 1
@@ -79,130 +85,136 @@
     RealValue<sym> s_3;  // power flow at side 3
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymBranch3Output = Branch3Output<true>;
-using AsymBranch3Output = Branch3Output<false>;
+using SymBranch3Output = Branch3Output<symmetric_t>;
+using AsymBranch3Output = Branch3Output<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct ApplianceOutput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     RealValue<sym> p;  // power flow of the appliance
     RealValue<sym> q;  // power flow of the appliance
     RealValue<sym> i;  // power flow of the appliance
     RealValue<sym> s;  // power flow of the appliance
     RealValue<sym> pf;  // power flow of the appliance
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymApplianceOutput = ApplianceOutput<true>;
-using AsymApplianceOutput = ApplianceOutput<false>;
+using SymApplianceOutput = ApplianceOutput<symmetric_t>;
+using AsymApplianceOutput = ApplianceOutput<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct VoltageSensorOutput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     RealValue<sym> u_residual;  // deviation between the measured value and calculated value
     RealValue<sym> u_angle_residual;  // deviation between the measured value and calculated value
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymVoltageSensorOutput = VoltageSensorOutput<true>;
-using AsymVoltageSensorOutput = VoltageSensorOutput<false>;
+using SymVoltageSensorOutput = VoltageSensorOutput<symmetric_t>;
+using AsymVoltageSensorOutput = VoltageSensorOutput<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct PowerSensorOutput {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
     RealValue<sym> p_residual;  // deviation between the measured value and calculated value
     RealValue<sym> q_residual;  // deviation between the measured value and calculated value
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
-using SymPowerSensorOutput = PowerSensorOutput<true>;
-using AsymPowerSensorOutput = PowerSensorOutput<false>;
+using SymPowerSensorOutput = PowerSensorOutput<symmetric_t>;
+using AsymPowerSensorOutput = PowerSensorOutput<asymmetric_t>;
 
 struct FaultOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct FaultShortCircuitOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
-    RealValue<false> i_f;  // three phase short circuit current magnitude
-    RealValue<false> i_f_angle;  // three phase short circuit current angle
+    RealValue<asymmetric_t> i_f;  // three phase short circuit current magnitude
+    RealValue<asymmetric_t> i_f_angle;  // three phase short circuit current angle
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct NodeShortCircuitOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
-    RealValue<false> u_pu;  // initial three phase line-to-ground short circuit voltage magnitude and angle
-    RealValue<false> u;  // initial three phase line-to-ground short circuit voltage magnitude and angle
-    RealValue<false> u_angle;  // initial three phase line-to-ground short circuit voltage magnitude and angle
+    RealValue<asymmetric_t> u_pu;  // initial three phase line-to-ground short circuit voltage magnitude and angle
+    RealValue<asymmetric_t> u;  // initial three phase line-to-ground short circuit voltage magnitude and angle
+    RealValue<asymmetric_t> u_angle;  // initial three phase line-to-ground short circuit voltage magnitude and angle
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct BranchShortCircuitOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
-    RealValue<false> i_from;  // initial three phase short circuit current flow at from-side
-    RealValue<false> i_from_angle;  // initial three phase short circuit current flow at from-side
-    RealValue<false> i_to;  // initial three phase short circuit current flow at to-side
-    RealValue<false> i_to_angle;  // initial three phase short circuit current flow at to-side
+    RealValue<asymmetric_t> i_from;  // initial three phase short circuit current flow at from-side
+    RealValue<asymmetric_t> i_from_angle;  // initial three phase short circuit current flow at from-side
+    RealValue<asymmetric_t> i_to;  // initial three phase short circuit current flow at to-side
+    RealValue<asymmetric_t> i_to_angle;  // initial three phase short circuit current flow at to-side
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct Branch3ShortCircuitOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
-    RealValue<false> i_1;  // initial three phase short circuit current flow at side 1
-    RealValue<false> i_1_angle;  // initial three phase short circuit current flow at side 1
-    RealValue<false> i_2;  // initial three phase short circuit current flow at side 2
-    RealValue<false> i_2_angle;  // initial three phase short circuit current flow at side 2
-    RealValue<false> i_3;  // initial three phase short circuit current flow at side 3
-    RealValue<false> i_3_angle;  // initial three phase short circuit current flow at side 3
+    RealValue<asymmetric_t> i_1;  // initial three phase short circuit current flow at side 1
+    RealValue<asymmetric_t> i_1_angle;  // initial three phase short circuit current flow at side 1
+    RealValue<asymmetric_t> i_2;  // initial three phase short circuit current flow at side 2
+    RealValue<asymmetric_t> i_2_angle;  // initial three phase short circuit current flow at side 2
+    RealValue<asymmetric_t> i_3;  // initial three phase short circuit current flow at side 3
+    RealValue<asymmetric_t> i_3_angle;  // initial three phase short circuit current flow at side 3
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct ApplianceShortCircuitOutput {
     ID id;  // ID of the object
     IntS energized;  // whether the object is energized
-    RealValue<false> i;  // initial three phase short circuit current flow of the appliance
-    RealValue<false> i_angle;  // initial three phase short circuit current flow of the appliance
+    RealValue<asymmetric_t> i;  // initial three phase short circuit current flow of the appliance
+    RealValue<asymmetric_t> i_angle;  // initial three phase short circuit current flow of the appliance
 
     // implicit conversions to BaseOutput
     operator BaseOutput&() { return reinterpret_cast<BaseOutput&>(*this); }
     operator BaseOutput const&() const { return reinterpret_cast<BaseOutput const&>(*this); }
 };
 
 struct SensorShortCircuitOutput {
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/deserializer.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/deserializer.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -287,18 +287,18 @@
     }
     bool visit_float64(double v) {
         value = v;
         return true;
     }
 };
 
-template <> struct ValueVisitor<RealValue<false>> : DefaultErrorVisitor<ValueVisitor<RealValue<false>>> {
+template <> struct ValueVisitor<RealValue<asymmetric_t>> : DefaultErrorVisitor<ValueVisitor<RealValue<asymmetric_t>>> {
     static constexpr std::string_view static_err_msg = "Expect an array of 3 numbers.";
 
-    RealValue<false>& value; // NOLINT(cppcoreguidelines-avoid-const-or-ref-data-members)
+    RealValue<asymmetric_t>& value; // NOLINT(cppcoreguidelines-avoid-const-or-ref-data-members)
     Idx idx{};
     bool inside_array{};
 
     bool visit_nil() { return true; } // NOLINT(readability-convert-member-functions-to-static)
     bool start_array(uint32_t num_elements) {
         if (inside_array || num_elements != 3) {
             this->throw_error();
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/serializer.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/serialization/serializer.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,19 @@
         msgpack::packer<Stream>& operator()(msgpack::packer<Stream>& p, T const* const& o) const {
             p.pack(o->name);
             return p;
         }
     };
 
     // pack double[3]
-    template <> struct pack<power_grid_model::RealValue<false>> {
+    template <> struct pack<power_grid_model::RealValue<power_grid_model::asymmetric_t>> {
         template <typename Stream>
-        msgpack::packer<Stream>& operator()(msgpack::packer<Stream>& p,
-                                            power_grid_model::RealValue<false> const& o) const {
+        msgpack::packer<Stream>&
+        operator()(msgpack::packer<Stream>& p,
+                   power_grid_model::RealValue<power_grid_model::asymmetric_t> const& o) const {
             p.pack_array(3);
             for (int8_t i = 0; i != 3; ++i) {
                 if (power_grid_model::is_nan(o(i))) {
                     p.pack_nil();
                 } else {
                     p.pack(o(i));
                 }
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/input.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/input.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -142,62 +142,62 @@
 static_assert(std::same_as<decltype(GenericLoadGenInput::id), decltype(ApplianceInput::id)>);
 static_assert(std::same_as<decltype(GenericLoadGenInput::node), decltype(ApplianceInput::node)>);
 static_assert(std::same_as<decltype(GenericLoadGenInput::status), decltype(ApplianceInput::status)>);
 static_assert(offsetof(GenericLoadGenInput, id) == offsetof(ApplianceInput, id));
 static_assert(offsetof(GenericLoadGenInput, node) == offsetof(ApplianceInput, node));
 static_assert(offsetof(GenericLoadGenInput, status) == offsetof(ApplianceInput, status));
 
-// static asserts for LoadGenInput<true>
-static_assert(std::is_standard_layout_v<LoadGenInput<true>>);
-// static asserts for conversion of LoadGenInput<true> to BaseInput
-static_assert(std::alignment_of_v<LoadGenInput<true>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(LoadGenInput<true>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of LoadGenInput<true> to ApplianceInput
-static_assert(std::alignment_of_v<LoadGenInput<true>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::id), decltype(ApplianceInput::id)>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::node), decltype(ApplianceInput::node)>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::status), decltype(ApplianceInput::status)>);
-static_assert(offsetof(LoadGenInput<true>, id) == offsetof(ApplianceInput, id));
-static_assert(offsetof(LoadGenInput<true>, node) == offsetof(ApplianceInput, node));
-static_assert(offsetof(LoadGenInput<true>, status) == offsetof(ApplianceInput, status));
-// static asserts for conversion of LoadGenInput<true> to GenericLoadGenInput
-static_assert(std::alignment_of_v<LoadGenInput<true>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::id), decltype(GenericLoadGenInput::id)>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::node), decltype(GenericLoadGenInput::node)>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::status), decltype(GenericLoadGenInput::status)>);
-static_assert(std::same_as<decltype(LoadGenInput<true>::type), decltype(GenericLoadGenInput::type)>);
-static_assert(offsetof(LoadGenInput<true>, id) == offsetof(GenericLoadGenInput, id));
-static_assert(offsetof(LoadGenInput<true>, node) == offsetof(GenericLoadGenInput, node));
-static_assert(offsetof(LoadGenInput<true>, status) == offsetof(GenericLoadGenInput, status));
-static_assert(offsetof(LoadGenInput<true>, type) == offsetof(GenericLoadGenInput, type));
-// static asserts for LoadGenInput<false>
-static_assert(std::is_standard_layout_v<LoadGenInput<false>>);
-// static asserts for conversion of LoadGenInput<false> to BaseInput
-static_assert(std::alignment_of_v<LoadGenInput<false>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(LoadGenInput<false>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of LoadGenInput<false> to ApplianceInput
-static_assert(std::alignment_of_v<LoadGenInput<false>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::id), decltype(ApplianceInput::id)>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::node), decltype(ApplianceInput::node)>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::status), decltype(ApplianceInput::status)>);
-static_assert(offsetof(LoadGenInput<false>, id) == offsetof(ApplianceInput, id));
-static_assert(offsetof(LoadGenInput<false>, node) == offsetof(ApplianceInput, node));
-static_assert(offsetof(LoadGenInput<false>, status) == offsetof(ApplianceInput, status));
-// static asserts for conversion of LoadGenInput<false> to GenericLoadGenInput
-static_assert(std::alignment_of_v<LoadGenInput<false>> >= std::alignment_of_v<GenericLoadGenInput>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::id), decltype(GenericLoadGenInput::id)>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::node), decltype(GenericLoadGenInput::node)>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::status), decltype(GenericLoadGenInput::status)>);
-static_assert(std::same_as<decltype(LoadGenInput<false>::type), decltype(GenericLoadGenInput::type)>);
-static_assert(offsetof(LoadGenInput<false>, id) == offsetof(GenericLoadGenInput, id));
-static_assert(offsetof(LoadGenInput<false>, node) == offsetof(GenericLoadGenInput, node));
-static_assert(offsetof(LoadGenInput<false>, status) == offsetof(GenericLoadGenInput, status));
-static_assert(offsetof(LoadGenInput<false>, type) == offsetof(GenericLoadGenInput, type));
+// static asserts for LoadGenInput<symmetric_t>
+static_assert(std::is_standard_layout_v<LoadGenInput<symmetric_t>>);
+// static asserts for conversion of LoadGenInput<symmetric_t> to BaseInput
+static_assert(std::alignment_of_v<LoadGenInput<symmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(LoadGenInput<symmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of LoadGenInput<symmetric_t> to ApplianceInput
+static_assert(std::alignment_of_v<LoadGenInput<symmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::id), decltype(ApplianceInput::id)>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::node), decltype(ApplianceInput::node)>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::status), decltype(ApplianceInput::status)>);
+static_assert(offsetof(LoadGenInput<symmetric_t>, id) == offsetof(ApplianceInput, id));
+static_assert(offsetof(LoadGenInput<symmetric_t>, node) == offsetof(ApplianceInput, node));
+static_assert(offsetof(LoadGenInput<symmetric_t>, status) == offsetof(ApplianceInput, status));
+// static asserts for conversion of LoadGenInput<symmetric_t> to GenericLoadGenInput
+static_assert(std::alignment_of_v<LoadGenInput<symmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::id), decltype(GenericLoadGenInput::id)>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::node), decltype(GenericLoadGenInput::node)>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::status), decltype(GenericLoadGenInput::status)>);
+static_assert(std::same_as<decltype(LoadGenInput<symmetric_t>::type), decltype(GenericLoadGenInput::type)>);
+static_assert(offsetof(LoadGenInput<symmetric_t>, id) == offsetof(GenericLoadGenInput, id));
+static_assert(offsetof(LoadGenInput<symmetric_t>, node) == offsetof(GenericLoadGenInput, node));
+static_assert(offsetof(LoadGenInput<symmetric_t>, status) == offsetof(GenericLoadGenInput, status));
+static_assert(offsetof(LoadGenInput<symmetric_t>, type) == offsetof(GenericLoadGenInput, type));
+// static asserts for LoadGenInput<asymmetric_t>
+static_assert(std::is_standard_layout_v<LoadGenInput<asymmetric_t>>);
+// static asserts for conversion of LoadGenInput<asymmetric_t> to BaseInput
+static_assert(std::alignment_of_v<LoadGenInput<asymmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(LoadGenInput<asymmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of LoadGenInput<asymmetric_t> to ApplianceInput
+static_assert(std::alignment_of_v<LoadGenInput<asymmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::id), decltype(ApplianceInput::id)>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::node), decltype(ApplianceInput::node)>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::status), decltype(ApplianceInput::status)>);
+static_assert(offsetof(LoadGenInput<asymmetric_t>, id) == offsetof(ApplianceInput, id));
+static_assert(offsetof(LoadGenInput<asymmetric_t>, node) == offsetof(ApplianceInput, node));
+static_assert(offsetof(LoadGenInput<asymmetric_t>, status) == offsetof(ApplianceInput, status));
+// static asserts for conversion of LoadGenInput<asymmetric_t> to GenericLoadGenInput
+static_assert(std::alignment_of_v<LoadGenInput<asymmetric_t>> >= std::alignment_of_v<GenericLoadGenInput>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::id), decltype(GenericLoadGenInput::id)>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::node), decltype(GenericLoadGenInput::node)>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::status), decltype(GenericLoadGenInput::status)>);
+static_assert(std::same_as<decltype(LoadGenInput<asymmetric_t>::type), decltype(GenericLoadGenInput::type)>);
+static_assert(offsetof(LoadGenInput<asymmetric_t>, id) == offsetof(GenericLoadGenInput, id));
+static_assert(offsetof(LoadGenInput<asymmetric_t>, node) == offsetof(GenericLoadGenInput, node));
+static_assert(offsetof(LoadGenInput<asymmetric_t>, status) == offsetof(GenericLoadGenInput, status));
+static_assert(offsetof(LoadGenInput<asymmetric_t>, type) == offsetof(GenericLoadGenInput, type));
 // static asserts for SymLoadGenInput
 static_assert(std::is_standard_layout_v<SymLoadGenInput>);
 // static asserts for conversion of SymLoadGenInput to BaseInput
 static_assert(std::alignment_of_v<SymLoadGenInput> >= std::alignment_of_v<GenericLoadGenInput>);
 static_assert(std::same_as<decltype(SymLoadGenInput::id), decltype(BaseInput::id)>);
 static_assert(offsetof(SymLoadGenInput, id) == offsetof(BaseInput, id));
 // static asserts for conversion of SymLoadGenInput to ApplianceInput
@@ -282,54 +282,54 @@
 // static asserts for conversion of GenericVoltageSensorInput to SensorInput
 static_assert(std::alignment_of_v<GenericVoltageSensorInput> >= std::alignment_of_v<SensorInput>);
 static_assert(std::same_as<decltype(GenericVoltageSensorInput::id), decltype(SensorInput::id)>);
 static_assert(std::same_as<decltype(GenericVoltageSensorInput::measured_object), decltype(SensorInput::measured_object)>);
 static_assert(offsetof(GenericVoltageSensorInput, id) == offsetof(SensorInput, id));
 static_assert(offsetof(GenericVoltageSensorInput, measured_object) == offsetof(SensorInput, measured_object));
 
-// static asserts for VoltageSensorInput<true>
-static_assert(std::is_standard_layout_v<VoltageSensorInput<true>>);
-// static asserts for conversion of VoltageSensorInput<true> to BaseInput
-static_assert(std::alignment_of_v<VoltageSensorInput<true>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(VoltageSensorInput<true>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of VoltageSensorInput<true> to SensorInput
-static_assert(std::alignment_of_v<VoltageSensorInput<true>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::id), decltype(SensorInput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::measured_object), decltype(SensorInput::measured_object)>);
-static_assert(offsetof(VoltageSensorInput<true>, id) == offsetof(SensorInput, id));
-static_assert(offsetof(VoltageSensorInput<true>, measured_object) == offsetof(SensorInput, measured_object));
-// static asserts for conversion of VoltageSensorInput<true> to GenericVoltageSensorInput
-static_assert(std::alignment_of_v<VoltageSensorInput<true>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::id), decltype(GenericVoltageSensorInput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::measured_object), decltype(GenericVoltageSensorInput::measured_object)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<true>::u_sigma), decltype(GenericVoltageSensorInput::u_sigma)>);
-static_assert(offsetof(VoltageSensorInput<true>, id) == offsetof(GenericVoltageSensorInput, id));
-static_assert(offsetof(VoltageSensorInput<true>, measured_object) == offsetof(GenericVoltageSensorInput, measured_object));
-static_assert(offsetof(VoltageSensorInput<true>, u_sigma) == offsetof(GenericVoltageSensorInput, u_sigma));
-// static asserts for VoltageSensorInput<false>
-static_assert(std::is_standard_layout_v<VoltageSensorInput<false>>);
-// static asserts for conversion of VoltageSensorInput<false> to BaseInput
-static_assert(std::alignment_of_v<VoltageSensorInput<false>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(VoltageSensorInput<false>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of VoltageSensorInput<false> to SensorInput
-static_assert(std::alignment_of_v<VoltageSensorInput<false>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::id), decltype(SensorInput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::measured_object), decltype(SensorInput::measured_object)>);
-static_assert(offsetof(VoltageSensorInput<false>, id) == offsetof(SensorInput, id));
-static_assert(offsetof(VoltageSensorInput<false>, measured_object) == offsetof(SensorInput, measured_object));
-// static asserts for conversion of VoltageSensorInput<false> to GenericVoltageSensorInput
-static_assert(std::alignment_of_v<VoltageSensorInput<false>> >= std::alignment_of_v<GenericVoltageSensorInput>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::id), decltype(GenericVoltageSensorInput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::measured_object), decltype(GenericVoltageSensorInput::measured_object)>);
-static_assert(std::same_as<decltype(VoltageSensorInput<false>::u_sigma), decltype(GenericVoltageSensorInput::u_sigma)>);
-static_assert(offsetof(VoltageSensorInput<false>, id) == offsetof(GenericVoltageSensorInput, id));
-static_assert(offsetof(VoltageSensorInput<false>, measured_object) == offsetof(GenericVoltageSensorInput, measured_object));
-static_assert(offsetof(VoltageSensorInput<false>, u_sigma) == offsetof(GenericVoltageSensorInput, u_sigma));
+// static asserts for VoltageSensorInput<symmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorInput<symmetric_t>>);
+// static asserts for conversion of VoltageSensorInput<symmetric_t> to BaseInput
+static_assert(std::alignment_of_v<VoltageSensorInput<symmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of VoltageSensorInput<symmetric_t> to SensorInput
+static_assert(std::alignment_of_v<VoltageSensorInput<symmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::id), decltype(SensorInput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::measured_object), decltype(SensorInput::measured_object)>);
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, id) == offsetof(SensorInput, id));
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, measured_object) == offsetof(SensorInput, measured_object));
+// static asserts for conversion of VoltageSensorInput<symmetric_t> to GenericVoltageSensorInput
+static_assert(std::alignment_of_v<VoltageSensorInput<symmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::id), decltype(GenericVoltageSensorInput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::measured_object), decltype(GenericVoltageSensorInput::measured_object)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<symmetric_t>::u_sigma), decltype(GenericVoltageSensorInput::u_sigma)>);
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, id) == offsetof(GenericVoltageSensorInput, id));
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, measured_object) == offsetof(GenericVoltageSensorInput, measured_object));
+static_assert(offsetof(VoltageSensorInput<symmetric_t>, u_sigma) == offsetof(GenericVoltageSensorInput, u_sigma));
+// static asserts for VoltageSensorInput<asymmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorInput<asymmetric_t>>);
+// static asserts for conversion of VoltageSensorInput<asymmetric_t> to BaseInput
+static_assert(std::alignment_of_v<VoltageSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of VoltageSensorInput<asymmetric_t> to SensorInput
+static_assert(std::alignment_of_v<VoltageSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::id), decltype(SensorInput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::measured_object), decltype(SensorInput::measured_object)>);
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, id) == offsetof(SensorInput, id));
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, measured_object) == offsetof(SensorInput, measured_object));
+// static asserts for conversion of VoltageSensorInput<asymmetric_t> to GenericVoltageSensorInput
+static_assert(std::alignment_of_v<VoltageSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericVoltageSensorInput>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::id), decltype(GenericVoltageSensorInput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::measured_object), decltype(GenericVoltageSensorInput::measured_object)>);
+static_assert(std::same_as<decltype(VoltageSensorInput<asymmetric_t>::u_sigma), decltype(GenericVoltageSensorInput::u_sigma)>);
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, id) == offsetof(GenericVoltageSensorInput, id));
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, measured_object) == offsetof(GenericVoltageSensorInput, measured_object));
+static_assert(offsetof(VoltageSensorInput<asymmetric_t>, u_sigma) == offsetof(GenericVoltageSensorInput, u_sigma));
 // static asserts for SymVoltageSensorInput
 static_assert(std::is_standard_layout_v<SymVoltageSensorInput>);
 // static asserts for conversion of SymVoltageSensorInput to BaseInput
 static_assert(std::alignment_of_v<SymVoltageSensorInput> >= std::alignment_of_v<GenericVoltageSensorInput>);
 static_assert(std::same_as<decltype(SymVoltageSensorInput::id), decltype(BaseInput::id)>);
 static_assert(offsetof(SymVoltageSensorInput, id) == offsetof(BaseInput, id));
 // static asserts for conversion of SymVoltageSensorInput to SensorInput
@@ -376,58 +376,58 @@
 // static asserts for conversion of GenericPowerSensorInput to SensorInput
 static_assert(std::alignment_of_v<GenericPowerSensorInput> >= std::alignment_of_v<SensorInput>);
 static_assert(std::same_as<decltype(GenericPowerSensorInput::id), decltype(SensorInput::id)>);
 static_assert(std::same_as<decltype(GenericPowerSensorInput::measured_object), decltype(SensorInput::measured_object)>);
 static_assert(offsetof(GenericPowerSensorInput, id) == offsetof(SensorInput, id));
 static_assert(offsetof(GenericPowerSensorInput, measured_object) == offsetof(SensorInput, measured_object));
 
-// static asserts for PowerSensorInput<true>
-static_assert(std::is_standard_layout_v<PowerSensorInput<true>>);
-// static asserts for conversion of PowerSensorInput<true> to BaseInput
-static_assert(std::alignment_of_v<PowerSensorInput<true>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(PowerSensorInput<true>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of PowerSensorInput<true> to SensorInput
-static_assert(std::alignment_of_v<PowerSensorInput<true>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::id), decltype(SensorInput::id)>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::measured_object), decltype(SensorInput::measured_object)>);
-static_assert(offsetof(PowerSensorInput<true>, id) == offsetof(SensorInput, id));
-static_assert(offsetof(PowerSensorInput<true>, measured_object) == offsetof(SensorInput, measured_object));
-// static asserts for conversion of PowerSensorInput<true> to GenericPowerSensorInput
-static_assert(std::alignment_of_v<PowerSensorInput<true>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::id), decltype(GenericPowerSensorInput::id)>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::measured_object), decltype(GenericPowerSensorInput::measured_object)>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::measured_terminal_type), decltype(GenericPowerSensorInput::measured_terminal_type)>);
-static_assert(std::same_as<decltype(PowerSensorInput<true>::power_sigma), decltype(GenericPowerSensorInput::power_sigma)>);
-static_assert(offsetof(PowerSensorInput<true>, id) == offsetof(GenericPowerSensorInput, id));
-static_assert(offsetof(PowerSensorInput<true>, measured_object) == offsetof(GenericPowerSensorInput, measured_object));
-static_assert(offsetof(PowerSensorInput<true>, measured_terminal_type) == offsetof(GenericPowerSensorInput, measured_terminal_type));
-static_assert(offsetof(PowerSensorInput<true>, power_sigma) == offsetof(GenericPowerSensorInput, power_sigma));
-// static asserts for PowerSensorInput<false>
-static_assert(std::is_standard_layout_v<PowerSensorInput<false>>);
-// static asserts for conversion of PowerSensorInput<false> to BaseInput
-static_assert(std::alignment_of_v<PowerSensorInput<false>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::id), decltype(BaseInput::id)>);
-static_assert(offsetof(PowerSensorInput<false>, id) == offsetof(BaseInput, id));
-// static asserts for conversion of PowerSensorInput<false> to SensorInput
-static_assert(std::alignment_of_v<PowerSensorInput<false>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::id), decltype(SensorInput::id)>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::measured_object), decltype(SensorInput::measured_object)>);
-static_assert(offsetof(PowerSensorInput<false>, id) == offsetof(SensorInput, id));
-static_assert(offsetof(PowerSensorInput<false>, measured_object) == offsetof(SensorInput, measured_object));
-// static asserts for conversion of PowerSensorInput<false> to GenericPowerSensorInput
-static_assert(std::alignment_of_v<PowerSensorInput<false>> >= std::alignment_of_v<GenericPowerSensorInput>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::id), decltype(GenericPowerSensorInput::id)>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::measured_object), decltype(GenericPowerSensorInput::measured_object)>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::measured_terminal_type), decltype(GenericPowerSensorInput::measured_terminal_type)>);
-static_assert(std::same_as<decltype(PowerSensorInput<false>::power_sigma), decltype(GenericPowerSensorInput::power_sigma)>);
-static_assert(offsetof(PowerSensorInput<false>, id) == offsetof(GenericPowerSensorInput, id));
-static_assert(offsetof(PowerSensorInput<false>, measured_object) == offsetof(GenericPowerSensorInput, measured_object));
-static_assert(offsetof(PowerSensorInput<false>, measured_terminal_type) == offsetof(GenericPowerSensorInput, measured_terminal_type));
-static_assert(offsetof(PowerSensorInput<false>, power_sigma) == offsetof(GenericPowerSensorInput, power_sigma));
+// static asserts for PowerSensorInput<symmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorInput<symmetric_t>>);
+// static asserts for conversion of PowerSensorInput<symmetric_t> to BaseInput
+static_assert(std::alignment_of_v<PowerSensorInput<symmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(PowerSensorInput<symmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of PowerSensorInput<symmetric_t> to SensorInput
+static_assert(std::alignment_of_v<PowerSensorInput<symmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::id), decltype(SensorInput::id)>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::measured_object), decltype(SensorInput::measured_object)>);
+static_assert(offsetof(PowerSensorInput<symmetric_t>, id) == offsetof(SensorInput, id));
+static_assert(offsetof(PowerSensorInput<symmetric_t>, measured_object) == offsetof(SensorInput, measured_object));
+// static asserts for conversion of PowerSensorInput<symmetric_t> to GenericPowerSensorInput
+static_assert(std::alignment_of_v<PowerSensorInput<symmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::id), decltype(GenericPowerSensorInput::id)>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::measured_object), decltype(GenericPowerSensorInput::measured_object)>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::measured_terminal_type), decltype(GenericPowerSensorInput::measured_terminal_type)>);
+static_assert(std::same_as<decltype(PowerSensorInput<symmetric_t>::power_sigma), decltype(GenericPowerSensorInput::power_sigma)>);
+static_assert(offsetof(PowerSensorInput<symmetric_t>, id) == offsetof(GenericPowerSensorInput, id));
+static_assert(offsetof(PowerSensorInput<symmetric_t>, measured_object) == offsetof(GenericPowerSensorInput, measured_object));
+static_assert(offsetof(PowerSensorInput<symmetric_t>, measured_terminal_type) == offsetof(GenericPowerSensorInput, measured_terminal_type));
+static_assert(offsetof(PowerSensorInput<symmetric_t>, power_sigma) == offsetof(GenericPowerSensorInput, power_sigma));
+// static asserts for PowerSensorInput<asymmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorInput<asymmetric_t>>);
+// static asserts for conversion of PowerSensorInput<asymmetric_t> to BaseInput
+static_assert(std::alignment_of_v<PowerSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::id), decltype(BaseInput::id)>);
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, id) == offsetof(BaseInput, id));
+// static asserts for conversion of PowerSensorInput<asymmetric_t> to SensorInput
+static_assert(std::alignment_of_v<PowerSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::id), decltype(SensorInput::id)>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::measured_object), decltype(SensorInput::measured_object)>);
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, id) == offsetof(SensorInput, id));
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, measured_object) == offsetof(SensorInput, measured_object));
+// static asserts for conversion of PowerSensorInput<asymmetric_t> to GenericPowerSensorInput
+static_assert(std::alignment_of_v<PowerSensorInput<asymmetric_t>> >= std::alignment_of_v<GenericPowerSensorInput>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::id), decltype(GenericPowerSensorInput::id)>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::measured_object), decltype(GenericPowerSensorInput::measured_object)>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::measured_terminal_type), decltype(GenericPowerSensorInput::measured_terminal_type)>);
+static_assert(std::same_as<decltype(PowerSensorInput<asymmetric_t>::power_sigma), decltype(GenericPowerSensorInput::power_sigma)>);
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, id) == offsetof(GenericPowerSensorInput, id));
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, measured_object) == offsetof(GenericPowerSensorInput, measured_object));
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, measured_terminal_type) == offsetof(GenericPowerSensorInput, measured_terminal_type));
+static_assert(offsetof(PowerSensorInput<asymmetric_t>, power_sigma) == offsetof(GenericPowerSensorInput, power_sigma));
 // static asserts for SymPowerSensorInput
 static_assert(std::is_standard_layout_v<SymPowerSensorInput>);
 // static asserts for conversion of SymPowerSensorInput to BaseInput
 static_assert(std::alignment_of_v<SymPowerSensorInput> >= std::alignment_of_v<GenericPowerSensorInput>);
 static_assert(std::same_as<decltype(SymPowerSensorInput::id), decltype(BaseInput::id)>);
 static_assert(offsetof(SymPowerSensorInput, id) == offsetof(BaseInput, id));
 // static asserts for conversion of SymPowerSensorInput to SensorInput
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/output.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/output.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 #include <cstddef>
 
 namespace power_grid_model::test {
 
 // static asserts for BaseOutput
 static_assert(std::is_standard_layout_v<BaseOutput>);
 
-// static asserts for NodeOutput<true>
-static_assert(std::is_standard_layout_v<NodeOutput<true>>);
-// static asserts for conversion of NodeOutput<true> to BaseOutput
-static_assert(std::alignment_of_v<NodeOutput<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(NodeOutput<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(NodeOutput<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(NodeOutput<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(NodeOutput<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for NodeOutput<false>
-static_assert(std::is_standard_layout_v<NodeOutput<false>>);
-// static asserts for conversion of NodeOutput<false> to BaseOutput
-static_assert(std::alignment_of_v<NodeOutput<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(NodeOutput<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(NodeOutput<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(NodeOutput<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(NodeOutput<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for NodeOutput<symmetric_t>
+static_assert(std::is_standard_layout_v<NodeOutput<symmetric_t>>);
+// static asserts for conversion of NodeOutput<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<NodeOutput<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(NodeOutput<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(NodeOutput<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(NodeOutput<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(NodeOutput<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for NodeOutput<asymmetric_t>
+static_assert(std::is_standard_layout_v<NodeOutput<asymmetric_t>>);
+// static asserts for conversion of NodeOutput<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<NodeOutput<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(NodeOutput<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(NodeOutput<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(NodeOutput<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(NodeOutput<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymNodeOutput
 static_assert(std::is_standard_layout_v<SymNodeOutput>);
 // static asserts for conversion of SymNodeOutput to BaseOutput
 static_assert(std::alignment_of_v<SymNodeOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymNodeOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymNodeOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymNodeOutput, id) == offsetof(BaseOutput, id));
@@ -45,30 +45,30 @@
 // static asserts for conversion of AsymNodeOutput to BaseOutput
 static_assert(std::alignment_of_v<AsymNodeOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(AsymNodeOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(AsymNodeOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(AsymNodeOutput, id) == offsetof(BaseOutput, id));
 static_assert(offsetof(AsymNodeOutput, energized) == offsetof(BaseOutput, energized));
 
-// static asserts for BranchOutput<true>
-static_assert(std::is_standard_layout_v<BranchOutput<true>>);
-// static asserts for conversion of BranchOutput<true> to BaseOutput
-static_assert(std::alignment_of_v<BranchOutput<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(BranchOutput<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(BranchOutput<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(BranchOutput<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(BranchOutput<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for BranchOutput<false>
-static_assert(std::is_standard_layout_v<BranchOutput<false>>);
-// static asserts for conversion of BranchOutput<false> to BaseOutput
-static_assert(std::alignment_of_v<BranchOutput<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(BranchOutput<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(BranchOutput<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(BranchOutput<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(BranchOutput<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for BranchOutput<symmetric_t>
+static_assert(std::is_standard_layout_v<BranchOutput<symmetric_t>>);
+// static asserts for conversion of BranchOutput<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<BranchOutput<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(BranchOutput<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(BranchOutput<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(BranchOutput<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(BranchOutput<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for BranchOutput<asymmetric_t>
+static_assert(std::is_standard_layout_v<BranchOutput<asymmetric_t>>);
+// static asserts for conversion of BranchOutput<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<BranchOutput<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(BranchOutput<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(BranchOutput<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(BranchOutput<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(BranchOutput<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymBranchOutput
 static_assert(std::is_standard_layout_v<SymBranchOutput>);
 // static asserts for conversion of SymBranchOutput to BaseOutput
 static_assert(std::alignment_of_v<SymBranchOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymBranchOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymBranchOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymBranchOutput, id) == offsetof(BaseOutput, id));
@@ -78,30 +78,30 @@
 // static asserts for conversion of AsymBranchOutput to BaseOutput
 static_assert(std::alignment_of_v<AsymBranchOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(AsymBranchOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(AsymBranchOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(AsymBranchOutput, id) == offsetof(BaseOutput, id));
 static_assert(offsetof(AsymBranchOutput, energized) == offsetof(BaseOutput, energized));
 
-// static asserts for Branch3Output<true>
-static_assert(std::is_standard_layout_v<Branch3Output<true>>);
-// static asserts for conversion of Branch3Output<true> to BaseOutput
-static_assert(std::alignment_of_v<Branch3Output<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(Branch3Output<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(Branch3Output<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(Branch3Output<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(Branch3Output<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for Branch3Output<false>
-static_assert(std::is_standard_layout_v<Branch3Output<false>>);
-// static asserts for conversion of Branch3Output<false> to BaseOutput
-static_assert(std::alignment_of_v<Branch3Output<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(Branch3Output<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(Branch3Output<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(Branch3Output<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(Branch3Output<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for Branch3Output<symmetric_t>
+static_assert(std::is_standard_layout_v<Branch3Output<symmetric_t>>);
+// static asserts for conversion of Branch3Output<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<Branch3Output<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(Branch3Output<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(Branch3Output<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(Branch3Output<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(Branch3Output<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for Branch3Output<asymmetric_t>
+static_assert(std::is_standard_layout_v<Branch3Output<asymmetric_t>>);
+// static asserts for conversion of Branch3Output<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<Branch3Output<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(Branch3Output<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(Branch3Output<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(Branch3Output<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(Branch3Output<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymBranch3Output
 static_assert(std::is_standard_layout_v<SymBranch3Output>);
 // static asserts for conversion of SymBranch3Output to BaseOutput
 static_assert(std::alignment_of_v<SymBranch3Output> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymBranch3Output::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymBranch3Output::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymBranch3Output, id) == offsetof(BaseOutput, id));
@@ -111,30 +111,30 @@
 // static asserts for conversion of AsymBranch3Output to BaseOutput
 static_assert(std::alignment_of_v<AsymBranch3Output> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(AsymBranch3Output::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(AsymBranch3Output::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(AsymBranch3Output, id) == offsetof(BaseOutput, id));
 static_assert(offsetof(AsymBranch3Output, energized) == offsetof(BaseOutput, energized));
 
-// static asserts for ApplianceOutput<true>
-static_assert(std::is_standard_layout_v<ApplianceOutput<true>>);
-// static asserts for conversion of ApplianceOutput<true> to BaseOutput
-static_assert(std::alignment_of_v<ApplianceOutput<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(ApplianceOutput<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(ApplianceOutput<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(ApplianceOutput<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(ApplianceOutput<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for ApplianceOutput<false>
-static_assert(std::is_standard_layout_v<ApplianceOutput<false>>);
-// static asserts for conversion of ApplianceOutput<false> to BaseOutput
-static_assert(std::alignment_of_v<ApplianceOutput<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(ApplianceOutput<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(ApplianceOutput<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(ApplianceOutput<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(ApplianceOutput<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for ApplianceOutput<symmetric_t>
+static_assert(std::is_standard_layout_v<ApplianceOutput<symmetric_t>>);
+// static asserts for conversion of ApplianceOutput<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<ApplianceOutput<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(ApplianceOutput<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(ApplianceOutput<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(ApplianceOutput<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(ApplianceOutput<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for ApplianceOutput<asymmetric_t>
+static_assert(std::is_standard_layout_v<ApplianceOutput<asymmetric_t>>);
+// static asserts for conversion of ApplianceOutput<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<ApplianceOutput<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(ApplianceOutput<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(ApplianceOutput<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(ApplianceOutput<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(ApplianceOutput<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymApplianceOutput
 static_assert(std::is_standard_layout_v<SymApplianceOutput>);
 // static asserts for conversion of SymApplianceOutput to BaseOutput
 static_assert(std::alignment_of_v<SymApplianceOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymApplianceOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymApplianceOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymApplianceOutput, id) == offsetof(BaseOutput, id));
@@ -144,30 +144,30 @@
 // static asserts for conversion of AsymApplianceOutput to BaseOutput
 static_assert(std::alignment_of_v<AsymApplianceOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(AsymApplianceOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(AsymApplianceOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(AsymApplianceOutput, id) == offsetof(BaseOutput, id));
 static_assert(offsetof(AsymApplianceOutput, energized) == offsetof(BaseOutput, energized));
 
-// static asserts for VoltageSensorOutput<true>
-static_assert(std::is_standard_layout_v<VoltageSensorOutput<true>>);
-// static asserts for conversion of VoltageSensorOutput<true> to BaseOutput
-static_assert(std::alignment_of_v<VoltageSensorOutput<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(VoltageSensorOutput<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorOutput<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(VoltageSensorOutput<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(VoltageSensorOutput<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for VoltageSensorOutput<false>
-static_assert(std::is_standard_layout_v<VoltageSensorOutput<false>>);
-// static asserts for conversion of VoltageSensorOutput<false> to BaseOutput
-static_assert(std::alignment_of_v<VoltageSensorOutput<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(VoltageSensorOutput<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(VoltageSensorOutput<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(VoltageSensorOutput<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(VoltageSensorOutput<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for VoltageSensorOutput<symmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorOutput<symmetric_t>>);
+// static asserts for conversion of VoltageSensorOutput<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<VoltageSensorOutput<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(VoltageSensorOutput<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorOutput<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(VoltageSensorOutput<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(VoltageSensorOutput<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for VoltageSensorOutput<asymmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorOutput<asymmetric_t>>);
+// static asserts for conversion of VoltageSensorOutput<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<VoltageSensorOutput<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(VoltageSensorOutput<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(VoltageSensorOutput<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(VoltageSensorOutput<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(VoltageSensorOutput<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymVoltageSensorOutput
 static_assert(std::is_standard_layout_v<SymVoltageSensorOutput>);
 // static asserts for conversion of SymVoltageSensorOutput to BaseOutput
 static_assert(std::alignment_of_v<SymVoltageSensorOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymVoltageSensorOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymVoltageSensorOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymVoltageSensorOutput, id) == offsetof(BaseOutput, id));
@@ -177,30 +177,30 @@
 // static asserts for conversion of AsymVoltageSensorOutput to BaseOutput
 static_assert(std::alignment_of_v<AsymVoltageSensorOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(AsymVoltageSensorOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(AsymVoltageSensorOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(AsymVoltageSensorOutput, id) == offsetof(BaseOutput, id));
 static_assert(offsetof(AsymVoltageSensorOutput, energized) == offsetof(BaseOutput, energized));
 
-// static asserts for PowerSensorOutput<true>
-static_assert(std::is_standard_layout_v<PowerSensorOutput<true>>);
-// static asserts for conversion of PowerSensorOutput<true> to BaseOutput
-static_assert(std::alignment_of_v<PowerSensorOutput<true>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(PowerSensorOutput<true>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(PowerSensorOutput<true>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(PowerSensorOutput<true>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(PowerSensorOutput<true>, energized) == offsetof(BaseOutput, energized));
-// static asserts for PowerSensorOutput<false>
-static_assert(std::is_standard_layout_v<PowerSensorOutput<false>>);
-// static asserts for conversion of PowerSensorOutput<false> to BaseOutput
-static_assert(std::alignment_of_v<PowerSensorOutput<false>> >= std::alignment_of_v<BaseOutput>);
-static_assert(std::same_as<decltype(PowerSensorOutput<false>::id), decltype(BaseOutput::id)>);
-static_assert(std::same_as<decltype(PowerSensorOutput<false>::energized), decltype(BaseOutput::energized)>);
-static_assert(offsetof(PowerSensorOutput<false>, id) == offsetof(BaseOutput, id));
-static_assert(offsetof(PowerSensorOutput<false>, energized) == offsetof(BaseOutput, energized));
+// static asserts for PowerSensorOutput<symmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorOutput<symmetric_t>>);
+// static asserts for conversion of PowerSensorOutput<symmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<PowerSensorOutput<symmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(PowerSensorOutput<symmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(PowerSensorOutput<symmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(PowerSensorOutput<symmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(PowerSensorOutput<symmetric_t>, energized) == offsetof(BaseOutput, energized));
+// static asserts for PowerSensorOutput<asymmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorOutput<asymmetric_t>>);
+// static asserts for conversion of PowerSensorOutput<asymmetric_t> to BaseOutput
+static_assert(std::alignment_of_v<PowerSensorOutput<asymmetric_t>> >= std::alignment_of_v<BaseOutput>);
+static_assert(std::same_as<decltype(PowerSensorOutput<asymmetric_t>::id), decltype(BaseOutput::id)>);
+static_assert(std::same_as<decltype(PowerSensorOutput<asymmetric_t>::energized), decltype(BaseOutput::energized)>);
+static_assert(offsetof(PowerSensorOutput<asymmetric_t>, id) == offsetof(BaseOutput, id));
+static_assert(offsetof(PowerSensorOutput<asymmetric_t>, energized) == offsetof(BaseOutput, energized));
 // static asserts for SymPowerSensorOutput
 static_assert(std::is_standard_layout_v<SymPowerSensorOutput>);
 // static asserts for conversion of SymPowerSensorOutput to BaseOutput
 static_assert(std::alignment_of_v<SymPowerSensorOutput> >= std::alignment_of_v<BaseOutput>);
 static_assert(std::same_as<decltype(SymPowerSensorOutput::id), decltype(BaseOutput::id)>);
 static_assert(std::same_as<decltype(SymPowerSensorOutput::energized), decltype(BaseOutput::energized)>);
 static_assert(offsetof(SymPowerSensorOutput, id) == offsetof(BaseOutput, id));
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/update.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/static_asserts/update.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -65,38 +65,38 @@
 static_assert(std::same_as<decltype(ThreeWindingTransformerUpdate::status_2), decltype(Branch3Update::status_2)>);
 static_assert(std::same_as<decltype(ThreeWindingTransformerUpdate::status_3), decltype(Branch3Update::status_3)>);
 static_assert(offsetof(ThreeWindingTransformerUpdate, id) == offsetof(Branch3Update, id));
 static_assert(offsetof(ThreeWindingTransformerUpdate, status_1) == offsetof(Branch3Update, status_1));
 static_assert(offsetof(ThreeWindingTransformerUpdate, status_2) == offsetof(Branch3Update, status_2));
 static_assert(offsetof(ThreeWindingTransformerUpdate, status_3) == offsetof(Branch3Update, status_3));
 
-// static asserts for LoadGenUpdate<true>
-static_assert(std::is_standard_layout_v<LoadGenUpdate<true>>);
-// static asserts for conversion of LoadGenUpdate<true> to BaseUpdate
-static_assert(std::alignment_of_v<LoadGenUpdate<true>> >= std::alignment_of_v<ApplianceUpdate>);
-static_assert(std::same_as<decltype(LoadGenUpdate<true>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(LoadGenUpdate<true>, id) == offsetof(BaseUpdate, id));
-// static asserts for conversion of LoadGenUpdate<true> to ApplianceUpdate
-static_assert(std::alignment_of_v<LoadGenUpdate<true>> >= std::alignment_of_v<ApplianceUpdate>);
-static_assert(std::same_as<decltype(LoadGenUpdate<true>::id), decltype(ApplianceUpdate::id)>);
-static_assert(std::same_as<decltype(LoadGenUpdate<true>::status), decltype(ApplianceUpdate::status)>);
-static_assert(offsetof(LoadGenUpdate<true>, id) == offsetof(ApplianceUpdate, id));
-static_assert(offsetof(LoadGenUpdate<true>, status) == offsetof(ApplianceUpdate, status));
-// static asserts for LoadGenUpdate<false>
-static_assert(std::is_standard_layout_v<LoadGenUpdate<false>>);
-// static asserts for conversion of LoadGenUpdate<false> to BaseUpdate
-static_assert(std::alignment_of_v<LoadGenUpdate<false>> >= std::alignment_of_v<ApplianceUpdate>);
-static_assert(std::same_as<decltype(LoadGenUpdate<false>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(LoadGenUpdate<false>, id) == offsetof(BaseUpdate, id));
-// static asserts for conversion of LoadGenUpdate<false> to ApplianceUpdate
-static_assert(std::alignment_of_v<LoadGenUpdate<false>> >= std::alignment_of_v<ApplianceUpdate>);
-static_assert(std::same_as<decltype(LoadGenUpdate<false>::id), decltype(ApplianceUpdate::id)>);
-static_assert(std::same_as<decltype(LoadGenUpdate<false>::status), decltype(ApplianceUpdate::status)>);
-static_assert(offsetof(LoadGenUpdate<false>, id) == offsetof(ApplianceUpdate, id));
-static_assert(offsetof(LoadGenUpdate<false>, status) == offsetof(ApplianceUpdate, status));
+// static asserts for LoadGenUpdate<symmetric_t>
+static_assert(std::is_standard_layout_v<LoadGenUpdate<symmetric_t>>);
+// static asserts for conversion of LoadGenUpdate<symmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<LoadGenUpdate<symmetric_t>> >= std::alignment_of_v<ApplianceUpdate>);
+static_assert(std::same_as<decltype(LoadGenUpdate<symmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(LoadGenUpdate<symmetric_t>, id) == offsetof(BaseUpdate, id));
+// static asserts for conversion of LoadGenUpdate<symmetric_t> to ApplianceUpdate
+static_assert(std::alignment_of_v<LoadGenUpdate<symmetric_t>> >= std::alignment_of_v<ApplianceUpdate>);
+static_assert(std::same_as<decltype(LoadGenUpdate<symmetric_t>::id), decltype(ApplianceUpdate::id)>);
+static_assert(std::same_as<decltype(LoadGenUpdate<symmetric_t>::status), decltype(ApplianceUpdate::status)>);
+static_assert(offsetof(LoadGenUpdate<symmetric_t>, id) == offsetof(ApplianceUpdate, id));
+static_assert(offsetof(LoadGenUpdate<symmetric_t>, status) == offsetof(ApplianceUpdate, status));
+// static asserts for LoadGenUpdate<asymmetric_t>
+static_assert(std::is_standard_layout_v<LoadGenUpdate<asymmetric_t>>);
+// static asserts for conversion of LoadGenUpdate<asymmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<LoadGenUpdate<asymmetric_t>> >= std::alignment_of_v<ApplianceUpdate>);
+static_assert(std::same_as<decltype(LoadGenUpdate<asymmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(LoadGenUpdate<asymmetric_t>, id) == offsetof(BaseUpdate, id));
+// static asserts for conversion of LoadGenUpdate<asymmetric_t> to ApplianceUpdate
+static_assert(std::alignment_of_v<LoadGenUpdate<asymmetric_t>> >= std::alignment_of_v<ApplianceUpdate>);
+static_assert(std::same_as<decltype(LoadGenUpdate<asymmetric_t>::id), decltype(ApplianceUpdate::id)>);
+static_assert(std::same_as<decltype(LoadGenUpdate<asymmetric_t>::status), decltype(ApplianceUpdate::status)>);
+static_assert(offsetof(LoadGenUpdate<asymmetric_t>, id) == offsetof(ApplianceUpdate, id));
+static_assert(offsetof(LoadGenUpdate<asymmetric_t>, status) == offsetof(ApplianceUpdate, status));
 // static asserts for SymLoadGenUpdate
 static_assert(std::is_standard_layout_v<SymLoadGenUpdate>);
 // static asserts for conversion of SymLoadGenUpdate to BaseUpdate
 static_assert(std::alignment_of_v<SymLoadGenUpdate> >= std::alignment_of_v<ApplianceUpdate>);
 static_assert(std::same_as<decltype(SymLoadGenUpdate::id), decltype(BaseUpdate::id)>);
 static_assert(offsetof(SymLoadGenUpdate, id) == offsetof(BaseUpdate, id));
 // static asserts for conversion of SymLoadGenUpdate to ApplianceUpdate
@@ -140,51 +140,51 @@
 // static asserts for conversion of ShuntUpdate to ApplianceUpdate
 static_assert(std::alignment_of_v<ShuntUpdate> >= std::alignment_of_v<ApplianceUpdate>);
 static_assert(std::same_as<decltype(ShuntUpdate::id), decltype(ApplianceUpdate::id)>);
 static_assert(std::same_as<decltype(ShuntUpdate::status), decltype(ApplianceUpdate::status)>);
 static_assert(offsetof(ShuntUpdate, id) == offsetof(ApplianceUpdate, id));
 static_assert(offsetof(ShuntUpdate, status) == offsetof(ApplianceUpdate, status));
 
-// static asserts for VoltageSensorUpdate<true>
-static_assert(std::is_standard_layout_v<VoltageSensorUpdate<true>>);
-// static asserts for conversion of VoltageSensorUpdate<true> to BaseUpdate
-static_assert(std::alignment_of_v<VoltageSensorUpdate<true>> >= std::alignment_of_v<BaseUpdate>);
-static_assert(std::same_as<decltype(VoltageSensorUpdate<true>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(VoltageSensorUpdate<true>, id) == offsetof(BaseUpdate, id));
-// static asserts for VoltageSensorUpdate<false>
-static_assert(std::is_standard_layout_v<VoltageSensorUpdate<false>>);
-// static asserts for conversion of VoltageSensorUpdate<false> to BaseUpdate
-static_assert(std::alignment_of_v<VoltageSensorUpdate<false>> >= std::alignment_of_v<BaseUpdate>);
-static_assert(std::same_as<decltype(VoltageSensorUpdate<false>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(VoltageSensorUpdate<false>, id) == offsetof(BaseUpdate, id));
+// static asserts for VoltageSensorUpdate<symmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorUpdate<symmetric_t>>);
+// static asserts for conversion of VoltageSensorUpdate<symmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<VoltageSensorUpdate<symmetric_t>> >= std::alignment_of_v<BaseUpdate>);
+static_assert(std::same_as<decltype(VoltageSensorUpdate<symmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(VoltageSensorUpdate<symmetric_t>, id) == offsetof(BaseUpdate, id));
+// static asserts for VoltageSensorUpdate<asymmetric_t>
+static_assert(std::is_standard_layout_v<VoltageSensorUpdate<asymmetric_t>>);
+// static asserts for conversion of VoltageSensorUpdate<asymmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<VoltageSensorUpdate<asymmetric_t>> >= std::alignment_of_v<BaseUpdate>);
+static_assert(std::same_as<decltype(VoltageSensorUpdate<asymmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(VoltageSensorUpdate<asymmetric_t>, id) == offsetof(BaseUpdate, id));
 // static asserts for SymVoltageSensorUpdate
 static_assert(std::is_standard_layout_v<SymVoltageSensorUpdate>);
 // static asserts for conversion of SymVoltageSensorUpdate to BaseUpdate
 static_assert(std::alignment_of_v<SymVoltageSensorUpdate> >= std::alignment_of_v<BaseUpdate>);
 static_assert(std::same_as<decltype(SymVoltageSensorUpdate::id), decltype(BaseUpdate::id)>);
 static_assert(offsetof(SymVoltageSensorUpdate, id) == offsetof(BaseUpdate, id));
 // static asserts for AsymVoltageSensorUpdate
 static_assert(std::is_standard_layout_v<AsymVoltageSensorUpdate>);
 // static asserts for conversion of AsymVoltageSensorUpdate to BaseUpdate
 static_assert(std::alignment_of_v<AsymVoltageSensorUpdate> >= std::alignment_of_v<BaseUpdate>);
 static_assert(std::same_as<decltype(AsymVoltageSensorUpdate::id), decltype(BaseUpdate::id)>);
 static_assert(offsetof(AsymVoltageSensorUpdate, id) == offsetof(BaseUpdate, id));
 
-// static asserts for PowerSensorUpdate<true>
-static_assert(std::is_standard_layout_v<PowerSensorUpdate<true>>);
-// static asserts for conversion of PowerSensorUpdate<true> to BaseUpdate
-static_assert(std::alignment_of_v<PowerSensorUpdate<true>> >= std::alignment_of_v<BaseUpdate>);
-static_assert(std::same_as<decltype(PowerSensorUpdate<true>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(PowerSensorUpdate<true>, id) == offsetof(BaseUpdate, id));
-// static asserts for PowerSensorUpdate<false>
-static_assert(std::is_standard_layout_v<PowerSensorUpdate<false>>);
-// static asserts for conversion of PowerSensorUpdate<false> to BaseUpdate
-static_assert(std::alignment_of_v<PowerSensorUpdate<false>> >= std::alignment_of_v<BaseUpdate>);
-static_assert(std::same_as<decltype(PowerSensorUpdate<false>::id), decltype(BaseUpdate::id)>);
-static_assert(offsetof(PowerSensorUpdate<false>, id) == offsetof(BaseUpdate, id));
+// static asserts for PowerSensorUpdate<symmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorUpdate<symmetric_t>>);
+// static asserts for conversion of PowerSensorUpdate<symmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<PowerSensorUpdate<symmetric_t>> >= std::alignment_of_v<BaseUpdate>);
+static_assert(std::same_as<decltype(PowerSensorUpdate<symmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(PowerSensorUpdate<symmetric_t>, id) == offsetof(BaseUpdate, id));
+// static asserts for PowerSensorUpdate<asymmetric_t>
+static_assert(std::is_standard_layout_v<PowerSensorUpdate<asymmetric_t>>);
+// static asserts for conversion of PowerSensorUpdate<asymmetric_t> to BaseUpdate
+static_assert(std::alignment_of_v<PowerSensorUpdate<asymmetric_t>> >= std::alignment_of_v<BaseUpdate>);
+static_assert(std::same_as<decltype(PowerSensorUpdate<asymmetric_t>::id), decltype(BaseUpdate::id)>);
+static_assert(offsetof(PowerSensorUpdate<asymmetric_t>, id) == offsetof(BaseUpdate, id));
 // static asserts for SymPowerSensorUpdate
 static_assert(std::is_standard_layout_v<SymPowerSensorUpdate>);
 // static asserts for conversion of SymPowerSensorUpdate to BaseUpdate
 static_assert(std::alignment_of_v<SymPowerSensorUpdate> >= std::alignment_of_v<BaseUpdate>);
 static_assert(std::same_as<decltype(SymPowerSensorUpdate::id), decltype(BaseUpdate::id)>);
 static_assert(offsetof(SymPowerSensorUpdate, id) == offsetof(BaseUpdate, id));
 // static asserts for AsymPowerSensorUpdate
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -76,32 +76,34 @@
     operator BaseUpdate const&() const { return reinterpret_cast<BaseUpdate const&>(*this); }
 
     // implicit conversions to Branch3Update
     operator Branch3Update&() { return reinterpret_cast<Branch3Update&>(*this); }
     operator Branch3Update const&() const { return reinterpret_cast<Branch3Update const&>(*this); }
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct LoadGenUpdate {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     IntS status;  // whether the appliance is connected
     RealValue<sym> p_specified;  // specified active/reactive power
     RealValue<sym> q_specified;  // specified active/reactive power
 
     // implicit conversions to BaseUpdate
     operator BaseUpdate&() { return reinterpret_cast<BaseUpdate&>(*this); }
     operator BaseUpdate const&() const { return reinterpret_cast<BaseUpdate const&>(*this); }
 
     // implicit conversions to ApplianceUpdate
     operator ApplianceUpdate&() { return reinterpret_cast<ApplianceUpdate&>(*this); }
     operator ApplianceUpdate const&() const { return reinterpret_cast<ApplianceUpdate const&>(*this); }
 };
 
-using SymLoadGenUpdate = LoadGenUpdate<true>;
-using AsymLoadGenUpdate = LoadGenUpdate<false>;
+using SymLoadGenUpdate = LoadGenUpdate<symmetric_t>;
+using AsymLoadGenUpdate = LoadGenUpdate<asymmetric_t>;
 
 struct SourceUpdate {
     ID id;  // ID of the object
     IntS status;  // whether the appliance is connected
     double u_ref;  // reference voltage
     double u_ref_angle;  // reference voltage
 
@@ -127,45 +129,49 @@
     operator BaseUpdate const&() const { return reinterpret_cast<BaseUpdate const&>(*this); }
 
     // implicit conversions to ApplianceUpdate
     operator ApplianceUpdate&() { return reinterpret_cast<ApplianceUpdate&>(*this); }
     operator ApplianceUpdate const&() const { return reinterpret_cast<ApplianceUpdate const&>(*this); }
 };
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct VoltageSensorUpdate {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     double u_sigma;  // sigma of error margin of voltage measurement
     RealValue<sym> u_measured;  // measured voltage magnitude and angle
     RealValue<sym> u_angle_measured;  // measured voltage magnitude and angle
 
     // implicit conversions to BaseUpdate
     operator BaseUpdate&() { return reinterpret_cast<BaseUpdate&>(*this); }
     operator BaseUpdate const&() const { return reinterpret_cast<BaseUpdate const&>(*this); }
 };
 
-using SymVoltageSensorUpdate = VoltageSensorUpdate<true>;
-using AsymVoltageSensorUpdate = VoltageSensorUpdate<false>;
+using SymVoltageSensorUpdate = VoltageSensorUpdate<symmetric_t>;
+using AsymVoltageSensorUpdate = VoltageSensorUpdate<asymmetric_t>;
 
-template <bool sym>
+template <symmetry_tag sym_type>
 struct PowerSensorUpdate {
+    using sym = sym_type;
+
     ID id;  // ID of the object
     double power_sigma;  // sigma of error margin of power measurement
     RealValue<sym> p_measured;  // measured active/reactive power
     RealValue<sym> q_measured;  // measured active/reactive power
     RealValue<sym> p_sigma;  // sigma of error margin of active/reactive power measurement
     RealValue<sym> q_sigma;  // sigma of error margin of active/reactive power measurement
 
     // implicit conversions to BaseUpdate
     operator BaseUpdate&() { return reinterpret_cast<BaseUpdate&>(*this); }
     operator BaseUpdate const&() const { return reinterpret_cast<BaseUpdate const&>(*this); }
 };
 
-using SymPowerSensorUpdate = PowerSensorUpdate<true>;
-using AsymPowerSensorUpdate = PowerSensorUpdate<false>;
+using SymPowerSensorUpdate = PowerSensorUpdate<symmetric_t>;
+using AsymPowerSensorUpdate = PowerSensorUpdate<asymmetric_t>;
 
 struct FaultUpdate {
     ID id;  // ID of the object
     IntS status;  // whether the fault is connected
     FaultType fault_type;  // type of the fault
     FaultPhase fault_phase;  // phase(s) of the fault
     ID fault_object;  // ID of the faulted object
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -16,95 +16,111 @@
     YBusElementType element_type{};
     Idx idx{}; // index of the component
 };
 
 // everything here always per unit
 
 // branch math calculation parameter and math output
-template <bool sym> struct BranchCalcParam {
+template <symmetry_tag sym_type> struct BranchCalcParam {
+    using sym = sym_type;
+
     std::array<ComplexTensor<sym>, 4> value;
     // getter
     ComplexTensor<sym>& yff() { return value[0]; }
     ComplexTensor<sym> const& yff() const { return value[0]; }
     ComplexTensor<sym>& yft() { return value[1]; }
     ComplexTensor<sym> const& yft() const { return value[1]; }
     ComplexTensor<sym>& ytf() { return value[2]; }
     ComplexTensor<sym> const& ytf() const { return value[2]; }
     ComplexTensor<sym>& ytt() { return value[3]; }
     ComplexTensor<sym> const& ytt() const { return value[3]; }
 };
 
-template <bool sym> struct BranchMathOutput {
+template <symmetry_tag sym_type> struct BranchMathOutput {
+    using sym = sym_type;
+
     ComplexValue<sym> s_f{};
     ComplexValue<sym> s_t{};
     ComplexValue<sym> i_f{};
     ComplexValue<sym> i_t{};
 };
 
-template <bool sym> struct BranchShortCircuitMathOutput {
+template <symmetry_tag sym_type> struct BranchShortCircuitMathOutput {
+    using sym = sym_type;
+
     ComplexValue<sym> i_f{};
     ComplexValue<sym> i_t{};
 };
 
 // fault math calculation parameters and math output
 struct FaultCalcParam {
     DoubleComplex y_fault{};
     FaultType fault_type{};
     FaultPhase fault_phase{};
 };
 
-template <bool sym> struct FaultShortCircuitMathOutput {
+template <symmetry_tag sym_type> struct FaultShortCircuitMathOutput {
+    using sym = sym_type;
+
     ComplexValue<sym> i_fault{};
 };
 
 // appliance math output, always injection direction
 // s > 0, energy appliance -> node
-template <bool sym> struct ApplianceMathOutput {
+template <symmetry_tag sym_type> struct ApplianceMathOutput {
+    using sym = sym_type;
+
     ComplexValue<sym> s{};
     ComplexValue<sym> i{};
 };
-template <bool sym> struct ApplianceShortCircuitMathOutput {
+template <symmetry_tag sym_type> struct ApplianceShortCircuitMathOutput {
+    using sym = sym_type;
+
     ComplexValue<sym> i{};
 };
 
 // Complex measured value of a sensor in p.u. with a uniform variance across all phases and axes of the complex plane
 // (circularly symmetric)
-template <bool sym> struct UniformComplexRandomVariable {
-    static constexpr bool symmetric{sym};
+template <symmetry_tag sym_type> struct UniformComplexRandomVariable {
+    using sym = sym_type;
+
+    static constexpr bool symmetric{is_symmetric_v<sym>};
 
     ComplexValue<sym> value{};
     double variance{}; // variance (sigma^2) of the error range, in p.u.
 };
 
 // voltage sensor calculation parameters for state estimation
 // The value is the complex voltage
 // If the imaginary part is NaN, it means the angle calculation is not correct
-template <bool sym> using VoltageSensorCalcParam = UniformComplexRandomVariable<sym>;
+template <symmetry_tag sym> using VoltageSensorCalcParam = UniformComplexRandomVariable<sym>;
 
 // power sensor calculation parameters for state estimation
 // The value is the complex power
 //   * for appliances, it is always in injection direction
 //   * for branches, the direction is node -> branch
-template <bool sym> struct PowerSensorCalcParam {
-    static constexpr bool symmetric{sym};
+template <symmetry_tag sym_type> struct PowerSensorCalcParam {
+    using sym = sym_type;
+
+    static constexpr bool symmetric{is_symmetric_v<sym>};
 
     ComplexValue<sym> value{};
     RealValue<sym> p_variance{}; // variance (sigma^2) of the error range of the active power, in p.u.
     RealValue<sym> q_variance{}; // variance (sigma^2) of the error range of the reactive power, in p.u.
 };
 
 template <typename T>
 concept sensor_calc_param_type =
-    std::same_as<T, VoltageSensorCalcParam<true>> || std::same_as<T, VoltageSensorCalcParam<false>> ||
-    std::same_as<T, PowerSensorCalcParam<true>> || std::same_as<T, PowerSensorCalcParam<false>>;
+    std::same_as<T, VoltageSensorCalcParam<symmetric_t>> || std::same_as<T, VoltageSensorCalcParam<asymmetric_t>> ||
+    std::same_as<T, PowerSensorCalcParam<symmetric_t>> || std::same_as<T, PowerSensorCalcParam<asymmetric_t>>;
 
-static_assert(sensor_calc_param_type<VoltageSensorCalcParam<true>>);
-static_assert(sensor_calc_param_type<VoltageSensorCalcParam<false>>);
-static_assert(sensor_calc_param_type<PowerSensorCalcParam<true>>);
-static_assert(sensor_calc_param_type<PowerSensorCalcParam<false>>);
+static_assert(sensor_calc_param_type<VoltageSensorCalcParam<symmetric_t>>);
+static_assert(sensor_calc_param_type<VoltageSensorCalcParam<asymmetric_t>>);
+static_assert(sensor_calc_param_type<PowerSensorCalcParam<symmetric_t>>);
+static_assert(sensor_calc_param_type<PowerSensorCalcParam<asymmetric_t>>);
 
 // from, to side
 // in case of indices for math model, -1 means the branch is not connected to that side
 using BranchIdx = std::array<Idx, 2>;
 // node 0, 1, 2 side
 // in case of indices for math model, -1 means the branch is not connected to that side
 using Branch3Idx = std::array<Idx, 3>;
@@ -147,31 +163,37 @@
     Idx n_branch_from_power_sensor() const { return power_sensors_per_branch_from.element_size(); }
 
     Idx n_branch_to_power_sensor() const { return power_sensors_per_branch_to.element_size(); }
 
     Idx n_bus_power_sensor() const { return power_sensors_per_bus.element_size(); }
 };
 
-template <bool sym> struct MathModelParam {
+template <symmetry_tag sym_type> struct MathModelParam {
+    using sym = sym_type;
+
     std::vector<BranchCalcParam<sym>> branch_param;
     ComplexTensorVector<sym> shunt_param;
     ComplexTensorVector<sym> source_param;
 };
 
 struct MathModelParamIncrement {
     std::vector<Idx> branch_param_to_change; // indices of changed branch_param
     std::vector<Idx> shunt_param_to_change;  // indices of changed shunt_param
 };
 
-template <bool sym> struct PowerFlowInput {
+template <symmetry_tag sym_type> struct PowerFlowInput {
+    using sym = sym_type;
+
     ComplexVector source;                // Complex u_ref of each source
     ComplexValueVector<sym> s_injection; // Specified injection power of each load_gen
 };
 
-template <bool sym> struct StateEstimationInput {
+template <symmetry_tag sym_type> struct StateEstimationInput {
+    using sym = sym_type;
+
     // connection status of shunt, load_gen, source
     // this is needed to determine if a measurement is relevant
     // if the shunt/load_gen/source is disconnected, all its measurements are discarded
     IntSVector shunt_status;
     IntSVector load_gen_status;
     IntSVector source_status;
     // measured value
@@ -188,101 +210,107 @@
     DenseGroupedIdxVector fault_buses;
     std::vector<FaultCalcParam> faults;
     ComplexVector source; // Complex u_ref of each source
 };
 
 template <typename T>
 concept symmetric_calculation_input_type =
-    std::same_as<T, PowerFlowInput<true>> || std::same_as<T, StateEstimationInput<true>>;
+    std::same_as<T, PowerFlowInput<symmetric_t>> || std::same_as<T, StateEstimationInput<symmetric_t>>;
 
-static_assert(symmetric_calculation_input_type<PowerFlowInput<true>>);
-static_assert(symmetric_calculation_input_type<StateEstimationInput<true>>);
-static_assert(!symmetric_calculation_input_type<PowerFlowInput<false>>);
-static_assert(!symmetric_calculation_input_type<StateEstimationInput<false>>);
+static_assert(symmetric_calculation_input_type<PowerFlowInput<symmetric_t>>);
+static_assert(symmetric_calculation_input_type<StateEstimationInput<symmetric_t>>);
+static_assert(!symmetric_calculation_input_type<PowerFlowInput<asymmetric_t>>);
+static_assert(!symmetric_calculation_input_type<StateEstimationInput<asymmetric_t>>);
 static_assert(!symmetric_calculation_input_type<ShortCircuitInput>);
 
 template <typename T>
 concept asymmetric_calculation_input_type =
-    std::same_as<T, PowerFlowInput<false>> || std::same_as<T, StateEstimationInput<false>> ||
+    std::same_as<T, PowerFlowInput<asymmetric_t>> || std::same_as<T, StateEstimationInput<asymmetric_t>> ||
     std::same_as<T, ShortCircuitInput>;
 
-static_assert(!asymmetric_calculation_input_type<PowerFlowInput<true>>);
-static_assert(!asymmetric_calculation_input_type<StateEstimationInput<true>>);
-static_assert(asymmetric_calculation_input_type<PowerFlowInput<false>>);
-static_assert(asymmetric_calculation_input_type<StateEstimationInput<false>>);
+static_assert(!asymmetric_calculation_input_type<PowerFlowInput<symmetric_t>>);
+static_assert(!asymmetric_calculation_input_type<StateEstimationInput<symmetric_t>>);
+static_assert(asymmetric_calculation_input_type<PowerFlowInput<asymmetric_t>>);
+static_assert(asymmetric_calculation_input_type<StateEstimationInput<asymmetric_t>>);
 static_assert(asymmetric_calculation_input_type<ShortCircuitInput>);
 
 template <typename T>
 concept calculation_input_type = symmetric_calculation_input_type<T> || asymmetric_calculation_input_type<T>;
 
-static_assert(calculation_input_type<PowerFlowInput<true>>);
-static_assert(calculation_input_type<StateEstimationInput<true>>);
-static_assert(calculation_input_type<PowerFlowInput<false>>);
-static_assert(calculation_input_type<StateEstimationInput<false>>);
+static_assert(calculation_input_type<PowerFlowInput<symmetric_t>>);
+static_assert(calculation_input_type<StateEstimationInput<symmetric_t>>);
+static_assert(calculation_input_type<PowerFlowInput<asymmetric_t>>);
+static_assert(calculation_input_type<StateEstimationInput<asymmetric_t>>);
 static_assert(calculation_input_type<ShortCircuitInput>);
 
-template <bool sym> struct MathOutput {
+template <symmetry_tag sym_type> struct MathOutput {
+    using sym = sym_type;
+
     std::vector<ComplexValue<sym>> u;
     std::vector<ComplexValue<sym>> bus_injection;
     std::vector<BranchMathOutput<sym>> branch;
     std::vector<ApplianceMathOutput<sym>> source;
     std::vector<ApplianceMathOutput<sym>> shunt;
     std::vector<ApplianceMathOutput<sym>> load_gen;
 };
 
-template <bool sym> struct ShortCircuitMathOutput {
+template <symmetry_tag sym_type> struct ShortCircuitMathOutput {
+    using sym = sym_type;
+
     std::vector<ComplexValue<sym>> u_bus;
     std::vector<FaultShortCircuitMathOutput<sym>> fault;
     std::vector<BranchShortCircuitMathOutput<sym>> branch;
     std::vector<ApplianceShortCircuitMathOutput<sym>> source;
     std::vector<ApplianceShortCircuitMathOutput<sym>> shunt;
 };
 
 template <typename T>
-concept symmetric_math_output_type = std::same_as<T, MathOutput<true>> || std::same_as<T, ShortCircuitMathOutput<true>>;
+concept symmetric_math_output_type =
+    std::same_as<T, MathOutput<symmetric_t>> || std::same_as<T, ShortCircuitMathOutput<symmetric_t>>;
 
-static_assert(symmetric_math_output_type<MathOutput<true>>);
-static_assert(!symmetric_math_output_type<MathOutput<false>>);
-static_assert(symmetric_math_output_type<ShortCircuitMathOutput<true>>);
-static_assert(!symmetric_math_output_type<ShortCircuitMathOutput<false>>);
+static_assert(symmetric_math_output_type<MathOutput<symmetric_t>>);
+static_assert(!symmetric_math_output_type<MathOutput<asymmetric_t>>);
+static_assert(symmetric_math_output_type<ShortCircuitMathOutput<symmetric_t>>);
+static_assert(!symmetric_math_output_type<ShortCircuitMathOutput<asymmetric_t>>);
 
 template <typename T>
 concept asymmetric_math_output_type =
-    std::same_as<T, MathOutput<false>> || std::same_as<T, ShortCircuitMathOutput<false>>;
+    std::same_as<T, MathOutput<asymmetric_t>> || std::same_as<T, ShortCircuitMathOutput<asymmetric_t>>;
 
-static_assert(!asymmetric_math_output_type<MathOutput<true>>);
-static_assert(asymmetric_math_output_type<MathOutput<false>>);
-static_assert(!asymmetric_math_output_type<ShortCircuitMathOutput<true>>);
-static_assert(asymmetric_math_output_type<ShortCircuitMathOutput<false>>);
+static_assert(!asymmetric_math_output_type<MathOutput<symmetric_t>>);
+static_assert(asymmetric_math_output_type<MathOutput<asymmetric_t>>);
+static_assert(!asymmetric_math_output_type<ShortCircuitMathOutput<symmetric_t>>);
+static_assert(asymmetric_math_output_type<ShortCircuitMathOutput<asymmetric_t>>);
 
 template <typename T>
-concept steady_state_math_output_type = std::same_as<T, MathOutput<true>> || std::same_as<T, MathOutput<false>>;
+concept steady_state_math_output_type =
+    std::same_as<T, MathOutput<symmetric_t>> || std::same_as<T, MathOutput<asymmetric_t>>;
 
-static_assert(steady_state_math_output_type<MathOutput<true>>);
-static_assert(steady_state_math_output_type<MathOutput<false>>);
-static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<true>>);
-static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<false>>);
+static_assert(steady_state_math_output_type<MathOutput<symmetric_t>>);
+static_assert(steady_state_math_output_type<MathOutput<asymmetric_t>>);
+static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<symmetric_t>>);
+static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<asymmetric_t>>);
 
 template <typename T>
 concept short_circuit_math_output_type =
-    std::same_as<T, ShortCircuitMathOutput<true>> || std::same_as<T, ShortCircuitMathOutput<false>>;
+    std::same_as<T, ShortCircuitMathOutput<symmetric_t>> || std::same_as<T, ShortCircuitMathOutput<asymmetric_t>>;
 
-static_assert(!short_circuit_math_output_type<MathOutput<true>>);
-static_assert(!short_circuit_math_output_type<MathOutput<false>>);
-static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<true>>);
-static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<false>>);
+static_assert(!short_circuit_math_output_type<MathOutput<symmetric_t>>);
+static_assert(!short_circuit_math_output_type<MathOutput<asymmetric_t>>);
+static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<symmetric_t>>);
+static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<asymmetric_t>>);
 
 template <typename T>
 concept math_output_type = (symmetric_math_output_type<T> || asymmetric_math_output_type<T>) &&
                            (steady_state_math_output_type<T> || short_circuit_math_output_type<T>);
 
-static_assert(math_output_type<MathOutput<true>>);
-static_assert(math_output_type<MathOutput<false>>);
-static_assert(math_output_type<ShortCircuitMathOutput<true>>);
-static_assert(math_output_type<ShortCircuitMathOutput<false>>);
+static_assert(math_output_type<MathOutput<symmetric_t>>);
+static_assert(math_output_type<MathOutput<asymmetric_t>>);
+static_assert(math_output_type<ShortCircuitMathOutput<symmetric_t>>);
+static_assert(math_output_type<ShortCircuitMathOutput<asymmetric_t>>);
 
 // component indices at physical model side
 // from, to node indices for branches
 // node1, node2, node3 indices for 3-way branches
 // node indices for source, load_gen, shunt
 struct ComponentTopology {
     Idx n_node{};
@@ -292,15 +320,15 @@
     IdxVector source_node_idx;
     IdxVector load_gen_node_idx;
     std::vector<LoadGenType> load_gen_type;
     IdxVector voltage_sensor_node_idx;
     IdxVector power_sensor_object_idx; // the index is relative to branch, source, shunt, or load_gen
     std::vector<MeasuredTerminalType> power_sensor_terminal_type;
 
-    inline Idx n_node_total() const { return n_node + (Idx)branch3_node_idx.size(); }
+    inline Idx n_node_total() const { return n_node + static_cast<Idx>(branch3_node_idx.size()); }
 };
 
 // connection property
 using BranchConnected = std::array<IntS, 2>;
 using Branch3Connected = std::array<IntS, 3>;
 
 // component connection property at model side
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/calculation_info.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/calculation_info.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/common.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/common.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,24 @@
 struct Idx2D {
     Idx group; // sequence number of outer module/groups
     Idx pos;   //  sequence number inside the group
 
     friend constexpr bool operator==(Idx2D x, Idx2D y) = default;
 };
 
+struct symmetric_t {};
+struct asymmetric_t {};
+
+template <typename T>
+concept symmetry_tag = std::derived_from<T, symmetric_t> || std::derived_from<T, asymmetric_t>;
+
+template <symmetry_tag T> constexpr bool is_symmetric_v = std::derived_from<T, symmetric_t>;
+
+template <symmetry_tag T> using other_symmetry_t = std::conditional_t<is_symmetric_v<T>, asymmetric_t, symmetric_t>;
+
 // math constant
 using namespace std::complex_literals;
 using DoubleComplex = std::complex<double>;
 
 using std::numbers::inv_sqrt3;
 using std::numbers::pi;
 using std::numbers::sqrt3;
@@ -47,16 +57,16 @@
 constexpr double nan = std::numeric_limits<double>::quiet_NaN();
 constexpr IntS na_IntS = std::numeric_limits<IntS>::min();
 constexpr ID na_IntID = std::numeric_limits<ID>::min();
 
 // power grid constant
 constexpr double base_power_3p = 1e6;
 constexpr double base_power_1p = base_power_3p / 3.0;
-template <bool sym> constexpr double u_scale = sym ? 1.0 : inv_sqrt3;
-template <bool sym> constexpr double base_power = sym ? base_power_3p : base_power_1p;
+template <symmetry_tag sym> constexpr double u_scale = is_symmetric_v<sym> ? 1.0 : inv_sqrt3;
+template <symmetry_tag sym> constexpr double base_power = is_symmetric_v<sym> ? base_power_3p : base_power_1p;
 // links are direct line between nodes with infinite element_admittance in theory
 // for numerical calculation, a big link element_admittance is assigned
 // 1e6 Siemens element_admittance in 10kV network
 constexpr double g_link = 1e6 / (base_power_3p / 10e3 / 10e3);
 constexpr DoubleComplex y_link{g_link, g_link};
 // default source short circuit power
 constexpr double default_source_sk = 1e10; // 10 GVA 10^10
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/enum.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/exception.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/grouped_index_vector.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/grouped_index_vector.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/three_phase_tensor.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/three_phase_tensor.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -84,67 +84,74 @@
         this->Eigen3DiagonalTensor<T>::operator=(other);
         return *this;
     }
 };
 } // namespace three_phase_tensor
 
 // three phase vector and tensor
-template <bool sym> using RealTensor = std::conditional_t<sym, double, three_phase_tensor::Tensor<double>>;
-template <bool sym>
-using ComplexTensor = std::conditional_t<sym, DoubleComplex, three_phase_tensor::Tensor<DoubleComplex>>;
-
-template <bool sym>
-using RealDiagonalTensor = std::conditional_t<sym, double, three_phase_tensor::DiagonalTensor<double>>;
-template <bool sym>
-using ComplexDiagonalTensor = std::conditional_t<sym, DoubleComplex, three_phase_tensor::DiagonalTensor<DoubleComplex>>;
-template <bool sym> using RealValue = std::conditional_t<sym, double, three_phase_tensor::Vector<double>>;
-template <bool sym>
-using ComplexValue = std::conditional_t<sym, DoubleComplex, three_phase_tensor::Vector<DoubleComplex>>;
+template <symmetry_tag sym>
+using RealTensor = std::conditional_t<is_symmetric_v<sym>, double, three_phase_tensor::Tensor<double>>;
+template <symmetry_tag sym>
+using ComplexTensor = std::conditional_t<is_symmetric_v<sym>, DoubleComplex, three_phase_tensor::Tensor<DoubleComplex>>;
+
+template <symmetry_tag sym>
+using RealDiagonalTensor = std::conditional_t<is_symmetric_v<sym>, double, three_phase_tensor::DiagonalTensor<double>>;
+template <symmetry_tag sym>
+using ComplexDiagonalTensor =
+    std::conditional_t<is_symmetric_v<sym>, DoubleComplex, three_phase_tensor::DiagonalTensor<DoubleComplex>>;
+template <symmetry_tag sym>
+using RealValue = std::conditional_t<is_symmetric_v<sym>, double, three_phase_tensor::Vector<double>>;
+template <symmetry_tag sym>
+using ComplexValue = std::conditional_t<is_symmetric_v<sym>, DoubleComplex, three_phase_tensor::Vector<DoubleComplex>>;
 
 // asserts to ensure alignment
-static_assert(sizeof(RealTensor<false>) == sizeof(double[9]));
-static_assert(alignof(RealTensor<false>) == alignof(double[9]));
-static_assert(std::is_standard_layout_v<RealTensor<false>>);
-static_assert(std::is_trivially_destructible_v<RealTensor<false>>);
-static_assert(sizeof(ComplexTensor<false>) == sizeof(double[18]));
-static_assert(alignof(ComplexTensor<false>) >= alignof(double[18]));
-static_assert(std::is_standard_layout_v<ComplexTensor<false>>);
-static_assert(std::is_trivially_destructible_v<ComplexTensor<false>>);
-static_assert(sizeof(RealValue<false>) == sizeof(double[3]));
-static_assert(alignof(RealValue<false>) == alignof(double[3]));
-static_assert(std::is_standard_layout_v<RealValue<false>>);
-static_assert(std::is_trivially_destructible_v<RealValue<false>>);
-static_assert(sizeof(ComplexValue<false>) == sizeof(double[6]));
-static_assert(alignof(ComplexValue<false>) >= alignof(double[6]));
-static_assert(std::is_standard_layout_v<ComplexValue<false>>);
-static_assert(std::is_trivially_destructible_v<ComplexValue<false>>);
+static_assert(sizeof(RealTensor<asymmetric_t>) == sizeof(double[9]));
+static_assert(alignof(RealTensor<asymmetric_t>) == alignof(double[9]));
+static_assert(std::is_standard_layout_v<RealTensor<asymmetric_t>>);
+static_assert(std::is_trivially_destructible_v<RealTensor<asymmetric_t>>);
+static_assert(sizeof(ComplexTensor<asymmetric_t>) == sizeof(double[18]));
+static_assert(alignof(ComplexTensor<asymmetric_t>) >= alignof(double[18]));
+static_assert(std::is_standard_layout_v<ComplexTensor<asymmetric_t>>);
+static_assert(std::is_trivially_destructible_v<ComplexTensor<asymmetric_t>>);
+static_assert(sizeof(RealValue<asymmetric_t>) == sizeof(double[3]));
+static_assert(alignof(RealValue<asymmetric_t>) == alignof(double[3]));
+static_assert(std::is_standard_layout_v<RealValue<asymmetric_t>>);
+static_assert(std::is_trivially_destructible_v<RealValue<asymmetric_t>>);
+static_assert(sizeof(ComplexValue<asymmetric_t>) == sizeof(double[6]));
+static_assert(alignof(ComplexValue<asymmetric_t>) >= alignof(double[6]));
+static_assert(std::is_standard_layout_v<ComplexValue<asymmetric_t>>);
+static_assert(std::is_trivially_destructible_v<ComplexValue<asymmetric_t>>);
 
 // enabler
 template <class T>
 concept column_vector = (T::ColsAtCompileTime == 1);
 template <class T>
 concept rk2_tensor = (static_cast<Idx>(T::RowsAtCompileTime) ==
                       static_cast<Idx>(T::ColsAtCompileTime)); // rank 2 tensor
 template <class T>
 concept column_vector_or_tensor = column_vector<T> || rk2_tensor<T>;
 
 // piecewise factory construction for complex vector
-template <bool sym = false> inline ComplexValue<sym> piecewise_complex_value(DoubleComplex const& x) {
-    if constexpr (sym) {
+template <symmetry_tag sym = asymmetric_t> inline ComplexValue<sym> piecewise_complex_value(DoubleComplex const& x) {
+    if constexpr (is_symmetric_v<sym>) {
         return x;
     } else {
-        return ComplexValue<false>{std::piecewise_construct, x};
+        return ComplexValue<asymmetric_t>{std::piecewise_construct, x};
     }
 }
 
-template <column_vector DerivedA>
-inline ComplexValue<false> piecewise_complex_value(Eigen::ArrayBase<DerivedA> const& val) {
-    return val;
+template <column_vector Derived, template <typename> typename T>
+    requires std::convertible_to<T<Derived>, Eigen::ArrayBase<Derived>>
+inline ComplexValue<asymmetric_t> piecewise_complex_value(T<Derived> const& x) {
+    return x;
 }
 
+// piecewise factory construction for complex vector
+inline ComplexValue<asymmetric_t> piecewise_complex_value(ComplexValue<asymmetric_t> const& x) { return x; }
+
 // abs
 inline double cabs(double x) { return std::abs(x); }
 inline double cabs(DoubleComplex const& x) { return std::sqrt(std::norm(x)); }
 inline double abs2(DoubleComplex const& x) { return std::norm(x); }
 template <column_vector_or_tensor DerivedA> inline auto cabs(Eigen::ArrayBase<DerivedA> const& m) {
     return sqrt(abs2(m));
 }
@@ -152,15 +159,15 @@
 // phase_shift(x) = e^{i arg(x)} = x / |x|
 inline DoubleComplex phase_shift(DoubleComplex const x) {
     if (auto const abs_x = cabs(x); abs_x > 0.0) {
         return x / abs_x;
     }
     return DoubleComplex{1.0};
 }
-inline ComplexValue<false> phase_shift(ComplexValue<false> const& m) {
+inline ComplexValue<asymmetric_t> phase_shift(ComplexValue<asymmetric_t> const& m) {
     return {phase_shift(m(0)), phase_shift(m(1)), phase_shift(m(2))};
 }
 
 // calculate kron product of two vector
 inline double vector_outer_product(double x, double y) { return x * y; }
 inline DoubleComplex vector_outer_product(DoubleComplex x, DoubleComplex y) { return x * y; }
 template <column_vector DerivedA, column_vector DerivedB>
@@ -218,16 +225,16 @@
 inline DoubleComplex sum_val(DoubleComplex const& z) { return z; }
 
 // function to mean vector
 template <column_vector DerivedA> inline auto mean_val(Eigen::ArrayBase<DerivedA> const& m) { return m.mean(); }
 inline DoubleComplex mean_val(DoubleComplex const& z) { return z; }
 inline double mean_val(double z) { return z; }
 
-template <bool sym, class T> inline auto process_mean_val(const T& m) {
-    if constexpr (sym) {
+template <symmetry_tag sym, class T> inline auto process_mean_val(const T& m) {
+    if constexpr (is_symmetric_v<sym>) {
         return mean_val(m);
     } else {
         return m;
     }
 }
 
 template <column_vector Derived> inline auto as_diag(Eigen::ArrayBase<Derived> const& x) {
@@ -250,30 +257,30 @@
 }
 
 inline auto pos_seq(DoubleComplex const& val) { return val; }
 
 // inverse of tensor
 inline auto inv(double val) { return 1.0 / val; }
 inline auto inv(DoubleComplex const& val) { return 1.0 / val; }
-inline auto inv(ComplexTensor<false> const& val) { return val.matrix().inverse().array(); }
+inline auto inv(ComplexTensor<asymmetric_t> const& val) { return val.matrix().inverse().array(); }
 
 // add_diag
 inline void add_diag(double& x, double y) { x += y; }
 inline void add_diag(DoubleComplex& x, DoubleComplex const& y) { x += y; }
 template <rk2_tensor DerivedA, column_vector DerivedB>
 inline void add_diag(Eigen::ArrayBase<DerivedA>& x, Eigen::ArrayBase<DerivedB> const& y) {
     x.matrix().diagonal() += y.matrix();
 }
 template <rk2_tensor DerivedA, column_vector DerivedB>
 inline void add_diag(Eigen::ArrayBase<DerivedA>&& x, Eigen::ArrayBase<DerivedB> const& y) {
     x.matrix().diagonal() += y.matrix();
 }
 
 // zero tensor
-template <bool sym> inline const ComplexTensor<sym> zero_tensor = ComplexTensor<sym>{0.0};
+template <symmetry_tag sym> inline const ComplexTensor<sym> zero_tensor = ComplexTensor<sym>{0.0};
 
 // inverse symmetric param
 inline std::pair<DoubleComplex, DoubleComplex> inv_sym_param(DoubleComplex const& s, DoubleComplex const& m) {
     DoubleComplex const det_1 = 1.0 / (s * s + s * m - 2.0 * m * m);
     return {(s + m) * det_1, -m * det_1};
 }
 
@@ -301,37 +308,39 @@
 }
 template <class Derived> inline auto is_normal(Eigen::ArrayBase<Derived> const& value) {
     return is_normal(value(0)) && is_normal(value(1)) && is_normal(value(2));
 }
 
 // isinf
 inline auto is_inf(std::floating_point auto value) { return std::isinf(value); }
-inline auto is_inf(RealValue<false> const& value) { return is_inf(value(0)) || is_inf(value(1)) || is_inf(value(2)); }
+inline auto is_inf(RealValue<asymmetric_t> const& value) {
+    return is_inf(value(0)) || is_inf(value(1)) || is_inf(value(2));
+}
 
 // any_zero
 inline auto any_zero(std::floating_point auto value) { return value == 0.0; }
-inline auto any_zero(RealValue<false> const& value) { return (value == RealValue<false>{0.0}).any(); }
+inline auto any_zero(RealValue<asymmetric_t> const& value) { return (value == RealValue<asymmetric_t>{0.0}).any(); }
 
 // all_zero
 inline auto all_zero(std::floating_point auto value) { return value == 0.0; }
-inline auto all_zero(RealValue<false> const& value) { return (value == RealValue<false>{0.0}).all(); }
+inline auto all_zero(RealValue<asymmetric_t> const& value) { return (value == RealValue<asymmetric_t>{0.0}).all(); }
 
 // update real values
 //
 // RealValue is only updated when the update value is not nan
 //
 // symmetric:  update 1.0 with nan -> 1.0
 //             update 1.0 with 2.0 -> 2.0
 //
 // asymmetric: update [1.0, nan, nan] with [nan, nan, 2.0] -> [1.0, nan, 2.0]
 //
 // The function assumes that the current value is normalized and new value should be normalized with scalar
-template <bool sym, class Proxy>
+template <symmetry_tag sym, class Proxy>
 inline void update_real_value(RealValue<sym> const& new_value, Proxy&& current_value, double scalar) {
-    if constexpr (sym) {
+    if constexpr (is_symmetric_v<sym>) {
         if (!is_nan(new_value)) {
             current_value = scalar * new_value;
         }
     } else {
         for (size_t i = 0; i != 3; ++i) {
             if (!is_nan(new_value(i))) {
                 current_value(i) = scalar * new_value(i);
@@ -344,40 +353,40 @@
 //
 // contrary to update_real_value, this function retains nan in the target
 template <typename T> inline void set_if_not_nan(T& target, T const& value) {
     if (!is_nan(target)) {
         target = value;
     }
 };
-inline void set_if_not_nan(RealValue<false>& target, RealValue<false> const& value) {
+inline void set_if_not_nan(RealValue<asymmetric_t>& target, RealValue<asymmetric_t> const& value) {
     for (Idx i = 0; i != 3; ++i) {
         set_if_not_nan(target(i), value(i));
     }
 };
 
 // symmetric component matrix
-inline ComplexTensor<false> get_sym_matrix() {
-    ComplexTensor<false> m;
+inline ComplexTensor<asymmetric_t> get_sym_matrix() {
+    ComplexTensor<asymmetric_t> m;
     m << 1.0, 1.0, 1.0, 1.0, a2, a, 1.0, a, a2;
     return m;
 }
-inline ComplexTensor<false> get_sym_matrix_inv() {
-    ComplexTensor<false> m;
+inline ComplexTensor<asymmetric_t> get_sym_matrix_inv() {
+    ComplexTensor<asymmetric_t> m;
     m << 1.0, 1.0, 1.0, 1.0, a, a2, 1.0, a2, a;
     m = m / 3.0;
     return m;
 }
 
 // conjugate (hermitian) transpose
 inline DoubleComplex hermitian_transpose(DoubleComplex const& z) { return conj(z); }
 inline double hermitian_transpose(double x) { return x; }
 template <rk2_tensor Derived> inline auto hermitian_transpose(Eigen::ArrayBase<Derived> const& x) {
     return x.matrix().adjoint().array();
 }
 
 // vector of values
-template <bool sym> using RealValueVector = std::vector<RealValue<sym>>;
-template <bool sym> using ComplexValueVector = std::vector<ComplexValue<sym>>;
-template <bool sym> using RealTensorVector = std::vector<RealTensor<sym>>;
-template <bool sym> using ComplexTensorVector = std::vector<ComplexTensor<sym>>;
+template <symmetry_tag sym> using RealValueVector = std::vector<RealValue<sym>>;
+template <symmetry_tag sym> using ComplexValueVector = std::vector<ComplexValue<sym>>;
+template <symmetry_tag sym> using RealTensorVector = std::vector<RealTensor<sym>>;
+template <symmetry_tag sym> using ComplexTensorVector = std::vector<ComplexTensor<sym>>;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/timer.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/common/typing.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/common/typing.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 namespace power_grid_model {
 
 class Appliance : public Base {
   public:
     using InputType = ApplianceInput;
     using UpdateType = ApplianceUpdate;
-    template <bool sym> using OutputType = ApplianceOutput<sym>;
+    template <symmetry_tag sym> using OutputType = ApplianceOutput<sym>;
     using ShortCircuitOutputType = ApplianceShortCircuitOutput;
     static constexpr char const* name = "appliance";
 
     Appliance(ApplianceInput const& appliance_input, double u)
         : Base{appliance_input},
           node_{appliance_input.node},
           status_{appliance_input.status != 0},
@@ -44,34 +44,35 @@
             return false;
         }
         status_ = static_cast<bool>(new_status);
         return true;
     }
 
     // empty output
-    template <bool sym> ApplianceOutput<sym> get_null_output() const {
+    template <symmetry_tag sym> ApplianceOutput<sym> get_null_output() const {
         ApplianceOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
     ApplianceShortCircuitOutput get_null_sc_output() const {
         ApplianceShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
-    template <bool sym> ApplianceOutput<sym> get_output(ApplianceMathOutput<sym> const& appliance_math_output) const {
+    template <symmetry_tag sym>
+    ApplianceOutput<sym> get_output(ApplianceMathOutput<sym> const& appliance_math_output) const {
         ApplianceOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(energized(true));
         output.p = base_power<sym> * real(appliance_math_output.s) * injection_direction();
         output.q = base_power<sym> * imag(appliance_math_output.s) * injection_direction();
         output.s = base_power<sym> * cabs(appliance_math_output.s);
         output.i = base_i_ * cabs(appliance_math_output.i);
         // pf
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             if (output.s < numerical_tolerance) {
                 output.pf = 0.0;
             } else {
                 output.pf = output.p / output.s;
             }
         } else {
             for (size_t j = 0; j != 3; ++j) {
@@ -80,43 +81,43 @@
                 } else {
                     output.pf(j) = output.p(j) / output.s(j);
                 }
             }
         }
         return output;
     }
-    ApplianceShortCircuitOutput get_sc_output(ComplexValue<false> const& i) const {
+    ApplianceShortCircuitOutput get_sc_output(ComplexValue<asymmetric_t> const& i) const {
         ApplianceShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(energized(true));
         output.i = base_i_ * cabs(i);
         output.i_angle = arg(i * injection_direction());
         return output;
     }
-    ApplianceShortCircuitOutput get_sc_output(ComplexValue<true> const& i) const {
-        ComplexValue<false> const iabc{i};
+    ApplianceShortCircuitOutput get_sc_output(ComplexValue<symmetric_t> const& i) const {
+        ComplexValue<asymmetric_t> const iabc{i};
         return get_sc_output(iabc);
     }
-    template <bool sym> ApplianceOutput<sym> get_output(ComplexValue<sym> const& u) const {
-        if constexpr (sym) {
-            return get_output<true>(sym_u2si(u));
+    template <symmetry_tag sym> ApplianceOutput<sym> get_output(ComplexValue<sym> const& u) const {
+        if constexpr (is_symmetric_v<sym>) {
+            return get_output<symmetric_t>(sym_u2si(u));
         } else {
-            return get_output<false>(asym_u2si(u));
+            return get_output<asymmetric_t>(asym_u2si(u));
         }
     }
-    template <bool sym>
+    template <symmetry_tag sym>
     ApplianceShortCircuitOutput get_sc_output(ApplianceShortCircuitMathOutput<sym> const& appliance_math_output) const {
         return get_sc_output(appliance_math_output.i);
     }
 
   private:
     ID node_;
     bool status_;
     double base_i_;
 
     // pure virtual functions for translate from u to s/i
-    virtual ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const = 0;
-    virtual ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const = 0;
+    virtual ApplianceMathOutput<symmetric_t> sym_u2si(ComplexValue<symmetric_t> const& u) const = 0;
+    virtual ApplianceMathOutput<asymmetric_t> asym_u2si(ComplexValue<asymmetric_t> const& u) const = 0;
 
     virtual double injection_direction() const = 0;
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 namespace power_grid_model {
 
 class Base {
   public:
     using InputType = BaseInput;
     using UpdateType = BaseUpdate;
-    template <bool sym> using OutputType = BaseOutput;
+    template <symmetry_tag sym> using OutputType = BaseOutput;
     static constexpr char const* name = "base";
     virtual ComponentType math_model_type() const = 0;
 
     explicit Base(BaseInput const& base_input) : id_{base_input.id} {}
     virtual ~Base() = default;
     constexpr ID id() const noexcept { return id_; }
     constexpr BaseOutput base_output(bool is_energized) const {
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 namespace power_grid_model {
 
 class Branch : public Base {
   public:
     using InputType = BranchInput;
     using UpdateType = BranchUpdate;
-    template <bool sym> using OutputType = BranchOutput<sym>;
+    template <symmetry_tag sym> using OutputType = BranchOutput<sym>;
     using ShortCircuitOutputType = BranchShortCircuitOutput;
     static constexpr char const* name = "branch";
     ComponentType math_model_type() const final { return ComponentType::branch; }
 
     explicit Branch(BranchInput const& branch_input)
         : Base{branch_input},
           from_node_{branch_input.from_node},
@@ -38,19 +38,19 @@
 
     // getter
     ID from_node() const { return from_node_; }
     ID to_node() const { return to_node_; }
     bool from_status() const { return from_status_; }
     bool to_status() const { return to_status_; }
     bool branch_status() const { return from_status_ && to_status_; }
-    template <bool sym> BranchCalcParam<sym> calc_param(bool is_connected_to_source = true) const {
+    template <symmetry_tag sym> BranchCalcParam<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return BranchCalcParam<sym>{};
         }
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return sym_calc_param();
         } else {
             return asym_calc_param();
         }
     }
 
     // virtual getter
@@ -59,27 +59,28 @@
     }
     virtual double base_i_from() const = 0;
     virtual double base_i_to() const = 0;
     virtual double loading(double max_s, double max_i) const = 0;
     virtual double phase_shift() const = 0; // shift theta_from - theta_to
     virtual bool is_param_mutable() const = 0;
 
-    template <bool sym> BranchOutput<sym> get_output(ComplexValue<sym> const& u_f, ComplexValue<sym> const& u_t) const {
+    template <symmetry_tag sym>
+    BranchOutput<sym> get_output(ComplexValue<sym> const& u_f, ComplexValue<sym> const& u_t) const {
         // calculate flow
         BranchCalcParam<sym> const param = calc_param<sym>();
         BranchMathOutput<sym> branch_math_output{};
         branch_math_output.i_f = dot(param.yff(), u_f) + dot(param.yft(), u_t);
         branch_math_output.i_t = dot(param.ytf(), u_f) + dot(param.ytt(), u_t);
         branch_math_output.s_f = u_f * conj(branch_math_output.i_f);
         branch_math_output.s_t = u_t * conj(branch_math_output.i_t);
         // calculate result
         return get_output<sym>(branch_math_output);
     }
 
-    template <bool sym> BranchOutput<sym> get_output(BranchMathOutput<sym> const& branch_math_output) const {
+    template <symmetry_tag sym> BranchOutput<sym> get_output(BranchMathOutput<sym> const& branch_math_output) const {
         // result object
         BranchOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
         output.p_from = base_power<sym> * real(branch_math_output.s_f);
         output.q_from = base_power<sym> * imag(branch_math_output.s_f);
         output.i_from = base_i_from() * cabs(branch_math_output.i_f);
@@ -90,38 +91,41 @@
         output.s_to = base_power<sym> * cabs(branch_math_output.s_t);
         double const max_s = std::max(sum_val(output.s_from), sum_val(output.s_to));
         double const max_i = std::max(max_val(output.i_from), max_val(output.i_to));
         output.loading = loading(max_s, max_i);
         return output;
     }
 
-    BranchShortCircuitOutput get_sc_output(ComplexValue<true> const& i_f, ComplexValue<true> const& i_t) const {
-        return get_sc_output(BranchShortCircuitMathOutput<true>{.i_f = i_f, .i_t = i_t});
+    BranchShortCircuitOutput get_sc_output(ComplexValue<symmetric_t> const& i_f,
+                                           ComplexValue<symmetric_t> const& i_t) const {
+        return get_sc_output(BranchShortCircuitMathOutput<symmetric_t>{.i_f = i_f, .i_t = i_t});
     }
-    BranchShortCircuitOutput get_sc_output(ComplexValue<false> const& i_f, ComplexValue<false> const& i_t) const {
-        return get_sc_output(BranchShortCircuitMathOutput<false>{.i_f = i_f, .i_t = i_t});
+    BranchShortCircuitOutput get_sc_output(ComplexValue<asymmetric_t> const& i_f,
+                                           ComplexValue<asymmetric_t> const& i_t) const {
+        return get_sc_output(BranchShortCircuitMathOutput<asymmetric_t>{.i_f = i_f, .i_t = i_t});
     }
 
-    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<false> const& branch_math_output) const {
+    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<asymmetric_t> const& branch_math_output) const {
         BranchShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
         output.i_from = base_i_from() * cabs(branch_math_output.i_f);
         output.i_to = base_i_to() * cabs(branch_math_output.i_t);
         output.i_from_angle = arg(branch_math_output.i_f);
         output.i_to_angle = arg(branch_math_output.i_t);
         return output;
     }
 
-    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<true> const& branch_math_output) const {
-        return get_sc_output(BranchShortCircuitMathOutput<false>{.i_f = ComplexValue<false>{branch_math_output.i_f},
-                                                                 .i_t = ComplexValue<false>{branch_math_output.i_t}});
+    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<symmetric_t> const& branch_math_output) const {
+        return get_sc_output(
+            BranchShortCircuitMathOutput<asymmetric_t>{.i_f = ComplexValue<asymmetric_t>{branch_math_output.i_f},
+                                                       .i_t = ComplexValue<asymmetric_t>{branch_math_output.i_t}});
     }
 
-    template <bool sym> BranchOutput<sym> get_null_output() const {
+    template <symmetry_tag sym> BranchOutput<sym> get_null_output() const {
         BranchOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     BranchShortCircuitOutput get_null_sc_output() const {
         BranchShortCircuitOutput output{};
@@ -160,20 +164,20 @@
         set_if_not_nan(update_data.to_status, static_cast<IntS>(to_status_));
 
         return update_data;
     }
 
   protected:
     // calculate branch param based on symmetric component
-    BranchCalcParam<true>
+    BranchCalcParam<symmetric_t>
     calc_param_y_sym(DoubleComplex const& y_series, // y_series must be converted to the "to" side of the branch
                      DoubleComplex const& y_shunt,  // y_shunt must be converted to the "to" side of the branch
                      DoubleComplex const& tap_ratio) const {
         double const tap = cabs(tap_ratio);
-        BranchCalcParam<true> param{};
+        BranchCalcParam<symmetric_t> param{};
         // not both connected
         if (!(from_status_ && to_status_)) {
             // single connected
             if (from_status_ || to_status_) {
                 DoubleComplex branch_shunt;
                 // shunt value
                 if (cabs(y_shunt) < numerical_tolerance) {
@@ -193,36 +197,36 @@
             param.yff() = (1.0 / tap / tap) * param.ytt();
             param.yft() = (-1.0 / conj(tap_ratio)) * y_series;
             param.ytf() = (-1.0 / tap_ratio) * y_series;
         }
         return param;
     }
     // calculate branch param for asymmetric
-    BranchCalcParam<false> calc_param_y_asym(DoubleComplex const& y1_series, DoubleComplex const& y1_shunt,
-                                             DoubleComplex const& y0_series, DoubleComplex const& y0_shunt,
-                                             DoubleComplex const& tap_ratio) const {
-        BranchCalcParam<true> const param1 = calc_param_y_sym(y1_series, y1_shunt, tap_ratio);
-        BranchCalcParam<true> const param0 = calc_param_y_sym(y0_series, y0_shunt, tap_ratio);
+    BranchCalcParam<asymmetric_t> calc_param_y_asym(DoubleComplex const& y1_series, DoubleComplex const& y1_shunt,
+                                                    DoubleComplex const& y0_series, DoubleComplex const& y0_shunt,
+                                                    DoubleComplex const& tap_ratio) const {
+        BranchCalcParam<symmetric_t> const param1 = calc_param_y_sym(y1_series, y1_shunt, tap_ratio);
+        BranchCalcParam<symmetric_t> const param0 = calc_param_y_sym(y0_series, y0_shunt, tap_ratio);
         // abc matrix
         // 1/3 *
         // [[2y1+y0, y0-y1, y0-y1],
         //  [y0-y1, 2y1+y0, y0-y1],
         //  [y0-y1, y0-y1, 2y1+y0]]
-        BranchCalcParam<false> param{};
+        BranchCalcParam<asymmetric_t> param{};
         for (size_t i = 0; i < 4; ++i) {
-            param.value[i] = ComplexTensor<false>{(2.0 * param1.value[i] + param0.value[i]) / 3.0,
-                                                  (param0.value[i] - param1.value[i]) / 3.0};
+            param.value[i] = ComplexTensor<asymmetric_t>{(2.0 * param1.value[i] + param0.value[i]) / 3.0,
+                                                         (param0.value[i] - param1.value[i]) / 3.0};
         }
         return param;
     }
 
   private:
     ID from_node_;
     ID to_node_;
     bool from_status_;
     bool to_status_;
 
-    virtual BranchCalcParam<true> sym_calc_param() const = 0;
-    virtual BranchCalcParam<false> asym_calc_param() const = 0;
+    virtual BranchCalcParam<symmetric_t> sym_calc_param() const = 0;
+    virtual BranchCalcParam<asymmetric_t> asym_calc_param() const = 0;
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 namespace power_grid_model {
 
 class Branch3 : public Base {
   public:
     using InputType = Branch3Input;
     using UpdateType = Branch3Update;
-    template <bool sym> using OutputType = Branch3Output<sym>;
+    template <symmetry_tag sym> using OutputType = Branch3Output<sym>;
     using ShortCircuitOutputType = Branch3ShortCircuitOutput;
     static constexpr char const* name = "branch3";
     ComponentType math_model_type() const final { return ComponentType::branch3; }
 
     explicit Branch3(Branch3Input const& branch3_input)
         : Base{branch3_input},
           node_1_{branch3_input.node_1},
@@ -53,26 +53,27 @@
     }
     virtual double base_i_1() const = 0;
     virtual double base_i_2() const = 0;
     virtual double base_i_3() const = 0;
     virtual double loading(double s_1, double s_2, double s_3) const = 0;
     virtual std::array<double, 3> phase_shift() const = 0;
 
-    template <bool sym> std::array<BranchCalcParam<sym>, 3> calc_param(bool is_connected_to_source = true) const {
+    template <symmetry_tag sym>
+    std::array<BranchCalcParam<sym>, 3> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return std::array<BranchCalcParam<sym>, 3>{};
         }
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return sym_calc_param();
         } else {
             return asym_calc_param();
         }
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     Branch3Output<sym> get_output(BranchMathOutput<sym> const& branch_math_output1,
                                   BranchMathOutput<sym> const& branch_math_output2,
                                   BranchMathOutput<sym> const& branch_math_output3) const {
         // result object
         Branch3Output<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
@@ -92,43 +93,44 @@
         output.s_3 = base_power<sym> * cabs(branch_math_output3.s_f);
 
         output.loading = loading(sum_val(output.s_1), sum_val(output.s_2), sum_val(output.s_3));
 
         return output;
     }
 
-    Branch3ShortCircuitOutput get_sc_output(ComplexValue<false> const& i_1, ComplexValue<false> const& i_2,
-                                            ComplexValue<false> const& i_3) const {
+    Branch3ShortCircuitOutput get_sc_output(ComplexValue<asymmetric_t> const& i_1,
+                                            ComplexValue<asymmetric_t> const& i_2,
+                                            ComplexValue<asymmetric_t> const& i_3) const {
         // result object
         Branch3ShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
         output.i_1 = base_i_1() * cabs(i_1);
         output.i_2 = base_i_2() * cabs(i_2);
         output.i_3 = base_i_3() * cabs(i_3);
         output.i_1_angle = arg(i_1);
         output.i_2_angle = arg(i_2);
         output.i_3_angle = arg(i_3);
         return output;
     }
-    Branch3ShortCircuitOutput get_sc_output(ComplexValue<true> const& i_1, ComplexValue<true> const& i_2,
-                                            ComplexValue<true> const& i_3) const {
-        ComplexValue<false> const iabc_1{i_1};
-        ComplexValue<false> const iabc_2{i_2};
-        ComplexValue<false> const iabc_3{i_3};
+    Branch3ShortCircuitOutput get_sc_output(ComplexValue<symmetric_t> const& i_1, ComplexValue<symmetric_t> const& i_2,
+                                            ComplexValue<symmetric_t> const& i_3) const {
+        ComplexValue<asymmetric_t> const iabc_1{i_1};
+        ComplexValue<asymmetric_t> const iabc_2{i_2};
+        ComplexValue<asymmetric_t> const iabc_3{i_3};
         return get_sc_output(iabc_1, iabc_2, iabc_3);
     }
-    template <bool sym>
+    template <symmetry_tag sym>
     Branch3ShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<sym> const& branch_math_output1,
                                             BranchShortCircuitMathOutput<sym> const& branch_math_output2,
                                             BranchShortCircuitMathOutput<sym> const& branch_math_output3) const {
         return get_sc_output(branch_math_output1.i_f, branch_math_output2.i_f, branch_math_output3.i_f);
     }
 
-    template <bool sym> Branch3Output<sym> get_null_output() const {
+    template <symmetry_tag sym> Branch3Output<sym> get_null_output() const {
         Branch3Output<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     Branch3ShortCircuitOutput get_null_sc_output() const {
         Branch3ShortCircuitOutput output{};
@@ -179,12 +181,12 @@
     ID node_1_;
     ID node_2_;
     ID node_3_;
     bool status_1_;
     bool status_2_;
     bool status_3_;
 
-    virtual std::array<BranchCalcParam<true>, 3> sym_calc_param() const = 0;
-    virtual std::array<BranchCalcParam<false>, 3> asym_calc_param() const = 0;
+    virtual std::array<BranchCalcParam<symmetric_t>, 3> sym_calc_param() const = 0;
+    virtual std::array<BranchCalcParam<asymmetric_t>, 3> asym_calc_param() const = 0;
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 namespace power_grid_model {
 
 class Fault final : public Base {
   public:
     using InputType = FaultInput;
     using UpdateType = FaultUpdate;
-    template <bool sym> using OutputType = FaultOutput;
+    template <symmetry_tag sym> using OutputType = FaultOutput;
     using ShortCircuitOutputType = FaultShortCircuitOutput;
     static constexpr char const* name = "fault";
     ComponentType math_model_type() const override { return ComponentType::fault; }
 
     explicit Fault(FaultInput const& fault_input)
         : Base{fault_input},
           status_{static_cast<bool>(fault_input.status)},
@@ -59,32 +59,32 @@
     FaultOutput get_null_output() const { return get_null_output_impl<FaultOutput>(); }
     FaultOutput get_output() const {
         // During power flow and state estimation the fault object will have an empty output
         return get_null_output();
     }
 
     FaultShortCircuitOutput get_null_sc_output() const { return get_null_output_impl<FaultShortCircuitOutput>(); }
-    FaultShortCircuitOutput get_sc_output(ComplexValue<false> i_f, double const u_rated) const {
+    FaultShortCircuitOutput get_sc_output(ComplexValue<asymmetric_t> i_f, double const u_rated) const {
         // translate pu to A
         double const base_i = base_power_3p / u_rated / sqrt3;
         i_f = i_f * base_i;
         // result object
         FaultShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         output.i_f = cabs(i_f);
         output.i_f_angle = arg(i_f);
         return output;
     }
 
-    FaultShortCircuitOutput get_sc_output(ComplexValue<true> i_f, double const u_rated) const {
-        ComplexValue<false> const iabc_f{i_f};
+    FaultShortCircuitOutput get_sc_output(ComplexValue<symmetric_t> i_f, double const u_rated) const {
+        ComplexValue<asymmetric_t> const iabc_f{i_f};
         return get_sc_output(iabc_f, u_rated);
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     FaultShortCircuitOutput get_sc_output(FaultShortCircuitMathOutput<sym> const& math_output,
                                           double const u_rated) const {
         return get_sc_output(math_output.i_fault, u_rated);
     }
 
     // update faulted object
     UpdateChange update(FaultUpdate const& update) {
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     double i_n_;
     double base_i_;
     DoubleComplex y1_series_;
     DoubleComplex y1_shunt_;
     DoubleComplex y0_series_;
     DoubleComplex y0_shunt_;
 
-    BranchCalcParam<true> sym_calc_param() const override { return calc_param_y_sym(y1_series_, y1_shunt_, 1.0); }
-    BranchCalcParam<false> asym_calc_param() const override {
+    BranchCalcParam<symmetric_t> sym_calc_param() const override {
+        return calc_param_y_sym(y1_series_, y1_shunt_, 1.0);
+    }
+    BranchCalcParam<asymmetric_t> asym_calc_param() const override {
         return calc_param_y_asym(y1_series_, y1_shunt_, y0_series_, y0_shunt_, 1.0);
     }
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,13 @@
     double loading(double /* max_s */, double /* max_i */) const override { return 0.0; };
     double phase_shift() const override { return 0.0; }
     bool is_param_mutable() const override { return false; }
 
   private:
     double base_i_from_;
     double base_i_to_;
-    BranchCalcParam<true> sym_calc_param() const override { return calc_param_y_sym(y_link, 0.0, 1.0); }
-    BranchCalcParam<false> asym_calc_param() const override { return calc_param_y_asym(y_link, 0.0, y_link, 0.0, 1.0); }
+    BranchCalcParam<symmetric_t> sym_calc_param() const override { return calc_param_y_sym(y_link, 0.0, 1.0); }
+    BranchCalcParam<asymmetric_t> asym_calc_param() const override {
+        return calc_param_y_asym(y_link, 0.0, y_link, 0.0, 1.0);
+    }
 };
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -13,159 +13,181 @@
 #include "../calculation_parameters.hpp"
 #include "../common/common.hpp"
 #include "../common/exception.hpp"
 #include "../common/three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
+struct load_appliance_t {};
+struct gen_appliance_t {};
+
+template <typename T>
+concept appliance_type_tag = std::same_as<T, load_appliance_t> || std::same_as<T, gen_appliance_t>;
+template <appliance_type_tag T> constexpr bool is_generator_v = std::same_as<T, gen_appliance_t>;
+
+static_assert(appliance_type_tag<load_appliance_t>);
+static_assert(appliance_type_tag<gen_appliance_t>);
+static_assert(!is_generator_v<load_appliance_t>);
+static_assert(is_generator_v<gen_appliance_t>);
+
 class GenericLoadGen : public Appliance {
   public:
     using InputType = GenericLoadGenInput;
     static constexpr char const* name = "generic_load_gen";
     ComponentType math_model_type() const final { return ComponentType::generic_load_gen; }
 
     explicit GenericLoadGen(GenericLoadGenInput const& generic_load_gen_input, double u)
         : Appliance{generic_load_gen_input, u}, type_{generic_load_gen_input.type} {}
 
     // getter for load type
     LoadGenType type() const { return type_; }
     // getter for calculation param, power injection
-    template <bool sym> ComplexValue<sym> calc_param(bool is_connected_to_source = true) const {
+    template <symmetry_tag sym> ComplexValue<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return ComplexValue<sym>{};
         }
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return sym_calc_param();
         } else {
             return asym_calc_param();
         }
     }
 
   private:
     LoadGenType type_;
-    virtual ComplexValue<true> sym_calc_param() const = 0;
-    virtual ComplexValue<false> asym_calc_param() const = 0;
+    virtual ComplexValue<symmetric_t> sym_calc_param() const = 0;
+    virtual ComplexValue<asymmetric_t> asym_calc_param() const = 0;
 };
 
 // abstraction of load/generation
 class GenericLoad : public GenericLoadGen {
   public:
     using GenericLoadGen::GenericLoadGen;
 };
 class GenericGenerator : public GenericLoadGen {
   public:
     using GenericLoadGen::GenericLoadGen;
 };
 
-template <bool sym, bool is_gen>
-class LoadGen final : public std::conditional_t<is_gen, GenericGenerator, GenericLoad> {
+template <symmetry_tag loadgen_symmetry_, appliance_type_tag appliance_type_>
+class LoadGen final : public std::conditional_t<is_generator_v<appliance_type_>, GenericGenerator, GenericLoad> {
   public:
-    using InputType = LoadGenInput<sym>;
-    using UpdateType = LoadGenUpdate<sym>;
-    using BaseClass = std::conditional_t<is_gen, GenericGenerator, GenericLoad>;
+    using loadgen_symmetry = loadgen_symmetry_;
+    using appliance_type = appliance_type_;
+
+    using InputType = LoadGenInput<loadgen_symmetry>;
+    using UpdateType = LoadGenUpdate<loadgen_symmetry>;
+    using BaseClass = std::conditional_t<is_generator_v<appliance_type>, GenericGenerator, GenericLoad>;
     static constexpr char const* name = [] {
-        if constexpr (sym) {
-            return is_gen ? "sym_gen" : "sym_load";
+        if constexpr (is_symmetric_v<loadgen_symmetry>) {
+            return is_generator_v<appliance_type> ? "sym_gen" : "sym_load";
         } else {
-            return is_gen ? "asym_gen" : "asym_load";
+            return is_generator_v<appliance_type> ? "asym_gen" : "asym_load";
         }
     }();
 
-    LoadGen(LoadGenInput<sym> const& load_gen_input, double u) : BaseClass{load_gen_input, u} {
+    LoadGen(LoadGenInput<loadgen_symmetry> const& load_gen_input, double u) : BaseClass{load_gen_input, u} {
         set_power(load_gen_input.p_specified, load_gen_input.q_specified);
     }
 
-    void set_power(RealValue<sym> const& new_p_specified, RealValue<sym> const& new_q_specified) {
-        double const scalar = direction_ / base_power<sym>;
-        RealValue<sym> ps = real(s_specified_);
-        RealValue<sym> qs = imag(s_specified_);
-        update_real_value<sym>(new_p_specified, ps, scalar);
-        update_real_value<sym>(new_q_specified, qs, scalar);
+    void set_power(RealValue<loadgen_symmetry> const& new_p_specified,
+                   RealValue<loadgen_symmetry> const& new_q_specified) {
+        double const scalar = direction_ / base_power<loadgen_symmetry>;
+        RealValue<loadgen_symmetry> ps = real(s_specified_);
+        RealValue<loadgen_symmetry> qs = imag(s_specified_);
+        update_real_value<loadgen_symmetry>(new_p_specified, ps, scalar);
+        update_real_value<loadgen_symmetry>(new_q_specified, qs, scalar);
 
-        s_specified_ = ComplexValue<sym>{ps, qs};
+        s_specified_ = ComplexValue<loadgen_symmetry>{ps, qs};
     }
 
     // update for load_gen
-    UpdateChange update(LoadGenUpdate<sym> const& update_data) {
+    UpdateChange update(LoadGenUpdate<loadgen_symmetry> const& update_data) {
         assert(update_data.id == this->id());
         this->set_status(update_data.status);
         set_power(update_data.p_specified, update_data.q_specified);
         // change load connection and/or value will not change topology or parameters
         return {false, false};
     }
 
-    LoadGenUpdate<sym> inverse(LoadGenUpdate<sym> update_data) const {
-        double const scalar = direction_ * base_power<sym>;
+    LoadGenUpdate<loadgen_symmetry> inverse(LoadGenUpdate<loadgen_symmetry> update_data) const {
+        double const scalar = direction_ * base_power<loadgen_symmetry>;
 
         assert(update_data.id == this->id());
 
         set_if_not_nan(update_data.status, static_cast<IntS>(this->status()));
         set_if_not_nan(update_data.p_specified, real(s_specified_) * scalar);
         set_if_not_nan(update_data.q_specified, imag(s_specified_) * scalar);
 
         return update_data;
     }
 
   private:
-    ComplexValue<sym> s_specified_{std::complex<double>{nan, nan}}; // specified power injection
+    ComplexValue<loadgen_symmetry> s_specified_{std::complex<double>{nan, nan}}; // specified power injection
 
     // direction of load_gen
-    static constexpr double direction_ = is_gen ? 1.0 : -1.0;
+    static constexpr double direction_ = is_generator_v<appliance_type> ? 1.0 : -1.0;
 
     // override calc_param
-    ComplexValue<true> sym_calc_param() const override {
-        if constexpr (sym) {
+    ComplexValue<symmetric_t> sym_calc_param() const override {
+        if constexpr (is_symmetric_v<loadgen_symmetry>) {
             if (is_nan(real(s_specified_)) || is_nan(imag(s_specified_))) {
                 return {nan, nan};
             }
         }
         return mean_val(s_specified_);
     }
-    ComplexValue<false> asym_calc_param() const override {
-        if constexpr (sym) {
+    ComplexValue<asymmetric_t> asym_calc_param() const override {
+        if constexpr (is_symmetric_v<loadgen_symmetry>) {
             if (is_nan(real(s_specified_)) || is_nan(imag(s_specified_))) {
-                return ComplexValue<false>{std::complex{nan, nan}};
+                return ComplexValue<asymmetric_t>{std::complex{nan, nan}};
             }
         }
         return piecewise_complex_value(s_specified_);
     }
-    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
-        ApplianceMathOutput<sym_calc> appliance_math_output;
-        appliance_math_output.s = scale_power<sym_calc>(u);
+    template <symmetry_tag calculation_symmetry>
+    ApplianceMathOutput<calculation_symmetry> u2si(ComplexValue<calculation_symmetry> const& u) const {
+        ApplianceMathOutput<calculation_symmetry> appliance_math_output;
+        appliance_math_output.s = scale_power<calculation_symmetry>(u);
         appliance_math_output.i = conj(appliance_math_output.s / u);
         return appliance_math_output;
     }
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const override { return u2si<true>(u); }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const override { return u2si<false>(u); }
+    ApplianceMathOutput<symmetric_t> sym_u2si(ComplexValue<symmetric_t> const& u) const override {
+        return u2si<symmetric_t>(u);
+    }
+    ApplianceMathOutput<asymmetric_t> asym_u2si(ComplexValue<asymmetric_t> const& u) const override {
+        return u2si<asymmetric_t>(u);
+    }
 
     double injection_direction() const override { return direction_; }
 
     // scale load
-    template <bool sym_calc> ComplexValue<sym_calc> scale_power(ComplexValue<sym_calc> u) const {
+    template <symmetry_tag calculation_symmetry>
+    ComplexValue<calculation_symmetry> scale_power(ComplexValue<calculation_symmetry> u) const {
         using enum LoadGenType;
 
-        auto const params = [this] { return this->template calc_param<sym_calc>(); };
+        auto const params = [this] { return this->template calc_param<calculation_symmetry>(); };
         switch (this->type()) {
         case const_pq:
             return params();
         case const_y:
             return params() * abs2(u);
         case const_i:
             return params() * cabs(u);
         default:
             throw MissingCaseForEnumError(std::string(this->name) + " power scaling factor", this->type());
         }
     }
 };
 
 // explicit instantiation
-template class LoadGen<true, true>;
-template class LoadGen<true, false>;
-template class LoadGen<false, true>;
-template class LoadGen<false, false>;
+template class LoadGen<symmetric_t, gen_appliance_t>;
+template class LoadGen<symmetric_t, load_appliance_t>;
+template class LoadGen<asymmetric_t, gen_appliance_t>;
+template class LoadGen<asymmetric_t, load_appliance_t>;
 // alias
-using SymGenerator = LoadGen<true, true>;
-using AsymGenerator = LoadGen<false, true>;
-using SymLoad = LoadGen<true, false>;
-using AsymLoad = LoadGen<false, false>;
+using SymGenerator = LoadGen<symmetric_t, gen_appliance_t>;
+using AsymGenerator = LoadGen<asymmetric_t, gen_appliance_t>;
+using SymLoad = LoadGen<symmetric_t, load_appliance_t>;
+using AsymLoad = LoadGen<asymmetric_t, load_appliance_t>;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -14,53 +14,53 @@
 #include "../common/three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Node final : public Base {
   public:
     using InputType = NodeInput;
-    template <bool sym> using OutputType = NodeOutput<sym>;
+    template <symmetry_tag sym> using OutputType = NodeOutput<sym>;
     using ShortCircuitOutputType = NodeShortCircuitOutput;
     static constexpr char const* name = "node";
     constexpr ComponentType math_model_type() const override { return ComponentType::node; }
 
     explicit Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {}
 
     // update node, nothing happens here
     static constexpr UpdateChange update(BaseUpdate const& /* update_data */) { return {false, false}; }
     static constexpr BaseUpdate inverse(BaseUpdate update_data) { return update_data; }
 
     // energized
-    template <bool sym>
+    template <symmetry_tag sym>
     NodeOutput<sym> get_output(ComplexValue<sym> const& u_pu, ComplexValue<sym> const& bus_injection) const {
         NodeOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         output.u_pu = cabs(u_pu);
         output.u = u_scale<sym> * u_rated_ * output.u_pu;
         output.u_angle = arg(u_pu);
         output.p = base_power<sym> * real(bus_injection);
         output.q = base_power<sym> * imag(bus_injection);
         return output;
     }
 
-    NodeShortCircuitOutput get_sc_output(ComplexValue<false> const& u_pu) const {
+    NodeShortCircuitOutput get_sc_output(ComplexValue<asymmetric_t> const& u_pu) const {
         NodeShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         output.u_pu = cabs(u_pu);
-        output.u = u_scale<false> * u_rated_ * output.u_pu;
+        output.u = u_scale<asymmetric_t> * u_rated_ * output.u_pu;
         output.u_angle = arg(u_pu);
 
         return output;
     }
-    NodeShortCircuitOutput get_sc_output(ComplexValue<true> const& u_pu) const {
+    NodeShortCircuitOutput get_sc_output(ComplexValue<symmetric_t> const& u_pu) const {
         // Convert the input positive sequence voltage to phase voltage
-        ComplexValue<false> const uabc_pu{u_pu};
+        ComplexValue<asymmetric_t> const uabc_pu{u_pu};
         return get_sc_output(uabc_pu);
     }
-    template <bool sym> NodeOutput<sym> get_null_output() const {
+    template <symmetry_tag sym> NodeOutput<sym> get_null_output() const {
         NodeOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     NodeShortCircuitOutput get_null_sc_output() const {
         NodeShortCircuitOutput output{};
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -18,31 +18,31 @@
     static constexpr char const* name = "generic_power_sensor";
 
     explicit GenericPowerSensor(GenericPowerSensorInput const& generic_power_sensor_input)
         : Sensor{generic_power_sensor_input}, terminal_type_{generic_power_sensor_input.measured_terminal_type} {}
 
     MeasuredTerminalType get_terminal_type() const { return terminal_type_; }
 
-    template <bool sym> PowerSensorOutput<sym> get_output(ComplexValue<sym> const& s) const {
-        if constexpr (sym) {
+    template <symmetry_tag sym> PowerSensorOutput<sym> get_output(ComplexValue<sym> const& s) const {
+        if constexpr (is_symmetric_v<sym>) {
             return get_sym_output(s);
         } else {
             return get_asym_output(s);
         }
     }
 
-    template <bool sym> PowerSensorOutput<sym> get_null_output() const {
+    template <symmetry_tag sym> PowerSensorOutput<sym> get_null_output() const {
         return {.id = id(), .energized = false, .p_residual = {}, .q_residual = {}};
     }
 
     SensorShortCircuitOutput get_null_sc_output() const { return {.id = id(), .energized = 0}; }
 
     // getter for calculation param
-    template <bool sym> PowerSensorCalcParam<sym> calc_param() const {
-        if constexpr (sym) {
+    template <symmetry_tag sym> PowerSensorCalcParam<sym> calc_param() const {
+        if constexpr (is_symmetric_v<sym>) {
             return sym_calc_param();
         } else {
             return asym_calc_param();
         }
     }
 
   protected:
@@ -55,127 +55,133 @@
     }
 
   private:
     MeasuredTerminalType terminal_type_;
 
     // virtual function getter for sym and asym param
     // override them in real sensors function
-    virtual PowerSensorCalcParam<true> sym_calc_param() const = 0;
-    virtual PowerSensorCalcParam<false> asym_calc_param() const = 0;
+    virtual PowerSensorCalcParam<symmetric_t> sym_calc_param() const = 0;
+    virtual PowerSensorCalcParam<asymmetric_t> asym_calc_param() const = 0;
 
-    virtual PowerSensorOutput<true> get_sym_output(ComplexValue<true> const& s) const = 0;
-    virtual PowerSensorOutput<false> get_asym_output(ComplexValue<false> const& s) const = 0;
+    virtual PowerSensorOutput<symmetric_t> get_sym_output(ComplexValue<symmetric_t> const& s) const = 0;
+    virtual PowerSensorOutput<asymmetric_t> get_asym_output(ComplexValue<asymmetric_t> const& s) const = 0;
 };
 
-template <bool sym> class PowerSensor : public GenericPowerSensor {
+template <symmetry_tag power_sensor_symmetry_> class PowerSensor : public GenericPowerSensor {
   public:
-    static constexpr char const* name = sym ? "sym_power_sensor" : "asym_power_sensor";
-    using InputType = PowerSensorInput<sym>;
-    using UpdateType = PowerSensorUpdate<sym>;
-    template <bool sym_calc> using OutputType = PowerSensorOutput<sym_calc>;
+    using power_sensor_symmetry = power_sensor_symmetry_;
 
-    explicit PowerSensor(PowerSensorInput<sym> const& power_sensor_input)
+    static constexpr char const* name =
+        is_symmetric_v<power_sensor_symmetry> ? "sym_power_sensor" : "asym_power_sensor";
+    using InputType = PowerSensorInput<power_sensor_symmetry>;
+    using UpdateType = PowerSensorUpdate<power_sensor_symmetry>;
+    template <symmetry_tag sym_calc> using OutputType = PowerSensorOutput<sym_calc>;
+
+    explicit PowerSensor(PowerSensorInput<power_sensor_symmetry> const& power_sensor_input)
         : GenericPowerSensor{power_sensor_input},
-          apparent_power_sigma_{power_sensor_input.power_sigma / base_power<sym>},
-          p_sigma_{power_sensor_input.p_sigma / base_power<sym>},
-          q_sigma_{power_sensor_input.q_sigma / base_power<sym>} {
+          apparent_power_sigma_{power_sensor_input.power_sigma / base_power<power_sensor_symmetry>},
+          p_sigma_{power_sensor_input.p_sigma / base_power<power_sensor_symmetry>},
+          q_sigma_{power_sensor_input.q_sigma / base_power<power_sensor_symmetry>} {
         set_power(power_sensor_input.p_measured, power_sensor_input.q_measured);
     };
 
-    UpdateChange update(PowerSensorUpdate<sym> const& update_data) {
-        constexpr double scalar = 1.0 / base_power<sym>;
+    UpdateChange update(PowerSensorUpdate<power_sensor_symmetry> const& update_data) {
+        constexpr double scalar = 1.0 / base_power<power_sensor_symmetry>;
 
         set_power(update_data.p_measured, update_data.q_measured);
 
         if (!is_nan(update_data.power_sigma)) {
             apparent_power_sigma_ = update_data.power_sigma * scalar;
         }
-        update_real_value<sym>(update_data.p_sigma, p_sigma_, scalar);
-        update_real_value<sym>(update_data.q_sigma, q_sigma_, scalar);
+        update_real_value<power_sensor_symmetry>(update_data.p_sigma, p_sigma_, scalar);
+        update_real_value<power_sensor_symmetry>(update_data.q_sigma, q_sigma_, scalar);
 
         return {false, false};
     }
 
-    PowerSensorUpdate<sym> inverse(PowerSensorUpdate<sym> update_data) const {
+    PowerSensorUpdate<power_sensor_symmetry> inverse(PowerSensorUpdate<power_sensor_symmetry> update_data) const {
         assert(update_data.id == this->id());
 
-        auto const scalar = convert_direction() * base_power<sym>;
+        auto const scalar = convert_direction() * base_power<power_sensor_symmetry>;
 
         set_if_not_nan(update_data.p_measured, real(s_measured_) * scalar);
         set_if_not_nan(update_data.q_measured, imag(s_measured_) * scalar);
-        set_if_not_nan(update_data.power_sigma, apparent_power_sigma_ * base_power<sym>);
-        set_if_not_nan(update_data.p_sigma, p_sigma_ * base_power<sym>);
-        set_if_not_nan(update_data.q_sigma, q_sigma_ * base_power<sym>);
+        set_if_not_nan(update_data.power_sigma, apparent_power_sigma_ * base_power<power_sensor_symmetry>);
+        set_if_not_nan(update_data.p_sigma, p_sigma_ * base_power<power_sensor_symmetry>);
+        set_if_not_nan(update_data.q_sigma, q_sigma_ * base_power<power_sensor_symmetry>);
 
         return update_data;
     }
 
   private:
-    ComplexValue<sym> s_measured_{};
+    ComplexValue<power_sensor_symmetry> s_measured_{};
 
     double apparent_power_sigma_{};
-    RealValue<sym> p_sigma_{};
-    RealValue<sym> q_sigma_{};
+    RealValue<power_sensor_symmetry> p_sigma_{};
+    RealValue<power_sensor_symmetry> q_sigma_{};
 
-    void set_power(RealValue<sym> const& p_measured, RealValue<sym> const& q_measured) {
-        double const scalar = convert_direction() / base_power<sym>;
-        RealValue<sym> ps = real(s_measured_);
-        RealValue<sym> qs = imag(s_measured_);
-        update_real_value<sym>(p_measured, ps, scalar);
-        update_real_value<sym>(q_measured, qs, scalar);
+    void set_power(RealValue<power_sensor_symmetry> const& p_measured,
+                   RealValue<power_sensor_symmetry> const& q_measured) {
+        double const scalar = convert_direction() / base_power<power_sensor_symmetry>;
+        RealValue<power_sensor_symmetry> ps = real(s_measured_);
+        RealValue<power_sensor_symmetry> qs = imag(s_measured_);
+        update_real_value<power_sensor_symmetry>(p_measured, ps, scalar);
+        update_real_value<power_sensor_symmetry>(q_measured, qs, scalar);
         s_measured_ = ps + 1.0i * qs;
     }
 
-    PowerSensorCalcParam<true> sym_calc_param() const final {
-        PowerSensorCalcParam<true> calc_param{};
+    PowerSensorCalcParam<symmetric_t> sym_calc_param() const final {
+        PowerSensorCalcParam<symmetric_t> calc_param{};
         if (is_normal(p_sigma_) && is_normal(q_sigma_)) {
             calc_param.p_variance = mean_val(p_sigma_ * p_sigma_);
             calc_param.q_variance = mean_val(q_sigma_ * q_sigma_);
         } else {
             auto const variance = is_nan(p_sigma_) ? apparent_power_sigma_ * apparent_power_sigma_ / 2
                                                    : std::numeric_limits<double>::infinity();
             calc_param.p_variance = variance;
             calc_param.q_variance = variance;
         }
         assert(is_nan(calc_param.p_variance) == is_nan(calc_param.q_variance));
 
         calc_param.value = mean_val(s_measured_);
         return calc_param;
     }
-    PowerSensorCalcParam<false> asym_calc_param() const final {
-        PowerSensorCalcParam<false> calc_param{};
+    PowerSensorCalcParam<asymmetric_t> asym_calc_param() const final {
+        PowerSensorCalcParam<asymmetric_t> calc_param{};
         if (is_normal(p_sigma_) && is_normal(q_sigma_)) {
-            calc_param.p_variance = RealValue<false>{p_sigma_ * p_sigma_};
-            calc_param.q_variance = RealValue<false>{q_sigma_ * q_sigma_};
+            calc_param.p_variance = RealValue<asymmetric_t>{p_sigma_ * p_sigma_};
+            calc_param.q_variance = RealValue<asymmetric_t>{q_sigma_ * q_sigma_};
         } else {
-            auto const variance = RealValue<false>{is_nan(p_sigma_) ? apparent_power_sigma_ * apparent_power_sigma_ / 2
-                                                                    : std::numeric_limits<double>::infinity()};
+            auto const variance =
+                RealValue<asymmetric_t>{is_nan(p_sigma_) ? apparent_power_sigma_ * apparent_power_sigma_ / 2
+                                                         : std::numeric_limits<double>::infinity()};
             calc_param.p_variance = variance;
             calc_param.q_variance = variance;
         }
         assert(is_nan(calc_param.p_variance) == is_nan(calc_param.q_variance));
 
         calc_param.value = piecewise_complex_value(s_measured_);
         return calc_param;
     }
-    PowerSensorOutput<true> get_sym_output(ComplexValue<true> const& s) const final {
-        return get_generic_output<true>(s);
+    PowerSensorOutput<symmetric_t> get_sym_output(ComplexValue<symmetric_t> const& s) const final {
+        return get_generic_output<symmetric_t>(s);
     }
-    PowerSensorOutput<false> get_asym_output(ComplexValue<false> const& s) const final {
-        return get_generic_output<false>(s);
+    PowerSensorOutput<asymmetric_t> get_asym_output(ComplexValue<asymmetric_t> const& s) const final {
+        return get_generic_output<asymmetric_t>(s);
     }
-    template <bool sym_calc> PowerSensorOutput<sym_calc> get_generic_output(ComplexValue<sym_calc> const& s) const {
+    template <symmetry_tag sym_calc>
+    PowerSensorOutput<sym_calc> get_generic_output(ComplexValue<sym_calc> const& s) const {
         PowerSensorOutput<sym_calc> output{};
         ComplexValue<sym_calc> const s_residual{process_mean_val<sym_calc>(s_measured_ - s) * convert_direction() *
                                                 base_power<sym_calc>};
         output.id = id();
         output.energized = 1; // power sensor is always energized
         output.p_residual = real(s_residual);
         output.q_residual = imag(s_residual);
         return output;
     }
 };
 
-using SymPowerSensor = PowerSensor<true>;
-using AsymPowerSensor = PowerSensor<false>;
+using SymPowerSensor = PowerSensor<symmetric_t>;
+using AsymPowerSensor = PowerSensor<asymmetric_t>;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 
     explicit Shunt(ShuntInput const& shunt_input, double u)
         : Appliance{shunt_input, u}, base_y_{base_i() / (u / sqrt3)} {
         update_params(shunt_input);
     }
 
     // getter for calculation param, shunt y
-    template <bool sym> ComplexTensor<sym> calc_param(bool is_connected_to_source = true) const {
+    template <symmetry_tag sym> ComplexTensor<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return ComplexTensor<sym>{};
         }
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return y1_;
         } else {
             // abc matrix
             // 1/3 *
             // [[2y1+y0, y0-y1, y0-y1],
             //  [y0-y1, 2y1+y0, y0-y1],
             //  [y0-y1, y0-y1, 2y1+y0]]
-            return ComplexTensor<false>{(2.0 * y1_ + y0_) / 3.0, (y0_ - y1_) / 3.0};
+            return ComplexTensor<asymmetric_t>{(2.0 * y1_ + y0_) / 3.0, (y0_ - y1_) / 3.0};
         }
     }
 
     UpdateChange update(ShuntUpdate const& update_data) {
         assert(update_data.id == id());
         bool changed = set_status(update_data.status);
         changed = update_params(update_data) || changed;
@@ -97,22 +97,26 @@
             return false;
         }
 
         target = value;
         return true;
     }
 
-    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
+    template <symmetry_tag sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
         ApplianceMathOutput<sym_calc> appliance_math_output;
         ComplexTensor<sym_calc> const param = calc_param<sym_calc>();
         // return value should be injection direction, therefore a negative sign for i
         appliance_math_output.i = -dot(param, u);
         appliance_math_output.s = u * conj(appliance_math_output.i);
         return appliance_math_output;
     }
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final { return u2si<true>(u); }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final { return u2si<false>(u); }
+    ApplianceMathOutput<symmetric_t> sym_u2si(ComplexValue<symmetric_t> const& u) const final {
+        return u2si<symmetric_t>(u);
+    }
+    ApplianceMathOutput<asymmetric_t> asym_u2si(ComplexValue<asymmetric_t> const& u) const final {
+        return u2si<asymmetric_t>(u);
+    }
 
     double injection_direction() const final { return -1.0; }
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -39,24 +39,24 @@
         double const x1 = z_abs / sqrt(rx_ratio * rx_ratio + 1.0);
         double const r1 = x1 * rx_ratio;
         y1_ref_ = 1.0 / DoubleComplex{r1, x1};
         y0_ref_ = y1_ref_ / z01_ratio;
     }
 
     // getter for calculation param, y_ref
-    template <bool sym> ComplexTensor<sym> math_param() const {
+    template <symmetry_tag sym> ComplexTensor<sym> math_param() const {
         // internal element_admittance
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return y1_ref_;
         } else {
-            ComplexTensor<false> const sym_matrix = get_sym_matrix();
-            ComplexTensor<false> const sym_matrix_inv = get_sym_matrix_inv();
-            ComplexTensor<false> y012;
+            ComplexTensor<asymmetric_t> const sym_matrix = get_sym_matrix();
+            ComplexTensor<asymmetric_t> const sym_matrix_inv = get_sym_matrix_inv();
+            ComplexTensor<asymmetric_t> y012;
             y012 << y1_ref_, 0.0, 0.0, 0.0, y1_ref_, 0.0, 0.0, 0.0, y0_ref_;
-            ComplexTensor<false> yabc = dot(sym_matrix, y012, sym_matrix_inv);
+            ComplexTensor<asymmetric_t> yabc = dot(sym_matrix, y012, sym_matrix_inv);
             return yabc;
         }
     }
 
     // setter
     bool set_u_ref(double new_u_ref, double new_u_ref_angle) {
         bool changed = false;
@@ -116,23 +116,27 @@
   private:
     double u_ref_;
     double u_ref_angle_;
     // positive and zero sequence ref
     DoubleComplex y1_ref_{};
     DoubleComplex y0_ref_{};
 
-    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
+    template <symmetry_tag sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
         ApplianceMathOutput<sym_calc> appliance_math_output;
         ComplexValue<sym_calc> const u_ref{u_ref_};
         ComplexTensor<sym_calc> const y_ref = math_param<sym_calc>();
         appliance_math_output.i = dot(y_ref, u_ref - u);
         appliance_math_output.s = u * conj(appliance_math_output.i);
         return appliance_math_output;
     }
 
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final { return u2si<true>(u); }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final { return u2si<false>(u); }
+    ApplianceMathOutput<symmetric_t> sym_u2si(ComplexValue<symmetric_t> const& u) const final {
+        return u2si<symmetric_t>(u);
+    }
+    ApplianceMathOutput<asymmetric_t> asym_u2si(ComplexValue<asymmetric_t> const& u) const final {
+        return u2si<asymmetric_t>(u);
+    }
 
     double injection_direction() const final { return 1.0; }
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -387,26 +387,26 @@
         Transformer const T2{transformer_input_T2, u2_rated_, u1_rated_};
         Transformer const T3{transformer_input_T3, u3_rated_, u1_rated_};
 
         return {T1, T2, T3};
     }
 
     // calculate branch parameters
-    std::array<BranchCalcParam<true>, 3> sym_calc_param() const final {
+    std::array<BranchCalcParam<symmetric_t>, 3> sym_calc_param() const final {
         std::array<Transformer, 3> const transformer_array = convert_to_two_winding_transformers();
-        std::array<BranchCalcParam<true>, 3> transformer_params{};
+        std::array<BranchCalcParam<symmetric_t>, 3> transformer_params{};
         for (size_t i = 0; i < transformer_array.size(); i++) {
-            transformer_params[i] = transformer_array[i].calc_param<true>();
+            transformer_params[i] = transformer_array[i].calc_param<symmetric_t>();
         }
         return transformer_params;
     }
-    std::array<BranchCalcParam<false>, 3> asym_calc_param() const final {
+    std::array<BranchCalcParam<asymmetric_t>, 3> asym_calc_param() const final {
         std::array<Transformer, 3> const transformer_array = convert_to_two_winding_transformers();
-        std::array<BranchCalcParam<false>, 3> transformer_params{};
+        std::array<BranchCalcParam<asymmetric_t>, 3> transformer_params{};
         for (size_t i = 0; i < transformer_array.size(); i++) {
-            transformer_params[i] = transformer_array[i].calc_param<false>();
+            transformer_params[i] = transformer_array[i].calc_param<asymmetric_t>();
         }
         return transformer_params;
     }
 };
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -198,26 +198,26 @@
         // y shunt
         y_shunt = y_shunt / base_y_to;
         // return
         return std::make_tuple(y_series, y_shunt, k);
     }
 
     // branch param
-    BranchCalcParam<true> sym_calc_param() const final {
+    BranchCalcParam<symmetric_t> sym_calc_param() const final {
         auto const [y_series, y_shunt, k] = transformer_params();
         return calc_param_y_sym(y_series, y_shunt, k * std::exp(1.0i * (clock_ * deg_30)));
     }
-    BranchCalcParam<false> asym_calc_param() const final {
+    BranchCalcParam<asymmetric_t> asym_calc_param() const final {
         auto const [y_series, y_shunt, k] = transformer_params();
         // positive sequence
         auto const param1 = calc_param_y_sym(y_series, y_shunt, k * std::exp(1.0i * (clock_ * deg_30)));
         // negative sequence
         auto const param2 = calc_param_y_sym(y_series, y_shunt, k * std::exp(1.0i * (-clock_ * deg_30)));
         // zero sequence, default zero
-        BranchCalcParam<true> param0{};
+        BranchCalcParam<symmetric_t> param0{};
         // YNyn
         if (winding_from_ == WindingType::wye_n && winding_to_ == WindingType::wye_n) {
             double phase_shift_0 = 0.0;
             // flip sign for reverse connected
             if (clock_ == 2 || clock_ == 6 || clock_ == 10) {
                 phase_shift_0 = 6.0 * deg_30;
             }
@@ -248,20 +248,20 @@
             DoubleComplex const z0_series = (1.0 / y_series) * 0.1 + 3.0 * z_grounding_to_;
             DoubleComplex const y0_series = 1.0 / z0_series;
             param0.ytt() = y0_series;
         }
 
         // for the rest param0 is zero
         // calculate yabc
-        ComplexTensor<false> const sym_matrix = get_sym_matrix();
-        ComplexTensor<false> const sym_matrix_inv = get_sym_matrix_inv();
-        BranchCalcParam<false> param;
+        ComplexTensor<asymmetric_t> const sym_matrix = get_sym_matrix();
+        ComplexTensor<asymmetric_t> const sym_matrix_inv = get_sym_matrix_inv();
+        BranchCalcParam<asymmetric_t> param;
         for (size_t i = 0; i != 4; ++i) {
             // Yabc = A * Y012 * A^-1
-            ComplexTensor<false> y012;
+            ComplexTensor<asymmetric_t> y012;
             y012 << param0.value[i], 0.0, 0.0, 0.0, param1.value[i], 0.0, 0.0, 0.0, param2.value[i];
             param.value[i] = dot(sym_matrix, y012, sym_matrix_inv);
         }
         return param;
     }
 };
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 class GenericVoltageSensor : public Sensor {
   public:
     static constexpr char const* name = "generic_voltage_sensor";
 
     explicit GenericVoltageSensor(GenericVoltageSensorInput const& generic_voltage_sensor_input)
         : Sensor{generic_voltage_sensor_input} {};
 
-    template <bool sym> VoltageSensorOutput<sym> get_output(ComplexValue<sym> const& u) const {
-        if constexpr (sym) {
+    template <symmetry_tag sym> VoltageSensorOutput<sym> get_output(ComplexValue<sym> const& u) const {
+        if constexpr (is_symmetric_v<sym>) {
             assert(u != 0.0 + 0.0i);
             return get_sym_output(u);
         } else {
             assert(u[0] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(u[1] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(u[2] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(abs(arg(u[0]) - arg(u[1])) > std::numeric_limits<double>::epsilon() &&
@@ -36,45 +36,45 @@
                    "Voltage angles should not be equal");
             assert(abs(arg(u[2]) - arg(u[0])) > std::numeric_limits<double>::epsilon() &&
                    "Voltage angles should not be equal");
             return get_asym_output(u);
         }
     }
 
-    template <bool sym> VoltageSensorOutput<sym> get_null_output() const {
+    template <symmetry_tag sym> VoltageSensorOutput<sym> get_null_output() const {
         return {.id = id(), .energized = false, .u_residual = {}, .u_angle_residual = {}};
     }
 
     SensorShortCircuitOutput get_null_sc_output() const { return {.id = id(), .energized = 0}; }
 
     // getter for calculation param
-    template <bool sym> VoltageSensorCalcParam<sym> calc_param() const {
-        if constexpr (sym) {
+    template <symmetry_tag sym> VoltageSensorCalcParam<sym> calc_param() const {
+        if constexpr (is_symmetric_v<sym>) {
             return sym_calc_param();
         } else {
             return asym_calc_param();
         }
     }
 
   private:
     // virtual function getter for sym and asym param
     // override them in real sensors function
-    virtual VoltageSensorCalcParam<true> sym_calc_param() const = 0;
-    virtual VoltageSensorCalcParam<false> asym_calc_param() const = 0;
+    virtual VoltageSensorCalcParam<symmetric_t> sym_calc_param() const = 0;
+    virtual VoltageSensorCalcParam<asymmetric_t> asym_calc_param() const = 0;
 
-    virtual VoltageSensorOutput<true> get_sym_output(ComplexValue<true> const& u) const = 0;
-    virtual VoltageSensorOutput<false> get_asym_output(ComplexValue<false> const& u) const = 0;
+    virtual VoltageSensorOutput<symmetric_t> get_sym_output(ComplexValue<symmetric_t> const& u) const = 0;
+    virtual VoltageSensorOutput<asymmetric_t> get_asym_output(ComplexValue<asymmetric_t> const& u) const = 0;
 };
 
-template <bool sym> class VoltageSensor : public GenericVoltageSensor {
+template <symmetry_tag sym> class VoltageSensor : public GenericVoltageSensor {
   public:
-    static constexpr char const* name = sym ? "sym_voltage_sensor" : "asym_voltage_sensor";
+    static constexpr char const* name = is_symmetric_v<sym> ? "sym_voltage_sensor" : "asym_voltage_sensor";
     using InputType = VoltageSensorInput<sym>;
     using UpdateType = VoltageSensorUpdate<sym>;
-    template <bool sym_calc> using OutputType = VoltageSensorOutput<sym_calc>;
+    template <symmetry_tag sym_calc> using OutputType = VoltageSensorOutput<sym_calc>;
 
     explicit VoltageSensor(VoltageSensorInput<sym> const& voltage_sensor_input, double u_rated)
         : GenericVoltageSensor{voltage_sensor_input},
           u_rated_{u_rated},
           u_sigma_{voltage_sensor_input.u_sigma / (u_rated_ * u_scale<sym>)},
           u_measured_{voltage_sensor_input.u_measured / (u_rated_ * u_scale<sym>)},
           u_angle_measured_{voltage_sensor_input.u_angle_measured} {};
@@ -109,64 +109,64 @@
   private:
     double u_rated_;
     double u_sigma_;
     RealValue<sym> u_measured_;
     RealValue<sym> u_angle_measured_;
 
     bool has_angle() const {
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return !is_nan(u_angle_measured_);
         } else {
             return !u_angle_measured_.isNaN().any();
         }
     }
 
-    VoltageSensorCalcParam<true> sym_calc_param() const final {
+    VoltageSensorCalcParam<symmetric_t> sym_calc_param() const final {
         double const u_variance = u_sigma_ * u_sigma_;
         if (has_angle()) {
-            ComplexValue<true> const u = pos_seq(u_measured_ * exp(1i * u_angle_measured_));
+            ComplexValue<symmetric_t> const u = pos_seq(u_measured_ * exp(1i * u_angle_measured_));
             return {u, u_variance};
         }
-        ComplexValue<true> const u{mean_val(u_measured_), nan};
+        ComplexValue<symmetric_t> const u{mean_val(u_measured_), nan};
         return {u, u_variance};
     }
 
-    VoltageSensorCalcParam<false> asym_calc_param() const final {
+    VoltageSensorCalcParam<asymmetric_t> asym_calc_param() const final {
         double const u_variance = u_sigma_ * u_sigma_;
         if (has_angle()) {
-            ComplexValue<false> const u{u_measured_ * exp(1i * u_angle_measured_)};
+            ComplexValue<asymmetric_t> const u{u_measured_ * exp(1i * u_angle_measured_)};
             return {u, u_variance};
         }
-        ComplexValue<false> const u = RealValue<false>{u_measured_} + DoubleComplex{0.0, nan};
+        ComplexValue<asymmetric_t> const u = RealValue<asymmetric_t>{u_measured_} + DoubleComplex{0.0, nan};
         return {u, u_variance};
     }
 
-    VoltageSensorOutput<true> get_sym_output(ComplexValue<true> const& u) const final {
-        VoltageSensorOutput<true> value;
+    VoltageSensorOutput<symmetric_t> get_sym_output(ComplexValue<symmetric_t> const& u) const final {
+        VoltageSensorOutput<symmetric_t> value;
         value.id = id();
         value.energized = 1;
 
         DoubleComplex const u1_measured = sym_calc_param().value;
         bool const has_angle = !is_nan(imag(u1_measured));
         if (has_angle) {
             value.u_residual = (cabs(u1_measured) - cabs(u)) * u_rated_;
         } else {
             value.u_residual = (real(u1_measured) - cabs(u)) * u_rated_;
         }
         value.u_angle_residual = arg(u1_measured) - arg(u);
         return value;
     }
 
-    VoltageSensorOutput<false> get_asym_output(ComplexValue<false> const& u) const final {
-        VoltageSensorOutput<false> value;
+    VoltageSensorOutput<asymmetric_t> get_asym_output(ComplexValue<asymmetric_t> const& u) const final {
+        VoltageSensorOutput<asymmetric_t> value;
         value.id = id();
         value.energized = 1;
         value.u_residual = (u_measured_ - cabs(u)) * u_rated_ / sqrt3;
         value.u_angle_residual = u_angle_measured_ - arg(u);
         return value;
     }
 };
 
-using SymVoltageSensor = VoltageSensor<true>;
-using AsymVoltageSensor = VoltageSensor<false>;
+using SymVoltageSensor = VoltageSensor<symmetric_t>;
+using AsymVoltageSensor = VoltageSensor<asymmetric_t>;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/index_mapping.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/index_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/calculation_info.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/calculation_info.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 // output node
 template <std::same_as<Node> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Node, Idx2D>(state, res_it, [&math_output](Node const& node, Idx2D math_id) {
-        constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+        using sym = typename MathOutputType::sym;
 
         if (math_id.group == -1) {
             return node.get_null_output<sym>();
         }
         return node.get_output<sym>(math_output[math_id.group].u[math_id.pos],
                                     math_output[math_id.group].bus_injection[math_id.pos]);
     });
@@ -123,15 +123,15 @@
 // output branch
 template <std::derived_from<Branch> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Branch const& branch, Idx2D math_id) {
-        constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+        using sym = typename MathOutputType::sym;
 
         if (math_id.group == -1) {
             return branch.get_null_output<sym>();
         }
         return branch.get_output<sym>(math_output[math_id.group].branch[math_id.pos]);
     });
 }
@@ -152,15 +152,15 @@
 template <std::derived_from<Branch3> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2DBranch3>(
         state, res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
-            constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+            using sym = typename MathOutputType::sym;
 
             if (math_id.group == -1) {
                 return branch3.get_null_output<sym>();
             }
 
             auto const& branches = math_output[math_id.group].branch;
             return branch3.get_output<sym>(branches[math_id.pos[0]], branches[math_id.pos[1]],
@@ -198,15 +198,15 @@
 // output source
 template <std::same_as<Source> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Source const& source, Idx2D math_id) {
-        constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+        using sym = typename MathOutputType::sym;
 
         if (math_id.group == -1) {
             return source.get_null_output<sym>();
         }
         return source.get_output<sym>(math_output[math_id.group].source[math_id.pos]);
     });
 }
@@ -227,15 +227,15 @@
 template <std::derived_from<GenericLoadGen> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(
         state, res_it, [&math_output](GenericLoadGen const& load_gen, Idx2D math_id) {
-            constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+            using sym = typename MathOutputType::sym;
 
             if (math_id.group == -1) {
                 return load_gen.get_null_output<sym>();
             }
             return load_gen.get_output<sym>(math_output[math_id.group].load_gen[math_id.pos]);
         });
 }
@@ -252,15 +252,15 @@
 // output shunt
 template <std::same_as<Shunt> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Shunt const& shunt, Idx2D math_id) {
-        constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+        using sym = typename MathOutputType::sym;
 
         if (math_id.group == -1) {
             return shunt.get_null_output<sym>();
         }
         return shunt.get_output<sym>(math_output[math_id.group].shunt[math_id.pos]);
     });
 }
@@ -281,15 +281,15 @@
 template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericVoltageSensor const& voltage_sensor, Idx const node_seq) {
-            constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+            using sym = typename MathOutputType::sym;
 
             Idx2D const node_math_id = state.topo_comp_coup->node[node_seq];
             if (node_math_id.group == -1) {
                 return voltage_sensor.get_null_output<sym>();
             }
             return voltage_sensor.get_output<sym>(math_output[node_math_id.group].u[node_math_id.pos]);
         });
@@ -309,15 +309,15 @@
 template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
     requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericPowerSensor const& power_sensor, Idx const obj_seq) {
-            constexpr auto sym = symmetric_math_output_type<MathOutputType>;
+            using sym = typename MathOutputType::sym;
 
             auto const terminal_type = power_sensor.get_terminal_type();
             Idx2D const obj_math_id = [&]() {
                 switch (terminal_type) {
                     using enum MeasuredTerminalType;
 
                 case branch_from:
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/topology.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -98,37 +98,37 @@
         [&destination, &state](UpdateType const& update_data, Idx2D const& sequence_single) {
             auto const& comp = state.components.template get_item<Component>(sequence_single);
             *destination++ = comp.inverse(update_data);
         },
         begin, end, sequence_idx);
 }
 
-template <bool sym>
+template <symmetry_tag sym>
 inline void update_y_bus(MathState& math_state, std::vector<MathModelParam<sym>> const& math_model_params) {
     auto& y_bus_vec = [&math_state]() -> auto& {
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return math_state.y_bus_vec_sym;
         } else {
             return math_state.y_bus_vec_asym;
         }
     }
     ();
 
     assert(y_bus_vec.size() == math_model_params.size());
 
     for (Idx i = 0; i != static_cast<Idx>(y_bus_vec.size()); ++i) {
         y_bus_vec[i].update_admittance(std::make_shared<MathModelParam<sym> const>(std::move(math_model_params[i])));
     }
 }
 
-template <bool sym>
+template <symmetry_tag sym>
 inline void update_y_bus(MathState& math_state, std::vector<MathModelParam<sym>> const& math_model_params,
                          std::vector<MathModelParamIncrement> const& math_model_param_increments) {
     auto& y_bus_vec = [&math_state]() -> auto& {
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return math_state.y_bus_vec_sym;
         } else {
             return math_state.y_bus_vec_asym;
         }
     }
     ();
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
               typename PrepareInputFn, typename SolveFn>
         requires std::invocable<std::remove_cvref_t<PrepareInputFn>> &&
                  std::invocable<std::remove_cvref_t<SolveFn>, MathSolverType&, YBus const&, InputType const&> &&
                  std::same_as<std::invoke_result_t<PrepareInputFn>, std::vector<InputType>> &&
                  std::same_as<std::invoke_result_t<SolveFn, MathSolverType&, YBus const&, InputType const&>,
                               MathOutputType>
     std::vector<MathOutputType> calculate_(PrepareInputFn&& prepare_input, SolveFn&& solve) {
-        constexpr bool sym = symmetric_math_output_type<MathOutputType>;
+        using sym = typename MathOutputType::sym;
 
         assert(construction_complete_);
         calculation_info_ = CalculationInfo{};
         // prepare
         auto const& input = [this, &prepare_input] {
             Timer const timer(calculation_info_, 2100, "Prepare");
             prepare_solvers<sym>();
@@ -355,38 +355,38 @@
             for (Idx i = 0; i != n_math_solvers_; ++i) {
                 math_output.emplace_back(solve(solvers[i], y_bus_vec[i], input[i]));
             }
             return math_output;
         }();
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<MathOutput<sym>> calculate_power_flow_(double err_tol, Idx max_iter,
                                                        CalculationMethod calculation_method) {
         return calculate_<MathOutput<sym>, MathSolver<sym>, YBus<sym>, PowerFlowInput<sym>>(
             [this] { return prepare_power_flow_input<sym>(); },
             [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, YBus<sym> const& y_bus,
                                                           PowerFlowInput<sym> const& input) {
                 return solver.run_power_flow(input, err_tol, max_iter, calculation_info_, calculation_method, y_bus);
             });
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<MathOutput<sym>> calculate_state_estimation_(double err_tol, Idx max_iter,
                                                              CalculationMethod calculation_method) {
         return calculate_<MathOutput<sym>, MathSolver<sym>, YBus<sym>, StateEstimationInput<sym>>(
             [this] { return prepare_state_estimation_input<sym>(); },
             [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, YBus<sym> const& y_bus,
                                                           StateEstimationInput<sym> const& input) {
                 return solver.run_state_estimation(input, err_tol, max_iter, calculation_info_, calculation_method,
                                                    y_bus);
             });
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<ShortCircuitMathOutput<sym>> calculate_short_circuit_(ShortCircuitVoltageScaling voltage_scaling,
                                                                       CalculationMethod calculation_method) {
         return calculate_<ShortCircuitMathOutput<sym>, MathSolver<sym>, YBus<sym>, ShortCircuitInput>(
             [this, voltage_scaling] { return prepare_short_circuit_input<sym>(voltage_scaling); },
             [this, calculation_method](MathSolver<sym>& solver, YBus<sym> const& y_bus,
                                        ShortCircuitInput const& input) {
                 return solver.run_short_circuit(input, calculation_info_, calculation_method, y_bus);
@@ -647,95 +647,95 @@
                                   [](UpdateType<Component> const& obj, UpdateType<Component> const& first) {
                                       return obj.id == first.id;
                                   });
             });
     }
 
     // Single load flow calculation, returning math output results
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<MathOutput<sym>> calculate_power_flow(double err_tol, Idx max_iter,
                                                       CalculationMethod calculation_method) {
         return calculate_power_flow_<sym>(err_tol, max_iter, calculation_method);
     }
 
     // Single load flow calculation, propagating the results to result_data
-    template <bool sym>
+    template <symmetry_tag sym>
     void calculate_power_flow(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                               Dataset const& result_data, Idx pos = 0) {
         assert(construction_complete_);
         auto const math_output = calculate_power_flow_<sym>(err_tol, max_iter, calculation_method);
         if (pos != ignore_output) {
             output_result(math_output, result_data, pos);
         }
     }
 
     // Batch load flow calculation, propagating the results to result_data
-    template <bool sym>
+    template <symmetry_tag sym>
     BatchParameter calculate_power_flow(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                         Dataset const& result_data, ConstDataset const& update_data,
                                         Idx threading = -1) {
         return batch_calculation_(
             [err_tol, max_iter, calculation_method](MainModelImpl& model, Dataset const& target_data, Idx pos) {
                 auto const err_tol_ = pos != ignore_output ? err_tol : std::numeric_limits<double>::max();
                 auto const max_iter_ = pos != ignore_output ? max_iter : 1;
 
                 model.calculate_power_flow<sym>(err_tol_, max_iter_, calculation_method, target_data, pos);
             },
             result_data, update_data, threading);
     }
 
     // Single state estimation calculation, returning math output results
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<MathOutput<sym>> calculate_state_estimation(double err_tol, Idx max_iter,
                                                             CalculationMethod calculation_method) {
         return calculate_state_estimation_<sym>(err_tol, max_iter, calculation_method);
     }
 
     // Single state estimation calculation, propagating the results to result_data
-    template <bool sym>
+    template <symmetry_tag sym>
     void calculate_state_estimation(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                     Dataset const& result_data, Idx pos = 0) {
         assert(construction_complete_);
         auto const math_output = calculate_state_estimation_<sym>(err_tol, max_iter, calculation_method);
         output_result(math_output, result_data, pos);
     }
 
     // Batch state estimation calculation, propagating the results to result_data
-    template <bool sym>
+    template <symmetry_tag sym>
     BatchParameter calculate_state_estimation(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                               Dataset const& result_data, ConstDataset const& update_data,
                                               Idx threading = -1) {
         return batch_calculation_(
             [err_tol, max_iter, calculation_method](MainModelImpl& model, Dataset const& target_data, Idx pos) {
                 auto const err_tol_ = pos != ignore_output ? err_tol : std::numeric_limits<double>::max();
                 auto const max_iter_ = pos != ignore_output ? max_iter : 1;
 
                 model.calculate_state_estimation<sym>(err_tol_, max_iter_, calculation_method, target_data, pos);
             },
             result_data, update_data, threading);
     }
 
     // Single short circuit calculation, returning short circuit math output results
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<ShortCircuitMathOutput<sym>> calculate_short_circuit(ShortCircuitVoltageScaling voltage_scaling,
                                                                      CalculationMethod calculation_method) {
         return calculate_short_circuit_<sym>(voltage_scaling, calculation_method);
     }
 
     // Single short circuit calculation, propagating the results to result_data
     void calculate_short_circuit(ShortCircuitVoltageScaling voltage_scaling, CalculationMethod calculation_method,
                                  Dataset const& result_data, Idx pos = 0) {
         assert(construction_complete_);
         if (std::all_of(state_.components.template citer<Fault>().begin(),
                         state_.components.template citer<Fault>().end(),
                         [](Fault const& fault) { return fault.get_fault_type() == FaultType::three_phase; })) {
-            auto const math_output = calculate_short_circuit_<true>(voltage_scaling, calculation_method);
+            auto const math_output = calculate_short_circuit_<symmetric_t>(voltage_scaling, calculation_method);
             output_result(math_output, result_data, pos);
         } else {
-            auto const math_output = calculate_short_circuit_<false>(voltage_scaling, calculation_method);
+            auto const math_output = calculate_short_circuit_<asymmetric_t>(voltage_scaling, calculation_method);
             output_result(math_output, result_data, pos);
         }
     }
 
     // Batch short circuit calculation, propagating the results to result_data
     BatchParameter calculate_short_circuit(ShortCircuitVoltageScaling voltage_scaling,
                                            CalculationMethod calculation_method, Dataset const& result_data,
@@ -756,26 +756,27 @@
     }
 
     template <math_output_type MathOutputType>
     void output_result(std::vector<MathOutputType> const& math_output, Dataset const& result_data, Idx pos = 0) {
         using OutputFunc = void (*)(MainModelImpl & x, std::vector<MathOutputType> const& math_output,
                                     MutableDataPointer const& data_ptr, Idx position);
 
-        static constexpr std::array<OutputFunc, n_types> get_result{
-            [](MainModelImpl& model, std::vector<MathOutputType> const& math_output_,
-               MutableDataPointer const& data_ptr, Idx position) {
-                auto const begin =
-                    data_ptr
-                        .get_iterators<std::conditional_t<
-                            steady_state_math_output_type<MathOutputType>,
-                            typename ComponentType::template OutputType<symmetric_math_output_type<MathOutputType>>,
-                            typename ComponentType::ShortCircuitOutputType>>(position)
-                        .first;
-                model.output_result<ComponentType>(math_output_, begin);
-            }...};
+        static constexpr std::array<OutputFunc, n_types> get_result{[](MainModelImpl& model,
+                                                                       std::vector<MathOutputType> const& math_output_,
+                                                                       MutableDataPointer const& data_ptr,
+                                                                       Idx position) {
+            auto const begin =
+                data_ptr
+                    .get_iterators<
+                        std::conditional_t<steady_state_math_output_type<MathOutputType>,
+                                           typename ComponentType::template OutputType<typename MathOutputType::sym>,
+                                           typename ComponentType::ShortCircuitOutputType>>(position)
+                    .first;
+            model.output_result<ComponentType>(math_output_, begin);
+        }...};
 
         Timer const t_output(calculation_info_, 3000, "Produce output");
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
             auto const found = result_data.find(entry.name);
             // skip if component does not exist
             if (found == result_data.cend()) {
                 continue;
@@ -806,32 +807,32 @@
     UpdateChange cached_state_changes_{};
     std::array<std::vector<Idx2D>, n_types> parameter_changed_components_{};
 #ifndef NDEBUG
     // construction_complete is used for debug assertions only
     bool construction_complete_{false};
 #endif // !NDEBUG
 
-    template <bool sym> bool& is_parameter_up_to_date() {
-        if constexpr (sym) {
+    template <symmetry_tag sym> bool& is_parameter_up_to_date() {
+        if constexpr (is_symmetric_v<sym>) {
             return is_sym_parameter_up_to_date_;
         } else {
             return is_asym_parameter_up_to_date_;
         }
     }
 
-    template <bool sym> std::vector<MathSolver<sym>>& get_solvers() {
-        if constexpr (sym) {
+    template <symmetry_tag sym> std::vector<MathSolver<sym>>& get_solvers() {
+        if constexpr (is_symmetric_v<sym>) {
             return math_state_.math_solvers_sym;
         } else {
             return math_state_.math_solvers_asym;
         }
     }
 
-    template <bool sym> std::vector<YBus<sym>>& get_y_bus() {
-        if constexpr (sym) {
+    template <symmetry_tag sym> std::vector<YBus<sym>>& get_y_bus() {
+        if constexpr (is_symmetric_v<sym>) {
             return math_state_.y_bus_vec_sym;
         } else {
             return math_state_.y_bus_vec_asym;
         }
     }
 
     void rebuild_topology() {
@@ -870,15 +871,15 @@
         std::tie(state_.math_topology, state_.topo_comp_coup) = topology.build_topology();
         n_math_solvers_ = static_cast<Idx>(state_.math_topology.size());
         is_topology_up_to_date_ = true;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
     }
 
-    template <bool sym> std::vector<MathModelParam<sym>> get_math_param() {
+    template <symmetry_tag sym> std::vector<MathModelParam<sym>> get_math_param() {
         std::vector<MathModelParam<sym>> math_param(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             math_param[i].branch_param.resize(state_.math_topology[i]->n_branch());
             math_param[i].shunt_param.resize(state_.math_topology[i]->n_shunt());
             math_param[i].source_param.resize(state_.math_topology[i]->n_source());
         }
         // loop all branch
@@ -922,15 +923,15 @@
             }
             // assign parameters
             math_param[math_idx.group].source_param[math_idx.pos] =
                 state_.components.template get_item_by_seq<Source>(i).template math_param<sym>();
         }
         return math_param;
     }
-    template <bool sym> std::vector<MathModelParamIncrement> get_math_param_increment() {
+    template <symmetry_tag sym> std::vector<MathModelParamIncrement> get_math_param_increment() {
         using AddToIncrement = void (*)(std::vector<MathModelParamIncrement>&, MainModelState const&, Idx2D const&);
 
         static constexpr std::array<AddToIncrement, n_types> add_to_increments{
             [](std::vector<MathModelParamIncrement>& increments, MainModelState const& state,
                Idx2D const& changed_component_idx) {
                 if constexpr (std::derived_from<ComponentType, Branch>) {
                     Idx2D const math_idx =
@@ -1074,34 +1075,33 @@
     {
         return c.calc_param(extra_args...);
     }
 
     template <calculation_input_type CalcInputType>
     auto calculate_param(auto const& c, auto const&... extra_args)
         requires requires {
-                     { c.template calc_param<symmetric_calculation_input_type<CalcInputType>>(extra_args...) };
+                     { c.template calc_param<typename CalcInputType::sym>(extra_args...) };
                  }
     {
-        static constexpr bool sym{symmetric_calculation_input_type<CalcInputType>};
-        return c.template calc_param<sym>(extra_args...);
+        return c.template calc_param<typename CalcInputType::sym>(extra_args...);
     }
 
-    template <bool sym, IntSVector(StateEstimationInput<sym>::*component), class Component>
+    template <symmetry_tag sym, IntSVector(StateEstimationInput<sym>::*component), class Component>
     void prepare_input_status(std::vector<Idx2D> const& objects, std::vector<StateEstimationInput<sym>>& input) {
         for (Idx i = 0, n = (Idx)objects.size(); i != n; ++i) {
             Idx2D const math_idx = objects[i];
             if (math_idx.group == -1) {
                 continue;
             }
             (input[math_idx.group].*component)[math_idx.pos] =
                 state_.components.template get_item_by_seq<Component>(i).status();
         }
     }
 
-    template <bool sym> std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
+    template <symmetry_tag sym> std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
         std::vector<PowerFlowInput<sym>> pf_input(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             pf_input[i].s_injection.resize(state_.math_topology[i]->n_load_gen());
             pf_input[i].source.resize(state_.math_topology[i]->n_source());
         }
         prepare_input<PowerFlowInput<sym>, DoubleComplex, &PowerFlowInput<sym>::source, Source>(
@@ -1109,15 +1109,15 @@
 
         prepare_input<PowerFlowInput<sym>, ComplexValue<sym>, &PowerFlowInput<sym>::s_injection, GenericLoadGen>(
             state_.topo_comp_coup->load_gen, pf_input);
 
         return pf_input;
     }
 
-    template <bool sym> std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
+    template <symmetry_tag sym> std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
 
         std::vector<StateEstimationInput<sym>> se_input(n_math_solvers_);
 
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             se_input[i].shunt_status.resize(state_.math_topology[i]->n_shunt());
             se_input[i].load_gen_status.resize(state_.math_topology[i]->n_load_gen());
@@ -1173,15 +1173,15 @@
                       &StateEstimationInput<sym>::measured_bus_injection, GenericPowerSensor>(
             state_.topo_comp_coup->power_sensor, se_input,
             [this](Idx i) { return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::node; });
 
         return se_input;
     }
 
-    template <bool sym>
+    template <symmetry_tag sym>
     std::vector<ShortCircuitInput> prepare_short_circuit_input(ShortCircuitVoltageScaling voltage_scaling) {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
 
         std::vector<IdxVector> topo_fault_indices(state_.math_topology.size());
         std::vector<IdxVector> topo_bus_indices(state_.math_topology.size());
 
         for (Idx fault_idx{0}; fault_idx < state_.components.template size<Fault>(); ++fault_idx) {
@@ -1222,18 +1222,18 @@
             state_.topo_comp_coup->source, sc_input, [this, voltage_scaling](Source const& source) {
                 return std::pair{state_.components.template get_item<Node>(source.node()).u_rated(), voltage_scaling};
             });
 
         return sc_input;
     }
 
-    template <bool sym> void prepare_y_bus() {
+    template <symmetry_tag sym> void prepare_y_bus() {
         std::vector<YBus<sym>>& y_bus_vec = get_y_bus<sym>();
         // also get the vector of other Y_bus (sym -> asym, or asym -> sym)
-        std::vector<YBus<!sym>>& other_y_bus_vec = get_y_bus<!sym>();
+        std::vector<YBus<other_symmetry_t<sym>>>& other_y_bus_vec = get_y_bus<other_symmetry_t<sym>>();
         // If no Ybus exists, build them
         if (y_bus_vec.empty()) {
             bool const other_y_bus_exist = (!other_y_bus_vec.empty());
             y_bus_vec.reserve(n_math_solvers_);
             auto math_params = get_math_param<sym>();
 
             // Check the branch and shunt indices
@@ -1257,15 +1257,15 @@
                     IdxVector{branch_param_in_seq_map.begin(), branch_param_in_seq_map.end()});
                 y_bus_vec.back().set_shunt_param_idx(
                     IdxVector{shunt_param_in_seq_map.begin(), shunt_param_in_seq_map.end()});
             }
         }
     }
 
-    template <bool sym> void prepare_solvers() {
+    template <symmetry_tag sym> void prepare_solvers() {
         std::vector<MathSolver<sym>>& solvers = get_solvers<sym>();
         // rebuild topology if needed
         if (!is_topology_up_to_date_) {
             rebuild_topology();
         }
         prepare_y_bus<sym>();
 
@@ -1281,24 +1281,24 @@
             for (Idx idx = 0; idx < n_math_solvers_; ++idx) {
                 get_y_bus<sym>()[idx].register_parameters_changed_callback(
                     [solver = std::ref(solvers[idx])](bool changed) { solver.get().parameters_changed(changed); });
             }
         } else if (!is_parameter_up_to_date<sym>()) {
             std::vector<MathModelParam<sym>> const math_params = get_math_param<sym>();
             std::vector<MathModelParamIncrement> const math_param_increments = get_math_param_increment<sym>();
-            if (last_updated_calculation_symmetry_mode_ == sym) {
+            if (last_updated_calculation_symmetry_mode_ == is_symmetric_v<sym>) {
                 main_core::update_y_bus(math_state_, math_params, math_param_increments);
             } else {
                 main_core::update_y_bus(math_state_, math_params);
             }
         }
         // else do nothing, set everything up to date
         is_parameter_up_to_date<sym>() = true;
         std::ranges::for_each(parameter_changed_components_, [](auto& comps) { comps.clear(); });
-        last_updated_calculation_symmetry_mode_ = sym;
+        last_updated_calculation_symmetry_mode_ = is_symmetric_v<sym>;
     }
 };
 
 using MainModel =
     MainModelImpl<ExtraRetrievableTypes<Base, Node, Branch, Branch3, Appliance, GenericLoadGen, GenericLoad,
                                         GenericGenerator, GenericPowerSensor, GenericVoltageSensor>,
                   AllComponents>;
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 // the name of block matrix getter can be overwritten by sub matrix
 
 #include "../common/common.hpp"
 #include "../common/three_phase_tensor.hpp"
 
 namespace power_grid_model::math_solver {
 
-template <scalar_value T, bool sym, bool is_tensor, int n_sub_block> struct block_trait {
-    static constexpr int sub_block_size = sym ? 1 : 3;
+template <scalar_value T, symmetry_tag sym, bool is_tensor, int n_sub_block> struct block_trait {
+    static constexpr int sub_block_size = is_symmetric_v<sym> ? 1 : 3;
     static constexpr int n_row = n_sub_block * sub_block_size;
     static constexpr int n_col = is_tensor ? n_sub_block * sub_block_size : 1;
 
     using ArrayType = Eigen::Array<T, n_row, n_col, Eigen::ColMajor>;
 };
 
-template <class T, bool sym, bool is_tensor, int n_sub_block>
+template <class T, symmetry_tag sym, bool is_tensor, int n_sub_block>
 class Block : public block_trait<T, sym, is_tensor, n_sub_block>::ArrayType {
   public:
     using block_traits = block_trait<T, sym, is_tensor, n_sub_block>;
     using ArrayType = typename block_traits::ArrayType;
     using ArrayType::operator();
 
     // default zero
@@ -57,19 +57,19 @@
             return Block::get_sequence<c, c_size, block_traits::n_col>();
         }
     }
     template <int r> static auto get_row_idx() { return Block::get_block_row_idx<r, 1>(); }
     template <int c> static auto get_col_idx() { return Block::get_block_col_idx<c, 1>(); }
 
     template <int r, int c>
-    using GetterType =
-        std::conditional_t<sym, T&, decltype(std::declval<ArrayType>()(get_row_idx<r>(), get_col_idx<c>()))>;
+    using GetterType = std::conditional_t<is_symmetric_v<sym>, T&,
+                                          decltype(std::declval<ArrayType>()(get_row_idx<r>(), get_col_idx<c>()))>;
 
     template <int r, int c> GetterType<r, c> get_val() {
-        if constexpr (sym) {
+        if constexpr (is_symmetric_v<sym>) {
             return (*this)(r, c);
         } else {
             return (*this)(get_row_idx<r>(), get_col_idx<c>());
         }
     }
 
     template <int r, int c, int r_size, int c_size>
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/common_solver_functions.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/common_solver_functions.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -8,47 +8,47 @@
 #include "y_bus.hpp"
 
 #include "../calculation_parameters.hpp"
 #include "../common/exception.hpp"
 
 namespace power_grid_model::math_solver::detail {
 
-template <bool sym>
+template <symmetry_tag sym>
 inline void add_sources(IdxRange const& sources, Idx /* bus_number */, YBus<sym> const& y_bus,
                         ComplexVector const& u_source_vector, ComplexTensor<sym>& diagonal_element,
                         ComplexValue<sym>& u_bus) {
     for (Idx const source_number : sources) {
         ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
         diagonal_element += y_source; // add y_source to the diagonal of Ybus
         u_bus += dot(y_source, ComplexValue<sym>{u_source_vector[source_number]}); // rhs += Y_source * U_source
     }
 }
 
-template <bool sym> inline void copy_y_bus(YBus<sym> const& y_bus, ComplexTensorVector<sym>& mat_data) {
+template <symmetry_tag sym> inline void copy_y_bus(YBus<sym> const& y_bus, ComplexTensorVector<sym>& mat_data) {
     ComplexTensorVector<sym> const& ydata = y_bus.admittance();
     std::transform(y_bus.map_lu_y_bus().cbegin(), y_bus.map_lu_y_bus().cend(), mat_data.begin(), [&](Idx k) {
         if (k == -1) {
             return ComplexTensor<sym>{};
         }
         return ydata[k];
     });
 }
 
-template <bool sym>
+template <symmetry_tag sym>
 inline void calculate_source_result(IdxRange const& sources, Idx bus_number, YBus<sym> const& y_bus,
                                     PowerFlowInput<sym> const& input, MathOutput<sym>& output) {
     for (Idx const source : sources) {
         ComplexValue<sym> const u_ref{input.source[source]};
         ComplexTensor<sym> const y_ref = y_bus.math_model_param().source_param[source];
         output.source[source].i = dot(y_ref, u_ref - output.u[bus_number]);
         output.source[source].s = output.u[bus_number] * conj(output.source[source].i);
     }
 }
 
-template <bool sym, class LoadGenFunc>
+template <symmetry_tag sym, class LoadGenFunc>
     requires std::invocable<std::remove_cvref_t<LoadGenFunc>, Idx> &&
              std::same_as<std::invoke_result_t<LoadGenFunc, Idx>, LoadGenType>
 inline void calculate_load_gen_result(IdxRange const& load_gens, Idx bus_number, PowerFlowInput<sym> const& input,
                                       MathOutput<sym>& output, LoadGenFunc&& load_gen_func) {
     for (Idx const load_gen : load_gens) {
         switch (LoadGenType const type = load_gen_func(load_gen); type) {
             using enum LoadGenType;
@@ -68,15 +68,15 @@
         default:
             throw MissingCaseForEnumError("Power injection", type);
         }
         output.load_gen[load_gen].i = conj(output.load_gen[load_gen].s / output.u[bus_number]);
     }
 }
 
-template <bool sym, typename LoadGenFunc>
+template <symmetry_tag sym, typename LoadGenFunc>
     requires std::invocable<std::remove_cvref_t<LoadGenFunc>, Idx> &&
              std::same_as<std::invoke_result_t<LoadGenFunc, Idx>, LoadGenType>
 inline void calculate_pf_result(YBus<sym> const& y_bus, PowerFlowInput<sym> const& input,
                                 grouped_idx_vector_type auto const& sources_per_bus,
                                 grouped_idx_vector_type auto const& load_gens_per_bus, MathOutput<sym>& output,
                                 LoadGenFunc&& load_gen_func) {
     assert(sources_per_bus.size() == load_gens_per_bus.size());
@@ -93,15 +93,15 @@
     for (auto const& [bus_number, sources, load_gens] : enumerated_zip_sequence(sources_per_bus, load_gens_per_bus)) {
         calculate_source_result<sym>(sources, bus_number, y_bus, input, output);
         calculate_load_gen_result<sym>(load_gens, bus_number, input, output, load_gen_func);
     }
     output.bus_injection = y_bus.calculate_injection(output.u);
 }
 
-template <bool sym>
+template <symmetry_tag sym>
 inline void calculate_se_result(YBus<sym> const& y_bus, MeasuredValues<sym> const& measured_value,
                                 MathOutput<sym>& output) {
     // call y bus
     output.branch = y_bus.template calculate_branch_flow<BranchMathOutput<sym>>(output.u);
     output.shunt = y_bus.template calculate_shunt_flow<ApplianceMathOutput<sym>>(output.u);
     output.bus_injection = y_bus.calculate_injection(output.u);
     std::tie(output.load_gen, output.source) = measured_value.calculate_load_gen_source(output.u, output.bus_injection);
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
 namespace power_grid_model::math_solver {
 
 // hide implementation in inside namespace
 namespace iterative_current_pf {
 
 // solver
-template <bool sym> class IterativeCurrentPFSolver : public IterativePFSolver<sym, IterativeCurrentPFSolver<sym>> {
+template <symmetry_tag sym>
+class IterativeCurrentPFSolver : public IterativePFSolver<sym, IterativeCurrentPFSolver<sym>> {
   public:
     using BlockPermArray =
         typename SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>>::BlockPermArray;
 
     IterativeCurrentPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : IterativePFSolver<sym, IterativeCurrentPFSolver>{y_bus, topo_ptr},
           rhs_u_(y_bus.size()),
@@ -184,15 +185,15 @@
             // I_inj_i += Y_source_j * U_ref_j
             rhs_u_[bus_number] += dot(y_bus.math_model_param().source_param[source_number],
                                       ComplexValue<sym>{input.source[source_number]});
         }
     }
 };
 
-template class IterativeCurrentPFSolver<true>;
-template class IterativeCurrentPFSolver<false>;
+template class IterativeCurrentPFSolver<symmetric_t>;
+template class IterativeCurrentPFSolver<asymmetric_t>;
 
 } // namespace iterative_current_pf
 
 using iterative_current_pf::IterativeCurrentPFSolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,53 @@
 
 namespace power_grid_model::math_solver {
 
 // hide implementation in inside namespace
 namespace iterative_linear_se {
 
 // block class for the unknown vector and/or right-hand side in state estimation equation
-template <bool sym> struct ILSEUnknown : public Block<DoubleComplex, sym, false, 2> {
+template <symmetry_tag sym> struct ILSEUnknown : public Block<DoubleComplex, sym, false, 2> {
     template <int r, int c> using GetterType = typename Block<DoubleComplex, sym, false, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<DoubleComplex, sym, false, 2>::Block;
     using Block<DoubleComplex, sym, false, 2>::operator=;
 
     GetterType<0, 0> u() { return this->template get_val<0, 0>(); }
     GetterType<1, 0> phi() { return this->template get_val<1, 0>(); }
 
     GetterType<0, 0> eta() { return this->template get_val<0, 0>(); }
     GetterType<1, 0> tau() { return this->template get_val<1, 0>(); }
 };
 
 // block class for the right hand side in state estimation equation
-template <bool sym> using ILSERhs = ILSEUnknown<sym>;
+template <symmetry_tag sym> using ILSERhs = ILSEUnknown<sym>;
 
 // class of 2*2 (6*6) se gain block
 // [
 //    [G, QH]
 //    [Q, R ]
 // ]
-template <bool sym> class ILSEGainBlock : public Block<DoubleComplex, sym, true, 2> {
+template <symmetry_tag sym> class ILSEGainBlock : public Block<DoubleComplex, sym, true, 2> {
   public:
     template <int r, int c> using GetterType = typename Block<DoubleComplex, sym, true, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<DoubleComplex, sym, true, 2>::Block;
     using Block<DoubleComplex, sym, true, 2>::operator=;
 
     GetterType<0, 0> g() { return this->template get_val<0, 0>(); }
     GetterType<0, 1> qh() { return this->template get_val<0, 1>(); }
     GetterType<1, 0> q() { return this->template get_val<1, 0>(); }
     GetterType<1, 1> r() { return this->template get_val<1, 1>(); }
 };
 
-template <bool sym> class IterativeLinearSESolver {
+template <symmetry_tag sym> class IterativeLinearSESolver {
     // block size 2 for symmetric, 6 for asym
-    static constexpr Idx bsr_block_size_ = sym ? 2 : 6;
+    static constexpr Idx bsr_block_size_ = is_symmetric_v<sym> ? 2 : 6;
 
   public:
     IterativeLinearSESolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> topo_ptr)
         : n_bus_{y_bus.size()},
           math_topo_{std::move(topo_ptr)},
           data_gain_(y_bus.nnz_lu()),
           x_rhs_(y_bus.size()),
@@ -316,15 +316,15 @@
         // if no angle measurement is present
         DoubleComplex const angle_offset = [&]() -> DoubleComplex {
             if (has_angle) {
                 return 1.0;
             }
             auto const& voltage = x_rhs_[math_topo_->slack_bus].u();
             auto const& voltage_a = [&voltage]() -> auto const& {
-                if constexpr (sym) {
+                if constexpr (is_symmetric_v<sym>) {
                     return voltage;
                 } else {
                     return voltage(0);
                 }
             }
             ();
             return cabs(voltage_a) / voltage_a;
@@ -343,15 +343,15 @@
     }
 
     auto linearize_measurements(ComplexValueVector<sym> const& current_u, MeasuredValues<sym> const& measured_values) {
         return measured_values.combine_voltage_iteration_with_measurements(current_u);
     }
 };
 
-template class IterativeLinearSESolver<true>;
-template class IterativeLinearSESolver<false>;
+template class IterativeLinearSESolver<symmetric_t>;
+template class IterativeLinearSESolver<asymmetric_t>;
 
 } // namespace iterative_linear_se
 
 using iterative_linear_se::IterativeLinearSESolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #include "../common/exception.hpp"
 #include "../common/three_phase_tensor.hpp"
 #include "../common/timer.hpp"
 
 namespace power_grid_model::math_solver {
 
 // solver
-template <bool sym, typename DerivedSolver> class IterativePFSolver {
+template <symmetry_tag sym, typename DerivedSolver> class IterativePFSolver {
   public:
     friend DerivedSolver;
     MathOutput<sym> run_power_flow(YBus<sym> const& y_bus, PowerFlowInput<sym> const& input, double err_tol,
                                    Idx max_iter, CalculationInfo& calculation_info) {
         // get derived reference for derived solver class
         auto derived_solver = static_cast<DerivedSolver&>(*this);
         std::vector<double> const& phase_shift = *phase_shift_;
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #include "../common/three_phase_tensor.hpp"
 #include "../common/timer.hpp"
 
 namespace power_grid_model::math_solver {
 
 namespace linear_pf {
 
-template <bool sym> class LinearPFSolver {
+template <symmetry_tag sym> class LinearPFSolver {
 
   public:
     LinearPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           load_gens_per_bus_{topo_ptr, &topo_ptr->load_gens_per_bus},
           sources_per_bus_{topo_ptr, &topo_ptr->sources_per_bus},
           mat_data_(y_bus.nnz_lu()),
@@ -114,14 +114,14 @@
 
     void calculate_result(YBus<sym> const& y_bus, PowerFlowInput<sym> const& input, MathOutput<sym>& output) {
         detail::calculate_pf_result(y_bus, input, *sources_per_bus_, *load_gens_per_bus_, output,
                                     [](Idx /*i*/) { return LoadGenType::const_y; });
     }
 };
 
-template class LinearPFSolver<true>;
-template class LinearPFSolver<false>;
+template class LinearPFSolver<symmetric_t>;
+template class LinearPFSolver<asymmetric_t>;
 } // namespace linear_pf
 
 using linear_pf::LinearPFSolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 #include <optional>
 
 namespace power_grid_model {
 
 namespace math_solver {
 
-template <bool sym> class MathSolver {
+template <symmetry_tag sym> class MathSolver {
   public:
     explicit MathSolver(std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : topo_ptr_{topo_ptr},
           all_const_y_{std::all_of(topo_ptr->load_gen_type.cbegin(), topo_ptr->load_gen_type.cend(),
                                    [](LoadGenType x) { return x == LoadGenType::const_y; })} {}
 
     MathOutput<sym> run_power_flow(PowerFlowInput<sym> const& input, double err_tol, Idx max_iter,
@@ -171,14 +171,14 @@
 
         // call calculation
         return newton_raphson_se_solver_.value().run_state_estimation(y_bus, input, err_tol, max_iter,
                                                                       calculation_info);
     }
 };
 
-template class MathSolver<true>;
-template class MathSolver<false>;
+template class MathSolver<symmetric_t>;
+template class MathSolver<asymmetric_t>;
 } // namespace math_solver
 
 using math_solver::MathSolver;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/measured_values.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/measured_values.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 #include "../common/three_phase_tensor.hpp"
 
 #include <memory>
 
 namespace power_grid_model::math_solver {
 
 namespace detail {
-template <bool sym> inline RealValue<sym> cabs_or_real(ComplexValue<sym> const& value) {
+template <symmetry_tag sym> inline RealValue<sym> cabs_or_real(ComplexValue<sym> const& value) {
     if (is_nan(imag(value))) {
         return real(value); // only keep real part
     }
     return cabs(value); // get abs of the value
 }
 } // namespace detail
 
 // processed measurement struct
 // combined all measurement of the same quantity
 // accumulate for bus injection measurement
-template <bool sym> class MeasuredValues {
+template <symmetry_tag sym> class MeasuredValues {
     static constexpr Idx disconnected = -1;
     static constexpr Idx unmeasured = -2;
     static constexpr Idx undefined = -3;
 
     // struct to store bus injection information
     struct BusInjection {
         // The index in main_value_ where the total measured bus injection is stored.
@@ -531,15 +531,15 @@
             }
         };
         for (auto const& x : voltage_main_value_) {
             unconstrained_min(x.variance);
         }
         for (auto const& x : power_main_value_) {
             auto const variance = x.p_variance + x.q_variance;
-            if constexpr (sym) {
+            if constexpr (is_symmetric_v<sym>) {
                 unconstrained_min(variance);
             } else {
                 for (Idx const phase : {0, 1, 2}) {
                     unconstrained_min(variance[phase]);
                 }
             }
         }
@@ -600,10 +600,10 @@
             if (has_source(source)) {
                 source_flow[source].s = calculate_injection(source_power(source));
             }
         }
     }
 };
 
-template class MeasuredValues<true>;
-template class MeasuredValues<false>;
+template class MeasuredValues<symmetric_t>;
+template class MeasuredValues<asymmetric_t>;
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -157,54 +157,54 @@
 
 namespace power_grid_model::math_solver {
 
 // hide implementation in inside namespace
 namespace newton_raphson_pf {
 
 // class for phasor in polar coordinate and/or complex power
-template <bool sym> struct PolarPhasor : public Block<double, sym, false, 2> {
+template <symmetry_tag sym> struct PolarPhasor : public Block<double, sym, false, 2> {
     template <int r, int c> using GetterType = typename Block<double, sym, false, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<double, sym, false, 2>::Block;
     using Block<double, sym, false, 2>::operator=;
 
     GetterType<0, 0> theta() { return this->template get_val<0, 0>(); }
     GetterType<1, 0> v() { return this->template get_val<1, 0>(); }
 
     GetterType<0, 0> p() { return this->template get_val<0, 0>(); }
     GetterType<1, 0> q() { return this->template get_val<1, 0>(); }
 };
 
 // class for complex power
-template <bool sym> using ComplexPower = PolarPhasor<sym>;
+template <symmetry_tag sym> using ComplexPower = PolarPhasor<sym>;
 
 // class of pf block
 // block of incomplete power flow jacobian
 // non-diagonal H, N, M, L
 // [ [H = dP/dTheta, N = V * dP/dV],
 // [M = dQ/dTheta = -N, L = V * dQ/dV = H] ]
 // Hij = Gij .* sij - Bij .* cij = L
 // Nij = Gij .* cij + Bij .* sij = -M
-template <bool sym> class PFJacBlock : public Block<double, sym, true, 2> {
+template <symmetry_tag sym> class PFJacBlock : public Block<double, sym, true, 2> {
   public:
     template <int r, int c> using GetterType = typename Block<double, sym, true, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<double, sym, true, 2>::Block;
     using Block<double, sym, true, 2>::operator=;
 
     GetterType<0, 0> h() { return this->template get_val<0, 0>(); }
     GetterType<0, 1> n() { return this->template get_val<0, 1>(); }
     GetterType<1, 0> m() { return this->template get_val<1, 0>(); }
     GetterType<1, 1> l() { return this->template get_val<1, 1>(); }
 };
 
 // solver
-template <bool sym> class NewtonRaphsonPFSolver : public IterativePFSolver<sym, NewtonRaphsonPFSolver<sym>> {
+template <symmetry_tag sym> class NewtonRaphsonPFSolver : public IterativePFSolver<sym, NewtonRaphsonPFSolver<sym>> {
   public:
     NewtonRaphsonPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : IterativePFSolver<sym, NewtonRaphsonPFSolver>{y_bus, topo_ptr},
           data_jac_(y_bus.nnz_lu()),
           x_(y_bus.size()),
           del_x_pq_(y_bus.size()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
@@ -269,40 +269,28 @@
     // 2. power unbalance: p/q_specified - p/q_calculated
     // 3. unknown iterative
     std::vector<ComplexPower<sym>> del_x_pq_;
     SparseLUSolver<PFJacBlock<sym>, ComplexPower<sym>, PolarPhasor<sym>> sparse_solver_;
     // permutation array
     typename SparseLUSolver<PFJacBlock<sym>, ComplexPower<sym>, PolarPhasor<sym>>::BlockPermArray perm_;
 
+    /// @brief power_flow_ij = (ui @* conj(uj))  .* conj(yij)
+    /// Hij = diag(Vi) * ( Gij .* sin(theta_ij) - Bij .* cos(theta_ij) ) * diag(Vj)
+    /// = imaginary(power_flow_ij)
+    /// Nij = diag(Vi) * ( Gij .* cos(theta_ij) + Bij .* sin(theta_ij) ) * diag(Vj)
+    /// = real(power_flow_ij)
+    /// Mij = -Nij
+    /// Lij = Hij
     static PFJacBlock<sym> calculate_hnml(ComplexTensor<sym> const& yij, ComplexValue<sym> const& ui,
                                           ComplexValue<sym> const& uj) {
         PFJacBlock<sym> block{};
-        // real and imag of addmittance
-        RealTensor<sym> const gij = real(yij);
-        RealTensor<sym> const bij = imag(yij);
-        // diag(Vi) * cos(theta_ij) * diag(Vj)
-        // Ui_r @* Uj_r + Ui_i @* Uj_i
-        // = cij
-        RealTensor<sym> const c_ij =
-            vector_outer_product(real(ui), real(uj)) + vector_outer_product(imag(ui), imag(uj));
-        // diag(Vi) * sin(theta_ij) * diag(Vj)
-        // = Ui_i @* Uj_r - Ui_r @* Uj_i
-        // = sij
-        RealTensor<sym> const s_ij =
-            vector_outer_product(imag(ui), real(uj)) - vector_outer_product(real(ui), imag(uj));
-        // calculate H, N, M, L
-        // Hij = diag(Vi) * ( Gij .* sin(theta_ij) - Bij .* cos(theta_ij) ) * diag(Vj)
-        // = Gij .* sij - Bij .* cij
-        block.h() = gij * s_ij - bij * c_ij;
-        // Nij = diag(Vi) * ( Gij .* cos(Theta_ij) + Bij .* sin(Theta_ij) ) * diag(Vj)
-        // = Gij .* cij + Bij .* sij
-        block.n() = gij * c_ij + bij * s_ij;
-        // Mij = - Nij
+        ComplexTensor<sym> const power_flow_ij = vector_outer_product(ui, conj(uj)) * conj(yij);
+        block.h() = imag(power_flow_ij);
+        block.n() = real(power_flow_ij);
         block.m() = -block.n();
-        // Lij = Hij
         block.l() = block.h();
         return block;
     }
 
     void prepare_matrix_and_rhs_from_network_perspective(YBus<sym> const& y_bus, ComplexValueVector<sym> const& u,
                                                          IdxVector const& bus_entry) {
         IdxVector const& indptr = y_bus.row_indptr_lu();
@@ -426,15 +414,15 @@
             data_jac_[diagonal_position].n() += block_mm.n();
             data_jac_[diagonal_position].m() += block_mm.m();
             data_jac_[diagonal_position].l() += block_mm.l();
         }
     }
 };
 
-template class NewtonRaphsonPFSolver<true>;
-template class NewtonRaphsonPFSolver<false>;
+template class NewtonRaphsonPFSolver<symmetric_t>;
+template class NewtonRaphsonPFSolver<asymmetric_t>;
 
 } // namespace newton_raphson_pf
 
 using newton_raphson_pf::NewtonRaphsonPFSolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_se_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_se_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 namespace power_grid_model::math_solver {
 
 // hide implementation in inside namespace
 namespace newton_raphson_se {
 
 // block class for the unknown vector and/or right-hand side in state estimation equation
-template <bool sym> struct NRSEUnknown : public Block<double, sym, false, 4> {
+template <symmetry_tag sym> struct NRSEUnknown : public Block<double, sym, false, 4> {
     template <int r, int c> using GetterType = typename Block<double, sym, false, 4>::template GetterType<r, c>;
 
     // eigen expression
     using Block<double, sym, false, 4>::Block;
     using Block<double, sym, false, 4>::operator=;
 
     GetterType<0, 0> theta() { return this->template get_val<0, 0>(); }
@@ -36,22 +36,22 @@
     GetterType<0, 0> eta_theta() { return this->template get_val<0, 0>(); }
     GetterType<1, 0> eta_v() { return this->template get_val<1, 0>(); }
     GetterType<2, 0> tau_p() { return this->template get_val<2, 0>(); }
     GetterType<3, 0> tau_q() { return this->template get_val<3, 0>(); }
 };
 
 // block class for the right hand side in state estimation equation
-template <bool sym> using NRSERhs = NRSEUnknown<sym>;
+template <symmetry_tag sym> using NRSERhs = NRSEUnknown<sym>;
 
 // class of 4*4 (12*12) se gain block
 // [
 //    [G, Q^T]
 //    [Q, R  ]
 // ]
-template <bool sym> class NRSEGainBlock : public Block<double, sym, true, 4> {
+template <symmetry_tag sym> class NRSEGainBlock : public Block<double, sym, true, 4> {
   public:
     template <int r, int c> using GetterType = typename Block<double, sym, true, 4>::template GetterType<r, c>;
     template <int r, int c, int r_size, int c_size>
     using BlockGetterType = typename Block<double, sym, true, 4>::template BlockGetterType<r, c, r_size, c_size>;
 
     // eigen expression
     using Block<double, sym, true, 4>::Block;
@@ -81,15 +81,15 @@
     BlockGetterType<0, 0, 2, 2> g() { return this->template get_block_val<0, 0, 2, 2>(); }
     BlockGetterType<0, 1, 2, 2> qt() { return this->template get_block_val<0, 1, 2, 2>(); }
     BlockGetterType<1, 0, 2, 2> q() { return this->template get_block_val<1, 0, 2, 2>(); }
     BlockGetterType<1, 1, 2, 2> r() { return this->template get_block_val<1, 1, 2, 2>(); }
 };
 
 // solver
-template <bool sym> class NewtonRaphsonSESolver {
+template <symmetry_tag sym> class NewtonRaphsonSESolver {
     enum class Order { row_major = 0, column_major = 1 };
 
     struct NRSEVoltageState {
         ComplexTensor<sym> ui_ui_conj{};
         ComplexTensor<sym> uj_uj_conj{};
         ComplexTensor<sym> ui_uj_conj{};
         ComplexTensor<sym> uj_ui_conj{};
@@ -649,15 +649,15 @@
         // phase shift anti offset of slack bus, phase a
         // if no angle measurement is present
         double const angle_offset = [&]() -> double {
             if (measured_values.has_angle()) {
                 return 0.0;
             }
             auto const& theta = x_[math_topo_->slack_bus].theta() + delta_x_rhs_[math_topo_->slack_bus].theta();
-            if constexpr (sym) {
+            if constexpr (is_symmetric_v<sym>) {
                 return theta;
             } else {
                 return theta(0);
             }
         }();
 
         for (Idx bus = 0; bus != n_bus_; ++bus) {
@@ -686,15 +686,15 @@
     }
 
     static auto diagonal_inverse(RealValue<sym> const& value) {
         return RealDiagonalTensor<sym>{static_cast<RealValue<sym>>(RealValue<sym>{1.0} / value)};
     }
 };
 
-template class NewtonRaphsonSESolver<true>;
-template class NewtonRaphsonSESolver<false>;
+template class NewtonRaphsonSESolver<symmetric_t>;
+template class NewtonRaphsonSESolver<asymmetric_t>;
 
 } // namespace newton_raphson_se
 
 using newton_raphson_se::NewtonRaphsonSESolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 namespace power_grid_model::math_solver {
 
 // hide implementation in inside namespace
 namespace short_circuit {
 
 // solver
-template <bool sym> class ShortCircuitSolver {
+template <symmetry_tag sym> class ShortCircuitSolver {
     using BlockPermArray =
         typename SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>>::BlockPermArray;
 
   public:
     ShortCircuitSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           n_source_{topo_ptr->n_source()},
@@ -122,15 +122,15 @@
                 // mat_data[:,bus] = 0
                 mat_data_[col_data_index] = ComplexTensor<sym>{0};
             }
             // mat_data[bus,bus] = -1
             diagonal_element = ComplexTensor<sym>{-1};
             u_bus = ComplexValue<sym>{0}; // update rhs
         }
-        if constexpr (!sym) {
+        if constexpr (!is_symmetric_v<sym>) {
             if (fault_type == single_phase_to_ground) {
                 for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                      data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                     Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                     // mat_data[:,bus][:, phase_1] = 0
                     mat_data_[col_data_index].col(phase_1) = 0;
                 }
@@ -180,15 +180,15 @@
                    IntS phase_1, IntS phase_2) {
         using enum FaultType;
 
         if (fault_type == three_phase) { // three phase fault
             // mat_data[bus,bus] += y_fault
             diagonal_element += ComplexTensor<sym>{y_fault};
         }
-        if constexpr (!sym) {
+        if constexpr (!is_symmetric_v<sym>) {
             if (fault_type == single_phase_to_ground) {
                 // mat_data[bus,bus][phase_1, phase_1] += y_fault
                 diagonal_element(phase_1, phase_1) += y_fault;
             } else if (fault_type == two_phase) {
                 // mat_data[bus,bus][phase_1, phase_1] += y_fault
                 // mat_data[bus,bus][phase_2, phase_2] += y_fault
                 // mat_data[bus,bus][phase_1, phase_2] -= y_fault
@@ -241,15 +241,15 @@
                     assert(std::isinf(y_fault.imag()));
                     if (fault_type == three_phase) { // three phase fault
                         i_fault = -1.0 * static_cast<ComplexValue<sym>>(x_bus_subtotal) /
                                   infinite_admittance_fault_counter_bus; // injection is
                                                                          // negative to fault
                         u_bus = ComplexValue<sym>{0.0};
                     }
-                    if constexpr (!sym) {
+                    if constexpr (!is_symmetric_v<sym>) {
                         if (fault_type == single_phase_to_ground) {
                             i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
                             u_bus(phase_1) = 0.0;
                         } else if (fault_type == two_phase) {
                             i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
                             i_fault(phase_2) = -1.0 * i_fault(phase_1);
                             u_bus(phase_2) = u_bus(phase_1);
@@ -269,15 +269,15 @@
                         // ignore fault objects with impedance, when there is a fault with infinite admittance on
                         // bus
                         continue;
                     }
                     if (fault_type == three_phase) { // three phase fault
                         i_fault = static_cast<ComplexValue<sym>>(y_fault * x_bus_subtotal);
                     }
-                    if constexpr (!sym) {
+                    if constexpr (!is_symmetric_v<sym>) {
                         if (fault_type == single_phase_to_ground) {
                             i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1];
                         } else if (fault_type == two_phase) {
                             i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1] - y_fault * x_bus_subtotal[phase_2];
                             i_fault(phase_2) = y_fault * x_bus_subtotal[phase_2] - y_fault * x_bus_subtotal[phase_1];
                         } else if (fault_type == two_phase_to_ground) {
                             i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2];
@@ -309,15 +309,15 @@
                 DoubleComplex const y_fault = input.faults[fault_number].y_fault;
 
                 if (std::isinf(y_fault.real())) {
                     assert(std::isinf(y_fault.imag()));
                     if (fault_type == three_phase) {
                         i_fault += static_cast<ComplexValue<sym>>(i_source_bus / infinite_admittance_fault_counter_bus);
                     }
-                    if constexpr (!sym) {
+                    if constexpr (!is_symmetric_v<sym>) {
                         if (fault_type == single_phase_to_ground) {
                             i_fault(phase_1) += i_source_bus[phase_1] / infinite_admittance_fault_counter_bus;
                         } else if (fault_type == two_phase) {
                             i_fault(phase_1) += i_source_inject[phase_1] / infinite_admittance_fault_counter_bus;
                             // i_inj_1 + i_inj_2 = i_ref_1 + i_ref_2
                             // i_fault_2_p = i_inj_1
                             //      i_fault_2_p is the i_fault_2 status quo after the first fault loop
@@ -332,15 +332,15 @@
                             assert((fault_type == three_phase));
                             continue;
                         }
                     }
                 } else {
                     // compensate for 2 phase to ground fault with impedance
                     assert(!std::isinf(y_fault.imag()));
-                    if constexpr (!sym) {
+                    if constexpr (!is_symmetric_v<sym>) {
                         if ((fault_type == two_phase_to_ground) && (infinite_admittance_fault_counter_bus == 0.0)) {
                             auto const finite_admittance_fault_counter_bus = static_cast<double>(faults.size());
                             // i_inj_1 + i_inj_2 = i_ref_1 + i_ref_2 - u_12 * y_fault
                             // i_fault_2_p = i_inj_1 + u_12 * y_fault
                             //      i_fault_2_p is the i_fault_2 status quo after the first fault loop
                             // i_inj_2 = - i_inj_1 + i_ref_1 + i_ref_2 - u_12 * y_fault
                             // i_fault_2 = i_ref_2 - i_inj_2 = i_ref_2 + i_inj_1 - i_ref_1 - i_ref_2 + u_12 *
@@ -432,15 +432,15 @@
 
         return std::all_of(cbegin(vec), cend(vec), [first = vec.front()](FaultCalcParam const& param) {
             return (param.fault_type == first.fault_type) && (param.fault_phase == first.fault_phase);
         });
     }
 };
 
-template class ShortCircuitSolver<true>;
-template class ShortCircuitSolver<false>;
+template class ShortCircuitSolver<symmetric_t>;
+template class ShortCircuitSolver<asymmetric_t>;
 
 } // namespace short_circuit
 
 using short_circuit::ShortCircuitSolver;
 
 } // namespace power_grid_model::math_solver
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
             lu_transpose_entry[entry_1] = entry_2;
             lu_transpose_entry[entry_2] = entry_1;
         }
     }
 };
 
 // See also "Node Admittance Matrix" in "State Estimation Alliander"
-template <bool sym> class YBus {
+template <symmetry_tag sym> class YBus {
   public:
     using ParamChangedCallback = std::function<void(bool param_changed)>;
 
     YBus(std::shared_ptr<MathModelTopology const> const& topo_ptr,
          std::shared_ptr<MathModelParam<sym> const> const& param,
          std::shared_ptr<YBusStructure const> const& y_bus_struct = {})
         : math_topology_{topo_ptr} {
@@ -538,15 +538,15 @@
     void parameters_changed(bool param_changed) const {
         std::ranges::for_each(parameters_changed_callbacks_, [param_changed](auto const& key_and_callback) {
             key_and_callback.second(param_changed);
         });
     }
 };
 
-template class YBus<true>;
-template class YBus<false>;
+template class YBus<symmetric_t>;
+template class YBus<asymmetric_t>;
 
 } // namespace math_solver
 
 using math_solver::YBus;
 
 } // namespace power_grid_model
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/serialization.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/serialization.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/dataset.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/dataset.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/forward_declarations.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/forward_declarations.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 
 #pragma once
 
 #ifndef PGM_DLL_EXPORTS
 #define PGM_DLL_EXPORTS
 #endif
 
+#include <power_grid_model/auxiliary/dataset_fwd.hpp>
+
 // forward declare all referenced struct/class in C++ core
 // alias them in the root namespace
 
 namespace power_grid_model::meta_data {
 
 struct MetaAttribute;
 struct MetaComponent;
 struct MetaDataset;
 class Serializer;
 class Deserializer;
-template <bool data_mutable, bool indptr_mutable>
-    requires(data_mutable || !indptr_mutable)
-class DatasetHandler;
+
+template <dataset_handler_tag dataset_handler_type> class DatasetHandler;
 
 struct DatasetInfo;
 
 } // namespace power_grid_model::meta_data
 
 using PGM_MetaAttribute = power_grid_model::meta_data::MetaAttribute;
 using PGM_MetaComponent = power_grid_model::meta_data::MetaComponent;
 using PGM_MetaDataset = power_grid_model::meta_data::MetaDataset;
 using PGM_Serializer = power_grid_model::meta_data::Serializer;
 using PGM_Deserializer = power_grid_model::meta_data::Deserializer;
-using PGM_ConstDataset = power_grid_model::meta_data::DatasetHandler<false, false>;
-using PGM_MutableDataset = power_grid_model::meta_data::DatasetHandler<true, false>;
-using PGM_WritableDataset = power_grid_model::meta_data::DatasetHandler<true, true>;
+using PGM_ConstDataset = power_grid_model::meta_data::DatasetHandler<power_grid_model::const_dataset_t>;
+using PGM_MutableDataset = power_grid_model::meta_data::DatasetHandler<power_grid_model::mutable_dataset_t>;
+using PGM_WritableDataset = power_grid_model::meta_data::DatasetHandler<power_grid_model::writable_dataset_t>;
 using PGM_DatasetInfo = power_grid_model::meta_data::DatasetInfo;
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 
 // create model
 PGM_PowerGridModel* PGM_create_model(PGM_Handle* handle, double system_frequency,
                                      PGM_ConstDataset const* input_dataset) {
     return call_with_catch(
         handle,
         [system_frequency, input_dataset] {
-            return new PGM_PowerGridModel{system_frequency, input_dataset->export_dataset<true>(), 0};
+            return new PGM_PowerGridModel{system_frequency, input_dataset->export_dataset<const_dataset_t>(), 0};
         },
         PGM_regular_error);
 }
 
 // update model
 void PGM_update_model(PGM_Handle* handle, PGM_PowerGridModel* model, PGM_ConstDataset const* update_dataset) {
     call_with_catch(
         handle,
         [model, update_dataset] {
-            model->update_component<MainModel::permanent_update_t>(update_dataset->export_dataset<true>());
+            model->update_component<MainModel::permanent_update_t>(update_dataset->export_dataset<const_dataset_t>());
         },
         PGM_regular_error);
 }
 
 // copy model
 PGM_PowerGridModel* PGM_copy_model(PGM_Handle* handle, PGM_PowerGridModel const* model) {
     return call_with_catch(
@@ -66,40 +66,40 @@
     // check dataset integrity
     if ((batch_dataset != nullptr) && (!batch_dataset->is_batch() || !output_dataset->is_batch())) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = "If batch_dataset is provided. Both batch_dataset and output_dataset should be a batch!\n";
         return;
     }
 
-    Dataset const exported_output_dataset = output_dataset->export_dataset<false>();
+    Dataset const exported_output_dataset = output_dataset->export_dataset<mutable_dataset_t>();
     auto const exported_update_dataset =
-        batch_dataset != nullptr ? batch_dataset->export_dataset<true>() : ConstDataset{};
+        batch_dataset != nullptr ? batch_dataset->export_dataset<const_dataset_t>() : ConstDataset{};
 
     // call calculation
     try {
         auto const calculation_method = static_cast<CalculationMethod>(opt->calculation_method);
         switch (opt->calculation_type) {
         case PGM_power_flow:
             if (opt->symmetric != 0) {
-                handle->batch_parameter =
-                    model->calculate_power_flow<true>(opt->err_tol, opt->max_iter, calculation_method,
-                                                      exported_output_dataset, exported_update_dataset, opt->threading);
+                handle->batch_parameter = model->calculate_power_flow<symmetric_t>(
+                    opt->err_tol, opt->max_iter, calculation_method, exported_output_dataset, exported_update_dataset,
+                    opt->threading);
             } else {
-                handle->batch_parameter = model->calculate_power_flow<false>(
+                handle->batch_parameter = model->calculate_power_flow<asymmetric_t>(
                     opt->err_tol, opt->max_iter, calculation_method, exported_output_dataset, exported_update_dataset,
                     opt->threading);
             }
             break;
         case PGM_state_estimation:
             if (opt->symmetric != 0) {
-                handle->batch_parameter = model->calculate_state_estimation<true>(
+                handle->batch_parameter = model->calculate_state_estimation<symmetric_t>(
                     opt->err_tol, opt->max_iter, calculation_method, exported_output_dataset, exported_update_dataset,
                     opt->threading);
             } else {
-                handle->batch_parameter = model->calculate_state_estimation<false>(
+                handle->batch_parameter = model->calculate_state_estimation<asymmetric_t>(
                     opt->err_tol, opt->max_iter, calculation_method, exported_output_dataset, exported_update_dataset,
                     opt->threading);
             }
             break;
         case PGM_short_circuit: {
             auto const short_circuit_voltage_scaling =
                 static_cast<ShortCircuitVoltageScaling>(opt->short_circuit_voltage_scaling);
```

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/power_grid_model_c/power_grid_model_c/src/serialization.cpp` & `power-grid-model-1.7.9/power_grid_model_c/power_grid_model_c/src/serialization.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/pyproject.toml` & `power-grid-model-1.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/setup.py` & `power-grid-model-1.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/__init__.py` & `power-grid-model-1.7.9/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/_utils.py` & `power-grid-model-1.7.9/src/power_grid_model/_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/buffer_handling.py` & `power-grid-model-1.7.9/src/power_grid_model/core/buffer_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.7.9/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.7.9/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/options.py` & `power-grid-model-1.7.9/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.7.9/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_dataset.py` & `power-grid-model-1.7.9/src/power_grid_model/core/power_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.7.9/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.7.9/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/core/serialization.py` & `power-grid-model-1.7.9/src/power_grid_model/core/serialization.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/data_types.py` & `power-grid-model-1.7.9/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/enum.py` & `power-grid-model-1.7.9/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/errors.py` & `power-grid-model-1.7.9/src/power_grid_model/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/utils.py` & `power-grid-model-1.7.9/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/errors.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/rules.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/utils.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model/validation/validation.py` & `power-grid-model-1.7.9/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.7.9/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.7.8a1374103622511
+Version: 1.7.9
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Contributors to the Power Grid Model project <powergridmodel@lfenergy.org>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.7.8a1374103622511/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.7.9/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 power_grid_model_c/power_grid_model/include/power_grid_model/batch_parameter.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/index_mapping.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_fwd.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset_handler.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/gen_getters.hpp
```

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-newton/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-newton/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-batch-shunt/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.7.9/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/multi-source-with-angle/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/multi-source-with-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/single-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/single-transformer/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/single-transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.7.9/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.7.9/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.7.9/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_maximum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/single_phase_to_ground_c_minimum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_maximum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_maximum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/three_phase_c_minimum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/three_phase_c_minimum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_maximum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_maximum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_c_minimum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_c_minimum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_maximum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json` & `power-grid-model-1.7.9/tests/data/short_circuit/two_phase_to_ground_c_minimum/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/high-variance-measurement/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/high-variance-measurement/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/residual-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/residual-test/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/residual-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-il/update_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-il/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/sensor-update-nr/update_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/sensor-update-nr/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/single-line-load-il/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/single-line-load-il/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.7.9/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-iterative-linear/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json` & `power-grid-model-1.7.9/tests/data/state_estimation/unbalanced-power-measurements-newton-raphson/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.7.9/tests/unit/deprecated/data/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/test_end_to_end.py` & `power-grid-model-1.7.9/tests/unit/deprecated/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/deprecated/test_utils.py` & `power-grid-model-1.7.9/tests/unit/deprecated/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.7.9/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_dataset.py` & `power-grid-model-1.7.9/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_error_handling.py` & `power-grid-model-1.7.9/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_internal_utils.py` & `power-grid-model-1.7.9/tests/unit/test_internal_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_meta_data.py` & `power-grid-model-1.7.9/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_power_grid_model.py` & `power-grid-model-1.7.9/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_serialization.py` & `power-grid-model-1.7.9/tests/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/test_utils.py` & `power-grid-model-1.7.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/utils.py` & `power-grid-model-1.7.9/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_assertions.py` & `power-grid-model-1.7.9/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.7.9/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_errors.py` & `power-grid-model-1.7.9/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.7.9/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_rules.py` & `power-grid-model-1.7.9/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_utils.py` & `power-grid-model-1.7.9/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.7.8a1374103622511/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.7.9/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

