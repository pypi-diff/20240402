# Comparing `tmp/pyiron_atomistics-0.4.8.tar.gz` & `tmp/pyiron_atomistics-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_atomistics-0.4.8.tar", last modified: Mon Jan 22 17:58:44 2024, max compression
+gzip compressed data, was "pyiron_atomistics-0.4.9.tar", last modified: Tue Jan 30 13:54:06 2024, max compression
```

## Comparing `pyiron_atomistics-0.4.8.tar` & `pyiron_atomistics-0.4.9.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.136459 pyiron_atomistics-0.4.8/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.136459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.136459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.136459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41978 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23340 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)   124785 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/atomsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/has_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/structurestorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.140459 pyiron_atomistics-0.4.8/pyiron_atomistics/calphy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/calphy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/data/
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/data/periodic_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/bader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.144459 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/quasi_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.148459 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41239 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41929 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    24684 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    30134 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.148459 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    82876 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/input_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.148459 pyiron_atomistics-0.4.8/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.148459 pyiron_atomistics-0.4.8/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.148459 pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)    51126 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/sxphonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105337 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/metadyn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (127)    45420 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/outcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34571 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-22 17:58:44.000000 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-22 17:58:44.000000 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 17:58:44.000000 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-22 17:58:44.000000 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 17:58:44.000000 pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-01-22 17:58:35.000000 pyiron_atomistics-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 17:58:44.152459 pyiron_atomistics-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-22 17:56:51.000000 pyiron_atomistics-0.4.8/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.733376 pyiron_atomistics-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-30 13:54:06.733376 pyiron_atomistics-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.709376 pyiron_atomistics-0.4.9/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-30 13:54:06.733376 pyiron_atomistics-0.4.9/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.713376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.713376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.713376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41982 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.717376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23340 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.717376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124882 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.717376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.717376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.717376 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/data/periodic_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.721376 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.725376 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41269 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41931 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30134 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.725376 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82876 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/input_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16340 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.725376 pyiron_atomistics-0.4.9/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.729376 pyiron_atomistics-0.4.9/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.729376 pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51126 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.729376 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105429 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/metadyn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.729376 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45544 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.733376 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-30 13:54:06.000000 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-30 13:54:06.000000 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 13:54:06.000000 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-30 13:54:06.000000 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-30 13:54:06.000000 pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-01-30 13:53:58.000000 pyiron_atomistics-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 13:54:06.733376 pyiron_atomistics-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:54:06.729376 pyiron_atomistics-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-30 13:52:14.000000 pyiron_atomistics-0.4.9/tests/test_toolkit.py
```

### Comparing `pyiron_atomistics-0.4.8/LICENSE` & `pyiron_atomistics-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/PKG-INFO` & `pyiron_atomistics-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.4.8
+Version: 0.4.9
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,30 +46,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ase==3.22.1
-Requires-Dist: atomistics<=0.1.21,>=0.1.12
+Requires-Dist: atomistics<=0.1.22,>=0.1.12
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0
 Requires-Dist: h5py<=3.10.0,>=3.9.0
 Requires-Dist: matplotlib<=3.8.2,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.39.5,>=0.37.0
 Requires-Dist: numpy<=1.26.3,>=1.26.0
 Requires-Dist: pandas<=2.2.0,>=2.0.3
 Requires-Dist: phonopy<=2.21.0,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: pyiron_base<=0.7.1,>=0.6.16
 Requires-Dist: pylammpsmpi<=0.2.11,>=0.2.7
 Requires-Dist: scipy<=1.12.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.0,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
-Requires-Dist: spglib<=2.2.0,>=2.0.2
+Requires-Dist: spglib<=2.3.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.18,>=0.0.15
 
 pyiron
 ======
 
 .. image:: https://coveralls.io/repos/github/pyiron/pyiron_atomistics/badge.svg?branch=main
     :target: https://coveralls.io/github/pyiron/pyiron_atomistics?branch=main
```

### Comparing `pyiron_atomistics-0.4.8/README.rst` & `pyiron_atomistics-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/__init__.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/_tests.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,23 +255,23 @@
         initial_temperature=True,
         langevin=False,
     ):
         self._generic_input["calc_mode"] = "md"
         self._generic_input["temperature"] = temperature
         self._generic_input["n_ionic_steps"] = n_ionic_steps
         self._generic_input["n_print"] = n_print
-        self._generic_input[
-            "temperature_damping_timescale"
-        ] = temperature_damping_timescale
+        self._generic_input["temperature_damping_timescale"] = (
+            temperature_damping_timescale
+        )
         if pressure is not None:
             self._generic_input["pressure"] = pressure
         if pressure_damping_timescale is not None:
-            self._generic_input[
-                "pressure_damping_timescale"
-            ] = pressure_damping_timescale
+            self._generic_input["pressure_damping_timescale"] = (
+                pressure_damping_timescale
+            )
         if time_step is not None:
             self._generic_input["time_step"] = time_step
         self._generic_input.remove_keys(["max_iter"])
 
     def from_hdf(self, hdf=None, group_name=None):
         """
         Recreates instance from the hdf5 file
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/elastic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/elastic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,17 @@
 
         with self.project_hdf5.open("output") as hdf5_out:
             hdf5_out["dos_total"] = dos_dict["total_dos"]
             hdf5_out["dos_energies"] = dos_dict["frequency_points"]
             hdf5_out["qpoints"] = mesh_dict["qpoints"]
             hdf5_out["supercell_matrix"] = self._phonopy_supercell_matrix()
             hdf5_out["displacement_dataset"] = self.phonopy.get_displacement_dataset()
-            hdf5_out[
-                "dynamical_matrix"
-            ] = self.phonopy.dynamical_matrix.get_dynamical_matrix()
+            hdf5_out["dynamical_matrix"] = (
+                self.phonopy.dynamical_matrix.get_dynamical_matrix()
+            )
             hdf5_out["force_constants"] = self.phonopy.force_constants
 
     def write_phonopy_force_constants(self, file_name="FORCE_CONSTANTS", cwd=None):
         """
 
         Args:
             file_name:
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/master/structure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -2440,23 +2440,25 @@
                         )
                     )
                     and list(set(spin_lst))[0] is not None
                     and "[" in list(set(spin_lst))[0]
                 ):
                     return np.array(
                         [
-                            [
-                                float(spin_dir)
-                                for spin_dir in spin.replace("[", "")
-                                .replace("]", "")
-                                .replace(",", "")
-                                .split()
-                            ]
-                            if spin
-                            else [0.0, 0.0, 0.0]
+                            (
+                                [
+                                    float(spin_dir)
+                                    for spin_dir in spin.replace("[", "")
+                                    .replace("]", "")
+                                    .replace(",", "")
+                                    .split()
+                                ]
+                                if spin
+                                else [0.0, 0.0, 0.0]
+                            )
                             for spin in spin_lst
                         ]
                     )
                 elif isinstance(spin_lst, (list, np.ndarray)):
                     return np.array([float(s) if s else 0.0 for s in spin_lst])
                 else:
                     return np.array([float(spin) if spin else 0.0 for spin in spin_lst])
@@ -3127,17 +3129,17 @@
                     pyiron_atoms.add_tag(selective_dynamics=[True, True, True])
                 pyiron_atoms.selective_dynamics[
                     constraint_dict["kwargs"]["indices"]
                 ] = [False, False, False]
             elif constraint_dict["name"] == "FixScaled":
                 if "selective_dynamics" not in pyiron_atoms.arrays.keys():
                     pyiron_atoms.add_tag(selective_dynamics=[True, True, True])
-                pyiron_atoms.selective_dynamics[
-                    constraint_dict["kwargs"]["a"]
-                ] = constraint_dict["kwargs"]["mask"]
+                pyiron_atoms.selective_dynamics[constraint_dict["kwargs"]["a"]] = (
+                    constraint_dict["kwargs"]["mask"]
+                )
             else:
                 warnings.warn("Unsupported ASE constraint: " + constraint_dict["name"])
     return pyiron_atoms
 
 
 def pyiron_to_ase(pyiron_obj):
     element_list = pyiron_obj.get_parent_symbols()
@@ -3398,15 +3400,14 @@
             return None
         return newdata
     else:
         return data
 
 
 class Symbols(ASESymbols):
-
     """
     Derived from the ase symbols class which has the following docs:
 
     Args:
         numbers list/numpy.ndarray): List of atomic numbers
     """
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/atomsk.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/atomsk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/compound.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/compound.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factories/materialsproject.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factories/materialsproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/has_structure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/has_structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/structure/structurestorage.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/structure/structurestorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/calphy/job.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/calphy/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/data/periodic_table.csv` & `pyiron_atomistics-0.4.9/pyiron_atomistics/data/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/bader.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/bader.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "May 1, 2021"
 
 
 class Bader:
-
     """
     Module to apply the Bader charge partitioning scheme to finished DFT jobs. This module is interfaced with the
     `Bader code`_ from the Greame Henkelmann group.
 
     .. _Bader code: http://theory.cm.utexas.edu/henkelman/code/bader
     """
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/job/generic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/dos.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/dos.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
 
 class Dos(object):
-
     """
     The DOS class stores all information to store and retrieve the total and resolved density of states from an
     electronic structure calculation.
 
     Args:
         n_bins (int): Number of histogram bins required to calculate the DOS
         es_obj: The pyiron_atomistics.objects.waves.core.ElectronicStructure instance for which the DOS has to be computed
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/dft/waves/electronic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/dft/waves/electronic.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,17 +458,17 @@
                 n_atoms,
                 n_orbitals,
             )
             self._grand_dos_matrix = np.zeros(dimension)
             for spin in range(self.n_spins):
                 for i, kpt in enumerate(self.kpoints):
                     for j, band in enumerate(kpt.bands):
-                        self._grand_dos_matrix[
-                            spin, i, j, :, :
-                        ] = band.resolved_dos_matrix
+                        self._grand_dos_matrix[spin, i, j, :, :] = (
+                            band.resolved_dos_matrix
+                        )
         return self._grand_dos_matrix
 
     @grand_dos_matrix.setter
     def grand_dos_matrix(self, val):
         """
         Setter for grand_dos_matrix
         """
@@ -620,17 +620,17 @@
             n_spin, _, length = np.shape(self._eigenvalue_matrix)
             for spin in range(n_spin):
                 for j in range(length):
                     val = self.eigenvalue_matrix[spin][i][j]
                     occ = self.occupancy_matrix[spin][i][j]
                     self.kpoints[-1].add_band(eigenvalue=val, occupancy=occ, spin=spin)
                     if self._grand_dos_matrix is not None:
-                        self.kpoints[-1].bands[spin][
-                            -1
-                        ].resolved_dos_matrix = self.grand_dos_matrix[spin, i, j, :, :]
+                        self.kpoints[-1].bands[spin][-1].resolved_dos_matrix = (
+                            self.grand_dos_matrix[spin, i, j, :, :]
+                        )
 
     def get_spin_resolved_dos(self, spin_indices=0):
         """
         Gets the spin resolved DOS
 
         Args:
             spin_indices (int): The index of the spin for which the DOS is required
@@ -747,15 +747,14 @@
         return "\n".join(output_string)
 
     def __repr__(self):
         return self.__str__()
 
 
 class Kpoint(object):
