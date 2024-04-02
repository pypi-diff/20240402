# Comparing `tmp/felupe-8.2.1.tar.gz` & `tmp/felupe-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-8.2.1.tar", last modified: Sat Mar 30 21:57:10 2024, max compression
+gzip compressed data, was "felupe-8.3.0.tar", last modified: Tue Apr  2 15:38:15 2024, max compression
```

## Comparing `felupe-8.2.1.tar` & `felupe-8.3.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.009934 felupe-8.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-03-30 21:57:06.000000 felupe-8.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-03-30 21:57:10.009934 felupe-8.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-03-30 21:57:06.000000 felupe-8.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-30 21:57:06.000000 felupe-8.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:57:10.009934 felupe-8.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.985934 felupe-8.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.989934 felupe-8.2.1/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.989934 felupe-8.2.1/src/felupe/assembly/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/_integral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.989934 felupe-8.2.1/src/felupe/assembly/expression/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_bilinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/assembly/expression/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.993934 felupe-8.2.1/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    18221 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_user_materials_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/constitution/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.993934 felupe-8.2.1/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.993934 felupe-8.2.1/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.997934 felupe-8.2.1/src/felupe/field/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.997934 felupe-8.2.1/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    44963 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:09.997934 felupe-8.2.1/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.001934 felupe-8.2.1/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    46977 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.001934 felupe-8.2.1/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.001934 felupe-8.2.1/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.001934 felupe-8.2.1/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.005934 felupe-8.2.1/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    21267 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-30 21:57:06.000000 felupe-8.2.1/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.005934 felupe-8.2.1/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-03-30 21:57:09.000000 felupe-8.2.1/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-03-30 21:57:09.000000 felupe-8.2.1/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:57:09.000000 felupe-8.2.1/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-30 21:57:09.000000 felupe-8.2.1/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 21:57:09.000000 felupe-8.2.1/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:10.005934 felupe-8.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-03-30 21:57:06.000000 felupe-8.2.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.984612 felupe-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-02 15:38:11.000000 felupe-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-02 15:38:15.984612 felupe-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-02 15:38:11.000000 felupe-8.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-02 15:38:11.000000 felupe-8.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:38:15.984612 felupe-8.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.960612 felupe-8.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.964612 felupe-8.3.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.964612 felupe-8.3.0/src/felupe/assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/_integral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.968612 felupe-8.3.0/src/felupe/assembly/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/assembly/expression/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.968612 felupe-8.3.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18221 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_user_materials_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/constitution/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.968612 felupe-8.3.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.972612 felupe-8.3.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.972612 felupe-8.3.0/src/felupe/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.972612 felupe-8.3.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45047 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.976612 felupe-8.3.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.976612 felupe-8.3.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48808 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.976612 felupe-8.3.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.980612 felupe-8.3.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.980612 felupe-8.3.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.980612 felupe-8.3.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20214 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-02 15:38:11.000000 felupe-8.3.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.984612 felupe-8.3.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-02 15:38:15.000000 felupe-8.3.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-02 15:38:15.000000 felupe-8.3.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:38:15.000000 felupe-8.3.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 15:38:15.000000 felupe-8.3.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 15:38:15.000000 felupe-8.3.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:38:15.984612 felupe-8.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-04-02 15:38:11.000000 felupe-8.3.0/tests/test_tools.py
```

### Comparing `felupe-8.2.1/LICENSE` & `felupe-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/PKG-INFO` & `felupe-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.2.1
+Version: 8.3.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-8.2.1/README.md` & `felupe-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/pyproject.toml` & `felupe-8.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/__init__.py` & `felupe-8.3.0/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/_axi.py` & `felupe-8.3.0/src/felupe/assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/_cartesian.py` & `felupe-8.3.0/src/felupe/assembly/_cartesian.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/_integral.py` & `felupe-8.3.0/src/felupe/assembly/_integral.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_basis.py` & `felupe-8.3.0/src/felupe/assembly/expression/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_bilinear.py` & `felupe-8.3.0/src/felupe/assembly/expression/_bilinear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_decorator.py` & `felupe-8.3.0/src/felupe/assembly/expression/_decorator.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_expression.py` & `felupe-8.3.0/src/felupe/assembly/expression/_expression.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_linear.py` & `felupe-8.3.0/src/felupe/assembly/expression/_linear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/assembly/expression/_mixed.py` & `felupe-8.3.0/src/felupe/assembly/expression/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/__init__.py` & `felupe-8.3.0/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_base.py` & `felupe-8.3.0/src/felupe/constitution/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_kinematics.py` & `felupe-8.3.0/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_mixed.py` & `felupe-8.3.0/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-8.3.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-8.3.0/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-8.3.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py` & `felupe-8.3.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-8.3.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_user_materials.py` & `felupe-8.3.0/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-8.3.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_user_materials_models.py` & `felupe-8.3.0/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/constitution/_view.py` & `felupe-8.3.0/src/felupe/constitution/_view.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/dof/_boundary.py` & `felupe-8.3.0/src/felupe/dof/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/dof/_loadcase.py` & `felupe-8.3.0/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/dof/_tools.py` & `felupe-8.3.0/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/__init__.py` & `felupe-8.3.0/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_base.py` & `felupe-8.3.0/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_hexahedron.py` & `felupe-8.3.0/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_lagrange.py` & `felupe-8.3.0/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_line.py` & `felupe-8.3.0/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_quad.py` & `felupe-8.3.0/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_tetra.py` & `felupe-8.3.0/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/element/_triangle.py` & `felupe-8.3.0/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_axi.py` & `felupe-8.3.0/src/felupe/field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_base.py` & `felupe-8.3.0/src/felupe/field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_container.py` & `felupe-8.3.0/src/felupe/field/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_dual.py` & `felupe-8.3.0/src/felupe/field/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_evaluate.py` & `felupe-8.3.0/src/felupe/field/_evaluate.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_fields.py` & `felupe-8.3.0/src/felupe/field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_indices.py` & `felupe-8.3.0/src/felupe/field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/field/_planestrain.py` & `felupe-8.3.0/src/felupe/field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/math/__init__.py` & `felupe-8.3.0/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/math/_field.py` & `felupe-8.3.0/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/math/_math.py` & `felupe-8.3.0/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/math/_spatial.py` & `felupe-8.3.0/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/math/_tensor.py` & `felupe-8.3.0/src/felupe/math/_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1342,24 +1342,27 @@
            [1.5, 1.4, 1.2]])
     
     >>> fem.math.tovoigt(C)[..., 0]
     array([1. , 1.1, 1.2, 1.3, 1.4, 1.5])
 
     """
     dim = A.shape[:2]
-    if dim == (2, 2):
+    if dim == (1, 1):
+        B = np.zeros((1, *A.shape[2:]))
+        ij = [(0, 0)]
+    elif dim == (2, 2):
         B = np.zeros((3, *A.shape[2:]))
         ij = [(0, 0), (1, 1), (0, 1)]
     elif dim == (3, 3):
         B = np.zeros((6, *A.shape[2:]))
         ij = [(0, 0), (1, 1), (2, 2), (0, 1), (1, 2), (0, 2)]
     else:
         raise TypeError("Input shape must be (2, 2, ...) or (3, 3, ...).")
-    for i6, (i, j) in enumerate(ij):
-        B[i6] = A[i, j]
+    for a, (i, j) in enumerate(ij):
+        B[a] = A[i, j]
     if strain:
         B[dim[0] :] *= 2
     return B
 
 
 def reshape(A, shape, trailing_axes=2):
     return A.reshape(np.append(shape, A.shape[-trailing_axes:]))
```

### Comparing `felupe-8.2.1/src/felupe/mechanics/__init__.py` & `felupe-8.3.0/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_curve.py` & `felupe-8.3.0/src/felupe/mechanics/_curve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_helpers.py` & `felupe-8.3.0/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_item.py` & `felupe-8.3.0/src/felupe/mechanics/_item.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_job.py` & `felupe-8.3.0/src/felupe/mechanics/_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_multipoint.py` & `felupe-8.3.0/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_pointload.py` & `felupe-8.3.0/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_solidbody.py` & `felupe-8.3.0/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-8.3.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-8.3.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-8.3.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mechanics/_step.py` & `felupe-8.3.0/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/__init__.py` & `felupe-8.3.0/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_container.py` & `felupe-8.3.0/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_convert.py` & `felupe-8.3.0/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_discrete_geometry.py` & `felupe-8.3.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_dual.py` & `felupe-8.3.0/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_geometry.py` & `felupe-8.3.0/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_helpers.py` & `felupe-8.3.0/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-8.3.0/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_mesh.py` & `felupe-8.3.0/src/felupe/mesh/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,61 @@
         -------
         meshio.Mesh
             The mesh as :class:`meshio.Mesh`.
         """
 
         import meshio
 
