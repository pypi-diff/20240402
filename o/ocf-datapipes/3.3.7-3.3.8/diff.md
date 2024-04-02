# Comparing `tmp/ocf_datapipes-3.3.7.tar.gz` & `tmp/ocf_datapipes-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocf_datapipes-3.3.7.tar", last modified: Wed Mar 27 15:58:20 2024, max compression
+gzip compressed data, was "ocf_datapipes-3.3.8.tar", last modified: Tue Apr  2 11:39:36 2024, max compression
```

## Comparing `ocf_datapipes-3.3.7.tar` & `ocf_datapipes-3.3.8.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.228243 ocf_datapipes-3.3.7/ocf_datapipes/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.228243 ocf_datapipes-3.3.7/ocf_datapipes/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/batches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/fake_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/gsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/nwp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/satellite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/sun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/merge_numpy_examples_to_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/merge_numpy_modalities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/batch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/config/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    31470 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/config/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/config/save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/gsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/pv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/gsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/nwp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/satellite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/wind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/convert/stack_xarray_to_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.232243 ocf_datapipes-3.3.7/ocf_datapipes/load/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/gsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/gsp_national.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/nwp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/excarta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/gfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/ukv.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/pv/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/pv/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/pv/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/pv/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/satellite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/sensor/awos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/topographic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/load/wind/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/wind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/wind/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/load/wind/wind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.236243 ocf_datapipes-3.3.7/ocf_datapipes/production/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/production/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/production/xgnational.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.240244 ocf_datapipes-3.3.7/ocf_datapipes/select/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/apply_pv_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/apply_standard_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_gsp_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_sys_generating_overnight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_sys_with_only_nan_in_a_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_systems_by_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/filter_to_overlapping_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/find_contiguous_t0_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/pick_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/pick_locations_and_t0_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/pick_t0_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/select_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/select_non_nan_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/select_spatial_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/select_time_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/select/select_time_slice_nwp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.240244 ocf_datapipes-3.3.7/ocf_datapipes/training/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47637 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.244243 ocf_datapipes-3.3.7/ocf_datapipes/training/example/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/example/gsp_national.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/example/gsp_pv_nwp_satellite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/example/pv_nwp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/example/simple_pv.py
--rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/pseudo_irradience.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/pvnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/pvnet_site.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/training/windnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.244243 ocf_datapipes-3.3.7/ocf_datapipes/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.244243 ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/add_fourier_space_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/add_topographic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/sun_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.244243 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/convert_pressure_levels_to_separate_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/create_sun_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/create_time_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/downsample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.244243 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/create_pv_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_infill_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/reproject_topographic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/ocf_datapipes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/datapipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/eso.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/pvlive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/ocf_datapipes/utils/split/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/split/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/split/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/split/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/ocf_datapipes/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/validation/check_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/validation/check_for_nans.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/validation/check_vars_and_dims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/ocf_datapipes/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/ocf_datapipes/visualization/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-03-27 15:58:20.000000 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-27 15:58:20.000000 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:58:20.000000 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-27 15:58:20.000000 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-27 15:58:20.000000 ocf_datapipes-3.3.7/ocf_datapipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18610 2024-03-27 15:58:14.000000 ocf_datapipes-3.3.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.248244 ocf_datapipes-3.3.7/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/tests/transform/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_assign_daynight_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_convert_pressure_levels_to_separate_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_create_time_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/transform/xarray/test_upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:20.252244 ocf_datapipes-3.3.7/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/utils/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/utils/test_trig_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-27 15:58:15.000000 ocf_datapipes-3.3.7/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.269097 ocf_datapipes-3.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-02 11:39:36.269097 ocf_datapipes-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.241098 ocf_datapipes-3.3.8/ocf_datapipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.241098 ocf_datapipes-3.3.8/ocf_datapipes/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/batches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/fake_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/merge_numpy_examples_to_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/merge_numpy_modalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/batch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31470 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/config/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/pv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/convert/stack_xarray_to_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.245098 ocf_datapipes-3.3.8/ocf_datapipes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/gsp_national.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/nwp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/excarta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/ukv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/pv/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/pv/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/pv/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/pv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/satellite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.249098 ocf_datapipes-3.3.8/ocf_datapipes/load/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/sensor/awos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/topographic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.253098 ocf_datapipes-3.3.8/ocf_datapipes/load/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/wind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/wind/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/load/wind/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.253098 ocf_datapipes-3.3.8/ocf_datapipes/production/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/production/xgnational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.253098 ocf_datapipes-3.3.8/ocf_datapipes/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/apply_pv_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/apply_standard_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_gsp_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_sys_generating_overnight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_sys_with_only_nan_in_a_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_systems_by_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/filter_to_overlapping_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/find_contiguous_t0_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/pick_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/pick_locations_and_t0_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/pick_t0_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/select_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/select_non_nan_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/select_spatial_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/select_time_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/select/select_time_slice_nwp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.257098 ocf_datapipes-3.3.8/ocf_datapipes/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48564 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.257098 ocf_datapipes-3.3.8/ocf_datapipes/training/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/example/gsp_national.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/example/gsp_pv_nwp_satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/example/pv_nwp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/example/simple_pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/pseudo_irradience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/pvnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/pvnet_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/training/windnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.257098 ocf_datapipes-3.3.8/ocf_datapipes/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.257098 ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/add_fourier_space_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/add_topographic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/sun_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.261098 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/convert_pressure_levels_to_separate_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/create_sun_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/create_time_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/downsample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.261098 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.261098 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/create_pv_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_infill_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/reproject_topographic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/ocf_datapipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/datapipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/eso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/pvlive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/ocf_datapipes/utils/split/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/split/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/split/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/split/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/ocf_datapipes/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/validation/check_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/validation/check_for_nans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/validation/check_vars_and_dims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/ocf_datapipes/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/ocf_datapipes/visualization/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.269097 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-02 11:39:36.000000 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-02 11:39:36.000000 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:39:36.000000 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 11:39:36.000000 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 11:39:36.000000 ocf_datapipes-3.3.8/ocf_datapipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:39:36.269097 ocf_datapipes-3.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18610 2024-04-02 11:39:31.000000 ocf_datapipes-3.3.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.265097 ocf_datapipes-3.3.8/tests/transform/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_assign_daynight_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_convert_pressure_levels_to_separate_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_create_time_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/transform/xarray/test_upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:36.269097 ocf_datapipes-3.3.8/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/utils/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/utils/test_trig_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-02 11:39:32.000000 ocf_datapipes-3.3.8/tests/utils/test_utils.py
```

### Comparing `ocf_datapipes-3.3.7/LICENSE` & `ocf_datapipes-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/PKG-INFO` & `ocf_datapipes-3.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocf_datapipes
-Version: 3.3.7
+Version: 3.3.8
 Summary: Pytorch Datapipes built for use in Open Climate Fix's forecasting work
 Author: Jacob Bieker, Jack Kelly, Peter Dudfield, James Fulton
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
```

### Comparing `ocf_datapipes-3.3.7/README.md` & `ocf_datapipes-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/batches.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/batches.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/fake_batch.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/fake_batch.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/gsp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/nwp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/pv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/satellite.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/sun.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/sun.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/fake/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/fake/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/merge_numpy_examples_to_batch.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/merge_numpy_examples_to_batch.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/merge_numpy_modalities.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/merge_numpy_modalities.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/batch/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/batch/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/config/load.py` & `ocf_datapipes-3.3.8/ocf_datapipes/config/load.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/config/model.py` & `ocf_datapipes-3.3.8/ocf_datapipes/config/model.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/config/save.py` & `ocf_datapipes-3.3.8/ocf_datapipes/config/save.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/coordinates.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/coordinates.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/gsp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy/pv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/gsp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/nwp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/pv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/satellite.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/sensor.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/sensor.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/numpy_batch/wind.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/numpy_batch/wind.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/convert/stack_xarray_to_numpy.py` & `ocf_datapipes-3.3.8/ocf_datapipes/convert/stack_xarray_to_numpy.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/configuration.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/configuration.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/database.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/database.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/gsp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/gsp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/gsp_national.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/gsp_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/gsp/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/gsp/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/nwp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/ecmwf.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/ecmwf.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/excarta.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/excarta.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/gfs.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/gfs.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/icon.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/icon.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/ukv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/ukv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/nwp/providers/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/nwp/providers/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/pv/database.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/pv/database.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/pv/pv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/pv/pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/pv/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/pv/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/satellite.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/sensor/awos.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/sensor/awos.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/topographic.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/topographic.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/wind/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/wind/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/load/wind/wind.py` & `ocf_datapipes-3.3.8/ocf_datapipes/load/wind/wind.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/production/xgnational.py` & `ocf_datapipes-3.3.8/ocf_datapipes/production/xgnational.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/apply_pv_dropout.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/apply_pv_dropout.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/apply_standard_dropout.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/apply_standard_dropout.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_channels.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_channels.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_gsp_ids.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_gsp_ids.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_sys_generating_overnight.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_sys_generating_overnight.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_sys_with_only_nan_in_a_day.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_sys_with_only_nan_in_a_day.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_pv_systems_by_capacity.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_pv_systems_by_capacity.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_time_periods.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_times.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_times.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/filter_to_overlapping_time_periods.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/filter_to_overlapping_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/find_contiguous_t0_time_periods.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/find_contiguous_t0_time_periods.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/pick_locations.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/pick_locations.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/pick_locations_and_t0_times.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/pick_locations_and_t0_times.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/pick_t0_times.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/pick_t0_times.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/select_id.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/select_id.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/select_non_nan_timestamps.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/select_non_nan_timestamps.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/select_spatial_slice.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/select_spatial_slice.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/select_time_slice.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/select_time_slice.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/select/select_time_slice_nwp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/select/select_time_slice_nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/common.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Common functionality for datapipes"""
 import logging
 from datetime import datetime, timedelta
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import xarray as xr
 from torch.utils.data import functional_datapipe
 from torch.utils.data.datapipes.datapipe import IterDataPipe
 
 from ocf_datapipes.batch import BatchKey, NumpyBatch
-from ocf_datapipes.config.model import Configuration
+from ocf_datapipes.config.model import Configuration, InputData
 from ocf_datapipes.load import (
     OpenAWOSFromNetCDF,
     OpenConfiguration,
     OpenGSP,
     OpenGSPFromDatabase,
     OpenNWP,
     OpenPVFromNetCDF,
@@ -33,14 +33,44 @@
     )
     pass
 
 
 logger = logging.getLogger(__name__)
 
 
+def is_config_and_path_valid(
+    use_flag: bool,
+    config,
+    filepath_resolver: Union[str, Callable[[InputData], str]],
+) -> bool:
+    """
+    Checks if the given configuration should be used based on specific criteria.
+
+    Args:
+        use_flag (bool): Indicates whether to consider using the configuration.
+        config (object): The configuration object to check.
+        filepath_resolver (str or callable): Specifies how to access the file path within config;
+            can be an attribute name (str) or a function (callable) that returns the file path.
+
+    Returns:
+        bool: True if all conditions are met (use_flag is True, config is not None,
+              and the resolved file path is not empty), otherwise False.
+    """
+
+    if not use_flag or config is None:
+        return False
+
+    filepath = (
+        filepath_resolver(config)
+        if callable(filepath_resolver)
+        else getattr(config, filepath_resolver, "")
+    )
+    return bool(filepath)
+
+
 def open_and_return_datapipes(
     configuration_filename: str,
     use_gsp: bool = True,
     use_nwp: bool = True,
     use_pv: bool = True,
     use_sat: bool = True,
     use_hrv: bool = True,
@@ -73,40 +103,31 @@
     conf_in = configuration.input_data
     use_nwp = (
         use_nwp
         and (conf_in.nwp is not None)
         and len(conf_in.nwp) != 0
         and all(v.nwp_zarr_path != "" for _, v in conf_in.nwp.items())
     )
-    use_pv = (
-        use_pv and (conf_in.pv is not None) and (conf_in.pv.pv_files_groups[0].pv_filename != "")
-    )
-    use_sat = (
-        use_sat
-        and (conf_in.satellite is not None)
-        and (conf_in.satellite.satellite_zarr_path != "")
-    )
-    use_hrv = (
-        use_hrv
-        and (conf_in.hrvsatellite is not None)
-        and (conf_in.hrvsatellite.hrvsatellite_zarr_path != "")
-    )
-    use_topo = (
-        use_topo
-        and (conf_in.topographic is not None)
-        and (conf_in.topographic.topographic_filename != "")
-    )
-    use_gsp = use_gsp and (conf_in.gsp is not None) and (conf_in.gsp.gsp_zarr_path != "")
-    use_sensor = (
-        use_sensor and (conf_in.sensor is not None) and (conf_in.sensor.sensor_filename != "")
-    )
-    use_wind = (
-        use_wind
-        and (conf_in.wind is not None)
-        and (conf_in.wind.wind_files_groups[0].wind_filename != "")
+
+    use_pv = is_config_and_path_valid(
+        use_pv,
+        conf_in.pv,
+        lambda config: config.pv_files_groups[0].pv_filename if config.pv_files_groups else "",
+    )
+    use_sat = is_config_and_path_valid(use_sat, conf_in.satellite, "satellite_zarr_path")
+    use_hrv = is_config_and_path_valid(use_hrv, conf_in.hrvsatellite, "hrvsatellite_zarr_path")
+    use_topo = is_config_and_path_valid(use_topo, conf_in.topographic, "topographic_filename")
+    use_gsp = is_config_and_path_valid(use_gsp, conf_in.gsp, "gsp_zarr_path")
+    use_sensor = is_config_and_path_valid(use_sensor, conf_in.sensor, "sensor_filename")
+    use_wind = is_config_and_path_valid(
+        use_wind,
+        conf_in.wind,
+        lambda config: config.wind_files_groups[0].wind_filename
+        if config.wind_files_groups
+        else "",
     )
 
     logger.debug(
         f"GSP: {use_gsp} NWP: {use_nwp} Sat: {use_sat},"
         f" HRV: {use_hrv} PV: {use_pv} Topo: {use_topo}"
         f" Sensor: {use_sensor} Wind: {use_wind}"
     )
```

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/example/gsp_national.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/example/gsp_national.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/example/gsp_pv_nwp_satellite.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/example/gsp_pv_nwp_satellite.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/example/pv_nwp.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/example/pv_nwp.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/example/simple_pv.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/example/simple_pv.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/pseudo_irradience.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/pseudo_irradience.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/pvnet.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/pvnet.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/pvnet_site.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/pvnet_site.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/training/windnet.py` & `ocf_datapipes-3.3.8/ocf_datapipes/training/windnet.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/add_fourier_space_time.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/add_fourier_space_time.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/add_topographic_data.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/add_topographic_data.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/numpy_batch/sun_position.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/numpy_batch/sun_position.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/add_t0idx_and_sample_period_duration.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/convert_pressure_levels_to_separate_variables.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/convert_pressure_levels_to_separate_variables.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/create_sun_image.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/create_sun_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/create_time_image.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/create_time_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/downsample.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/downsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/create_gsp_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/gsp/ensure_n_gsp_per_example.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/normalize.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/normalize.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/assign_daynight_status.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/create_pv_image.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/create_pv_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/create_pv_meta_image.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/ensure_n_pv_systems_per_example.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_fill_nighttime_nans_with_zeros.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_infill_interpolate.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_infill_interpolate.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/pv_power_rolling_window.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/pv/remove_pv_zero_examples.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/reproject_topographic_data.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/reproject_topographic_data.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/transform/xarray/upsample.py` & `ocf_datapipes-3.3.8/ocf_datapipes/transform/xarray/upsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/consts.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/consts.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/datapipes.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/datapipes.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/eso.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/eso.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/future.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/future.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/geospatial.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/geospatial.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/location.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/location.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/parallel.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/pvlive.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/pvlive.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/split/method.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/split/method.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/split/model.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/split/model.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/split/split.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/split/split.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/utils/utils.py` & `ocf_datapipes-3.3.8/ocf_datapipes/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/validation/__init__.py` & `ocf_datapipes-3.3.8/ocf_datapipes/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/validation/check_equality.py` & `ocf_datapipes-3.3.8/ocf_datapipes/validation/check_equality.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/validation/check_for_nans.py` & `ocf_datapipes-3.3.8/ocf_datapipes/validation/check_for_nans.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes/validation/check_vars_and_dims.py` & `ocf_datapipes-3.3.8/ocf_datapipes/validation/check_vars_and_dims.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes.egg-info/PKG-INFO` & `ocf_datapipes-3.3.8/ocf_datapipes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocf_datapipes
-Version: 3.3.7
+Version: 3.3.8
 Summary: Pytorch Datapipes built for use in Open Climate Fix's forecasting work
 Author: Jacob Bieker, Jack Kelly, Peter Dudfield, James Fulton
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
```

### Comparing `ocf_datapipes-3.3.7/ocf_datapipes.egg-info/SOURCES.txt` & `ocf_datapipes-3.3.8/ocf_datapipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/setup.py` & `ocf_datapipes-3.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="ocf_datapipes",
-    version="3.3.7",
+    version="3.3.8",
     license="MIT",
     description="Pytorch Datapipes built for use in Open Climate Fix's forecasting work",
     author="Jacob Bieker, Jack Kelly, Peter Dudfield, James Fulton",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `ocf_datapipes-3.3.7/tests/conftest.py` & `ocf_datapipes-3.3.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/transform/xarray/test_assign_daynight_status.py` & `ocf_datapipes-3.3.8/tests/transform/xarray/test_assign_daynight_status.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/transform/xarray/test_convert_pressure_levels_to_separate_variables.py` & `ocf_datapipes-3.3.8/tests/transform/xarray/test_convert_pressure_levels_to_separate_variables.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/transform/xarray/test_downsample.py` & `ocf_datapipes-3.3.8/tests/transform/xarray/test_downsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/transform/xarray/test_normalize.py` & `ocf_datapipes-3.3.8/tests/transform/xarray/test_normalize.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/transform/xarray/test_upsample.py` & `ocf_datapipes-3.3.8/tests/transform/xarray/test_upsample.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/utils/test_location.py` & `ocf_datapipes-3.3.8/tests/utils/test_location.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/utils/test_trig_transform.py` & `ocf_datapipes-3.3.8/tests/utils/test_trig_transform.py`

 * *Files identical despite different names*

### Comparing `ocf_datapipes-3.3.7/tests/utils/test_utils.py` & `ocf_datapipes-3.3.8/tests/utils/test_utils.py`

 * *Files identical despite different names*

