# Comparing `tmp/openlane-2.0.0b8.tar.gz` & `tmp/openlane-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0b8.tar", last modified: Sun Aug 20 12:30:31 2023, max compression
+gzip compressed data, was "openlane-2.0.0b9.tar", last modified: Wed Aug 23 09:52:43 2023, max compression
```

## Comparing `openlane-2.0.0b8.tar` & `openlane-2.0.0b9.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.147660 openlane-2.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-20 12:30:31.147660 openlane-2.0.0b8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.123660 openlane-2.0.0b8/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.127660 openlane-2.0.0b8/openlane/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/design_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/drc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/generic_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/tcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/common/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.127660 openlane-2.0.0b8/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20710 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/pdk_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/removals.py
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.127660 openlane-2.0.0b8/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/flows/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.127660 openlane-2.0.0b8/openlane/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/open_pdks_rev
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.127660 openlane-2.0.0b8/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.131660 openlane-2.0.0b8/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4670 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6512 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/klayout/stream_out.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.131660 openlane-2.0.0b8/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.131660 openlane-2.0.0b8/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2740 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/def/mag_gds.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/def/read.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.131660 openlane-2.0.0b8/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/gds/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.131660 openlane-2.0.0b8/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/lef/maglef.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/lef.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/magic/wrapper.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.135660 openlane-2.0.0b8/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/disconnected_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/padringer.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/set_power_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.139660 openlane-2.0.0b8/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/basic_mp.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/check_antennas.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/cts.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3636 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/rsz_timing_postgrt.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/scripts/openroad/sta/
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/sta/corner.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/sta/multi_corner.tcl.bk
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/yosys/common.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/yosys/json_header.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/smoke_test_design/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/smoke_test_design/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/smoke_test_design/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/smoke_test_design/src/spm.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.143660 openlane-2.0.0b8/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.147660 openlane-2.0.0b8/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    55092 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (123)    33002 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-20 12:26:31.000000 openlane-2.0.0b8/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.123660 openlane-2.0.0b8/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-20 12:30:30.000000 openlane-2.0.0b8/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-20 12:30:31.000000 openlane-2.0.0b8/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-20 12:30:30.000000 openlane-2.0.0b8/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-20 12:30:30.000000 openlane-2.0.0b8/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-20 12:30:30.000000 openlane-2.0.0b8/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-20 12:30:30.000000 openlane-2.0.0b8/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-20 12:30:31.147660 openlane-2.0.0b8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1560 2023-08-20 12:26:31.000000 openlane-2.0.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 12:30:31.147660 openlane-2.0.0b8/test/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-20 12:26:31.000000 openlane-2.0.0b8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-20 12:26:31.000000 openlane-2.0.0b8/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-23 09:52:43.860095 openlane-2.0.0b9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.844095 openlane-2.0.0b9/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/drc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/generic_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21190 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/pdk_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/removals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/open_pdks_rev
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4712 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6639 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/stream_out.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2740 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/mag_gds.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/read.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef/maglef.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/wrapper.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/disconnected_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/padringer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/set_power_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/basic_mp.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/check_antennas.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/cts.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3636 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/sta/
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/sta/corner.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/sta/multi_corner.tcl.bk
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/common.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/json_header.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/smoke_test_design/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/smoke_test_design/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/smoke_test_design/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/smoke_test_design/src/spm.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55107 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-23 09:52:43.860095 openlane-2.0.0b9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1560 2023-08-23 09:49:46.000000 openlane-2.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-23 09:49:46.000000 openlane-2.0.0b9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-23 09:49:46.000000 openlane-2.0.0b9/test/conftest.py
```

### Comparing `openlane-2.0.0b8/PKG-INFO` & `openlane-2.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0b8 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0b9 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
```

### Comparing `openlane-2.0.0b8/openlane/__init__.py` & `openlane-2.0.0b9/openlane/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/__main__.py` & `openlane-2.0.0b9/openlane/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/__version__.py` & `openlane-2.0.0b9/openlane/scripts/openroad/write_views.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.0b8"
-
-if __name__ == "__main__":
-    print(__version__, end="")
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
+write_views
```

### Comparing `openlane-2.0.0b8/openlane/common/__init__.py` & `openlane-2.0.0b9/openlane/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/cli.py` & `openlane-2.0.0b9/openlane/common/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/design_format.py` & `openlane-2.0.0b9/openlane/common/design_format.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/drc.py` & `openlane-2.0.0b9/openlane/common/drc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/generic_dict.py` & `openlane-2.0.0b9/openlane/common/generic_dict.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/metrics.py` & `openlane-2.0.0b9/openlane/common/metrics.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/misc.py` & `openlane-2.0.0b9/openlane/common/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import pathlib
 import unicodedata
 from enum import Enum
 from collections import UserString
 
 from typing import (
     Any,
+    ClassVar,
     Iterable,
     Sequence,
     TypeVar,
 )
 
 
 T = TypeVar("T")
@@ -57,17 +58,19 @@
     )
 
 
 def get_opdks_rev() -> str:
     """
     Gets the Open_PDKs revision confirmed compatible with this version of OpenLane.
     """
-    return open(
-        os.path.join(get_openlane_root(), "open_pdks_rev"), encoding="utf8"
-    ).read()
+    return (
+        open(os.path.join(get_openlane_root(), "open_pdks_rev"), encoding="utf8")
+        .read()
+        .strip()
+    )
 
 
 # The following code snippet has been adapted under the following license:
 #
 # Copyright (c) Django Software Foundation and individual contributors.
 # All rights reserved.
 
@@ -154,23 +157,35 @@
 class Path(UserString, os.PathLike):
     """
     A Path type for OpenLane configuration variables.
 
     Basically just a string.
     """
 
+    # This path will pass the validate() call, but will
+    # fail to open. It should be used for deprecated variable
+    # translation only.
+    _dummy_path: ClassVar[str] = "__openlane_dummy_path"
+
     def __fspath__(self) -> str:
         return str(self)
 
     def exists(self) -> bool:
         """
         A convenience method calling :meth:`os.path.exists`
         """
         return os.path.exists(self)
 