-        cells = {self.cell_type: self.cells}
-        return meshio.Mesh(self.points, cells, **kwargs)
+        points = np.pad(self.points, ((0, 0), (0, 3 - self.points.shape[1])))
+
+        return meshio.Mesh(points=points, cells={self.cell_type: self.cells}, **kwargs)
+
+    def as_pyvista(self, cell_type=None, **kwargs):
+        """Export the mesh as :class:`pyvista.UnstructuredGrid`.
+
+        Parameters
+        ----------
+        cell_type : pyvista.CellType or None, optional
+            Cell-type of PyVista (default is None).
+        **kwargs : dict, optional
+            Additional keyword-arguments for :class:`pyvista.UnstructuredGrid`.
+
+        Returns
+        -------
+        pyvista.UnstructuredGrid
+            The mesh as :class:`pyvista.UnstructuredGrid`.
+        """
+
+        import pyvista as pv
+
+        if cell_type is None:
+            cell_type = {
+                "line": pv.CellType.LINE,
+                "triangle": pv.CellType.TRIANGLE,
+                "triangle6": pv.CellType.QUADRATIC_TRIANGLE,
+                "tetra": pv.CellType.TETRA,
+                "tetra10": pv.CellType.QUADRATIC_TETRA,
+                "quad": pv.CellType.QUAD,
+                "quad8": pv.CellType.QUADRATIC_QUAD,
+                "quad9": pv.CellType.BIQUADRATIC_QUAD,
+                "hexahedron": pv.CellType.HEXAHEDRON,
+                "hexahedron20": pv.CellType.QUADRATIC_HEXAHEDRON,
+                "hexahedron27": pv.CellType.TRIQUADRATIC_HEXAHEDRON,
+                "VTK_LAGRANGE_HEXAHEDRON": pv.CellType.LAGRANGE_HEXAHEDRON,
+                "VTK_LAGRANGE_QUADRILATERAL": pv.CellType.LAGRANGE_QUADRILATERAL,
+                "VTK_LAGRANGE_LINE": pv.CellType.LAGRANGE_CURVE,
+            }[self.cell_type]
+
+        points = np.pad(self.points, ((0, 0), (0, 3 - self.points.shape[1])))
+        cells = np.pad(
+            self.cells, ((0, 0), (1, 0)), constant_values=self.cells.shape[1]
+        )
+        cell_types = cell_type * np.ones(self.ncells, dtype=int)
+
+        return pv.UnstructuredGrid(cells, cell_types, points)
 
     def write(self, filename="mesh.vtk", **kwargs):
         """Write the mesh to a file.
 
         Parameters
         ----------
         filename : str, optional
```

### Comparing `felupe-8.2.1/src/felupe/mesh/_read.py` & `felupe-8.3.0/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/mesh/_tools.py` & `felupe-8.3.0/src/felupe/mesh/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/quadrature/_gausslegendre.py` & `felupe-8.3.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/quadrature/_scheme.py` & `felupe-8.3.0/src/felupe/quadrature/_scheme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/quadrature/_sphere.py` & `felupe-8.3.0/src/felupe/quadrature/_sphere.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/quadrature/_tetra.py` & `felupe-8.3.0/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/quadrature/_triangle.py` & `felupe-8.3.0/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/region/__init__.py` & `felupe-8.3.0/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/region/_boundary.py` & `felupe-8.3.0/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/region/_region.py` & `felupe-8.3.0/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/region/_templates.py` & `felupe-8.3.0/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/solve/_solve.py` & `felupe-8.3.0/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/__init__.py` & `felupe-8.3.0/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_misc.py` & `felupe-8.3.0/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_newton.py` & `felupe-8.3.0/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_plot.py` & `felupe-8.3.0/src/felupe/tools/_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         plotter=None,
         notebook=False,
         extract_surface=False,
         nonlinear_subdivision=1,
         smooth_shading=True,
         split_sharp_edges=True,
         edge_color="black",
-        line_width=2.0,
+        line_width=1.0,
         **kwargs,
     ):
         """Plot scalars, selected by name and component.
 
         Parameters
         ----------
         name: str or None, optional