-
     """
     All data related to a single k-point is stored in this module
 
 
     Attributes:
 
         bands (dict): Dict of pyiron_atomistics.objects.waves.settings.Band objects for each spin channel
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/gpaw.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/quasi_newton.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/quasi_newton.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,60 @@
 import warnings
 from pyiron_atomistics.atomistics.job.interactivewrapper import (
     InteractiveWrapper,
     ReferenceJobOutput,
 )
 
 
+def get_SR(dx, dg, H, threshold=1e-4):
+    """
+    Args:
+        dx ((n,)-numpy.ndarray/list): Change in positions
+        dg ((n,)-numpy.ndarray/list): Change in derivatives
+        H ((n,n)-numpy.ndarray/list): Current Hessian
+        threshold (float): Minimum value that the denominator can have (the
+            resulting Hessian matrix might explode if too small)
+
+    Returns:
+        ((n,n)-numpy.ndarray): Updated Hessian matrix
+    """
+    H_tmp = dg - np.einsum("ij,j->i", H, dx)
+    denominator = np.dot(H_tmp, dx)
+    if np.absolute(denominator) < threshold:
+        denominator += threshold
+    return np.outer(H_tmp, H_tmp) / denominator + H
+
+
+def get_PSB(dx, dg, H):
+    """
+    Args:
+        dx ((n,)-numpy.ndarray/list): Change in positions
+        dg ((n,)-numpy.ndarray/list): Change in derivatives
+        H ((n,n)-numpy.ndarray/list): Current Hessian
+
+    Returns:
+        ((n,n)-numpy.ndarray): Updated Hessian matrix
+    """
+    H_tmp = dg - np.einsum("ij,j->i", H, dx)
+    dxdx = np.einsum("i,i->", dx, dx)
+    dH = np.einsum("i,j->ij", H_tmp, dx)
+    dH = (dH + dH.T) / dxdx
+    return (
+        dH - np.einsum("i,i,j,k->jk", dx, H_tmp, dx, dx, optimize="optimal") / dxdx**2
+    ) + H
+
+
+def get_BFGS(dx, dg, H):
+    Hx = H.dot(dx)
+    return np.outer(dg, dg) / dg.dot(dx) - np.outer(Hx, Hx) / dx.dot(Hx) + H
+
+
+get_BFGS.__doc__ = get_PSB.__doc__
+
+
 class QuasiNewtonInteractive:
     """
     Interactive class of Quasi Newton. This class can be used without a pyiron job definition.
     After the initialization, the displacement is obtained by calling `get_dx` successively.
     """
 
     def __init__(
@@ -87,16 +133,15 @@
     def inv_hessian(self):
         if self.regularization is None:
             return np.linalg.inv(self.hessian)
         if self.use_eigenvalues:
             return np.einsum(
                 "ik,k,jk->ij",
                 self.eigenvectors,
-                self.eigenvalues
-                / (self.eigenvalues**2 + np.exp(self.regularization)),
+                self.eigenvalues / (self.eigenvalues**2 + np.exp(self.regularization)),
                 self.eigenvectors,
             )
         else:
             return np.linalg.inv(
                 self.hessian + np.eye(len(self.hessian)) * np.exp(self.regularization)
             )
 
@@ -140,50 +185,26 @@
         ):
             self._set_regularization(g=g.flatten())
             return self.get_dx(
                 g=g, threshold=threshold, mode=mode, update_hessian=False
             )
         return self.dx
 
-    @staticmethod
-    def _get_SR(dx, dg, H_tmp, threshold=1e-4):
-        denominator = np.dot(H_tmp, dx)
-        if np.absolute(denominator) < threshold:
-            denominator += threshold
-        return np.outer(H_tmp, H_tmp) / denominator
-
-    @staticmethod
-    def _get_PSB(dx, dg, H_tmp):
-        dxdx = np.einsum("i,i->", dx, dx)
-        dH = np.einsum("i,j->ij", H_tmp, dx)
-        dH = (dH + dH.T) / dxdx
-        return (
-            dH
-            - np.einsum("i,i,j,k->jk", dx, H_tmp, dx, dx, optimize="optimal")
-            / dxdx**2
-        )
-
-    @staticmethod
-    def _get_BFGS(dx, dg, H):
-        Hx = H.dot(dx)
-        return np.outer(dg, dg) / dg.dot(dx) - np.outer(Hx, Hx) / dx.dot(Hx)
-
     def update_hessian(self, g, threshold=1e-4, mode="PSB"):
         if self.g_old is None:
             self.g_old = g
             return
         dg = self.get_dg(g).flatten()
         dx = self.dx.flatten()
-        H_tmp = dg - np.einsum("ij,j->i", self.hessian, dx)
         if mode == "SR":
-            self.hessian = self._get_SR(dx, dg, H_tmp) + self.hessian
+            self.hessian = get_SR(dx, dg, self.hessian)
         elif mode == "PSB":
-            self.hessian = self._get_PSB(dx, dg, H_tmp) + self.hessian
+            self.hessian = get_PSB(dx, dg, self.hessian)
         elif mode == "BFGS":
-            self.hessian = self._get_BFGS(dx, dg, self.hessian) + self.hessian
+            self.hessian = get_BFGS(dx, dg, self.hessian)
         else:
             raise ValueError(
                 "Mode not recognized: {}. Choose from `SR`, `PSB` and `BFGS`".format(
                     mode
                 )
             )
         self.g_old = g
@@ -251,15 +272,14 @@
             job.run()
         else:
             job.run(delete_existing_job=True)
     return qn
 
 
 class QuasiNewton(InteractiveWrapper):
-
     """
     Structure optimization scheme via Quasi-Newton algorithm.
 
     Example:
 
     >>> from pyiron_atomistics import Project
     >>> spx = pr.create.job.Sphinx('spx')
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/base.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -362,17 +362,17 @@
         """
 
         Returns:
 
         """
         del self.input.control["dump_modify___1"]
         del self.input.control["dump___1"]
