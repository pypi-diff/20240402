# Comparing `tmp/goupil-1.0.0.tar.gz` & `tmp/goupil-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goupil-1.0.0.tar", last modified: Thu Mar 21 15:25:40 2024, max compression
+gzip compressed data, was "goupil-1.1.0.tar", last modified: Tue Apr  2 13:28:38 2024, max compression
```

## Comparing `goupil-1.0.0.tar` & `goupil-1.1.0.tar`

### file list

```diff
@@ -1,396 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.782150 goupil-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-21 15:25:34.000000 goupil-1.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-21 15:25:34.000000 goupil-1.0.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-21 15:25:34.000000 goupil-1.0.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-21 15:25:34.000000 goupil-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-21 15:25:40.782150 goupil-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-21 15:25:34.000000 goupil-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-21 15:25:34.000000 goupil-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-21 15:25:40.782150 goupil-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-21 15:25:34.000000 goupil-1.0.0/src/interfaces/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/interfaces/geant4/
--rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/interfaces/geant4/G4Goupil.cc
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-21 15:25:34.000000 goupil-1.0.0/src/interfaces/geant4/G4Goupil.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/interfaces/geant4/goupil.h
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/interfaces/goupil.h
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-21 15:25:34.000000 goupil-1.0.0/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/numerics/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/consts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/float.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/grids.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/integrate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/interpolate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/rand.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics/table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-21 15:25:34.000000 goupil-1.0.0/src/numerics.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/physics/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/consts.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.726150 goupil-1.0.0/src/physics/elements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/elements/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/elements/data/elements.rs
--rw-r--r--   0 runner    (1001) docker     (127)    75853 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/elements/data/shells.rs
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/elements/data.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/elements/serialise.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/elements.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/materials/
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/materials/electronic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/materials/table.rs
--rw-r--r--   0 runner    (1001) docker     (127)    26891 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/materials.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/process/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/process/absorption/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/absorption/table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/absorption.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/process/compton/
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/compton/compute.rs
--rw-r--r--   0 runner    (1001) docker     (127)    26983 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/compton/sample.rs
--rw-r--r--   0 runner    (1001) docker     (127)    22523 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/compton/table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/compton.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/physics/process/rayleigh/
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/rayleigh/sample.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/rayleigh/table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process/rayleigh.rs
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics/process.rs
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-21 15:25:34.000000 goupil-1.0.0/src/physics.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/python/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/density.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/elements.rs
--rw-r--r--   0 runner    (1001) docker     (127)    30255 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/geometry.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.730150 goupil-1.0.0/src/python/goupil/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.722150 goupil-1.0.0/src/python/goupil/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.722150 goupil-1.0.0/src/python/goupil/data/elements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.750150 goupil-1.0.0/src/python/goupil/data/elements/absorption/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ac.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ag.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Al.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Am.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ar.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/As.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/At.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:29.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Au.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ba.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Be.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Bi.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Bk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Br.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ca.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ce.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:37.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cf.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:10.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Co.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Cu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Dy.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Er.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-28 16:41:37.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Es.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Eu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/F.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:10.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Fe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-09-28 16:41:38.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Fm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Fr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ga.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Gd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ge.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:01.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:01.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/He.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:26.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Hf.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:29.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Hg.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ho.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-09-28 16:41:19.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/In.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:28.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Kr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/La.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Li.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Lu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Mg.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Mn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Mo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/N.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Na.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Nb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Nd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ne.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ni.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Np.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/O.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Os.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:06.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/P.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:34.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pa.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Po.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:28.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Pu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ra.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Rb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Re.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Rh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Rn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ru.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:06.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/S.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Sb.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Sc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Se.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Si.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Sm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Sn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Sr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:26.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ta.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Tb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Tc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-09-28 16:41:19.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Te.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Th.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Ti.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:30.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Tl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Tm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/W.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Xe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Y.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Yb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Zn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/absorption/Zr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.722150 goupil-1.0.0/src/python/goupil/data/elements/scattering/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.762150 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ac.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ag.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Al.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Am.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ar.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/As.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/At.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:29.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Au.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ba.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Be.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Bi.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Bk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Br.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ca.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ce.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:37.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cf.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:36.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:10.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Co.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Dy.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Er.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-09-28 16:41:37.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Es.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Eu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/F.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:10.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-09-28 16:41:38.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ga.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Gd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ge.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:01.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:01.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/He.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:26.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Hf.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:29.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Hg.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:24.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ho.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-09-28 16:41:19.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/In.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:28.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Kr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/La.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Li.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Lu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mg.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/N.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Na.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Nb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Nd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ne.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ni.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Np.txt
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/O.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Os.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:06.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/P.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:34.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pa.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:17.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pd.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-28 16:41:31.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Po.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-09-28 16:41:21.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:28.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ra.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Re.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:32.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ru.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:06.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/S.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sb.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Se.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:05.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Si.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:22.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:18.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:26.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ta.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-09-28 16:41:19.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Te.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-28 16:41:33.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Th.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ti.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:30.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:35.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:27.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/W.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-09-28 16:41:20.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Xe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Y.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Yb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:11.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Zn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Zr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.778150 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-09-28 15:22:13.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ac.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2023-09-28 15:21:56.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ag.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2023-09-28 15:21:42.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Al.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2023-09-28 15:22:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Am.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2023-09-28 15:21:44.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ar.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2023-09-28 15:21:50.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/As.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2023-09-28 15:22:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/At.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2023-09-28 15:22:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Au.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2023-09-28 15:21:40.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2023-09-28 15:22:00.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ba.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2023-09-28 15:21:40.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Be.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-09-28 15:22:11.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Bi.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2023-09-28 15:22:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Bk.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2023-09-28 15:21:50.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Br.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2023-09-28 15:21:40.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/C.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2023-09-28 15:21:45.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ca.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2023-09-28 15:21:57.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-09-28 15:22:01.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ce.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2023-09-28 15:22:17.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cf.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2023-09-28 15:21:44.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2023-09-28 15:22:16.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2023-09-28 15:21:47.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Co.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2023-09-28 15:21:46.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-09-28 15:22:00.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2023-09-28 15:21:48.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2023-09-28 15:22:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Dy.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2023-09-28 15:22:05.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Er.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2023-09-28 15:22:17.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Es.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2023-09-28 15:22:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Eu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2023-09-28 15:21:41.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/F.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-09-28 15:21:47.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2023-09-28 15:22:18.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2023-09-28 15:22:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2023-09-28 15:21:49.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ga.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Gd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2023-09-28 15:21:49.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ge.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2023-09-28 15:21:39.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15729 2023-09-28 15:21:39.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/He.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-09-28 15:22:06.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Hf.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2023-09-28 15:22:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Hg.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2023-09-28 15:22:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ho.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2023-09-28 15:21:59.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2023-09-28 15:21:57.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/In.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-09-28 15:22:08.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ir.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2023-09-28 15:21:45.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/K.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2023-09-28 15:21:51.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Kr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-09-28 15:22:01.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/La.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2023-09-28 15:21:40.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Li.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-09-28 15:22:06.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Lu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13089 2023-09-28 15:21:42.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mg.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-09-28 15:21:47.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2023-09-28 15:21:53.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mo.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13737 2023-09-28 15:21:41.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/N.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2023-09-28 15:21:42.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Na.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2023-09-28 15:21:52.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Nb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:02.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Nd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2023-09-28 15:21:42.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ne.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2023-09-28 15:21:48.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ni.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2023-09-28 15:22:15.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Np.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13521 2023-09-28 15:21:41.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/O.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-09-28 15:22:08.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Os.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2023-09-28 15:21:43.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/P.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-09-28 15:22:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pa.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-09-28 15:22:10.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2023-09-28 15:21:54.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:02.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-09-28 15:22:11.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Po.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-09-28 15:22:01.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-09-28 15:22:09.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2023-09-28 15:22:15.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-09-28 15:22:13.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ra.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-09-28 15:21:51.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-09-28 15:22:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Re.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2023-09-28 15:21:54.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2023-09-28 15:22:12.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-09-28 15:21:54.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ru.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2023-09-28 15:21:44.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/S.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2023-09-28 15:21:58.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2023-09-28 15:21:45.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-09-28 15:21:50.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Se.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2023-09-28 15:21:43.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Si.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2023-09-28 15:22:03.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2023-09-28 15:21:58.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-09-28 15:21:51.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2023-09-28 15:22:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ta.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2023-09-28 15:22:04.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2023-09-28 15:21:53.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2023-09-28 15:21:59.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Te.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2023-09-28 15:22:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Th.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2023-09-28 15:21:46.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ti.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-09-28 15:22:10.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9945 2023-09-28 15:22:05.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tm.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-09-28 15:22:14.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2023-09-28 15:21:46.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-09-28 15:22:07.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/W.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-09-28 15:21:59.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Xe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2023-09-28 15:21:52.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Y.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2023-09-28 15:22:06.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Yb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2023-09-28 15:21:48.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Zn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2023-09-28 15:21:52.000000 goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Zr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.778150 goupil-1.0.0/src/python/goupil/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/interfaces/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.782150 goupil-1.0.0/src/python/goupil/interfaces/geant4/
--rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/interfaces/geant4/G4Goupil.cc
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/interfaces/geant4/G4Goupil.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/interfaces/geant4/goupil.h
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/goupil/interfaces/goupil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.782150 goupil-1.0.0/src/python/goupil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-21 15:25:40.000000 goupil-1.0.0/src/python/goupil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-03-21 15:25:40.000000 goupil-1.0.0/src/python/goupil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:25:40.000000 goupil-1.0.0/src/python/goupil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-21 15:25:40.000000 goupil-1.0.0/src/python/goupil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 15:25:40.000000 goupil-1.0.0/src/python/goupil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48465 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/materials.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24275 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/numpy.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/process.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/rand.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24652 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python/transport.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-21 15:25:34.000000 goupil-1.0.0/src/python.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.782150 goupil-1.0.0/src/transport/
--rw-r--r--   0 runner    (1001) docker     (127)    23837 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/agent.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/density.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:40.782150 goupil-1.0.0/src/transport/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/geometry/external.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/geometry/simple.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21608 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/geometry/stratified.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport/geometry.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-03-21 15:25:34.000000 goupil-1.0.0/src/transport.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.922732 goupil-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-02 13:28:34.000000 goupil-1.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-02 13:28:34.000000 goupil-1.1.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 13:28:34.000000 goupil-1.1.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 13:28:34.000000 goupil-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-02 13:28:38.922732 goupil-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-02 13:28:34.000000 goupil-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-02 13:28:34.000000 goupil-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 13:28:38.922732 goupil-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.858731 goupil-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.858731 goupil-1.1.0/src/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 13:28:34.000000 goupil-1.1.0/src/interfaces/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/interfaces/geant4/
+-rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/interfaces/geant4/G4Goupil.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 13:28:34.000000 goupil-1.1.0/src/interfaces/geant4/G4Goupil.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/interfaces/geant4/goupil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/interfaces/goupil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-02 13:28:34.000000 goupil-1.1.0/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/numerics/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/consts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/float.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/grids.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/integrate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/interpolate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/rand.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics/table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-02 13:28:34.000000 goupil-1.1.0/src/numerics.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/consts.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/physics/elements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/physics/elements/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/elements/data/elements.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    75853 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/elements/data/shells.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/elements/data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/elements/serialise.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/elements.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.862731 goupil-1.1.0/src/physics/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/materials/electronic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/materials/table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/materials.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/physics/process/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/physics/process/absorption/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/absorption/table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/absorption.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/physics/process/compton/
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/compton/compute.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    26983 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/compton/sample.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    22523 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/compton/table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/compton.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/physics/process/rayleigh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/rayleigh/sample.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/rayleigh/table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process/rayleigh.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics/process.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 13:28:34.000000 goupil-1.1.0/src/physics.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/boundary.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/density.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/elements.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/geometry.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.866731 goupil-1.1.0/src/python/goupil/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.858731 goupil-1.1.0/src/python/goupil/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.858731 goupil-1.1.0/src/python/goupil/data/elements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.886731 goupil-1.1.0/src/python/goupil/data/elements/absorption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ac.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Al.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Am.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/As.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/At.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:29.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Au.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Be.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Bi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Bk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Br.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ca.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:37.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:10.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Co.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Cu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Dy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Er.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-28 16:41:37.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Es.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Eu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:10.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Fe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-09-28 16:41:38.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Fm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Fr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ga.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Gd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ge.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:01.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:01.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/He.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:26.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Hf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:29.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Hg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ho.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-09-28 16:41:19.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/In.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:28.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Kr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/La.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Li.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Lu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Mg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Mn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Mo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/N.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Na.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Nb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Nd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ne.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ni.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Np.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Os.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:06.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:34.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Po.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:28.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Pu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Rb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Re.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Rh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Rn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ru.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:06.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/S.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Sb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Sc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Se.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Sm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Sn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Sr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:26.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ta.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Tb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Tc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-09-28 16:41:19.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Te.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Th.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Ti.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:30.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Tl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Tm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/W.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Xe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Y.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Yb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Zn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/absorption/Zr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.858731 goupil-1.1.0/src/python/goupil/data/elements/scattering/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.902731 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ac.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Al.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Am.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/As.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/At.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:29.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Au.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Be.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Bi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Bk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Br.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ca.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:37.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-28 16:41:36.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:10.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Co.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Dy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Er.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-09-28 16:41:37.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Es.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Eu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:10.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-09-28 16:41:38.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ga.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Gd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ge.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:01.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:01.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/He.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:26.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Hf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:29.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Hg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:24.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ho.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-09-28 16:41:19.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/In.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:28.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Kr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/La.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:02.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Li.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Lu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/N.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Na.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Nb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Nd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ne.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ni.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Np.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-28 16:41:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Os.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:06.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:34.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:17.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-28 16:41:31.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Po.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-09-28 16:41:21.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:28.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Re.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:32.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ru.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:06.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/S.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:13.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Se.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:05.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-28 16:41:22.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:18.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:26.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ta.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:23.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-28 16:41:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-09-28 16:41:19.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Te.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-28 16:41:33.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Th.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:08.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ti.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:30.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-28 16:41:35.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-28 16:41:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-09-28 16:41:27.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/W.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-09-28 16:41:20.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Xe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Y.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-28 16:41:25.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Yb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-28 16:41:11.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Zn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 16:41:15.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Zr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.918732 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-09-28 15:22:13.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ac.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2023-09-28 15:21:56.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2023-09-28 15:21:42.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Al.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2023-09-28 15:22:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Am.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2023-09-28 15:21:44.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2023-09-28 15:21:50.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/As.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2023-09-28 15:22:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/At.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2023-09-28 15:22:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Au.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2023-09-28 15:21:40.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2023-09-28 15:22:00.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2023-09-28 15:21:40.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Be.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-09-28 15:22:11.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Bi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2023-09-28 15:22:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Bk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2023-09-28 15:21:50.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Br.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2023-09-28 15:21:40.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2023-09-28 15:21:45.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ca.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2023-09-28 15:21:57.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-09-28 15:22:01.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2023-09-28 15:22:17.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2023-09-28 15:21:44.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2023-09-28 15:22:16.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2023-09-28 15:21:47.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Co.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2023-09-28 15:21:46.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-09-28 15:22:00.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2023-09-28 15:21:48.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2023-09-28 15:22:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Dy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2023-09-28 15:22:05.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Er.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2023-09-28 15:22:17.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Es.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2023-09-28 15:22:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Eu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2023-09-28 15:21:41.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-09-28 15:21:47.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2023-09-28 15:22:18.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2023-09-28 15:22:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2023-09-28 15:21:49.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ga.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Gd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2023-09-28 15:21:49.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ge.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2023-09-28 15:21:39.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15729 2023-09-28 15:21:39.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/He.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-09-28 15:22:06.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Hf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2023-09-28 15:22:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Hg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2023-09-28 15:22:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ho.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2023-09-28 15:21:59.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2023-09-28 15:21:57.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/In.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-09-28 15:22:08.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2023-09-28 15:21:45.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2023-09-28 15:21:51.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Kr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-09-28 15:22:01.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/La.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2023-09-28 15:21:40.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Li.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-09-28 15:22:06.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Lu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13089 2023-09-28 15:21:42.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-09-28 15:21:47.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2023-09-28 15:21:53.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2023-09-28 15:21:41.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/N.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2023-09-28 15:21:42.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Na.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2023-09-28 15:21:52.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Nb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:02.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Nd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2023-09-28 15:21:42.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ne.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2023-09-28 15:21:48.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ni.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2023-09-28 15:22:15.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Np.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2023-09-28 15:21:41.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-09-28 15:22:08.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Os.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2023-09-28 15:21:43.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-09-28 15:22:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-09-28 15:22:10.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2023-09-28 15:21:54.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-28 15:22:02.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-09-28 15:22:11.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Po.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-09-28 15:22:01.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-09-28 15:22:09.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2023-09-28 15:22:15.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-09-28 15:22:13.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-09-28 15:21:51.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-09-28 15:22:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Re.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2023-09-28 15:21:54.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2023-09-28 15:22:12.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10809 2023-09-28 15:21:54.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ru.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2023-09-28 15:21:44.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/S.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2023-09-28 15:21:58.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2023-09-28 15:21:45.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-09-28 15:21:50.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Se.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2023-09-28 15:21:43.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2023-09-28 15:22:03.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2023-09-28 15:21:58.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-09-28 15:21:51.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2023-09-28 15:22:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ta.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2023-09-28 15:22:04.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2023-09-28 15:21:53.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2023-09-28 15:21:59.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Te.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2023-09-28 15:22:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Th.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2023-09-28 15:21:46.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ti.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-09-28 15:22:10.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9945 2023-09-28 15:22:05.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-09-28 15:22:14.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2023-09-28 15:21:46.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-09-28 15:22:07.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/W.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-09-28 15:21:59.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Xe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2023-09-28 15:21:52.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Y.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2023-09-28 15:22:06.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Yb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2023-09-28 15:21:48.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Zn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2023-09-28 15:21:52.000000 goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Zr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.918732 goupil-1.1.0/src/python/goupil/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/interfaces/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.918732 goupil-1.1.0/src/python/goupil/interfaces/geant4/
+-rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/interfaces/geant4/G4Goupil.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/interfaces/geant4/G4Goupil.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/interfaces/geant4/goupil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/goupil/interfaces/goupil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.922732 goupil-1.1.0/src/python/goupil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-02 13:28:38.000000 goupil-1.1.0/src/python/goupil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-04-02 13:28:38.000000 goupil-1.1.0/src/python/goupil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:28:38.000000 goupil-1.1.0/src/python/goupil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 13:28:38.000000 goupil-1.1.0/src/python/goupil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 13:28:38.000000 goupil-1.1.0/src/python/goupil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48465 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/materials.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/numpy.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/process.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/rand.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/spectrum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25788 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python/transport.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-02 13:28:34.000000 goupil-1.1.0/src/python.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.918732 goupil-1.1.0/src/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)    23695 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/agent.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/boundary.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/density.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:28:38.918732 goupil-1.1.0/src/transport/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/geometry/external.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/geometry/simple.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/geometry/stratified.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport/geometry.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-02 13:28:34.000000 goupil-1.1.0/src/transport.rs
```

### Comparing `goupil-1.0.0/COPYING` & `goupil-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/COPYING.LESSER` & `goupil-1.1.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/Cargo.toml` & `goupil-1.1.0/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "goupil"
-version = "1.0.0"
+version = "1.1.0"
 edition = "2021"
 license = "LGPL-3.0-only AND MIT"
 
 [dependencies]
 anyhow = "1"
 enum-iterator = "1.4"
 libloading = "0.8"