@@ -114,15 +114,15 @@
         split_sharp_edges : bool, optional
             A flag to split sharp edges (default is True). Use this flag in combination
             with smooth shading. Only considered if number of subdivisions is greater
             than 1.
         edge_color : str, optional
             The color of the edge lines (default is "black").
         line_width : float, optional
-            The line-width of the edge lines (default is 2.0).
+            The line-width of the edge lines (default is 1.0).
 
 
         Returns
         -------
         plotter : pyvista.Plotter
             A Plotter object with methods ``plot()``, ``screenshot()``, etc.
 
@@ -209,28 +209,34 @@
 
             else:
                 component_label = "Magnitude"
 
             label = f"{data_label} {component_label}"
 
         if show_undeformed:
-            plotter.add_mesh(self.mesh, show_edges=False, opacity=0.2)
+            plotter.add_mesh(
+                self.mesh, show_edges=False, opacity=0.2, line_width=line_width
+            )
 
         mesh = self.mesh
         if "Displacement" in self.mesh.point_data.keys():
             mesh = mesh.warp_by_vector("Displacement", factor=factor)
 
         surface = mesh
         show_edges_surface = show_edges
+        kwargs_with_line_width = {**kwargs}
+
         if mesh.number_of_cells > 0:
             if extract_surface or nonlinear_subdivision > 1:
                 surface = surface.extract_surface(
                     nonlinear_subdivision=nonlinear_subdivision
                 )
                 show_edges_surface = False