-        self.input.control[
-            "dump___1"
-        ] = "all h5md ${dumptime} dump.h5 position force create_group yes"
+        self.input.control["dump___1"] = (
+            "all h5md ${dumptime} dump.h5 position force create_group yes"
+        )
 
     def write_input(self):
         """
         Call routines that generate the code specific input files
 
         Returns:
 
@@ -893,87 +893,87 @@
                     not_constrained_xyz[np.setdiff1d(np.setdiff1d(ind_z, ind_x), ind_y)]
                     + 1
                 )
                 if len(constraint_xyz) > 0:
                     self.input.control["group___constraintxyz"] = "id " + " ".join(
                         [str(ind) for ind in constraint_xyz]
                     )
-                    self.input.control[
-                        "fix___constraintxyz"
-                    ] = "constraintxyz setforce 0.0 0.0 0.0"
+                    self.input.control["fix___constraintxyz"] = (
+                        "constraintxyz setforce 0.0 0.0 0.0"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintxyz"
-                        ] = "set 0.0 0.0 0.0"
+                        self.input.control["velocity___constraintxyz"] = (
+                            "set 0.0 0.0 0.0"
+                        )
                 if len(constraint_xy) > 0:
                     self.input.control["group___constraintxy"] = "id " + " ".join(
                         [str(ind) for ind in constraint_xy]
                     )
-                    self.input.control[
-                        "fix___constraintxy"
-                    ] = "constraintxy setforce 0.0 0.0 NULL"
+                    self.input.control["fix___constraintxy"] = (
+                        "constraintxy setforce 0.0 0.0 NULL"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintxy"
-                        ] = "set 0.0 0.0 NULL"
+                        self.input.control["velocity___constraintxy"] = (
+                            "set 0.0 0.0 NULL"
+                        )
                 if len(constraint_yz) > 0:
                     self.input.control["group___constraintyz"] = "id " + " ".join(
                         [str(ind) for ind in constraint_yz]
                     )
-                    self.input.control[
-                        "fix___constraintyz"
-                    ] = "constraintyz setforce NULL 0.0 0.0"
+                    self.input.control["fix___constraintyz"] = (
+                        "constraintyz setforce NULL 0.0 0.0"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintyz"
-                        ] = "set NULL 0.0 0.0"
+                        self.input.control["velocity___constraintyz"] = (
+                            "set NULL 0.0 0.0"
+                        )
                 if len(constraint_zx) > 0:
                     self.input.control["group___constraintxz"] = "id " + " ".join(
                         [str(ind) for ind in constraint_zx]
                     )
-                    self.input.control[
-                        "fix___constraintxz"
-                    ] = "constraintxz setforce 0.0 NULL 0.0"
+                    self.input.control["fix___constraintxz"] = (
+                        "constraintxz setforce 0.0 NULL 0.0"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintxz"
-                        ] = "set 0.0 NULL 0.0"
+                        self.input.control["velocity___constraintxz"] = (
+                            "set 0.0 NULL 0.0"
+                        )
                 if len(constraint_x) > 0:
                     self.input.control["group___constraintx"] = "id " + " ".join(
                         [str(ind) for ind in constraint_x]
                     )
-                    self.input.control[
-                        "fix___constraintx"
-                    ] = "constraintx setforce 0.0 NULL NULL"
+                    self.input.control["fix___constraintx"] = (
+                        "constraintx setforce 0.0 NULL NULL"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintx"
-                        ] = "set 0.0 NULL NULL"
+                        self.input.control["velocity___constraintx"] = (
+                            "set 0.0 NULL NULL"
+                        )
                 if len(constraint_y) > 0:
                     self.input.control["group___constrainty"] = "id " + " ".join(
                         [str(ind) for ind in constraint_y]
                     )
-                    self.input.control[
-                        "fix___constrainty"
-                    ] = "constrainty setforce NULL 0.0 NULL"
+                    self.input.control["fix___constrainty"] = (
+                        "constrainty setforce NULL 0.0 NULL"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constrainty"
-                        ] = "set NULL 0.0 NULL"
+                        self.input.control["velocity___constrainty"] = (
+                            "set NULL 0.0 NULL"
+                        )
                 if len(constraint_z) > 0:
                     self.input.control["group___constraintz"] = "id " + " ".join(
                         [str(ind) for ind in constraint_z]
                     )
-                    self.input.control[
-                        "fix___constraintz"
-                    ] = "constraintz setforce NULL NULL 0.0"
+                    self.input.control["fix___constraintz"] = (
+                        "constraintz setforce NULL NULL 0.0"
+                    )
                     if self._generic_input["calc_mode"] == "md":
-                        self.input.control[
-                            "velocity___constraintz"
-                        ] = "set NULL NULL 0.0"
+                        self.input.control["velocity___constraintz"] = (
+                            "set NULL NULL 0.0"
+                        )
 
     @staticmethod
     def _modify_structure_to_allow_requested_deformation(
         structure, pressure, prism=None
     ):
         """
         Lammps will not allow xy/xz/yz cell deformations in minimization or MD for non-triclinic cells. In case the
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/control.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,17 +812,17 @@
         for i, v in enumerate(vector):
             if v is None:
                 vector[i] = "NULL"
             else:
                 vector[i] = str(v * conversion)
         name = str(hash(tuple(ids))).replace("-", "m")  # A unique name for the group
         self._set_group_by_id(name, ids)
-        self[
-            "fix___{}_{}".format(fix_string.replace(" ", "_"), name)
-        ] = "{} {} {}".format(name, fix_string, " ".join(vector))
+        self["fix___{}_{}".format(fix_string.replace(" ", "_"), name)] = (
+            "{} {} {}".format(name, fix_string, " ".join(vector))
+        )
 
     def fix_move_linear_by_id(self, ids, velocity):
         """
         Displace atoms at each timestep. Creates a new group with a unique name based off the hash of the ids.
 
         Args:
             ids (list/numpy.ndarray): Integer ids of the atoms to move in the job's structure.
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/interactive.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,17 +270,17 @@
         Note: Do NOT overwrite `fexternal`, because it points to the internal memory of LAMMPS and
         therefore overwriting it will erase its functionality. E.g. DO `fexternal.fill(0)` and NOT
         `fexternal = np.zeros_like(x)`.
         """
         if not self.server.run_mode.interactive:
             raise AssertionError("Callback works only in interactive mode")
         self._user_fix_external = _FixExternal(function)
