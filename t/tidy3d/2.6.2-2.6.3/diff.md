# Comparing `tmp/tidy3d-2.6.2.tar.gz` & `tmp/tidy3d-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.6.2.tar", max compression
+gzip compressed data, was "tidy3d-2.6.3.tar", max compression
```

## Comparing `tidy3d-2.6.2.tar` & `tidy3d-2.6.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0    26526 2024-03-21 23:02:05.342739 tidy3d-2.6.2/LICENSE
--rw-r--r--   0        0        0     4867 2024-03-21 23:02:05.342739 tidy3d-2.6.2/README.md
--rw-r--r--   0        0        0     7560 2024-03-21 23:02:05.394738 tidy3d-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     2978 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/README.md
--rw-r--r--   0        0        0    10818 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/__init__.py
--rw-r--r--   0        0        0     3085 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/__main__.py
--rw-r--r--   0        0        0    10303 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/README.md
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/__init__.py
--rw-r--r--   0        0        0     3228 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/apodization.py
--rw-r--r--   0        0        0    35583 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/data/__init__.py
--rw-r--r--   0        0        0      666 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/data/monitor_data.py
--rw-r--r--   0        0        0     4710 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/data/sim_data.py
--rw-r--r--   0        0        0     3061 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/monitor.py
--rw-r--r--   0        0        0    23738 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/simulation.py
--rw-r--r--   0        0        0      633 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/base_sim/source.py
--rw-r--r--   0        0        0     3211 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/bc_placement.py
--rw-r--r--   0        0        0    33071 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/boundary.py
--rw-r--r--   0        0        0     9733 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/README.md
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/__init__.py
--rw-r--r--   0        0        0    23366 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/data_array.py
--rw-r--r--   0        0        0    58738 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/dataset.py
--rw-r--r--   0        0        0   105026 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/monitor_data.py
--rw-r--r--   0        0        0    31485 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/sim_data.py
--rw-r--r--   0        0        0     2344 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/data/validators.py
--rw-r--r--   0        0        0    38186 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/field_projection.py
--rw-r--r--   0        0        0      823 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/file_util.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/geometry/__init__.py
--rw-r--r--   0        0        0   103970 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/geometry/base.py
--rw-r--r--   0        0        0    17269 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/geometry/mesh.py
--rw-r--r--   0        0        0    62546 2024-03-21 23:02:05.402738 tidy3d-2.6.2/tidy3d/components/geometry/polyslab.py
--rw-r--r--   0        0        0    23375 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/geometry/primitives.py
--rw-r--r--   0        0        0     4013 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/geometry/triangulation.py
--rw-r--r--   0        0        0     7648 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/geometry/utils.py
--rw-r--r--   0        0        0     8383 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/geometry/utils_2d.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/grid/__init__.py
--rw-r--r--   0        0        0    18411 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/grid/grid.py
--rw-r--r--   0        0        0    26013 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0        0        0    50912 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/grid/mesher.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/__init__.py
--rw-r--r--   0        0        0     2340 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/boundary.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/data/__init__.py
--rw-r--r--   0        0        0     3807 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/data/monitor_data.py
--rw-r--r--   0        0        0    10737 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/data/sim_data.py
--rw-r--r--   0        0        0     3871 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/grid.py
--rw-r--r--   0        0        0     1629 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/monitor.py
--rw-r--r--   0        0        0    33781 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/simulation.py
--rw-r--r--   0        0        0     1264 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/source.py
--rw-r--r--   0        0        0      347 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat/viz.py
--rw-r--r--   0        0        0     1135 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/heat_spec.py
--rw-r--r--   0        0        0   208534 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/medium.py
--rw-r--r--   0        0        0     9497 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/mode.py
--rw-r--r--   0        0        0    60116 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/monitor.py
--rw-r--r--   0        0        0    35480 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/parameter_perturbation.py
--rw-r--r--   0        0        0    51297 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/scene.py
--rw-r--r--   0        0        0   167277 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/simulation.py
--rw-r--r--   0        0        0    42331 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/source.py
--rw-r--r--   0        0        0    18017 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/structure.py
--rw-r--r--   0        0        0     7081 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/time.py
--rw-r--r--   0        0        0    10164 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/time_modulation.py
--rw-r--r--   0        0        0     3562 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/transformation.py
--rw-r--r--   0        0        0     7251 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/types.py
--rw-r--r--   0        0        0      362 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/types_extra.py
--rw-r--r--   0        0        0    15102 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/validators.py
--rw-r--r--   0        0        0     8944 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/components/viz.py
--rw-r--r--   0        0        0     1621 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/config.py
--rw-r--r--   0        0        0     2933 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/constants.py
--rw-r--r--   0        0        0     1265 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/exceptions.py
--rw-r--r--   0        0        0    15149 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/log.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.406738 tidy3d-2.6.2/tidy3d/material_library/__init__.py
--rw-r--r--   0        0        0    70598 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/material_library/material_library.py
--rw-r--r--   0        0        0     9498 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/material_library/material_reference.py
--rw-r--r--   0        0        0    15924 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/material_library/parametric_materials.py
--rw-r--r--   0        0        0     5708 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/packaging.py
--rw-r--r--   0        0        0       77 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/__init__.py
--rw-r--r--   0        0        0    33133 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/README.md
--rw-r--r--   0        0        0     1416 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/__init__.py
--rw-r--r--   0        0        0      898 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0        0        0    10610 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/base.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0        0        0    19097 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0        0        0     1049 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0        0        0    18604 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0        0        0    10720 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0        0        0    26055 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0        0        0    16767 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0        0        0    33012 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0        0        0     8591 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0        0        0     2093 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/utils/__init__.py
--rw-r--r--   0        0        0     8126 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/utils/filter.py
--rw-r--r--   0        0        0     9065 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/utils/penalty.py
--rw-r--r--   0        0        0    29641 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/adjoint/web.py
--rw-r--r--   0        0        0     6401 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/README.md
--rw-r--r--   0        0        0      441 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/__init__.py
--rw-r--r--   0        0        0     6596 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/design.py
--rw-r--r--   0        0        0    14172 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/method.py
--rw-r--r--   0        0        0     7087 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/parameter.py
--rw-r--r--   0        0        0    11780 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/design/result.py
--rw-r--r--   0        0        0      366 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0        0        0    22651 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0        0        0    33833 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/dispersion/fit_fast.py
--rw-r--r--   0        0        0      213 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/dispersion/fit_web.py
--rw-r--r--   0        0        0    13282 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/dispersion/web.py
--rw-r--r--   0        0        0     1213 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/LICENSE
--rw-r--r--   0        0        0       42 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/README.md
--rw-r--r--   0        0        0      138 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0        0        0     5733 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0        0        0    41403 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0        0        0    29953 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/solver.py
--rw-r--r--   0        0        0     4370 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/transforms.py
--rw-r--r--   0        0        0       81 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/mode/web.py
--rw-r--r--   0        0        0      116 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0        0        0     2705 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/polyslab/polyslab.py
--rw-r--r--   0        0        0      117 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0        0        0    17644 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/resonance/resonance.py
--rw-r--r--   0        0        0      170 2024-03-21 23:02:05.410738 tidy3d-2.6.2/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0        0        0    20777 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/plugins/smatrix/smatrix.py
--rw-r--r--   0        0        0      129 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0        0        0    36178 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0        0        0   521877 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/schema.json
--rw-r--r--   0        0        0    10908 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/updater.py
--rw-r--r--   0        0        0       87 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/version.py
--rw-r--r--   0        0        0     1083 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/__init__.py
--rw-r--r--   0        0        0     2669 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/asynchronous.py
--rw-r--r--   0        0        0   275233 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/cacert.pem
--rw-r--r--   0        0        0     2284 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/connect_util.py
--rw-r--r--   0        0        0    28268 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/container.py
--rw-r--r--   0        0        0     3792 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/material_fitter.py
--rw-r--r--   0        0        0     1449 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/material_libray.py
--rw-r--r--   0        0        0    18711 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/mode.py
--rw-r--r--   0        0        0     8109 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/tidy3d_stub.py
--rw-r--r--   0        0        0    32481 2024-03-21 23:02:05.414738 tidy3d-2.6.2/tidy3d/web/api/webapi.py
--rw-r--r--   0        0        0       88 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/__init__.py
--rw-r--r--   0        0        0     3491 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/app.py
--rw-r--r--   0        0        0      348 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/constants.py
--rw-r--r--   0        0        0    63715 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/converter.py
--rw-r--r--   0        0        0     1949 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/__init__.py
--rw-r--r--   0        0        0    12380 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/documentation.py
--rw-r--r--   0        0        0      400 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/index.py
--rw-r--r--   0        0        0    15383 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/install.py
--rw-r--r--   0        0        0     4159 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/packaging.py
--rw-r--r--   0        0        0     1961 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/tests.py
--rw-r--r--   0        0        0     1700 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/develop/utils.py
--rw-r--r--   0        0        0     3590 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/migrate.py
--rw-r--r--   0        0        0     3959 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/cli/readme.md
--rw-r--r--   0        0        0       35 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/__init__.py
--rw-r--r--   0        0        0       58 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/cache.py
--rw-r--r--   0        0        0      754 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/constants.py
--rw-r--r--   0        0        0      940 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/core_config.py
--rw-r--r--   0        0        0     4982 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/environment.py
--rw-r--r--   0        0        0      331 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/exceptions.py
--rw-r--r--   0        0        0     2235 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/file_util.py
--rw-r--r--   0        0        0     5917 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/http_util.py
--rw-r--r--   0        0        0    12450 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/s3utils.py
--rw-r--r--   0        0        0     2243 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/stub.py
--rw-r--r--   0        0        0    18838 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/task_core.py
--rw-r--r--   0        0        0     2188 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/task_info.py
--rw-r--r--   0        0        0     1435 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/core/types.py
--rw-r--r--   0        0        0      132 2024-03-21 23:02:05.418738 tidy3d-2.6.2/tidy3d/web/environment.py
--rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 tidy3d-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-02 18:49:48.744887 tidy3d-2.6.3/LICENSE
+-rw-r--r--   0        0        0     4867 2024-04-02 18:49:48.744887 tidy3d-2.6.3/README.md
+-rw-r--r--   0        0        0     7560 2024-04-02 18:49:48.796888 tidy3d-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2978 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/README.md
+-rw-r--r--   0        0        0    10818 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/__init__.py
+-rw-r--r--   0        0        0     3085 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/__main__.py
+-rw-r--r--   0        0        0    10303 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/__init__.py
+-rw-r--r--   0        0        0     3228 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/apodization.py
+-rw-r--r--   0        0        0    35578 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/data/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/data/monitor_data.py
+-rw-r--r--   0        0        0     4710 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/data/sim_data.py
+-rw-r--r--   0        0        0     3061 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/monitor.py
+-rw-r--r--   0        0        0    23738 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/simulation.py
+-rw-r--r--   0        0        0      633 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/base_sim/source.py
+-rw-r--r--   0        0        0     3211 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/bc_placement.py
+-rw-r--r--   0        0        0    33071 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/boundary.py
+-rw-r--r--   0        0        0     9733 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/__init__.py
+-rw-r--r--   0        0        0    23366 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/data_array.py
+-rw-r--r--   0        0        0    58738 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/dataset.py
+-rw-r--r--   0        0        0   105026 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0        0        0    31485 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/sim_data.py
+-rw-r--r--   0        0        0     2344 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/data/validators.py
+-rw-r--r--   0        0        0    38186 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/field_projection.py
+-rw-r--r--   0        0        0      823 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/file_util.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.804888 tidy3d-2.6.3/tidy3d/components/geometry/__init__.py
+-rw-r--r--   0        0        0   103970 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/base.py
+-rw-r--r--   0        0        0    17269 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/mesh.py
+-rw-r--r--   0        0        0    62546 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/polyslab.py
+-rw-r--r--   0        0        0    23375 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/primitives.py
+-rw-r--r--   0        0        0     4013 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/triangulation.py
+-rw-r--r--   0        0        0     7648 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/utils.py
+-rw-r--r--   0        0        0     8383 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/geometry/utils_2d.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/grid/__init__.py
+-rw-r--r--   0        0        0    18411 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/grid/grid.py
+-rw-r--r--   0        0        0    26013 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0        0        0    50912 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/grid/mesher.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/__init__.py
+-rw-r--r--   0        0        0     2340 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/boundary.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/data/__init__.py
+-rw-r--r--   0        0        0     3807 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/data/monitor_data.py
+-rw-r--r--   0        0        0    10737 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/data/sim_data.py
+-rw-r--r--   0        0        0     3871 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/grid.py
+-rw-r--r--   0        0        0     1629 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/monitor.py
+-rw-r--r--   0        0        0    35561 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/simulation.py
+-rw-r--r--   0        0        0     1579 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/source.py
+-rw-r--r--   0        0        0      347 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat/viz.py
+-rw-r--r--   0        0        0     1135 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/heat_spec.py
+-rw-r--r--   0        0        0   208534 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/medium.py
+-rw-r--r--   0        0        0     9497 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/mode.py
+-rw-r--r--   0        0        0    60116 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/monitor.py
+-rw-r--r--   0        0        0    35480 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/parameter_perturbation.py
+-rw-r--r--   0        0        0    51297 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/scene.py
+-rw-r--r--   0        0        0   167277 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/simulation.py
+-rw-r--r--   0        0        0    42331 2024-04-02 18:49:48.808888 tidy3d-2.6.3/tidy3d/components/source.py
+-rw-r--r--   0        0        0    18017 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/structure.py
+-rw-r--r--   0        0        0     7081 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/time.py
+-rw-r--r--   0        0        0    10164 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/time_modulation.py
+-rw-r--r--   0        0        0     3562 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/transformation.py
+-rw-r--r--   0        0        0     7251 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/types.py
+-rw-r--r--   0        0        0      362 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/types_extra.py
+-rw-r--r--   0        0        0    15102 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/validators.py
+-rw-r--r--   0        0        0     8944 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/components/viz.py
+-rw-r--r--   0        0        0     1621 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/config.py
+-rw-r--r--   0        0        0     2933 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/constants.py
+-rw-r--r--   0        0        0     1265 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/exceptions.py
+-rw-r--r--   0        0        0    15149 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/log.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/material_library/__init__.py
+-rw-r--r--   0        0        0    70598 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/material_library/material_library.py
+-rw-r--r--   0        0        0     9498 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/material_library/material_reference.py
+-rw-r--r--   0        0        0    15924 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/material_library/parametric_materials.py
+-rw-r--r--   0        0        0     5708 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/packaging.py
+-rw-r--r--   0        0        0       77 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/__init__.py
+-rw-r--r--   0        0        0    33133 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/README.md
+-rw-r--r--   0        0        0     1416 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/__init__.py
+-rw-r--r--   0        0        0      898 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0        0        0    10610 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/base.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0        0        0    19097 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0        0        0     1049 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0        0        0    18604 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0        0        0    10720 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0        0        0    26055 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0        0        0    16767 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0        0        0    33012 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0        0        0     8591 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0        0        0     2093 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/utils/__init__.py
+-rw-r--r--   0        0        0     8126 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/utils/filter.py
+-rw-r--r--   0        0        0     9065 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/utils/penalty.py
+-rw-r--r--   0        0        0    29641 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/adjoint/web.py
+-rw-r--r--   0        0        0     6401 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/README.md
+-rw-r--r--   0        0        0      441 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/design.py
+-rw-r--r--   0        0        0    14172 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/method.py
+-rw-r--r--   0        0        0     7087 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/parameter.py
+-rw-r--r--   0        0        0    11780 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/design/result.py
+-rw-r--r--   0        0        0      366 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0        0        0    22651 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0        0        0    33833 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/dispersion/fit_fast.py
+-rw-r--r--   0        0        0      213 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0        0        0    13282 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/dispersion/web.py
+-rw-r--r--   0        0        0     1213 2024-04-02 18:49:48.812888 tidy3d-2.6.3/tidy3d/plugins/mode/LICENSE
+-rw-r--r--   0        0        0       42 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/README.md
+-rw-r--r--   0        0        0      138 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0        0        0     5733 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0        0        0    41403 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0        0        0    29953 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0        0        0     4370 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/transforms.py
+-rw-r--r--   0        0        0       81 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/mode/web.py
+-rw-r--r--   0        0        0      116 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/polyslab/polyslab.py
+-rw-r--r--   0        0        0      117 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0        0        0    17644 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/resonance/resonance.py
+-rw-r--r--   0        0        0      170 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0        0        0    20777 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/smatrix/smatrix.py
+-rw-r--r--   0        0        0      129 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0        0        0    36178 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0        0        0   521877 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/schema.json
+-rw-r--r--   0        0        0    10908 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/updater.py
+-rw-r--r--   0        0        0       87 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/version.py
+-rw-r--r--   0        0        0     1083 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/web/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/web/api/__init__.py
+-rw-r--r--   0        0        0     2669 2024-04-02 18:49:48.816888 tidy3d-2.6.3/tidy3d/web/api/asynchronous.py
+-rw-r--r--   0        0        0   275233 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/cacert.pem
+-rw-r--r--   0        0        0     2284 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/connect_util.py
+-rw-r--r--   0        0        0    28266 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/container.py
+-rw-r--r--   0        0        0     3792 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/material_fitter.py
+-rw-r--r--   0        0        0     1449 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/material_libray.py
+-rw-r--r--   0        0        0    18711 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/mode.py
+-rw-r--r--   0        0        0     8109 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/tidy3d_stub.py
+-rw-r--r--   0        0        0    32481 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/api/webapi.py
+-rw-r--r--   0        0        0       88 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/__init__.py
+-rw-r--r--   0        0        0     3491 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/app.py
+-rw-r--r--   0        0        0      348 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/constants.py
+-rw-r--r--   0        0        0    63715 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/converter.py
+-rw-r--r--   0        0        0     1949 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/__init__.py
+-rw-r--r--   0        0        0    12380 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/documentation.py
+-rw-r--r--   0        0        0      400 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/index.py
+-rw-r--r--   0        0        0    15383 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/install.py
+-rw-r--r--   0        0        0     4159 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/packaging.py
+-rw-r--r--   0        0        0     1961 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/tests.py
+-rw-r--r--   0        0        0     1700 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/develop/utils.py
+-rw-r--r--   0        0        0     3590 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/migrate.py
+-rw-r--r--   0        0        0     3959 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/cli/readme.md
+-rw-r--r--   0        0        0       35 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/__init__.py
+-rw-r--r--   0        0        0       58 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/cache.py
+-rw-r--r--   0        0        0      754 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/constants.py
+-rw-r--r--   0        0        0      940 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/core_config.py
+-rw-r--r--   0        0        0     4982 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/environment.py
+-rw-r--r--   0        0        0      331 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/exceptions.py
+-rw-r--r--   0        0        0     2235 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/file_util.py
+-rw-r--r--   0        0        0     5917 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/http_util.py
+-rw-r--r--   0        0        0    12450 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/s3utils.py
+-rw-r--r--   0        0        0     2243 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/stub.py
+-rw-r--r--   0        0        0    18838 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/task_core.py
+-rw-r--r--   0        0        0     2188 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/task_info.py
+-rw-r--r--   0        0        0     1435 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/core/types.py
+-rw-r--r--   0        0        0      132 2024-04-02 18:49:48.820888 tidy3d-2.6.3/tidy3d/web/environment.py
+-rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 tidy3d-2.6.3/PKG-INFO
```

### Comparing `tidy3d-2.6.2/LICENSE` & `tidy3d-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/README.md` & `tidy3d-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/pyproject.toml` & `tidy3d-2.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidy3d"
-version = "2.6.2"
+version = "2.6.3"
 description = "A fast FDTD solver"
 authors = ["Tyler Hughes <tyler@flexcompute.com>"]
 license = "LGPLv2+"
 readme = "README.md"
 homepage = "https://github.com/flexcompute/tidy3d"
 repository = "https://github.com/flexcompute/tidy3d"
 classifiers = [
@@ -182,15 +182,15 @@
   "C",  # flake8-comprehensions
   "B",  # flake8-bugbear
   "UP",
   "NPY201", # numpy 2.* compatibility check
 ]
 
 [tool.bumpversion]