```

### Comparing `goupil-1.0.0/PKG-INFO` & `goupil-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: goupil
-Version: 1.0.0
-Summary: A backward accelerator for gamma rays transport.
+Version: 1.1.0
+Summary: A Monte Carlo engine for the backward transport of low energy gamma-rays.
 Author-email: Valentin Niess <valentin.niess@gmail.com>
 License: LGPLv3
 Project-URL: source, https://github.com/niess/goupil
 Keywords: gamma rays,Monte Carlo,backward
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7.0
@@ -27,12 +27,14 @@
 
 Documentation for Goupil can be found online at [Read the Docs][RTD].
 
 ## License
 
 The Goupil library is  under the **GNU LGPLv3** license (see the provided
 [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER) files), except for
-[interfaces](src/interfaces) which are MIT-licensed.
+[examples][EXAMPLES] and [interfaces][INTERFACES] which are MIT-licensed.
 
 
+[EXAMPLES]: https://github.com/niess/goupil/tree/master/examples
+[INTERFACES]: https://github.com/niess/goupil/tree/master/src/interfaces
 [RTD]: https://goupil.readthedocs.io/en/latest/
 [RTD_BADGE]: https://readthedocs.org/projects/goupil/badge/?version=latest
```

### Comparing `goupil-1.0.0/pyproject.toml` & `goupil-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "goupil"
 authors = [
     {name = "Valentin Niess", email = "valentin.niess@gmail.com"}
 ]