+    def validate(self):
+        """
+        Raises an error if the path does not exist.
+        """
+        if not self.exists() and not self == Path._dummy_path:
+            raise ValueError(f"'{self}' does not exist")
+
 
 class zip_first(object):
     """
     Works like ``zip_longest`` if ｜a｜ > ｜b｜ and ``zip`` if ｜a｜ <= ｜b｜.
     """
 
     def __init__(self, a: Iterable, b: Iterable, fillvalue: Any) -> None:
```

### Comparing `openlane-2.0.0b8/openlane/common/tcl.py` & `openlane-2.0.0b9/openlane/common/tcl.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/common/toolbox.py` & `openlane-2.0.0b9/openlane/common/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     An assisting object shared by a Flow and all its constituent Steps.
 
     The toolbox may create artifacts that are cached to avoid constant re-creation
     between steps.
     """
 
     def __init__(self, tmp_dir: str) -> None:
-        self.tmp_dir = os.path.abspath(tmp_dir)
+        self.tmp_dir = tmp_dir
         self.remove_cells_from_lib = lru_cache(16, True)(self.remove_cells_from_lib)  # type: ignore
 
     @deprecated(
         version="2.0.0b1",
         reason="Use 'aggregate_metrics' from 'openlane.common'",
         action="once",
     )
@@ -153,17 +153,18 @@
                     if len(alt_views) != 0:
                         continue
             if isinstance(views, dict):
                 views_filtered = self.filter_views(config, views, timing_corner)
                 result += views_filtered
             elif isinstance(views, list):
                 result += views
-            elif views is not None and str(views) != "":
+            elif views is not None:
                 result += [Path(views)]
-        return result
+
+        return [element for element in result if str(element) != Path._dummy_path]
 
     def get_timing_files(
         self,
         config: Mapping[str, Any],
         timing_corner: Optional[str] = None,
         prioritize_nl: bool = False,
     ) -> Tuple[str, List[str]]:
```

### Comparing `openlane-2.0.0b8/openlane/config/__init__.py` & `openlane-2.0.0b9/openlane/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/config/config.py` & `openlane-2.0.0b9/openlane/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Callable,
     Dict,
     Set,
 )
 
 from immutabledict import immutabledict
 
-from .variable import Macro, Variable
+from .variable import Variable
 from .removals import removed_variables
 from .flow import pdk_variables, scl_variables, flow_common_variables
 from .pdk_compat import migrate_old_config
 from .preprocessor import preprocess_dict, Keys as SpecialKeys
 from ..logging import info, warn
 from ..__version__ import __version__
 from ..common import GenericDict, GenericImmutableDict, TclUtils, Path
@@ -358,15 +358,14 @@
         *,
         config_override_strings: Optional[Sequence[str]] = None,
         pdk: Optional[str] = None,
         pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         design_dir: Optional[str] = None,
         _load_pdk_configs: bool = True,
-        complete: bool = True,
     ) -> Tuple["Config", str]:
         """
         Creates a new Config object based on a Tcl file, a JSON file, or a
         dictionary.
 
         The returned config object is locked and cannot be modified.
 
@@ -854,15 +853,14 @@
                 if dis in [3, 6]:
                     mutable["GRT_REPAIR_ANTENNAS"] = True
                 if dis in [4, 6]:
                     mutable["RUN_HEURISTIC_DIODE_INSERTION"] = True
                     mutable["DIODE_ON_PORTS"] = "in"
 
         # Macros
-        translated_macros = False
         if mutable.get("EXTRA_SPEFS") is not None and mutable.get("MACROS") is None:
             mutable["MACROS"] = {}
 
             extra_spef_list = mutable["EXTRA_SPEFS"]
             del mutable["EXTRA_SPEFS"]
             if isinstance(extra_spef_list, str):
                 extra_spef_list = extra_spef_list.split(" ")
@@ -872,30 +870,29 @@
                     f"Invalid type for 'EXTRA_SPEFS': {type(extra_spef_list)}. It is recommended that you update your configuration to use the Macro object."
                 )
             elif len(extra_spef_list) % 4 != 0:
                 errors.append(
                     "Invalid value for 'EXTRA_SPEFS': Element count not divisible by four. It is recommended that you update your configuration to use the Macro object."
                 )
             else:
-                translated_macros = True
                 warnings.append(
                     "The configuration variable 'EXTRA_SPEFS' is deprecated. Check the docs on how to use the new 'MACROS' configuration variable."
                 )
                 for i in range(len(extra_spef_list) // 4):
                     start = i * 4
                     module, min, nom, max = (
                         extra_spef_list[start],
                         extra_spef_list[start + 1],
                         extra_spef_list[start + 2],
                         extra_spef_list[start + 3],
                     )
                     macro_dict = {
                         "module": module,
-                        "gds": ["/dev/null"],
-                        "lef": ["/dev/null"],
+                        "gds": [Path._dummy_path],
+                        "lef": [Path._dummy_path],
                     }
                     macro_dict["spef"] = {
                         "min_*": [min],
                         "nom_*": [nom],
                         "max_*": [max],
                     }
                     mutable["MACROS"][module] = macro_dict
@@ -957,18 +954,8 @@
                     if key in Variable.known_variable_names:
                         warnings.append(
                             f"Key '{key}' provided is unused by the current flow."
                         )
                     else:
                         warnings.append(f"An unknown key '{key}' was provided.")
 
-        if (
-            translated_macros and final.get("MACROS") is not None
-        ):  # Second check in case an error was generated
-            for macro in final["MACROS"].values():
-                assert isinstance(macro, Macro)
-                if "/dev/null" in macro.gds:
-                    macro.gds = [Path("")]
-                if "/dev/null" in macro.lef:
-                    macro.lef = [Path("")]
-
         return (final, warnings, errors)
```

### Comparing `openlane-2.0.0b8/openlane/config/flow.py` & `openlane-2.0.0b9/openlane/config/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,14 @@
     Variable(
         "TECH_LEFS",
         Dict[str, Path],
         "Map of corner patterns to to technology LEF files. A corner not matched here will not be supported by OpenRCX in the default flow.",
         pdk=True,
     ),
     Variable(
-        "CELL_LEFS",
-        List[Path],
-        "Path(s) to the cell LEF file(s).",
-        deprecated_names=["CELLS_LEF"],
-        pdk=True,
-    ),
-    Variable(
-        "CELL_GDS",
-        List[Path],
-        "Path(s) to the cell GDSII file(s).",
-        deprecated_names=["GDS_FILES", "CELLS_GDS"],
-        pdk=True,
-    ),
-    Variable(
         "GPIO_PADS_LEF",
         Optional[List[Path]],
         "Path(s) to GPIO pad LEF file(s).",
         pdk=True,
     ),
     Variable(
         "GPIO_PADS_LEF_CORE_SIDE",
@@ -100,17 +86,24 @@
         "DEFAULT_MAX_TRAN",
         Optional[Decimal],
         "Defines the default maximum transition value used in Synthesis and CTS.\nA minimum of 0.1 * CLOCK_PERIOD and this variable, if defined, is used.",
         units="ns",
         pdk=True,
     ),
     Variable(
-        "WIRE_RC_LAYER",
+        "DATA_WIRE_RC_LAYER",
+        Optional[str],
+        "A metal layer with which to estimate parasitics for data nets in earlier stages of the flow.",
+        pdk=True,
+        deprecated_names=["WIRE_RC_LAYER"],
+    ),
+    Variable(
+        "CLOCK_WIRE_RC_LAYER",
         Optional[str],
-        "A metal layer with which to estimate parasitics in earlier stages of the flow.",
+        "A metal layer with which to estimate parasitics for clock nets in earlier stages of the flow.",
         pdk=True,
     ),
     Variable(
         "DEFAULT_CORNER",
         str,
         "The interconnect/process/voltage/temperature corner (IPVT) to use the characterized lib files compatible with by default.",
         pdk=True,
@@ -260,14 +253,34 @@
     Variable(
         "LIB",
         Dict[str, List[Path]],
         "A map from corner patterns to a list of associated liberty files. Exactly one entry must match the `DEFAULT_CORNER`.",
         pdk=True,
     ),
     Variable(
+        "CELL_LEFS",
+        List[Path],
+        "Path(s) to the cells' LEF file(s).",
+        deprecated_names=["CELLS_LEF"],
+        pdk=True,
+    ),
+    Variable(
+        "CELL_GDS",
+        List[Path],
+        "Path(s) to the cells' GDSII file(s).",
+        deprecated_names=["GDS_FILES", "CELLS_GDS"],
+        pdk=True,
+    ),
+    Variable(
+        "CELL_SPICE_MODELS",
+        Optional[List[Path]],
+        "Path(s) to cells' SPICE model(s)",
+        pdk=True,
+    ),
+    Variable(
         "SYNTH_EXCLUSION_CELL_LIST",
         Path,
         "Path to a text file containing a list of cells to be excluded from the lib file in synthesis alone. If not defined, the original lib file will be used as-is.",
         deprecated_names=["NO_SYNTH_CELL_LIST"],
         pdk=True,
     ),
     Variable(
@@ -568,15 +581,15 @@
         Optional[List[Path]],
         "Specifies miscellaneous Verilog models to be loaded indiscriminately during synthesis.",
         deprecated_names=["VERILOG_FILES_BLACKBOX"],
     ),
     Variable(
         "EXTRA_SPICE_MODELS",
         Optional[List[Path]],
-        "Miscellaneous SPICE files .",
+        "Specifies miscellaneous SPICE models to be loaded indiscriminately whenever SPICE models are loaded.",
     ),
     Variable(
         "EXTRA_LIBS",
         Optional[List[Path]],
         "Specifies LIB files of pre-hardened macros used in the current design, used during timing analyses (and during parasitics-based STA as a fallback). These are loaded indiscriminately for all timing corners.",
     ),
     Variable(
```

### Comparing `openlane-2.0.0b8/openlane/config/pdk_compat.py` & `openlane-2.0.0b9/openlane/config/pdk_compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
+from glob import glob
 from typing import Any, List, Mapping, Dict
 
 
 def migrate_old_config(config: Mapping[str, Any]) -> Dict[str, Any]:
     new = dict(config)
 
     # 1. Migrate SYNTH_DRIVING_CELL
@@ -132,15 +133,27 @@
 
     new["MAX_FANOUT_CONSTRAINT"] = 10
     new["CLOCK_UNCERTAINTY_CONSTRAINT"] = 0.25
     new["CLOCK_TRANSITION_CONSTRAINT"] = 0.15
     new["TIME_DERATING_CONSTRAINT"] = 5
     new["IO_DELAY_CONSTRAINT"] = 20
 
-    # 8. Primary Signoff Tool
+    # 8. SPICE models
+    if new["PDK"].startswith("sky130") or new["PDK"].startswith("gf180mcu"):
+        spice_glob = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.ref",
+            config["STD_CELL_LIBRARY"],
+            "spice",
+            "*.spice",
+        )
+        new["CELL_SPICE_MODELS"] = glob(spice_glob)
+
+    # 9. Primary Signoff Tool
     if new["PDK"].startswith("sky130") or new["PDK"].startswith("gf180mcu"):
         new["PRIMARY_SIGNOFF_TOOL"] = "magic"
 
     # x1. Disconnected Modules (sky130)
     if new["PDK"].startswith("sky130"):
         new["IGNORE_DISCONNECTED_MODULES"] = "sky130_fd_sc_hd__conb_1"
```

### Comparing `openlane-2.0.0b8/openlane/config/preprocessor.py` & `openlane-2.0.0b9/openlane/config/preprocessor.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/config/removals.py` & `openlane-2.0.0b9/openlane/config/removals.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/config/variable.py` & `openlane-2.0.0b9/openlane/config/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 import shlex
 import inspect
 from enum import Enum
 from decimal import Decimal, InvalidOperation
 from dataclasses import _MISSING_TYPE, MISSING, dataclass, field, fields, is_dataclass
 from typing import (
     ClassVar,
@@ -472,19 +471,22 @@
                 )
                 kwargs_dict[key] = value__processed
             return validating_type(**kwargs_dict)
         elif validating_type == Path:
             # Handle one-file globs
             if isinstance(value, list) and len(value) == 1:
                 value = value[0]
-            if not os.path.exists(str(value)):
+            result = Path(value)
+            try:
+                result.validate()
+            except ValueError as e:
                 raise ValueError(
-                    f"Path provided for variable '{key_path}' does not exist: '{value}'"
+                    f"Path provided for variable '{key_path}' is invalid: '{e}'"
                 )
-            return Path(value)
+            return result
         elif validating_type == bool:
             if not permissive_typing and not isinstance(value, bool):
                 raise ValueError(
                     f"Refusing to automatically convert '{value}' at '{key_path}' to a boolean"
                 )
             if value in ["1", "true", 1, True]:
                 return True
```

### Comparing `openlane-2.0.0b8/openlane/container.py` & `openlane-2.0.0b9/openlane/container.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/env_info.py` & `openlane-2.0.0b9/openlane/env_info.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/__init__.py` & `openlane-2.0.0b9/openlane/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/builtins.py` & `openlane-2.0.0b9/openlane/flows/builtins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/classic.py` & `openlane-2.0.0b9/openlane/flows/classic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/cli.py` & `openlane-2.0.0b9/openlane/flows/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/flow.py` & `openlane-2.0.0b9/openlane/flows/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import os
 import glob
+import logging
 import datetime
 import textwrap
+import contextlib
 from abc import abstractmethod, ABC
 from concurrent.futures import Future
 from functools import wraps
 from typing import (
     List,
     Sequence,
     Tuple,
@@ -46,15 +48,21 @@
 from ..config import (
     Config,
     Variable,
     universal_flow_config_variables,
 )
 from ..state import State
 from ..steps import Step
-from ..logging import console, info, verbose
+from ..logging import (
+    console,
+    info,
+    verbose,
+    register_additional_handler,
+    deregister_additional_handler,
+)
 from ..common import get_tpe, mkdirp, protected, final, slugify, Toolbox
 
 
 class FlowError(RuntimeError):
     """
     A ``RuntimeError`` that occurs when a Flow, or one of its underlying Steps,
     fails to finish execution properly.
@@ -462,14 +470,28 @@
             raise FlowException(
                 f"Run directory for '{tag}' already exists as a file and not a directory."
             )
         except FileNotFoundError:
             info(f"Starting a new run of the '{self.name}' flow with the tag '{tag}'.")
             mkdirp(self.run_dir)
 
+        warning_log_path = os.path.join(self.run_dir, "warnings.log")
+        warning_handler = logging.FileHandler(warning_log_path, mode="a+")
+        warning_handler.setLevel("WARNING")
+        register_additional_handler(warning_handler)
+
+        error_log_path = os.path.join(self.run_dir, "errors.log")
+        error_handler = logging.FileHandler(error_log_path, mode="a+")
+        error_handler.setLevel("ERROR")
+        register_additional_handler(error_handler)
+
+        with contextlib.ExitStack() as stack:
+            stack.callback(deregister_additional_handler, warning_handler)
+            stack.callback(deregister_additional_handler, error_handler)
+
         config_res_path = os.path.join(self.run_dir, "resolved.json")
         with open(config_res_path, "w") as f:
             f.write(self.config.dumps())
 
         self.progress_bar = FlowProgressBar(
             self.name, starting_ordinal=starting_ordinal
         )
```

### Comparing `openlane-2.0.0b8/openlane/flows/misc.py` & `openlane-2.0.0b9/openlane/flows/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/optimizing.py` & `openlane-2.0.0b9/openlane/flows/optimizing.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/flows/sequential.py` & `openlane-2.0.0b9/openlane/flows/sequential.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/logging/__init__.py` & `openlane-2.0.0b9/openlane/logging/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .logger import (
     LogLevels,
     LogLevelsDict,
     console,
     set_log_level,
     reset_log_level,
     get_log_level,
+    register_additional_handler,
+    deregister_additional_handler,
     verbose,
     debug,
     info,
     rule,
     success,
     warn,
     err,
```

### Comparing `openlane-2.0.0b8/openlane/logging/logger.py` & `openlane-2.0.0b9/openlane/logging/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -70,23 +70,55 @@
     logger.addHandler(handler)
     return logger
 
 
 __openlane_logger = __logger()
 
 
+def register_additional_handler(handler: logging.Handler):
+    """
+    Adds a new handler to the default OpenLane logger.
+
+    :param handler: The new handler. Must be of type ``logging.Handler``
+        or its subclasses.
+    """
+    __openlane_logger.addHandler(handler)
+
+
+def deregister_additional_handler(handler: logging.Handler):
+    """
+    Removes a registered handler from the default OpenLane logger.
+
+    :param handler: The handler. If not registered, the behavior
+        of this function is undefined.
+    """
+    __openlane_logger.removeHandler(handler)
+
+
 def set_log_level(lv: Union[str, int]):
+    """
+    Sets the log level of the default OpenLane logger.
+
+    :param lv: Either the name or number of the desired log level.
+    """
     __openlane_logger.setLevel(lv)
 
 
 def reset_log_level():
+    """
+    Sets the log level of the default OpenLane logger back to the
+    default log level.
+    """
     set_log_level("VERBOSE")
 
 
 def get_log_level() -> int:
+    """
+    Obtains the numeric log level of the OpenLane logger.
+    """
     return __openlane_logger.getEffectiveLevel()
 
 
 def debug(msg: object, /, **kwargs):
     """
     Logs to the OpenLane logger with the log level DEBUG.
```

### Comparing `openlane-2.0.0b8/openlane/plugins.py` & `openlane-2.0.0b9/openlane/plugins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/base.sdc` & `openlane-2.0.0b9/openlane/scripts/base.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/klayout/open_design.py` & `openlane-2.0.0b9/openlane/scripts/klayout/open_design.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             "klayout",
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
-                value = ";".join(value)
+                value = ";".join([os.path.abspath(element) for element in value])
             elif (
                 isinstance(value, str)
                 and os.path.exists(value)
                 and key != "design_name"
             ):
                 value = os.path.abspath(value)
```

### Comparing `openlane-2.0.0b8/openlane/scripts/klayout/render.py` & `openlane-2.0.0b9/openlane/scripts/klayout/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             "-b",
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
-                value = ";".join(value)
+                value = ";".join([os.path.abspath(element) for element in value])
             elif (
                 isinstance(value, str)
                 and os.path.exists(value)
                 and key != "design_name"
             ):
                 value = os.path.abspath(value)
```

### Comparing `openlane-2.0.0b8/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.0b9/openlane/scripts/klayout/stream_out.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,26 +86,29 @@
     @click.option(
         "-t",
         "--top",
         "design_name",
         required=True,
         help="Name of the design/top module",
     )
-    @click.argument("input")
+    @click.argument(
+        "input",
+        type=click.Path(exists=True, file_okay=True, dir_okay=False),
+    )
     def stream_out(**kwargs):
         args = [
             "klayout",
             "-b",
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
-                value = ";".join(value)
+                value = ";".join([os.path.abspath(element) for element in value])
             elif (
                 isinstance(value, str)
                 and os.path.exists(value)
                 and key != "design_name"
             ):
                 value = os.path.abspath(value)
```

### Comparing `openlane-2.0.0b8/openlane/scripts/klayout/xor.drc` & `openlane-2.0.0b9/openlane/scripts/klayout/xor.drc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/def/mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/def/mag_gds.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/def/mag_gds.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/def/read.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/def/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/drc.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/drc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/extract_spice.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/gds/extras_mag.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/gds/extras_mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/gds/read.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/gds/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/lef.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/lef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/magic/wrapper.tcl` & `openlane-2.0.0b9/openlane/scripts/magic/wrapper.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/apply_def_template.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/defutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/diodes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/disconnected_pins.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/disconnected_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/io_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/padringer.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/padringer.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/power_utils.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/power_utils.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/reader.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,47 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # flake8: noqa E402
 import odb
 
-import os
 import sys
 import locale
 import inspect
 import functools
 from typing import Callable, Dict
 
 # -- START: Environment Fixes
 try:
     locale.setlocale(locale.LC_ALL, "C.UTF-8")
 except locale.Error:
     # We tried. :)
     pass
-
-if python_path := os.environ.get("ODB_PYTHONPATH", None):
-    sys.path = python_path.split(":") + sys.path
-
-sys.path.insert(0, os.path.dirname(os.environ["OPENLANE_ROOT"]))
 # -- END
 
 import click
 import rich
 from rich.table import Table
-from openlane.common.design_format import DesignFormat, DesignFormatObject
 
-# Re-export now that the environment actually works properly
+# Re-export for subfunctions
 rich
 click
 Table
 
-write_fn: Dict[DesignFormat, Callable] = {
-    DesignFormat.DEF: lambda reader, file: odb.write_def(reader.block, file),
-    DesignFormat.ODB: lambda reader, file: odb.write_db(reader.db, file),
+write_fn: Dict[str, Callable] = {
+    "def": lambda reader, file: odb.write_def(reader.block, file),
+    "odb": lambda reader, file: odb.write_db(reader.db, file),
 }
 
 
 class OdbReader(object):
     def __init__(self, *args):
         self.db = odb.dbDatabase.create()
         if len(args) == 1:
@@ -89,15 +82,15 @@
         kwargs = kwargs.copy()
         kwargs["reader"] = reader
 
         outputs = []
         for key, value in kwargs.items():
             if key.startswith("output_"):
                 id = key[7:]
-                outputs.append((DesignFormat.by_id(id), value))
+                outputs.append((id, value))
 
         kwargs = {k: kwargs[k] for k in kwargs.keys() if not k.startswith("output_")}
 
         if "input_db" in parameter_keys:
             kwargs["input_db"] = input_db
         if "input_lefs" in parameter_keys:
             kwargs["input_lefs"] = input_lefs
@@ -110,23 +103,19 @@
 
         function(**kwargs)
 
         for format, path in outputs:
             fn = write_fn[format]
             fn(reader, path)
 
-    for format in DesignFormat:
-        if write_fn.get(format) is None:
-            continue
-        # For type-checker: all guaranteed to be DesignFormatObjects
-        assert isinstance(format.value, DesignFormatObject)
+    for format in write_fn:
         wrapper = click.option(
-            f"--output-{format.value.id}",
+            f"--output-{format}",
             default=None,
-            help=f"Write {format.value.name}",
+            help=f"Write {format} view",
         )(wrapper)
 
     wrapper = click.option(
         "-l",
         "--input-lef",
         "input_lefs",
         default=(),
```

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/set_power_connections.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/set_power_connections.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.0b9/openlane/scripts/odbpy/wire_lengths.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/basic_mp.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/check_antennas.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/check_antennas.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/grt.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/io.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/io.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/resizer.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/resizer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/set_global_connections.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/set_global_connections.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/set_power_nets.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -31,11 +31,13 @@
         set layer_name [lindex $layer_rc 0]
         set capacitance [lindex $layer_rc 1]
         set resistance [lindex $layer_rc 2]
         set_layer_rc -layer $layer_name -capacitance $capacitance -resistance $resistance
     }
 }
 
-if { [info exist ::env(WIRE_RC_LAYER)] } {
-    set_wire_rc -signal -layer $::env(WIRE_RC_LAYER)
-    set_wire_rc -clock -layer $::env(WIRE_RC_LAYER)
+if { [info exist ::env(DATA_WIRE_RC_LAYER)] } {
+    set_wire_rc -signal -layer $::env(DATA_WIRE_RC_LAYER)
 }
+if { [info exist ::env(CLOCK_WIRE_RC_LAYER)] } {
+    set_wire_rc -clock -layer $::env(CLOCK_WIRE_RC_LAYER)
+}
```

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/cts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/drt.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/drt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/fill.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/floorplan.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/gpl.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/gpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/grt.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/gui.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/ioplacer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/irdrop.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/pdn.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/rcx.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/repair_design.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/repair_design.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/sta/corner.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/sta/corner.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/sta/multi_corner.tcl.bk` & `openlane-2.0.0b9/openlane/scripts/openroad/sta/multi_corner.tcl.bk`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.0b9/openlane/scripts/openroad/tapcell.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.0b9/openlane/__version__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read_current_odb
-write_views
+__version__ = "2.0.0b9"
+
+if __name__ == "__main__":
+    print(__version__, end="")
```

### Comparing `openlane-2.0.0b8/openlane/scripts/yosys/common.tcl` & `openlane-2.0.0b9/openlane/scripts/yosys/common.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/yosys/json_header.tcl` & `openlane-2.0.0b9/openlane/scripts/yosys/json_header.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/scripts/yosys/synthesize.tcl` & `openlane-2.0.0b9/openlane/scripts/yosys/synthesize.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/smoke_test_design/src/spm.v` & `openlane-2.0.0b9/openlane/smoke_test_design/src/spm.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/state/__init__.py` & `openlane-2.0.0b9/openlane/state/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/state/state.py` & `openlane-2.0.0b9/openlane/state/state.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/__init__.py` & `openlane-2.0.0b9/openlane/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/__main__.py` & `openlane-2.0.0b9/openlane/steps/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,31 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import json
+import shlex
+import shutil
 import datetime
 from functools import partial
-from typing import Optional
+from typing import Any, Dict, Optional, Sequence, Union
 
 from click import pass_context, Context
 from cloup import (
     group,
     option,
     command,
     Path,
 )
 
 from .step import Step, StepError, StepException
-from ..logging import err, warn
-from ..common import mkdirp, Toolbox
-from ..common.cli import formatter_settings
+from ..logging import info, err, warn
 from ..__version__ import __version__
+from ..common.cli import formatter_settings
+from ..common import mkdirp, Toolbox, get_openlane_root
 
 
 def extract_step_id(ctx: Context, json_in_path: str) -> Optional[str]:
     try:
         cfg = json.load(open(json_in_path, encoding="utf8"))
         meta = cfg.get("meta") or {}
         return meta.get("step")
@@ -148,14 +150,147 @@
 
 @command(formatter_settings=formatter_settings)
 @o(
     "-o",
     "--output",
     type=Path(
         exists=False,
+        file_okay=True,
+        dir_okay=False,
+    ),
+    help="Ejected run script",
+    default="run.sh",
+)
+@o(
+    "--id",
+    type=str,
+    required=False,
+    help="The ID for the step. Can be omitted if the configuration object has the ID in the key-path .meta.step.",
+)
+@o(
+    "-c",
+    "--config",
+    type=Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+    ),
+    required=True,
+    help="A step-specific config.json file",
+)
+@o(
+    "-i",
+    "--state-in",
+    type=Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+    ),
+    required=False,
+)
+@pass_context
+def eject(ctx, output, state_in, config, id):
+    """
+    For steps that rely on underlying utilities using a subprocess, this scripts
+    "ejects" OpenLane and just returns a shell script that runs this subprocess.
+
+    This is useful for:
+
+    * OpenLane developers and maintainers reporting issues to original tool
+      developers
+    * Advanced users who are sure that the issue is not OpenLane-specific and
+      would like to skip reporting an issue with OpenLane first
+    """
+
+    step = load_step_from_inputs(ctx, id, config, state_in)
+
+    if step.config.meta.openlane_version != __version__:
+        warn(
+            "OpenLane version being used is different from the version this step was originally run with. Procceed with caution."
+        )
+
+    toolbox_dir = os.path.join(".", "toolbox_tmp")
+
+    found_cmd: Optional[Sequence[Union[str, os.PathLike]]] = None
+    found_env: Optional[Dict[str, Any]] = None
+
+    class Stop(Exception):
+        pass
+
+    def run_subprocess_subsitute(
+        cmd: Sequence[Union[str, os.PathLike]],
+        env: Optional[Dict[str, Any]] = None,
+        *args,
+        **kwargs,
+    ):
+        nonlocal found_env, found_cmd
+        found_cmd = cmd
+        found_env = env
+        raise Stop()
+
+    step.run_subprocess = run_subprocess_subsitute
+
+    try:
+        step.start(
+            toolbox=Toolbox(toolbox_dir),
+            step_dir=".",
+        )
+    except Stop:
+        pass
+    except Exception as e:
+        info("An error occurred while attempting to execute the step:")
+        err(e)
+        info("This may affect the ejection process.")
+
+    if found_cmd is None:
+        err(
+            "Could not eject: The step did not successfully invoke a subprocess using run_subprocess."
+        )
+        exit(-1)
+
+    canon_scripts_dir = os.path.join(get_openlane_root(), "scripts")
+    target_scripts_dir = os.path.join(".", "scripts")
+
+    try:
+        shutil.rmtree(target_scripts_dir)
+    except FileNotFoundError:
+        pass
+
+    shutil.copytree(canon_scripts_dir, target_scripts_dir)
+
+    current_env = os.environ
+    filtered_env = {
+        "STEP_DIR": ".",
+        "SCRIPTS_DIR": target_scripts_dir,
+    }
+    if found_env is not None:
+        for key, value in found_env.items():
+            if value != current_env.get(key) and key not in filtered_env:
+                filtered_env[key] = value
+
+    with open(output, "w", encoding="utf8") as f:
+        f.write("#!/bin/sh\n")
+        for key, value in filtered_env.items():
+            f.write(f"export {key}={shlex.quote(str(value))}\n")
+        f.write("\n")
+        f.write(shlex.join([str(e) for e in found_cmd]))
+        f.write("\n")
+
+    if hasattr(os, "chmod"):
+        os.chmod(output, 0o755)
+
+    info("Ejected successfully.")
+
+
+@command(formatter_settings=formatter_settings)
+@o(
+    "-o",
+    "--output",
+    type=Path(
+        exists=False,
         file_okay=False,
         dir_okay=True,
     ),
     help="The output directory for the reproducible.",
     default="reproducible",
 )
 @o(
@@ -240,11 +375,12 @@
     Try 'python3 -m openlane.steps COMMAND --help' for help with a specific
     command.
     """
     pass
 
 
 cli.add_command(run)
+cli.add_command(eject)
 cli.add_command(create_reproducible)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `openlane-2.0.0b8/openlane/steps/checker.py` & `openlane-2.0.0b9/openlane/steps/checker.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/common_variables.py` & `openlane-2.0.0b9/openlane/steps/common_variables.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/klayout.py` & `openlane-2.0.0b9/openlane/steps/klayout.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/magic.py` & `openlane-2.0.0b9/openlane/steps/magic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/misc.py` & `openlane-2.0.0b9/openlane/steps/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/openlane/steps/netgen.py` & `openlane-2.0.0b9/openlane/steps/netgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
-import glob
 import json
+from decimal import Decimal
 from abc import abstractmethod
 from typing import List, Dict, Tuple
 
 from .step import ViewsUpdate, MetricsUpdate, Step
 from .tclstep import TclStep
 
-from ..config import Variable, Keys
-from ..state import DesignFormat, State
 from ..common import Path
+from ..logging import warn
+from ..config import Variable
+from ..state import DesignFormat, State
 
 
 def get_metrics(stats: Dict) -> Dict:
     metrics: Dict = {}
     if not stats:
         return metrics
 
@@ -144,23 +145,21 @@
     def get_command(self) -> List[str]:
         return super().get_command() + [self.get_script_path()]
 
     def get_script_path(self):
         return os.path.join(self.step_dir, "lvs_script.lvs")
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        spice_glob = os.path.join(
-            self.config[Keys.pdk_root],
-            self.config[Keys.pdk],
-            "libs.ref",
-            self.config[Keys.scl],
-            "spice",
-            "*.spice",
-        )
-        spice_files: List[str] = glob.glob(spice_glob)
+        spice_files = []
+        if self.config["CELL_SPICE_MODELS"] is None:
+            warn(
+                "This PDK does not appear to define any SPICE models. LVS will still run, but all cells will be black-boxed and the result may be inaccurate."
+            )
+        else:
+            spice_files = self.config["CELL_SPICE_MODELS"].copy()
 
         if pdk_spice_files := self.config.get("SPICE_MODELS"):
             spice_files = pdk_spice_files.copy()
 
         if extra_spice_files := self.config.get("EXTRA_SPICE_MODELS"):
             spice_files += extra_spice_files
 
@@ -174,18 +173,18 @@
                 )
                 print(
                     f"readnet spice {lib} 1",
                     file=f,
                 )
 
             print(
-                f"lvs {{ {state_in[DesignFormat.SPICE]} {design_name} }} {{ {state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {self.config['NETGEN_SETUP']} {os.path.abspath(self.step_dir)}/lvs.rpt -json",
+                f"lvs {{ {state_in[DesignFormat.SPICE]} {design_name} }} {{ {state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {self.config['NETGEN_SETUP']} {self.step_dir}/lvs.rpt -json",
                 file=f,
             )
 
         views_updates, metrics_updates = super().run(state_in, **kwargs)
         stats_file = os.path.join(self.step_dir, "lvs.json")
         stats_string = open(stats_file).read()
-        lvs_metrics = get_metrics(json.loads(stats_string))
+        lvs_metrics = get_metrics(json.loads(stats_string, parse_float=Decimal))
         metrics_updates.update(lvs_metrics)
 
         return (views_updates, metrics_updates)
```

### Comparing `openlane-2.0.0b8/openlane/steps/odb.py` & `openlane-2.0.0b9/openlane/steps/odb.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
-import sys
 import json
 import shutil
 from math import inf
 from decimal import Decimal
 from functools import reduce
 from abc import abstractmethod
 from typing import List, Optional, Tuple
 
 from .common_variables import io_layer_variables
 from .step import ViewsUpdate, MetricsUpdate, Step, StepException
 from ..logging import warn
 from ..config import Variable, Macro
 from ..state import State, DesignFormat
-from ..common import Path, get_openlane_root, get_script_dir, StringEnum
+from ..common import Path, get_script_dir, StringEnum
 
 inf_rx = re.compile(r"\b(-?)inf\b")
 
 
 class OdbpyStep(Step):
     inputs = [DesignFormat.ODB]
     outputs = [DesignFormat.ODB, DesignFormat.DEF]
@@ -49,27 +48,24 @@
             command.append(file_path)
             out_paths[output] = Path(file_path)
 
         command += [
             str(state_in[DesignFormat.ODB]),
         ]
 
-        env["OPENLANE_ROOT"] = get_openlane_root()
-        env["ODB_PYTHONPATH"] = ":".join(sys.path)
-
         generated_metrics = self.run_subprocess(
             command,
             env=env,
             **kwargs,
         )
 
         metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
         metrics_updates: MetricsUpdate = generated_metrics
         if os.path.exists(metrics_path):
-            or_metrics_out = json.loads(open(metrics_path).read())
+            or_metrics_out = json.loads(open(metrics_path).read(), parse_float=Decimal)
             for key, value in or_metrics_out.items():
                 if value == "Infinity":
                     or_metrics_out[key] = inf
                 elif value == "-Infinity":
                     or_metrics_out[key] = -inf
             metrics_updates.update(or_metrics_out)
```

### Comparing `openlane-2.0.0b8/openlane/steps/openroad.py` & `openlane-2.0.0b9/openlane/steps/openroad.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     dpl_variables,
     grt_variables,
     routing_layer_variables,
 )
 
 from ..config import Variable
 from ..state import State, DesignFormat
-from ..logging import debug, err, info, warn, console
+from ..logging import debug, err, info, warn, verbose
 from ..common import (
     Path,
     TclUtils,
     StringEnum,
     get_script_dir,
     get_tpe,
     mkdirp,
@@ -188,15 +188,15 @@
         """
         kwargs, env = self.extract_env(kwargs)
 
         views_updates, metrics_updates = super().run(state_in, env=env, **kwargs)
 
         metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
         if os.path.exists(metrics_path):
-            or_metrics_out = json.loads(open(metrics_path).read())
+            or_metrics_out = json.loads(open(metrics_path).read(), parse_float=Decimal)
             for key, value in or_metrics_out.items():
                 if value == "Infinity":
                     or_metrics_out[key] = inf
                 elif value == "-Infinity":
                     or_metrics_out[key] = -inf
             metrics_updates.update(or_metrics_out)
 
@@ -463,15 +463,15 @@
                 row.append(
                     format_count(
                         metric_updates_with_aggregates.get(f"{metric}{modifier}")
                     )
                 )
             table.add_row(*row)
 
-        console.print(table)
+        verbose(table)
         with open(os.path.join(self.step_dir, "summary.rpt"), "w") as f:
             rich.print(table, file=f)
 
         views_updates: ViewsUpdate = {}
         lib_dict = state_in[DesignFormat.LIB] or {}
         if not isinstance(lib_dict, dict):
             raise StepException(
```

### Comparing `openlane-2.0.0b8/openlane/steps/step.py` & `openlane-2.0.0b9/openlane/steps/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
+from decimal import Decimal
 
 import os
 import time
 import json
 import shutil
 import textwrap
 import subprocess
@@ -484,22 +485,26 @@
         :param pdk_root: The PDK root, which is needed for some utilities.
 
             If your utility doesn't require it, just keep the default value
             as-is.
         :returns: The created step object
         """
         config, _ = Config.load(
-            config_in=json.loads(open(config_path).read()),
+            config_in=json.loads(open(config_path).read(), parse_float=Decimal),
             flow_config_vars=Self.get_all_config_variables(),
             design_dir=".",
             pdk_root=pdk_root,
             _load_pdk_configs=False,
         )
         state_in = State.loads(open(state_in_path).read())
-        return Self(config=config, state_in=state_in)
+        return Self(
+            config=config,
+            state_in=state_in,
+            _no_revalidate_conf=True,
+        )
 
     @classmethod
     def get_all_config_variables(Self) -> List[Variable]:
         variables_by_name: Dict[str, Variable] = {
             variable.name: variable for variable in universal_flow_config_variables
         }
         for variable in Self.config_vars:
@@ -554,45 +559,47 @@
         # 1. Config
         dumpable_config = copy_recursive(self.config, translator=visitor)
         dumpable_config["meta"] = {
             "openlane_version": __version__,
             "step": self.__class__.id,
         }
 
-        # pdk_root = dumpable_config["PDK_ROOT"]
-        # pdk_root_resolved = os.path.join(".", "files", pdk_root[1:])
-        # dumpable_config["PDK_ROOT"] = pdk_root_resolved
         del dumpable_config["PDK_ROOT"]
 
         config_path = os.path.join(target_dir, "config.json")
         with open(config_path, "w") as f:
             f.write(json.dumps(dumpable_config, cls=GenericDictEncoder))
 
         # 2. State
         state_in = self.state_in.result()
         dumpable_state = copy_recursive(self.state_in.result(), translator=visitor)
         dumpable_state["metrics"] = state_in.metrics.to_raw_dict()
         state_path = os.path.join(target_dir, "state_in.json")
         with open(state_path, "w") as f:
             f.write(json.dumps(dumpable_state, cls=GenericDictEncoder))
 
-        # 3. Runner
-        script_path = os.path.join(target_dir, "run.sh")
+        # 3. Runner (OpenLane)
+        script_path = os.path.join(target_dir, "run_ol.sh")
         with open(script_path, "w") as f:
             f.write(
                 textwrap.dedent(
                     """
                     #!/bin/sh
                     set -e
-                    version="$(python3 -m openlane --bare-version)"
+                    python3 -m openlane --version
                     if [ "$?" != "0" ]; then
-                        echo "Failed to run 'python3 -m openlane --bare-version'."
+                        echo "Failed to run 'python3 -m openlane --version'."
                         exit -1
                     fi
-                    python3 -m openlane.steps run\\
+
+                    command=run
+                    if [ "$1" == "eject" ]; then
+                        command=eject
+                    fi
+                    python3 -m openlane.steps $command\\
                         --config ./config.json\\
                         --state-in ./state_in.json
                     """
                 ).strip()
             )
         if hasattr(os, "chmod"):
             os.chmod(script_path, 0o755)
```

### Comparing `openlane-2.0.0b8/openlane/steps/tclstep.py` & `openlane-2.0.0b9/openlane/steps/tclstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
         :param env: The input environment dictionary
         :param state: The input state
         :returns: a copy of the environment dictionary where ``self.config`` variables
         """
         env = env.copy()
 
-        env["SCRIPTS_DIR"] = get_script_dir()
+        env["SCRIPTS_DIR"] = os.path.abspath(get_script_dir())
         env["STEP_DIR"] = os.path.abspath(self.step_dir)
 
         tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
         if len(tech_lefs) != 1:
             raise StepException(
                 "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
             )
```

### Comparing `openlane-2.0.0b8/openlane/steps/yosys.py` & `openlane-2.0.0b9/openlane/steps/yosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
 import io
 import json
+from decimal import Decimal
 from abc import abstractmethod
 from typing import List, Optional, Tuple
 
 from .tclstep import TclStep
 from .step import ViewsUpdate, MetricsUpdate, Step
 
 from ..config import Variable
@@ -318,15 +319,15 @@
         return os.path.join(get_script_dir(), "yosys", "synthesize.tcl")
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         views_updates, metric_updates = super().run(state_in, **kwargs)
 
         stats_file = os.path.join(self.step_dir, "reports", "stat.json")
         stats_str = open(stats_file).read()
-        stats = json.loads(stats_str)
+        stats = json.loads(stats_str, parse_float=Decimal)
 
         metric_updates = {}
         metric_updates["design__instance__count"] = stats["design"]["num_cells"]
         if chip_area := stats["design"].get("area"):  # needs nonzero area
             metric_updates["design__instance__area"] = chip_area
 
         cells = stats["design"]["num_cells_by_type"]
```

### Comparing `openlane-2.0.0b8/openlane.egg-info/PKG-INFO` & `openlane-2.0.0b9/openlane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0b8 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0b9 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
```

### Comparing `openlane-2.0.0b8/openlane.egg-info/SOURCES.txt` & `openlane-2.0.0b9/openlane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/setup.py` & `openlane-2.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b8/test/conftest.py` & `openlane-2.0.0b9/test/conftest.py`

 * *Files identical despite different names*