-        self.input.control[
-            "fix___fix_external"
-        ] = "all external pf/callback {} {}".format(n_call, n_apply)
+        self.input.control["fix___fix_external"] = (
+            "all external pf/callback {} {}".format(n_call, n_apply)
+        )
         if overload_internal_fix_external:
             self._user_fix_external.fix_external = function
 
     def calc_minimize(
         self,
         ionic_energy_tolerance=0.0,
         ionic_force_tolerance=1.0e-4,
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/lammps.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/output.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/potential.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
 class LammpsPotential(GenericParameters):
-
     """
     This module helps write commands which help in the control of parameters related to the potential used in LAMMPS
     simulations
     """
 
     def __init__(self, input_file_name=None):
         super(LammpsPotential, self).__init__(
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/structure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/lammps/units.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/lammps/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/project.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/base.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/input_writer.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/input_writer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/interactive.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/output_parser.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/output_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from functools import cached_property
 import numpy as np
 import re
 import scipy.constants
 from pathlib import Path
+import h5py
 import warnings
 
 
 BOHR_TO_ANGSTROM = (
     scipy.constants.physical_constants["Bohr radius"][0] / scipy.constants.angstrom
 )
 HARTREE_TO_EV = scipy.constants.physical_constants["Hartree energy in eV"][0]
@@ -416,7 +418,109 @@
             if key == "job_finished" or len(value) > 0:
                 results["generic"][key] = value
         for key, func in self.dft_dict.items():
             value = func()
             if len(value) > 0:
                 results["dft"][key] = value
         return results
+
+
+class SphinxWavesReader:
+    """Class to read SPHInX waves.sxb files (HDF5 format)
+
+    Initialize with waves.sxb filename, or use load ()
+
+    """
+
+    def __init__(self, file_name="waves.sxb", cwd="."):
+        """
+        Args:
+            file_name (str): file name
+            cwd (str): directory path
+        """
+        if Path(file_name).is_absolute():
+            self.wfile = h5py.File(Path(file_name))
+        else:
+            path = Path(cwd) / Path(file_name)
+            self.wfile = h5py.File(path)
+
+    @property
+    def _n_gk(self):
+        return self.wfile["nGk"][:]
+
+    @cached_property
+    def mesh(self):
+        return self.wfile["meshDim"][:]
+
+    @property
+    def Nx(self):
+        return self.mesh[0]
+
+    @property
+    def Ny(self):
+        return self.mesh[1]
+
+    @property
+    def Nz(self):
+        return self.mesh[2]
+
+    @cached_property
+    def n_states(self):
+        return self.wfile["nPerK"][0]
+
+    @cached_property
+    def n_spin(self):
+        return self.wfile["nSpin"].shape[0]
+
+    @cached_property
+    def k_weights(self):
+        return self.wfile["kWeights"][:]
+
+    @cached_property
+    def k_vec(self):
+        return self.wfile["kVec"][:]
+
+    @cached_property
+    def eps(self):
+        """All eigenvalues (in Hartree) as (nk,n_states) block"""
+        return (self.wfile["eps"][:].reshape(-1, self.n_spin, self.n_states)).T
+
+    @cached_property
+    def _fft_idx(self):
+        fft_idx = []
+        off = 0
+        for ngk in self._n_gk:
+            fft_idx.append(self.wfile["fftIdx"][off : off + ngk])
+            off += ngk
+        return fft_idx
+
+    def get_psi_rec(self, i, ispin, ik, compact=False):
+        """
+        Loads a single wavefunction on full FFT mesh of shape mesh.
+
+        params: i: state index (int)
+               ispin: spin index (int)
+               ik: k index (int)
+               compact: (bool)
+        returns:
+            res: complex valued wavefunction indexed by (i,ispin,ik) loaded on to the FFT mesh.
+            compact_wave: compact wavefunctions, without loading on FFT mesh.
+        """
+        # translate indices to pythonic style.
+        i = np.arange(self.n_states)[i]
+        ik = np.arange(self.nk)[ik]
+        ispin = np.arange(self.n_spin)[ispin]
+
+        off = self._n_gk[ik] * (i + ispin * self.n_states)
+        psire = self.wfile[f"psi-{ik+1}.re"][off : off + self._n_gk[ik]]
+        psiim = self.wfile[f"psi-{ik+1}.im"][off : off + self._n_gk[ik]]
+        compact_wave = psire + 1j * psiim
+        if compact:
+            return compact_wave
+        res = np.zeros(shape=self.mesh, dtype=np.complex128)
+        res.flat[self._fft_idx[ik]] = compact_wave
+        return res
+
+    @property
+    def nk(self):
+        """Number of k-points"""
+        return self.k_weights.shape[0]
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/potential.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/sphinx.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/structure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/util.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/table/datamining.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/table/funct.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/testing/executable.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/testing/randomatomistic.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/testing/randomatomistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,33 +463,25 @@
         return self._structure.cell.copy()
 
     @property
     def _s_r(self):
         return self.input["sigma"] / self.neigh.flattened.distances
 
     def interactive_energy_pot_getter(self):
-        return self.input["epsilon"] * (
-            np.sum(self._s_r**12) - np.sum(self._s_r**6)
-        )
+        return self.input["epsilon"] * (np.sum(self._s_r**12) - np.sum(self._s_r**6))
 
     def interactive_energy_tot_getter(self):
         return (
             self.interactive_energy_pot_getter() + self.interadtive_energy_kin_getter()
         )
 
     def interadtive_energy_kin_getter(self):
         v = np.einsum("ni,n->", self._velocity**2, self.structure.get_masses()) / 2
         return (
-            (
-                v
-                * self._unit.angstrom**2
-                / self._unit.second**2
-                / 1e-30
-                * self._unit.amu
-            )
+            (v * self._unit.angstrom**2 / self._unit.second**2 / 1e-30 * self._unit.amu)
             .to("eV")
             .magnitude
         )
 
     def interactive_forces_getter(self):
         all_values = self.input["epsilon"] * np.einsum(
             "ni,n,n->ni",
@@ -525,17 +517,15 @@
             )
             * self._unit.angstrom**2
             / self._unit.second**2
             / 1e-30
             * self._unit.amu
         )
         return (
-            (pot_part + kin_part)
-            / self.structure.get_volume()
-            / self._unit.angstrom**3
+            (pot_part + kin_part) / self.structure.get_volume() / self._unit.angstrom**3
         ).to(self._unit.pascal).magnitude / 1e9
 
     def interactive_stress_getter(self):
         return np.random.random((len(self._structure), 3, 3))
 
     def interactive_steps_getter(self):
         return len(self.interactive_cache["steps"])
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/toolkit.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/base.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,17 +454,17 @@
                     valence_charges = self._output_parser.generic_output.dft_log_dict[
                         "valence_charges"
                     ]
                     # Positive values indicate electron depletion
                     self._output_parser.generic_output.dft_log_dict["bader_charges"] = (
                         valence_charges - charges
                     )
-                self._output_parser.generic_output.dft_log_dict[
-                    "bader_volumes"
-                ] = volumes
+                self._output_parser.generic_output.dft_log_dict["bader_volumes"] = (
+                    volumes
+                )
         return self._output_parser.to_dict()
 
     # define routines that collect all output files
     def collect_output(self):
         """
         Collects the outputs and stores them to the hdf file
         """
@@ -835,34 +835,36 @@
             input_structure = self.structure.copy()
             try:
                 output_structure = read_atoms(
                     filename=filename,
                     species_list=input_structure.get_parent_symbols(),
                 )
                 input_structure.cell = output_structure.cell.copy()
-                input_structure.positions[
-                    self.sorted_indices
-                ] = output_structure.positions
+                input_structure.positions[self.sorted_indices] = (
+                    output_structure.positions
+                )
             except (IndexError, ValueError, IOError):
                 raise IOError("Unable to read output structure")
         return input_structure
 
     def write_magmoms(self):
         """
         Write the magnetic moments in INCAR from that assigned to the species
         """
         if self.structure.has("initial_magmoms"):
             if "ISPIN" not in self.input.incar._dataset["Parameter"]:
                 self.input.incar["ISPIN"] = 2
             if self.input.incar["ISPIN"] != 1:
                 final_cmd = "   ".join(
                     [
-                        " ".join([str(spinmom) for spinmom in spin])
-                        if isinstance(spin, (list, np.ndarray))
-                        else str(spin)
+                        (
+                            " ".join([str(spinmom) for spinmom in spin])
+                            if isinstance(spin, (list, np.ndarray))
+                            else str(spin)
+                        )
                         for spin in self.structure.get_initial_magnetic_moments()[
                             self.sorted_indices
                         ]
                     ]
                 )
                 state.logger.debug("Magnetic Moments are: {0}".format(final_cmd))
                 if "MAGMOM" not in self.input.incar._dataset["Parameter"]:
@@ -2049,20 +2051,20 @@
                 )
                 # magnetization[sorted_indices] = magnetization.copy()
                 if len(final_magmoms) != 0:
                     if len(final_magmoms.shape) == 3:
                         final_magmoms[:, sorted_indices, :] = final_magmoms.copy()
                     else:
                         final_magmoms[:, sorted_indices] = final_magmoms.copy()