+            else:
+                kwargs_with_line_width["line_width"] = line_width
 
         # disable surface-related arguments if the mesh contains no cells
         if mesh.number_of_cells == 0 or nonlinear_subdivision == 1:
             smooth_shading = None
             split_sharp_edges = None
 
         # don't show edges for the base (surface) mesh to hide internal edges of
@@ -245,15 +251,15 @@
                 "title": label,
                 "interactive": True,
                 "vertical": scalar_bar_vertical,
                 **scalar_bar_args,
             },
             smooth_shading=smooth_shading,
             split_sharp_edges=split_sharp_edges,
-            **kwargs,
+            **kwargs_with_line_width,
         )
 
         # extract the feature edges (without cell-internal edges)
         if (
             mesh.number_of_cells > 0
             and show_edges
             and (extract_surface or nonlinear_subdivision > 1)
@@ -353,43 +359,15 @@
     mesh : pyvista.UnstructuredGrid
         A generalized Dataset with the mesh as well as point- and cell-data. This is
         not an instance of :class:`felupe.Mesh`.
 
     """
 
     def __init__(self, mesh, point_data=None, cell_data=None, cell_type=None):
-        import pyvista as pv
-
-        points = np.pad(mesh.points, ((0, 0), (0, 3 - mesh.points.shape[1])))
-        cells = np.pad(
-            mesh.cells, ((0, 0), (1, 0)), constant_values=mesh.cells.shape[1]
-        )
-
-        if cell_type is None:
-            pyvista_cell_types = {
-                "line": pv.CellType.LINE,
-                "triangle": pv.CellType.TRIANGLE,
-                "triangle6": pv.CellType.QUADRATIC_TRIANGLE,
-                "tetra": pv.CellType.TETRA,
-                "tetra10": pv.CellType.QUADRATIC_TETRA,
-                "quad": pv.CellType.QUAD,
-                "quad8": pv.CellType.QUADRATIC_QUAD,
-                "quad9": pv.CellType.BIQUADRATIC_QUAD,
-                "hexahedron": pv.CellType.HEXAHEDRON,
-                "hexahedron20": pv.CellType.QUADRATIC_HEXAHEDRON,
-                "hexahedron27": pv.CellType.TRIQUADRATIC_HEXAHEDRON,
-                "VTK_LAGRANGE_HEXAHEDRON": pv.CellType.LAGRANGE_HEXAHEDRON,
-                "VTK_LAGRANGE_QUADRILATERAL": pv.CellType.LAGRANGE_QUADRILATERAL,
-                "VTK_LAGRANGE_LINE": pv.CellType.LAGRANGE_CURVE,
-            }
-            cell_type = pyvista_cell_types[mesh.cell_type]
-
-        cell_types = cell_type * np.ones(mesh.ncells, dtype=int)
-
-        self.mesh = pv.UnstructuredGrid(cells, cell_types, points)
+        self.mesh = mesh.as_pyvista(cell_type=cell_type)
 
         if point_data is None:
             point_data = {}
 
         if cell_data is None:
             cell_data = {}
```

### Comparing `felupe-8.2.1/src/felupe/tools/_post.py` & `felupe-8.3.0/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_project.py` & `felupe-8.3.0/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_save.py` & `felupe-8.3.0/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe/tools/_solve.py` & `felupe-8.3.0/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/src/felupe.egg-info/PKG-INFO` & `felupe-8.3.0/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.2.1
+Version: 8.3.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-8.2.1/src/felupe.egg-info/SOURCES.txt` & `felupe-8.3.0/src/felupe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_basis.py` & `felupe-8.3.0/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_bilinearform.py` & `felupe-8.3.0/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_composite.py` & `felupe-8.3.0/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_constitution.py` & `felupe-8.3.0/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_dof.py` & `felupe-8.3.0/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_element.py` & `felupe-8.3.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_field.py` & `felupe-8.3.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_form.py` & `felupe-8.3.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_job.py` & `felupe-8.3.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_math.py` & `felupe-8.3.0/tests/test_math.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     fem.math.deformation_gradient(v)
 
     fem.math.norm([u.values, u.values])
     fem.math.norm(u.values)
     fem.math.interpolate(u)
     fem.math.grad(u)
     fem.math.grad(u, sym=True)
+    fem.math.tovoigt(fem.math.strain(v)[:1, :1])
     fem.math.tovoigt(fem.math.strain(v), strain=False)
     fem.math.tovoigt(fem.math.strain(v), strain=True)
     fem.math.strain(v)
     fem.math.extract(u)
     fem.math.extract(u, grad=False)
     fem.math.extract(u, sym=True)
     fem.math.extract(u, grad=True, sym=False, add_identity=False)
@@ -80,15 +81,19 @@
     fem.math.dot(A, C, mode=(4, 2))
 
     fem.math.transpose(F, mode=1)
     fem.math.transpose(A, mode=2)
 
     with pytest.raises(ValueError):
         fem.math.transpose(F, mode=3)
+
+    with pytest.raises(TypeError):
         fem.math.dot(A, B, mode=(4, 3))
+
+    with pytest.raises(TypeError):
         fem.math.dot(B, B, mode=(3, 3))
 
     fem.math.dot(C, B, mode=(2, 3))
     fem.math.dot(B, C, mode=(3, 2))
 
     assert fem.math.dot(C, a, mode=(2, 1)).shape == (3, 5, 7)
     assert fem.math.dot(a, C, mode=(1, 2)).shape == (3, 5, 7)
@@ -104,14 +109,16 @@
 
     assert fem.math.ddot(A, A, mode=(4, 4)).shape == (3, 3, 3, 3, 5, 7)
     assert fem.math.equivalent_von_mises(C).shape == (5, 7)
     assert fem.math.equivalent_von_mises(C[:2, :2, ...]).shape == (5, 7)
 
     with pytest.raises(TypeError):
         fem.math.ddot(A, B, mode=(4, 3))
+
+    with pytest.raises(TypeError):
         fem.math.ddot(B, B, mode=(3, 3))
 
     fem.math.ddot(C, B, mode=(2, 3))
     fem.math.ddot(B, C, mode=(3, 2))
 
     detC = fem.math.det(C)
     fem.math.det(C[:2, :2])
```

### Comparing `felupe-8.2.1/tests/test_mechanics.py` & `felupe-8.3.0/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_mesh.py` & `felupe-8.3.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_mpc.py` & `felupe-8.3.0/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_planestrain.py` & `felupe-8.3.0/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_plot.py` & `felupe-8.3.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_quadrature.py` & `felupe-8.3.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_readme.py` & `felupe-8.3.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_region.py` & `felupe-8.3.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_solve.py` & `felupe-8.3.0/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.2.1/tests/test_tools.py` & `felupe-8.3.0/tests/test_tools.py`

 * *Files identical despite different names*