-description = "A backward accelerator for gamma rays transport."
+description = "A Monte Carlo engine for the backward transport of low energy gamma-rays."
 readme = "README.md"
 license = {text = "LGPLv3"}
 keywords = ["gamma rays", "Monte Carlo", "backward"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics"
 ]
-version = "1.0.0"
+version = "1.1.0"
 requires-python = ">=3.7.0"
 dependencies = [
     "numpy >= 1.6.0",
 ]
 
 [project.urls]
 source = "https://github.com/niess/goupil"
```

### Comparing `goupil-1.0.0/src/interfaces/LICENSE` & `goupil-1.1.0/src/interfaces/LICENSE`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/interfaces/geant4/G4Goupil.cc` & `goupil-1.1.0/src/interfaces/geant4/G4Goupil.cc`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/interfaces/geant4/goupil.h` & `goupil-1.1.0/src/interfaces/geant4/goupil.h`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/interfaces/goupil.h` & `goupil-1.1.0/src/interfaces/goupil.h`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/lib.rs` & `goupil-1.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics/consts.rs` & `goupil-1.1.0/src/numerics/consts.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics/float.rs` & `goupil-1.1.0/src/transport/boundary.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,331 +1,256 @@
-use std::fmt;
-use std::ops::{Add, AddAssign, Div, DivAssign, Mul, MulAssign, Neg, Sub, SubAssign};
+use crate::numerics::float::{Float, Float3, Float3x3};
+use serde_derive::{Deserialize, Serialize};
 
 
-//================================================================================================
-// Floating point type (defined at compilation).
-//================================================================================================
-#[cfg(not(feature = "f32"))]
-pub type Float = f64;
-#[cfg(feature = "f32")]
-pub type Float = f32;
-
-
-//================================================================================================
-// Vectorized floating point type.
-//================================================================================================
-#[derive(Copy, Clone, Default, PartialEq)]
-pub struct Float3 (pub Float, pub Float, pub Float);
+// ===============================================================================================
+// External boundaries.
+// ===============================================================================================
+
+#[derive(Clone, Copy, Default, Deserialize, Serialize)]
+pub enum TransportBoundary {
+    #[default]
+    None,
+    Box(BoxShape),
+    Sector(usize),
+    Sphere(SphereShape),
+}
 