-                self.generic_output.dft_log_dict[
-                    "magnetization"
-                ] = magnetization.tolist()
-                self.generic_output.dft_log_dict[
-                    "final_magmoms"
-                ] = final_magmoms.tolist()
+                self.generic_output.dft_log_dict["magnetization"] = (
+                    magnetization.tolist()
+                )
+                self.generic_output.dft_log_dict["final_magmoms"] = (
+                    final_magmoms.tolist()
+                )
             self.generic_output.dft_log_dict["e_fermi_list"] = self.outcar.parse_dict[
                 "e_fermi_list"
             ]
             self.generic_output.dft_log_dict["vbm_list"] = self.outcar.parse_dict[
                 "vbm_list"
             ]
             self.generic_output.dft_log_dict["cbm_list"] = self.outcar.parse_dict[
@@ -2116,17 +2118,17 @@
                 ] = self.electronic_structure.grand_dos_matrix[:, :, :, :, :].copy()
             if self.electronic_structure.resolved_densities is not None:
                 self.electronic_structure.resolved_densities[
                     :, sorted_indices, :, :
                 ] = self.electronic_structure.resolved_densities[:, :, :, :].copy()
             self.structure.positions = log_dict["positions"][-1]
             self.structure.set_cell(log_dict["cells"][-1])
-            self.generic_output.dft_log_dict[
-                "potentiostat_output"
-            ] = self.vp_new.get_potentiostat_output()
+            self.generic_output.dft_log_dict["potentiostat_output"] = (
+                self.vp_new.get_potentiostat_output()
+            )
             valence_charges_orig = self.vp_new.get_valence_electrons_per_atom()
             valence_charges = valence_charges_orig.copy()
             valence_charges[sorted_indices] = valence_charges_orig
             self.generic_output.dft_log_dict["valence_charges"] = valence_charges
 
         elif outcar_working:
             # log_dict = self.outcar.parse_dict.copy()