-current_version = "2.6.2"
+current_version = "2.6.3"
 parse = """(?x)
     (?P<major>0|[1-9]\\d*)\\.
     (?P<minor>0|[1-9]\\d*)\\.
     (?P<patch>0|[1-9]\\d*)
     (?:
         -                             # dash seperator for pre-release section
         (?P<pre_l>[a-zA-Z-]+)         # pre-release label
```

### Comparing `tidy3d-2.6.2/tidy3d/README.md` & `tidy3d-2.6.3/tidy3d/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/__init__.py` & `tidy3d-2.6.3/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/__main__.py` & `tidy3d-2.6.3/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/README.md` & `tidy3d-2.6.3/tidy3d/components/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/apodization.py` & `tidy3d-2.6.3/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/base.py` & `tidy3d-2.6.3/tidy3d/components/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 INDENT_JSON_FILE = 4  # default indentation of json string in json files
 INDENT = None  # default indentation of json string used internally
 JSON_TAG = "JSON_STRING"
 # If json string is larger than ``MAX_STRING_LENGTH``, split the string when storing in hdf5
 MAX_STRING_LENGTH = 1e9
-FORBID_SPECIAL_CHARACTERS = ["/", '"']
+FORBID_SPECIAL_CHARACTERS = ["/"]
 
 
 def cache(prop):
     """Decorates a property to cache the first computed value and return it on subsequent calls."""
 
     # note, we could also just use `prop` as dict key, but hashing property might be slow
     prop_name = prop.__name__
```

### Comparing `tidy3d-2.6.2/tidy3d/components/base_sim/data/monitor_data.py` & `tidy3d-2.6.3/tidy3d/components/base_sim/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/base_sim/data/sim_data.py` & `tidy3d-2.6.3/tidy3d/components/base_sim/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/base_sim/monitor.py` & `tidy3d-2.6.3/tidy3d/components/base_sim/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/base_sim/simulation.py` & `tidy3d-2.6.3/tidy3d/components/base_sim/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/base_sim/source.py` & `tidy3d-2.6.3/tidy3d/components/base_sim/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/bc_placement.py` & `tidy3d-2.6.3/tidy3d/components/bc_placement.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/boundary.py` & `tidy3d-2.6.3/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/README.md` & `tidy3d-2.6.3/tidy3d/components/data/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/data_array.py` & `tidy3d-2.6.3/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/dataset.py` & `tidy3d-2.6.3/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/monitor_data.py` & `tidy3d-2.6.3/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/sim_data.py` & `tidy3d-2.6.3/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/data/validators.py` & `tidy3d-2.6.3/tidy3d/components/data/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/field_projection.py` & `tidy3d-2.6.3/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/file_util.py` & `tidy3d-2.6.3/tidy3d/components/file_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/base.py` & `tidy3d-2.6.3/tidy3d/components/geometry/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/mesh.py` & `tidy3d-2.6.3/tidy3d/components/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/polyslab.py` & `tidy3d-2.6.3/tidy3d/components/geometry/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/primitives.py` & `tidy3d-2.6.3/tidy3d/components/geometry/primitives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/triangulation.py` & `tidy3d-2.6.3/tidy3d/components/geometry/triangulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/utils.py` & `tidy3d-2.6.3/tidy3d/components/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/geometry/utils_2d.py` & `tidy3d-2.6.3/tidy3d/components/geometry/utils_2d.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/grid/grid.py` & `tidy3d-2.6.3/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.6.3/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/grid/mesher.py` & `tidy3d-2.6.3/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/boundary.py` & `tidy3d-2.6.3/tidy3d/components/heat/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/data/monitor_data.py` & `tidy3d-2.6.3/tidy3d/components/heat/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/data/sim_data.py` & `tidy3d-2.6.3/tidy3d/components/heat/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/grid.py` & `tidy3d-2.6.3/tidy3d/components/heat/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/monitor.py` & `tidy3d-2.6.3/tidy3d/components/heat/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/simulation.py` & `tidy3d-2.6.3/tidy3d/components/heat/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ..viz import add_ax_if_none, equal_aspect, PlotParams
 from ..structure import Structure
 from ..geometry.base import Box, GeometryGroup
 from ..geometry.primitives import Sphere, Cylinder
 from ..geometry.polyslab import PolySlab
 from ..geometry.mesh import TriangleMesh
 from ..scene import Scene
+from ..heat_spec import SolidSpec
 
 from ..bc_placement import StructureBoundary, StructureStructureInterface
 from ..bc_placement import StructureSimulationBoundary, SimulationBoundary
 from ..bc_placement import MediumMediumInterface
 
 from ...exceptions import SetupError
 from ...constants import inf, VOLUMETRIC_HEAT_RATE
@@ -104,29 +105,35 @@
         "at the simulation center of each axis, respectively. "
         "Each element can be ``0`` (symmetry off) or ``1`` (symmetry on).",
     )
 
     @pd.validator("structures", always=True)
     def check_unsupported_geometries(cls, val):
         """Error if structures contain unsupported yet geometries."""
-        for structure in val:
+        for ind, structure in enumerate(val):
+            bbox = structure.geometry.bounding_box
+            if any(s == 0 for s in bbox.size):
+                raise SetupError(
+                    f"'HeatSimulation' does not currently support structures with dimensions of zero size ('structures[{ind}]')."
+                )
+
             if isinstance(structure.geometry, GeometryGroup):
                 geometries = structure.geometry.geometries
             else:
                 geometries = [structure.geometry]
             for geom in geometries:
                 if isinstance(geom, (GeometryGroup)):
                     raise SetupError(
-                        "'HeatSimulation' does not currently support recursive 'GeometryGroup's."
+                        "'HeatSimulation' does not currently support recursive 'GeometryGroup's ('structures[{ind}]')."
                     )
                 if not isinstance(geom, HeatSingleGeometryType):
                     geom_names = [f"'{cl.__name__}'" for cl in HeatSingleGeometryType]
                     raise SetupError(
                         "'HeatSimulation' does not currently support geometries of type "
-                        f"'{geom.type}'. Allowed geometries are "
+                        f"'{geom.type}'  ('structures[{ind}]'). Allowed geometries are "
                         f"{', '.join(geom_names)}, "
                         "and non-recursive 'GeometryGroup'."
                     )
         return val
 
     @pd.validator("size", always=True)
     def check_zero_dim_domain(cls, val, values):
@@ -172,14 +179,25 @@
                         raise SetupError(
                             f"Material '{med_name}' provided in "
                             f"'boundary_spec[{bc_ind}].placement' (type '{bc_place.type}') "
                             "is not found among simulation mediums."
                         )
         return val
 
+    @pd.validator("boundary_spec", always=True)
+    def not_all_neumann(cls, val):
+        """Error if all boundary conditions are Neumann bc."""
+
+        if len(val) == 0 or all(isinstance(bc_spec.condition, HeatFluxBC) for bc_spec in val):
+            raise SetupError(
+                "Heat simulation contains only 'HeatFluxBC' (Neumann) boundary conditions. Steady-state solution is undefined in this case."
+            )
+
+        return val
+
     @pd.validator("grid_spec", always=True)
     @skip_if_fields_missing(["structures"])
     def names_exist_grid_spec(cls, val, values):
         """Warn if UniformUnstructuredGrid points at a non-existing structure."""
 
         structures = values.get("structures")
         structures_names = {s.name for s in structures}
@@ -205,14 +223,29 @@
                 if name not in structures_names:
                     raise SetupError(
                         f"Structure '{name}' provided in a '{source.type}' "
                         "is not found among simulation structures."
                     )
         return val
 
+    @pd.root_validator(skip_on_failure=True)
+    def check_medium_heat_spec(cls, values):
+        """Error if no structures with SolidSpec."""
+        medium = values["medium"]
+        structures = values["structures"]
+        if not (
+            isinstance(medium.heat_spec, SolidSpec)
+            or any(isinstance(struct.medium.heat_spec, SolidSpec) for struct in structures)
+        ):
+            raise SetupError(
+                "No solid materials ('SolidSpec') are detected in heat simulation. Solution domain is empty."
+            )
+
+        return values
+
     @equal_aspect
     @add_ax_if_none
     def plot_heat_conductivity(
         self,
         x: float = None,
         y: float = None,
         z: float = None,
@@ -810,21 +843,32 @@
         >>> from tidy3d import Scene, Medium, Box, Structure, UniformUnstructuredGrid
         >>> box = Structure(
         ...     geometry=Box(center=(0, 0, 0), size=(1, 2, 3)),
         ...     medium=Medium(permittivity=5),
         ... )
         >>> scene = Scene(
         ...     structures=[box],
-        ...     medium=Medium(permittivity=3),
+        ...     medium=Medium(
+        ...         permittivity=3,
+        ...         heat_spec=SolidSpec(
+        ...             conductivity=1, capacity=1,
+        ...         ),
+        ...     ),
         ... )
         >>> sim = HeatSimulation.from_scene(
         ...     scene=scene,
         ...     center=(0, 0, 0),
         ...     size=(5, 6, 7),
         ...     grid_spec=UniformUnstructuredGrid(dl=0.4),
+        ...     boundary_spec=[
+        ...         HeatBoundarySpec(
+        ...             placement=SimulationBoundary(),
+        ...             condition=TemperatureBC(temperature=300)
+        ...         )
+        ...     ],
         ... )
         """
 
         return cls(
             structures=scene.structures,
             medium=scene.medium,
             **kwargs,
```

### Comparing `tidy3d-2.6.2/tidy3d/components/heat/source.py` & `tidy3d-2.6.3/tidy3d/components/heat/source.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from ..base import cached_property
 from ..base_sim.source import AbstractSource
 from ..data.data_array import TimeDataArray
 from ..viz import PlotParams
 
 from ...constants import VOLUMETRIC_HEAT_RATE
+from ...exceptions import SetupError
 
 
 class HeatSource(AbstractSource, ABC):
     """Abstract heat source."""
 
     structures: Tuple[str, ...] = pd.Field(
         title="Target Structures",
@@ -25,14 +26,22 @@
     )
 
     @cached_property
     def plot_params(self) -> PlotParams:
         """Default parameters for plotting a Source object."""
         return plot_params_heat_source
 
+    @pd.validator("structures", always=True)
+    def check_non_empty_structures(cls, val):
+        """Error if source doesn't point at any structures."""
+        if len(val) == 0:
+            raise SetupError("List of structures for heat source is empty.")
+
+        return val
+
 
 class UniformHeatSource(HeatSource):
     """Volumetric heat source.
 
     Example
     -------
     >>> heat_source = UniformHeatSource(rate=1, structures=["box"])
```

### Comparing `tidy3d-2.6.2/tidy3d/components/heat_spec.py` & `tidy3d-2.6.3/tidy3d/components/heat_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/medium.py` & `tidy3d-2.6.3/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/mode.py` & `tidy3d-2.6.3/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/monitor.py` & `tidy3d-2.6.3/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/parameter_perturbation.py` & `tidy3d-2.6.3/tidy3d/components/parameter_perturbation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/scene.py` & `tidy3d-2.6.3/tidy3d/components/scene.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/simulation.py` & `tidy3d-2.6.3/tidy3d/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/source.py` & `tidy3d-2.6.3/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/structure.py` & `tidy3d-2.6.3/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/time.py` & `tidy3d-2.6.3/tidy3d/components/time.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/time_modulation.py` & `tidy3d-2.6.3/tidy3d/components/time_modulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/transformation.py` & `tidy3d-2.6.3/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/types.py` & `tidy3d-2.6.3/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/validators.py` & `tidy3d-2.6.3/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/components/viz.py` & `tidy3d-2.6.3/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/config.py` & `tidy3d-2.6.3/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/constants.py` & `tidy3d-2.6.3/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/exceptions.py` & `tidy3d-2.6.3/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/log.py` & `tidy3d-2.6.3/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/material_library/material_library.py` & `tidy3d-2.6.3/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/material_library/material_reference.py` & `tidy3d-2.6.3/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.6.3/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/packaging.py` & `tidy3d-2.6.3/tidy3d/packaging.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/README.md` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/__init__.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/utils/filter.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/utils/filter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/utils/penalty.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/utils/penalty.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.6.3/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/design/README.md` & `tidy3d-2.6.3/tidy3d/plugins/design/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/design/design.py` & `tidy3d-2.6.3/tidy3d/plugins/design/design.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/design/method.py` & `tidy3d-2.6.3/tidy3d/plugins/design/method.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/design/parameter.py` & `tidy3d-2.6.3/tidy3d/plugins/design/parameter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/design/result.py` & `tidy3d-2.6.3/tidy3d/plugins/design/result.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.6.3/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/dispersion/fit_fast.py` & `tidy3d-2.6.3/tidy3d/plugins/dispersion/fit_fast.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/dispersion/web.py` & `tidy3d-2.6.3/tidy3d/plugins/dispersion/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/mode/LICENSE` & `tidy3d-2.6.3/tidy3d/plugins/mode/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.6.3/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.6.3/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/mode/solver.py` & `tidy3d-2.6.3/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.6.3/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.6.3/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.6.3/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.6.3/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.6.3/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/schema.json` & `tidy3d-2.6.3/tidy3d/schema.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
   "title": "Simulation",
-  "description": "Custom implementation of Maxwell\u2019s equations which represents the physical model to be solved using the FDTD\nmethod.\n\nParameters\n----------\ncenter : Tuple[float, float, float] = (0.0, 0.0, 0.0)\n    [units = um].  Center of object in x, y, and z.\nsize : Tuple[NonNegativeFloat, NonNegativeFloat, NonNegativeFloat]\n    [units = um].  Size in x, y, and z directions.\nmedium : Union[Medium, AnisotropicMedium, PECMedium, PoleResidue, Sellmeier, Lorentz, Debye, Drude, FullyAnisotropicMedium, CustomMedium, CustomPoleResidue, CustomSellmeier, CustomLorentz, CustomDebye, CustomDrude, CustomAnisotropicMedium, PerturbationMedium, PerturbationPoleResidue] = Medium(name=None, frequency_range=None, allow_gain=False, nonlinear_spec=None, modulation_spec=None, heat_spec=None, type='Medium', permittivity=1.0, conductivity=0.0)\n    Background medium of simulation, defaults to vacuum if not specified.\nstructures : Tuple[Structure, ...] = ()\n    Tuple of structures present in simulation. Note: Structures defined later in this list override the simulation material properties in regions of spatial overlap.\nsymmetry : Tuple[Literal[0, -1, 1], Literal[0, -1, 1], Literal[0, -1, 1]] = (0, 0, 0)\n    Tuple of integers defining reflection symmetry across a plane bisecting the simulation domain normal to the x-, y-, and z-axis at the simulation center of each axis, respectively. Each element can be ``0`` (no symmetry), ``1`` (even, i.e. 'PMC' symmetry) or ``-1`` (odd, i.e. 'PEC' symmetry). Note that the vectorial nature of the fields must be taken into account to correctly determine the symmetry value.\nsources : Tuple[Annotated[Union[tidy3d.components.source.UniformCurrentSource, tidy3d.components.source.PointDipole, tidy3d.components.source.GaussianBeam, tidy3d.components.source.AstigmaticGaussianBeam, tidy3d.components.source.ModeSource, tidy3d.components.source.PlaneWave, tidy3d.components.source.CustomFieldSource, tidy3d.components.source.CustomCurrentSource, tidy3d.components.source.TFSF], FieldInfo(default=PydanticUndefined, discriminator='type', extra={})], ...] = ()\n    Tuple of electric current sources injecting fields into the simulation.\nboundary_spec : BoundarySpec = BoundarySpec(x=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), y=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), z=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), type='BoundarySpec')\n    Specification of boundary conditions along each dimension. If ``None``, PML boundary conditions are applied on all sides.\nmonitors : Tuple[Annotated[Union[tidy3d.components.monitor.FieldMonitor, tidy3d.components.monitor.FieldTimeMonitor, tidy3d.components.monitor.PermittivityMonitor, tidy3d.components.monitor.FluxMonitor, tidy3d.components.monitor.FluxTimeMonitor, tidy3d.components.monitor.ModeMonitor, tidy3d.components.monitor.ModeSolverMonitor, tidy3d.components.monitor.FieldProjectionAngleMonitor, tidy3d.components.monitor.FieldProjectionCartesianMonitor, tidy3d.components.monitor.FieldProjectionKSpaceMonitor, tidy3d.components.monitor.DiffractionMonitor], FieldInfo(default=PydanticUndefined, discriminator='type', extra={})], ...] = ()\n    Tuple of monitors in the simulation. Note: monitor names are used to access data after simulation is run.\ngrid_spec : GridSpec = GridSpec(grid_x=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), grid_y=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), grid_z=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), wavelength=None, override_structures=(), type='GridSpec')\n    Specifications for the simulation grid along each of the three directions.\nversion : str = 2.6.2\n    String specifying the front end version number.\ncourant : ConstrainedFloatValue = 0.99\n    Courant stability factor, controls time step to spatial step ratio. Lower values lead to more stable simulations for dispersive materials, but result in longer simulation times. This factor is normalized to no larger than 1 when CFL stability condition is met in 3D.\nnormalize_index : Optional[NonNegativeInt] = 0\n    Index of the source in the tuple of sources whose spectrum will be used to normalize the frequency-dependent data. If ``None``, the raw field data is returned unnormalized.\nshutoff : NonNegativeFloat = 1e-05\n    Ratio of the instantaneous integrated E-field intensity to the maximum value at which the simulation will automatically terminate time stepping. Used to prevent extraneous run time of simulations with fully decayed fields. Set to ``0`` to disable this feature.\nsubpixel : bool = True\n    If ``True``, uses subpixel averaging of the permittivity based on structure definition, resulting in much higher accuracy for a given grid size.\nrun_time : PositiveFloat\n    [units = sec].  Total electromagnetic evolution time in seconds. Note: If simulation 'shutoff' is specified, simulation will terminate early when shutoff condition met. \n\nNotes\n-----\n\n    A ``Simulation`` defines a custom implementation of Maxwell's equations which represents the physical model\n    to be solved using `the Finite-Difference Time-Domain (FDTD) method\n    <https://www.flexcompute.com/fdtd101/Lecture-1-Introduction-to-FDTD-Simulation/>`_. ``tidy3d`` simulations\n    run very quickly in the cloud through GPU parallelization.\n\n    .. image:: ../../_static/img/field_update_fdtd.png\n        :width: 50%\n        :align: left\n\n    FDTD is a method for simulating the interaction of electromagnetic waves with structures and materials. It is\n    the most widely used method in photonics design. The Maxwell's\n    equations implemented in the ``Simulation`` are solved per time-step in the order shown in this image.\n\n    The simplified input to FDTD solver consists of the permittivity distribution defined by :attr:`structures`\n    which describe the device and :attr:`sources` of electromagnetic excitation. This information is used to\n    computate the time dynamics of the electric and magnetic fields in this system. From these time-domain\n    results, frequency-domain information of the simulation can also be extracted, and used for device design and\n    optimization.\n\n    If you are new to the FDTD method, we recommend you get started with the `FDTD 101 Lecture Series\n    <https://www.flexcompute.com/tidy3d/learning-center/fdtd101/>`_\n\n    **Dimensions Selection**\n\n    By default, simulations are defined as 3D. To make the simulation 2D, we can just set the simulation\n    :attr:`size` in one of the dimensions to be 0. However, note that we still have to define a grid size (eg.\n    ``tidy3d.Simulation(size=[size_x, size_y, 0])``) and specify a periodic boundary condition in that direction.\n\n    .. TODO sort out inheritance problem https://aware-moon.cloudvent.net/tidy3d/examples/notebooks/RingResonator/\n\n    See further parameter explanations below.\n\nExample\n-------\n>>> from tidy3d import Sphere, Cylinder, PolySlab\n>>> from tidy3d import UniformCurrentSource, GaussianPulse\n>>> from tidy3d import FieldMonitor, FluxMonitor\n>>> from tidy3d import GridSpec, AutoGrid\n>>> from tidy3d import BoundarySpec, Boundary\n>>> from tidy3d import Medium\n>>> sim = Simulation(\n...     size=(3.0, 3.0, 3.0),\n...     grid_spec=GridSpec(\n...         grid_x = AutoGrid(min_steps_per_wvl = 20),\n...         grid_y = AutoGrid(min_steps_per_wvl = 20),\n...         grid_z = AutoGrid(min_steps_per_wvl = 20)\n...     ),\n...     run_time=40e-11,\n...     structures=[\n...         Structure(\n...             geometry=Box(size=(1, 1, 1), center=(0, 0, 0)),\n...             medium=Medium(permittivity=2.0),\n...         ),\n...     ],\n...     sources=[\n...         UniformCurrentSource(\n...             size=(0, 0, 0),\n...             center=(0, 0.5, 0),\n...             polarization=\"Hx\",\n...             source_time=GaussianPulse(\n...                 freq0=2e14,\n...                 fwidth=4e13,\n...             ),\n...         )\n...     ],\n...     monitors=[\n...         FluxMonitor(size=(1, 1, 0), center=(0, 0, 0), freqs=[2e14, 2.5e14], name='flux'),\n...     ],\n...     symmetry=(0, 0, 0),\n...     boundary_spec=BoundarySpec(\n...         x = Boundary.pml(num_layers=20),\n...         y = Boundary.pml(num_layers=30),\n...         z = Boundary.periodic(),\n...     ),\n...     shutoff=1e-6,\n...     courant=0.8,\n...     subpixel=False,\n... )\n\nSee Also\n--------\n\n**Notebooks:**\n    * `Quickstart <../../notebooks/StartHere.html>`_: Usage in a basic simulation flow.\n    * `Using automatic nonuniform meshing <../../notebooks/AutoGrid.html>`_\n    * See nearly all notebooks for :class:`Simulation` applications.\n\n**Lectures:**\n    * `Introduction to FDTD Simulation <https://www.flexcompute.com/fdtd101/Lecture-1-Introduction-to-FDTD-Simulation/#presentation-slides>`_: Usage in a basic simulation flow.\n    * `Prelude to Integrated Photonics Simulation: Mode Injection <https://www.flexcompute.com/fdtd101/Lecture-4-Prelude-to-Integrated-Photonics-Simulation-Mode-Injection/>`_\n\n**GUI:**\n    * `FDTD Walkthrough <https://www.flexcompute.com/tidy3d/learning-center/tidy3d-gui/Lecture-1-FDTD-Walkthrough/#presentation-slides>`_",
+  "description": "Custom implementation of Maxwell\u2019s equations which represents the physical model to be solved using the FDTD\nmethod.\n\nParameters\n----------\ncenter : Tuple[float, float, float] = (0.0, 0.0, 0.0)\n    [units = um].  Center of object in x, y, and z.\nsize : Tuple[NonNegativeFloat, NonNegativeFloat, NonNegativeFloat]\n    [units = um].  Size in x, y, and z directions.\nmedium : Union[Medium, AnisotropicMedium, PECMedium, PoleResidue, Sellmeier, Lorentz, Debye, Drude, FullyAnisotropicMedium, CustomMedium, CustomPoleResidue, CustomSellmeier, CustomLorentz, CustomDebye, CustomDrude, CustomAnisotropicMedium, PerturbationMedium, PerturbationPoleResidue] = Medium(name=None, frequency_range=None, allow_gain=False, nonlinear_spec=None, modulation_spec=None, heat_spec=None, type='Medium', permittivity=1.0, conductivity=0.0)\n    Background medium of simulation, defaults to vacuum if not specified.\nstructures : Tuple[Structure, ...] = ()\n    Tuple of structures present in simulation. Note: Structures defined later in this list override the simulation material properties in regions of spatial overlap.\nsymmetry : Tuple[Literal[0, -1, 1], Literal[0, -1, 1], Literal[0, -1, 1]] = (0, 0, 0)\n    Tuple of integers defining reflection symmetry across a plane bisecting the simulation domain normal to the x-, y-, and z-axis at the simulation center of each axis, respectively. Each element can be ``0`` (no symmetry), ``1`` (even, i.e. 'PMC' symmetry) or ``-1`` (odd, i.e. 'PEC' symmetry). Note that the vectorial nature of the fields must be taken into account to correctly determine the symmetry value.\nsources : Tuple[Annotated[Union[tidy3d.components.source.UniformCurrentSource, tidy3d.components.source.PointDipole, tidy3d.components.source.GaussianBeam, tidy3d.components.source.AstigmaticGaussianBeam, tidy3d.components.source.ModeSource, tidy3d.components.source.PlaneWave, tidy3d.components.source.CustomFieldSource, tidy3d.components.source.CustomCurrentSource, tidy3d.components.source.TFSF], FieldInfo(default=PydanticUndefined, discriminator='type', extra={})], ...] = ()\n    Tuple of electric current sources injecting fields into the simulation.\nboundary_spec : BoundarySpec = BoundarySpec(x=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), y=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), z=Boundary(plus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, minus=PML(name=None,, type='PML',, num_layers=12,, parameters=PMLParams(sigma_order=3,, sigma_min=0.0,, sigma_max=1.5,, type='PMLParams',, kappa_order=3,, kappa_min=1.0,, kappa_max=3.0,, alpha_order=1,, alpha_min=0.0,, alpha_max=0.0)),, type='Boundary'), type='BoundarySpec')\n    Specification of boundary conditions along each dimension. If ``None``, PML boundary conditions are applied on all sides.\nmonitors : Tuple[Annotated[Union[tidy3d.components.monitor.FieldMonitor, tidy3d.components.monitor.FieldTimeMonitor, tidy3d.components.monitor.PermittivityMonitor, tidy3d.components.monitor.FluxMonitor, tidy3d.components.monitor.FluxTimeMonitor, tidy3d.components.monitor.ModeMonitor, tidy3d.components.monitor.ModeSolverMonitor, tidy3d.components.monitor.FieldProjectionAngleMonitor, tidy3d.components.monitor.FieldProjectionCartesianMonitor, tidy3d.components.monitor.FieldProjectionKSpaceMonitor, tidy3d.components.monitor.DiffractionMonitor], FieldInfo(default=PydanticUndefined, discriminator='type', extra={})], ...] = ()\n    Tuple of monitors in the simulation. Note: monitor names are used to access data after simulation is run.\ngrid_spec : GridSpec = GridSpec(grid_x=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), grid_y=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), grid_z=AutoGrid(type='AutoGrid',, min_steps_per_wvl=10.0,, max_scale=1.4,, dl_min=0.0,, mesher=GradedMesher(type='GradedMesher')), wavelength=None, override_structures=(), type='GridSpec')\n    Specifications for the simulation grid along each of the three directions.\nversion : str = 2.6.3\n    String specifying the front end version number.\ncourant : ConstrainedFloatValue = 0.99\n    Courant stability factor, controls time step to spatial step ratio. Lower values lead to more stable simulations for dispersive materials, but result in longer simulation times. This factor is normalized to no larger than 1 when CFL stability condition is met in 3D.\nnormalize_index : Optional[NonNegativeInt] = 0\n    Index of the source in the tuple of sources whose spectrum will be used to normalize the frequency-dependent data. If ``None``, the raw field data is returned unnormalized.\nshutoff : NonNegativeFloat = 1e-05\n    Ratio of the instantaneous integrated E-field intensity to the maximum value at which the simulation will automatically terminate time stepping. Used to prevent extraneous run time of simulations with fully decayed fields. Set to ``0`` to disable this feature.\nsubpixel : bool = True\n    If ``True``, uses subpixel averaging of the permittivity based on structure definition, resulting in much higher accuracy for a given grid size.\nrun_time : PositiveFloat\n    [units = sec].  Total electromagnetic evolution time in seconds. Note: If simulation 'shutoff' is specified, simulation will terminate early when shutoff condition met. \n\nNotes\n-----\n\n    A ``Simulation`` defines a custom implementation of Maxwell's equations which represents the physical model\n    to be solved using `the Finite-Difference Time-Domain (FDTD) method\n    <https://www.flexcompute.com/fdtd101/Lecture-1-Introduction-to-FDTD-Simulation/>`_. ``tidy3d`` simulations\n    run very quickly in the cloud through GPU parallelization.\n\n    .. image:: ../../_static/img/field_update_fdtd.png\n        :width: 50%\n        :align: left\n\n    FDTD is a method for simulating the interaction of electromagnetic waves with structures and materials. It is\n    the most widely used method in photonics design. The Maxwell's\n    equations implemented in the ``Simulation`` are solved per time-step in the order shown in this image.\n\n    The simplified input to FDTD solver consists of the permittivity distribution defined by :attr:`structures`\n    which describe the device and :attr:`sources` of electromagnetic excitation. This information is used to\n    computate the time dynamics of the electric and magnetic fields in this system. From these time-domain\n    results, frequency-domain information of the simulation can also be extracted, and used for device design and\n    optimization.\n\n    If you are new to the FDTD method, we recommend you get started with the `FDTD 101 Lecture Series\n    <https://www.flexcompute.com/tidy3d/learning-center/fdtd101/>`_\n\n    **Dimensions Selection**\n\n    By default, simulations are defined as 3D. To make the simulation 2D, we can just set the simulation\n    :attr:`size` in one of the dimensions to be 0. However, note that we still have to define a grid size (eg.\n    ``tidy3d.Simulation(size=[size_x, size_y, 0])``) and specify a periodic boundary condition in that direction.\n\n    .. TODO sort out inheritance problem https://aware-moon.cloudvent.net/tidy3d/examples/notebooks/RingResonator/\n\n    See further parameter explanations below.\n\nExample\n-------\n>>> from tidy3d import Sphere, Cylinder, PolySlab\n>>> from tidy3d import UniformCurrentSource, GaussianPulse\n>>> from tidy3d import FieldMonitor, FluxMonitor\n>>> from tidy3d import GridSpec, AutoGrid\n>>> from tidy3d import BoundarySpec, Boundary\n>>> from tidy3d import Medium\n>>> sim = Simulation(\n...     size=(3.0, 3.0, 3.0),\n...     grid_spec=GridSpec(\n...         grid_x = AutoGrid(min_steps_per_wvl = 20),\n...         grid_y = AutoGrid(min_steps_per_wvl = 20),\n...         grid_z = AutoGrid(min_steps_per_wvl = 20)\n...     ),\n...     run_time=40e-11,\n...     structures=[\n...         Structure(\n...             geometry=Box(size=(1, 1, 1), center=(0, 0, 0)),\n...             medium=Medium(permittivity=2.0),\n...         ),\n...     ],\n...     sources=[\n...         UniformCurrentSource(\n...             size=(0, 0, 0),\n...             center=(0, 0.5, 0),\n...             polarization=\"Hx\",\n...             source_time=GaussianPulse(\n...                 freq0=2e14,\n...                 fwidth=4e13,\n...             ),\n...         )\n...     ],\n...     monitors=[\n...         FluxMonitor(size=(1, 1, 0), center=(0, 0, 0), freqs=[2e14, 2.5e14], name='flux'),\n...     ],\n...     symmetry=(0, 0, 0),\n...     boundary_spec=BoundarySpec(\n...         x = Boundary.pml(num_layers=20),\n...         y = Boundary.pml(num_layers=30),\n...         z = Boundary.periodic(),\n...     ),\n...     shutoff=1e-6,\n...     courant=0.8,\n...     subpixel=False,\n... )\n\nSee Also\n--------\n\n**Notebooks:**\n    * `Quickstart <../../notebooks/StartHere.html>`_: Usage in a basic simulation flow.\n    * `Using automatic nonuniform meshing <../../notebooks/AutoGrid.html>`_\n    * See nearly all notebooks for :class:`Simulation` applications.\n\n**Lectures:**\n    * `Introduction to FDTD Simulation <https://www.flexcompute.com/fdtd101/Lecture-1-Introduction-to-FDTD-Simulation/#presentation-slides>`_: Usage in a basic simulation flow.\n    * `Prelude to Integrated Photonics Simulation: Mode Injection <https://www.flexcompute.com/fdtd101/Lecture-4-Prelude-to-Integrated-Photonics-Simulation-Mode-Injection/>`_\n\n**GUI:**\n    * `FDTD Walkthrough <https://www.flexcompute.com/tidy3d/learning-center/tidy3d-gui/Lecture-1-FDTD-Walkthrough/#presentation-slides>`_",
   "type": "object",
   "properties": {
     "type": {
       "title": "Type",
       "default": "Simulation",
       "enum": [
         "Simulation"
@@ -471,15 +471,15 @@
           "$ref": "#/definitions/GridSpec"
         }
       ]
     },
     "version": {
       "title": "Version",
       "description": "String specifying the front end version number.",
-      "default": "2.6.2",
+      "default": "2.6.3",
       "type": "string"
     },
     "courant": {
       "title": "Courant Factor",
       "description": "Courant stability factor, controls time step to spatial step ratio. Lower values lead to more stable simulations for dispersive materials, but result in longer simulation times. This factor is normalized to no larger than 1 when CFL stability condition is met in 3D.",
       "default": 0.99,
       "exclusiveMinimum": 0.0,
```

### Comparing `tidy3d-2.6.2/tidy3d/updater.py` & `tidy3d-2.6.3/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/__init__.py` & `tidy3d-2.6.3/tidy3d/web/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/asynchronous.py` & `tidy3d-2.6.3/tidy3d/web/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/cacert.pem` & `tidy3d-2.6.3/tidy3d/web/api/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/connect_util.py` & `tidy3d-2.6.3/tidy3d/web/api/connect_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/container.py` & `tidy3d-2.6.3/tidy3d/web/api/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
         path_dir : str = './'
             Base directory where data will be downloaded, by default the current working directory.
 
         Note
         ----
         To load and iterate through the data, use :meth:`Batch.items()`.
 
-        The data for each task will be named as ``{path_dir}/{task_name}.hdf5``.
+        The data for each task will be named as ``{path_dir}/{task_id}.hdf5``.
         The :class:`Batch` hdf5 file will be automatically saved as ``{path_dir}/batch.hdf5``,
         allowing one to load this :class:`Batch` later using ``batch = Batch.from_file()``.
         """
 
         self.to_file(self._batch_path(path_dir=path_dir))
 
         for task_name, job in self.jobs.items():
```

### Comparing `tidy3d-2.6.2/tidy3d/web/api/material_fitter.py` & `tidy3d-2.6.3/tidy3d/web/api/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/material_libray.py` & `tidy3d-2.6.3/tidy3d/web/api/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/mode.py` & `tidy3d-2.6.3/tidy3d/web/api/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/tidy3d_stub.py` & `tidy3d-2.6.3/tidy3d/web/api/tidy3d_stub.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/api/webapi.py` & `tidy3d-2.6.3/tidy3d/web/api/webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/app.py` & `tidy3d-2.6.3/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/converter.py` & `tidy3d-2.6.3/tidy3d/web/cli/converter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/__init__.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/documentation.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/documentation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/install.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/install.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/packaging.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/packaging.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/tests.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/tests.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/develop/utils.py` & `tidy3d-2.6.3/tidy3d/web/cli/develop/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/migrate.py` & `tidy3d-2.6.3/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/cli/readme.md` & `tidy3d-2.6.3/tidy3d/web/cli/readme.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/constants.py` & `tidy3d-2.6.3/tidy3d/web/core/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/core_config.py` & `tidy3d-2.6.3/tidy3d/web/core/core_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/environment.py` & `tidy3d-2.6.3/tidy3d/web/core/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/file_util.py` & `tidy3d-2.6.3/tidy3d/web/core/file_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/http_util.py` & `tidy3d-2.6.3/tidy3d/web/core/http_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/s3utils.py` & `tidy3d-2.6.3/tidy3d/web/core/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/stub.py` & `tidy3d-2.6.3/tidy3d/web/core/stub.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/task_core.py` & `tidy3d-2.6.3/tidy3d/web/core/task_core.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/task_info.py` & `tidy3d-2.6.3/tidy3d/web/core/task_info.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/tidy3d/web/core/types.py` & `tidy3d-2.6.3/tidy3d/web/core/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.6.2/PKG-INFO` & `tidy3d-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.6.2
+Version: 2.6.3
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 License: LGPLv2+
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