-impl Float3 {
-    // Constructors.
-    pub const fn new(x: Float, y: Float, z: Float) -> Float3 { Float3(x, y, z) }
-    pub const fn splat(x: Float) -> Float3 { Float3(x, x, x) }
-    pub const fn zero() -> Float3 { Float3(0.0, 0.0, 0.0) }
-
-    // L2-norm and related functions.
-    pub fn norm(self) -> Float {
-        self.dot(self).sqrt()
-    }
-    pub fn norm2(self) -> Float {
-        (self.0 * self.0 + self.1 * self.1) + self.2 * self.2
-    }
-    pub fn normalise(&mut self) {
-        *self /= self.norm();
-    }
-    pub fn unit(self) -> Self {
-        self / self.norm()
+impl TransportBoundary {
+    pub fn distance(&self, position: Float3, direction: Float3) -> Float {
+        let distance = match self {
+            Self::Box(shape) => shape.distance(position, direction),
+            Self::Sphere(shape) => shape.distance(position, direction),
+            _ => None,
+        };
+        distance.unwrap_or(Float::INFINITY)
     }
 
-    // Inner and outer products.
-    pub fn dot(self, rhs: Self) -> Float {
-        (self.0 * rhs.0 + self.1 * rhs.1) + self.2 * rhs.2
-    }
-    pub fn cross(self, rhs: Self) -> Self {
-        Self (
-            self.1 * rhs.2 - self.2 * rhs.1,
-            self.2 * rhs.0 - self.0 * rhs.2,
-            self.0 * rhs.1 - self.1 * rhs.0,
-        )
+    pub fn inside(&self, position: Float3, sector: usize) -> bool {
+        match self {
+            Self::None => false,
+            Self::Box(shape) => shape.inside(position),
+            Self::Sector(index) => *index == sector,
+            Self::Sphere(shape) => shape.inside(position),
+        }
     }
+}
 
-    // In-place transforms.
-    pub fn reverse(&mut self) {
-        *self = Self (-self.0, -self.1, -self.2);
-    }
-    pub fn rotate(&mut self, cos_theta: Float, phi: Float) {
-        // Compute (and check) the sine.
-        let sin_theta = {
-            let stsq = 1.0 - cos_theta * cos_theta;
-            if stsq < 0.0 { return }
-            stsq.sqrt()
-        };
 
-        // Get norm and unit vector.
-        let norm = self.norm();
-        let direction = *self / norm;
-
-        // Generate co-vectors for the local basis.
-        let e: Float3 = {
-            let a0 = direction.0.abs();
-            let a1 = direction.1.abs();
-            let a2 = direction.2.abs();
-
-            if a0 < a1 {
-                if a0 < a2 {
-                    Float3::new(1.0, 0.0, 0.0)
-                } else {
-                    Float3::new(0.0, 0.0, 1.0)
-                }
-            } else {
-                if a1 < a2 {
-                    Float3::new(0.0, 1.0, 0.0)
-                } else {
-                    Float3::new(0.0, 0.0, 1.0)
-                }
-            }
-        };
+// ===============================================================================================
+// Generic geometry shape.
+// ===============================================================================================
+
+pub trait GeometryShape {
+    /// Returns the distance to the shape, starting from *position* and along the given
+    /// *direction*.
+    fn distance(&self, position: Float3, direction: Float3) -> Option<Float>;
 
-        let mut u0 = direction.cross(e);
-        u0.normalise();
-        let u1 = u0.cross(direction);
-
-        // Apply the rotation.
-        *self = (norm * cos_theta) * direction +
-                (norm * sin_theta) * (phi.cos() * u0 + phi.sin() * u1);
-    }
+    /// Indicates wether or not the given *position* is inside the shape.
+    fn inside(&self, position: Float3) -> bool;
 }
 
-impl fmt::Display for Float3 {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "({}, {}, {})", self.0, self.1, self.2)
-    }
+
+// ===============================================================================================
+// Box shape.
+// ===============================================================================================
+
+#[derive(Clone, Copy, Default, PartialEq, Deserialize, Serialize)]
+pub struct BoxShape {
+    pub center: Float3,
+    pub size: Float3,
+    pub rotation: Option<Float3x3>,
 }
 
-macro_rules! impl_binary_operator {
-    ($trait:ident, $func:ident, $op:tt) => {
-        impl $trait for Float3 {
-            type Output = Self;
-            fn $func (self, rhs: Self) -> Self {
-                Self (self.0 $op rhs.0, self.1 $op rhs.1, self.2 $op rhs.2)
+impl GeometryShape for BoxShape {
+    fn distance(&self, position: Float3, direction: Float3) -> Option<Float> {
+        let (v, u) = {
+            let v = position - self.center;
+            match self.rotation.as_ref() {
+                None => (v, direction),
+                Some(rotation) => (v * rotation, direction * rotation),
             }
-        }
-        impl $trait<Float3> for Float {
-            type Output = Float3;
-            fn $func (self, rhs: Float3) -> Float3 {
-                Float3 (self $op rhs.0, self $op rhs.1, self $op rhs.2)
-            }
-        }
-        impl $trait<Float> for Float3 {
-            type Output = Self;
-            fn $func (self, rhs: Float) -> Self {
-                Self (self.0 $op rhs, self.1 $op rhs, self.2 $op rhs)
+        };
+
+        // Intersection with an axis aligned box, avoiding (some) branchings.
+        // Ref: https://tavianator.com/2011/ray_box.html
+        let mut tmin = -Float::INFINITY;
+        let mut tmax = Float::INFINITY;
+        let mut update = |x: &Float, hx: Float, ux: &Float| {
+            if *ux != 0.0 {
+                let uxinv = 1.0 / ux;
+                let tx1 = (-hx - x) * uxinv;
+                let tx2 = (hx - x) * uxinv;
+                tmin = tmin.max(tx1.min(tx2));
+                tmax = tmax.min(tx1.max(tx2));
             }
+        };
+        update(&v.0, 0.5 * self.size.0, &u.0);
+        update(&v.1, 0.5 * self.size.1, &u.1);
+        update(&v.2, 0.5 * self.size.2, &u.2);
+        if tmin <= 0.0 {
+            if tmax > 0.0 { Some(tmax) } else { None }
+        } else if tmax >= tmin {
+            Some(tmin)
+        } else {
+            None
         }
     }
-}
-
-impl_binary_operator!(Add, add, +);
-impl_binary_operator!(Mul, mul, *);
-impl_binary_operator!(Sub, sub, -);
-
-impl Div<Float> for Float3 {
-    type Output = Self;
-    fn div(self, rhs: Float) -> Self {
-        let tmp = 1.0 / rhs;
-        Self (self.0 * tmp, self.1 * tmp, self.2 * tmp)
-    }
-}
 
-macro_rules! impl_assign_operator {
-    ($trait:ident, $func:ident, $op:tt) => {
-        impl $trait for Float3 {
-            fn $func (&mut self, rhs: Self) {
-                *self = Self (self.0 $op rhs.0, self.1 $op rhs.1, self.2 $op rhs.2);
+    fn inside(&self, position: Float3) -> bool {
+        let r = {
+            let mut r = position - self.center;
+            if let Some(rotation) = self.rotation.as_ref() {
+                r = r * rotation
             }
-        }
-        impl $trait<Float> for Float3 {
-            fn $func (&mut self, rhs: Float) {
-                *self = Self (self.0 $op rhs, self.1 $op rhs, self.2 $op rhs);
-            }
-        }
+            r
+        };
+        (r.0.abs() < 0.5 * self.size.0) &&
+        (r.1.abs() < 0.5 * self.size.1) &&
+        (r.2.abs() < 0.5 * self.size.2)
     }
 }
 
-impl_assign_operator!(AddAssign, add_assign, +);
-impl_assign_operator!(MulAssign, mul_assign, *);
-impl_assign_operator!(SubAssign, sub_assign, -);
-
-impl DivAssign<Float> for Float3 {
-    fn div_assign(&mut self, rhs: Float) {
-        let tmp = 1.0 / rhs;
-        *self = Self (self.0 * tmp, self.1 * tmp, self.2 * tmp);
-    }
-}
 
-impl Neg for Float3 {
-    type Output = Self;
-    fn neg(self) -> Self {
-        Self (-self.0, -self.1, -self.2)
-    }
+// ===============================================================================================
+// Spherical shape.
+// ===============================================================================================
+
+#[derive(Clone, Copy, Default, PartialEq, Deserialize, Serialize)]
+pub struct SphereShape {
+    pub center: Float3,
+    pub radius: Float,
 }
 
-impl From<[Float; 3]> for Float3 {
-    fn from(array: [Float; 3]) -> Self {
-        Self::new(array[0], array[1], array[2])
+impl GeometryShape for SphereShape {
+    fn distance(&self, position: Float3, direction: Float3) -> Option<Float> {
+        let v = self.center - position;
+        let vu = v.dot(direction);
+        let h2 = v.norm2() - vu * vu;
+        let r2 = self.radius * self.radius;
+        if h2 > r2 {
+            // No intersection case.
+            None
+        } else if h2 == r2 {
+            // Tangent intersection case.
+            if vu > 0.0 {
+                Some(vu)
+            } else {
+                None
+            }
+        } else {
+            // Two intersections case.
+            let delta = (r2 - h2).sqrt();
+            let d0 = vu + delta;
+            if d0 > 0.0 {
+                let d1 = vu - delta;
+                if d1 > 0.0 {
+                    Some(d1)
+                } else {
+                    Some(d0)
+                }
+            } else {
+                None
+            }
+        }
     }
-}
 
-impl From<Float3> for [Float; 3] {
-    fn from(array: Float3) -> Self {
-        [array.0, array.1, array.2]
+    fn inside(&self, position: Float3) -> bool {
+        (position - self.center).norm2() < self.radius * self.radius
     }
 }
 
 
 //================================================================================================
 // Unit tests.
 //================================================================================================
 #[cfg(test)]
 mod tests {
-    use super::super::consts::{FRAC_1_SQRT_2, PI};
-    use super::super::tests::{assert_float_eq, assert_float3_eq};
+    use crate::numerics::tests::assert_float_eq;
     use super::*;
 
     #[test]
-    fn add() {
-        let mut v0 = Float3::new(1.0, 2.0, 3.0);
-        let mut v1 = Float3::new(4.0, 5.0, 6.0);
-        const V2: Float3 = Float3::new(5.0, 7.0, 9.0);
-        assert!(v0 + v1 == V2);
-        assert!(v0 + 1.0 == v0 + Float3::splat(1.0));
-        assert!(1.0 + v0 == Float3::splat(1.0) + v0);
-
-        v0 += v1;
-        assert!(v0 == V2);
-        v1 += 1.0;
-        assert!(v1 == Float3::new(5.0, 6.0, 7.0));
-    }
-
-    #[test]
-    fn constexpr() {
-        const V0: Float3 = Float3::new(1.0, 2.0, 3.0);
-        let mut v1 = Float3::new(V0.0, V0.1, V0.2);
-        assert!(v1 == V0);
-
-        const V2: Float3 = Float3::splat(1.0);
-        const V3: Float3 = Float3::zero();
-        v1 += 1.0;
-        assert!(v1 == V0 + V2 + V3);
-    }
-
-    #[test]
-    fn copy() {
-        let v0 = Float3::new(1.0, 2.0, 3.0);
-        let v1 = v0;
-        assert!(v0 == v1);
-    }
-
-    #[test]
-    fn div() {
-        let mut v0 = Float3::new(2.0, 4.0, 6.0);
-        const V1: Float3 = Float3::new(1.0, 2.0, 3.0);
-        assert!(v0 / 2.0 == V1);
-        v0 /= 2.0;
-        assert!(v0 == V1);
-    }
-
-    #[test]
-    fn equal() {
-        let v0 = Float3::new(1.0, 2.0, 3.0);
-        let v1 = Float3::new(1.0, 2.0, 3.0);
-        assert!(v0 == v1);
-        assert!(v0 != Float3::zero());
-    }
-
-    #[test]
-    fn mul() {
-        let mut v0 = Float3::new(1.0, 2.0, 3.0);
-        let mut v1 = Float3::new(4.0, 5.0, 6.0);
-        const V2: Float3 = Float3::new(4.0, 10.0, 18.0);
-        assert!(v0 * v1 == V2);
-        assert!(v0 * 2.0 == v0 * Float3::splat(2.0));
-        assert!(2.0 * v0 == Float3::splat(2.0) * v0);
-
-        v0 *= v1;
-        assert!(v0 == V2);
-        v1 *= 2.0;
-        assert!(v1 == Float3::new(8.0, 10.0, 12.0));
-    }
-
-    #[test]
-    fn neg() {
-        let v0 = Float3::new(1.0, 2.0, 3.0);
-        assert!(-v0 == v0 * -1.0);
-    }
-
-    #[test]
-    fn norm() {
-        const V: Float3 = Float3::new(1.0, 2.0, 3.0);
-        const F: Float = 14.0;
-        assert_eq!(V.norm2(), F);
-        assert_eq!(V.norm(), F.sqrt());
-
-        let u = V.unit();
-        assert_float_eq!(u.norm(), 1.0);
-
-        let mut v = V;
-        v.normalise();
-        assert_float_eq!(v.norm(), 1.0);
-    }
-
-    #[test]
-    fn product() {
-        let v0 = Float3::new(1.0, 1.0, 1.0);
-        let v1 = Float3::new(0.0, 1.0, 1.0);
-        let v2 = v0.cross(v1);
-        assert_eq!(v2.dot(v0), 0.0);
-        assert_eq!(v2.dot(v1), 0.0);
-        let cos_theta = v0.dot(v1) / (v0.norm() * v1.norm());
-        let sin_theta = (1.0 - cos_theta * cos_theta).sqrt();
-        assert_float_eq!(v2.norm(), v0.norm() * v1.norm() * sin_theta);
-    }
-
-    #[test]
-    fn rotate() {
-        let mut v0 = Float3::new(1.0, 0.0, 1.0);
-        let mut v1 = v0;
-        v0.rotate(-1.0, 0.0);
-        v1.reverse();
-        assert_float3_eq!(v0, v1);
-
-        v1.reverse();
-        v1.rotate(0.0, PI / 2.0);
-        assert_eq!(v0.dot(v1), 0.0);
-
-        let v2 = v1;
-        v1.rotate(0.5, PI / 4.0);
-        assert_float_eq!(v2.dot(v1), 1.0);
-
-        let mut v3 = Float3::new(0.0, 0.0, 1.0);
-        v3.rotate(0.0, PI / 4.0);
-        const TMP: Float = FRAC_1_SQRT_2;
-        assert_float_eq!(v3.0, -TMP);
-        assert_float_eq!(v3.1, TMP);
-    }
-
-    #[test]
-    fn sub() {
-        let mut v0 = Float3::new(1.0, 2.0, 3.0);
-        let mut v1 = Float3::new(4.0, 6.0, 8.0);
-        const V2: Float3 = Float3::new(-3.0, -4.0, -5.0);
-        assert!(v0 - v1 == V2);
-        assert!(v0 - 1.0 == v0 - Float3::splat(1.0));
-        assert!(1.0 - v0 == Float3::splat(1.0) - v0);
-
-        v0 -= v1;
-        assert!(v0 == V2);
-        v1 -= 1.0;
-        assert!(v1 == Float3::new(3.0, 5.0, 7.0));
+    fn inside_box() {
+        let center = Float3::zero();
+        let size = Float3::splat(2.0);
+        let shape = BoxShape{ center, size, rotation: None };
+
+        let position = Float3::splat(0.5);
+        assert!(shape.inside(position));
+
+        let position = Float3::splat(1.5);
+        assert!(!shape.inside(position));
+    }
+
+    #[test]
+    fn distance_box() {
+        let center = Float3::zero();
+        let size = Float3::splat(2.0);
+        let shape = BoxShape{ center, size, rotation: None };
+
+        let direction = Float3::new(0.0, 0.0, 1.0);
+        let position = Float3::new(0.0, 0.0, -1.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, -0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.5);
+        let position = Float3::new(0.0, 0.0, 0.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.0);
+        let position = Float3::new(0.0, 0.0, 0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, 1.5);
+        assert!(shape.distance(position, direction).is_none());
+
+        let direction = Float3::new(0.0, 0.0, -1.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, 0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.5);
+        let position = Float3::new(0.0, 0.0, 0.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.0);
+        let position = Float3::new(0.0, 0.0, -0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, -1.5);
+        assert!(shape.distance(position, direction).is_none());
+    }
+
+    #[test]
+    fn inside_sphere() {
+        let center = Float3::zero();
+        let radius = 1.0;
+        let shape = SphereShape{ center, radius };
+
+        let position = Float3::splat(0.5);
+        assert!(shape.inside(position));
+
+        let position = Float3::splat(1.0);
+        assert!(!shape.inside(position));
+    }
+
+    #[test]
+    fn distance_sphere() {
+        let center = Float3::zero();
+        let radius = 1.0;
+        let shape = SphereShape{ center, radius };
+
+        let direction = Float3::new(0.0, 0.0, 1.0);
+        let position = Float3::new(0.0, 0.0, -1.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, -0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.5);
+        let position = Float3::new(0.0, 0.0, 0.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.0);
+        let position = Float3::new(0.0, 0.0, 0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, 1.5);
+        assert!(shape.distance(position, direction).is_none());
+
+        let direction = Float3::new(0.0, 0.0, -1.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, 0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.5);
+        let position = Float3::new(0.0, 0.0, 0.0);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 1.0);
+        let position = Float3::new(0.0, 0.0, -0.5);
+        assert_float_eq!(shape.distance(position, direction).unwrap(), 0.5);
+        let position = Float3::new(0.0, 0.0, -1.5);
+        assert!(shape.distance(position, direction).is_none());
     }
 }
```

### Comparing `goupil-1.0.0/src/numerics/grids.rs` & `goupil-1.1.0/src/numerics/grids.rs`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if tmp < 0.0 {
             return GridCoordinate::Below
         }
         let i = tmp as usize;
         if i > self.n - 1 {
             GridCoordinate::Above(self.n)
         } else if i == self.n - 1 {
-            if x == self.xmax {
+            if x <= self.xmax {
                 GridCoordinate::Inside(self.n - 2, 1.0)
             } else {
                 GridCoordinate::Above(self.n)
             }
         } else {
             let h = tmp - (i as Float);
             GridCoordinate::Inside(i, h)
@@ -188,15 +188,15 @@
             return GridCoordinate::Below;
         }
         let n = self.x.len();
         let i = tmp as usize;
         if i > n - 1 {
             return GridCoordinate::Above(n);
         } else if i == n - 1 {
-            if x == self.x[n - 1] {
+            if x <= self.x[n - 1] {
                 return GridCoordinate::Inside(n - 2, 1.0);
             } else {
                 return GridCoordinate::Above(n);
             }
         } else {
             let h = (x - self.x[i]) / (self.x[i + 1] - self.x[i]);
             return GridCoordinate::Inside(i, h);
```

### Comparing `goupil-1.0.0/src/numerics/integrate.rs` & `goupil-1.1.0/src/numerics/integrate.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics/interpolate.rs` & `goupil-1.1.0/src/numerics/interpolate.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics/rand.rs` & `goupil-1.1.0/src/numerics/rand.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics/table.rs` & `goupil-1.1.0/src/numerics/table.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/numerics.rs` & `goupil-1.1.0/src/numerics.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 // ===============================================================================================
 // Public API.
 // ===============================================================================================
 
 pub mod consts;
 
-pub use self::float::{Float, Float3};
+pub use self::float::{Float, Float3, Float3x3};
 pub use self::rand::FloatRng;
 
 
 // ===============================================================================================
 // Unit tests.
 // ===============================================================================================
 #[cfg(test)]
```

### Comparing `goupil-1.0.0/src/physics/elements/data/elements.rs` & `goupil-1.1.0/src/physics/elements/data/elements.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/elements/data/shells.rs` & `goupil-1.1.0/src/physics/elements/data/shells.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/elements/serialise.rs` & `goupil-1.1.0/src/physics/elements/serialise.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/elements.rs` & `goupil-1.1.0/src/physics/elements.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/materials/electronic.rs` & `goupil-1.1.0/src/physics/materials/electronic.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/materials/table.rs` & `goupil-1.1.0/src/physics/materials/table.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/materials.rs` & `goupil-1.1.0/src/physics/materials.rs`

 * *Files 2% similar despite different names*

```diff
@@ -673,22 +673,14 @@
             .as_ref()
     }
 
     /// Returns the sampling weight for Compton collisions. Depending on the specified `model` and
     /// `mode`, pre-computed material tables might be required (see e.g. the registry
     /// [`compute`](MaterialRegistry::compute) method).
     ///
-    /// # Examples
-    ///
-    /// ```
-    /// # use goupil::physics::{ComptonModel, ElectronicStructure, Material, ComptonMode};
-    /// # let material = Material::new("material", 1.0, ElectronicStructure::default());
-    /// #
-    /// let weight = material.weight(ComptonModel::KleinNishina, ComptonMode::Adjoint, 0.5, 1.0);
-    /// ```
     pub fn compton_weight(
         &self,
         model: ComptonModel,
         mode: ComptonMode,
         energy_in: Float,
         energy_out: Float,
     ) -> Result<Float> {
```

### Comparing `goupil-1.0.0/src/physics/process/absorption/table.rs` & `goupil-1.1.0/src/physics/process/absorption/table.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/absorption.rs` & `goupil-1.1.0/src/physics/process/absorption.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/compton/compute.rs` & `goupil-1.1.0/src/physics/process/compton/compute.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/compton/sample.rs` & `goupil-1.1.0/src/physics/process/compton/sample.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/compton/table.rs` & `goupil-1.1.0/src/physics/process/compton/table.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/compton.rs` & `goupil-1.1.0/src/physics/process/compton.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/rayleigh/sample.rs` & `goupil-1.1.0/src/physics/process/rayleigh/sample.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/rayleigh/table.rs` & `goupil-1.1.0/src/physics/process/rayleigh/table.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process/rayleigh.rs` & `goupil-1.1.0/src/physics/process/rayleigh.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics/process.rs` & `goupil-1.1.0/src/physics/process.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/physics.rs` & `goupil-1.1.0/src/physics.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/density.rs` & `goupil-1.1.0/src/python/density.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/elements.rs` & `goupil-1.1.0/src/python/elements.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/geometry.rs` & `goupil-1.1.0/src/python/geometry.rs`

 * *Files 4% similar despite different names*

```diff
@@ -187,53 +187,67 @@
                 .getattr("LoadLibrary")?;
             let cdll = loader.call1((self.path.as_str(),))?;
             self.cdll = cdll.into_py(py);
         }
         Ok(self.cdll.clone_ref(py))
     }
 
+    fn material_index(&self, name: &str) -> Result<usize> {
+        self.inner.find_material(name)
+    }
+
     fn locate(&self, states: &PyArray<CState>) -> Result<PyObject> {
         locate::<ExternalGeometry, ExternalTracer>(&self.inner, states)
     }
 
+    fn sector_index(&self, description: &str) -> Result<usize> {
+        self.inner.find_sector(description)
+    }
+
     fn trace(
         &self,
         states: &PyArray<CState>,
         lengths: Option<ArrayOrFloat>,
         density: Option<bool>,
     ) -> Result<PyObject> {
         trace::<ExternalGeometry, ExternalTracer>(&self.inner, states, lengths, density)
     }
 
     fn update_material(
         &mut self,
         py: Python,
-        index: usize,
-        material: MaterialLike,
+        material: IndexArg,
+        definition: MaterialLike,
     ) -> Result<()> {
         // Update inner state.
-        let material = material.unpack()?;
+        let index = material.sector_index(&self.inner)?;
+        let material = definition.unpack()?;
         self.inner.update_material(index, &material)?;
 
         // Update external state.
         let materials: &PyTuple = self.materials.extract(py)?;
         let mut this: PyRefMut<PyMaterialDefinition> = materials[index].extract()?;
         this.0 = material.into_owned();
 
         Ok(())
     }
 
     fn update_sector(
         &mut self,
         py: Python,
-        index: usize,
-        material: Option<usize>,
+        sector: IndexArg,
+        material: Option<IndexArg>,
         density: Option<DensityModel>,
     ) -> Result<()> {
         // Update inner state.
+        let index = sector.sector_index(&self.inner)?;
+        let material = match material {
+            None => None,
+            Some(material) => Some(material.material_index(&self.inner)?),
+        };
         self.inner.update_sector(index, material, density.as_ref())?;
 
         // Update external state.
         let sectors: &PyTuple = self.sectors.extract(py)?;
         let mut this: PyRefMut<PyGeometrySector> = sectors[index].extract()?;
         if let Some(material) = material {
             let materials: &PyTuple = self.materials.extract(py)?;
@@ -617,18 +631,26 @@
 
     fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
         visit.call(&self.materials)?;
         visit.call(&self.sectors)?;
         Ok(())
     }
 
+    fn material_index(&self, name: &str) -> Result<usize> {
+        self.inner.find_material(name)
+    }
+
     fn locate(&self, states: &PyArray<CState>) -> Result<PyObject> {
         locate::<StratifiedGeometry, StratifiedTracer>(&self.inner, states)
     }
 
+    fn sector_index(&self, description: &str) -> Result<usize> {
+        self.inner.find_sector(description)
+    }
+
     fn trace(
         &self,
         states: &PyArray<CState>,
         lengths: Option<ArrayOrFloat>,
         density: Option<bool>,
     ) -> Result<PyObject> {
         trace::<StratifiedGeometry, StratifiedTracer>(&self.inner, states, lengths, density)
@@ -930,7 +952,103 @@
         match self {
             Self::External(external) => external.into_py(py),
             Self::Simple(simple) => simple.into_py(py),
             Self::Stratified(stratified) => stratified.into_py(py),
         }
     }
 }
+
+impl PyGeometryDefinition {
+    pub(crate) fn sector_index(&self, py: Python, description: &str) -> Result<usize> {
+        match self {
+            Self::External(external) => {
+                let external = &external.borrow(py).inner;
+                external.find_sector(description)
+            },
+            Self::Simple(simple) => {
+                let simple = &simple.borrow(py).0;
+                simple.find_sector(description)
+            },
+            Self::Stratified(stratified) => {
+                let stratified = &stratified.borrow(py).inner;
+                stratified.find_sector(description)
+            },
+        }
+    }
+}
+
+
+// ===============================================================================================
+// Generic geometry indexing.
+// ===============================================================================================
+
+trait GeometryIndexing: GeometryDefinition {
+    fn find_material(&self, name: &str) -> Result<usize> {
+        let mut index: Option<usize> = None;
+        for (i, material) in self.materials().iter().enumerate() {
+            if material.name() == name {
+                if index.is_some() {
+                    value_error!("multiple matches for material '{}'", name)
+                } else {
+                    index = Some(i);
+                }
+            }
+        }
+        match index {
+            None => value_error!(
+                "could not find any material for '{}'",
+                name
+            ),
+            Some(index) => Ok(index),
+        }
+    }
+
+    fn find_sector(&self, description: &str) -> Result<usize> {
+        let mut index: Option<usize> = None;
+        for (i, sector) in self.sectors().iter().enumerate() {
+            if let Some(d) = &sector.description {
+                if d == description {
+                    if index.is_some() {
+                        value_error!("multiple matches for sector '{}'", description)
+                    } else {
+                        index = Some(i);
+                    }
+                }
+            }
+        }
+        match index {
+            None => value_error!(
+                "could not find any sector for '{}'",
+                description
+            ),
+            Some(index) => Ok(index),
+        }
+    }
+}
+
+impl GeometryIndexing for ExternalGeometry {}
+impl GeometryIndexing for SimpleGeometry {}
+impl GeometryIndexing for StratifiedGeometry {}
+
+#[derive(FromPyObject)]
+enum IndexArg<'a> {
+    Index(usize),
+    Description(&'a str)
+}
+
+impl<'a> IndexArg<'a> {
+    fn material_index<G: GeometryIndexing>(&self, geometry: &G) -> Result<usize> {
+        let index  = match self {
+            Self::Index(index) => *index,
+            Self::Description(description) => geometry.find_material(description)?,
+        };
+        Ok(index)
+    }
+
+    fn sector_index<G: GeometryIndexing>(&self, geometry: &G) -> Result<usize> {
+        let index  = match self {
+            Self::Index(index) => *index,
+            Self::Description(description) => geometry.find_sector(description)?,
+        };
+        Ok(index)
+    }
+}
```

### Comparing `goupil-1.0.0/src/python/goupil/__main__.py` & `goupil-1.1.0/src/python/goupil/__main__.py`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ac.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ac.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ag.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ag.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Al.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Al.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Am.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Am.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ar.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ar.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/As.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/As.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/At.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/At.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Au.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Au.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/B.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/B.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ba.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ba.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Be.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Be.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Bi.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Bi.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Bk.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Bk.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Br.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Br.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/C.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/C.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ca.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ca.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ce.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ce.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Co.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Co.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cs.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cs.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Cu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Cu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Dy.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Dy.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Er.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Er.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Es.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Es.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Eu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Eu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/F.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/F.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Fe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Fe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Fm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Fm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Fr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Fr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ga.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ga.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Gd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Gd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ge.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ge.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/H.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/H.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/He.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/He.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Hf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Hf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Hg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Hg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ho.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ho.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/I.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/I.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/In.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/In.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ir.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ir.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/K.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/K.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Kr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Kr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/La.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/La.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Li.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Li.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Lu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Lu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Mg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Mg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Mn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Mn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Mo.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Mo.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/N.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/N.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Na.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Na.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Nb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Nb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Nd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Nd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ne.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ne.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ni.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ni.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Np.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Np.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/O.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/O.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Os.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Os.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/P.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/P.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pa.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pa.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Po.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Po.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pt.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pt.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Pu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Pu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ra.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ra.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Rb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Rb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Re.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Re.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Rh.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Rh.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Rn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Rn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ru.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ru.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/S.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/S.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Sb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Sb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Sc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Sc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Se.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Se.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Si.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Si.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Sm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Sm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Sn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Sn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Sr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Sr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ta.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ta.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Tb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Tb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Tc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Tc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Te.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Te.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Th.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Th.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Ti.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Ti.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Tl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Tl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Tm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Tm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/U.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/U.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/V.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/V.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/W.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/W.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Xe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Xe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Y.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Y.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Yb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Yb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Zn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Zn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/absorption/Zr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/absorption/Zr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ac.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ac.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ag.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ag.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Al.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Al.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Am.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Am.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ar.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ar.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/As.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/As.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/At.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/At.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Au.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Au.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/B.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/B.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ba.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ba.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Be.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Be.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Bi.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Bi.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Bk.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Bk.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Br.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Br.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/C.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/C.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ca.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ca.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ce.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ce.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Co.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Co.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cs.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cs.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Cu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Cu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Dy.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Dy.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Er.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Er.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Es.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Es.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Eu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Eu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/F.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/F.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Fr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Fr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ga.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ga.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Gd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Gd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ge.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ge.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/H.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/H.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/He.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/He.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Hf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Hf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Hg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Hg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ho.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ho.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/I.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/I.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/In.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/In.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ir.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ir.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/K.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/K.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Kr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Kr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/La.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/La.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Li.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Li.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Lu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Lu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Mo.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Mo.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/N.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/N.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Na.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Na.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Nb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Nb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Nd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Nd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ne.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ne.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ni.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ni.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Np.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Np.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/O.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/O.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Os.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Os.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/P.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/P.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pa.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pa.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Po.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Po.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pt.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pt.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Pu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Pu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ra.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ra.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Re.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Re.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rh.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rh.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Rn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Rn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ru.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ru.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/S.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/S.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Se.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Se.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Si.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Si.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Sr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Sr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ta.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ta.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Te.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Te.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Th.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Th.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Ti.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Ti.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Tm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Tm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/U.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/U.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/V.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/V.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/W.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/W.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Xe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Xe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Y.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Y.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Yb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Yb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Zn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Zn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/cross-section/Zr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/cross-section/Zr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ac.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ac.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ag.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ag.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Al.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Al.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Am.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Am.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ar.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ar.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/As.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/As.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/At.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/At.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Au.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Au.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/B.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/B.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ba.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ba.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Be.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Be.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Bi.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Bi.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Bk.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Bk.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Br.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Br.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/C.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/C.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ca.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ca.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ce.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ce.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Co.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Co.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cs.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cs.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Cu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Cu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Dy.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Dy.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Er.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Er.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Es.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Es.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Eu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Eu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/F.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/F.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Fr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Fr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ga.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ga.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Gd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Gd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ge.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ge.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/H.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/H.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/He.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/He.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Hf.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Hf.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Hg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Hg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ho.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ho.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/I.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/I.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/In.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/In.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ir.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ir.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/K.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/K.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Kr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Kr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/La.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/La.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Li.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Li.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Lu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Lu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mg.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mg.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Mo.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Mo.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/N.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/N.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Na.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Na.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Nb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Nb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Nd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Nd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ne.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ne.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ni.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ni.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Np.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Np.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/O.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/O.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Os.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Os.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/P.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/P.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pa.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pa.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pd.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pd.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Po.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Po.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pt.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pt.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Pu.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Pu.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ra.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ra.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Re.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Re.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rh.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rh.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Rn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Rn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ru.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ru.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/S.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/S.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Se.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Se.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Si.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Si.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Sr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Sr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ta.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ta.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tc.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tc.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Te.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Te.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Th.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Th.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Ti.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Ti.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tl.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tl.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Tm.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Tm.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/U.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/U.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/V.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/V.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/W.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/W.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Xe.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Xe.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Y.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Y.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Yb.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Yb.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Zn.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Zn.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/data/elements/scattering/form-factor/Zr.txt` & `goupil-1.1.0/src/python/goupil/data/elements/scattering/form-factor/Zr.txt`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/interfaces/LICENSE` & `goupil-1.1.0/src/python/goupil/interfaces/LICENSE`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/interfaces/geant4/G4Goupil.cc` & `goupil-1.1.0/src/python/goupil/interfaces/geant4/G4Goupil.cc`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/interfaces/geant4/goupil.h` & `goupil-1.1.0/src/python/goupil/interfaces/geant4/goupil.h`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil/interfaces/goupil.h` & `goupil-1.1.0/src/python/goupil/interfaces/goupil.h`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/goupil.egg-info/PKG-INFO` & `goupil-1.1.0/src/python/goupil.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: goupil
-Version: 1.0.0
-Summary: A backward accelerator for gamma rays transport.
+Version: 1.1.0
+Summary: A Monte Carlo engine for the backward transport of low energy gamma-rays.
 Author-email: Valentin Niess <valentin.niess@gmail.com>
 License: LGPLv3
 Project-URL: source, https://github.com/niess/goupil
 Keywords: gamma rays,Monte Carlo,backward
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7.0
@@ -27,12 +27,14 @@
 
 Documentation for Goupil can be found online at [Read the Docs][RTD].
 
 ## License
 
 The Goupil library is  under the **GNU LGPLv3** license (see the provided
 [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER) files), except for
-[interfaces](src/interfaces) which are MIT-licensed.
+[examples][EXAMPLES] and [interfaces][INTERFACES] which are MIT-licensed.
 
 
+[EXAMPLES]: https://github.com/niess/goupil/tree/master/examples
+[INTERFACES]: https://github.com/niess/goupil/tree/master/src/interfaces
 [RTD]: https://goupil.readthedocs.io/en/latest/
 [RTD_BADGE]: https://readthedocs.org/projects/goupil/badge/?version=latest
```

### Comparing `goupil-1.0.0/src/python/goupil.egg-info/SOURCES.txt` & `goupil-1.1.0/src/python/goupil.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,23 @@
 src/physics/process/rayleigh.rs
 src/physics/process/absorption/table.rs
 src/physics/process/compton/compute.rs
 src/physics/process/compton/sample.rs
 src/physics/process/compton/table.rs
 src/physics/process/rayleigh/sample.rs
 src/physics/process/rayleigh/table.rs
+src/python/boundary.rs
 src/python/density.rs
 src/python/elements.rs
 src/python/geometry.rs
 src/python/materials.rs
 src/python/numpy.rs
 src/python/process.rs
 src/python/rand.rs
+src/python/spectrum.rs
 src/python/transport.rs
 src/python/goupil/__init__.py
 src/python/goupil/__main__.py
 src/python/goupil.egg-info/PKG-INFO
 src/python/goupil.egg-info/SOURCES.txt
 src/python/goupil.egg-info/dependency_links.txt
 src/python/goupil.egg-info/requires.txt
@@ -358,12 +360,13 @@
 src/python/goupil/data/elements/scattering/form-factor/Zr.txt
 src/python/goupil/interfaces/LICENSE
 src/python/goupil/interfaces/goupil.h
 src/python/goupil/interfaces/geant4/G4Goupil.cc
 src/python/goupil/interfaces/geant4/G4Goupil.hh
 src/python/goupil/interfaces/geant4/goupil.h
 src/transport/agent.rs
+src/transport/boundary.rs
 src/transport/density.rs
 src/transport/geometry.rs
 src/transport/geometry/external.rs
 src/transport/geometry/simple.rs
 src/transport/geometry/stratified.rs
```

### Comparing `goupil-1.0.0/src/python/materials.rs` & `goupil-1.1.0/src/python/materials.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/numpy.rs` & `goupil-1.1.0/src/python/numpy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::numerics::float::{Float, Float3};
+use crate::numerics::float::{Float, Float3, Float3x3};
 use crate::physics::materials::electronic::ElectronicShell;
 // PyO3 interface.
 use pyo3::conversion::{FromPyObject, IntoPy, ToPyObject};
 use pyo3::exceptions::{PyIndexError, PyTypeError, PyValueError};
 use pyo3::{ffi, FromPyPointer};
 use pyo3::marker::Python;
 use pyo3::once_cell::GILOnceCell;
@@ -34,14 +34,15 @@
 // ===============================================================================================
 
 struct ArrayInterface {
     // Keep the capsule alive.
     #[allow(dead_code)]
     capsule: PyObject,
     // Type objects.
+    dtype_bool: PyObject,
     dtype_float: PyObject,
     dtype_int32: PyObject,
     dtype_shell: PyObject,
     dtype_state: PyObject,
     dtype_usize: PyObject,
     type_ndarray: PyObject,
     // Functions.
@@ -130,14 +131,18 @@
     let numpy = PyModule::import(py, "numpy")?;
     let capsule = PyModule::import(py, "numpy.core.multiarray")?
         .getattr("_ARRAY_API")?;
 
     // Cache used dtypes, generated from numpy Python interface.
     let dtype = numpy.getattr("dtype")?;
 
+    let dtype_bool: PyObject = dtype
+        .call1(("bool",))?
+        .into_py(py);
+
     let dtype_float: PyObject = dtype
         .call1((FLOAT_FORMAT,))?
         .into_py(py);
 
     let dtype_int32: PyObject = dtype
         .call1(("i4",))?
         .into_py(py);
@@ -183,14 +188,15 @@
     let function = |offset: isize| unsafe {
         ptr.offset(offset)
     };
 
     let api = ArrayInterface {
         capsule: capsule.into(),
         // Type objects.
+        dtype_bool,
         dtype_float,
         dtype_int32,
         dtype_shell,
         dtype_state,
         dtype_usize,
         type_ndarray: object(2),
         // Functions.
@@ -646,14 +652,21 @@
 //
 // ===============================================================================================
 
 pub trait Dtype {
     fn dtype(py: Python) -> PyResult<PyObject>;
 }
 
+impl Dtype for bool {
+    #[inline]
+    fn dtype(py: Python) -> PyResult<PyObject> {
+        Ok(api(py).dtype_bool.clone_ref(py))
+    }
+}
+
 impl Dtype for Float {
     #[inline]
     fn dtype(py: Python) -> PyResult<PyObject> {
         Ok(api(py).dtype_float.clone_ref(py))
     }
 }
 
@@ -847,14 +860,32 @@
         result.set(1, self.1).unwrap();
         result.set(2, self.2).unwrap();
         result.readonly();
         result.into_py(py)
     }
 }
 
+impl IntoPy<PyObject> for Float3x3 {
+    fn into_py(self, py: Python) -> PyObject {
+        let result = PyArray::<Float>::empty(py, &[3, 3]).unwrap();
+        let data: &[Float] = self.as_ref();
+        for i in 0..9 {
+            result.set(i, data[i]).unwrap();
+        }
+        result.readonly();
+        result.into_py(py)
+    }
+}
+
+#[derive(pyo3::FromPyObject)]
+pub enum FloatOrFloat3 {
+    Float(Float),
+    Float3(Float3),
+}
+
 #[derive(pyo3::FromPyObject)]
 pub enum ShapeArg {
     Scalar(usize),
     Vector(Vec<usize>),
 }
 
 impl From<ShapeArg> for Vec<usize> {
```

### Comparing `goupil-1.0.0/src/python/process.rs` & `goupil-1.1.0/src/python/process.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/rand.rs` & `goupil-1.1.0/src/python/rand.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/python/transport.rs` & `goupil-1.1.0/src/python/transport.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 use crate::physics::materials::MaterialRegistry;
 use crate::physics::process::{
     absorption::AbsorptionMode,
     compton::{ComptonModel, ComptonMethod, ComptonMode::{self, Adjoint, Direct, Inverse}},
     rayleigh::RayleighMode,
 };
 use crate::transport::{
-    agent::{TransportAgent, TransportBoundary, TransportStatus},
+    agent::{TransportAgent, TransportStatus},
+    boundary::TransportBoundary,
     geometry::{ExternalTracer, GeometryDefinition, GeometryTracer, SimpleTracer, StratifiedTracer},
     PhotonState,
     TransportMode::{self, Backward, Forward},
     TransportSettings,
 };
 use pyo3::{
     prelude::*,
     gc::PyVisit,
     PyTraverseError,
     types::{PyBytes, PyDict, PyString},
 };
 use rmp_serde::{Deserializer, Serializer};
 use serde::{Deserialize, Serialize};
 use super::{
+    boundary::PyTransportBoundary,
     ctrlc_catched,
     geometry::{PyExternalGeometry, PyGeometryDefinition},
     macros::{type_error, value_error},
     materials::PyMaterialRegistry,
     numpy::{ArrayOrFloat, PyArray, PyScalar, ShapeArg},
     rand::PyRandomStream,
     prefix,
@@ -121,26 +123,23 @@
     #[setter]
     fn set_absorption(&mut self, value: Option<&str>) -> Result<()> {
         from_optstr!(AbsorptionMode, self.inner.absorption, value);
         Ok(())
     }
 
     #[getter]
-    fn get_boundary(&self) -> Option<usize> {
-        match self.inner.boundary {
-            TransportBoundary::None => None,
-            TransportBoundary::Sector(index) => Some(index),
-        }
+    fn get_boundary(&self) -> TransportBoundary {
+        self.inner.boundary
     }
 
     #[setter]
-    fn set_boundary(&mut self, value: Option<usize>) -> Result<()> {
+    fn set_boundary(&mut self, value: Option<PyTransportBoundary>) -> Result<()> {
         match value {
             None => self.inner.boundary = TransportBoundary::None,
-            Some(index) => self.inner.boundary = TransportBoundary::Sector(index),
+            Some(boundary) => self.inner.boundary = boundary.into(),
         };
         Ok(())
     }
 
     #[getter]
     fn get_compton_method(&self) -> &str {
         self.inner.compton_method.into()
@@ -263,19 +262,19 @@
 // ===============================================================================================
 
 #[pyclass(name = "TransportEngine", module = "goupil")]
 pub struct PyTransportEngine {
     #[pyo3(get)]
     geometry: Option<PyGeometryDefinition>,
     #[pyo3(get)]
-    random: Py<PyRandomStream>,
+    pub(crate) random: Py<PyRandomStream>,
     #[pyo3(get)]
     registry: Py<PyMaterialRegistry>,
     #[pyo3(get)]
-    settings: Py<PyTransportSettings>,
+    pub(crate) settings: Py<PyTransportSettings>,
 
     compiled: bool,
 }
 
 #[derive(FromPyObject)]
 enum GeometryArg {
     Object(PyGeometryDefinition),
@@ -330,14 +329,36 @@
 
     fn __getattr__(&self, py: Python, name: &PyString) -> Result<PyObject> {
         Ok(self.settings.getattr(py, name)?)
     }
 
     fn __setattr__(&mut self, py: Python, name: &str, value: PyObject) -> Result<()> {
         match name {
+            "boundary" => {
+                let boundary: TransportBoundary = if value.is_none(py) {
+                    TransportBoundary::None
+                } else {
+                    let value: BoundaryArg = value.extract(py)?;
+                    match value {
+                        BoundaryArg::Description(description) => {
+                            let index = match &self.geometry {
+                                None => value_error!(
+                                    "could not find any sector for '{}'",
+                                    description
+                                ),
+                                Some(geometry) => geometry.sector_index(py, description)?,
+                            };
+                            TransportBoundary::Sector(index)
+                        },
+                        BoundaryArg::Explicit(boundary) => boundary.into(),
+                    }
+                };
+                let settings = &mut self.settings.borrow_mut(py).inner;
+                settings.boundary = boundary;
+            },
             "geometry" => {
                 if value.is_none(py) {
                     self.geometry = None;
                 } else {
                     let geometry: PyGeometryDefinition = value.extract(py)?;
                     self.geometry = Some(geometry);
                 }
@@ -628,14 +649,20 @@
         }
 
         let status: &PyAny = status;
         Ok(status.into())
     }
 }
 
+#[derive(FromPyObject)]
+enum BoundaryArg<'p> {
+    Description(&'p str),
+    Explicit(PyTransportBoundary<'p>),
+}
+
 
 // ===============================================================================================
 // C representation of a photon state.
 // ===============================================================================================
 #[repr(C)]
 #[derive(Clone, Copy)]
 pub(crate) struct CState {
```

### Comparing `goupil-1.0.0/src/python.rs` & `goupil-1.1.0/src/python.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use anyhow::Result;
-use crate::numerics::{Float, Float3};
+use crate::numerics::{Float, Float3, Float3x3};
 use pyo3::prelude::*;
 use pyo3::exceptions::PyKeyboardInterrupt;
 use pyo3::ffi;
 use pyo3::once_cell::GILOnceCell;
+use self::boundary::{PyBoxShape, PySphereShape};
 use self::density::PyDensityGradient;
 use self::elements::{elements as elements_fun, PyAtomicElement};
 use self::geometry::{
     PyExternalGeometry,
     PyGeometrySector,
     PySimpleGeometry,
     PyStratifiedGeometry,
@@ -23,25 +24,28 @@
     PyMaterialDefinition,
     PyMaterialRecord,
     PyMaterialRegistry
 };
 use self::rand::PyRandomStream;
 use process_path::get_dylib_path;
 use self::process::{PyAbsorptionProcess, PyComptonProcess, PyRayleighProcess};
+use self::spectrum::PyDiscreteSpectrum;
 use self::transport::{PyTransportEngine, PyTransportSettings, PyTransportStatus};
 use self::transport::{states as states_fun};
 use std::path::PathBuf;
 
+mod boundary;
 mod density;
 mod elements;
 mod geometry;
 mod materials;
 mod numpy;
 mod rand;
 mod process;
+mod spectrum;
 mod transport;
 
 
 //================================================================================================
 // Check for a keyboard interrupt.
 //================================================================================================
 
@@ -105,24 +109,31 @@
         }
     }
     pub(crate) use value_error;
 }
 
 
 //================================================================================================
-// Implement from Python for Float3.
+// Implement from Python for Float3 and Float3x3.
 //================================================================================================
 
 impl<'py> FromPyObject<'py> for Float3 {
     fn extract(ob: &'py PyAny) -> PyResult<Self> {
         let v: [Float; 3] = ob.extract()?;
         Ok(v.into())
     }
 }
 
+impl<'py> FromPyObject<'py> for Float3x3 {
+    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+        let v: [[Float; 3]; 3] = ob.extract()?;
+        Ok(v.into())
+    }
+}
+
 
 // ===============================================================================================
 // Goupil Python 3 module.
 // ===============================================================================================
 
 #[pymodule]
 fn goupil(py: Python, module: &PyModule) -> PyResult<()> {
@@ -132,30 +143,33 @@
 
     // Register attributes.
     module.add("PREFIX", prefix(py)?)?;
 
     // Register class object(s).
     module.add_class::<PyAbsorptionProcess>()?;
     module.add_class::<PyAtomicElement>()?;
+    module.add_class::<PyBoxShape>()?;
     module.add_class::<PyComptonProcess>()?;
     module.add_class::<PyCrossSection>()?;
     module.add_class::<PyDensityGradient>()?;
+    module.add_class::<PyDiscreteSpectrum>()?;
     module.add_class::<PyDistributionFunction>()?;
     module.add_class::<PyElectronicStructure>()?;
     module.add_class::<PyExternalGeometry>()?;
     module.add_class::<PyFormFactor>()?;
     module.add_class::<PyGeometrySector>()?;
     module.add_class::<PyInverseDistribution>()?;
     module.add_class::<PyMaterialDefinition>()?;
     module.add_class::<PyMaterialRecord>()?;
     module.add_class::<PyMaterialRegistry>()?;
     module.add_class::<PySimpleGeometry>()?;
     module.add_class::<PyStratifiedGeometry>()?;
     module.add_class::<PyRandomStream>()?;
     module.add_class::<PyRayleighProcess>()?;
+    module.add_class::<PySphereShape>()?;
     module.add_class::<PyTopographyMap>()?;
     module.add_class::<PyTopographySurface>()?;
     module.add_class::<PyTransportEngine>()?;
     module.add_class::<PyTransportSettings>()?;
     module.add_class::<PyTransportStatus>()?;
 
     // Register function(s).
```

### Comparing `goupil-1.0.0/src/transport/agent.rs` & `goupil-1.1.0/src/transport/agent.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
             self,
             sample::ComptonSampler,
             ComptonMode::{self, Adjoint, Direct, Inverse},
         },
         rayleigh::sample::RayleighSampler,
     },
 };
-use serde_derive::{Deserialize, Serialize};
 use std::fmt;
 use super::{
+    boundary::TransportBoundary,
     density::DensityModel,
     geometry::{GeometryDefinition, GeometrySector, GeometryTracer},
     PhotonState,
     TransportMode::{Backward, Forward},
     TransportSettings,
 };
 
@@ -185,18 +185,16 @@
 
         // Initialise stepping.
         let mut direction = self.get_direction(&state, &settings);
         self.tracer.reset(state.position, direction)?;
         let mut properties = match self.tracer.sector() {
             None => return Ok(TransportStatus::Exit),
             Some(index) => {
-                if let TransportBoundary::Sector(sector) = settings.boundary {
-                    if index == sector {
-                        return Ok(TransportStatus::Boundary)
-                    }
+                if settings.boundary.inside(state.position, index) {
+                    return Ok(TransportStatus::Boundary)
                 }
                 LocalProperties::new(self.geometry, index, &self.records)?
             },
         };
 
         let mut status = SteppingStatus::new(settings, state.length, energy_in);
         if let SteppingStatus::Stop(status) = status {
@@ -233,15 +231,15 @@
                 Float::INFINITY
             } else {
                 let lambda = properties.material.definition.mass() /
                     (cross_section * AVOGADRO_NUMBER);
                 -lambda * self.rng.uniform01().ln()
             };
 
-            // Apply boundary weight in reverse mode (flux end-condition).
+            // Check for initial energy constraint.
             if status.is_first() {
                 status = SteppingStatus::Next;
                 if !settings.is_forward() {
                     if let Some(energy_constraint) = energy_constraint {
                         if energy_in == energy_constraint {
                             status = SteppingStatus::Last;
                         }
@@ -265,17 +263,22 @@
             if geometry_length <= 0.0 {
                 bail!(
                     "bad geometry step length (expected a positive value, found {})",
                     geometry_length
                 )
             }
 
+            // Compute the boundary step length.
+            let boundary_length = settings.boundary.distance(state.position, direction);
+
             // Compute the effective step length.
             let length = {
-                let length = physical_length.min(geometry_length);
+                let length = physical_length
+                    .min(geometry_length)
+                    .min(boundary_length);
                 match settings.length_max {
                     None => length,
                     Some(length_max) => {
                         let step_max = length_max - state.length;
                         if length > step_max {
                             status = SteppingStatus::Stop(TransportStatus::LengthMax);
                             step_max
@@ -370,14 +373,17 @@
             state.position = self.tracer.position();
             state.length += length;
 
             // Check for any termination condition. Else, update the physical properties of the
             // local geometry.
             if status.is_stop() {
                 break
+            } else if length == boundary_length {
+                status = SteppingStatus::Stop(TransportStatus::Boundary);
+                break
             } else if length == geometry_length {
                 match self.tracer.sector() {
                     None => {
                         status = SteppingStatus::Stop(TransportStatus::Exit);
                         break
                     },
                     Some(index) => {
@@ -401,15 +407,15 @@
                 match status {
                     TransportStatus::EnergyMin |
                     TransportStatus::EnergyMax |
                     TransportStatus::Absorbed => {
                         state.weight = 0.0;
                     },
                     TransportStatus::EnergyConstraint => {
-                        // Patch boundary weight in reverse mode (flux end-condition).
+                        // Apply volume weight in reverse mode.
                         if let Some(lambda) = interaction_length {
                             let density_value = Self::get_density(
                                 properties.density,
                                 state.position
                             )?;
                             state.weight *= lambda / density_value;
                         }
@@ -669,19 +675,7 @@
                         return
                     }
                 }
             }
         }
     }
 }
-
-
-// ===============================================================================================
-// External boundaries.
-// ===============================================================================================
-
-#[derive(Clone, Copy, Default, Deserialize, Serialize)]
-pub enum TransportBoundary {
-    #[default]
-    None,
-    Sector(usize),
-}
```

### Comparing `goupil-1.0.0/src/transport/density.rs` & `goupil-1.1.0/src/transport/density.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/transport/geometry/external.rs` & `goupil-1.1.0/src/transport/geometry/external.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/transport/geometry/simple.rs` & `goupil-1.1.0/src/transport/geometry/simple.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/transport/geometry/stratified.rs` & `goupil-1.1.0/src/transport/geometry/stratified.rs`

 * *Files 2% similar despite different names*

```diff
@@ -459,16 +459,17 @@
         None
     }
 }
 
 impl<'a> StratifiedTracer<'a> {
     fn locate(&mut self, r: Float3) -> (Option<usize>, Float) {
         let size = &self.definition.size;
-        if (r.0 < size.xmin) || (r.0 > size.xmax) ||
-           (r.1 < size.ymin) || (r.1 > size.ymax) {
+        let eps = 10.0 * Float::EPSILON;
+        if (r.0 <= size.xmin + eps) || (r.0 >= size.xmax - eps) ||
+           (r.1 <= size.ymin + eps) || (r.1 >= size.ymax - eps) {
                return (None, Float::INFINITY)
         }
 
         let interfaces = &self.definition.interfaces;
         let n = interfaces.len();
         let mut delta = Float::INFINITY;
 
@@ -489,15 +490,15 @@
         for i in 1..n {
             let zi = interfaces[i].z(r.0, r.1, &mut self.cache);
             match zi {
                 None => {
                     if i == n - 1 {
                         return (Some(i - 1), bound(delta))
                     } else {
-                        unreachable!();
+                        unreachable!("zi = {:?}, i = {}, r = {:}", zi, i, r);
                     }
                 },
                 Some(zi) => {
                     let d = (r.2 - zi).abs();
                     if d < delta { delta = d }
                     if r.2 < zi {
                         return (Some(i - 1), bound(delta))
```

### Comparing `goupil-1.0.0/src/transport/geometry.rs` & `goupil-1.1.0/src/transport/geometry.rs`

 * *Files identical despite different names*

### Comparing `goupil-1.0.0/src/transport.rs` & `goupil-1.1.0/src/transport.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 use crate::physics::{AbsorptionMode, ComptonMethod, ComptonMode, ComptonModel, RayleighMode};
 use crate::pretty_enumerate;
 use enum_iterator::{all, Sequence};
 use serde_derive::{Deserialize, Serialize};
 use std::fmt;
 
 pub(crate) mod agent;
+pub(crate) mod boundary;
 pub(crate) mod density;
 pub(crate) mod geometry;
 
 
 // ===============================================================================================
 // Public API.
 // ===============================================================================================
 
 pub use self::agent::{
     TransportAgent,
-    TransportBoundary,
     TransportStatus
 };
+pub use self::boundary::{
+    BoxShape,
+    GeometryShape,
+    SphereShape,
+    TransportBoundary,
+};
 pub use self::density::DensityModel;
 pub use self::geometry::{
     ExternalGeometry,
     ExternalTracer,
     GeometryDefinition,
     GeometrySector,
     GeometryTracer,
```