@@ -2150,17 +2152,17 @@
                 raise VaspCollectError("Improper OUTCAR parsing")
             log_dict["time"] = self.outcar.parse_dict["time"]
             log_dict["steps"] = self.outcar.parse_dict["steps"]
             log_dict["cells"] = self.outcar.parse_dict["cells"]
             log_dict["volume"] = np.array(
                 [np.linalg.det(cell) for cell in self.outcar.parse_dict["cells"]]
             )
-            self.generic_output.dft_log_dict[
-                "scf_energy_free"
-            ] = self.outcar.parse_dict["scf_energies"]
+            self.generic_output.dft_log_dict["scf_energy_free"] = (
+                self.outcar.parse_dict["scf_energies"]
+            )
             self.generic_output.dft_log_dict["scf_dipole_mom"] = self.outcar.parse_dict[
                 "scf_dipole_moments"
             ]
             self.generic_output.dft_log_dict["n_elect"] = self.outcar.parse_dict[
                 "n_elect"
             ]
             self.generic_output.dft_log_dict["energy_int"] = self.outcar.parse_dict[
@@ -2194,34 +2196,34 @@
                         ]
                 except ValueError:
                     pass
         # important that we "reverse sort" the atoms in the vasp format into the atoms in the atoms class
         self.generic_output.log_dict = log_dict
         if vasprun_working:
             # self.dft_output.log_dict["parameters"] = self.vp_new.vasprun_dict["parameters"]
-            self.generic_output.dft_log_dict[
-                "scf_dipole_mom"
-            ] = self.vp_new.vasprun_dict["scf_dipole_moments"]
+            self.generic_output.dft_log_dict["scf_dipole_mom"] = (
+                self.vp_new.vasprun_dict["scf_dipole_moments"]
+            )
             if len(self.generic_output.dft_log_dict["scf_dipole_mom"][0]) > 0:
                 total_dipole_moments = np.array(
                     [
                         dip[-1]
                         for dip in self.generic_output.dft_log_dict["scf_dipole_mom"]
                     ]
                 )
                 self.generic_output.dft_log_dict["dipole_mom"] = total_dipole_moments
-            self.generic_output.dft_log_dict[
-                "scf_energy_int"
-            ] = self.vp_new.vasprun_dict["scf_energies"]
-            self.generic_output.dft_log_dict[
-                "scf_energy_free"
-            ] = self.vp_new.vasprun_dict["scf_fr_energies"]
-            self.generic_output.dft_log_dict[
-                "scf_energy_zero"
-            ] = self.vp_new.vasprun_dict["scf_0_energies"]
+            self.generic_output.dft_log_dict["scf_energy_int"] = (
+                self.vp_new.vasprun_dict["scf_energies"]
+            )
+            self.generic_output.dft_log_dict["scf_energy_free"] = (
+                self.vp_new.vasprun_dict["scf_fr_energies"]
+            )
+            self.generic_output.dft_log_dict["scf_energy_zero"] = (
+                self.vp_new.vasprun_dict["scf_0_energies"]
+            )
             self.generic_output.dft_log_dict["energy_int"] = np.array(
                 [
                     e_int[-1]
                     for e_int in self.generic_output.dft_log_dict["scf_energy_int"]
                 ]
             )
             self.generic_output.dft_log_dict["energy_free"] = np.array(
@@ -2232,34 +2234,34 @@
             )
             # Overwrite energy_free with much better precision from the OSZICAR file
             if "energy_pot" in self.oszicar.parse_dict.keys():
                 if np.array_equal(
                     self.generic_output.dft_log_dict["energy_free"],
                     np.round(self.oszicar.parse_dict["energy_pot"], 8),
                 ):
-                    self.generic_output.dft_log_dict[
-                        "energy_free"
-                    ] = self.oszicar.parse_dict["energy_pot"]
+                    self.generic_output.dft_log_dict["energy_free"] = (
+                        self.oszicar.parse_dict["energy_pot"]
+                    )
             self.generic_output.dft_log_dict["energy_zero"] = np.array(
                 [
                     e_zero[-1]
                     for e_zero in self.generic_output.dft_log_dict["scf_energy_zero"]
                 ]
             )
             self.generic_output.dft_log_dict["n_elect"] = float(
                 self.vp_new.vasprun_dict["parameters"]["electronic"]["NELECT"]
             )
             if "kinetic_energies" in self.vp_new.vasprun_dict.keys():
                 # scf_energy_kin is for backwards compatibility
-                self.generic_output.dft_log_dict[
-                    "scf_energy_kin"
-                ] = self.vp_new.vasprun_dict["kinetic_energies"]
-                self.generic_output.dft_log_dict[
-                    "energy_kin"
-                ] = self.vp_new.vasprun_dict["kinetic_energies"]
+                self.generic_output.dft_log_dict["scf_energy_kin"] = (
+                    self.vp_new.vasprun_dict["kinetic_energies"]
+                )
+                self.generic_output.dft_log_dict["energy_kin"] = (
+                    self.vp_new.vasprun_dict["kinetic_energies"]
+                )
 
         if (
             "LOCPOT" in files_present
             and os.stat(posixpath.join(directory, "LOCPOT")).st_size != 0
         ):
             self.electrostatic_potential.from_file(
                 filename=posixpath.join(directory, "LOCPOT"), normalize=False
@@ -2279,17 +2281,17 @@
             "generic": self.generic_output.to_dict(),
         }
 
         if self._structure is not None:
             hdf5_output["structure"] = self.structure.to_dict()
 
         if self.electrostatic_potential.total_data is not None:
-            hdf5_output[
-                "electrostatic_potential"
-            ] = self.electrostatic_potential.to_dict()
+            hdf5_output["electrostatic_potential"] = (
+                self.electrostatic_potential.to_dict()
+            )
 
         if self.charge_density.total_data is not None:
             hdf5_output["charge_density"] = self.charge_density.to_dict()
 
         if len(self.electronic_structure.kpoint_list) > 0:
             hdf5_output["electronic_structure"] = self.electronic_structure.to_dict()
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/interactive.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/metadyn.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/oszicar.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/outcar.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/outcar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1146,20 +1146,22 @@
         )
         try:
             return [
                 np.array(
                     [
                         np.hstack(
                             [
-                                float(lines[ind + i].split()[-1])
-                                if i != 7
-                                else [
-                                    float(lines[ind_lst[-1] + 7].split()[-2]),
-                                    float(lines[ind_lst[-1] + 7].split()[-1]),
-                                ]
+                                (
+                                    float(lines[ind + i].split()[-1])
+                                    if i != 7
+                                    else [
+                                        float(lines[ind_lst[-1] + 7].split()[-2]),
+                                        float(lines[ind_lst[-1] + 7].split()[-1]),
+                                    ]
+                                )
                                 for i in range(2, 12)
                             ]
                         )
                         for ind in ind_lst
                     ]
                 ).T
                 for ind_lst in ind_combo_lst
@@ -1201,17 +1203,19 @@
         ind_elec_lst (list): indices of lines which matched the electronic pattern
 
     Returns:
         list: nested list of electronic pattern matches within an ionic pattern match
     """
     ind_elec_array = np.array(ind_elec_lst)
     return [
-        ind_elec_array[(ind_elec_array < j2) & (j1 < ind_elec_array)]
-        if j1 < j2
-        else ind_elec_array[(ind_elec_array < j2)]
+        (
+            ind_elec_array[(ind_elec_array < j2) & (j1 < ind_elec_array)]
+            if j1 < j2
+            else ind_elec_array[(ind_elec_array < j2)]
+        )
         for j1, j2 in zip(np.roll(ind_ionic_lst, 1), ind_ionic_lst)
     ]
 
 
 def _get_lines_from_file(filename, lines=None):
     """
     If lines is None read the lines from the file with the filename filename.
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/parser/report.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/parser/report.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/potential.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/procar.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/structure.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vasp.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vasprun.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vasprun.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
 class Vasprun(object):
-
     """
     This module is used to parse vasprun.xml files and store the data consistent with the pyiron input/output storage
     formats.
 
     Attributes:
 
         vasprun_dict (dict): Dictionary containing all information from the calculation parsed from the vasprun.xml
@@ -225,17 +224,17 @@
                                             species_key,
                                         )
                                         special_element = pse.element(species_key)
                                         species_dict[special_element] = dict()
                                         species_dict[special_element]["n_atoms"] = int(
                                             elements[0].text
                                         )
-                                        species_dict[special_element][
-                                            "valence"
-                                        ] = float(elements[3].text)
+                                        species_dict[special_element]["valence"] = (
+                                            float(elements[3].text)
+                                        )
                                 else:
                                     species_key = elements[1].text
                                     species_dict[species_key] = dict()
                                     species_dict[species_key]["n_atoms"] = int(
                                         elements[0].text
                                     )
                                     species_dict[species_key]["valence"] = float(
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/vaspsol.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron_atomistics-0.4.9/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.4.8
+Version: 0.4.9
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,30 +46,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ase==3.22.1
-Requires-Dist: atomistics<=0.1.21,>=0.1.12
+Requires-Dist: atomistics<=0.1.22,>=0.1.12
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0
 Requires-Dist: h5py<=3.10.0,>=3.9.0
 Requires-Dist: matplotlib<=3.8.2,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.39.5,>=0.37.0
 Requires-Dist: numpy<=1.26.3,>=1.26.0
 Requires-Dist: pandas<=2.2.0,>=2.0.3
 Requires-Dist: phonopy<=2.21.0,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: pyiron_base<=0.7.1,>=0.6.16
 Requires-Dist: pylammpsmpi<=0.2.11,>=0.2.7
 Requires-Dist: scipy<=1.12.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.0,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
-Requires-Dist: spglib<=2.2.0,>=2.0.2
+Requires-Dist: spglib<=2.3.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.18,>=0.0.15
 
 pyiron
 ======
 
 .. image:: https://coveralls.io/repos/github/pyiron/pyiron_atomistics/badge.svg?branch=main
     :target: https://coveralls.io/github/pyiron/pyiron_atomistics?branch=main
```

### Comparing `pyiron_atomistics-0.4.8/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron_atomistics-0.4.9/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/pyproject.toml` & `pyiron_atomistics-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "ase==3.22.1",
-    "atomistics>=0.1.12,<=0.1.21",
+    "atomistics>=0.1.12,<=0.1.22",
     "defusedxml>=0.7.0,<=0.7.1",
     "h5py>=3.9.0,<=3.10.0",
     "matplotlib>=3.5.3,<=3.8.2",
     "mendeleev>=0.12.0,<=0.15.0",
     "mp-api>=0.37.0,<=0.39.5",
     "numpy>=1.26.0,<=1.26.3",
     "pandas>=2.0.3,<=2.2.0",
     "phonopy>=2.20.0,<=2.21.0",
     "pint>=0.18,<=0.23",
     "pyiron_base>=0.6.16,<=0.7.1",
     "pylammpsmpi>=0.2.7,<=0.2.11",
     "scipy>=1.11.1,<=1.12.0",
     "scikit-learn>=1.2.1,<=1.4.0",
     "seekpath>=1.9.5,<=2.1.0",
-    "spglib>=2.0.2,<=2.2.0",
+    "spglib>=2.0.2,<=2.3.0",
     "structuretoolkit>=0.0.15,<=0.0.18",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://pyiron.org"
 Documentation = "https://pyiron.readthedocs.io"
```

### Comparing `pyiron_atomistics-0.4.8/tests/test_project.py` & `pyiron_atomistics-0.4.9/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.4.8/tests/test_toolkit.py` & `pyiron_atomistics-0.4.9/tests/test_toolkit.py`

 * *Files identical despite different names*

