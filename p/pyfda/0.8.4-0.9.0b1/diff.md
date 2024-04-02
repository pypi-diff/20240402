# Comparing `tmp/pyfda-0.8.4.tar.gz` & `tmp/pyfda-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfda-0.8.4.tar", last modified: Tue Oct 10 12:17:43 2023, max compression
+gzip compressed data, was "pyfda-0.9.0b1.tar", last modified: Tue Apr  2 18:16:13 2024, max compression
```

## Comparing `pyfda-0.8.4.tar` & `pyfda-0.9.0b1.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-10-10 12:17:34.000000 pyfda-0.8.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-10-10 12:17:34.000000 pyfda-0.8.4/BUILDING.md
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2023-10-10 12:17:34.000000 pyfda-0.8.4/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5489 2023-10-10 12:17:34.000000 pyfda-0.8.4/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-10 12:17:34.000000 pyfda-0.8.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2023-10-10 12:17:34.000000 pyfda-0.8.4/LICENSE_GPLv3.md
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-10-10 12:17:34.000000 pyfda-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2023-10-10 12:17:43.885454 pyfda-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2023-10-10 12:17:34.000000 pyfda-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-10-10 12:17:34.000000 pyfda-0.8.4/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.861453 pyfda-0.8.4/pyfda/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.861453 pyfda-0.8.4/pyfda/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/bessel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/butter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/cheby1.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/cheby2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/delay.py
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/ellip.py
--rw-r--r--   0 runner    (1001) docker     (127)    25674 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/ellip_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)    18568 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/equiripple.py
--rw-r--r--   0 runner    (1001) docker     (127)    25219 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/firwin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15681 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filter_widgets/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    14993 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/filterbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/default_fx_img.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    23218 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/fx_ui_wq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    15201 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/no_fx_filter.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/old/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/old/delay/
--rw-r--r--   0 runner    (1001) docker     (127)    24656 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/delay/delay.png
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/delay/fx_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.865453 pyfda-0.8.4/pyfda/fixpoint_widgets/old/fir_df/
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    32749 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/fixpoint_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/fixpoint_widgets/old/fixpoint_helpers_nmigen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.857452 pyfda-0.8.4/pyfda/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.869453 pyfda-0.8.4/pyfda/images/icons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.873453 pyfda-0.8.4/pyfda/images/icons/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/action-redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/action-undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/appbar.disk.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/appbar.from_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/appbar.list.add.above.svg
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/appbar.list.delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/appbar.to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/brush.svg
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/circle-check.svg
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/circle-x.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/cog.svg
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/data-transfer-download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/data-transfer-upload.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/density_large.svg
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/density_medium.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/density_small.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ellipses_h.svg
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ellipses_v.svg
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/fullscreen-enter.svg
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/graph_90.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/grid_coarse.svg
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/grid_fine.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/grid_none.svg
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/home.svg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_help_24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_pause_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_play_arrow_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_stop_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_volume_up_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/lock-locked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/lock-unlocked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/magnifying-glass.svg
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/map-marker.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/quantize.svg
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/sort-ascending.svg
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/stars_black_24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/dark/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/fft.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.873453 pyfda-0.8.4/pyfda/images/icons/light/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/light/ic_pause_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-line-mkr.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-line.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-mkr.png
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-none.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-stem-mkr.png
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-stem.png
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-steps-mkr.png
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/plot_style-steps.png
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (127)    20271 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_256.png
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_48.png
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_64.png
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/icons/pyfda_icon_nobg.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.873453 pyfda-0.8.4/pyfda/images/unused/
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/appbar.base.select_grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/appbar.list.add.above_grey.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.877453 pyfda-0.8.4/pyfda/images/unused/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/audio_90.odg
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/audio_90.png
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/audio_90.svg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/ic_forward_10_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/ic_mic_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/ic_skip_next_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-pause-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-play-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-record-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-skip-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-skip-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-step-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-step-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/audio/media-stop-4x.png
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/camera-slr.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/graph_90.odg
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/graph_90.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/grid-four-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/grid-three-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/grid-two-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/ic_volume_mute_48px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/question-mark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/square_outlined.svg
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/table_chart_outlined.svg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/images/unused/table_outlined.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.877453 pyfda-0.8.4/pyfda/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/amplitude_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/freq_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21020 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/freq_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    44860 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_coeffs_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    37825 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_fixpoint_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22453 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_info_about.py
--rw-r--r--   0 runner    (1001) docker     (127)    36659 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_pz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_pz_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    18515 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/input_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20844 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/select_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/target_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/input_widgets/weight_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.881453 pyfda-0.8.4/pyfda/libs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/csv_option_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/frozendict.py
--rw-r--r--   0 runner    (1001) docker     (127)    12407 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39669 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_fft_windows_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    44490 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_fix_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    63688 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_io_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    61770 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_log_template.conf
--rw-r--r--   0 runner    (1001) docker     (127)    27576 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_qt_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    30574 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_sig_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/pyfda_template.conf
--rw-r--r--   0 runner    (1001) docker     (127)    30964 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/libs/tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/license_info.md
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/module_versions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.881453 pyfda-0.8.4/pyfda/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/mpl_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    29222 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_fft_win.py
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    92975 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_impz.py
--rw-r--r--   0 runner    (1001) docker     (127)    35600 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_impz_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_phi.py
--rw-r--r--   0 runner    (1001) docker     (127)    23911 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_pz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/plot_tau_g.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/plot_widgets/tran/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/tran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25287 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/tran/plot_tran_stim.py
--rw-r--r--   0 runner    (1001) docker     (127)    48939 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/tran/tran_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/plot_widgets/tran/tran_io_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/pyfda.qrc
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/pyfda_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    22055 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/pyfda_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/pyfdax.py
--rw-r--r--   0 runner    (1001) docker     (127)   124603 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/qrc_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/widget_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/widget_templates/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/filter_widgets/my_filter_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/widget_templates/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/fixpoint_widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/widget_templates/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/input_widgets/my_input_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.885454 pyfda-0.8.4/pyfda/widget_templates/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfda/widget_templates/plot_widgets/myplot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:17:43.861453 pyfda-0.8.4/pyfda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-10 12:17:43.000000 pyfda-0.8.4/pyfda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2023-10-10 12:17:34.000000 pyfda-0.8.4/pyfdax.spec
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-10-10 12:17:34.000000 pyfda-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 12:17:43.885454 pyfda-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-10-10 12:17:34.000000 pyfda-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/BUILDING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20501 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5489 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/LICENSE_GPLv3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.500084 pyfda-0.9.0b1/pyfda/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.504084 pyfda-0.9.0b1/pyfda/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/butter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/cheby1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/cheby2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/ellip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25670 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/ellip_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18633 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/equiripple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25308 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/firwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filter_widgets/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16671 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/filterbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.504084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/default_fx_img.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.508084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/fx_ui_wq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.508084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15201 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/no_fx_filter.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.508084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.508084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/delay/
+-rw-r--r--   0 runner    (1001) docker     (127)    24656 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/delay/delay.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/delay/fx_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.508084 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fir_df/
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32745 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fixpoint_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.496084 pyfda-0.9.0b1/pyfda/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.512084 pyfda-0.9.0b1/pyfda/images/icons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.516084 pyfda-0.9.0b1/pyfda/images/icons/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/action-redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/action-undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.disk.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.from_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.list.add.above.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.list.delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/brush.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/circle-check.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/circle-x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/cog.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/data-transfer-download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/data-transfer-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/density_large.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/density_medium.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/density_small.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ellipses_h.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ellipses_v.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/fullscreen-enter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/graph_90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/grid_coarse.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/grid_fine.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/grid_none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/home.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_help_24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_pause_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_play_arrow_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_stop_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_volume_up_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/lock-locked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/lock-unlocked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/magnifying-glass.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/map-marker.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/quantize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/sort-ascending.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/stars_black_24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/dark/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/fft.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.516084 pyfda-0.9.0b1/pyfda/images/icons/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/light/ic_pause_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-line-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-line.png
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-none.png
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-stem-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-stem.png
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-steps-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/plot_style-steps.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20271 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_nobg.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.520084 pyfda-0.9.0b1/pyfda/images/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/appbar.base.select_grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/appbar.list.add.above_grey.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.524084 pyfda-0.9.0b1/pyfda/images/unused/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.odg
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/ic_forward_10_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/ic_mic_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/ic_skip_next_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-pause-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-play-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-record-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-skip-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-skip-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-step-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-step-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/audio/media-stop-4x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/camera-slr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/graph_90.odg
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/graph_90.png
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/grid-four-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/grid-three-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/grid-two-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/ic_volume_mute_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/question-mark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/square_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/table_chart_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/images/unused/table_outlined.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.524084 pyfda-0.9.0b1/pyfda/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/amplitude_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/freq_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/freq_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44389 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_coeffs_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41600 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_fixpoint_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22453 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_info_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37044 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_pz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_pz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/input_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22058 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/select_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/target_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/input_widgets/weight_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.528084 pyfda-0.9.0b1/pyfda/libs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/csv_option_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12407 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39663 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_fft_windows_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56027 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_fix_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_fix_lib_amaranth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69700 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_io_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64897 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_log_template.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    29371 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_qt_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30576 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_sig_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/pyfda_template.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    31054 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/libs/tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/license_info.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/module_versions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.528084 pyfda-0.9.0b1/pyfda/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/mpl_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28959 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27109 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_fft_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35152 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93871 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_impz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34855 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_impz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_phi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23944 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_pz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/plot_tau_g.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/plot_widgets/tran/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/tran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25329 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/tran/plot_tran_stim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48845 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/tran/tran_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/plot_widgets/tran/tran_io_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/pyfda.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/pyfda_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/pyfda_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/pyfdax.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124603 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/qrc_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/widget_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/widget_templates/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/filter_widgets/my_filter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/widget_templates/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/fixpoint_widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/widget_templates/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/input_widgets/my_input_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda/widget_templates/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfda/widget_templates/plot_widgets/myplot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/pyfda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 18:16:13.000000 pyfda-0.9.0b1/pyfda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/pyfdax.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:16:13.532084 pyfda-0.9.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-02 18:16:07.000000 pyfda-0.9.0b1/setup.py
```

### Comparing `pyfda-0.8.4/AUTHORS.md` & `pyfda-0.9.0b1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/BUILDING.md` & `pyfda-0.9.0b1/BUILDING.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/CHANGELOG.md` & `pyfda-0.9.0b1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,36 @@
 # Changelog
+## [v0.9.0b1](https://github.com/chipmuenk/pyfda/tree/v0.9.0b1) (2024-04-02)
+### Changed settings and behaviour
+- Minimum initial number of data points in the y[n] tab now is 25
+- Initial width of rect pulse now is T_1 = 10
+
+### New features
+- load / save filters to 9 different memory locations
+- coefficients can be saved in CMSIS format directly via 'save coefficients', this
+  is no longer hidden in the CSV options
+- in 'float' mode, fixpoint widget is now invisible and fixpoint simulations are no longer run
+- filters can be saved and loaded in JSON format
+- show fixpoint ranges for input and output separately
+- filter coefficients can also be complex as float2frmt() now handles complex numbers
+- accept complex number of the kind +.234j (pos. sign, no leading zero)
+- add separate quantizers for partial products x*b and y*a in iir_df1_pyfixp
+- new fixpoint number format 'octal'
+- numexpr >= 2.8.8 is now required as '1j' is parsed by numexpr again
+
+### Bugfixes
+- fixed bugs w.r.t. behaviour of locking absolute frequencies in filter design widget
+- highlighting frequencies outside the first Nyquist zone 0 ... f_S resp. -f_S/2 ... f_S/2 didn't work
+  reliably
+- #243 where deleting all cells results in an index error
+- #239: lots of bugs fixed w.r.t. fixpoint and especially integer fixpoint behaviour
+- fix behaviour when no fixpoint filter exists for a filter class
+- lots of bugs fixed for loading / saving filters
+- fixed several bugs w.r.t. signalling, causing multiple executions of code and erroneous ui updates
+
 
 ## [v0.8.4](https://github.com/chipmuenk/pyfda/tree/v0.8.4) (2023-10-10)
 
 ### Bugfixes
 
 - Require numexpr <= 2.8.4 to avoid limitations / bugs of newer versions (https://github.com/pydata/numexpr/issues/442) which prevents parsing of complex arguments ["numexpr: Value error: Expression 1.0j has forbidden control characters."]
 - Fix deprecation of plt.stem(... 'use_line_collection' ...)  introduced in matplotlib 3.8.0.
```

### Comparing `pyfda-0.8.4/INSTALLATION.md` & `pyfda-0.9.0b1/INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/LICENSE.md` & `pyfda-0.9.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/LICENSE_GPLv3.md` & `pyfda-0.9.0b1/LICENSE_GPLv3.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/MANIFEST.in` & `pyfda-0.9.0b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/PKG-INFO` & `pyfda-0.9.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.8.4
+Version: 0.9.0b1
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
@@ -26,15 +26,15 @@
 License-File: AUTHORS.md
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.2.0
 Requires-Dist: matplotlib>=3.1
 Requires-Dist: pyqt5
 Requires-Dist: docutils
 Requires-Dist: mplcursors
-Requires-Dist: numexpr<=2.8.4
+Requires-Dist: numexpr>=2.8.8
 Requires-Dist: markdown
 
 pyfda
 ======
 ## Python Filter Design Analysis Tool
 
 pyfda is a GUI based tool in Python / Qt for analysing and designing discrete time filters. Fixpoint implementations (for some filter types) can be simulated.
```

### Comparing `pyfda-0.8.4/README.md` & `pyfda-0.9.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 pyfda source code ist distributed under a permissive MIT license, binaries / bundles come with a GPLv3 license due to bundled components with stricter licenses.
 
 ## Installing, running and uninstalling pyfda
 For details, see [INSTALLATION.md](INSTALLATION.md).
 ### Binaries
 Binaries can be downloaded under [Releases](https://github.com/chipmuenk/pyfda/releases) for versioned releases and for a latest release, automatically created for each push to the main branch.
 
-Binaries for **64 bit Windows** and **OS X** are created with **[pyInstaller](https://www.pyinstaller.org/)**. These executables self-extract to a temporary directory that is automatically deleted when pyfda is terminated (except when it crashes), they don't modify the system except for two ASCII configuration files and a log file. No additional software / libraries need to be installed, there is no interaction with existing python installations and you can simply overwrite or delete the executables when updating.
+Self-extracting archives for **64 bit Windows**, **OS X** and **Ubuntu Linux** are created with **[pyInstaller](https://www.pyinstaller.org/)**. The archives self-extract to a temporary directory that is automatically deleted when pyfda is terminated (except when it crashes), they don't modify the system except for two ASCII configuration files and a log file. No additional software / libraries need to be installed, there is no interaction with existing python installations and you can simply overwrite or delete the executables when updating. After downloading the Linux archive, you need to make it executable (`chmod 775 pyfda_linux`).
 
-Binaries for **Linux** are created as Flatpaks **(currently defunct)**, they can also be downloaded from **[Flathub](https://flathub.org/apps/details/com.github.chipmuenk.pyfda)**. Many Linux distros have built-in flatpak support, for others it's easy to install with e.g. `sudo apt install flatpak`. For details check the [Flatpak](https://www.flatpak.org/) home page.
+Binaries for **Linux** are created as Flatpaks as well **(currently defunct)** which can also be downloaded from **[Flathub](https://flathub.org/apps/details/com.github.chipmuenk.pyfda)**. Many Linux distros have built-in flatpak support, for others it's easy to install with e.g. `sudo apt install flatpak`. For details check the [Flatpak](https://www.flatpak.org/) home page.
 
 ### pip
 Supported Python versions are 3.7 ... 3.11, there is only one version of pyfda for all operating systems at [PyPI](https://pypi.org/project/pyfda/). As pyfda is a pure Python project (no compilation required), you can install pyfda the usual way, required libraries are downloaded automatically if missing:
 
     > pip install pyfda
 
 Upgrade:
@@ -58,39 +58,43 @@
 
     > pip uninstall pyfda
  
 <!--
 If you have cloned `pyfda` to your local drive you can install the local copy (i.e. create local config files and the `pyfdax` starter script) via
 
     > pip install -e <YOUR_PATH_TO_PYFDA_setup.py>
+
 -->
 
 #### Starting pyfda
 A pip installation creates a start script `pyfdax` in `<python>/Scripts` which should be in your path. So, simply start pyfda using
 
     > pyfdax
 
 The following libraries are required and installed automatically by pip when missing.
-* [**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and [**Qt5**](https://qt.io/)
-* [**numpy**](https://numpy.org/)
-* [**numexpr**](https://github.com/pydata/numexpr)
-* [**scipy**](https://scipy.org/): **1.2.0** or higher
-* [**matplotlib**](https://matplotlib.org/): **3.1** or higher
-* [**Markdown**](https://github.com/Python-Markdown/markdown)
+- [**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and [**Qt5**](https://qt.io/)
+- [**numpy**](https://numpy.org/)
+- [**numexpr**](https://github.com/pydata/numexpr)
+- [**scipy**](https://scipy.org/): **1.2.0** or higher
+- [**matplotlib**](https://matplotlib.org/): **3.1** or higher
+- [**Markdown**](https://github.com/Python-Markdown/markdown)
   
 **Optional libraries:**
+
 * [**mplcursors**](https://mplcursors.readthedocs.io/) for annotating cursors
 * [**docutils**](https://docutils.sourceforge.io) for rich text in documentation
 * **xlwt** and / or **XlsxWriter** for exporting filter coefficients as *.xls(x) files
 
 ### conda
 If you're working with Anaconda's packet manager conda, there is a recipe for pyfda on `conda-forge` since July 2023:
 
     > conda install --channel=conda-forge pyfda
 
+You should install pyfda into a new environment to avoid unwanted interaction with other installations.
+
 Start pyfda with
 
     > pyfdax
 
 ### git
 If you want to contribute to pyfda (great idea!), fork the latest version from https://github.com/chipmuenk/pyfda.git and create a local copy using
```

#### html2text {}

```diff
@@ -26,89 +26,92 @@
 stimulus]
 ## License pyfda source code ist distributed under a permissive MIT license,
 binaries / bundles come with a GPLv3 license due to bundled components with
 stricter licenses. ## Installing, running and uninstalling pyfda For details,
 see [INSTALLATION.md](INSTALLATION.md). ### Binaries Binaries can be downloaded
 under [Releases](https://github.com/chipmuenk/pyfda/releases) for versioned
 releases and for a latest release, automatically created for each push to the
-main branch. Binaries for **64 bit Windows** and **OS X** are created with **
-[pyInstaller](https://www.pyinstaller.org/)**. These executables self-extract
-to a temporary directory that is automatically deleted when pyfda is terminated
-(except when it crashes), they don't modify the system except for two ASCII
-configuration files and a log file. No additional software / libraries need to
-be installed, there is no interaction with existing python installations and
-you can simply overwrite or delete the executables when updating. Binaries for
-**Linux** are created as Flatpaks **(currently defunct)**, they can also be
+main branch. Self-extracting archives for **64 bit Windows**, **OS X** and
+**Ubuntu Linux** are created with **[pyInstaller](https://www.pyinstaller.org/
+)**. The archives self-extract to a temporary directory that is automatically
+deleted when pyfda is terminated (except when it crashes), they don't modify
+the system except for two ASCII configuration files and a log file. No
+additional software / libraries need to be installed, there is no interaction
+with existing python installations and you can simply overwrite or delete the
+executables when updating. After downloading the Linux archive, you need to
+make it executable (`chmod 775 pyfda_linux`). Binaries for **Linux** are
+created as Flatpaks as well **(currently defunct)** which can also be
 downloaded from **[Flathub](https://flathub.org/apps/details/
 com.github.chipmuenk.pyfda)**. Many Linux distros have built-in flatpak
 support, for others it's easy to install with e.g. `sudo apt install flatpak`.
 For details check the [Flatpak](https://www.flatpak.org/) home page. ### pip
 Supported Python versions are 3.7 ... 3.11, there is only one version of pyfda
 for all operating systems at [PyPI](https://pypi.org/project/pyfda/). As pyfda
 is a pure Python project (no compilation required), you can install pyfda the
 usual way, required libraries are downloaded automatically if missing: > pip
 install pyfda Upgrade: > pip install pyfda -U Uninstall: > pip uninstall pyfda
 #### Starting pyfda A pip installation creates a start script `pyfdax` in `/
 Scripts` which should be in your path. So, simply start pyfda using > pyfdax
 The following libraries are required and installed automatically by pip when
-missing. * [**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and
-[**Qt5**](https://qt.io/) * [**numpy**](https://numpy.org/) * [**numexpr**]
-(https://github.com/pydata/numexpr) * [**scipy**](https://scipy.org/):
-**1.2.0** or higher * [**matplotlib**](https://matplotlib.org/): **3.1** or
-higher * [**Markdown**](https://github.com/Python-Markdown/markdown) **Optional
+missing. - [**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and
+[**Qt5**](https://qt.io/) - [**numpy**](https://numpy.org/) - [**numexpr**]
+(https://github.com/pydata/numexpr) - [**scipy**](https://scipy.org/):
+**1.2.0** or higher - [**matplotlib**](https://matplotlib.org/): **3.1** or
+higher - [**Markdown**](https://github.com/Python-Markdown/markdown) **Optional
 libraries:** * [**mplcursors**](https://mplcursors.readthedocs.io/) for
 annotating cursors * [**docutils**](https://docutils.sourceforge.io) for rich
 text in documentation * **xlwt** and / or **XlsxWriter** for exporting filter
 coefficients as *.xls(x) files ### conda If you're working with Anaconda's
 packet manager conda, there is a recipe for pyfda on `conda-forge` since July
-2023: > conda install --channel=conda-forge pyfda Start pyfda with > pyfdax ###
-git If you want to contribute to pyfda (great idea!), fork the latest version
-from https://github.com/chipmuenk/pyfda.git and create a local copy using > git
-clone https://github.com/pyfda This command creates a new folder `pyfda` at
-your current directory level and copies the complete pyfda project into it.
-This [Github tutorial](https://docs.github.com/en/get-started/quickstart/fork-
-a-repo) provides a good starting point for working with git repos. pyfda can
-then be installed (i.e. creating local config files and the `pyfdax` starter
-script) from local files using > pip install -e Now you can edit the code and
-test it. If you're happy with it, push it to your repo and create a Pull
-Request so that the code can be reviewed and merged into the `chipmuenk/pyfda`
-repo. ## Building pyfda For details on how to publish pyfda to PyPI, how to
-create pyInstaller and Flatpak bundles, see [BUILDING.md](BUILDING.md). ##
-Customization The location of the following two configuration files (copied to
-user space) can be checked via the tab `Files -> About`: * Logging verbosity
-can be controlled via the file `pyfda_log.conf` * Widgets and filters can be
-enabled / disabled via the file `pyfda.conf`. You can also define one or more
-user directories containing your own widgets and / or filters. Layout and some
-default paths can be customized using the file `pyfda/pyfda_rc.py`, at the
-moment you have to edit that file at its original location. ## Features ###
-Filter design ### * **Design methods**: Equiripple, Firwin, Moving Average,
-Bessel, Butterworth, Elliptic, Chebyshev 1 and 2 (from scipy.signal and custom
-methods) * **Second-Order Sections** are used in the filter design when
-available for more robust filter design and analysis * **Fine-tune** manually
-the filter order and corner frequencies calculated by minimum order algorithms
-* **Compare filter designs** for a given set of specifications and different
-design methods * **Filter coefficients and poles / zeroes** can be displayed,
-edited and quantized in various formats ### User Interface ### * only widgets
-needed for the currently selected design method are visible * specifications
-are remembered when switching between filter design methods * enhanced
-Matplotlib NavigationToolbar (nicer icons, additional functions) * tooltips for
-all UI widgets and help files * specify frequencies as absolute values or
-normalized to sampling or Nyquist frequency * specify ripple and attenuations
-in dB, as voltage or as power ratios * enter values as expressions like `exp(-
-pi/4 * 1j)` using [numexpr](https://github.com/pydata/numexpr) syntax ###
-Graphical Analyses * Magnitude response (lin / power / log) with optional
-display of specification bands, phase and an inset plot * Phase response
-(wrapped / unwrapped) and group delay * Pole / Zero plot * Transient response
-(impulse, step and various stimulus signals) in the time and frequency domain.
-Define your own stimuli like `abs(sin(2*pi*n*f1))` using [numexpr](https://
-github.com/pydata/numexpr) syntax and the UI. * 3D-Plots (|H(f)|, mesh,
-surface, contour) with optional pole / zero display ### Modular Architecture
-Facilitate the implementation of new filter design / analysis / display
-methods. Generate your own * Filter design widgets with your algorithm *
-Plotting widgets * Input widgets * Fixpoint filter widgets, using the
+2023: > conda install --channel=conda-forge pyfda You should install pyfda into
+a new environment to avoid unwanted interaction with other installations. Start
+pyfda with > pyfdax ### git If you want to contribute to pyfda (great idea!),
+fork the latest version from https://github.com/chipmuenk/pyfda.git and create
+a local copy using > git clone https://github.com/pyfda This command creates a
+new folder `pyfda` at your current directory level and copies the complete
+pyfda project into it. This [Github tutorial](https://docs.github.com/en/get-
+started/quickstart/fork-a-repo) provides a good starting point for working with
+git repos. pyfda can then be installed (i.e. creating local config files and
+the `pyfdax` starter script) from local files using > pip install -e Now you
+can edit the code and test it. If you're happy with it, push it to your repo
+and create a Pull Request so that the code can be reviewed and merged into the
+`chipmuenk/pyfda` repo. ## Building pyfda For details on how to publish pyfda
+to PyPI, how to create pyInstaller and Flatpak bundles, see [BUILDING.md]
+(BUILDING.md). ## Customization The location of the following two configuration
+files (copied to user space) can be checked via the tab `Files -> About`: *
+Logging verbosity can be controlled via the file `pyfda_log.conf` * Widgets and
+filters can be enabled / disabled via the file `pyfda.conf`. You can also
+define one or more user directories containing your own widgets and / or
+filters. Layout and some default paths can be customized using the file `pyfda/
+pyfda_rc.py`, at the moment you have to edit that file at its original
+location. ## Features ### Filter design ### * **Design methods**: Equiripple,
+Firwin, Moving Average, Bessel, Butterworth, Elliptic, Chebyshev 1 and 2 (from
+scipy.signal and custom methods) * **Second-Order Sections** are used in the
+filter design when available for more robust filter design and analysis *
+**Fine-tune** manually the filter order and corner frequencies calculated by
+minimum order algorithms * **Compare filter designs** for a given set of
+specifications and different design methods * **Filter coefficients and poles /
+zeroes** can be displayed, edited and quantized in various formats ### User
+Interface ### * only widgets needed for the currently selected design method
+are visible * specifications are remembered when switching between filter
+design methods * enhanced Matplotlib NavigationToolbar (nicer icons, additional
+functions) * tooltips for all UI widgets and help files * specify frequencies
+as absolute values or normalized to sampling or Nyquist frequency * specify
+ripple and attenuations in dB, as voltage or as power ratios * enter values as
+expressions like `exp(-pi/4 * 1j)` using [numexpr](https://github.com/pydata/
+numexpr) syntax ### Graphical Analyses * Magnitude response (lin / power / log)
+with optional display of specification bands, phase and an inset plot * Phase
+response (wrapped / unwrapped) and group delay * Pole / Zero plot * Transient
+response (impulse, step and various stimulus signals) in the time and frequency
+domain. Define your own stimuli like `abs(sin(2*pi*n*f1))` using [numexpr]
+(https://github.com/pydata/numexpr) syntax and the UI. * 3D-Plots (|H(f)|,
+mesh, surface, contour) with optional pole / zero display ### Modular
+Architecture Facilitate the implementation of new filter design / analysis /
+display methods. Generate your own * Filter design widgets with your algorithm
+* Plotting widgets * Input widgets * Fixpoint filter widgets, using the
 integrated `Fixed()` class ### Import / Export * Filter designs in pickled and
 in numpy's NPZ-format * Coefficients and poles/zeros as comma-separated values
 (CSV) in numpy's NPY- and NPZ-formats, in Excel (R), as a Matlab (R) workspace
 or in FPGA vendor specific formats like Xilinx (R) COE-format * Transient
 stimuli (y[n] tab) as wav and csv files ## Why yet another filter design tool?
 * **Education:** Provide an easy-to-use FOSS tool for demonstrating basic
 digital stuff and filter design interactively that also works with the limited
```

### Comparing `pyfda-0.8.4/README_PYPI.md` & `pyfda-0.9.0b1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/filter_factory.py` & `pyfda-0.9.0b1/pyfda/filter_factory.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/bessel.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/bessel.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/butter.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/butter.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
          
    :2.2: Rename `filter_classes` -> `classes`, remove Py2 compatibility  
 """
 import scipy.signal as sig
 from scipy.signal import buttord
 
 from pyfda.libs.pyfda_lib import fil_save, lin2unit
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 
 __version__ = "2.2"
 
 classes = {'Butter':'Butterworth'}
 
 class Butter(object):
 
@@ -160,15 +160,15 @@
     #--------------------------------------------------------------------------
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 25:
-            return qfilter_warning(None, self.N, "Butterworth")
+            return popup_warning(None, self.N, "Butterworth")
         else:
             return True
 
     #--------------------------------------------------------------------------
     def _save(self, fil_dict, arg):
         """
         Convert results of filter design to all available formats (pz, ba, sos)
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/cheby1.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/cheby1.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    :2.2: Rename `filter_classes` -> `classes`, remove Py2 compatibility
 """
 import scipy.signal as sig
 from scipy.signal import cheb1ord
 
 from pyfda.libs.pyfda_lib import fil_save, lin2unit
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from .common import Common
 
 __version__ = "2.2"
 
 classes = {'Cheby1':'Chebyshev 1'} #: Dict containing class name : display name
 
 class Cheby1(object):
@@ -132,15 +132,15 @@
 
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 30:
-            return qfilter_warning(None, self.N, "Chebyshev 1")
+            return popup_warning(None, self.N, "Chebyshev 1")
         else:
             return True
 
 
     def _save(self, fil_dict, arg):
         """
         Convert results of filter design to all available formats (pz, ba, sos)
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/cheby2.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/cheby2.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
    :2.2: Rename `filter_classes` -> `classes`, remove Py2 compatibility
 """
 import scipy.signal as sig
 from scipy.signal import cheb2ord
 from .common import Common
 
 from pyfda.libs.pyfda_lib import fil_save, lin2unit
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 
 __version__ = "2.2"
 
 classes = {'Cheby2':'Chebyshev 2'} #: Dict containing class name : display name
 
 class Cheby2(object):
 
@@ -130,15 +130,15 @@
     #--------------------------------------------------------------------------
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 25:
-            return qfilter_warning(None, self.N, "Chebyshev 2")
+            return popup_warning(None, self.N, "Chebyshev 2")
         else:
             return True
 
     #--------------------------------------------------------------------------
     def _save(self, fil_dict, arg):
         """
         Convert results of filter design to all available formats (pz, ba, sos)
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/common.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/common.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/delay.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 from pyfda.libs.compat import QWidget, QLabel, QLineEdit, pyqtSignal, QVBoxLayout, QHBoxLayout
 
 import scipy.signal as sig
 import numpy as np
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_lib import fil_save, safe_eval
 
 __version__ = "1.0"
 
 classes = {'Delay':'Delay'} #: Dict containing class name : display name
 
 class Delay(QWidget):
@@ -150,15 +150,15 @@
         
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 2000:
-            return qfilter_warning(self, self.N, "Delay")
+            return popup_warning(self, self.N, "Delay")
         else:
             return True
 
     def _save(self, fil_dict, arg=None):
         """
         Convert between poles / zeros / gain, filter coefficients (polynomes)
         and second-order sections and store all available formats in the passed
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/ellip.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/ellip.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
          self.wdg and self.hdl
 
    :2.2: Rename `filter_classes` -> `classes`, remove Py2 compatibility
 """
 import scipy.signal as sig
 from scipy.signal import ellipord
 from pyfda.libs.pyfda_lib import fil_save, lin2unit
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 
 from .common import Common
 
 __version__ = "2.2"
 
 classes = {'Ellip':'Elliptic'} #: Dict containing class name : display name
 
@@ -126,15 +126,15 @@
     #--------------------------------------------------------------------------
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 25:
-            return qfilter_warning(None, self.N, "Elliptic")
+            return popup_warning(None, self.N, "Elliptic")
         else:
             return True
 
 
     #--------------------------------------------------------------------------
     def _save(self, fil_dict, arg):
         """
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/ellip_zero.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/ellip_zero.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 import os, io
 import scipy.signal as sig
 from numpy import conj, sqrt, sum, zeros
 import numpy as np
 from scipy.signal import ellipord
 from pyfda.libs.pyfda_lib import fil_save, lin2unit
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_io_lib import extract_file_ext
 import pyfda.libs.pyfda_dirs as dirs
 
 from .common import Common
 from pyfda.libs.compat import (QWidget, QFrame, pyqtSignal, QFileDialog,
                       QCheckBox, QVBoxLayout, QHBoxLayout, QPushButton)
 
@@ -286,15 +286,15 @@
 
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 30:
-            return qfilter_warning(self, self.N, "Zero-phase Elliptic")
+            return popup_warning(self, self.N, "Zero-phase Elliptic")
         else:
             return True
 
 #   custom save of filter dictionary
     def _save(self, fil_dict, arg):
         """
         First design initial elliptic filter meeting sqRoot Amp specs;
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/equiripple.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/equiripple.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 from pyfda.libs.compat import QWidget, QLabel, QLineEdit, pyqtSignal, QVBoxLayout, QHBoxLayout
 
 import scipy.signal as sig
 import numpy as np
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_lib import fil_save, round_odd, ceil_even, safe_eval
 from .common import remezord
 
 __version__ = "2.2"
 
 classes = {'Equiripple':'Equiripple'} #: Dict containing class name : display name
 
@@ -76,17 +76,18 @@
 
 ``scipy.signal.remez()``, ``pyfda_lib.remezord()``
     """
 
     sig_tx = pyqtSignal(object)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self):
+    def __init__(self, objectName='equiripple_inst'):
         QWidget.__init__(self)
 
+        self.setObjectName(objectName)
         self.grid_density = 16
 
         self.ft = 'FIR'
 
         self.rt_dicts = ('com',)
 
         self.rt_dict = {
@@ -252,15 +253,15 @@
 
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 2000:
-            return qfilter_warning(self, self.N, "Equiripple")
+            return popup_warning(self, self.N, "Equiripple")
         else:
             return True
 
     def _save(self, fil_dict, arg):
         """
         Convert between poles / zeros / gain, filter coefficients (polynomes)
         and second-order sections and store all available formats in the passed
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/firwin.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/firwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import numpy as np
 import scipy.signal as sig
 from scipy.signal import signaltools
 from scipy.special import sinc
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
 from pyfda.libs.pyfda_lib import fil_save, round_odd, pprint_log
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_fft_windows_lib import QFFTWinSelector, get_windows_dict
 from pyfda.plot_widgets.plot_fft_win import Plot_FFT_win
 from .common import Common, remezord
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -64,17 +64,18 @@
     FRMT = 'ba'     # output format(s) of filter design routines 'zpk' / 'ba' / 'sos'
                     # currently, only 'ba' is supported for firwin routines
 
     sig_tx = pyqtSignal(object)  # local signal between FFT widget and FFTWin_Selector
     sig_tx_local = pyqtSignal(object)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self):
+    def __init__(self, objectName='firwin_inst'):
         QWidget.__init__(self)
 
+        self.setObjectName(objectName)
         self.ft = 'FIR'
 
         win_names_list = ["Boxcar", "Rectangular", "Barthann", "Bartlett", "Blackman",
                           "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev", "DPSS",
                           "Flattop", "General Gaussian", "Gauss", "Hamming", "Hann",
                           "Kaiser", "Nuttall", "Parzen", "Triangular", "Tukey"]
         self.cur_win_name = "Kaiser"  # set initial window type
@@ -152,15 +153,15 @@
                 self.hide_fft_wdg()
                 return
             else:
                 if 'view_changed' in dict_sig and 'fft_win' in dict_sig['view_changed']:
                     # self._update_fft_window()  # TODO: needed?
                     # local connection to FFT window widget and qfft_win_select
                     self.emit(dict_sig, sig_name='sig_tx_local')
-                    # global connection to upper hierachies
+                    # global connection to upper hierarchies
                     # send notification that filter design has changed
                     self.emit({'filt_changed': 'firwin'})
 
     # --------------------------------------------------------------------------
     def construct_UI(self):
         """
         Create additional subwidget(s) needed for filter design:
@@ -171,15 +172,15 @@
         self.cmb_firwin_alg = QComboBox(self)
         self.cmb_firwin_alg.setObjectName('wdg_cmb_firwin_alg')
         self.cmb_firwin_alg.addItems(['ichige', 'kaiser', 'herrmann'])
         # Minimum size, can be changed in the upper hierarchy levels using layouts:
         self.cmb_firwin_alg.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmb_firwin_alg.hide()
 
-        self.qfft_win_select = QFFTWinSelector(self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict, objectName='fir_win_qfft')
         # Minimum size, can be changed in the upper hierarchy levels using layouts:
         # self.qfft_win_select.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.but_fft_wdg = QPushButton(self)
         self.but_fft_wdg.setIcon(QIcon(":/fft.svg"))
         but_height = self.qfft_win_select.sizeHint().height()
         self.but_fft_wdg.setIconSize(QSize(but_height, but_height))
@@ -280,15 +281,15 @@
 
     def _test_N(self):
         """
         Warn the user if the calculated order is too high for a reasonable filter
         design.
         """
         if self.N > 1000:
-            return qfilter_warning(self, self.N, "FirWin")
+            return popup_warning(self, self.N, "FirWin")
         else:
             return True
 
     def _save(self, fil_dict, arg):
         """
         Convert between poles / zeros / gain, filter coefficients (polynomes)
         and second-order sections and store all available formats in the passed
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/ma.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/ma.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from pyfda.libs.compat import (QWidget, QLabel, QLineEdit, pyqtSignal, QCheckBox,
                       QVBoxLayout, QHBoxLayout)
 
 import numpy as np
 
 import pyfda.filterbroker as fb
 from pyfda.libs.pyfda_lib import fil_save, fil_convert, ceil_odd, safe_eval
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_sig_lib import zeros_with_val
 
 __version__ = "2.2"
 
 classes = {'MA':'Moving Average'} #: Dict containing class name : display name
 
 class MA(QWidget):
@@ -68,17 +68,18 @@
 **Design routines:**
 
 ``ma.calc_ma()``
     """
     sig_tx = pyqtSignal(object)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self):
+    def __init__(self, objectName='ma_inst'):
         QWidget.__init__(self)
 
+        self.setObjectName(objectName)
         self.delays = 12 # number of delays per stage
         self.stages = 1 # number of stages
 
         self.ft = 'FIR'
 
         self.rt_dicts = ()
         # Common data for all filter response types:
@@ -323,15 +324,15 @@
             L = L + 1
             i = np.arange(L) # create N + 2 zeros around the unit circle and ...
             i = np.delete(i, [0, L // 2]) # ... remove first and middle element
 
             norm = np.sum(b0)
 
         if self.delays > 1000:
-            if not qfilter_warning(None, self.delays*self.stages, "Moving Average"):
+            if not popup_warning(None, self.delays*self.stages, "Moving Average"):
                 return -1
 
 
         z0 = np.exp(-2j*np.pi*i/L)
         # calculate filter for multiple cascaded stages
         for i in range(self.stages):
             b = np.convolve(b0, b)
```

### Comparing `pyfda-0.8.4/pyfda/filter_widgets/manual.py` & `pyfda-0.9.0b1/pyfda/filter_widgets/manual.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/filterbroker.py` & `pyfda-0.9.0b1/pyfda/filterbroker.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,24 +32,33 @@
 * http://stackoverflow.com/questions/13034496/using-global-variables-between-files-in-python
 * http://stackoverflow.com/questions/1977362/how-to-create-module-wide-variables-in-python
 * http://pymotw.com/2/articles/data_persistence.html
 * http://stackoverflow.com/questions/9058305/getting-attributes-of-a-class
 * http://stackoverflow.com/questions/2447353/getattr-on-a-module
 
 """
+import logging
+logger = logging.getLogger(__name__)
+
+import copy
+import time
 from collections import OrderedDict
 from pyfda.libs.frozendict import freeze_hierarchical
 
 clipboard = None
 """ Handle to central clipboard instance """
 
 base_dir = ""  #: Project base directory
 
-# State of filter design: "ok", "changed", "error", "failed", "active"
-design_filt_state = "changed"
+# State of filter design: 'ok', 'changed', 'error', 'failed', 'active'
+design_filt_state = 'changed'
+
+UNDO_LEN = 10  # depth of circular undo buffer
+undo_step = 0  # number of undo steps, limited to UNDO_LEN
+undo_ptr = 0  # pointer to current undo memory % UNDO_LEN
 
 #==============================================================================
 # -----------------------------------------------------------------------------
 # Dicts with class names found in the main configuration file,
 # parsed in `tree_builder.build_class_dict()`. Those initial definitions
 # are only meant as examples and for module test, they are overwritten during
 # the initialization.
@@ -88,23 +97,23 @@
      # FIR
      ('Equiripple', {'name': 'Equiripple', 'mod': 'pyfda.filter_widgets.equiripple'}),
      ('Firwin', {'name': 'Windowed FIR', 'mod': 'pyfda.filter_widgets.firwin'}),
      ('MA', {'name': 'Moving Average', 'mod': 'pyfda.filter_widgets.ma'}),
      ('Manual_FIR', {'name': 'Manual', 'mod': 'pyfda.filter_widgets.manual'}),
      ('Manual_IIR', {'name': 'Manual', 'mod': 'pyfda.filter_widgets.manual'})
      ])
-
 """
 The keys of this dictionary are the names of all found filter classes, the values
 are the name to be displayed e.g. in the comboboxes and the fully qualified
 name of the module containing the class.
 """
 
 # Dictionary describing the available combinations of response types (rt),
-# filter types (ft), design methods (dm) and filter order (fo):
+# filter types (ft), design methods (dm) and filter order (fo). This dictionary
+# is also overwritten during initialization:
 fil_tree = freeze_hierarchical({
     'LP': {
         'FIR': {
             'Equiripple': {
                 'man':{'fo':     ('a', 'N'),
                        'fspecs': ('a', 'F_C'),
                        'wspecs': ('a', 'W_PB', 'W_SB'),
@@ -215,105 +224,165 @@
                           }
                 }
         }
     })
 
 # -----------------------------------------------------------------------------
 # Dictionary containing current filter type, specifications, design and some
-# auxiliary information, the initial definition here is copied into fil[0]
-# and can be overwritten by input widgets and design routines
+# auxiliary information, the initial definition here is copied into fil[0] ... [9]
+# which can be modified by input widgets and design routines
 # ------------------------------------------------------------------------------
-fil_init = {'rt': 'LP', 'ft': 'IIR', 'fc': 'Cheby1', 'fo': 'man',  # filter type
-            'N': 10,  # filter order
-            'f_S': 1, 'T_S': 1,  # current sampling frequency and period
-            # 'f_s_wav': 16000,  # sampling frequency for wav files
-            'f_S_prev': 1,  # previous sampling frequency
-            'freq_locked': False,  # don't update absolute frequencies when f_S is changed
-            'f_s_scale': 1,  #
-            'f_max': 1,
-            'freqSpecsRangeType': 'Half',
-            'freqSpecsRange': [0, 0.5],
-            'freq_specs_sort': True,  # sort freq. specs in ascending order
-            'freq_specs_unit': 'f_S',
-            'plt_fLabel': r'$F = 2f \, / \, f_S = \Omega \, / \, \mathrm{\pi} \; \rightarrow$',
-            'plt_fUnit': 'f_S',
-            'plt_tLabel': r'$n \; \rightarrow$',
-            'plt_tUnit': 's',
-            'A_PB': 0.02, 'A_PB2': 0.01, 'F_PB': 0.1, 'F_PB2': 0.4, 'F_C': 0.2, 'F_N': 0.2,
-            'A_SB': 0.001, 'A_SB2': 0.0001, 'F_SB': 0.2, 'F_SB2': 0.3, 'F_C2': 0.4, 'F_N2': 0.4,
-            'W_PB': 1, 'W_PB2': 1, 'W_SB': 1, 'W_SB2': 1,
-            #
-            'ba': ([1, 1, 1], [1, 0.1, 0.5]),  # (bb, aa) tuple coefficient lists
-            # causal zeros/poles/gain
-            'zpk': [[-0.5 + 3**0.5/2.j, -0.5 - 3**0.5/2.j],
-                   [(2./3)**0.5 * 1j, -(2./3)**0.5 * 1j],
-                   [1, 0]],
-            #
-            'sos': [],
-            # input, output, accu, coeffs, ... fixpoint word formats and quantizer
-            # settings:
-            'fxqc':
-                {'QI': {'WI': 0, 'WF': 15, 'W': 16, 'ovfl': 'sat',  'quant': 'round',
-                        'fx_base': 'dec'},
-                 'QO': {'WI': 0, 'WF': 15, 'W': 16, 'ovfl': 'wrap', 'quant': 'floor',
-                        'fx_base': 'dec'},
-                 'QACC': {'WI': 0, 'WF': 31, 'W': 32, 'ovfl': 'wrap', 'quant': 'floor',
-                          'fx_base': 'dec'},
-                 'QCB': {'WI': 0, 'WF': 15, 'W': 16, 'ovfl': 'wrap', 'quant': 'floor',
-                         'scale': 1, 'fx_base': 'float'},
-                 'QCA': {'WI': 2, 'WF': 13, 'W': 16, 'ovfl': 'wrap', 'quant': 'floor',
-                         'scale': 1, 'fx_base': 'float'}
-                },
-                # 'b': [32768, 32768, 32768],
-                # 'a': [65536, 6553, 0]
-                # },
-            'fx_sim': False,  # fixpoint simulation mode 
-            'creator': ('ba', 'filterbroker'),  #(format ['ba', 'zpk', 'sos'], routine)
-            'amp_specs_unit': 'dB',
-
-            'plt_phiUnit': 'rad',
-            'plt_phiLabel': r'$\angle H(\mathrm{e}^{\mathrm{j} \Omega})$  in rad '\
-                    + r'$\rightarrow $',
-            'time_designed': -1,
-            'wdg_dyn': {'win': 'hann'},
-            # Parameters for spectral analysis window function
-            'win_fft':
-                {'name': 'Kaiser',  # Window name
-                 'fn_name': 'kaiser',  # function name or array with values
-                 'par': [{'name': '&beta;',
-                          'name_tex': r'$\beta$',
-                          'val': 10,
-                          'min': 0,
-                          'max': 30,
-                          'tooltip':
-                              ("<span>Shape parameter; lower values reduce main lobe width, "
-                              "higher values reduce side lobe level, typ. in the range "
-                              "5 ... 20.</span>")}],
-                 'n_par': 1,   # number of window parameters
-                 'info': "",     # Docstring for the window
-                 'win_len': 1024,
-                 },
-            # Parameters for filter design window function
-            'win_fir':
-                {'name': 'Hann',  # Window name
-                 'fn_name': 'hann',  # function name or array with values
-                 'par': [],    # set of list of window parameters
-                 'n_par': 0,   # number of window parameters
-                 'info': "",   # Docstring for the window
-                 'win_len': 1024
-                 }
-            }
+fil_ref = {
+    '_id': [], # a list with the keyword 'pyfda' and the version, e.g. ['pyfda', 1]
+    'info': 'Initial filter design',
+    'rt': 'LP', 'ft': 'IIR', 'fc': 'Cheby1', 'fo': 'man',  # filter type
+    'N': 10,  # filter order
+    'f_S': 1, 'T_S': 1,  # current sampling frequency and period
+    # 'f_s_wav': 16000,  # sampling frequency for wav files
+    'f_S_prev': 1,  # previous sampling frequency
+    'freq_locked': False,  # don't update absolute frequencies when f_S is changed
+    'f_s_scale': 1,  #
+    'f_max': 1,
+    'freqSpecsRangeType': 'Half',
+    'freqSpecsRange': [0, 0.5],
+    'freq_specs_sort': True,  # sort freq. specs in ascending order
+    'freq_specs_unit': 'f_S',
+    'plt_fLabel': r'$F = 2f \, / \, f_S = \Omega \, / \, \mathrm{\pi} \; \rightarrow$',
+    'plt_fUnit': 'f_S',
+    'plt_tLabel': r'$n \; \rightarrow$',
+    'plt_tUnit': 's',
+    'A_PB': 0.02, 'A_PB2': 0.01, 'F_PB': 0.1, 'F_PB2': 0.4, 'F_C': 0.2, 'F_N': 0.2,
+    'A_SB': 0.001, 'A_SB2': 0.0001, 'F_SB': 0.2, 'F_SB2': 0.3, 'F_C2': 0.4, 'F_N2': 0.4,
+    'W_PB': 1, 'W_PB2': 1, 'W_SB': 1, 'W_SB2': 1,
+    #
+    'ba': ([0.3, 0.3, 0.3], [1, 0, 0.66666666]),  # (bb, aa) tuple coefficient lists
+    # causal zeros/poles/gain
+    'zpk': [[-0.5 + 3**0.5/2.j, -0.5 - 3**0.5/2.j],
+            [(2./3)**0.5 * 1j, -(2./3)**0.5 * 1j],
+            [0.3, 0]],
+    #
+    'sos': [],
+    # global quantization format {'qint', 'qfrac'}
+    'qfrmt': 'qfrac',
+    # number format for fixpoint display {'dec', 'hex', 'bin', 'oct', 'csd'}
+    'fx_base': 'dec',
+
+    # Settings for quantization subwidgets:
+    #   'QI':input, 'QO': output, 'QCA': coeffs a, 'QCB': coeffs b, 'QACC': accumulator
+    #    (more subwidget can be added by fixpoint widgets if needed)
+    #  Keys:
+    #   'WI': integer bits, 'WF': fractional bits,
+    #   'w_a_m': word length automatic / manual calculation (not needed for 'QI', 'QO')
+    #   'ovfl': overflow behaviour, 'quant': quantizer behaviour
+    #   'N_over': number of overflows during last quantization process
+    'fxq':{
+        # Input quantization
+        'QI': {'WI': 0, 'WF': 15, 'w_a_m': 'm',
+               'ovfl': 'sat', 'quant': 'round', 'N_over': 0},
+        # Output quantization
+        'QO': {'WI': 0, 'WF': 15, 'w_a_m': 'm',
+               'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+        # 'b' coefficient quantization
+        'QCB': {'WI': 0, 'WF': 15, 'w_a_m': 'a',
+                'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+        # 'a' coefficient quantization
+        'QCA': {'WI': 2, 'WF': 13, 'w_a_m': 'a',
+                'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+        # accumulator quantization
+        'QACC': {'WI': 0, 'WF': 31, 'w_a_m': 'a',
+                 'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0}
+        },
+        # 'b': [32768, 32768, 32768],
+        # 'a': [65536, 6553, 0]
+        # },
+    'fx_sim': False,  # fixpoint simulation mode
+    'fx_mod_class_name': '',  # string with current fixpoint module and class
+    'creator': ('ba', 'filterbroker'),  #(format ['ba', 'zpk', 'sos'], routine)
+    'timestamp': time.time(),
+    'amp_specs_unit': 'dB',
+    'plt_phiUnit': 'rad',
+    'plt_phiLabel': r'$\angle H(\mathrm{e}^{\mathrm{j} \Omega})$  in rad '\
+            + r'$\rightarrow $',
+    # Parameters for spectral analysis window function
+    'win_fft':
+        {'name': 'Kaiser',  # Window name
+        'fn_name': 'kaiser',  # function name or array with values
+        'par': [{'name': '&beta;',
+                'name_tex': r'$\beta$',
+                'val': 10,
+                'min': 0,
+                'max': 30,
+                'tooltip':
+                    ("<span>Shape parameter; lower values reduce main lobe width, "
+                    "higher values reduce side lobe level, typ. in the range "
+                    "5 ... 20.</span>")}],
+        'n_par': 1,   # number of window parameters
+        'info': "",     # Docstring for the window
+        'win_len': 1024,
+        },
+    # dynamically instantiated filter widget
+    'wdg_fil' :
+        {'equiripple': {'grid_density': 16}},
+    # Parameters for filter design window function
+    'win_fir':
+        {'name': 'Hann',  # Window name
+            'fn_name': 'hann',  # function name or array with values
+            'par': [],    # set of list of window parameters
+            'n_par': 0,   # number of window parameters
+            'info': "",   # Docstring for the window
+            'win_len': 1024
+        }
+    }
 
-fil = [None] * 10  # create empty list with length 10 for multiple filter designs
-# This functionality is not implemented yet, currently only fil[0] is used
+  # create empty lists with length 10 for multiple filter designs and undo functions
+fil = [None] * 10
+fil_undo = [None] * 10
 
+# https://nedbatchelder.com/text/names.html :
 # define fil[0] as a dict with "built-in" default. The argument defines the default
 # factory that is called when a key is missing. Here, lambda simply returns a float.
 # When e.g. list is given as the default_factory, an empty list is returned.
 # fil[0] = defaultdict(lambda: 0.123)
 fil[0] = {}
 # Now, copy each key-value pair into the defaultdict
-for k in fil_init:
-    fil[0].update({k: fil_init[k]})
+# for k in fil_ref:
+#     fil[0].update({k: fil_ref[k]})
+
+# Copy fil_ref to fil[0] ... fil[9] to initialize all memories
+for l in range(len(fil)):
+    fil[l] = copy.deepcopy(fil_ref)
+
+def undo():
+    """
+    Restore current filter from undo memory `fil_undo`
+    """
+    global undo_step
+    global undo_ptr
+
+    # TODO: Limit undo memory to UNDO_LEN, implement circular buffer
+
+    # undo buffer is empty, don't copy anything
+    if undo_step < 1:
+        undo_step = 0
+        return -1
+    else:
+        fil[0] = copy.deepcopy(fil_undo[undo_ptr])
+        undo_step -= 1
+        undo_ptr = (undo_ptr + UNDO_LEN - 1) % UNDO_LEN
+
+def redo():
+    """
+    Store current filter to undo memory `fil_undo`
+    """
+    global undo_step
+    global undo_ptr
+
+    # prevent buffer overflow
+    undo_step += 1
+    if undo_step > UNDO_LEN:
+        undo_step = UNDO_LEN
+    # increase buffer pointer, allowing for circular wrap around
+    undo_ptr = (undo_ptr + 1) % UNDO_LEN
+    fil_undo[undo_ptr] = copy.deepcopy(fil[0])
 
-# Define dictionary with default settings for  FiXpoint Quantization and Coefficients:
-# 'fxqc'
+# Comparing nested dicts
+# https://stackoverflow.com/questions/27265939/comparing-python-dictionaries-and-nested-dictionaries
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/default_fx_img.png` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/default_fx_img.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df.png` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,18 @@
             When `len(zi) != len(b)`, truncate or fill up with zeros.
             When `zi == None`, all registers are filled with zeros.
 
         Returns
         -------
         None.
         """
+        # Do not initialize filter unless fixpoint mode is active
+        if not fb.fil[0]['fx_sim']:
+            return
+
         self.p = p  # parameter dictionary with coefficients etc.
 
         q_mul = p['QACC'].copy()
 
         # update the quantizers
         self.Q_b.set_qdict(self.p['QCB'])  # transversal coeffs.s
         self.Q_mul.set_qdict(q_mul)  # partial products
@@ -123,14 +127,15 @@
         Calculate FIR filter (direct form) response via difference equation with
         quantization. Registers can be initialized with `zi`.
 
         Parameters
         ----------
         x : array of float or float or None
             input value(s) scaled and quantized according to the setting of `p['QI']`
+            and fb.fil[0]['qfrmt']
             - When x is a scalar, calculate impulse response with the
                 amplitude defined by the scalar.
             - When `x == None`, calculate impulse response with amplitude = 1.
 
         zi : array-like
              initial conditions for filter memory; when `zi == None`, register contents
              from last run are used.
@@ -161,41 +166,49 @@
         # - quantize the partial products x*b, yielding xb_q
         # - accumulate the quantized partial products and quantize result, yielding y_q[k]
 
         self.zi = np.concatenate((self.zi, x))
 
         for k in range(len(x)):
             # partial products xb_q at time k, quantized with Q_mul:
-            xb_q = self.Q_mul.fixp(self.zi[k:k + self.L] * self.b_q)
+            xb_q = self.Q_mul.fixp(self.zi[k:k + self.L] * self.b_q,
+                                   in_frmt=fb.fil[0]['qfrmt'],
+                                   out_frmt=fb.fil[0]['qfrmt'])
             # accumulate x_bq to get accu[k]
-            y_q[k] = self.Q_acc.fixp(np.sum(xb_q))
+            y_q[k] = self.Q_acc.fixp(np.sum(xb_q), in_frmt=fb.fil[0]['qfrmt'],
+                                     out_frmt=fb.fil[0]['qfrmt'])
 
         self.zi = self.zi[-(self.L-1):]  # store last L-1 inputs (i.e. the L-1 registers)
 
         # Overflows in Q_mul are added to overflows in Q_Acc, then Q_mul is reset
         if self.Q_acc.q_dict['N_over'] > 0 or self.Q_mul.q_dict['N_over'] > 0:
             logger.warning(f"Overflows: N_Acc = {self.Q_acc.q_dict['N_over']}, "
                            f"N_Mul = {self.Q_mul.q_dict['N_over']}")
 
         self.Q_acc.q_dict['N_over'] = self.Q_acc.q_dict['N_over'] + self.Q_mul.q_dict['N_over']
         self.Q_mul.resetN()
 
-        return self.Q_O.fixp(y_q[:len(x)]), self.zi
+        return self.Q_O.requant(y_q[:len(x)], self.Q_acc), self.zi
 
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """
     Run widget standalone with
     `python -m pyfda.fixpoint_widgets.fir_df.fir_df_pyfixp`
     """
 
-    p = {'b': [1, 2, 3, 2, 1], 'QACC': {'Q': '4.3', 'ovfl': 'wrap', 'quant': 'round'},
-         'QI': {'Q': '2.3', 'ovfl': 'sat', 'quant': 'round'},
-         'QO': {'Q': '5.3', 'ovfl': 'wrap', 'quant': 'round'}
+    p = {'QCB': {'WI': 0, 'WF': 5, 'w_a_m': 'a',
+                'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+         'QACC': {'WI': 4, 'WF': 3, 'ovfl': 'wrap', 'quant': 'round'},
+         'QI': {'WI': 2, 'WF': 3, 'ovfl': 'sat', 'quant': 'round'},
+         'QO': {'WI': 5, 'WF': 3, 'ovfl': 'wrap', 'quant': 'round'}
          }
     dut = FIR_DF_pyfixp(p)
-    x = np.ones(4)
+    print("Filter fixpoint response and state variables for input =")
+    print("x = np.ones(7):")
+    x = np.ones(7)
     y = dut.fxfilter(x=x)
     print(y)
+    print("\nfollowed by x = np.zeros(5):")
     y = dut.fxfilter(x=np.zeros(5))
     print(y)
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,47 +42,59 @@
     def __init__(self):
         super().__init__()
 
         self.title = ("<b>Direct-Form (DF) FIR Filter</b>")
         self.description = "Standard FIR topology, suitable for most use cases."
         self.img_name = "fir_df.png"
 
+        self.cmb_wq_accu_items = [
+            "<span>Calculate word format manually / automatically</span>",
+            ("m", "M", "<span><b>Manual</b> entry of accumulator format.</span>"),
+            ("a", "A",
+            "<span><b>Automatic</b> calculation for given input word format "
+            "and coefficients (<i>coefficient area</i>).</span>"),
+            ("f", "F",
+            "<span><b>Full</b> accumulator width for given input word format "
+            "and arbitrary coefficients.</span>")
+            ]
+
         self._construct_UI()
         # Construct an instance of the fixpoint filter using the settings from
-        # the 'fxqc' quantizer dict
-        self.fx_filt = FIR_DF_pyfixp(fb.fil[0]['fxqc'])
-        self.update_disp()  # initial setting of overflow counter display
+        # the 'fxq' quantizer dict
+        self.fx_filt = FIR_DF_pyfixp(fb.fil[0]['fxq'])
+        self.update_ovfl_cnt_all()  # initialize all overflow counters / display
 
     # --------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the UI with widgets for coefficient format and input and
         output quantization
         """
         # widget for quantization of coefficients 'b'
-        # Attention: fb.fil[0]['fxqc']['QCB'] == self.wdg_wq_coeffs.q_dict
-        if 'QCB' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc'].update({'QCB': {}})  # no coefficient settings in dict yet
+        # Attention: fb.fil[0]['fxq']['QCB'] == self.wdg_wq_coeffs.q_dict
+        if 'QCB' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq'].update({'QCB': {}})  # no coefficient settings in dict yet
             logger.warning("QCB key missing")
         self.wdg_wq_coeffs = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QCB'], wdg_name='wq_coeffs',
+            fb.fil[0]['fxq']['QCB'], objectName='fx_ui_wq_fir_df_coeffs_b',
             label='<b>Coeff. Quantization <i>b<sub>I.F&nbsp;</sub></i>:</b>',
             MSB_LSB_vis='max')
         layV_wq_coeffs = QVBoxLayout()
         layV_wq_coeffs.addWidget(self.wdg_wq_coeffs)
 
         # widget for accumulator quantization
-        # Attention: fb.fil[0]['fxqc']['QACC'] == self.wdg_wq_accu.q_dict
-        if 'QACC' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc']['QACC'] = {}
-        set_dict_defaults(fb.fil[0]['fxqc']['QACC'],
-                          {'WI': 0, 'WF': 31, 'W': 32, 'ovfl': 'wrap', 'quant': 'floor'})
+        # Attention: fb.fil[0]['fxq']['QACC'] == self.wdg_wq_accu.q_dict
+        if 'QACC' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq']['QACC'] = {}
+        set_dict_defaults(fb.fil[0]['fxq']['QACC'],
+            {'WI': 0, 'WF': 31, 'ovfl': 'wrap', 'quant': 'floor', 'w_a_m': 'a',
+             'N_over': 0})
         self.wdg_wq_accu = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QACC'], wdg_name='wq_accu', cmb_w_vis='on',
-            cmb_w_init='auto',
+            fb.fil[0]['fxq']['QACC'], objectName='fx_ui_wq_fir_df_accu',
+            cmb_w_vis='on', cmb_w_items=self.cmb_wq_accu_items,
             label='<b>Accu Format <i>Q<sub>A&nbsp;</sub></i>:</b>')
         layV_wq_accu = QVBoxLayout()
         layV_wq_accu.addWidget(self.wdg_wq_accu)
 
         # ----------------------------------------------------------------------
         layVWdg = QVBoxLayout()
         # margins are created in input_fixpoint_specs widget
@@ -105,40 +117,42 @@
     def process_sig_rx(self, dict_sig=None):
         """
         - For locally generated signals (key = 'ui_local_changed'), emit
           `{'fx_sim': 'specs_changed'}` with local id.
           Update accu wordlengths for 'auto' or 'full' settings
 
         - For external changes, i.e. `{'fx_sim': 'specs_changed'}` or
-          `{'data_changed': xxx}` update the UI via `self.dict_ui`.
+          `{'data_changed': xxx}` update the UI via `self.dict2ui`.
 
         Ignore all other signals
 
         Note: If coefficient / accu quantization settings have been changed in the UI,
-        the referenced dicts `fb.fil[0]['fxqc']['QCB']` and `...['QACC']` have already
+        the referenced dicts `fb.fil[0]['fxq']['QCB']` and `...['QACC']` have already
         been updated by the corresponding subwidgets `FX_UI_WQ`
         """
-        logger.debug("sig_rx:\n{0}".format(pprint_log(dict_sig)))
+        # logger.warning("sig_rx:\n{0}".format(pprint_log(dict_sig)))
         if dict_sig['id'] == id(self):
             logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'ui_local_changed' in dict_sig:
             # signal generated locally by modifying coefficient / accu format
-            if not dict_sig['wdg_name'] in {'wq_coeffs', 'wq_accu'}:  # coeffs format
-                logger.error(f"Unknown widget name '{dict_sig['wdg_name']}' "
+            if not dict_sig['sender_name']\
+                    in {'fx_ui_wq_fir_df_coeffs_b', 'fx_ui_wq_fir_df_accu'}:
+                logger.error(f"Unknown widget name '{dict_sig['sender_name']}' "
                              f"in '{__name__}' !")
                 return
 
-            elif dict_sig['wdg_name'] == 'wq_accu':  # accu format updated
+            elif dict_sig['sender_name'] == 'fx_ui_wq_fir_df_accu':  # accu format updated
                 cmbW = qget_cmb_box(self.wdg_wq_accu.cmbW)
-                if cmbW in {'full', 'auto'}\
+                if cmbW in {'f', 'a'}\
                         or dict_sig['ui_local_changed'] in {'WF', 'WI'}:
                     self.update_accu_settings()
-                elif cmbW == 'man':  # switched to manual, don't do anything
+                elif cmbW == 'm':  # switched to manual, don't do anything
+                    # self.wdg_wq_accu.dict2ui()?
                     return
 
             # emit signal, replace id with id of *this* widget
             self.emit({'fx_sim': 'specs_changed', 'id': id(self)})
 
         # quantization dictionary has been updated outside the widget, update UI
         elif 'data_changed' in dict_sig or\
@@ -154,71 +168,71 @@
         Calculate number of extra integer bits for the accumulator (guard bits)
         depending on the coefficient area (sum of absolute coefficient
         values) for `cmbW == 'auto'` or depending on the number of coefficients
         for `cmbW == 'full'`. The latter works for arbitrary coefficients but
         requires more bits.
 
         The new values are written to the fixpoint coefficient dict
-        `fb.fil[0]['fxqc']['QACC']`.
+        `fb.fil[0]['fxq']['QACC']` and the UI is updated.
         """
         try:
-            if qget_cmb_box(self.wdg_wq_accu.cmbW) == "full":
+            if qget_cmb_box(self.wdg_wq_accu.cmbW) == 'f':
                 A_coeff = int(np.ceil(np.log2(len(fb.fil[0]['ba'][0]))))
-            elif qget_cmb_box(self.wdg_wq_accu.cmbW) == "auto":
+            elif qget_cmb_box(self.wdg_wq_accu.cmbW) == 'a':
                 A_coeff = int(np.ceil(np.log2(np.sum(np.abs(fb.fil[0]['ba'][0])))))
             else:
                 A_coeff = 0
         except BaseException as e: # Exception as e:
             logger.error("An error occured:", exc_info=True)
             return
 
-        # calculate required accumulator word format
-        if qget_cmb_box(self.wdg_wq_accu.cmbW) in {"full", "auto"}:
-            fb.fil[0]['fxqc']['QACC']['WF'] = fb.fil[0]['fxqc']['QI']['WF']\
-                + fb.fil[0]['fxqc']['QCB']['WF']
-            fb.fil[0]['fxqc']['QACC']['WI'] = fb.fil[0]['fxqc']['QI']['WI']\
-                + fb.fil[0]['fxqc']['QCB']['WI'] + A_coeff
-
-        # update quantization settings like 'Q', 'W' etc. and UI
-        self.wdg_wq_accu.QObj.set_qdict({})  # update `self.wdg_wq_accu.q_dict`
-        self.wdg_wq_accu.dict2ui()
+        # calculate required accumulator word format and update filter dict
+        if qget_cmb_box(self.wdg_wq_accu.cmbW) in {'f', 'a'}:
+            fb.fil[0]['fxq']['QACC']['WF'] = fb.fil[0]['fxq']['QI']['WF']\
+                + fb.fil[0]['fxq']['QCB']['WF']
+            fb.fil[0]['fxq']['QACC']['WI'] = fb.fil[0]['fxq']['QI']['WI']\
+                + fb.fil[0]['fxq']['QCB']['WI'] + A_coeff
+
+        # update UI and Q.q_dict (quantization settings) from filter dict
+        self.wdg_wq_accu.dict2ui(fb.fil[0]['fxq']['QACC'])
 
     # --------------------------------------------------------------------------
     def dict2ui(self):
         """
         Update all parts of the UI that need to be updated when specs have been
         changed outside this class, e.g. coefficients and coefficient wordlength.
         This also provides the initial setting for the widgets when the filter has
         been changed.
 
         This is called from one level above by
         :class:`pyfda.input_widgets.input_fixpoint_specs.Input_Fixpoint_Specs`.
         """
-        fxqc_dict = fb.fil[0]['fxqc']
-        if 'QACC' not in fxqc_dict:
-            fxqc_dict.update({'QACC': {}})  # no accumulator settings in dict yet
-            logger.warning("QA key missing")
+        fxq_dict = fb.fil[0]['fxq']
 
-        if 'QCB' not in fxqc_dict:
-            fxqc_dict.update({'QCB': {}})  # no coefficient settings in dict yet
-            logger.warning("QCB key missing")
+        # if 'QACC' not in fxq_dict:
+        #     fxq_dict.update({'QACC': {}})  # no accumulator settings in dict yet
+        #     logger.warning("'QACC' key missing")
+
+        # if 'QCB' not in fxq_dict:
+        #     fxq_dict.update({'QCB': {}})  # no coefficient settings in dict yet
+        #     logger.warning("'QCB' key missing in filter dict")
 
-        self.wdg_wq_coeffs.dict2ui()  # update coefficient wordlength
-        self.update_accu_settings()   # update accumulator settings and UI
+        self.wdg_wq_coeffs.dict2ui(fxq_dict['QCB'])  # update coefficient wordlength
+        self.update_accu_settings()   # update accumulator q settings and UI
 
     # --------------------------------------------------------------------------
-    def update_disp(self):
+    def update_ovfl_cnt_all(self):
         """
-        Update the overflow counters etc. of the UI after simulation has finished.
+        Update all overflow counters of the UI after simulation has finished.
 
         This is usually called from one level above by
         :class:`pyfda.input_widgets.input_fixpoint_specs.Input_Fixpoint_Specs`.
         """
-        self.wdg_wq_coeffs.update_disp()
-        self.wdg_wq_accu.update_disp()
+        self.wdg_wq_coeffs.update_ovfl_cnt()
+        self.wdg_wq_accu.update_ovfl_cnt()
 
     # --------------------------------------------------------------------------
     def fxfilter(self, stimulus):
         """
         Provide wrapper around fixpoint filter simulation method:
         * takes stimulus (iterable or float or None) as parameter
         * returns fixpoint response (ndarray of float)
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/fx_ui_wq.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/fx_ui_wq.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 # (see file LICENSE in root directory for details)
 
 """
 Helper classes and functions for generating and simulating fixpoint filters
 """
 import sys
 import inspect
+import copy
 
 # from numpy.lib.function_base import iterable
 
+import pyfda.filterbroker as fb
+from pyfda.libs.tree_builder import merge_dicts_hierarchically
 import pyfda.libs.pyfda_fix_lib as fx
 
 from pyfda.libs.compat import (
     Qt, QWidget, QLabel, QLineEdit, QComboBox, QPushButton, QIcon,
     QVBoxLayout, QHBoxLayout, QGridLayout, QFrame, pyqtSignal)
 
 from pyfda.libs.pyfda_qt_lib import (
@@ -28,86 +31,122 @@
 import logging
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
 class FX_UI_WQ(QWidget):
     """
-    Widget for selecting quantization / overflow options.
+    Subwidget for selecting and displaying fixpoint quantization / overflow options.
 
-    A reference to a quantization dictionary `q_dict` is passed to the constructor.
-    This can be a global quantization dict like `fb.fil[0]['fxqc']['QCB']` or a local
-    dict.
+    When ui subwidgets are modified, the dictionary specified during the construction
+    is modified.
 
-    This widget allows the user to modify the values for the following keys:
+    Subwidgets can be modified by calling the instance method `dict2ui(q_dict)`.
+    q_dict is an optional quantization dict, when omitted, the dictionary passed
+    during construction is used.
+
+    Constructor parameters
+    ----------------------
+    q_dict: dict
+        A dictionary containing the quantization settings that can be modified via
+        the UI of this widget. This is usually a global quantization dict like
+        `fb.fil[0]['fxq']['QCB']`, it can also be a local dict.
+
+        Attention: The dict is passed by reference, its values are modified via the UI.
+        The quantizer dict `self.Q.q_dict` contains a copy of these keys / values.
+
+    objectName: str
+        The string  is used to set the objectName of the Qt widget.
+
+    Returns
+    -------
+    None
+
+    The values for the following keys can be modified via the UI:
 
     - `quant`   : quantization behaviour
     - `ovfl`    : overflow behaviour
     - `WI`      : number of integer bits
     - `WF`      : number of fractional bits
-    - `scale`   : scaling factor between real world value and integer representation
 
-    These quantization settings are also stored in the instance quantizer object
-    `self.QObj`.
+    Programmatically, the values for the following keys can be modified.
+    - `w_a_m`   : automatic or manual update of word format
 
-    Widget settings are stored in the local `dict_ui` dictionary with the keys and their
-    default settings described below. When instantiating the widget, these settings can
-    be modified by corresponding keyword parameters, e.g.
 
-    ```
-        self.wdg_wq_accu = UI_WQ(
-            fb.fil[0]['fxqc']['QACC'], wdg_name='wq_accu',
-            label='<b>Accu Quantizer <i>Q<sub>A&nbsp;</sub></i>:</b>')
-    ```
+    Widget (UI) settings are stored in the local `ui_dict` dictionary with the keys and
+    their default settings described below.
 
-    All labels support HTML formatting.
 
-    'wdg_name'      : 'fx_ui_wq'                # widget name, used to discern between
-                                                # multiple instances
+        Key         : Default value             # Comment
+    ----------------:---------------------------#-------------------------------------
     'label'         : ''                        # widget text label, usually set by the
-
     'label_q'       : 'Quant.'                  # subwidget text label
     'cmb_q'         : List with tooltip and combo box choices (default: 'round', 'fix',
                         'floor'), see `pyfda_qt_lib.qcmb_box_populate()` or code below
-    'quant'         : 'round'                   # initial / current setting
 
     'label_ov'      : 'Ovfl.'                   # subwidget text label
     'cmb_ov'        : List with tooltip and combo box choices (default: 'wrap', 'sat')
-    'ovfl'          : 'wrap'                    # initial / current setting
 
     'fractional'    : True                      # Display WF, otherwise WF=0
     'lbl_sep'       : '.'                       # label between WI and WF field
     'max_led_width' : 30                        # max. length of lineedit field
-    'WI'            : 0                         # number of frac. *bits*
     'WI_len'        : 2                         # max. number of integer *digits*
     'tip_WI'        : 'Number of integer bits'  # Mouse-over tooltip
-    'WF'            : 15                        # number of frac. *bits*
     'WF_len'        : 2                         # max. number of frac. *digits*
     'tip_WF'        : 'Number of frac. bits'    # Mouse-over tooltip
 
     'lock_vis'      : 'off''                    # Pushbutton for locking visible
-    'tip_lock'      : 'Sync input/output quant.'# Tooltip for  lock push button
+    'tip_lock'      : 'Sync input/output quant.'# Tooltip for lock push button
 
-    'cmb_w_vis'     : 'off'                     # Integrated combo widget visible?
+    'cmb_w_vis'     : 'off'                     # Is Auto/Man. selection visible?
+                                                #  ['a', 'm', 'f']
     'cmb_w_items'   : List with tooltip and combo box choices
-    'cmb_w_init'    : 'man'                     # initial setting
     'count_ovfl_vis': 'on'                      # Is overflow counter visible?
                                                 #   ['on', 'off', 'auto']
     'MSB_LSB_vis'   : 'off'                     # Are MSB / LSB settings visible?
+
+
+    All labels support HTML formatting.
+
+    When instantiating the widget, these settings can be modified by setting keyword
+    parameters, e.g.:
+
+    ```
+        self.wdg_wq_accu = FX_UI_WQ(
+            fb.fil[0]['fxq']['QACC'], objectName='wdg_wq_accu_inst',
+            label='<b>Accu Quantizer <i>Q<sub>A&nbsp;</sub></i>:</b>')
+    ```
+
+
     """
     # sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outcgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, q_dict: dict, **kwargs) -> None:
+    def __init__(self, q_dict: dict, objectName: str = 'fx_ui_wq_inst',
+                 **kwargs) -> None:
         super().__init__()
 
+        self.setObjectName(objectName)
+        if not q_dict:
+            logger(crash)
+
+        # default settings for q_dict
+        # q_dict_default = {'WI': 0, 'WF': 15, 'w_a_m': 'm', 'quant': 'round',
+        #                   'ovfl': 'sat'}
+        # make a deep copy of passed dictionary to prevent messing it up
+        # self.q_dict = copy.deepcopy(q_dict)
+        # merge 'q_dict_default' into `self.q_dict``, prioritizing `self.q_dict`` entries
+        # merge_dicts_hierarchically(self.q_dict, q_dict_default)
+
         self.q_dict = q_dict
+
         self._construct_UI(**kwargs)
 
+    # This is not needed, it is called from one level above
     # # --------------------------------------------------------------------------
     # def process_sig_rx(self, dict_sig=None):
     #     """ Update the UI when the quantization dictionary has been updated outside
     #         (signal `{'fx_sim': 'specs_changed'}` received)"""
 
     #     logger.warning("sig_rx:\n{0}".format(dict_sig))
 
@@ -127,126 +166,118 @@
                   "<span>No quantization (only for debugging)</span>")]
         cmb_ov = ["<span>Select overflow behaviour.</span>",
                   ("wrap", "Wrap", "Two's complement wrap around"),
                   ("sat", "Sat",
                    "<span>Saturation, i.e. limit at min. / max. value</span>"),
                   ("none", "None",
                    "<span>No overflow behaviour (only for debugging)</span>")]
-        cmb_w = ["<span>Set Accumulator word format</span>",
-                 ("man", "M", "<span><b>Manual</b> entry of accumulator format.</span>"),
-                 ("auto", "A",
-                  "<span><b>Automatic</b> calculation for given input word format "
-                  "and coefficients (<i>coefficient area</i>).</span>"),
-                 ("full", "F",
-                  "<span><b>Full</b> accumulator width for given input word format "
-                  "and arbitrary coefficients.</span>")
-                 ]
+        cmb_w = ["<span>Select word format manually / automatically</span>",
+                ("m", "M", "<span><b>Manual</b> entry of integer and fractional "
+                "word length.</span>"),
+                ("a", "A", "<span><b>Automatic</b> estimation of required integer "
+                 "and fractional word length.</span>")                 ]
         # default widget settings:
-        dict_ui = {'wdg_name': 'fx_ui_wq', 'label': '',
-                   'label_q': 'Quant.', 'cmb_q_items': cmb_q, 'quant': 'round',
-                   'label_ov': 'Ovfl.', 'cmb_ov_items': cmb_ov, 'ovfl': 'wrap',
+        ui_dict = {'label': '',
+                   'label_q': 'Quant.', 'cmb_q_items': cmb_q,
+                   'label_ov': 'Ovfl.', 'cmb_ov_items': cmb_ov,
                    #
                    'lbl_sep': '.', 'max_led_width': 30,
-                   'WG': 0, 'WG_len': 2, 'tip_WG': 'Number of guard bits',
-                   'WI': 0, 'WI_len': 2, 'tip_WI': 'Number of integer bits',
-                   'WF': 15, 'WF_len': 2, 'tip_WF': 'Number of fractional bits',
+                   'WI_len': 2, 'tip_WI': 'Number of integer bits',
+                   'WF_len': 2, 'tip_WF': 'Number of fractional bits',
                    'fractional': True,
-                   'cmb_w_vis': 'off', 'cmb_w_items': cmb_w, 'cmb_w_init': 'man',
+                   'cmb_w_vis': 'on', 'cmb_w_items': cmb_w,
                    'lock_vis': 'off',
                    'tip_lock':
                        '<span>Sync input and output quantization formats.</span>',
                    'count_ovfl_vis': 'auto', 'MSB_LSB_vis': 'off'
                    }
 
-        # update local `dict_ui` with keyword arguments passed during construction
+        # update local `ui_dict` with keyword arguments passed during construction
         for key, val in kwargs.items():
-            if key not in dict_ui:
+            if key not in ui_dict:
                 logger.warning(f"Unknown key '{key}'")
             else:
-                dict_ui.update({key: val})
-        # dict_ui.update(map(kwargs)) # same as above?
+                ui_dict.update({key: val})
+        # ui_dict.update(map(kwargs)) # same as above?
 
-        self.wdg_name = dict_ui['wdg_name']
-        lbl_wdg = QLabel(dict_ui['label'], self)
+        lbl_wdg = QLabel(ui_dict['label'], self)
 
-        self.cmbQuant = QComboBox(self)
-        qcmb_box_populate(self.cmbQuant, dict_ui['cmb_q_items'], dict_ui['quant'])
-        self.cmbQuant.setObjectName('quant')
-
-        self.cmbOvfl = QComboBox(self)
-        qcmb_box_populate(self.cmbOvfl, dict_ui['cmb_ov_items'], dict_ui['ovfl'])
-        self.cmbOvfl.setObjectName('ovfl')
+        self.cmbQuant = QComboBox(self, objectName='quant')
+        idx = qcmb_box_populate(self.cmbQuant, ui_dict['cmb_q_items'], self.q_dict['quant'])
+        if idx == -1:
+            logger.warning(
+                f"""Initialization value "{self.q_dict['quant']}" was not found in """
+                f"""'quant' combo box.""")
+
+        self.cmbOvfl = QComboBox(self, objectName='ovfl')
+        idx = qcmb_box_populate(self.cmbOvfl, ui_dict['cmb_ov_items'], self.q_dict['ovfl'])
+        if idx == -1:
+            logger.warning(
+                f"""Initialization value "{self.q_dict['ovfl']}" was not found in """
+                f"""'ovfl' combo box.""")
 
         # ComboBox size is adjusted automatically to fit the longest element
         self.cmbQuant.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmbOvfl.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
-        self.cmbW = QComboBox(self)
-        qcmb_box_populate(self.cmbW, dict_ui['cmb_w_items'], dict_ui['cmb_w_init'])
-        self.cmbW.setVisible(dict_ui['cmb_w_vis'] == 'on')
-        self.cmbW.setObjectName("cmbW")
+        self.cmbW = QComboBox(self, objectName="cmbW")
+        idx = qcmb_box_populate(self.cmbW, ui_dict['cmb_w_items'], self.q_dict['w_a_m'])
+        if idx == -1:
+            logger.warning(
+                f"""Initialization value "{self.q_dict['w_a_m']}" was not found in """
+                f"""'auto/man' combo box.""")
+        self.cmbW.setVisible(ui_dict['cmb_w_vis'] == 'on')
 
         self.butLock = QPushButton(self)
         self.butLock.setCheckable(True)
         self.butLock.setChecked(False)
-        self.butLock.setVisible(dict_ui['lock_vis'] == 'on')
-        self.butLock.setToolTip(dict_ui['tip_lock'])
+        self.butLock.setVisible(ui_dict['lock_vis'] == 'on')
+        self.butLock.setToolTip(ui_dict['tip_lock'])
         self.butLock.setFixedWidth(self.butLock.height())
         # retain size of lock widget even when hidden
         sp_retain = self.butLock.sizePolicy()
         sp_retain.setRetainSizeWhenHidden(True)
         self.butLock.setSizePolicy(sp_retain)
 
-        self.ledWG = QLineEdit(self)
-        self.ledWG.setToolTip("<span>Number of guard bits</span>")
-        self.ledWG.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
-        self.ledWG.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
-        self.ledWG.setVisible(False)
-        self.ledWG.setObjectName("WG")
-
-        self.lblPlus = QLabel("+", self)
-        self.lblPlus.setVisible(False)
-
-        self.ledWI = QLineEdit(self)
-        self.ledWI.setToolTip(dict_ui['tip_WI'])
-        self.ledWI.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
-        self.ledWI.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
-        self.ledWI.setObjectName("WI")
-
-        self.lblDot = QLabel(dict_ui['lbl_sep'], self)
-        self.lblDot.setVisible(dict_ui['fractional'])
-
-        self.ledWF = QLineEdit(self)
-        self.ledWF.setToolTip(dict_ui['tip_WF'])
-        self.ledWF.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
-        self.ledWF.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
-        self.ledWF.setVisible(dict_ui['fractional'])
-        self.ledWF.setObjectName("WF")
+        self.ledWI = QLineEdit(self, objectName="WI")
+        self.ledWI.setToolTip(ui_dict['tip_WI'])
+        self.ledWI.setMaxLength(ui_dict['WI_len'])  # maximum of 2 digits
+        self.ledWI.setFixedWidth(ui_dict['max_led_width'])  # width of lineedit in points
+
+        self.lbl_sep1 = QLabel(to_html(ui_dict['lbl_sep'], frmt='b'), self)
+        self.lbl_sep1.setVisible(ui_dict['fractional'])
+        self.lbl_sep2 = QLabel(to_html(')', frmt='b'), self)
+        self.lbl_sep2.setVisible(False)
+
+        self.ledWF = QLineEdit(self, objectName="WF")
+        self.ledWF.setToolTip(ui_dict['tip_WF'])
+        self.ledWF.setMaxLength(ui_dict['WI_len'])  # maximum of 2 digits
+        self.ledWF.setFixedWidth(ui_dict['max_led_width'])  # width of lineedit in points
+        self.ledWF.setVisible(ui_dict['fractional'])
 
-        self.count_ovfl_vis = dict_ui['count_ovfl_vis']
+        self.count_ovfl_vis = ui_dict['count_ovfl_vis']
         self.lbl_ovfl_count = QLabel(to_html("N_ov = 0"))
         self.lbl_ovfl_count.setAutoFillBackground(True)
 
-        self.MSB_LSB_vis = dict_ui['MSB_LSB_vis']
+        self.MSB_LSB_vis = ui_dict['MSB_LSB_vis']
 
         # -------------------------------------------------------------------
         # MSB / LSB size
         # ---------------------------------------------------------------------
         self.lbl_MSB = QLabel(self)
         self.lbl_MSB.setText("undefined")
 
         self.lbl_LSB = QLabel(self)
         self.lbl_LSB.setText("undefined")
 
         layH_W = QHBoxLayout()
-        layH_W.addWidget(self.ledWG)
-        layH_W.addWidget(self.lblPlus)
         layH_W.addWidget(self.ledWI)
-        layH_W.addWidget(self.lblDot)
+        layH_W.addWidget(self.lbl_sep1)
         layH_W.addWidget(self.ledWF)
+        layH_W.addWidget(self.lbl_sep2)
         layH_W.setContentsMargins(0, 0, 0, 0)
 
         layG = QGridLayout()
         layG.setColumnStretch(1, 10)
         # first row
         layG.addWidget(lbl_wdg, 0, 0)
         layG.addWidget(self.butLock, 0, 3)
@@ -269,258 +300,275 @@
         layVMain.setContentsMargins(0, 0, 0, 0)
 
         self.setLayout(layVMain)
 
         # ----------------------------------------------------------------------
         # INITIAL SETTINGS OF UI AND FIXPOINT QUANTIZATION OBJECT
         # ----------------------------------------------------------------------
-        WG = int(dict_ui['WG'])
-        WI = int(dict_ui['WI'])
-        WF = int(dict_ui['WF'])
+        WI = int(self.q_dict['WI'])
+        WF = int(self.q_dict['WF'])
         W = WI + WF + 1
-        self.ledWG.setText(str(WG))
         self.ledWI.setText(str(WI))
         self.ledWF.setText(str(WF))
-        ovfl = qget_cmb_box(self.cmbOvfl)
-        quant = qget_cmb_box(self.cmbQuant)
 
-        self.q_dict.update({'ovfl': ovfl, 'quant': quant, 'WI': WI, 'WF': WF,
-                            'WG': WG, 'W': W})
         # create fixpoint quantization object from passed quantization dict
-        self.QObj = fx.Fixed(self.q_dict)
+        self.Q = fx.Fixed(self.q_dict)
+        # use only self.Q.q_dict from here on!!
 
         # initialize button icon
-        self.butLock_clicked(self.butLock.isChecked())
-
-        # initialize overflow counter and MSB / LSB display
-        self.update_disp()
+        self.but_lock_update_icon(self.butLock.isChecked())
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS
         # ----------------------------------------------------------------------
         # self.sig_rx.connect(self.process_sig_rx)
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.cmbOvfl.currentIndexChanged.connect(self.ui2dict)
         self.cmbQuant.currentIndexChanged.connect(self.ui2dict)
-        self.ledWG.editingFinished.connect(self.ui2dict)
         self.ledWI.editingFinished.connect(self.ui2dict)
         self.ledWF.editingFinished.connect(self.ui2dict)
         self.cmbW.currentIndexChanged.connect(self.ui2dict)
 
-        self.butLock.clicked.connect(self.butLock_clicked)
+        self.butLock.clicked.connect(self.but_lock_checked)
+
+        # initialize the UI from the global dictionary
+        self.dict2ui()
+        # reset overflow counter and update MSB / LSB display
+        self.update_ovfl_cnt()
+
+    # --------------------------------------------------------------------------
+    def but_lock_checked(self, checked: bool) -> None:
+        """
+        Update the icon of the push button depending on its state (checked or not)
+        and fire the signal {'ui_local_changed': 'butLock'}
+        """
+        self.but_lock_update_icon(checked)
+        self.emit({'sender_name': self.objectName(), 'ui_local_changed': 'butLock'})
 
     # --------------------------------------------------------------------------
-    def butLock_clicked(self, clicked):
+    def but_lock_update_icon(self, checked: bool) -> None:
         """
         Update the icon of the push button depending on its state
         """
-        if clicked:
+        if checked:
             self.butLock.setIcon(QIcon(':/lock-locked.svg'))
         else:
             self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
-
-        dict_sig = {'wdg_name': self.wdg_name, 'ui_local_changed': 'butLock'}
-        self.emit(dict_sig)
+        return
 
     # --------------------------------------------------------------------------
-    def update_disp(self):
+    def update_ovfl_cnt(self):
         """
         Update the overflow counter and MSB / LSB display (if visible)
         """
-        if self.MSB_LSB_vis == 'off':
-            self.lbl_MSB.setVisible(False)
-            self.lbl_LSB.setVisible(False)
-        elif self.MSB_LSB_vis == 'max':
-            self.lbl_MSB.setVisible(True)
-            self.lbl_LSB.setVisible(True)
-            self.lbl_MSB.setText(
-                "<b><i>&nbsp;&nbsp;Max</i><sub>10</sub> = </b>"
-                f"{self.QObj.q_dict['MAX']:.{params['FMT_ba']}g}")
-            self.lbl_LSB.setText(
-                "<b><i>LSB</i><sub>10</sub> = </b>"
-                f"{self.QObj.q_dict['LSB']:.{params['FMT_ba']}g}")
-        elif self.MSB_LSB_vis == 'msb':
-            self.lbl_MSB.setVisible(True)
-            self.lbl_LSB.setVisible(True)
-            self.lbl_MSB.setText(
-                "<b><i>&nbsp;&nbsp;MSB</i><sub>10</sub> = </b>"
-                f"{self.QObj.q_dict['MSB']:.{params['FMT_ba']}g}")
-            self.lbl_LSB.setText(
-                "<b><i>LSB</i><sub>10</sub> = </b>"
-                f"{self.QObj.q_dict['LSB']:.{params['FMT_ba']}g}")
-        else:
-            logger.error(f"Unknown option MSB_LSB_vis = '{self.MSB_LSB_vis}'")
         # -------
-        frm = inspect.stack()[1]
-        logger.debug(f"update: {id(self)}|{id(self.q_dict)} | {self.wdg_name} :"
-                     f"{self.q_dict['N_over']} "
-                     f"{inspect.getmodule(frm[0]).__name__.split('.')[-1]}."
-                     f"{frm[3]}:{frm[2]}")
+        # frm = inspect.stack()[1]
+        # logger.warning(f"update: {id(self)}|{id(self.q_dict)}:"
+        #              f"{self.q_dict['N_over']} "
+        #              f"{inspect.getmodule(frm[0]).__name__.split('.')[-1]}."
+        #              f"{frm[3]}:{frm[2]}")
 
         if self.count_ovfl_vis == 'off':
             self.lbl_ovfl_count.setVisible(False)
-        elif self.count_ovfl_vis == 'auto' and self.q_dict['N_over'] == 0:
+        elif self.count_ovfl_vis == 'auto' and self.Q.q_dict['N_over'] == 0:
             self.lbl_ovfl_count.setVisible(False)
         elif self.count_ovfl_vis == 'on' or\
-                self.count_ovfl_vis == 'auto' and self.q_dict['N_over'] > 0:
+                self.count_ovfl_vis == 'auto' and self.Q.q_dict['N_over'] > 0:
 
             self.lbl_ovfl_count.setVisible(True)
             self.lbl_ovfl_count.setText(
-                to_html(f"<b><i>&nbsp;&nbsp;N_ov </i>= {self.q_dict['N_over']}</b>"))
-            if self.q_dict['N_over'] == 0:
+                to_html(
+                    f"<b><i>&nbsp;&nbsp;N_ov </i>= {self.Q.q_dict['N_over']}</b>"))
+            if self.Q.q_dict['N_over'] == 0:
                 qstyle_widget(self.lbl_ovfl_count, "normal")
             else:
                 qstyle_widget(self.lbl_ovfl_count, "failed")
         else:
             logger.error(f"Unknown option count_ovfl_vis = '{self.count_ovfl_vis}'")
         return
 
     # --------------------------------------------------------------------------
-    def ui2dict(self):
+    def ui2dict(self) -> None:
         """
-        Update the entries in the quantization dict from the UI for `ovfl`, `quant`,
-        'WG', `WI`, `WF`, `W` when one of the widgets has been edited.
+        The subwidgets for `ovfl`, `quant`, `WI`, `WF`, `w_a_m` trigger this method
+        when modified.
+
+        Update the quantization dict `self.Q.q_dict` and the global quantization
+        dict `self.q_dict` from the UI.
 
         Emit a signal with `{'ui_local_changed': <objectName of the sender>}`.
         """
-        WG = int(safe_eval(self.ledWG.text(), self.QObj.q_dict['WG'], return_type="int",
+        WF = int(safe_eval(self.ledWF.text(), self.Q.q_dict['WF'], return_type="int",
                            sign='poszero'))
-        self.ledWG.setText(str(WG))
-        WI = int(safe_eval(self.ledWI.text(), self.QObj.q_dict['WI'], return_type="int",
+        self.ledWF.setText(str(WF))
+
+        WI = int(safe_eval(self.ledWI.text(), self.Q.q_dict['WI'] + WF + 1, return_type="int",
                            sign='poszero'))
+        if fb.fil[0]['qfrmt'] == 'qint':
+            if WI <= WF:
+                logger.warning(f"Total word length has to be larger than Fractional scaling WF = {WF}!")
+                WI = self.Q.q_dict['WI'] + WF + 1
+
         self.ledWI.setText(str(WI))
-        WF = int(safe_eval(self.ledWF.text(), self.QObj.q_dict['WF'], return_type="int",
-                           sign='poszero'))
-        self.ledWF.setText(str(WF))
 
-        # W = int(WG + WI + WF + 1)
+        # In 'qint' mode, the WI field shows the total word lenghth W. Nevertheless, the value
+        # for 'WI' is stored in the dicts.
+        if fb.fil[0]['qfrmt'] == 'qint':
+            WI = WI - WF - 1
 
         ovfl = qget_cmb_box(self.cmbOvfl)
         quant = qget_cmb_box(self.cmbQuant)
-
-        self.q_dict.update({'ovfl': ovfl, 'quant': quant, 'WG': WG, 'WI': WI, 'WF': WF})
-        self.QObj.set_qdict(self.q_dict)  # set quant. object, update derived quantities
-                                          # like W and Q and reset counter
+        w_a_m = qget_cmb_box(self.cmbW)
+        if not w_a_m in {'m', 'a', 'f'}:
+            logger.error(f"Unknown option '{w_a_m}' for cmbW combobox!")
+
+        # update quantizer dict and derived quantities like W and reset counters
+        self.Q.set_qdict(
+            {'ovfl': ovfl, 'quant': quant, 'WI': WI, 'WF': WF, 'w_a_m': w_a_m})
+        # update global filter dict
+        self.q_dict.update(self.Q.q_dict)
+        # update display of WI and WF depending on fixpoint mode
+        self.update_WI_WF()
 
         if self.sender():
-            dict_sig = {'wdg_name': self.wdg_name,
+            # logger.error(f"sender = {self.sender().objectName()}")
+#             if self.sender().objectName() == 'cmbW':
+#                self.enable_subwidgets()  # enable / disable WI and WF subwidgets
+            dict_sig = {'sender_name': self.objectName(),
                         'ui_local_changed': self.sender().objectName()}
-            # logger.warning(f"ui2dict:emit {dict_sig}")
             self.emit(dict_sig)
         else:
             logger.error("Sender has no object name!")
 
     # --------------------------------------------------------------------------
-    def dict2ui(self, q_dict=None):
+    def dict2ui(self, q_dict: dict = None) -> None:
         """
-        Use the passed dict `q_dict` to update:
+        Use the passed quantization dict `q_dict` to update:
 
-        * UI widgets `WI`, `WF` `quant` and `ovfl`
-        * the instance quantization dict `self.q_dict` (usually a reference to some
-          global quantization dict like `fb.fil[0]['fxqc']['QCB']`)
-        * the `scale` setting of the instance quantization dict if WF / WI require this
-        * the instance quantization object `self.QObj` from the instance quantization dict
+        * UI subwidgets `WI`, `WF` `quant`, `ovfl`, `cmbW`
+        * the instance quantizer object `self.Q.q_dict`
         * overflow counters need to be updated from calling instance
 
-        If `q_dict is None`, use data from the instance quantization dict `self.q_dict`
-        instead.
+        If `q_dict is None`, use data from the quantizer dict `self.Q.q_dict`
+        instead, this can be used to update the UI.
         """
-
         if q_dict is None:
-            q_dict = self.q_dict
+            q_dict = self.q_dict  # update UI from instance / global qdict
         else:
             for k in q_dict:
-                if k not in {'quant', 'quant_last', 'ovfl', 'WI', 'WF', 'qfrmt'}:
-                    logger.warning(f"Unknown quantization option '{k}'")
-
-        if 'qfrmt' in q_dict:
-            err = False
-            qfrmt = q_dict['qfrmt']
-            if 'qfrmt_last' not in q_dict:
-                q_dict['qfrmt_last'] = qfrmt
-
-            # logger.warning(f"qfrmt = {q_dict['qfrmt']} (was: {q_dict['qfrmt_last']})")
-
-            if qfrmt == 'qint':  # integer format
-                if self.q_dict['qfrmt_last'] != 'qint':  # convert to int
-                    self.q_dict.update({'WG': self.q_dict['WI'], 'WI': self.q_dict['WF'],
-                                        'WF': 0, 'scale': 1 << self.q_dict['WF']})
-            elif qfrmt == 'q31':  # Q0.31
-                self.q_dict.update({'WG': 0, 'WI': 0, 'WF': 31, 'scale': 1})
-            elif qfrmt == 'q15':  # Q0.15
-                self.q_dict.update({'WG': 0, 'WI': 0, 'WF': 15, 'scale': 1})
-
-            else:
-                if self.q_dict['qfrmt_last'] == 'qint':  # convert from int
-                    self.q_dict.update({'WF': self.q_dict['WI'], 'WI': self.q_dict['WG']})
-
-                self.q_dict.update({'scale': 1, 'WG': 0})
-
-                if qfrmt == 'qnfrac':  # normalized fractional format
-                    self.q_dict.update({'WI': 0, 'WF': self.q_dict['W'] - 1})
-                elif qfrmt in {'qfrac', 'float'}:
-                    pass
-
-                else:
-                    logger.warning(f"Unknown quantization format '{qfrmt}'")
-                    err = True
-
-            if not err:
-                self.ledWF.setEnabled(qfrmt in {'qnfrac', 'qfrac'})
-                self.ledWF.setVisible(qfrmt != 'qint')
-                self.ledWG.setVisible(qfrmt == 'qint')
-                self.ledWG.setEnabled(True)
-                self.lblPlus.setVisible(qfrmt == 'qint')
-                self.lblDot.setVisible(qfrmt != 'qint')
-                self.ledWI.setEnabled(qfrmt in {'qint', 'qfrac'})
-                self.ledWG.setText(str(self.q_dict['WG']))
-                self.ledWF.setText(str(self.q_dict['WF']))
-                self.ledWI.setText(str(self.q_dict['WI']))
+                if k not in {'quant', 'ovfl', 'WI', 'WF', 'w_a_m', 'N_over'}:
+                    logger.warning(f"Unknown quantization dict key '{k}'")
 
-        q_dict['qfrmt_last'] = qfrmt  # store current setting
+        # Update all non-numeric instance quantization dict entries from passed `q_dict`
+        # Auto-calculation of integer bits etc. needs to performed in parent subwidget!
+        if 'w_a_m' in q_dict:
+            i = qset_cmb_box(self.cmbW, q_dict['w_a_m'])
+            if i < 0:
+                logger.error(f"Unknown value q_dict['w_a_m'] = {q_dict['w_a_m']}")
 
         if 'quant' in q_dict:
             qset_cmb_box(self.cmbQuant, q_dict['quant'])
-            self.q_dict.update({'quant': qget_cmb_box(self.cmbQuant)})
+            if i < 0:
+                logger.error(f"Unknown value q_dict['quant'] = {q_dict['quant']}")
 
         if 'ovfl' in q_dict:
             qset_cmb_box(self.cmbOvfl, q_dict['ovfl'])
-            self.q_dict.update({'ovfl': qget_cmb_box(self.cmbOvfl)})
+            if i < 0:
+                logger.error(f"Unknown value q_dict['ovfl'] = {q_dict['ovfl']}")
+
+        if fb.fil[0]['qfrmt'] not in {'qfrac', 'qint'}:
+            logger.error(f"Unknown quantization format '{fb.fil[0]['qfrmt']}'")
+
+        WI = safe_eval(
+            q_dict['WI'], self.Q.q_dict['WI'], return_type="int", sign='poszero')
+
+        self.ledWI.setText(str(WI))
+
+        WF = safe_eval(
+            q_dict['WF'], self.Q.q_dict['WF'], return_type="int", sign='poszero')
+        self.ledWF.setText(str(WF))
+
+        self.Q.set_qdict(q_dict)  # update quantization object and derived parameters
+
+        self.update_WI_WF()  # set WI / WF widgets visibility depending on 'w_a_m'
+
+    # --------------------------------------------------------------------------
+    def update_WI_WF(self):
+        """
+        Update display, visibility / writability of integer and fractional part of the
+        quantization format. depending on `fb.fil[0]['fx_sim']` ...['qfrmt'] and
+        ...['w_a_m'] settings
+        """
+        self.ledWI.setVisible(fb.fil[0]['fx_sim'])
+        self.ledWF.setVisible(fb.fil[0]['fx_sim'])
 
-        if 'WG' in q_dict:
-            WG = safe_eval(
-                q_dict['WG'], self.QObj.q_dict['WG'], return_type="int", sign='poszero')
-            self.ledWG.setText(str(WG))
-            self.q_dict.update({'WG': WG})
-
-        if 'WI' in q_dict:
-            WI = safe_eval(
-                q_dict['WI'], self.QObj.q_dict['WI'], return_type="int", sign='poszero')
-            self.ledWI.setText(str(WI))
-            self.q_dict.update({'WI': WI})
-
-        if 'WF' in q_dict:
-            WF = safe_eval(
-                q_dict['WF'], self.QObj.q_dict['WF'], return_type="int", sign='poszero')
-            self.ledWF.setText(str(WF))
-            self.q_dict.update({'WF': WF})
-
-        # logger.error(f"Bef: WG = {self.q_dict['WG']}, WI = {self.q_dict['WI']}, "
-        #             f"WF = {self.q_dict['WF']}, W = {self.q_dict['W']}")
-
-        self.q_dict.update(
-            {'W': self.q_dict['WG'] + self.q_dict['WI'] + self.q_dict['WF'] + 1})
-
-        self.QObj.set_qdict(self.q_dict)  # update instance q_dict
-        # logger.error(f"Aft: WG = {self.q_dict['WG']}, WI = {self.q_dict['WI']}, "
-        #              f"WF = {self.q_dict['WF']}, W = {self.q_dict['W']}")
+        if not fb.fil[0]['fx_sim']:
+            self.lbl_sep1.setText(to_html("---", frmt='b'))
+            self.lbl_sep2.setVisible(False)
+        elif fb.fil[0]['qfrmt'] == 'qint':
+            self.lbl_sep1.setText(to_html("(", frmt='b'))
+            self.ledWF.setToolTip("Scale factor 2<sup>-WF</sup>")
+            self.ledWI.setText(str(self.Q.q_dict['WI'] + self.Q.q_dict['WF'] + 1))
+            self.ledWI.setToolTip("Total number of bits")
+            self.lbl_sep2.setVisible(True)
+
+            LSB = 1.
+            MSB = 2. ** (self.Q.q_dict['WI'] + self.Q.q_dict['WF'] - 1)
+        elif fb.fil[0]['qfrmt'] == "qfrac":
+            self.lbl_sep1.setText(to_html(".", frmt='b'))
+            self.ledWF.setToolTip("Number of fractional bits")
+            self.ledWI.setText(str(self.Q.q_dict['WI']))
+            self.ledWI.setToolTip("Number of integer bits")
+            self.lbl_sep2.setVisible(False)
 
+            LSB = 2 ** -self.Q.q_dict['WF']
+            MSB = 2. ** (self.Q.q_dict['WI'] - 1)
+        else:
+            logger.error(f"Unknown quantization format '{fb.fil[0]['qfrmt']}'!")
+
+        self.ledWF.setText(str(self.Q.q_dict['WF']))
+
+
+        if self.MSB_LSB_vis == 'off' or not fb.fil[0]['fx_sim']:
+            # Don't show any data
+            self.lbl_MSB.setVisible(False)
+            self.lbl_LSB.setVisible(False)
+        elif self.MSB_LSB_vis == 'max':
+            # Show MAX and LSB data
+            self.lbl_MSB.setVisible(True)
+            self.lbl_LSB.setVisible(True)
+            self.lbl_MSB.setText(
+                "<b><i>&nbsp;&nbsp;Max</i><sub>10</sub> = </b>"
+                f"{2. * MSB - LSB:.{params['FMT_ba']}g}")
+            self.lbl_LSB.setText(
+                f"<b><i>LSB</i><sub>10</sub> = </b>{LSB:.{params['FMT_ba']}g}")
+        elif self.MSB_LSB_vis == 'msb':
+            # Show MSB and LSB data
+            self.lbl_MSB.setVisible(True)
+            self.lbl_LSB.setVisible(True)
+            self.lbl_MSB.setText(
+                "<b><i>&nbsp;&nbsp;MSB</i><sub>10</sub> = </b>"
+                f"{MSB:.{params['FMT_ba']}g}")
+            self.lbl_LSB.setText(
+                f"<b><i>LSB</i><sub>10</sub> = </b>{LSB:.{params['FMT_ba']}g}")
+        else:
+            logger.error(f"Unknown option MSB_LSB_vis = '{self.MSB_LSB_vis}'")
+
+        self.enable_subwidgets()
 
+    # --------------------------------------------------------------------------
+    def enable_subwidgets(self):
+        """
+        Enable integer and fractional part of the quantization format, depending on
+        'w_a_m' settings.
+        """
+        self.ledWI.setEnabled(self.Q.q_dict['w_a_m'] == 'm')
+        self.ledWF.setEnabled(self.Q.q_dict['w_a_m'] == 'm')
 # ==============================================================================
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.fixpoint_widgets.fx_ui_wq` """
 
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1.png` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,16 +43,18 @@
             currently unused, created from a copy of the QACC dict
     """
     def __init__(self, p):
         self.p = p
 
         logger.info("Instantiating filter")
         # create various quantizers and initialize / reset them
-        self.Q_b = fx.Fixed(self.p['QCB'])  # transversal coeffs.
         self.Q_a = fx.Fixed(self.p['QCA'])  # recursive coeffs
+        self.Q_b = fx.Fixed(self.p['QCB'])  # transversal coeffs.
+        self.Q_mul_a = fx.Fixed(self.p['QACC'].copy())  # partial products a y
+        self.Q_mul_b = fx.Fixed(self.p['QACC'].copy())  # partial products b x
         self.Q_mul = fx.Fixed(self.p['QACC'].copy())  # partial products
         self.Q_acc = fx.Fixed(self.p['QACC'])  # accumulator
         self.Q_O = fx.Fixed(self.p['QO'])  # output
 
         self.init(p)
 
     # ---------------------------------------------------------
@@ -82,30 +84,54 @@
             When `zi_b == None`, all registers are filled with zeros.
             When `len(b) != len(a)` throw an error
 
         Returns
         -------
         None.
         """
-        self.p = p  # update parameter dictionary with coefficients etc.
+        # Do not initialize filter unless fixpoint mode is active
+        if not fb.fil[0]['fx_sim']:
+            return
 
-        q_mul = p['QACC'].copy()
+        self.p = p  # update parameter dictionary with coefficients etc.
 
         # update the quantizers
-        self.Q_b.set_qdict(self.p['QCB'])  # transversal coeffs.
-        self.Q_a.set_qdict(self.p['QCA'])  # recursive coeffs
-        self.Q_mul.set_qdict(q_mul)  # partial products
+        self.Q_a.set_qdict(self.p['QCA'])  # recursive coeffs (a)
+        self.Q_b.set_qdict(self.p['QCB'])  # transversal b coeffs (b)
         self.Q_acc.set_qdict(self.p['QACC'])  # accumulator
         self.Q_O.set_qdict(self.p['QO'])  # output
 
+        # Quantizer dict for partial products yq * aq
+        DW_a = int(np.ceil(np.log2(len(self.p['QCA']))))  # word growth
+        # word format for sum of partial products a_i * y_i
+        self.Q_mul_a.set_qdict(
+            {'WI': self.p['QO']['WI'] + self.p['QCA']['WI'] + DW_a,
+             'WF': self.p['QO']['WF'] + self.p['QCA']['WF']})
+
+        # Quantizer dict for partial products xq * bq
+        DW_b = int(np.ceil(np.log2(len(self.p['QCB']))))  # word growth
+        # word format for sum of partial products b_i * x_i
+        self.Q_mul_b.set_qdict(
+            {'WI': self.p['QI']['WI'] + self.p['QCB']['WI'] + DW_b,
+             'WF': self.p['QI']['WF'] + self.p['QCB']['WF']})
+
         # Quantize coefficients and store them in local attributes
         # This also resets the overflow counters.
         self.a_q = quant_coeffs(fb.fil[0]['ba'][1], self.Q_a, recursive=True)
         self.b_q = quant_coeffs(fb.fil[0]['ba'][0], self.Q_b)
 
+        if np.iscomplexobj(self.a_q):
+            self.a_q = self.a_q.real
+            logger.warning(
+                "Complex fixpoint coefficients a_q are not supported, casting to real.")
+        if np.iscomplexobj(self.b_q):
+            self.b_q = self.b_q.real
+            logger.warning(
+                "Complex fixpoint coefficients b_q are not supported, casting to real.")
+
         self.L = max(len(self.b_q), len(self.a_q))  # filter length = number of taps
 
         self.reset() # reset overflow counters (except coeffs) and registers
 
         # Initialize filter memory with passed values zi_b, zi_a and fill up with zeros
         # or truncate to filter length L
         if zi_b is not None:
@@ -125,15 +151,16 @@
 
     # ---------------------------------------------------------
     def reset(self):
         """
         Reset registers and overflow counters of quantizers
         (except for coefficient quant.)
         """
-        self.Q_mul.resetN()
+        self.Q_mul_a.resetN()
+        self.Q_mul_b.resetN()
         self.Q_acc.resetN()
         self.Q_O.resetN()
         self.N_over_filt = 0
         self.zi_a = np.zeros(self.L - 1)
         self.zi_b = np.zeros(self.L - 1)
 
     # ---------------------------------------------------------
@@ -142,36 +169,60 @@
         """
         Calculate quantized IIR filter (direct form 1) response via difference equation
         with quantized coefficient values `self.a_q` and `self.b_q` and quantized
         arithmetics.
 
         Registers can be initialized by passing `zi_a` and `zi_b`.
 
+        Calculate response by:
+        - append new stimuli `x` to transversal register state `self.zi_b`
+
+        - slide a window with length `len(b)` over `self.zi_b`, starting at position `k`
+          and multiply it with the coefficients `b`, yielding the partial products x*b
+          TODO: Doing this for the last len(x) terms should be enough
+        - do the same `self.zi_a` and coefficients `a`, yielding partial products y*a
+        - quantize the partial products x*b and y*a, yielding xb_q and x_aq
+        - accumulate the quantized partial products and quantize result as `y_q[k]`
+        - insert last output `y_q[k]` into the recursive register `self.zi_a`
+
+          TODO: complex inputs?
+
         Parameters
         ----------
         x : array of float or float or None
             input value(s) scaled and quantized according to the setting of `p['QI']`
             - When x is a scalar, calculate impulse response with the
                 amplitude defined by the scalar.
             - When `x == None`, calculate impulse response with amplitude = 1.
 
         zi_b : array-like
              initial conditions for transversal registers; when `zi_b == None`,
-             the register contents from the last run are used.
+             register contents from last run are used.
 
         zi_a : array-like
              initial conditions for recursive registers; when `zi_a == None`,
-             the register contents from the last run are used.
+             register contents from last run are used.
 
         Returns
         -------
         yq : ndarray
             The quantized input value(s) as an ndarray of np.float64
             and the same shape as `x` resp. `b` or `a`(impulse response).
+
+        zi_b : ndarray
+            The content of the L-1 transversal state registers with the
+            last L-1 input values
+
+        zi_a : ndarray
+            The content of the L-1 recursive state registers with the
+            last L-1 output values
         """
+        qfrmt = fb.fil[0]['qfrmt']
+
+        # if initial conditions `zi_a` or `zi_b` have been given, use them:
         if zi_b is not None:
             if len(zi_b) == self.L - 1:   # use zi_b as it is
                 self.zi_b = zi_b
             elif len(zi_b) < self.L - 1:  # append zeros
                 self.zi_b = np.concatenate((zi_b, np.zeros(self.L - 1 - len(zi_b))))
             else:                         # truncate zi_b
                 self.zi_b = zi_b[:self.L - 1]
@@ -184,72 +235,76 @@
                 self.zi_a = np.concatenate((zi_a, np.zeros(self.L - 1 - len(zi_a))))
             else:                         # truncate zi_b
                 self.zi_a = zi_a[:self.L - 1]
                 logger.warning("len(zi_a) > len(coeff) - 1, zi_a was truncated")
 
         # initialize quantized partial products and output arrays
         y_q = xb_q = np.zeros(len(x))
-        xa_q = np.zeros(self.L - 1)
-
-        # Calculate response by:
-        # - feed last output `y_q[k]`` into the recursive register `self.zi_a`
-        # - append new stimuli `x` to transversal register state `self.zi_b`
-        # - slide a window with length `len(b)` over `self.zi`, starting at position `k`
-        #   and multiply it with the coefficients `b`, yielding the partial products x*b
-        #   TODO: Doing this for the last len(x) terms should be enough
-        # - quantize the partial products x*b and x*a, yielding xb_q and x_aq
-        # - accumulate the quantized partial products and quantize result, yielding y_q[k]
+        ya_q = np.zeros(self.L - 1)
 
         self.zi_b = np.concatenate((self.zi_b, x))
 
-        for k in range(len(x)):
-            # partial products xa_q and xb_q at time k, quantized with Q_mul:
-            xb_q = self.Q_mul.fixp(self.zi_b[k:k + len(self.b_q)] * self.b_q)
-            # append a zero to xa_q to equalize length of xb_q and xa_q
-            xa_q = np.append(self.Q_mul.fixp(self.zi_a * self.a_q[1:]), 0)
-
-            # accumulate partial products x_bq and x_aq and quantize them (Q_acc)
-            # quantize individual accumulation steps - needed?!
-            # y_q[k] = 0.0
-            # for i in range(len(self.b_q)):
-            #     y_q[k] += self.Q_acc.fixp(xb_q[i] - xa_q[i])
-
-            y_q[k] = self.Q_acc.fixp(np.sum(xb_q) - np.sum(xa_q))
-            self.zi_a[1:] = self.zi_a[:-1]  # shift right by one
+        # logger.warning(f"a_q = \n{self.a_q}\nb_q = \n{self.b_q}\nx= {x}\n")
 
-            # and insert last output value quantized to output format
-            self.zi_a[0] = self.Q_O.fixp(y_q[k])
-
-            # logger.warning(f"zi_a = {self.zi_a}\n"
-            #                f"zi_b = {self.zi_b}")
+        for k in range(len(x)):
+            # calculate partial products xb_q and ya_q at time k and quantize them
+            # with Q_mul_b resp. Q_mul_a:
+            xb_q = self.Q_mul_b.fixp(self.zi_b[k:k + len(self.b_q)] * self.b_q,
+                                     in_frmt=qfrmt, out_frmt=qfrmt)
+
+            # append a zero to ya_q to equalize length of xb_q and ya_q
+            ya_q = np.append(self.Q_mul_a.fixp(self.zi_a * self.a_q[1:],
+                                               in_frmt=qfrmt, out_frmt=qfrmt),
+                                               0)
+
+            # - shift right recursive state (output) register
+            # - accumulate partial products `xb_q` and `ya_q`, requantize the results
+            #   to accumulator word formats `Q_acc` and calculate the difference
+            # - requantize the result to output word format `Q_O`
+            # - insert last accumulator value quantized to output format into recursive
+            #   (output) state register
+            self.zi_a[1:] = self.zi_a[:-1]
+            y_q[k] = self.Q_O.requant(
+                (self.Q_acc.requant(np.sum(xb_q), self.Q_mul_b)
+                - self.Q_acc.requant(np.sum(ya_q), self.Q_mul_a)),
+                                self.Q_acc)
+            self.zi_a[0] = y_q[k]
 
         self.zi_b = self.zi_b[-(self.L-1):]  # store last L-1 inputs (i.e. the L-1 registers)
 
         # Overflows in Q_mul are added to overflows in Q_Acc, then Q_mul is reset
-        if self.Q_acc.q_dict['N_over'] > 0 or self.Q_mul.q_dict['N_over'] > 0:
-            logger.warning(f"Overflows: N_Acc = {self.Q_acc.q_dict['N_over']}, "
-                           f"N_Mul = {self.Q_mul.q_dict['N_over']}")
-        self.Q_acc.q_dict['N_over'] += self.Q_mul.q_dict['N_over']
-        self.Q_mul.resetN()
+        if self.Q_acc.N_over > 0 or self.Q_mul_a.N_over > 0 or self.Q_mul_b.N_over > 0:
+            logger.warning(f"Overflows: N_Acc = {self.Q_acc.N_over}, "
+                           f"N_Mul_a = {self.Q_mul_a.N_over}, "
+                           f"N_Mul_b = {self.Q_mul_b.N_over}.")
+        self.Q_acc.N_over += self.Q_mul_a.N_over + self.Q_mul_b.N_over
+        self.Q_mul_a.resetN()
+        self.Q_mul_b.resetN()
 
-        return self.Q_O.fixp(y_q[:len(x)]), self.zi_b, self.zi_a
+        return y_q[:len(x)], self.zi_b, self.zi_a
 
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """
     Run widget standalone with
     `python -m pyfda.fixpoint_widgets.iir_df1.iir_df1_pyfixp`
     """
-
-    p = {'b': [-0.2, 0.2, 0], 'QACC': {'Q': '3.6', 'ovfl': 'wrap', 'quant': 'round'},
-         'a': [1, 0, -0.81],
-         'QI': {'Q': '1.3', 'ovfl': 'sat', 'quant': 'round'},
-         'QO': {'Q': '3.3', 'ovfl': 'sat', 'quant': 'round'}
+    p = {'QCB': {'WI': 0, 'WF': 5, 'w_a_m': 'a',
+                'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+        'QCA': {'WI': 1, 'WF': 5, 'w_a_m': 'a',
+                'ovfl': 'wrap', 'quant': 'floor', 'N_over': 0},
+         'QACC': {'WI': 4, 'WF': 3, 'ovfl': 'wrap', 'quant': 'round'},
+         'QI': {'WI': 2, 'WF': 3, 'ovfl': 'sat', 'quant': 'round'},
+         'QO': {'WI': 5, 'WF': 3, 'ovfl': 'wrap', 'quant': 'round'}
          }
+
     dut = IIR_DF1_pyfixp(p)
+    print("Filter fixpoint response and state variables for input =")
+    print("x = (1, 0, 0, 0, 0)")
     x = np.zeros(5)
     x[0] = 1
     y = dut.fxfilter(x=x)
     print(y)
+    print("\nfollowed by x = np.zeros(5):")
     y = dut.fxfilter(x=np.zeros(5))
     print(y)
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,75 +45,84 @@
         self.title = ("<b>Direct-Form 1 (DF1) IIR Filter</b>")
         self.description = ("Topology with one accumulator, more robust against "
                             "overflows than DF2. Only suitable for low-order filters.")
         self.img_name = "iir_df1.png"
 
         self.cmb_wq_accu_items = [
             "<span>Set Accumulator word format</span>",
-            ("man", "M", "<span><b>Manual</b> entry</span>"),
-            ("auto", "A",
-             "<span><b>Automatic</b> estimation from coefficients and input word "
-             "formats (worst case estimation).</span>")
+            ("m", "M", "<span><b>Manual</b> entry</span>"),
+            ("a", "A",
+             "<span><b>Automatic</b> worst case estimation from coefficients "
+             "and input word formats.</span>")
             ]
-        self.cmb_wq_accu_init = 'man'
 
         self.cmb_wq_coeffs_a_items = [
             "<span>Number of integer bits</span>",
-            ("man", "M", "<span><b>Manual</b> entry</span>"),
-            ("auto", "A",
+            ("m", "M", "<span><b>Manual</b> entry</span>"),
+            ("a", "A",
+             "<span><b>Automatic</b> calculation from largest coefficient.</span>")
+            ]
+
+        self.cmb_wq_coeffs_b_items = [
+            "<span>Number of integer bits</span>",
+            ("m", "M", "<span><b>Manual</b> entry</span>"),
+            ("a", "A",
              "<span><b>Automatic</b> calculation from largest coefficient.</span>")
             ]
-        self.cmb_wq_coeffs_a_init = 'auto'
 
         self._construct_UI()
         # Construct an instance of the fixpoint filter using the settings from
-        # the 'fxqc' quantizer dict:
-        self.fx_filt = IIR_DF1_pyfixp(fb.fil[0]['fxqc'])
-        self.update_disp()  # initial setting of overflow counter display
+        # the 'fxq' quantizer dict:
+        self.fx_filt = IIR_DF1_pyfixp(fb.fil[0]['fxq'])
+        self.update_ovfl_cnt_all()  # initialize all overflow counters / display
 
     # --------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the UI with widgets for coefficient format and input and
         output quantization
         """
         # widget for quantization of coefficients 'b'
-        if 'QCB' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc'].update({'QCB': {}})  # no coefficient settings in dict yet
-            logger.warning("Empty dict / missing key 'fxqc['QCB]'!")
+        if 'QCB' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq'].update({'QCB': {}})  # no coefficient settings in dict yet
+            logger.warning("Empty dict / missing key 'fb.fil{0]['fxq']['QCB']'!")
         self.wdg_wq_coeffs_b = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QCB'], wdg_name='wq_coeffs_b',
+            fb.fil[0]['fxq']['QCB'], objectName='fx_ui_wq_iir_df1_coeffs_b',
             label='<b>Coeff. Quantization <i>b<sub>I.F&nbsp;</sub></i>:</b>',
-            MSB_LSB_vis='msb')
+            MSB_LSB_vis='max', cmb_w_vis='on', cmb_w_items=self.cmb_wq_coeffs_b_items)
         layV_wq_coeffs_b = QVBoxLayout()
         layV_wq_coeffs_b.addWidget(self.wdg_wq_coeffs_b)
 
         # widget for quantization of coefficients 'a'
-        if 'QCA' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc'].update({'QCA': {}})  # no coefficient settings in dict yet
-            logger.warning("Empty dict / missing key 'fxqc['QCA]'!")
+        if 'QCA' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq'].update({'QCA': {}})  # no coefficient settings in dict yet
+            logger.warning("Empty dict / missing key 'fb.fil{0]['fxq']['QCA']'!")
         self.wdg_wq_coeffs_a = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QCA'], wdg_name='wq_coeffs_a',
+            fb.fil[0]['fxq']['QCA'], objectName='fx_ui_wq_iir_df1_coeffs_a',
             label='<b>Coeff. Quantization <i>a<sub>I.F&nbsp;</sub></i>:</b>',
-            MSB_LSB_vis='max', cmb_w_vis='on', cmb_w_items=self.cmb_wq_coeffs_a_items,
-            cmb_w_init=self.cmb_wq_coeffs_a_init)
+            MSB_LSB_vis='max', cmb_w_vis='on', cmb_w_items=self.cmb_wq_coeffs_a_items)
         layV_wq_coeffs_a = QVBoxLayout()
         layV_wq_coeffs_a.addWidget(self.wdg_wq_coeffs_a)
-        self.update_coeffs_settings()
+        # calculate wordlength needed for coefficients if required
+        if qget_cmb_box(self.wdg_wq_coeffs_a.cmbW) == 'a':
+            self.calc_wi_coeffs_a()
+        if qget_cmb_box(self.wdg_wq_coeffs_b.cmbW) == 'a':
+            self.calc_wi_coeffs_b()
 
         # widget for accumulator quantization
-        if 'QACC' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc']['QACC'] = {}
-        set_dict_defaults(fb.fil[0]['fxqc']['QACC'],
-                          {'WI': 0, 'WF': 31, 'W': 32, 'ovfl': 'wrap', 'quant': 'floor'})
+        if 'QACC' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq']['QACC'] = {}  # initialize dict settings
+        set_dict_defaults(
+            fb.fil[0]['fxq']['QACC'],
+            {'WI': 0, 'WF': 31, 'ovfl': 'wrap', 'quant': 'floor', 'w_a_m': 'a',
+             'N_over': 0})
         self.wdg_wq_accu = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QACC'], wdg_name='wq_accu',
+            fb.fil[0]['fxq']['QACC'], objectName='fx_ui_wq_iir_df1_accu',
             label='<b>Accu Quantizer <i>Q<sub>A&nbsp;</sub></i>:</b>',
-            cmb_w_vis='on', cmb_w_items=self.cmb_wq_accu_items,
-            cmb_w_init=self.cmb_wq_accu_init)
+            cmb_w_vis='on', cmb_w_items=self.cmb_wq_accu_items)
         layV_wq_accu = QVBoxLayout()
         layV_wq_accu.addWidget(self.wdg_wq_accu)
 
         # ----------------------------------------------------------------------
         layVWdg = QVBoxLayout()
         # margins are created in input_fixpoint_specs widget
         layVWdg.setContentsMargins(0, 0, 0, 0)
@@ -135,159 +144,208 @@
 
     # --------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         - For locally generated signals (key = 'ui_local_changed'), emit
           `{'fx_sim': 'specs_changed'}` with local id.
         - For external changes, i.e. `{'fx_sim': 'specs_changed'}` or
-          `{'data_changed': xxx}` update the UI via `self.dict_ui`.
+          `{'data_changed': xxx}` update the UI via `self.dict2ui`.
 
         Ignore all other signals
 
         Note: If coefficient / accu quantization settings have been changed in the UI,
-        the referenced dicts `fb.fil[0]['fxqc']['QCB']`, `['QCA']` and `...['QACC']`
+        the referenced dicts `fb.fil[0]['fxq']['QCB']`, `['QCA']` and `...['QACC']`
         have already been updated by the corresponding subwidgets `FX_UI_WQ`
         """
         logger.debug("sig_rx:\n{0}".format(pprint_log(dict_sig)))
         if dict_sig['id'] == id(self):
             logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'ui_local_changed' in dict_sig:
             # signal generated locally by modifying coefficient / accu format
             ui_changed = dict_sig['ui_local_changed']  # name of changed ui element
-            if not dict_sig['wdg_name'] in {'wq_coeffs_b', 'wq_coeffs_a', 'wq_accu'}:
-                logger.error(f"Unknown widget name '{dict_sig['wdg_name']}' "
+            if not dict_sig['sender_name']\
+                    in {'fx_ui_wq_iir_df1_coeffs_b', 'fx_ui_wq_iir_df1_coeffs_a',
+                        'fx_ui_wq_iir_df1_accu'}:
+                logger.error(f"Unknown sender name '{dict_sig['sender_name']}' "
                              f"in '{__name__}' !")
                 return
 
-            elif dict_sig['wdg_name'] == 'wq_accu':  # accu format updated
+            # changes in accu widget
+            elif dict_sig['sender_name'] == 'fx_ui_wq_iir_df1_accu':  # accu format updated
                 if ui_changed in {'cmbW', 'WF', 'WI'}:
                     cmbW = qget_cmb_box(self.wdg_wq_accu.cmbW)
-                    if cmbW == 'man':
+                    if cmbW == 'm':
                         if ui_changed == 'cmbW':
                             # returning to manual setting, don't do anything
                             return
                         else:
                             pass  # WI or WF have been edited, emit 'specs_changed'
-                    elif cmbW == 'auto':
+                    elif cmbW == 'a':
                         # when switching to auto settings, run automatic accu calculation
                         # this also reverses manual edits of WI or WF wordlengths
                         # manual entry of word lengths cannot be disabled easily due to
                         # additional logic in the wdg_wq_accu widget (class FX_UI_WQ)
                         self.update_accu_settings()
                     else:
                         logger.error(f"Unknown accu combobox setting '{cmbW}'!")
                         return
 
-            elif dict_sig['wdg_name'] in {'wq_coeffs_a', 'wq_coeffs_b'}:  # coeffs updated
+            # changes in coeffs 'a' widget
+            elif dict_sig['sender_name'] == 'fx_ui_wq_iir_df1_coeffs_a':
                 if ui_changed in {'cmbW', 'WF', 'WI'}:
                     cmbW = qget_cmb_box(self.wdg_wq_coeffs_a.cmbW)
-                    if cmbW == 'man':
+                    if cmbW == 'm':
                         if ui_changed == 'cmbW':
                             # returning to manual setting, don't do anything
                             return
                         else:
                             pass  # WI or WF have been edited, emit 'specs_changed'
 
-                    elif cmbW == 'auto':
+                    elif cmbW == 'a':
                         # when switching to auto settings, run automatic calculation
                         # of required integer bits for coeffs a
                         # this also reverses manual edits of WI or WF wordlengths
-                        # manual entry of word lengths cannot be disabled easily due to
-                        # additional logic in the wdg_wq_accu widget (class FX_UI_WQ)
-                        self.update_coeffs_settings()
+                        self.calc_wi_coeffs_a()
                     else:
                         logger.error(f"Unknown coeff. combobox setting '{cmbW}'!")
                         return
 
                     # in case coefficient length has been changed, update accu as well
-                    if qget_cmb_box(self.wdg_wq_accu.cmbW) == 'auto':
+                    if qget_cmb_box(self.wdg_wq_accu.cmbW) == 'a':
                         self.update_accu_settings()
 
+            # changes in coeffs 'b' widget
+            elif dict_sig['sender_name'] == 'fx_ui_wq_iir_df1_coeffs_b':
+                if ui_changed in {'cmbW', 'WF', 'WI'}:
+                    cmbW = qget_cmb_box(self.wdg_wq_coeffs_b.cmbW)
+                    if cmbW == 'm':
+                        if ui_changed == 'cmbW':
+                            # returning to manual setting, don't do anything
+                            return
+                        else:
+                            pass  # WI or WF have been edited, emit 'specs_changed'
+
+                    elif cmbW == 'a':
+                        # when switching to auto settings, run automatic calculation
+                        # of required integer bits for coeffs b
+                        # this also reverses manual edits of WI or WF wordlengths
+                        self.calc_wi_coeffs_b()
+                    else:
+                        logger.error(f"Unknown coeff. combobox setting '{cmbW}'!")
+                        return
+
+                    # in case coefficient length has been changed, update accu as well
+                    if qget_cmb_box(self.wdg_wq_accu.cmbW) == 'a':
+                        self.update_accu_settings()
+
+
             # emit signal, replace UI id with id of *this* widget
             self.emit({'fx_sim': 'specs_changed', 'id': id(self)})
 
         # quantization dictionary has been updated outside the widget, update UI
         elif 'data_changed' in dict_sig or\
                 'fx_sim' in dict_sig and dict_sig['fx_sim'] == 'specs_changed':
             self.dict2ui()
 
     # --------------------------------------------------------------------------
-    def update_coeffs_settings(self):
+    def calc_wi_coeffs_a(self):
         """
-        Calculate required number of integer bits for the largest coefficient
+        Calculate required number of integer bits for the largest 'a' coefficient
 
         The new value is written to the fixpoint coefficient dict
-        `fb.fil[0]['fxqc']['QCA']` and the UI is updated.
+        `fb.fil[0]['fxq']['QCA']` and the UI is updated.
         """
         WI_A = int(np.ceil(np.log2((np.abs(np.max(fb.fil[0]['ba'][1]))))))
-        fb.fil[0]['fxqc']['QCA']['WI'] = WI_A
-        # update quantization settings ('W', 'Q', ...) and UI
-        self.wdg_wq_coeffs_a.QObj.set_qdict({})  # update `self.wdg_wq_coeffs_a.q_dict`
-        self.wdg_wq_coeffs_a.dict2ui()
+        fb.fil[0]['fxq']['QCA']['WI'] = WI_A
+        # update quantizer settings and UI
+        self.wdg_wq_coeffs_a.dict2ui(fb.fil[0]['fxq']['QCA'])
+
+    # --------------------------------------------------------------------------
+    def calc_wi_coeffs_b(self):
+        """
+        Calculate required number of integer bits for the largest 'b' coefficient
+
+        The new value is written to the fixpoint coefficient dict
+        `fb.fil[0]['fxq']['QCB']` and the UI is updated.
+        """
+        WI_B = int(np.ceil(np.log2((np.abs(np.max(fb.fil[0]['ba'][0]))))))
+        fb.fil[0]['fxq']['QCB']['WI'] = max(WI_B, 0)
+        # update quantizer settings and UI
+        self.wdg_wq_coeffs_b.dict2ui(fb.fil[0]['fxq']['QCB'])
 
     # --------------------------------------------------------------------------
     def update_accu_settings(self):
         """
         Calculate required number of fractional bits for the accumulator from
         the sum of coefficient and input resp. output fractional bits, using
         the maximum of both.
 
         Calculate number of extra integer bits for the accumulator (guard bits)
         for `cmbW == 'auto'` from the sum of the integer part of recursive
         coefficients and output signal resp. the integer part of non-recursive
         coefficients and input signal, depending on which one is larger.
 
         The new values are written to the fixpoint coefficient dict
-        `fb.fil[0]['fxqc']['QACC']`.
+        `fb.fil[0]['fxq']['QACC']` and the UI is updated.
         """
         # except BaseException as e: # Exception as e:
         #     logger.error("An error occured:", exc_info=True)
         #     return
 
-        if qget_cmb_box(self.wdg_wq_accu.cmbW) == "auto":
-            fb.fil[0]['fxqc']['QACC']['WF'] = max(
-                fb.fil[0]['fxqc']['QI']['WF'] + fb.fil[0]['fxqc']['QCB']['WF'],
-                fb.fil[0]['fxqc']['QO']['WF'] + fb.fil[0]['fxqc']['QCA']['WF'])
-
-            fb.fil[0]['fxqc']['QACC']['WI'] = max(
-                fb.fil[0]['fxqc']['QI']['WI'] + fb.fil[0]['fxqc']['QCB']['WI'],
-                fb.fil[0]['fxqc']['QO']['WI'] + fb.fil[0]['fxqc']['QCA']['WI'])
-
-        # update quantization settings like 'Q', 'W' etc. and UI
-        self.wdg_wq_accu.QObj.set_qdict({})  # update `self.wdg_wq_accu.q_dict`
-        self.wdg_wq_accu.dict2ui()
+        if qget_cmb_box(self.wdg_wq_accu.cmbW) == 'a':
+            fb.fil[0]['fxq']['QACC']['WF'] = max(
+                fb.fil[0]['fxq']['QI']['WF'] + fb.fil[0]['fxq']['QCB']['WF'],
+                fb.fil[0]['fxq']['QO']['WF'] + fb.fil[0]['fxq']['QCA']['WF'])
+
+            fb.fil[0]['fxq']['QACC']['WI'] = max(
+                fb.fil[0]['fxq']['QI']['WI'] + fb.fil[0]['fxq']['QCB']['WI'],
+                fb.fil[0]['fxq']['QO']['WI'] + fb.fil[0]['fxq']['QCA']['WI'])
+
+        # update UI and Q.q_dict (quantization settings) from filter dict
+        self.wdg_wq_accu.dict2ui(fb.fil[0]['fxq']['QACC'])
 
     # --------------------------------------------------------------------------
     def dict2ui(self):
         """
         Update all parts of the UI that need to be updated when specs or data have been
         changed outside this class, e.g. coefficients and coefficient quantization
         settings. This also provides the initial setting for the widgets when
         the filter has been changed.
 
         This is called from one level above by
         :class:`pyfda.input_widgets.input_fixpoint_specs.Input_Fixpoint_Specs`.
         """
-        self.wdg_wq_coeffs_b.dict2ui()  # update coefficient quantization
-        self.wdg_wq_coeffs_a.dict2ui()  # settings
-        self.wdg_wq_accu.dict2ui()
+        fxq_dict = fb.fil[0]['fxq']
+
+        # if 'QACC' not in fxq_dict:
+        #     fxq_dict.update({'QACC': {}})  # no accumulator settings in dict yet
+        #     logger.warning("'QACC' key missing in filter dict")
+
+        # if 'QCB' not in fxq_dict:
+        #     fxq_dict.update({'QCB': {}})  # no coefficient settings in dict yet
+        #     logger.warning("'QCB' key missing in filter dict")
+
+        self.wdg_wq_coeffs_b.dict2ui(fxq_dict['QCB'])  # update coefficient quantization
+        self.wdg_wq_coeffs_a.dict2ui(fxq_dict['QCA'])  # settings
+        # TODO: In the past, only 'QCB' was passed directly - why?!
+        self.update_accu_settings()   # update accumulator settings and UI
 
     # --------------------------------------------------------------------------
-    def update_disp(self):
+    def update_ovfl_cnt_all(self):
         """
-        Update the overflow counters etc. of the UI after simulation has finished.
+        Update the overflow counters of the UI after simulation has finished.
 
         This is usually called from one level above by
         :class:`pyfda.input_widgets.input_fixpoint_specs.Input_Fixpoint_Specs`.
         """
-        self.wdg_wq_coeffs_b.update_disp()
-        self.wdg_wq_coeffs_a.update_disp()
-        self.wdg_wq_accu.update_disp()
+        self.wdg_wq_coeffs_b.update_ovfl_cnt()
+        self.wdg_wq_coeffs_a.update_ovfl_cnt()
+        self.wdg_wq_accu.update_ovfl_cnt()
 
     # --------------------------------------------------------------------------
     def fxfilter(self, stimulus):
         """
         Provide  wrapper around fixpoint filter simulation method:
         * takes stimulus (iterable or float or None) as parameter
         * returns fixpoint response (ndarray of float)
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/no_fx_filter.png` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/no_fx_filter.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/delay/delay.png` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/delay/delay.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/delay/fx_delay.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/delay/fx_delay.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,18 @@
         return response
 ###############################################################################
 
 ###############################################################################
 # A delay with quantization and parametrizable length
 class Delay(Module):
     def __init__(self):
-        p = fb.fil[0]['fxqc']
+        p = fb.fil[0]['fxq']
         # ------------- Define I/Os -------------------------------------------
-        self.WI = p['QI']['W']
-        self.WO = p['QO']['W']
+        self.WI = p['QI']['WI'] + p['QI']['WF'] + 1
+        self.WO = p['QO']['WI'] + p['QO']['WF'] + 1
         N = len(p['b']) - 1 # number of coefficients = Order + 1
         # ------------- Define I/Os -------------------------------------------
         self.i = Signal((self.WI, True)) # input signal
         self.o = Signal((self.WO, True)) # output signal
 
         src = self.i
         for c in range(N):
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,52 +86,56 @@
             When `len(zi) != len(b)`, truncate or fill up with zeros.
             When `zi == None`, all registers are filled with zeros.
 
         Returns
         -------
         None.
         """
-        self.p = p  # fb.fil[0]['fxqc']  # parameter dictionary with coefficients etc.
+        self.p = p  # fb.fil[0]['fxq']  # parameter dictionary with coefficients etc.
         # ------------- Define I/Os --------------------------------------
-        self.i = Signal(signed(self.p['QI']['W']))  # input signal
-        self.o = Signal(signed(self.p['QO']['W']))  # output signal
+        self.WI = p['QI']['WI'] + p['QI']['WF'] + 1  # total input word length
+        self.WO = p['QO']['WI'] + p['QO']['WF'] + 1  # total output word length
+        self.i = Signal(signed(self.WI))  # input signal
+        self.o = Signal(signed(self.WO))  # output signal
 
     # ---------------------------------------------------------
     def elaborate(self, platform) -> Module:
         """
         `platform` normally specifies FPGA platform, not needed here.
         """
         m = Module()  # instantiate a module
         ###
         muls = [0] * len(self.p['b'])
+        WACC = p['QACC']['WI'] + p['QACC']['WF'] + 1  # total accu word length
 
         DW = int(np.ceil(np.log2(len(self.p['b']))))  # word growth
         # word format for sum of partial products b_i * x_i
         QP = {'WI': self.p['QI']['WI'] + self.p['QCB']['WI'] + DW,
               'WF': self.p['QI']['WF'] + self.p['QCB']['WF']}
-        QP.update({'W': QP['WI'] + QP['WF'] + 1})
+        WP = QP['WI'] + QP['WF'] + 1
+        # QP.update({'W': QP['WI'] + QP['WF'] + 1})
 
         src = self.i  # first register is connected to input signal
 
         i = 0
         for b in self.p['b']:
-            sreg = Signal(signed(self.p['QI']['W']))  # create chain of registers
-            m.d.sync += sreg.eq(src)            # with input word length
+            sreg = Signal(signed(self.WI))  # create chain of registers
+            m.d.sync += sreg.eq(src)        # with input word length
             src = sreg
             # TODO: keep old data sreg to allow frame based processing (requiring reset)
             muls[i] = int(b)*sreg
             i += 1
 
         # logger.debug(f"b = {pprint_log(self.p['b'])}\nW(b) = {self.p['QCB']['W']}")
 
-        sum_full = Signal(signed(QP['W']))  # sum of all multiplication products with
+        sum_full = Signal(signed(WP))  # sum of all multiplication products with
         m.d.sync += sum_full.eq(reduce(add, muls))  # full product wordlength
 
         # rescale from full product wordlength to accumulator format
-        sum_accu = Signal(signed(self.p['QA']['W']))
+        sum_accu = Signal(signed(WACC))
         m.d.comb += sum_accu.eq(requant(m, sum_full, QP, self.p['QA']))
 
         # rescale from accumulator format to output width
         m.d.comb += self.o.eq(requant(m, sum_accu, self.p['QA'], self.p['QO']))
 
         return m   # return result as list of integers
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen_ui.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,51 +48,52 @@
 
         self.title = ("<b>Direct-Form (DF) FIR Filter</b><br />"
                       "Standard FIR topology.")
         self.img_name = "fir_df.png"
 
         self._construct_UI()
         # Construct an instance of the fixpoint filter using the settings from
-        # the 'fxqc' quantizer dict
+        # the 'fxq' quantizer dict
 # ------------------------------------------------------------------------------
 
     def _construct_UI(self):
         """
         Intitialize the UI with widgets for coefficient format and input and
         output quantization
         """
-        if 'QA' not in fb.fil[0]['fxqc']:
-            fb.fil[0]['fxqc']['QA'] = {}
-        set_dict_defaults(fb.fil[0]['fxqc']['QA'],
-                          {'WI': 0, 'WF': 30, 'W': 32, 'ovfl': 'wrap', 'quant': 'floor'})
+        if 'QA' not in fb.fil[0]['fxq']:
+            fb.fil[0]['fxq']['QA'] = {}
+        set_dict_defaults(fb.fil[0]['fxq']['QA'],
+                          {'WI': 0, 'WF': 30, 'ovfl': 'wrap', 'quant': 'floor',
+                           'w_a_m': 'a', 'N_over': 0, 'wdg_name': 'unknown'})
 
-        self.wdg_w_coeffs = UI_W(self, fb.fil[0]['fxqc']['QCB'], wdg_name='w_coeff',
+        self.wdg_w_coeffs = UI_W(self, fb.fil[0]['fxq']['QCB'], wdg_name='w_coeff',
                                  label='Coeff. Format <i>B<sub>I.F&nbsp;</sub></i>:',
                                  tip_WI='Number of integer bits - edit in "b,a" tab',
                                  tip_WF='Number of fractional bits - edit in "b,a" tab',
-                                 WI=fb.fil[0]['fxqc']['QCB']['WI'],
-                                 WF=fb.fil[0]['fxqc']['QCB']['WF'])
+                                 WI=fb.fil[0]['fxq']['QCB']['WI'],
+                                 WF=fb.fil[0]['fxq']['QCB']['WF'])
 
 
-#        self.wdg_q_coeffs = UI_Q(self, fb.fil[0]['fxqc']['QCB'],
-#                                        cur_ov=fb.fil[0]['fxqc']['QCB']['ovfl'],
-#                                        cur_q=fb.fil[0]['fxqc']['QCB']['quant'])
+#        self.wdg_q_coeffs = UI_Q(self, fb.fil[0]['fxq']['QCB'],
+#                                        cur_ov=fb.fil[0]['fxq']['QCB']['ovfl'],
+#                                        cur_q=fb.fil[0]['fxq']['QCB']['quant'])
 #        self.wdg_q_coeffs.sig_tx.connect(self.update_q_coeff)
 
-        self.wdg_w_accu = UI_W(self, fb.fil[0]['fxqc']['QA'],
+        self.wdg_w_accu = UI_W(self, fb.fil[0]['fxq']['QA'],
                                label='', wdg_name='w_accu',
                                fractional=True, combo_visible=True)
 
-        self.wdg_q_accu = UI_Q(self, fb.fil[0]['fxqc']['QA'], wdg_name='q_accu',
+        self.wdg_q_accu = UI_Q(self, fb.fil[0]['fxq']['QA'], wdg_name='q_accu',
                                label='Accu Format <i>Q<sub>A&nbsp;</sub></i>:')
 
         # initial setting for accumulator
         cmbW = qget_cmb_box(self.wdg_w_accu.cmbW, data=False)
-        self.wdg_w_accu.ledWF.setEnabled(cmbW == 'man')
-        self.wdg_w_accu.ledWI.setEnabled(cmbW == 'man')
+        self.wdg_w_accu.ledWF.setEnabled(cmbW == 'm')
+        self.wdg_w_accu.ledWI.setEnabled(cmbW == 'm')
 
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs & EVENTFILTERS
         # ----------------------------------------------------------------------
         self.wdg_w_coeffs.sig_tx.connect(self.update_q_coeff)
         self.wdg_w_accu.sig_tx.connect(self.process_sig_rx)
         self.wdg_q_accu.sig_tx.connect(self.process_sig_rx)
@@ -118,116 +119,114 @@
         # if not, just emit the dict.
         if 'ui' in dict_sig:
             if dict_sig['wdg_name'] == 'w_coeff':  # coefficient format updated
                 """
                 Update coefficient quantization settings and coefficients.
 
                 The new values are written to the fixpoint coefficient dict as
-                `fb.fil[0]['fxqc']['QCB']` and  `fb.fil[0]['fxqc']['b']`.
+                `fb.fil[0]['fxq']['QCB']` and  `fb.fil[0]['fxq']['b']`.
                 """
 
-                fb.fil[0]['fxqc'].update(self.ui2dict())
+                fb.fil[0]['fxq'].update(self.ui2dict())
 
             elif dict_sig['wdg_name'] == 'w_accu':  # accu format updated
                 cmbW = qget_cmb_box(self.wdg_w_accu.cmbW, data=False)
-                self.wdg_w_accu.ledWF.setEnabled(cmbW == 'man')
-                self.wdg_w_accu.ledWI.setEnabled(cmbW == 'man')
-                if cmbW in {'full', 'auto'}\
+                self.wdg_w_accu.ledWF.setEnabled(cmbW == 'm')
+                self.wdg_w_accu.ledWI.setEnabled(cmbW == 'm')
+                if cmbW in {'f', 'a'}\
                         or ('ui' in dict_sig and dict_sig['ui'] in {'WF', 'WI'}):
                     pass
 
-                elif cmbW == 'man':  # switched to manual, don't do anything
+                elif cmbW == 'm':  # switched to manual, don't do anything
                     return
 
             # Accu quantization or overflow settings have been changed
             elif dict_sig['wdg_name'] == 'q_accu':
                 pass
 
             else:
                 logger.error(f"Unknown widget name '{dict_sig['wdg_name']}' "
                              f"in '{__name__}' !")
                 return
 
             # - update fixpoint accu and coefficient quantization dict
             # - emit {'fx_sim': 'specs_changed'}
-            fb.fil[0]['fxqc'].update(self.ui2dict())
+            fb.fil[0]['fxq'].update(self.ui2dict())
             self.emit({'fx_sim': 'specs_changed'})
 
         else:
             logger.error(f"Unknown key '{dict_sig['wdg_name']}' (should be 'ui')"
                          f"in '{__name__}' !")
 
 # ------------------------------------------------------------------------------
     def update_q_coeff(self, dict_sig):
         """
         Update coefficient quantization settings and coefficients.
 
         The new values are written to the fixpoint coefficient dict as
-        `fb.fil[0]['fxqc']['QCB']` and
-        `fb.fil[0]['fxqc']['b']`.
+        `fb.fil[0]['fxq']['QCB']` and
+        `fb.fil[0]['fxq']['b']`.
         """
         logger.debug("update q_coeff - dict_sig:\n{0}".format(pprint_log(dict_sig)))
         # dict_sig.update({'ui':'C'+dict_sig['ui']})
-        fb.fil[0]['fxqc'].update(self.ui2dict())
-        logger.debug("b = {0}".format(pprint_log(fb.fil[0]['fxqc']['b'])))
+        fb.fil[0]['fxq'].update(self.ui2dict())
+        logger.debug("b = {0}".format(pprint_log(fb.fil[0]['fxq']['b'])))
 
         self.process_sig_rx(dict_sig)
 
 # ------------------------------------------------------------------------------
     def update_accu_settings(self):
         """
         Calculate number of extra integer bits needed in the accumulator (bit
         growth) depending on the coefficient area (sum of absolute coefficient
         values) for `cmbW == 'auto'` or depending on the number of coefficients
         for `cmbW == 'full'`. The latter works for arbitrary coefficients but
         requires more bits.
 
         The new values are written to the fixpoint coefficient dict
-        `fb.fil[0]['fxqc']['QA']`.
+        `fb.fil[0]['fxq']['QA']`.
         """
         try:
-            if qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == "full":
-                A_coeff = int(np.ceil(np.log2(len(fb.fil[0]['fxqc']['b']))))
-            elif qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == "auto":
+            if qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == 'f':
+                A_coeff = int(np.ceil(np.log2(len(fb.fil[0]['fxq']['b']))))
+            elif qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == 'a':
                 A_coeff = int(np.ceil(np.log2(np.sum(np.abs(fb.fil[0]['ba'][0])))))
         except Exception as e:
             logger.error(e)
             return
 
-        if qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == "full" or\
-                qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == "auto":
-            fb.fil[0]['fxqc']['QA']['WF'] = fb.fil[0]['fxqc']['QI']['WF']\
-                + fb.fil[0]['fxqc']['QCB']['WF']
-            fb.fil[0]['fxqc']['QA']['WI'] = fb.fil[0]['fxqc']['QI']['WI']\
-                + fb.fil[0]['fxqc']['QCB']['WI'] + A_coeff
-
-        # calculate total accumulator word length and 'Q' format
-        fb.fil[0]['fxqc']['QA']['W'] = fb.fil[0]['fxqc']['QA']['WI']\
-            + fb.fil[0]['fxqc']['QA']['WF'] + 1
-        fb.fil[0]['fxqc']['QA']['Q'] = str(fb.fil[0]['fxqc']['QA']['WI'])\
-            + '.' + str(fb.fil[0]['fxqc']['QA']['WF'])
+        if qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == 'f' or\
+                qget_cmb_box(self.wdg_w_accu.cmbW, data=False) == 'a':
+            fb.fil[0]['fxq']['QA']['WF'] = fb.fil[0]['fxq']['QI']['WF']\
+                + fb.fil[0]['fxq']['QCB']['WF']
+            fb.fil[0]['fxq']['QA']['WI'] = fb.fil[0]['fxq']['QI']['WI']\
+                + fb.fil[0]['fxq']['QCB']['WI'] + A_coeff
+
+        # calculate total accumulator word length
+        fb.fil[0]['fxq']['QA']['W'] = fb.fil[0]['fxq']['QA']['WI']\
+            + fb.fil[0]['fxq']['QA']['WF'] + 1
 
         # update quantization settings
-        fb.fil[0]['fxqc']['QA'].update(self.wdg_q_accu.q_dict)
+        fb.fil[0]['fxq']['QA'].update(self.wdg_q_accu.q_dict)
 
         # update UI
-        self.wdg_w_accu.dict2ui(fb.fil[0]['fxqc']['QA'])
+        self.wdg_w_accu.dict2ui(fb.fil[0]['fxq']['QA'])
 
 # ------------------------------------------------------------------------------
     def dict2ui(self):
         """
         Update all parts of the UI that need to be updated when specs have been
         changed outside this class, e.g. coefficients and coefficient wordlength.
         This also provides the initial setting for the widgets when the filter has
         been changed.
 
         This is called from one level above by
         :class:`pyfda.input_widgets.input_fixpoint_specs.Input_Fixpoint_Specs`.
         """
-        fxqc_dict = fb.fil[0]['fxqc']
+        fxqc_dict = fb.fil[0]['fxq']
         if 'QA' not in fxqc_dict:
             fxqc_dict.update({'QA': {}})  # no accumulator settings in dict yet
             logger.warning("QA key missing")
 
         if 'QCB' not in fxqc_dict:
             fxqc_dict.update({'QCB': {}})  # no coefficient settings in dict yet
             logger.warning("QCB key missing")
@@ -235,21 +234,21 @@
         self.wdg_w_coeffs.dict2ui(fxqc_dict['QCB'])  # update coefficient wordlength
         self.update_accu_settings()                  # update accumulator settings
 
 # ------------------------------------------------------------------------------
     def ui2dict(self):
         """
         Read out the quantization subwidgets and store their settings in the central
-        fixpoint dictionary `fb.fil[0]['fxqc']` using the keys described below.
+        fixpoint dictionary `fb.fil[0]['fxq']` using the keys described below.
 
         Coefficients are quantized with these settings in the subdictionary under
         the key 'b'.
 
         Additionally, these subdictionaries are returned  to the caller
-        (``input_fixpoint_specs``) where they are used to update ``fb.fil[0]['fxqc']``
+        (``input_fixpoint_specs``) where they are used to update ``fb.fil[0]['fxq']``
 
         Parameters
         ----------
 
         None
 
         Returns
@@ -261,40 +260,40 @@
         - 'QCB': dictionary with b coefficients quantization settings
 
         - 'QA': dictionary with accumulator quantization settings
 
         - 'b' : list of quantized b coefficients in format WI.WF
 
         """
-        fxqc_dict = fb.fil[0]['fxqc']
+        fxqc_dict = fb.fil[0]['fxq']
         if 'QA' not in fxqc_dict:
             # no accumulator settings in dict yet:
             fxqc_dict.update({'QA': self.wdg_w_accu.q_dict})
-            logger.warning("Empty dict 'fxqc['QA]'!")
+            logger.warning("Empty dict 'fb.fil{0]['fxq']['QA']'!")
         else:
             fxqc_dict['QA'].update(self.wdg_w_accu.q_dict)
 
         if 'QCB' not in fxqc_dict:
             # no coefficient settings in dict yet
             fxqc_dict.update({'QCB': self.wdg_w_coeffs.q_dict})
-            logger.warning("Empty dict 'fxqc['QCB]'!")
+            logger.warning("Empty dict 'fb.fil{0]['fxq']['QCB']'!")
         else:
             fxqc_dict['QCB'].update(self.wdg_w_coeffs.q_dict)
 
         fxqc_dict.update({'b': self.wdg_w_coeffs.quant_coeffs(
             self.wdg_w_coeffs.q_dict, fb.fil[0]['ba'][0], to_int=True)})
         return fxqc_dict
 
 # ------------------------------------------------------------------------------
     def init_filter(self):
         """
         Construct an instance of the fixpoint filter object using the settings from
-        the 'fxqc' quantizer dict
+        the 'fxq' quantizer dict
         """
-        p = fb.fil[0]['fxqc']  # parameter dictionary with coefficients etc.
+        p = fb.fil[0]['fxq']  # parameter dictionary with coefficients etc.
         if not all(np.isfinite(p['b'])):
             logger.error("Coefficients contain non-finite values!")
             return
         if any(np.iscomplex(p['b'])):
             logger.error("Coefficients contain complex values!")
             return
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/fixpoint_helpers.py` & `pyfda-0.9.0b1/pyfda/fixpoint_widgets/old/fixpoint_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     'tip_WF'        : 'Number of frac. bits'    # Mouse-over tooltip
 
 
     'lock_visible'  : False                     # Pushbutton for locking visible
     'tip_lock'      : 'Lock input/output quant.'# Tooltip for  lock push button
 
     'combo_visible' : False                     # Enable integrated combo widget
-    'combo_items'   : ['auto', 'full', 'man']   # Combo selection
+    'combo_items'   : ['a', 'f', 'm']           # Combo selection
     'tip_combo'     : 'Calculate Acc. width.'   # tooltip for combo
     """
     # sig_rx = pyqtSignal(object)  # incoming,
     sig_tx = pyqtSignal(object)  # outcgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
     def __init__(self, q_dict, **kwargs):
@@ -122,31 +122,31 @@
 
         self.ledWI = QLineEdit(self)
         self.ledWI.setToolTip(dict_ui['tip_WI'])
         self.ledWI.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
         self.ledWI.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
         self.ledWI.setObjectName("WI")
 
-        lblDot = QLabel(dict_ui['lbl_sep'], self)
-        lblDot.setVisible(dict_ui['fractional'])
+        lbl_sep = QLabel(dict_ui['lbl_sep'], self)
+        lbl_sep.setVisible(dict_ui['fractional'])
 
         self.ledWF = QLineEdit(self)
         self.ledWF.setToolTip(dict_ui['tip_WF'])
         self.ledWF.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
         self.ledWF.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
         self.ledWF.setVisible(dict_ui['fractional'])
         self.ledWF.setObjectName("WF")
 
         layH = QHBoxLayout()
         layH.addWidget(lblW)
         layH.addStretch()
         layH.addWidget(self.cmbW)
         layH.addWidget(self.butLock)
         layH.addWidget(self.ledWI)
-        layH.addWidget(lblDot)
+        layH.addWidget(lbl_sep)
         layH.addWidget(self.ledWF)
         layH.setContentsMargins(0, 0, 0, 0)
 
         frmMain = QFrame(self)
         frmMain.setLayout(layH)
 
         layVMain = QVBoxLayout()  # Widget main layout
@@ -487,15 +487,15 @@
     'tip_WF'        : 'Number of frac. bits'    # Mouse-over tooltip
 
     'lock_visible'  : False                     # Pushbutton for locking visible
     'tip_lock'      : 'Lock input/output quant.'# Tooltip for  lock push button
 
     'cmb_w_vis'     : False                     # Integrated combo widget visible?
     'cmb_w_items'   : List with tooltip and combo box choices
-    'cmb_w_init'    : 'man'                     # initial setting
+    'cmb_w_init'    : 'm'                       # initial setting
 
     'enabled'       : True                      # Is widget enabled?
     'visible'       : True                      # Is widget visible?
     """
     # incoming,
     # sig_rx = pyqtSignal(object)
     # outcgoing
@@ -517,33 +517,33 @@
                  ("floor", "Floor", "<span>Round towards negative infinity / "
                   "two's complement truncation.</span>")]
         cmb_ov = ["<span>Select overflow behaviour.</span>",
                   ("wrap", "Wrap", "Two's complement wrap around"),
                   ("sat", "Sat",
                    "<span>Saturation, i.e. limit at min. / max. value</span>")]
         cmb_w = ["<span>Set Accumulator word format</span>",
-                 ("man", "Man", "<span>Manual entry of word format.</span>"),
-                 ("auto", "Auto",
+                 ("m", "Man", "<span>Manual entry of word format.</span>"),
+                 ("a", "Auto",
                   "<span>Automatic calculation from coefficients and input word formats "
                   "taking coefficients area into account.</span>"),
-                 ("full", "Full",
+                 ("f", "Full",
                   "<span>Automatic calculation from coefficients and input word formats "
                   "for arbitrary coefficients.</span>")
                  ]
         # default widget settings:
         dict_ui = {'wdg_name': 'ui_wq', 'label': '',
                    'label_q': 'Quant.', 'cmb_q_items': cmb_q, 'quant': 'round',
                    'label_ov': 'Ovfl.', 'cmb_ov_items': cmb_ov, 'ovfl': 'wrap',
                    'enabled': True, 'visible': True,
                    #
                    'label_w': '<i>WI.WF</i>&nbsp;:', 'lbl_sep': '.', 'max_led_width': 30,
                    'WI': 0, 'WI_len': 2, 'tip_WI': 'Number of integer bits',
                    'WF': 15, 'WF_len': 2, 'tip_WF': 'Number of fractional bits',
                    'fractional': True,
-                   'cmb_w_vis': False, 'cmb_w_items': cmb_w, 'cmb_w_init': 'man',
+                   'cmb_w_vis': False, 'cmb_w_items': cmb_w, 'cmb_w_init': 'm',
                    'lock_visible': False, 'tip_lock': 'Lock input/output quantization.'
                    }
         # test whether quantization and overflow parameters in self.q_dict are
         # in the lists of combobox entries and assign them when True
         # TODO: doesn't work at the moment, dict_ui['cmb_q_items'] is not a simple list
         # if 'quant' in self.q_dict and self.q_dict['quant'] in dict_ui['cmb_q_items']:
         #     dict_ui['quant'] = self.q_dict['quant']
@@ -589,16 +589,16 @@
 
         self.ledWI = QLineEdit(self)
         self.ledWI.setToolTip(dict_ui['tip_WI'])
         self.ledWI.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
         self.ledWI.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
         self.ledWI.setObjectName("WI")
 
-        lblDot = QLabel(dict_ui['lbl_sep'], self)
-        lblDot.setVisible(dict_ui['fractional'])
+        lbl_sep = QLabel(dict_ui['lbl_sep'], self)
+        lbl_sep.setVisible(dict_ui['fractional'])
 
         self.ledWF = QLineEdit(self)
         self.ledWF.setToolTip(dict_ui['tip_WF'])
         self.ledWF.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
         self.ledWF.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
         self.ledWF.setVisible(dict_ui['fractional'])
         self.ledWF.setObjectName("WF")
@@ -606,15 +606,15 @@
         lay_W = QHBoxLayout()
         lay_W.addStretch()
         lay_W.addWidget(lbl_W)
         # lay_W.addStretch()
         lay_W.addWidget(self.cmbW)
         lay_W.addWidget(self.butLock)
         lay_W.addWidget(self.ledWI)
-        lay_W.addWidget(lblDot)
+        lay_W.addWidget(lbl_sep)
         lay_W.addWidget(self.ledWF)
         lay_W.setContentsMargins(0, 0, 0, 0)
 
         layG = QGridLayout()
         layG.addWidget(lbl_wdg, 0, 0)
         layG.addLayout(lay_W, 1, 0)
         # lay_W.addStretch()
```

### Comparing `pyfda-0.8.4/pyfda/fixpoint_widgets/old/fixpoint_helpers_nmigen.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_fix_lib_amaranth.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 Helper classes and functions for nmigen fixpoint filters
 """
 from pyfda.libs.pyfda_lib import cmp_version
 import logging
 logger = logging.getLogger(__name__)
 
 # ------------------------------------------------------------------------------
-if cmp_version("nmigen", "0.2") >= 0:
-    from nmigen import Signal, signed, Cat, Module, Repl
+if cmp_version("nmigen", "0.3") >= 0:
+    from amaranth import Signal, signed, Cat, Module, Repl
 
     def requant(mod: Module, sig_i: Signal, QI: dict, QO: dict) -> Signal:
         """
-        Change word length of input signal `sig_i` to `WO` bits, using the
-        quantization and saturation methods specified by ``QO['quant']`` and
-        ``QO['ovfl']``.
+        Change word length of input signal `sig_i` to the wordlength of the output
+        signal, using the quantization and saturation methods specified by
+        ``QO['quant']`` and ``QO['ovfl']``.
 
         Parameters
         ----------
 
         mod: Module (nmigen)
             instance of migen module
 
@@ -42,15 +42,15 @@
             Quantization dict for output word format; the keys 'WI' and 'WF' for
             integer and fractional wordlength are evaluated as well as the keys 'quant'
             and 'ovfl' describing requantization and overflow behaviour.
 
         Returns
         -------
 
-        sig_o: Signal (nmigen)
+        sig_o: Signal (amaranth)
             Requantized signal
 
         Documentation
         -------------
 
         **Input and output word are aligned at their binary points.**
 
@@ -58,53 +58,53 @@
         using wrap-around and truncation. It's easy to see that for simple wrap-around
         logic, the sign of the result may change.
 
         ::
 
         S | WI1 | WI0 * WF0 | WF1 | WF2 | WF3  :  WI = 2, WF = 4, W = 7
         0 |  1  |  0  *  1  |  0  |  1  |  1   =  43 (dec) or 43/16 = 2 + 11/16 (float)
-                        *
+                      *
                 |  S  * WF0 | WF1 | WF2        :  WI = 0, WF = 3, W = 4
-                    0  *  1  |  0  |  1         =  7 (dec) or 7/8 (float)
+                   0  *  1  |  0  |  1         =  7 (dec) or 7/8 (float)
 
 
         The float or "real (world) value" is calculated by multiplying the integer
         value by 2 ** (-WF).
 
         For requantizing two numbers to the same WI and WF, imagine both binary numbers
         to be right-aligned. Changes in the number of integer bits `dWI` and fractional
         bits `dWF` are handled separately.
 
         Fractional Bits
         ---------------
 
         - For reducing the number of fractional bits by `dWF`, simply right-shift the
-        integer number by `dWF`. For rounding, add '1' to the bit below the truncation
-        point before right-shifting.
+          integer number by `dWF`. For rounding, add '1' to the bit below the truncation
+          point before right-shifting.
 
         - Extend the number of fractional bits by left-shifting the integer by `dWF`,
-        LSB's are filled with zeros.
+          LSB's are filled with zeros.
 
         Integer Bits
         ------------
 
         - For reducing the number of integer bits by `dWI`, simply right-shift the
-        integer by `dWI`.
+          integer by `dWI`.
 
         - The number of fractional bits is SIGN-EXTENDED by filling up the left-most
-        bits with the sign bit.
+          bits with the sign bit.
 
         """
         WI_I = QI['WI']         # number of integer bits (input signal)
-        WI_F = QI['WF']         # number of integer bits (output signal)
+        WI_F = QI['WF']         # number of fractional bits (input signal)
         WI   = WI_I + WI_F + 1  # total word length (input signal)
 
-        WO_I = QO['WI']         # number of integer bits (input signal)
-        WO_F = QO['WF']         # number of integer bits (output signal)
-        WO   = WO_I + WO_F + 1  # total word length (input signal)
+        WO_I = QO['WI']         # number of integer bits (output signal)
+        WO_F = QO['WF']         # number of fractional bits (output signal)
+        WO   = WO_I + WO_F + 1  # total word length (output signal)
 
         dWF = WI_F - WO_F       # difference of fractional lengths
         dWI = WI_I - WO_I       # difference of integer lengths
 
         # max. resp. min, output values
         MIN_o = - 1 << (WO - 1)
         MAX_o = -MIN_o - 1
@@ -156,12 +156,12 @@
             mod.d.comb += sig_o.eq(sig_i_q)
 
         else:
             raise Exception(u'Unknown overflow method "%s"!' % (QI['ovfl']))
 
         return sig_o
 else:
-    logger.error('Module "nmigen" not found!')
+    logger.error('Module "amaranth" not found!')
 
 # ==============================================================================
 if __name__ == '__main__':
     pass
```

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/appbar.from_clipboard.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.from_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/appbar.list.add.above.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.list.add.above.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/appbar.list.delete.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.list.delete.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/appbar.to_clipboard.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/appbar.to_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/cog.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/cog.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/grid_fine.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/grid_fine.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/dark/quantize.svg` & `pyfda-0.9.0b1/pyfda/images/icons/dark/quantize.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/fft.svg` & `pyfda-0.9.0b1/pyfda/images/icons/fft.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon.svg` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_128.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_128.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_16.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_16.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_256.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_256.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_32.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_32.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_48.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_48.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_64.png` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_64.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/icons/pyfda_icon_nobg.svg` & `pyfda-0.9.0b1/pyfda/images/icons/pyfda_icon_nobg.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/appbar.base.select_grey.svg` & `pyfda-0.9.0b1/pyfda/images/unused/appbar.base.select_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/appbar.list.add.above_grey.svg` & `pyfda-0.9.0b1/pyfda/images/unused/appbar.list.add.above_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/audio/audio.svg` & `pyfda-0.9.0b1/pyfda/images/unused/audio/audio.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/audio/audio_90.odg` & `pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/audio/audio_90.png` & `pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/audio/audio_90.svg` & `pyfda-0.9.0b1/pyfda/images/unused/audio/audio_90.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/audio/ic_forward_10_48px.svg` & `pyfda-0.9.0b1/pyfda/images/unused/audio/ic_forward_10_48px.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/graph_90.odg` & `pyfda-0.9.0b1/pyfda/images/unused/graph_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/images/unused/graph_90.png` & `pyfda-0.9.0b1/pyfda/images/unused/graph_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/input_widgets/amplitude_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/amplitude_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,43 +8,61 @@
 import sys
 
 from pyfda.libs.compat import (
     QtCore, Qt, QEvent, pyqtSignal, QWidget, QLabel, QLineEdit, QComboBox, QFrame,
     QFont, QVBoxLayout, QHBoxLayout, QGridLayout)
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_lib import to_html, lin2unit, unit2lin, safe_eval
+from pyfda.libs.pyfda_lib import(
+    to_html, lin2unit, unit2lin, safe_eval, pprint_log, first_item)
 from pyfda.libs.pyfda_qt_lib import qstyle_widget, qget_cmb_box
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class AmplitudeSpecs(QWidget):
     """
     Build and update widget for entering the amplitude
     specifications like A_SB, A_PB etc.
     """
+    sig_rx = pyqtSignal(object)  # receive signals from higher hierarchies
     sig_tx = pyqtSignal(object)  # emitted when amplitude unit or spec has been changed
+
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None, title="Amplitude Specs"):
+    def __init__(self, parent=None, title="Amplitude Specs", objectName=""):
         """
         Initialize
         """
         super(AmplitudeSpecs, self).__init__(parent)
         self.title = title
+        self.setObjectName(objectName)
 
         self.qlabels = []    # list with references to QLabel widgets
         self.qlineedit = []  # list with references to QLineEdit widgets
 
         self.spec_edited = False  # flag whether QLineEdit field has been edited
         self._construct_UI()
 
+# -------------------------------------------------------------
+    def process_sig_rx(self, dict_sig=None):
+        """
+        Process signals coming in via subwidgets and sig_rx
+        """
+        # logger.warning(
+        #    f"SIG_RX: {first_item(dict_sig)}")
+        if dict_sig['id'] == id(self):
+            # this should never happen
+            logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
+            return
+        elif 'data_changed' in dict_sig and dict_sig['data_changed'] == 'filter_loaded':
+            self.load_dict()
+
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct User Interface
         """
         amp_units = ["dB", "V", "W"]
 
@@ -52,17 +70,16 @@
         bfont.setBold(True)
         lblTitle = QLabel(str(self.title), self)  # field for widget title
         lblTitle.setFont(bfont)
         lblTitle.setWordWrap(True)
 
         lblUnits = QLabel("in", self)
 
-        self.cmbUnitsA = QComboBox(self)
+        self.cmbUnitsA = QComboBox(self, objectName="cmbUnitsA")
         self.cmbUnitsA.addItems(amp_units)
-        self.cmbUnitsA.setObjectName("cmbUnitsA")
         self.cmbUnitsA.setToolTip(
             "<span>Unit for amplitude specifications:"
             " dB is attenuation (&gt; 0); levels in V and W have to be &lt; 1.</span>")
 
         # fit size dynamically to largest element:
         self.cmbUnitsA.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
@@ -100,14 +117,19 @@
         #   with "A" (= amplitude specifications of the current filter)
         # - Pass the list to update_UI which recreates the widget
         # ATTENTION: Entries need to be converted from QString to str for Py 2
         new_labels = [str(l) for l in fb.fil[0] if l[0] == 'A']
         self.update_UI(new_labels=new_labels)
 
         # ----------------------------------------------------------------------
+        # GLOBAL SIGNALS & SLOTs
+        # ----------------------------------------------------------------------
+        self.sig_rx.connect(self.process_sig_rx)
+
+        # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs / EVENT MONITORING
         # ----------------------------------------------------------------------
         self.cmbUnitsA.currentIndexChanged.connect(self._set_amp_unit)
         #       ^ this also triggers the initial load_dict
         # DYNAMIC EVENT MONITORING
         # Every time a field is edited, call self._store_entry and
         # self.load_dict. This is achieved by dynamically installing and
@@ -130,15 +152,15 @@
           `spec_edited`== True) and display the stored value in selected format
         """
         if isinstance(source, QLineEdit):  # could be extended for other widgets
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
                 self.load_dict()
                 # store current entry in case new value can't be evaluated:
-                fb.data_old = source.text()
+                self.data_prev = source.text()
             elif event.type() == QEvent.KeyPress:
                 self.spec_edited = True  # entry has been changed
                 key = event.key()
                 if key in {QtCore.Qt.Key_Return, QtCore.Qt.Key_Enter}:  # store entry
                     self._store_entry(source)
                 elif key == QtCore.Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
@@ -244,15 +266,15 @@
         Spec entries are *always* stored in linear units; only the
         displayed values are adapted to the amplitude unit, not the dictionary!
         """
         if self.spec_edited:
             unit = str(self.cmbUnitsA.currentText())
             filt_type = fb.fil[0]['ft']
             amp_label = str(source.objectName())
-            amp_value = safe_eval(source.text(), fb.data_old, sign='pos')
+            amp_value = safe_eval(source.text(), self.data_prev, sign='pos')
             fb.fil[0].update({amp_label: unit2lin(amp_value, filt_type, amp_label, unit)})
             self.emit({'specs_changed': 'a_specs'})
             self.spec_edited = False  # reset flag
         self.load_dict()
 
 # -------------------------------------------------------------
     def _hide_entries(self, num_new_labels):
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/freq_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/freq_specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 # Licensed under the terms of the MIT License
 # (see file LICENSE in root directory for details)
 
 """
 Subwidget for entering frequency specifications
 """
 import sys
+import re
 from pyfda.libs.compat import (
     QtCore, Qt, QWidget, QLabel, QLineEdit, QFrame, QFont, QVBoxLayout, QHBoxLayout,
     QGridLayout, pyqtSignal, QEvent)
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_lib import to_html, safe_eval, unique_roots
+from pyfda.libs.pyfda_lib import to_html, safe_eval, unique_roots, pprint_log, first_item
 from pyfda.libs.pyfda_qt_lib import qstyle_widget
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
 import logging
 logger = logging.getLogger(__name__)
 
 MIN_FREQ_STEP = 1e-4
@@ -30,38 +31,41 @@
     specifications like F_sb, F_pb etc.
     """
     # class variables (shared between instances if more than one exists)
     sig_tx = pyqtSignal(object)  # outgoing
     sig_rx = pyqtSignal(object)  # incoming
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None, title="Frequency Specs"):
+    def __init__(self, parent=None, title="Frequency Specs", objectName=""):
 
         super(FreqSpecs, self).__init__(parent)
         self.title = title
 
         self.qlabels = []    # list with references to QLabel widgets
         self.qlineedit = []  # list with references to QLineEdit widgetss
 
         self.spec_edited = False  # flag whether QLineEdit field has been edited
+        self.setObjectName(objectName)
 
         self._construct_UI()
 
 # -------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming in via subwidgets and sig_rx
         """
-        # logger.debug("Processing {0}: {1}".format(type(dict_sig).__name__, dict_sig))
+        # logger.warning(
+        #     f"SIG_RX: {first_item(dict_sig)}")
         if dict_sig['id'] == id(self):
             # logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
             return
-        elif 'specs_changed' in dict_sig and dict_sig['specs_changed'] == 'f_specs':
-            self.sort_dict_freqs()
-        elif 'view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S':
+        elif ('view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S')\
+                or ('data_changed' in dict_sig
+                and dict_sig['data_changed'] in {'filter_loaded', 'filter_designed'}):
+            # update frequencies and unit and load_dict.
             self.recalc_freqs()
 
 # -------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct the User Interface
         """
@@ -126,89 +130,82 @@
         - When a QLineEdit widget loses input focus (QEvent.FocusOut`), store
           current value normalized to f_S with full precision (only if
           `spec_edited`== True) and display the stored value in selected format
         """
         if isinstance(source, QLineEdit):  # could be extended for other widgets
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
-                self.load_dict()
                 # store current entry in case new value can't be evaluated:
-                fb.data_old = source.text()
+                self.data_prev = source.text()
+                self.update_f_display(source)
             elif event.type() == QEvent.KeyPress:
                 self.spec_edited = True  # entry has been changed
                 key = event.key()
                 if key in {QtCore.Qt.Key_Return, QtCore.Qt.Key_Enter}:
                     self._store_entry(source)
                 elif key == QtCore.Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
-                    self.load_dict()
-
+                    self.update_f_display(source)
             elif event.type() == QEvent.FocusOut:
                 self._store_entry(source)
         # Call base class method to continue normal event processing:
         return super(FreqSpecs, self).eventFilter(source, event)
 
     # --------------------------------------------------------------------------
     def _store_entry(self, event_source):
         """
-        _store_entry is triggered by `QEvent.focusOut` in the eventFilter:
-        When the textfield of `widget` has been edited (`self.spec_edited` =  True),
-        sort and store all entries in filter dict, then reload the text fields.
-        Finally, emit a SpecsChanged signal.
+        `_store_entry()` is triggered by `QEvent.focusOut` in the eventFilter:
+        When the `event_source` has been edited (`self.spec_edited ==  True`),
+        evaluate the text field, normalize it with f_S and store it in the filter
+        dict. Sort and store all entries in filter dict, then reload the text fields.
+        Finally, emit a 'specs_changed': 'f_specs' signal.
         """
         if self.spec_edited:
             f_label = str(event_source.objectName())
             f_value = safe_eval(
-                event_source.text(), fb.data_old, sign='pos') / fb.fil[0]['f_S']
+                event_source.text(), self.data_prev, sign='pos') / fb.fil[0]['f_S']
             fb.fil[0].update({f_label: f_value})
-            self.sort_dict_freqs()
-            self.emit({'specs_changed': 'f_specs'})
+            self.sort_dict_freqs()  # sort and update display
+            self.emit({'specs_changed': 'f_specs', 'sender_name': f_label})
             self.spec_edited = False  # reset flag
-
-        # nothing has changed, but display frequencies in rounded format anyway
         else:
-            self.load_dict()
+            self.update_f_display(event_source)  # just update / restore display
 
     # --------------------------------------------------------------------------
     def update_UI(self, new_labels=()):
         """
-        Called from filter_specs.update_UI() and target_specs.update_UI()
+        Called by `input_specs.update_UI()` and `target_specs.update_UI()`
         Set labels and get corresponding values from filter dictionary.
         When number of entries has changed, the layout of subwidget is rebuilt,
         using
 
         - `self.qlabels`, a list with references to existing QLabel widgets,
         - `new_labels`, a list of strings from the filter_dict for the current
           filter design
         - 'num_new_labels`, their number
         - `self.n_cur_labels`, the number of currently visible labels / qlineedit
           fields
         """
-        self.update_f_unit()
         state = new_labels[0]
         new_labels = new_labels[1:]
         num_new_labels = len(new_labels)
         # hide / show labels / create new subwidgets if neccessary:
         self._show_entries(num_new_labels)
 
 #        W_lbl = max([self.qfm.width(l) for l in new_labels]) # max. label width in pixel
 
         # ---------------------------- logging -----------------------------
-        logger.debug("update_UI: {0}-{1}-{2}".format(
-                            fb.fil[0]['rt'], fb.fil[0]['fc'], fb.fil[0]['fo']))
+        # logger.debug("update_UI: {0}-{1}-{2}".format(
+        #                     fb.fil[0]['rt'], fb.fil[0]['fc'], fb.fil[0]['fo']))
 
         f_range = " (0 &lt; <i>f</i> &lt; <i>f<sub>S </sub></i>/2)"
         for i in range(num_new_labels):
             # Update ALL labels and corresponding values
-            if fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny"}:
-                self.qlabels[i].setText(to_html(new_labels[i], frmt='bi'))
-            else:  # convert 'F' to 'f' for frequencies in Hz
-                self.qlabels[i].setText(
-                    to_html(new_labels[i][0].lower() + new_labels[i][1:], frmt='bi'))
-
+            self.qlabels[i].setText(
+                to_html(new_labels[i][0].lower() + new_labels[i][1:], frmt='bi'))
             self.qlineedit[i].setText(str(fb.fil[0][new_labels[i]]))
             self.qlineedit[i].setObjectName(new_labels[i])  # update ID
             qstyle_widget(self.qlineedit[i], state)
 
             if "sb" in new_labels[i].lower():
                 self.qlineedit[i].setToolTip(
                     "<span>Corner frequency for (this) stop band" + f_range + ".</span>")
@@ -221,78 +218,118 @@
 
         self.n_cur_labels = num_new_labels  # update number of currently visible labels
         self.sort_dict_freqs()  # sort frequency entries in dictionary and update display
 
     # --------------------------------------------------------------------------
     def recalc_freqs(self):
         """
-        Update normalized frequencies if required. This is called by via signal
-        ['view_changed': 'f_S']
+        Update normalized frequencies when absolute frequencies are locked and
+        update frequency unit. This is called by via signal {'view_changed': 'f_S'}.
         """
         if fb.fil[0]['freq_locked']:
             for i in range(len(self.qlineedit)):
                 f_name = str(self.qlineedit[i].objectName()).split(":", 1)
                 f_label = f_name[0]
                 f_value = fb.fil[0][f_label] * fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']
+                # logger.warning(f"Updating freq_specs: f_S = {fb.fil[0]['f_S']}, "
+                #                f"f_S_prev = {fb.fil[0]['f_S_prev']}\n{f_label}: {f_value}")
 
                 fb.fil[0].update({f_label: f_value})
-                self.sort_dict_freqs()
-
             self.emit({'specs_changed': 'f_specs'})
 
-# -------------------------------------------------------------
-    def update_f_unit(self):
-        """
-        Set label for frequency unit according to selected unit.
-        """
+        # Always reload normalized frequencies from dict, check whether they are outside
+        # the Nyquist range and display them in the selected unit.
+        self.load_dict()
+
+        # Always set label for frequency unit according to selected unit.
         unit = fb.fil[0]['plt_fUnit']
         if unit in {"f_S", "f_Ny"}:
             unit_frmt = 'bi'
         else:
             unit_frmt = 'b'
         self.lblUnit.setText(" in " + to_html(unit, frmt=unit_frmt))
 
 # -------------------------------------------------------------
+    def update_f_display(self, source):
+        """
+        Update frequency display when frequency or sampling frequency has been
+        updated. Depending on whether it has focus or not, the value is displayed
+        with full precision or rounded.
+
+        Triggered by
+        """
+        f_name = str(source.objectName()).split(':', 1)
+        f_label = f_name[0]
+        f_value = fb.fil[0][f_label] * fb.fil[0]['f_S']
+
+        if source.hasFocus():
+            # widget has focus, show full precision
+            # logger.warning(f"freq_specs: update_f_display {f_label}: {f_value} (disp) "
+            #                 f"{fb.fil[0][f_label]} (dict) FOK")
+            source.setText(str(f_value))
+        else:
+            # widget has no focus, round the display
+            # logger.warning(f"freq_specs: update_f_display {f_label}: {f_value} (disp) "
+            #                f"{fb.fil[0][f_label]} (dict) NFOK")
+            source.setText(params['FMT'].format(f_value))
+
+        # Check whether normalized freqs are inside the range ]0, 0.5[. If not, highlight
+        # widget.
+        if fb.fil[0][f_label] <= 0:
+            logger.warning(
+                f"Frequency {str(source.objectName())} has to be >= 0")
+            source.setProperty("state", 'failed')
+        elif fb.fil[0][f_label] >= 0.5:
+            logger.warning(
+                f"Frequency {str(source.objectName())} has to be < f_S /2.")
+            qstyle_widget(source, 'failed')
+        else:
+            qstyle_widget(source, 'normal')
+
+        return
+
+# -------------------------------------------------------------
     def load_dict(self):
         """
+        Triggered by FocusIn, FocusOut and ESC-Key in LineEdit fields and by
+        `sort_dict_freqs():
+
+        `load_dict()` is called during init and when the frequency unit or the
+          sampling frequency have been changed via
+          `filter_specs.update_UI()` -> `self.update_UI()` -> `self.sort_dict_freqs()`
+
         - Reload textfields from filter dictionary
 
         - Transform the displayed frequency spec input fields according to the units
           setting (i.e. f_S). Spec entries are always stored normalized w.r.t. f_S
           in the dictionary; when f_S or the unit are changed, only the displayed values
           of the frequency entries are updated, not the dictionary!
 
         - Update the displayed frequency unit
 
-        `load_dict()` is called during init and when the frequency unit or the
-          sampling frequency have been changed.
-
         It should be called when `specs_changed` or `data_changed` is emitted
         at another place, indicating that a reload is required.
         """
-
-        # recalculate displayed freq spec values for (maybe) changed f_S
-        logger.debug("exec load_dict")
-        self.update_f_unit()
-
+        # update displayed freq spec values for (maybe) changed f_S
         for i in range(len(self.qlineedit)):
-            f_name = str(self.qlineedit[i].objectName()).split(":", 1)
-            f_label = f_name[0]
-            f_value = fb.fil[0][f_label] * fb.fil[0]['f_S']
-
-            if not self.qlineedit[i].hasFocus():
-                # widget has no focus, round the display
-                self.qlineedit[i].setText(params['FMT'].format(f_value))
+            self.update_f_display(self.qlineedit[i])
+
+            # Print label with "f" for absolute and with "F" for normalized frequencies
+            lbl_text = self.qlabels[i].text()
+            if fb.fil[0]['freq_specs_unit'] in {'f_S', 'f_Ny'}:
+                lbl_text = re.sub(r'[fF]', 'F', lbl_text)
             else:
-                # widget has focus, show full precision
-                self.qlineedit[i].setText(str(f_value))
+                lbl_text = re.sub(r'[fF]', 'f', lbl_text)
+
+            self.qlabels[i].setText(lbl_text)
 
 # ------------------------------------------------------------------------
     def _show_entries(self, num_new_labels):
         """
+        Called by `update_UI()` when filter has changed
         - check whether subwidgets need to be shown or hidden
         - check whether enough subwidgets (QLabel und QLineEdit) exist for the
           the required number of `num_new_labels`:
               - create new ones if required
               - initialize them with dummy information
               - install eventFilter for new QLineEdit widgets so that the filter
                   dict is updated automatically when a QLineEdit field has been
@@ -338,45 +375,33 @@
         The method is called when:
         - update_UI has been called after changing the filter design algorithm
           that the response type has been changed
           eg. from LP -> HP, requiring a different order of frequency entries
         - a frequency spec field has been edited
         - the sort button has been clicked (from filter_specs.py)
         """
-
+        # create list with the normalized frequency values of visible
+        # QLineEdit widgets from the filter dict
         f_specs = [fb.fil[0][str(self.qlineedit[i].objectName())]
                    for i in range(self.n_cur_labels)]
+        # sort them if required
         if fb.fil[0]['freq_specs_sort']:
             f_specs.sort()
-
-        # Make sure normalized freqs are in the range ]0, 0.5[ and are different
-        # by at least MIN_FREQ_STEP
+        # and write them back to the filter dict
         for i in range(self.n_cur_labels):
-            if f_specs[i] <= 0:
-                logger.warning(
-                    f"Frequency {str(self.qlineedit[i].objectName())} has to be >= 0")
-                self.qlineedit[i].setProperty("state", 'failed')
-            elif f_specs[i] >= 0.5:
-                logger.warning(
-                    f"Frequency {str(self.qlineedit[i].objectName())} has to be < f_S /2.")
-                qstyle_widget(self.qlineedit[i], 'failed')
-            else:
-                fb.fil[0][str(self.qlineedit[i].objectName())] = f_specs[i]
-                qstyle_widget(self.qlineedit[i], 'normal')
+            fb.fil[0][str(self.qlineedit[i].objectName())] = f_specs[i]
 
-        # check for (nearly) identical elements:
+        # verify that elements differ by at least MIN_FREQ_STEP by
+        # checking for (nearly) identical elements:
         _, mult = unique_roots(f_specs, tol=MIN_FREQ_STEP)
         ident = [x for x in mult if x > 1]
         if ident:
             logger.warning("Frequencies must differ by at least {0:.4g}"
                            .format(MIN_FREQ_STEP * fb.fil[0]['f_S']))
-
         self.load_dict()
-
-
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.input_widgets.freq_specs` """
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
 
     app = QApplication(sys.argv)
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/freq_units.py` & `pyfda-0.9.0b1/pyfda/input_widgets/freq_units.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 # (see file LICENSE in root directory for details)
 
 """
 Subwidget for entering frequency units
 """
 import sys
 from pyfda.libs.compat import (
-    QtCore, QWidget, QLabel, QLineEdit, QComboBox, QFrame, QFont, QToolButton,
+    QtCore, QWidget, QLabel, QLineEdit, QComboBox, QFrame, QFont, QSizePolicy,
     QIcon, QVBoxLayout, QHBoxLayout, QGridLayout, pyqtSignal, QEvent)
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log
-from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qset_cmb_box, qcmb_box_populate
+from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log, first_item
+from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qset_cmb_box, qcmb_box_populate, PushButton
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class FreqUnits(QWidget):
     """
     Build and update widget for entering frequency unit, frequency range and
     sampling frequency f_S
 
     The following key-value pairs of the `fb.fil[0]` dict are modified:
 
-        - `'freq_specs_unit'` : The unit ('k', 'f_S', 'f_Ny', 'Hz' etc.) as a string
+        - `'freq_specs_unit'` : The unit ('f_S', 'f_Ny', 'Hz' etc.) as a string
         - `'freqSpecsRange'` : A list with two entries for minimum and maximum frequency
                                values for labelling the frequency axis
         - `'f_S'` : The sampling frequency for referring frequency values to as a float
         - `'f_max'` : maximum frequency for scaling frequency axis
         - `'plt_fUnit'`: frequency unit as string
         - `'plt_tUnit'`: time unit as string
         - `'plt_fLabel'`: label for frequency axis
@@ -45,32 +45,31 @@
     # class variables (shared between instances if more than one exists)
     # incoming:
     sig_rx = pyqtSignal(object)
     # outgoing: from various and when normalized frequencies have been changed
     sig_tx = pyqtSignal(object)  # outgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None, title="Frequency Units"):
+    def __init__(self, parent=None, title="Frequency Units", objectName=""):
 
         super(FreqUnits, self).__init__(parent)
         self.title = title
+        self.setObjectName(objectName)
         self.spec_edited = False  # flag whether QLineEdit field has been edited
 
         # combobox tooltip + data / text / tooltip for frequency unit
         self.cmb_f_unit_items = [
             "<span>Select whether frequencies are specified w.r.t. the sampling "
             "frequency " + to_html("f_S", frmt = 'i') + ", to the Nyquist frequency "
-            + to_html("f_Ny = f_S", frmt='i') + "/2 or as absolute values."
-            "'<i>k</i>' specifies frequencies w.r.t. " + to_html("f_S", frmt = 'i') +
-            " but plots graphs over the frequency index <i>k</i>.</span>",
+            + to_html("f_Ny = f_S", frmt='i') + "/2 or as absolute values.",
             ("fs", "f_S", "Relative to sampling frequency, "
              + to_html("F = f / f_S", frmt='i')),
             ("fny", "f_Ny", "Relative to Nyquist frequency, "
-             + to_html("F = f / f_Ny", frmt='i')),
-            ("k", "k", "Frequency index " + to_html("k = 0 ... N_FFT - 1", frmt='i')),
+             + to_html("F = f / f_Ny = 2f / f_S", frmt='i')),
+            # ("k", "k", "Frequency index " + to_html("k = 0 ... N_FFT - 1", frmt='i')),
             ("mhz", "mHz", "Absolute sampling frequency in mHz"),
             ("hz", "Hz", "Absolute sampling frequency in Hz"),
             ("khz", "kHz", "Absolute sampling frequency in kHz"),
             ("meghz", "MHz", "Absolute sampling frequency in MHz"),
             ("ghz", "GHz", "Absolute sampling frequency in GHz")
         ]
         self.cmb_f_unit_init = "fs"
@@ -79,30 +78,30 @@
             "Select one- or two-sided spectrum and symmetry around <i>f</i> = 0",
             ("half", "0...½", "One-sided spectrum"),
             ("whole", "0...1", "Two-sided spectrum, starting at <i>f</i> = 0"),
             ("sym", "-½...½", "Two-sided spectrum, symmetrical around <i>f</i> = 0")
             ]
         self.cmb_f_range_init = "half"
 
-        # t_units and f_scale have the same index as the f_unit_items
-        self.t_units = ['T_S', 'T_S', '', 'ks', 's', 'ms', r'$\mu$s', 'ns']
-        self.f_scale = [1, 1, 1, 1e-3, 1, 1e3, 1e6, 1e9]
+        # t_units and f_scale have the same index as the f_unit_items, i.e.
+        # 'f_S', 'f_Ny', 'mHz', 'Hz', 'kHz', 'MHz', 'GHz'
+        self.t_units = ['T_S', 'T_S', 'ks', 's', 'ms', r'$\mu$s', 'ns']
+        self.f_scale = [1, 1, 1e-3, 1, 1e3, 1e6, 1e9]
 
         self._construct_UI()
 
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from
         - FFT window widget
         - qfft_win_select
         """
 
-        # logger.warning("PROCESS_SIG_RX - vis: {0}\n{1}"
-        #            .format(self.isVisible(), pprint_log(dict_sig)))
+        # logger.warning(f"SIG_RX: {first_item(dict_sig)}")
 
         if 'id' in dict_sig and dict_sig['id'] == id(self):
             logger.debug("Stopped infinite loop")
             return
         elif ('view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S')\
             or 'data_changed' in dict_sig:
             self.update_UI(emit=False)
@@ -118,60 +117,51 @@
         bfont.setBold(True)
 
         self.lblUnits = QLabel(self)
         self.lblUnits.setText("Freq. Unit")
         self.lblUnits.setFont(bfont)
 
         self.f_s_old = fb.fil[0]['f_S']  # store current sampling frequency
+        self.T_s_old = fb.fil[0]['T_S']  # store current sampling period
 
         self.lbl_f_s = QLabel(self)
         self.lbl_f_s.setText(to_html("f_S =", frmt='bi'))
 
-        self.led_f_s = QLineEdit()
+        self.led_f_s = QLineEdit(objectName="f_S")
         self.led_f_s.setText(str(fb.fil[0]["f_S"]))
-        self.led_f_s.setObjectName("f_S")
         self.led_f_s.installEventFilter(self)  # filter events
 
-        self.butLock = QToolButton(self)
+        self.butLock = PushButton(self, icon=QIcon(':/lock-unlocked.svg'))
         self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
-        self.butLock.setCheckable(True)
-        self.butLock.setChecked(False)
         self.butLock.setToolTip(
             "<span><b>Unlocked:</b> When f_S is changed, all frequency related "
             "widgets are updated, normalized frequencies stay the same.<br />"
             "<b>Locked:</b> When f_S is changed, displayed absolute frequency "
             "values don't change but normalized frequencies do.</span>")
 
         layHF_S = QHBoxLayout()
         layHF_S.addWidget(self.led_f_s)
         layHF_S.addWidget(self.butLock)
 
-        self.cmb_f_units = QComboBox(self)
-        self.cmb_f_units.setObjectName("cmb_f_units")
+        self.cmb_f_units = QComboBox(self, objectName="cmb_f_units")
         qcmb_box_populate(self.cmb_f_units, self.cmb_f_unit_items, self.cmb_f_unit_init)
 #        self.cmb_f_units.setItemData(0, (0,QColor("#FF333D"),Qt.BackgroundColorRole))#
 #        self.cmb_f_units.setItemData(0, (QFont('Verdana', bold=True), Qt.FontRole)
 
-        self.cmb_f_range = QComboBox(self)
-        self.cmb_f_range.setObjectName("cmb_f_range")
+        self.cmb_f_range = QComboBox(self, objectName="cmb_f_range")
         qcmb_box_populate(self.cmb_f_range, self.cmb_f_range_items,
                           self.cmb_f_range_init)
 
         # Combobox resizes with longest entry
         self.cmb_f_units.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmb_f_range.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
-        self.butSort = QToolButton(self)
-        self.butSort.setText("Sort")
-        self.butSort.setIcon(QIcon(':/sort-ascending.svg'))
-        #self.butDelCells.setIconSize(q_icon_size)
-        self.butSort.setCheckable(True)
-        self.butSort.setChecked(True)
+        self.butSort = PushButton(self, icon=QIcon(':/sort-ascending.svg'), checked=True)
         self.butSort.setToolTip("Sort frequencies in ascending order when pushed.")
-        self.butSort.setStyleSheet("QToolButton:checked {font-weight:bold}")
+        self.butSort.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
 
         self.layHUnits = QHBoxLayout()
         self.layHUnits.addWidget(self.cmb_f_units)
         self.layHUnits.addWidget(self.cmb_f_range)
         self.layHUnits.addWidget(self.butSort)
 
         # Create a gridLayout consisting of QLabel and QLineEdit fields
@@ -242,70 +232,76 @@
             fb.fil[0]['freq_locked'] = False
             self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
 
 # -------------------------------------------------------------
     def update_UI(self, emit=True):
         """
         update_UI is called
-        - during init
-        - when the unit combobox is changed
-        - when the signal {'view_changed': 'f_S'} has been received. In this case,
-          the UI is updated from the fb.fil[0] dictionary and no signal is emitted.
+        - during init (direct call)
+        - when the unit combobox is changed (signal-slot)
+        - when a signal {'view_changed': 'f_S'} or {'data_changed': ...} has been
+          received. In this case, the UI is updated from the fb.fil[0] dictionary
+          and no signal is emitted (`emit==False`).
 
         Set various scale factors and labels depending on the setting of the unit
         combobox.
 
         Update the freqSpecsRange and finally, emit 'view_changed':'f_S' signal
         """
-        if not emit:  # triggered from outside
+        if not emit:  # triggered by function call, not by a change of UI
+            # Load f_S display from dict
             self.led_f_s.setText(str(fb.fil[0]['f_S']))
+            # Load freq. unit setting from dict
             idx = qset_cmb_box(self.cmb_f_units, fb.fil[0]['freq_specs_unit'],
                                caseSensitive=True)
             if idx == -1:
                 logger.warning(
                     f"Unknown frequency unit {fb.fil[0]['freq_specs_unit']}, "
                     "using 'f_S'.")
+            # Load Frequency range type (0 ... f_S/2 etc.) from dict
             qset_cmb_box(self.cmb_f_range, fb.fil[0]['freqSpecsRangeType'],
                          data=True, fireSignals=True)
 
         f_unit = qget_cmb_box(self.cmb_f_units, data=False)  # selected frequency unit,
         idx = self.cmb_f_units.currentIndex()  # its index
         f_s_scale = self.f_scale[idx]  # and its scaling factor
 
-        is_normalized_freq = f_unit in {"f_S", "f_Ny", "k"}
+        is_normalized_freq = f_unit in {"f_S", "f_Ny"}
 
         self.led_f_s.setVisible(not is_normalized_freq)  # only vis. when
         self.lbl_f_s.setVisible(not is_normalized_freq)  # not normalized
         self.butLock.setVisible(not is_normalized_freq)
 
         if is_normalized_freq:
             # store current sampling frequency to restore it when returning to
-            # unnormalized frequencies
+            # absolute (not normalized) frequencies
             if f_unit == "f_S":  # normalized to f_S
                 fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = 1.
-                fb.fil[0]['T_S'] = 1.
                 f_label = r"$F = f\, /\, f_S = \Omega \, /\,  2 \mathrm{\pi} \; \rightarrow$"
-                t_label = r"$n = t\, /\, T_S \; \rightarrow$"
             elif f_unit == "f_Ny":  # normalized to f_nyq = f_S / 2
                 fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = 2.
-                fb.fil[0]['T_S'] = 1.
                 f_label = r"$F = 2f \, / \, f_S = \Omega \, / \, \mathrm{\pi} \; \rightarrow$"
-                t_label = r"$n = t\, /\, T_S \; \rightarrow$"
             else: # frequency index k,
-                fb.fil[0]['f_S'] = 1.
-                fb.fil[0]['T_S'] = 1.
-                fb.fil[0]['f_max'] = params['N_FFT']
-                f_label = r"$k \; \rightarrow$"
-                t_label = r"$n\; \rightarrow$"
+                logger.error("Unit k is no longer supported!")
+
+            # always use T_S = 1 for normalized frequencies
+            fb.fil[0]['T_S'] = 1.
+            t_label = r"$n = t\, /\, T_S \; \rightarrow$"
+
+            # Don't lock frequency scaling with normalized frequencies
+            fb.fil[0]['freq_locked'] = False
+            self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
 
         else:  # Hz, kHz, ...
-            # Restore sampling frequency when user selected an absolute sampling frequency,
-            # returning from f_S / f_Ny / k
-            if fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny", "k"}:  # previous setting normalized?
+            # Restore sampling frequency when selecting absolute instead of
+            # normalized frequencies
+
+            if fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny"}:  # previous setting normalized?
                 fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = self.f_s_old  # yes, restore prev. f_S
+                fb.fil[0]['T_S'] = self.T_s_old  # yes, restore prev. T_S
 
             # --- try to pick the most suitable unit for f_S --------------
             f_S = fb.fil[0]['f_S'] * f_s_scale
             if f_S >= 1e9:
                 f_unit = "GHz"
             elif f_S >= 1e6:
                 f_unit = "MHz"
@@ -313,44 +309,39 @@
                 f_unit = "kHz"
             elif f_S >= 1:
                 f_unit = "Hz"
             else:
                 f_unit = "mHz"
 
             new_idx = qset_cmb_box(self.cmb_f_units, f_unit, caseSensitive=True)
-            if new_idx != idx:  # sampling frequency needs to be scaled
+            if new_idx != idx:
+                # sampling frequency unit has been changed, f_S and T_S need to be scaled
                 idx = new_idx
                 f_s_scale = self.f_scale[idx]
                 fb.fil[0]['f_S'] = f_S / f_s_scale
+                fb.fil[0]['T_S'] = f_s_scale / f_S
                 emit = True
             # -------------------------------------------------------------
             self.f_s_old = fb.fil[0]['f_S']
+            self.T_s_old = fb.fil[0]['T_S']
             self.led_f_s.setText(params['FMT'].format(fb.fil[0]['f_S']))
 
             f_label = r"$f$ in " + f_unit + r"$\; \rightarrow$"
             t_label = r"$t$ in " + self.t_units[idx] + r"$\; \rightarrow$"
 
-        if f_unit == "k":
-            plt_f_unit = "f_S"
-        else:
-            plt_f_unit = f_unit
-
-        fb.fil[0]['T_S'] = 1./fb.fil[0]['f_S']
-
         fb.fil[0].update({'f_s_scale': f_s_scale})  # scale factor for f_S (Hz, kHz, ...)
         fb.fil[0].update({'freq_specs_unit': f_unit})  # frequency unit
         # time and frequency unit as string e.g. for plot axis labeling
-        fb.fil[0].update({"plt_fUnit": plt_f_unit})
+        fb.fil[0].update({"plt_fUnit": f_unit})
         fb.fil[0].update({"plt_tUnit": self.t_units[idx]})
         # complete plot axis labels including unit and arrow
         fb.fil[0].update({"plt_fLabel": f_label})
         fb.fil[0].update({"plt_tLabel": t_label})
 
         self._freq_range(emit=False)  # update f_lim setting without emitting signal
-
         if emit:  # UI was updated by user or a rescaling of f_S
             self.emit({'view_changed': 'f_S'})
 
 # ------------------------------------------------------------------------------
     def eventFilter(self, source, event):
 
         """
@@ -361,29 +352,35 @@
         - When a QLineEdit widget gains input focus (QEvent.FocusIn`), display
           the stored value from filter dict with full precision
         - When a key is pressed inside the text field, set the `spec_edited` flag
           to True.
         - When a QLineEdit widget loses input focus (QEvent.FocusOut`), store
           current value with full precision (only if `spec_edited`== True) and
           display the stored value in selected format. Emit 'view_changed':'f_S'
-        """
+        - When f_S has been changed, update `fb.fil[0]['f_S']`,
+          emit `{'view_changed': 'f_S'}` to update other widgets and only *then*
+          update {'f_S_prev': fb.fil[0]['f_S']} to allow correction of normalized
+          frequency with the old value of f_S.
+                  """
         def _store_entry():
             """
-            Update filter dictionary, set line edit entry with reduced precision
-            again.
+            Update filter dictionary with sampling frequency and related parameters
+            and emit `{'view_changed': 'f_S'}`.
             """
             if self.spec_edited:
-                fb.fil[0].update({'f_S_prev': fb.fil[0]['f_S']})
-                fb.fil[0].update({'f_S': safe_eval(source.text(), fb.fil[0]['f_S'],
-                                                   sign='pos')})
-                fb.fil[0].update({'T_S': 1./fb.fil[0]['f_S']})
-                fb.fil[0].update({'f_max': fb.fil[0]['f_S']})
+                f_S_tmp = safe_eval(source.text(), fb.fil[0]['f_S'], sign='pos')
+                fb.fil[0].update({'f_S': f_S_tmp})
+                fb.fil[0].update({'T_S': 1./f_S_tmp})
+                fb.fil[0].update({'f_max': f_S_tmp})
 
                 self._freq_range(emit=False)  # update plotting range
                 self.emit({'view_changed': 'f_S'})
+                # Now store current f_S as f_S_prev
+                fb.fil[0].update({'f_S_prev': fb.fil[0]['f_S']})
+
                 self.spec_edited = False  # reset flag, changed entry has been saved
         # ----------------------
         if source.objectName() == 'f_S':
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
                 source.setText(str(fb.fil[0]['f_S']))  # full precision
             elif event.type() == QEvent.KeyPress:
@@ -393,15 +390,16 @@
                     _store_entry()
                 elif key == QtCore.Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
                     source.setText(str(fb.fil[0]['f_S']))  # full precision
             elif event.type() == QEvent.FocusOut:
                 _store_entry()
                 source.setText(params['FMT'].format(fb.fil[0]['f_S']))  # reduced prec.
-        # Call base class method to continue normal event processing:
+
+            # Call base class method to continue normal event processing:
         return super(FreqUnits, self).eventFilter(source, event)
 
     # -------------------------------------------------------------
     def _freq_range(self, emit=True):
         """
         Set frequency plotting range for single-sided spectrum up to f_S/2 or f_S
         or for double-sided spectrum between -f_S/2 and f_S/2
@@ -431,40 +429,31 @@
     # -------------------------------------------------------------
     def load_dict(self):
         """
         Reload comboBox settings and textfields from filter dictionary
         Block signals during update of combobox / lineedit widgets
         This is called from `input_specs.load_dict()`
         """
-        # self.led_f_s.setText(params['FMT'].format(fb.fil[0]['f_S']))
-
-        # qset_cmb_box(self.cmb_f_units, fb.fil[0]['freq_specs_unit'])
-        # is_normalized_freq = fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny", "k"}
-        # self.led_f_s.setVisible(not is_normalized_freq)  # only vis. when
-        # self.lbl_f_s.setVisible(not is_normalized_freq)  # not normalized
-        # self.butLock.setVisible(not is_normalized_freq)
-
-        # qset_cmb_box(self.cmb_f_range, fb.fil[0]['freqSpecsRangeType'])
-
-        # self.butSort.blockSignals(True)
-        # self.butSort.setChecked(fb.fil[0]['freq_specs_sort'])
-        # self.butSort.blockSignals(False)
         self.update_UI(emit=False)
+        # This updates the following widgets:
+        # - `self.led_f_s` from `fb.fil[0]['f_S']`
+        # - `self.cmb_f_units` with `fb.fil[0]['freq_specs_unit']`
+        # - `self.cmb_f_range` from `fb.fil[0]['freqSpecsRangeType']``
+        # The other widgets are updated automatically.
 
 # -------------------------------------------------------------
     def _store_sort_flag(self):
         """
         Store sort flag in filter dict and emit 'specs_changed':'f_sort'
         when sort button is checked.
         """
         fb.fil[0]['freq_specs_sort'] = self.butSort.isChecked()
         if self.butSort.isChecked():
             self.emit({'specs_changed': 'f_sort'})
 
-
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.input_widgets.freq_units` """
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
 
     app = QApplication(sys.argv)
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_coeffs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_coeffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,24 @@
 import numpy as np
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
 from pyfda.libs.pyfda_lib import fil_save, safe_eval, pprint_log
 from pyfda.libs.pyfda_sig_lib import zeros_with_val
 from pyfda.libs.pyfda_qt_lib import (
     qstyle_widget, qset_cmb_box, qget_cmb_box, qget_selected)
-from pyfda.libs.pyfda_io_lib import qtable2csv, data2array, save_data_csv
+from pyfda.libs.pyfda_io_lib import qtable2csv, data2array, export_fil_data
 from pyfda.libs.csv_option_box import CSV_option_box
 
 from pyfda.pyfda_rc import params
 
 from .input_coeffs_ui import Input_Coeffs_UI
 
 import logging
 logger = logging.getLogger(__name__)
 
-# TODO: implement checking for complex-valued filters somewhere (pyfda_lib?),
-#       h[n] detects complex data (although it isn't)
 # TODO: Fixpoint coefficients do not properly convert complex -> float when saving
 #       the filter?
 # TODO: This ItemDelegate method displayText is called again and again when an
 #        item is selected?!
 # TODO: negative values for WI don't work correctly
 #
 # TODO: Filters need to be scaled properly, see e.g.
@@ -70,16 +68,16 @@
     def __init__(self, parent):
         """
         Pass instance `parent` of parent class (Input_Coeffs)
         """
         super(ItemDelegate, self).__init__(parent)
         self.parent = parent  # instance of the parent (not the base) class
         # handles to quantization objects (fx.Fixed() instance) of coefficient widgets
-        self.QObj = [self.parent.ui.wdg_wq_coeffs_b.QObj,
-                     self.parent.ui.wdg_wq_coeffs_a.QObj]
+        self.Q = [self.parent.ui.wdg_wq_coeffs_b.Q,
+                     self.parent.ui.wdg_wq_coeffs_a.Q]
 
 # ==============================================================================
 #     def paint(self, painter, option, index):
 #         """
 #         Override painter
 #
 #         painter: instance of QPainter
@@ -95,15 +93,15 @@
 #             #     painter.setPen(option.palette.color( QPalette.Active, QPalette.Dark ))
 #             painter.drawLine(option.rect.left(), y, option.rect.right(), y )
 #         else:
 #             # continue with the original `paint()` method
 #             super(ItemDelegate, self).paint(painter, option, index)
 #             #painter.restore()
 # ----------------------------------
-#         logger.debug("Ovr_flag:".format(self.parent.self.QObj[0].ovr_flag))
+#         logger.debug("Ovr_flag:".format(self.parent.self.Q[0].ovr_flag))
 #         #option.backgroundBrush = QBrush(QColor(000, 100, 100, 200)) # lightGray
 #             #option.backgroundBrush.setColor(QColor(000, 100, 100, 200))
 #         # continue with the original `paint()` method
 #         #option.palette.setColor(QPalette.Window, QColor(Qt.red))
 #         #option.palette.setColor(QPalette.Base, QColor(Qt.green))
 #         super(ItemDelegate, self).paint(painter, option, index)
 #
@@ -145,24 +143,24 @@
     def displayText(self, text, locale) -> str:
         """
         Display `text` with selected fixpoint base and number of places
 
         text:   string / QVariant from QTableWidget to be rendered
         locale: locale for the text
 
-        The instance parameter `QObj[c].ovr_flag` is set to +1 or -1 for
+        The instance parameter `Q[c].ovr_flag` is set to +1 or -1 for
          positive / negative overflows, else it is 0.
         """
 
-        if fb.fil[0]['fxqc']['QCB']['fx_base'] == 'float':
+        if not fb.fil[0]['fx_sim']:
             data = safe_eval(text, return_type='auto')  # convert to float
             return "{0:.{1}g}".format(data, params['FMT_ba'])
 
-        elif fb.fil[0]['fxqc']['QCB']['fx_base'] == 'dec':
-            return "{0:>{1}}".format(text, self.QObj[0].q_dict['places'])
+        elif fb.fil[0]['fx_base'] == 'dec':
+            return "{0:>{1}}".format(text, self.Q[0].places)
 
         else:
             return text
 # see:
 # http://stackoverflow.com/questions/30615090/pyqt-using-qtextedit-as-editor-in-a-qstyleditemdelegate
 
     # -------------------------------------------------------------------------
@@ -188,68 +186,76 @@
         - retrieve data with full accuracy from self.ba (in float format)
         - requantize data according to settings in fixpoint object
         - represent it in the selected format (int, hex, ...)
 
         editor: instance of e.g. QLineEdit
         index:  instance of QModelIndex
         """
-        data_str = str(safe_eval(self.parent.ba[index.column()][index.row()],
-                                 return_type="auto"))
-        if self.QObj[index.column()].q_dict['fx_base'] == 'float':
-            # floating point format: pass data with full resolution
-            editor.setText(data_str)
-        else:
+        data = safe_eval(self.parent.ba[index.column()][index.row()],
+                         return_type="auto")
+
+        if fb.fil[0]['fx_sim']:
             # fixpoint format with base:
             # pass requantized data with required number of decimal places
             editor.setText(
-                "{0:>{1}}".format(self.QObj[index.column()].float2frmt(data_str),
-                                  self.QObj[index.column()].q_dict['places']))
+                "{0:>{1}}".format(self.Q[index.column()].float2frmt(data),
+                                  self.Q[index.column()].places))
+        else:
+            # floating point format: pass data with full resolution
+            editor.setText(str(data))
 
     # -------------------------------------------------------------------------
     def setModelData(self, editor, model, index) -> None:
         """
         When editing has finished, read the updated data from the editor (= QTableWidget),
-        convert it back to floating point format and store it in `self.ba` as float via
-        `float2frmt()`. Next, convert it back to fixpoint format via `frmt2float()`  and
-        store it in `self.ba_q`. Finally, refresh the table item to
-        display it in the selected format via `_refresh_table_item()`.
+        and store it in `self.ba` as float / complex for `fb.fil[0]['fx_sim'] == False`.
+
+        For all other formats, convert data back to floating point format via
+        `frmt2float()` and store it in `self.ba` as float / complex. Next, use
+        `float2frmt()` to quantize data and and store it in `parent.ba_q`.
+        Finally, refresh the table item to display it in the selected format via
+        `_refresh_table_item()`.
 
         editor: instance of e.g. QLineEdit
         model:  instance of QAbstractTableModel
         index:  instance of QModelIndex
         """
 
         # check for different editor environments if needed and provide a default:
 #        if isinstance(editor, QtGui.QTextEdit):
 #            model.setData(index, editor.toPlainText())
 #        elif isinstance(editor, QComboBox):
 #            model.setData(index, editor.currentText())
 #        else:
 #            super(ItemDelegate, self).setModelData(editor, model, index)
-        if self.QObj[index.column()].q_dict['fx_base'] == 'float':
+        if not fb.fil[0]['fx_sim']:
             data = safe_eval(
                 str(editor.text()), self.parent.ba[index.column()][index.row()],
-                return_type='auto')  # raw data without fixpoint formatting
-            data_q = data  # TODO: complex data
-        else:   # fixpoint format, transform to float
-            data = self.QObj[index.column()].frmt2float(
-                str(editor.text()), self.QObj[index.column()].q_dict['fx_base'])
-            data_q = self.QObj[index.column()].float2frmt(data)
+                return_type='auto')  # raw float data without fixpoint formatting
+            data_q = data
+        else:
+            # fixpoint format: read editor string and transform to float (`data`)
+            # convert `data` to fixpoint format as `data_q`
+            data = self.Q[index.column()].frmt2float(str(editor.text()))
+            data_q = self.Q[index.column()].float2frmt(data)
 
-        # model.setData(index, data)                          # store in QTableWidget
-        # if data is complex, convert whole ba (list of arrays) to complex type
         if isinstance(data, complex):
+            # if data is complex, convert whole column (b or a array) to complex
             self.parent.ba[index.column()] = self.parent.ba[index.column()].astype(complex)
+        if isinstance(data_q, complex):
+            # if data_q is complex, convert whole column (b or a array) to complex
             self.parent.ba_q[index.column()] = self.parent.ba_q[index.column()].astype(complex)
-
         # store new data in self.ba and ba_q
         self.parent.ba[index.column()][index.row()] = data
         self.parent.ba_q[index.column()][index.row()] = data_q
+        # logger.error(f"data_q: {data_q}")
         qstyle_widget(self.parent.ui.butSave, 'changed')
-        self.parent._refresh_table_item(index.row(), index.column())  # refresh table item
+        # this is needed to adapt text width to e.g. complex number representation
+        self.parent.refresh_table()
+        # self.parent._refresh_table_item(index.row(), index.column())  # refresh table item
 
 ###############################################################################
 
 
 class Input_Coeffs(QWidget):
     """
     Create widget with a (sort of) model-view architecture for viewing /
@@ -280,51 +286,50 @@
 
         self.data_changed = True  # initialize flag: filter data has been changed
         self.fx_specs_changed = True  # fixpoint specs have been changed outside
 
         self.ui = Input_Coeffs_UI(self)  # create the UI part with buttons etc.
 
         # handles to quantization objects (`fx.Fixed()` instances) of coefficient widgets
-        self.QObj = [self.ui.wdg_wq_coeffs_b.QObj,
-                     self.ui.wdg_wq_coeffs_a.QObj]
+        self.Q = [self.ui.wdg_wq_coeffs_b.Q,
+                     self.ui.wdg_wq_coeffs_a.Q]
 
         self._construct_UI()
 
     # -------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from sig_rx
         """
-        logger.debug("process_sig_rx(): vis={0}\n{1}"\
-                     .format(self.isVisible(), pprint_log(dict_sig)))
+        # logger.warning(f"SIG_RX: vis={self.isVisible()}\n{pprint_log(dict_sig)}")
 
         if dict_sig['id'] == id(self):
             # logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'ui_global_changed' in dict_sig\
                 and dict_sig['ui_global_changed'] == 'csv':
             # CSV options have been changed, update icons (file vs. clipboard)
             self.ui._set_load_save_icons()
 
-        elif 'ui_local_changed' in dict_sig and 'wdg_name' in dict_sig and\
-                dict_sig['wdg_name'] in {'wq_coeffs_a', 'wq_coeffs_b'}:
+        elif 'ui_local_changed' in dict_sig and 'sender_name' in dict_sig and\
+                dict_sig['sender_name'] in {'fx_ui_wq_coeffs_a', 'fx_ui_wq_coeffs_b'}:
             # local events from UI, trigger requant and refresh table
             self.refresh_table()
             self.emit({'fx_sim': 'specs_changed'})
             return
 
         elif self.isVisible():
             if self.data_changed or 'data_changed' in dict_sig:
                 self.load_dict()
                 self.data_changed = False
             if self.fx_specs_changed or\
                     ('fx_sim' in dict_sig and dict_sig['fx_sim'] == 'specs_changed'):
                 # global event, update widget dicts and table
-                self.qdict2ui()
+                self.dict2ui()
                 self.fx_specs_changed = False
         else:
             # TODO: draw wouldn't be necessary for 'view_changed', only update view
             # TODO: what is emitted when fixpoint formats are changed?
             if 'data_changed' in dict_sig:
                 self.data_changed = True
             elif 'fx_sim' in dict_sig and dict_sig['fx_sim'] == 'specs_changed':
@@ -371,30 +376,30 @@
         # LOCAL (UI) SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         # wdg.textChanged() is emitted when contents of widget changes
         # wdg.textEdited() is only emitted for user changes
         # wdg.editingFinished() is only emitted for user changes
         self.ui.spnDigits.editingFinished.connect(self.refresh_table)
 
-        self.ui.butFromTable.clicked.connect(self._export)
+        self.ui.butFromTable.clicked.connect(self.export_table)
         self.ui.butToTable.clicked.connect(self._import)
 
         self.ui.cmbFilterType.currentIndexChanged.connect(self._filter_type)
 
         self.ui.butDelCells.clicked.connect(self._delete_cells)
         self.ui.butAddCells.clicked.connect(self._add_cells)
         self.ui.butLoad.clicked.connect(self.load_dict)
         self.ui.butSave.clicked.connect(self._save_dict)
         self.ui.butClear.clicked.connect(self.clear_table)
         self.ui.ledEps.editingFinished.connect(self._set_eps)
         self.ui.butSetZero.clicked.connect(self._set_coeffs_zero)
 
         # store new settings and refresh table
-        self.ui.cmb_fx_base.currentIndexChanged.connect(self.fx_base2qdict)
-        self.ui.cmb_q_frmt.currentIndexChanged.connect(self.qfrmt2qdict)
+        self.ui.cmb_fx_base.currentIndexChanged.connect(self.fx_base2dict)
+        self.ui.cmb_qfrmt.currentIndexChanged.connect(self.qfrmt2dict)
 
         self.ui.wdg_wq_coeffs_a.sig_tx.connect(self.process_sig_rx)
         self.ui.wdg_wq_coeffs_b.sig_tx.connect(self.process_sig_rx)
 
         self.ui.but_quant.clicked.connect(self.quant_coeffs_save)
 
         self.ui.sig_tx.connect(self.sig_tx)
@@ -404,93 +409,98 @@
         """
         This method only creates a view on the quantized coefficients and stores
         it in `self.ba_q`, the actual coefficients in `self.ba` remain unchanged!
 
         * Reset overflow counters
 
         * Quantize filter coefficients `self.ba` with quantizer objects
-          `self.QObj[0]` and `self.QObj[1]` for `b` and `a` coefficients respectively
+          `self.Q[0]` and `self.Q[1]` for `b` and `a` coefficients respectively
           and store them in the array `self.ba_q`. Depending on the number base
           (float, dec, hex, ...) the result can be of type float or string.
 
         *  Store pos. / neg. overflows in the 3rd and 4th column of `self.ba_q` as
            0 or +/- 1.
         """
-        self.QObj[0].resetN()
-        self.QObj[1].resetN()
+
+        # Reset overflow counters of quantization objects
+        self.Q[0].resetN()
+        self.Q[1].resetN()
 
         if np.isscalar(self.ba[0]) or np.isscalar(self.ba[1]):
             logger.error("No proper filter, coefficients are scalar!")
             return
 
         len_b = len(self.ba[0])
         len_a = len(self.ba[1])
 
-        # Create a copy of the a coefficients without the "1" as this could create
+        # Create a copy of the 'a' coefficients without the "1" as this could create
         # false overflows during quantization. The "1" is always printed though
         # by the `ItemDelegate.initStyleOption()` method
-        #
-        # TODO: Replacing the first element by 0  doesn't work, a is always converted
-        # to integer for non-dec formats somehwhere - Why???
 
-        # logger.error(f"ba[1]: {self.ba[1].dtype}")
-        a = np.concatenate(([0.123], self.ba[1][1:]))
+        a = np.concatenate(([0.], self.ba[1][1:]))
+        # self.ba[1][0] = 0  # Is this safe?
         # a = self.ba[1]
-        # logger.error(f"a: {a.dtype}")
+        # logger.error(f"a: {a[1].dtype}")
 
-        if fb.fil[0]['fxqc']['QCB']['fx_base'] == 'float':
+        # Float format: Set ba_q = ba, overflows are all = 0
+        if not fb.fil[0]['fx_sim']:
             self.ba_q = [self.ba[0],
                          self.ba[1],
                          np.zeros(len_b),
                          np.zeros(len_a),
                          ]
-        elif fb.fil[0]['fxqc']['QCB']['fx_base'] == 'dec':
+        # Fixpoint decimal format: Print coefficients in numeric format
+        # with a defined number of places
+        elif fb.fil[0]['fx_base'] == 'dec':
             self.ba_q = [
-                ["{0:>{1}}".format(x, self.QObj[0].q_dict['places'])
-                    for x in self.QObj[0].float2frmt(self.ba[0])],
-                ["{0:>{1}}".format(x, self.QObj[0].q_dict['places'])
-                    for x in self.QObj[1].float2frmt(a)],
-                self.QObj[0].q_dict['ovr_flag'],
-                self.QObj[1].q_dict['ovr_flag']
+                ["{0:>{1}}".format(x, self.Q[0].places)
+                    for x in self.Q[0].float2frmt(self.ba[0])],
+                ["{0:>{1}}".format(x, self.Q[1].places)
+                    for x in self.Q[1].float2frmt(a)],
+                self.Q[0].ovr_flag,
+                self.Q[1].ovr_flag
                         ]
+        # Other fixpoint formats: Print coefficients as strings
         else:
             self.ba_q = [
-                self.QObj[0].float2frmt(self.ba[0]),
-                self.QObj[1].float2frmt(a),
-                self.QObj[0].q_dict['ovr_flag'],
-                self.QObj[1].q_dict['ovr_flag']
+                self.Q[0].float2frmt(self.ba[0]),
+                self.Q[1].float2frmt(a),
+                self.Q[0].ovr_flag,
+                self.Q[1].ovr_flag
                         ]
-        self.ui.wdg_wq_coeffs_b.update_disp()
-        self.ui.wdg_wq_coeffs_a.update_disp()
+        # convert self.ba_q to list of arrays for easier handling
+        self.ba_q = [np.asarray(self.ba_q[i]) for i in range(4)]
+        self.ui.wdg_wq_coeffs_b.update_ovfl_cnt()
+        self.ui.wdg_wq_coeffs_a.update_ovfl_cnt()
 
 # ------------------------------------------------------------------------------
     def quant_coeffs_save(self):
         """
+        Triggered by pushing "Quantize button":
         - Store selected / all quantized coefficients in `self.ba`
         - Refresh table (for the case that anything weird happens during quantization)
         - Reset Overflow flags `self.ba_q[2]` and `self.ba_q[3]`
         - Save quantized `self.ba` to filter dict (in `_save_dict()`). This emits
           {'data_changed': 'input_coeffs'}
         """
         idx = qget_selected(self.tblCoeff)['idx']  # get all selected indices
         # returns e.g. [[0, 0], [0, 6]]
-
         if not idx:  # nothing selected, quantize all elements
-            self.ba[0] = self.QObj[0].frmt2float(self.ba_q[0])
-            self.ba[1] = self.QObj[1].frmt2float(self.ba_q[1])
+            self.ba[0] = self.Q[0].frmt2float(self.ba_q[0])
+            self.ba[1] = self.Q[1].frmt2float(self.ba_q[1])
             self.ba_q[2] = np.zeros(len(self.ba_q[0]))
             self.ba_q[3] = np.zeros(len(self.ba_q[1]))
             # idx = [[j, i] for i in range(self.num_rows) for j in range(self.num_cols)]
         else:
             try:
                 idx.remove([1, 0])  # don't process '1' of recursive filters
             except ValueError:
                 pass
             for i in idx:
-                self.ba[i[0]][i[1]] = self.QObj[i[0]].frmt2float(self.ba_q[i[0]][i[1]])
+                self.ba[i[0]][i[1]] = self.Q[i[0]].frmt2float(self.ba_q[i[0]][i[1]])
                 self.ba_q[i[0] + 2][i[1]] = 0
 
         self.refresh_table()
         # qstyle_widget(self.ui.butSave, 'changed')
         self._save_dict()
 
     # --------------------------------------------------------------------------
@@ -539,32 +549,32 @@
             item = QTableWidgetItem(str(self.ba_q[col][row]).strip('()'))
             self.tblCoeff.setItem(row, col, item)
 
         brush = QBrush(Qt.SolidPattern)
         brush.setColor(QColor(255, 255, 255, 0))  # transparent white
 
         if self.ba_q[col + 2][row] > 0:
-            # Color item backgrounds with pos. Overflows red
+            # Color item backgrounds with pos. overflows in red
             brush.setColor(QColor(100, 0, 0, 80))
 
         elif self.ba_q[col + 2][row] < 0:
-            # Color item backgrounds with neg. Overflows blue
+            # Color item backgrounds with neg. overflows in blue
             brush.setColor(QColor(0, 0, 100, 80))
 
         item.setTextAlignment(Qt.AlignRight | Qt.AlignCenter)
         item.setBackground(brush)
 
     # --------------------------------------------------------------------------
     def refresh_table(self):
         """
         Update `self.ba_q` from `self.ba` (list with 2 one-dimensional numpy arrays),
         i.e. requantize displayed values (not `self.ba`) and overflow counters.
 
         Refresh the table from it. Data is displayed via `ItemDelegate.displayText()` in
-        the number format set by `self.q_dict['fx_base']`.
+        the number format set by `fb.fil[0]['fx_base']`.
 
         - self.ba[0] -> b coefficients
         - self.ba[1] -> a coefficients
 
         The table dimensions are set according to the filter type set in
         `fb.fil[0]['ft']` which is either 'FIR' or 'IIR' and by the number of
         rows in `self.ba`.
@@ -576,18 +586,19 @@
         self.quant_coeffs_view()
         if np.ndim(self.ba) == 1 or fb.fil[0]['ft'] == 'FIR':
             self.num_rows = len(self.ba[0])
         else:
             self.num_rows = max(len(self.ba[1]), len(self.ba[0]))
 
         # When format is 'float', disable all fixpoint options and widgets:
-        is_float = (qget_cmb_box(self.ui.cmb_fx_base, data=False).lower() == 'float')
+        is_float = (qget_cmb_box(self.ui.cmb_qfrmt) == 'float')
         self.ui.spnDigits.setVisible(is_float)  # select number of float digits
         self.ui.lblDigits.setVisible(is_float)
-        self.ui.frm_q_frmt.setVisible(not is_float)  # hide quantization widgets
+        self.ui.cmb_fx_base.setVisible(not is_float)  # hide fx base combobosx
+        self.ui.but_quant.setVisible(not is_float)  # hide quantization button
 
         # hide all q-settings for float
         self.ui.wdg_wq_coeffs_b.setVisible(not is_float)
 
         # check whether filter is FIR and only needs one column
         if fb.fil[0]['ft'] == 'FIR':
             self.num_cols = 1
@@ -637,63 +648,64 @@
           counter
         - Update the display via `self.refresh_table()`.
 
         The filter dict is a "normal" 2D-numpy float array for the b and a coefficients
         while the coefficient list `self.ba` is a list of two float ndarrays to allow
         for different lengths of b and a subarrays while adding / deleting items.
         """
-        self.ba = list(fb.fil[0]['ba'].copy())
+        self.ba = list(fb.fil[0]['ba']).copy()
 
         # set quantization UI from dictionary, update quantized coeff. display and
         # overflow counter, and refresh table
-        self.qdict2ui()
+        self.dict2ui()
 
         qstyle_widget(self.ui.butSave, 'normal')
+ 
 
     # --------------------------------------------------------------------------
-    def _export(self):
+    def export_table(self):
         """
         Export data from coefficient table `self.tblCoeff` to clipboard / file in
         CSV format.
         """
-        if not params['CSV']['cmsis']:
-            text = qtable2csv(
-                self.tblCoeff, self.ba, formatted=self.ui.but_format.isChecked())
-            if params['CSV']['clipboard']:  # clipboard is selected as export target
-                fb.clipboard.setText(text)
-            else:
-                # pass csv formatted text, key for accessing data in ``*.npz`` file or
-                # Matlab workspace (``*.mat``) and a title for the file export dialog
-                save_data_csv(self, text, 'ba', title="Export Filter Coefficients")
-
-        elif fb.fil[0]['ft'] != 'IIR':
-            logger.warning("CMSIS SOS export is only possible for IIR filters!")
-        else:
-            # Get coefficients in SOS format and delete 4th column containing the
-            # '1.0' of the recursive parts:
-            sos_coeffs = np.delete(fb.fil[0]['sos'], 3, 1)
-            # TODO: check `scipy.signal.zpk2sos` for details concerning sos paring
-
-            delim = params['CSV']['delimiter'].lower()
-            if delim == 'auto':  # 'auto' doesn't make sense when exporting
-                delim = ","
-            cr = params['CSV']['lineterminator']
-
-            text = ""
-            for r in range(np.shape(sos_coeffs)[0]):  # number of rows
-                for c in range(5):  # always has 5 columns
-                    text += str(safe_eval(sos_coeffs[r][c], return_type='auto')) + delim
-                text = text.rstrip(delim) + cr
-            text = text.rstrip(cr)  # delete last CR
-
-            if params['CSV']['clipboard']:
-                fb.clipboard.setText(text)
-            else:
-                save_data_csv(self, text, title="Export in CMSIS DSP SOS format",
-                                file_types=('csv',))
+        text = qtable2csv(
+            self.tblCoeff, self.ba, formatted=self.ui.but_format.isChecked())
+        if params['CSV']['destination'] == 'clipboard':
+            # clipboard is selected as export target
+            fb.clipboard.setText(text)
+        else:
+            # pass csv formatted text, key for accessing data in ``*.npz`` file or
+            # Matlab workspace (``*.mat``) and a title for the file export dialog
+            export_fil_data(self, text, 'ba', title="Export Filter Coefficients")
+
+        # elif fb.fil[0]['ft'] != 'IIR':
+        #     logger.warning("CMSIS SOS export is only possible for IIR filters!")
+        # else:
+        #     # Get coefficients in SOS format and delete 4th column containing the
+        #     # '1.0' of the recursive parts:
+        #     sos_coeffs = np.delete(fb.fil[0]['sos'], 3, 1)
+        #     # TODO: check `scipy.signal.zpk2sos` for details concerning sos paring
+
+        #     delim = params['CSV']['delimiter'].lower()
+        #     if delim == 'auto':  # 'auto' doesn't make sense when exporting
+        #         delim = ","
+        #     cr = params['CSV']['lineterminator']
+
+        #     text = ""
+        #     for r in range(np.shape(sos_coeffs)[0]):  # number of rows
+        #         for c in range(5):  # always has 5 columns
+        #             text += str(safe_eval(sos_coeffs[r][c], return_type='auto')) + delim
+        #         text = text.rstrip(delim) + cr
+        #     text = text.rstrip(cr)  # delete last CR
+
+        #     if params['CSV']['clipboard']:
+        #         fb.clipboard.setText(text)
+        #     else:
+        #         export_fil_data(self, text, title="Export in CMSIS DSP SOS format",
+        #                         file_types=('csv',))
 
     # --------------------------------------------------------------------------
     def _import(self) -> None:
         """
         Import data from clipboard / file and copy it to `self.ba` as float / cmplx.
 
         Quantize data to `self.ba_q` and refresh table.
@@ -704,15 +716,14 @@
         # get data as ndarray of str
         data_str = data2array(self, 'ba', title="Import Filter Coefficients",
                               as_str = self.ui.but_format.isChecked())
         if data_str is None:  # file operation has been aborted or some other error
             logger.info(f"Data was not imported.")
             return
 
-        frmt = self.QObj[0].q_dict['fx_base']
 
         if np.ndim(data_str) > 1:
             num_cols, num_rows = np.shape(data_str)
             orientation_horiz = num_cols > num_rows  # need to transpose data
             if min(num_cols, num_rows) > 2:
                 logger.error(
                     f"Data cannot be imported, its shape is {num_cols} x {num_rows}.")
@@ -727,38 +738,38 @@
             return
 
         self.ba = [[], []]
         if orientation_horiz:
             for c in range(num_cols):
                 if formatted_import:
                     self.ba[0].append(
-                        self.QObj[0].frmt2float(data_str[c][0], frmt))
+                        self.Q[0].frmt2float(data_str[c][0]))
                     if num_rows > 1:
                         self.ba[1].append(
-                            self.QObj[1].frmt2float(data_str[c][1], frmt))
+                            self.Q[1].frmt2float(data_str[c][1]))
                 else:
                     self.ba[0].append(data_str[c][0])
                     if num_rows > 1:
                         self.ba[1].append(data_str[c][1])
             if num_rows > 1:
                 self._filter_type(ftype='IIR')
             else:
                 self.ba[1] = zeros_with_val(len(self.ba[0]))
                 self._filter_type(ftype='FIR')
         else:
             if formatted_import:
                 self.ba[0] =\
-                    [self.QObj[0].frmt2float(s, frmt) for s in data_str[0]]
+                    [self.Q[0].frmt2float(s) for s in data_str[0]]
             else:
                 self.ba[0] = data_str[0]
             # IIR
             if num_cols > 1:
                 if formatted_import:
                     self.ba[1] =\
-                        [self.QObj[1].frmt2float(s, frmt) for s in data_str[1]]
+                        [self.Q[1].frmt2float(s) for s in data_str[1]]
                 else:
                     self.ba[1] = data_str[1]
                 self._filter_type(ftype='IIR')
             else:
                 self.ba[1] = zeros_with_val(len(self.ba[0]))
                 self._filter_type(ftype='FIR')
 
@@ -770,86 +781,76 @@
 
         self._equalize_ba_length()
         self.refresh_table()
         logger.info(f"Successfully imported data.")
         qstyle_widget(self.ui.butSave, 'changed')
 
     # --------------------------------------------------------------------------
-    def qdict2ui(self):
+    def dict2ui(self):
         """
-        - set the UI from the quantization dict
+        - update the UI from the dictionary
         - Update the fixpoint quant. object
         - Update the quantized coefficient view and the overflow counter
         - Refresh the table
 
         Triggered by:
         - `process_sig_rx()`: self.fx_specs_changed == True or
                                 dict_sig['fx_sim'] == 'specs_changed'
-        - `self.qfrmt2qdict()`
-        - `self.fx_base2qdict()`
+        - `self.qfrmt2dict()`
+        - `self.fx_base2dict()`
 
         """
-        if self.ui.wdg_wq_coeffs_b.q_dict['WI'] != 0\
-                and self.ui.wdg_wq_coeffs_b.q_dict['WF'] != 0:
-            qset_cmb_box(self.ui.cmb_q_frmt, 'qfrac', data=True)
+        # update ui
+        if not fb.fil[0]['fx_sim']:  # float mode
+            qset_cmb_box(self.ui.cmb_qfrmt, 'float', data=True)
+        else:  # fixpoint mode
+            qset_cmb_box(self.ui.cmb_qfrmt, fb.fil[0]['qfrmt'], data=True)
 
         # update quantizer objects and widgets
-        self.ui.wdg_wq_coeffs_a.dict2ui()
-        self.ui.wdg_wq_coeffs_b.dict2ui()
-
-        # qset_cmb_box(self.ui.cmb_q_frmt, self.ui.wdg_wq_coeffs_b.q_dict['qfrmt'])
-        # qset_cmb_box(self.ui.cmb_fx_base, self.ui.wdg_wq_coeffs_b.q_dict['fx_base'])
+        self.ui.wdg_wq_coeffs_a.dict2ui(fb.fil[0]['fxq']['QCA'])
+        self.ui.wdg_wq_coeffs_b.dict2ui(fb.fil[0]['fxq']['QCB'])
 
+        # quantize coefficient view according to new settings and update table
         self.quant_coeffs_view()
         self.refresh_table()
 
 # ------------------------------------------------------------------------------
-    def qfrmt2qdict(self):
+    def qfrmt2dict(self):
         """
-        Read out the UI settings of  `self.ui.cmb_q_frmt` (triggering this method)
-        and store the old 'qfrmt' setting under the 'qfrmt_last' key.
-
-        The coefficient quantization settings are copied to the quantization dicts
-        fb.fil[0]['fxqc']['QCB']` and `...['QCA']` inside the quantization widget
-        instances of `FX_UI_WQ` every time something is updated there. This information
-        is also kept in the quantization objects `QObj` of the quantization widgets.
+        Read out the UI settings of  `self.ui.cmb_qfrmt` (triggering this method)
+        and store it under the 'qfrmt' key if it is a fixpoint format. Set the
+        `fb.fil[0]['fx_sim']` flag accordingly.
 
         Refresh the table and update quantization widgets, finally emit a signal
         `{'fx_sim': 'specs_changed'}`.
         """
-        fb.fil[0]['fxqc']['QCB'].update(
-            {'qfrmt_last': fb.fil[0]['fxqc']['QCB']['qfrmt'],
-             'qfrmt': qget_cmb_box(self.ui.cmb_q_frmt)})
-        fb.fil[0]['fxqc']['QCA'].update(
-            {'qfrmt_last': fb.fil[0]['fxqc']['QCA']['qfrmt'],
-             'qfrmt': qget_cmb_box(self.ui.cmb_q_frmt)})
-
-        # update quant. widgets and table with the new `qfrmt` settings
-        self.qdict2ui()
+        qfrmt = qget_cmb_box(self.ui.cmb_qfrmt)
+        fb.fil[0]['fx_sim'] = (qfrmt != 'float')
+        if qfrmt != 'float':
+            fb.fil[0]['qfrmt'] = qfrmt
+
+        # update quant. widgets and table with the new `qfrmt` settings and propagate
+        # change in fixpoint settings to other widgets
+        self.dict2ui()
         self.emit({'fx_sim': 'specs_changed'})
 
 # ------------------------------------------------------------------------------
-    def fx_base2qdict(self):
+    def fx_base2dict(self):
         """
         Read out the UI settings of `self.ui.cmb_fx_base` (triggering this method)
-        which specifies the number base (dec, bin, ...)
-
-        The coefficient quantization settings are copied to the quantization dicts
-        fb.fil[0]['fxqc']['QCB']` and `...['QCA']` inside the quantization widget
-        instances of `FX_UI_WQ` every time something is updated there. This information
-        is also kept in the quantization objects `QObj` of the quantization widgets.
+        which specifies the fx number base (dec, bin, ...) for display
+        and store it in `fb.fil[0]['fx_base'].
 
         Refresh the table and update quantization widgets. Don't emit a signal
         because this only influences the view not the data itself.
         """
-        fb.fil[0]['fxqc']['QCB'].update({'fx_base': qget_cmb_box(self.ui.cmb_fx_base)})
-        fb.fil[0]['fxqc']['QCA'].update({'fx_base': qget_cmb_box(self.ui.cmb_fx_base)})
+        fb.fil[0]['fx_base'] = qget_cmb_box(self.ui.cmb_fx_base)
 
         # update quant. widgets and table with the new `fx_base` settings
-        self.qdict2ui()
+        self.dict2ui()
 
 # ------------------------------------------------------------------------------
     def _save_dict(self):
         """
         Save the coefficient register `self.ba` to the filter dict `fb.fil[0]['ba']`.
         """
         logger.debug("_save_dict called")
@@ -927,26 +928,28 @@
 
         if not any(sel) and len(self.ba[0]) > 0:  # nothing selected, delete last row
             self.ba = np.delete(self.ba, -1, axis=1)
         elif np.all(sel[0] == sel[1]) or fb.fil[0]['ft'] == 'FIR':
             # only complete rows selected or FIR -> delete row
             self.ba = np.delete(self.ba, sel[0], axis=1)
         else:
-            self.ba[0][sel[0]] = 0
-            self.ba[1][sel[1]] = 0
-            # self.ba[0] = np.delete(self.ba[0], sel[0])
-            # self.ba[1] = np.delete(self.ba[1], sel[1])
-        # test and equalize if b and a array have different lengths:
-        self._equalize_ba_length()
-        self.refresh_table()
-        # if length is less than 2, clear the table: this ain't no filter!
-        if len(self.ba[0]) < 2:
-            self.clear_table()  # sets 'changed' attribute
-
-        qstyle_widget(self.ui.butSave, 'changed')
+            # self.ba[0][sel[0]] = 0
+            # self.ba[1][sel[1]] = 0
+            self.ba[0] = np.delete(self.ba[0], sel[0])
+            self.ba[1] = np.delete(self.ba[1], sel[1])
+
+        # If length is less than 2, re-initialize the table: this ain't no filter!
+        # `_clear_table() also refreshes the table and sets 'changed' attribute
+        if len(self.ba[0]) < 2 and len(self.ba[1]) < 2:
+            self.clear_table()
+        else:
+            # test and equalize if b and a array have different lengths:
+            self._equalize_ba_length()
+            self.refresh_table()
+            qstyle_widget(self.ui.butSave, 'changed')
 
 # ------------------------------------------------------------------------------
     def _add_cells(self):
         """
         Add the number of selected rows to self.ba and fill new cells with
         zeros from the bottom. If nothing is selected, add one row at the bottom.
         Refresh QTableWidget.
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_coeffs_ui.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_coeffs_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     pyqtSignal, Qt, QtGui, QWidget, QLabel, QLineEdit, QComboBox, QPushButton, QFrame,
     QSpinBox, QFont, QIcon, QVBoxLayout, QHBoxLayout, QGridLayout, QSizePolicy)
 from pyfda.libs.pyfda_lib import to_html
 
 from pyfda.libs.pyfda_qt_lib import (
     qset_cmb_box, qstyle_widget, qcmb_box_populate, QHLine, PushButton)
 from pyfda.libs.csv_option_box import CSV_option_box
-# from pyfda.libs.pyfda_lib import pprint_log
+from pyfda.libs.pyfda_lib import first_item
 import pyfda.libs.pyfda_dirs as dirs
 from pyfda.fixpoint_widgets.fx_ui_wq import FX_UI_WQ
 from pyfda.pyfda_rc import params
 import pyfda.filterbroker as fb
 
 import logging
 logger = logging.getLogger(__name__)
@@ -37,57 +37,59 @@
     from pyfda.libs.pyfda_qt_lib import emit
 
     def __init__(self, parent=None):
         super(Input_Coeffs_UI, self).__init__(parent)
         self.eps = 1.e-6  # initialize tolerance value
 
         self.cmb_q_frmt_items = [
-            "<span>Quantization format for signed fixpoint coefficients (affects only "
+            "<span>Quantization format for coefficients (affects only "
             "the display, not the stored values).</span>",
-            # ("float", "Float", "<span>Coefficients with full precision in floating "
-            # "point format</span>"),
-            ("qint", "Integer", "<span>Integer format with <i>WI</i> + 1 bits "
+            ('float', "Float", "<span>Full precision floating point format</span>"),
+            ('qint', "Integer", "<span>Integer format with <i>WI</i> + 1 bits "
              "(range -2<sup>WI</sup> ... 2<sup>WI</sup> - 1)</span>"),
-            ("qfrac", "Fractional",
+            ('qfrac', "Fractional",
              "<span>General fractional format with <i>WI</i> + <i>WF</i> + 1 bits "
-             "(range -2<sup>WI</sup> ... 2<sup>WI</sup> - 2<sup>WF</sup>).</span>"),
-            ("qnfrac", "Norm. Frac.",
-             "<span>Normalized fractional format with <i>WF</i> + 1 bits "
-             "(range -1 ... +1 - 2<sup>WF</sup>).</span>"),
-            ("q31", "Q31", "<span>Normalized fractional format with 32 bits "
-             "(31 fractional bits).</span>")
+             "(range -2<sup>WI</sup> ... 2<sup>WI</sup> - 2<sup>WF</sup>).</span>")
             ]
-        self.cmb_q_frmt_default = "qfrac"
+        self.cmb_q_frmt_default = "float"
 
         self.cmb_fx_base_items = [
-            "<span>Select the coefficient display format.</span>",
-            ("float", "Float", "<span>Coefficients with full precision in floating "
-             "point format</span>"),
-            ("dec", "Dec", "<span>Fixpoint coefficients in decimal format</span>"),
-            ("hex", "Hex", "<span>Fixpoint coefficients in hexadecimal format</span>"),
-            ("bin", "Bin", "<span>Fixpoint coefficients in binary format</span>"),
-            ("csd", "CSD", "<span>Fixpoint coefficients in Canonically Signed Digit "
+            "<span>Select the coefficient fixpoint display format.</span>",
+            # ("float", "Float", "<span>Coefficients with full precision in floating "
+            # "point format</span>"),
+            ('dec', "Dec", "<span>Fixpoint coefficients in decimal format</span>"),
+            ('hex', "Hex", "<span>Fixpoint coefficients in hexadecimal format</span>"),
+            ('bin', "Bin", "<span>Fixpoint coefficients in binary format</span>"),
+            ('oct', "Oct", "<span>Fixpoint coefficients in octal format</span>"),
+            ('csd', "CSD", "<span>Fixpoint coefficients in Canonically Signed Digit "
              "(ternary logic) format</span>")
             ]
-        self.cmb_fx_base_default = "float"
+        self.cmb_fx_base_default = "dec"
+
         self._construct_UI()
 
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from the CSV pop-up window
         """
-        # logger.debug("PROCESS_SIG_RX:\n{0}".format(pprint_log(dict_sig)))
-
-        if 'closeEvent' in dict_sig:
+        # logger.warning("PROCESS_SIG_RX:\n{0}".format(pprint_log(dict_sig)))
+        if dict_sig['id'] == id(self):
+            # this should not happen as the rx slot is not connected globally
+            logger.warning(
+                f'Stopped infinite loop: "{first_item(dict_sig)}"')
+            return
+        elif 'closeEvent' in dict_sig:
             self._close_csv_win()
+            # send signal that pop-up box is closed
             self.emit({'ui_global_changed': 'csv'})
-        elif 'ui_global_changed' in dict_sig:
+        elif 'ui_global_changed' in dict_sig and dict_sig['ui_global_changed'] == 'csv':
             self._set_load_save_icons()  # update icons file <-> clipboard
-            # set state of CSV options button according to state of CSV popup handle
+            # signal change of CSV options to other widgets with current id
+            self.emit({'ui_global_changed': 'csv'})
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the widget, consisting of:
         - top chkbox row
         - coefficient table
@@ -106,40 +108,30 @@
         # This frame contains all the buttons
         #######################################################################
         # ---------------------------------------------
         #
         # UI Elements for controlling the display
         # ---------------------------------------------
 
+        self.cmb_qfrmt = QComboBox(self)
+        qcmb_box_populate(self.cmb_qfrmt, self.cmb_q_frmt_items,
+                          self.cmb_q_frmt_default)
+        self.cmb_qfrmt.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+
         self.cmb_fx_base = QComboBox(self)
         qcmb_box_populate(self.cmb_fx_base, self.cmb_fx_base_items,
                           self.cmb_fx_base_default)
 
-        model = self.cmb_fx_base.model()
-        # create header "Fixpoint:" between separators
-        item = QtGui.QStandardItem('Fixpoint:')
-        item.setData('parent', Qt.AccessibleDescriptionRole)
-        item.setData(0, role=QtGui.QFont.Bold)
-        item.setFlags(item.flags() & Qt.ItemIsEnabled)  # | Qt.ItemIsSelectable))
-        model.insertRow(1, item)
-        self.cmb_fx_base.insertSeparator(1)
-        self.cmb_fx_base.insertSeparator(3)
-
         self.spnDigits = QSpinBox(self)
         self.spnDigits.setRange(0, 16)
         self.spnDigits.setValue(params['FMT_ba'])
         self.spnDigits.setToolTip("Number of digits to display.")
         self.lblDigits = QLabel("Digits", self)
         self.lblDigits.setFont(self.bifont)
 
-        self.cmb_q_frmt = QComboBox(self)
-        qcmb_box_populate(self.cmb_q_frmt, self.cmb_q_frmt_items,
-                          self.cmb_q_frmt_default)
-        self.cmb_q_frmt.setSizeAdjustPolicy(QComboBox.AdjustToContents)
-
         self.but_quant = QPushButton(self)
         self.but_quant.setToolTip(
             "<span>Quantize selected coefficients / whole table with specified "
             "settings and save to dict. This modifies the data, not only the view."
             "</span>")
         self.but_quant.setIcon(QIcon(':/quantize.svg'))
         # self.but_quant.setIconSize(q_icon_size)
@@ -150,28 +142,29 @@
         self.but_format.setToolTip(
             "<span>Load and save coefficients with the table format when activated, "
             "i.e. with the selected number of digits, in Hex, Binary etc.</span>"
             )
         self.but_format.setIconSize(q_icon_size)
         self.but_format.setCheckable(True)
 
-        layH_q_frmt = QHBoxLayout()
-        layH_q_frmt.addWidget(self.cmb_q_frmt)
-        layH_q_frmt.addWidget(self.but_quant)
-        layH_q_frmt.setContentsMargins(5, 0, 0, 0)  # 5 pixels extra left space
-        self.frm_q_frmt = QFrame(self)
-        self.frm_q_frmt.setLayout(layH_q_frmt)
+        # layH_q_frmt = QHBoxLayout()
+        # layH_q_frmt.addWidget(self.cmb_qfrmt)
+        # layH_q_frmt.addWidget(self.but_quant)
+        # layH_q_frmt.setContentsMargins(5, 0, 0, 0)  # 5 pixels extra left space
+        # self.frm_q_frmt = QFrame(self)
+        # self.frm_q_frmt.setLayout(layH_q_frmt)
 
         layH_display = QHBoxLayout()
         layH_display.setContentsMargins(*params['wdg_margins'])
         layH_display.setAlignment(Qt.AlignLeft)
-        layH_display.addWidget(self.cmb_fx_base)
+        layH_display.addWidget(self.cmb_qfrmt)
         layH_display.addWidget(self.spnDigits)
         layH_display.addWidget(self.lblDigits)
-        layH_display.addWidget(self.frm_q_frmt)
+        layH_display.addWidget(self.cmb_fx_base)
+        layH_display.addWidget(self.but_quant)
         layH_display.addWidget(self.but_format)
         layH_display.addStretch()
 
         self.frm_display = QFrame(self)
         self.frm_display.setLayout(layH_display)
 
         #######################################################################
@@ -179,16 +172,15 @@
         #
         # This frame contains all buttons for manipulating coefficients
         # -----------------------------------------------------------------
         # layH_buttons_coeffs1
         #
         # UI Elements for loading / storing / manipulating cells and rows
         # -----------------------------------------------------------------
-        self.cmbFilterType = QComboBox(self)
-        self.cmbFilterType.setObjectName("comboFilterType")
+        self.cmbFilterType = QComboBox(self, objectName="comboFilterType")
         self.cmbFilterType.setToolTip(
             "<span>Select between IIR and FIR filter for manual entry. "
             "Changing the type reloads the filter from the filter dict.</span>")
         self.cmbFilterType.addItems(["FIR", "IIR"])
         self.cmbFilterType.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.butAddCells = QPushButton(self)
@@ -229,15 +221,15 @@
         self.butFromTable = QPushButton(self)
         self.butFromTable.setIconSize(q_icon_size)
         self.butToTable = QPushButton(self)
         self.butToTable.setIconSize(q_icon_size)
 
         self.but_csv_options = PushButton(self, icon=QIcon(':/settings.svg'),
                                           checked=False)
-        self.but_csv_options.setIconSize(q_icon_size)
+        # self.but_csv_options.setIconSize(q_icon_size)
         self.but_csv_options.setToolTip(
             "<span>Select CSV format and whether "
             "to copy to/from clipboard or file.</span>")
 
         self._set_load_save_icons()  # initialize icon / button settings
 
         layH_buttons_coeffs1 = QHBoxLayout()
@@ -285,20 +277,20 @@
         # This frame encompasses all Quantization Settings
         self.frm_buttons_coeffs = QFrame(self)
         self.frm_buttons_coeffs.setLayout(layV_buttons_coeffs)
         #######################################################################
 
         # -------------------
         self.wdg_wq_coeffs_b = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QCB'], wdg_name='wq_coeffs_b',
+            fb.fil[0]['fxq']['QCB'], objectName='fx_ui_wq_coeffs_b',
             label='<b>Coeff. Quantization <i>b<sub>I.F&nbsp;</sub></i>:</b>',
             MSB_LSB_vis='max')
         # -------------------
         self.wdg_wq_coeffs_a = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QCA'], wdg_name='wq_coeffs_a',
+            fb.fil[0]['fxq']['QCA'], objectName='fx_ui_wq_coeffs_a',
             label='<b>Coeff. Quantization <i>a<sub>I.F&nbsp;</sub></i>:</b>',
             MSB_LSB_vis='max')
 
         #######################################################################
         # ########################  Main UI Layout ############################
         #######################################################################
 
@@ -351,15 +343,15 @@
 
     # ------------------------------------------------------------------------------
     def _set_load_save_icons(self):
         """
         Set icons / tooltipps for loading and saving data to / from file or
         clipboard depending on selected options.
         """
-        if params['CSV']['clipboard']:
+        if params['CSV']['destination'] == 'clipboard':
             self.butFromTable.setIcon(QIcon(':/to_clipboard.svg'))
             self.butFromTable.setToolTip(
                 "<span>Copy table to clipboard in float format with full precision "
                 "when the &lt;FORMAT&gt; button is not selected.<br>"
                 "Otherwise, copy the table as displayed.</span>")
 
             self.butToTable.setIcon(QIcon(':/from_clipboard.svg'))
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_fixpoint_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_fixpoint_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     Qt, QWidget, QPushButton, QComboBox, QFileDialog, QLabel, QPixmap,
     QVBoxLayout, QHBoxLayout, pyqtSignal, QFrame, QSizePolicy)
 
 import numpy as np
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
 import pyfda.libs.pyfda_dirs as dirs
-from pyfda.libs.pyfda_lib import qstr, pprint_log, first_item
-from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qstyle_widget
+from pyfda.libs.pyfda_lib import pprint_log, first_item
+from pyfda.libs.pyfda_qt_lib import (
+    qget_cmb_box, qstyle_widget, qcmb_box_populate, qset_cmb_box)
 from pyfda.fixpoint_widgets.fx_ui_wq import FX_UI_WQ
 from pyfda.pyfda_rc import params
 
 # when deltasigma module is present, add a corresponding entry to the combobox
 try:
     import deltasigma
     HAS_DS = True
@@ -42,225 +43,268 @@
 classes = {'Input_Fixpoint_Specs': 'Fixpoint'}  #: Dict with class name : display name
 
 
 class Input_Fixpoint_Specs(QWidget):
     """
     Create the widget that holds the dynamically loaded fixpoint filter UI
     """
-
-    # sig_resize = pyqtSignal()  # emit a signal when the image has been resized
     sig_rx_local = pyqtSignal(object)  # incoming from subwidgets -> process_sig_rx_local
     sig_rx = pyqtSignal(object)  # incoming, connected to input_tab_widget.sig_rx
     sig_tx = pyqtSignal(object)  # outcgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName="input_fixpoint_spec_inst"):
         super(Input_Fixpoint_Specs, self).__init__(parent)
     # def __init__(self) -> None:
     #    super().__init__()
 
+        self.setObjectName(objectName)
         self.tab_label = 'Fixpoint'
         self.tool_tip = ("<span>Select a fixpoint implementation for the filter,"
                          " simulate it or generate a Verilog netlist.</span>")
         self.parent = parent
-        self.fx_specs_changed = True  # fixpoint specs have been changed outside
+        self.fx_specs_changed = False
+        self.fx_filt_changed = False
+
         self.fx_path = os.path.realpath(
             os.path.join(dirs.INSTALL_DIR, 'fixpoint_widgets'))
 
         self.no_fx_filter_img = os.path.join(self.fx_path, "no_fx_filter.png")
         if not os.path.isfile(self.no_fx_filter_img):
             logger.error("Image {0:s} not found!".format(self.no_fx_filter_img))
 
         self.default_fx_img = os.path.join(self.fx_path, "default_fx_img.png")
         if not os.path.isfile(self.default_fx_img):
             logger.error("Image {0:s} not found!".format(self.default_fx_img))
 
+        self.cmb_qfrmt_items = [
+            "<span>Quantization format for coefficients (affects only "
+            "the display, not the stored values).</span>",
+            ('float', "Float", "<span>Full precision floating point format</span>"),
+            ('qint', "Integer", "<span>Integer format with <i>WI</i> + 1 bits "
+             "(range -2<sup>WI</sup> ... 2<sup>WI</sup> - 1)</span>"),
+            ('qfrac', "Fractional",
+             "<span>General fractional format with <i>WI</i> + <i>WF</i> + 1 bits "
+             "(range -2<sup>WI</sup> ... 2<sup>WI</sup> - 2<sup>WF</sup>).</span>")
+            ]
+        self.cmb_qfrmt_default = "float"
+
         self._construct_UI()
         inst_wdg_list = self._update_filter_cmb()
         if len(inst_wdg_list) == 0:
             logger.warning("No fixpoint filter found for this type of filter!")
         else:
             logger.debug("Imported {0:d} fixpoint filters:\n{1}"
                          .format(len(inst_wdg_list.split("\n"))-1, inst_wdg_list))
         self._update_fixp_widget()
+        self.dict2ui()  # update fixpoint widgets
 
 # ------------------------------------------------------------------------------
     def process_sig_rx_local(self, dict_sig: dict = None) -> None:
         """
         Process signals coming in from input and output quantizer subwidget and
         emit {'fx_sim': 'specs_changed'} in the end.
         """
-        logger.debug(
-            f"SIG_RX_LOCAL(): vis={self.isVisible()}\n{pprint_log(dict_sig)}")
+        # logger.warning(
+        #     f"SIG_RX_LOCAL(): vis={self.isVisible()}\n{pprint_log(dict_sig)}")
+        # logger.warning(
+        #    f"SIG_RX_LOCAL: vis={self.isVisible()}, fx_sim={fb.fil[0]['fx_sim']}\n{first_item(dict_sig)}")
         if dict_sig['id'] == id(self):
-            logger.warning(
-                f'RX_LOCAL - Stopped infinite loop: "{first_item(dict_sig)}"')
+            # logger.warning(
+            #     f'RX_LOCAL - Stopped infinite loop: "{pprint_log(dict_sig)}"')
             return
         # ---------------------------------------------------------------------
         # Updated fixpoint specs in filter widget, update UI + emit with self id
 
         elif 'fx_sim' in dict_sig and dict_sig['fx_sim'] == 'specs_changed':
-            self.wdg_dict2ui()  # update wordlengths in UI, set RUN button to 'changed'
+            self.dict2ui() # update fixpoint widgets
             dict_sig.update({'id': id(self)})  # propagate 'specs_changed' with self 'id'
             self.emit(dict_sig)
             return
 
         # ---- Process input and output quantizer settings ('ui_local_changed') --
         elif 'ui_local_changed' in dict_sig:
-            if 'wdg_name' not in dict_sig:
-                logger.warning(f"No key 'wdg_name' in dict_sig:\n{pprint_log(dict_sig)}")
+            if 'sender_name' not in dict_sig:
+                logger.warning(f"No key 'sender_name' in dict_sig:\n{pprint_log(dict_sig)}")
                 return
 
             elif dict_sig['ui_local_changed']\
                     not in {'WI', 'WF', 'ovfl', 'quant', 'cmbW', 'butLock'}:
                 logger.warning(
                     f"Unknown value '{dict_sig['ui_local_changed']}' "
                     "for key 'ui_local_changed'")
                 return
 
-            elif dict_sig['wdg_name'] == 'wq_input':
+            elif dict_sig['sender_name'] == 'fx_ui_wq_input':
                 """
-                Input fixpoint format has been changed or butLock has been clicked.
-                When I/O lock is active, copy input fixpoint word format to output
-                word format.
+                Input fixpoint format has been changed: Update filter dict with the
+                settings of the input quantizer dict. If I/O lock is active, copy
+                input fixpoint word format to output word format. Do the same
+                if butLock has been activated.
                 """
+                fb.fil[0]['fxq']['QI'].update(self.wdg_wq_input.Q.q_dict)
                 if dict_sig['ui_local_changed'] == 'butLock'\
                         and not self.wdg_wq_input.butLock.isChecked():
                     # butLock was deactivitated, don't do anything
                     return
                 elif self.wdg_wq_input.butLock.isChecked():
                     # button lock was activated or wordlength settings have been changed
-                    fb.fil[0]['fxqc']['QO']['WI'] = fb.fil[0]['fxqc']['QI']['WI']
-                    fb.fil[0]['fxqc']['QO']['WF'] = fb.fil[0]['fxqc']['QI']['WF']
-                    fb.fil[0]['fxqc']['QO']['W'] = fb.fil[0]['fxqc']['QI']['W']
+                    # with active lock -> copy input settings to output
+                    fb.fil[0]['fxq']['QO']['WI'] = fb.fil[0]['fxq']['QI']['WI']
+                    fb.fil[0]['fxq']['QO']['WF'] = fb.fil[0]['fxq']['QI']['WF']
 
-            elif dict_sig['wdg_name'] == 'wq_output':
+            elif dict_sig['sender_name'] == 'fx_ui_wq_output':
                 """
-                Output fixpoint format has been changed. When I/O lock is active, copy
+                Output fixpoint format has been changed: Update filter dict with the
+                settings of the output quantizer dict. When I/O lock is active, copy
                 output fixpoint word format to input word format.
                 """
+                fb.fil[0]['fxq']['QO'].update(self.wdg_wq_output.Q.q_dict)
+
                 if self.wdg_wq_input.butLock.isChecked():
-                    fb.fil[0]['fxqc']['QI']['WI'] = fb.fil[0]['fxqc']['QO']['WI']
-                    fb.fil[0]['fxqc']['QI']['WF'] = fb.fil[0]['fxqc']['QO']['WF']
-                    fb.fil[0]['fxqc']['QI']['W'] = fb.fil[0]['fxqc']['QO']['W']
+                    fb.fil[0]['fxq']['QI']['WI'] = fb.fil[0]['fxq']['QO']['WI']
+                    fb.fil[0]['fxq']['QI']['WF'] = fb.fil[0]['fxq']['QO']['WF']
             else:
-                logger.error("Unknown wdg_name '{0}' in dict_sig:\n{1}"
-                             .format(dict_sig['wdg_name'], pprint_log(dict_sig)))
+                logger.error("Unknown wdg_name / sender_name '{0}' in dict_sig:\n{1}"
+                             .format(dict_sig['sender_name'], pprint_log(dict_sig)))
                 return
 
-            self.wdg_dict2ui()  # update wordlengths in UI and set RUN button to 'changed'
+            self.dict2ui() # update fixpoint widgets
             self.emit({'fx_sim': 'specs_changed'})  # propagate 'specs_changed'
         # --------------------------------------------------------------------------------
 
         else:
             logger.error(f"Unknown key/value in 'dict_sig':\n{pprint_log(dict_sig)}")
         return
 
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig: dict = None) -> None:
         """
         Process signals coming in via `sig_rx` from other widgets.
 
         Trigger fx simulation:
 
-        1. ``fx_sim': 'init'``: Start fixpoint simulation by sending
-           'fx_sim':'start_fx_response_calculation'
+        1. `fx_sim': 'init'`: Start fixpoint simulation by sending
+           `'fx_sim':'start_fx_response_calculation'`
 
         2. Store fixpoint response in `fb.fx_result` and return to initiating routine
         """
 
-        logger.debug(
-            "SIG_RX(): vis={0}\n{1}".format(self.isVisible(), pprint_log(dict_sig)))
-        # logger.debug(f'SIG_RX():  "{first_item(dict_sig)}"')
-
+        # logger.warning(
+        #     "SIG_RX(): vis={0}\n{1}".format(self.isVisible(), pprint_log(dict_sig)))
+        # logger.warning(
+        #     f"SIG_RX: vis={self.isVisible()}, fx_sim={fb.fil[0]['fx_sim']}\n{pprint_log(dict_sig)}")
         if dict_sig['id'] == id(self):
             # logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
-        #  =================== UI_CHANGED =======================================
-        elif 'ui_global_changed' in dict_sig and dict_sig['ui_global_changed']\
-                in {'resized', 'tab'} and self.isVisible():
-            # Widget size has changed / "Fixpoint" tab has been selected -> resize image
-            self.resize_img()
-
-        # =================== DATA CHANGED =====================================
-        elif 'data_changed' in dict_sig and\
-                dict_sig['data_changed'] == "filter_designed":
-            # New filter has been designed, update list of available filter topologies
-            self._update_filter_cmb()
-            return
-
+        # always update visibility of subwidgets and resize image, also when in float mode
+        # or invisible (?)
+        if 'fx_sim' in dict_sig and dict_sig['fx_sim'] == 'specs_changed':
+            self.dict2ui()
         elif 'data_changed' in dict_sig:
-            # Filter data has changed (but not the filter type):
-            # - reload UI from dict and set RUN button to "changed"
-            self.wdg_dict2ui()
-
-        # =================== FX SIM ============================================
-        elif 'fx_sim' in dict_sig:
-
-            # --------------- init -------------------
-            if dict_sig['fx_sim'] == 'init':
-                # fixpoint simulation has been started externally, e.g. by
-                # `impz.impz_init()`, return a handle to the fixpoint filter function
-                # via signal-slot connection
-                if not self.fx_wdg_found:
-                    logger.error("No fixpoint widget found!")
-                    qstyle_widget(self.butSimFx, "error")
-                    self.emit({'fx_sim': 'error'})
-                    return
-                # initialize fixpoint filter and check for error during initialization
-                err = self.fx_filt_init()
-                if err != 0:  # returned an error
-                    qstyle_widget(self.butSimFx, "error")
-                    self.emit({'fx_sim': 'error'})
-                else:
-                    # Reset overflow counter for input and output quantization,
-                    self.wdg_wq_input.QObj.resetN()
-                    self.wdg_wq_output.QObj.resetN()
-                    # Trigger fixpoint response calculation, passing a handle to the
-                    # fixpoint filter function in the emitted dict
-                    if hasattr(self.fx_filt_ui, 'fxfilter'):
-                        self.emit({'fx_sim': 'start_fx_response_calculation',
-                                   'fxfilter_func': self.fx_filt_ui.fxfilter})
-                    else:
-                        logger.error(
-                            "Couldn't find fixpoint filter definition\n"
-                            f"\t'{self.fx_filt_ui.__class__.__name__}.fxfilter'!")
+            if dict_sig['data_changed'] == 'filter_loaded':
+                self.load_fx_filter()
+                # TODO: should self._update_filter_cmb() be called here?
+                return
+            elif dict_sig['data_changed'] == "filter_designed":
+                # New filter has been designed, update list of available filter topologies
+                self._update_filter_cmb()
+
+        if fb.fil[0]['fx_sim']:  # fixpoint mode active
+            #  =================== UI_CHANGED =======================================
+            if 'ui_global_changed' in dict_sig and dict_sig['ui_global_changed']\
+                    in {'resized', 'tab'} and self.isVisible():
+                # Widget size has changed / "Fixpoint" tab has been selected -> resize image
+                self.resize_img()
+
+            # =================== DATA CHANGED =====================================
+            elif 'data_changed' in dict_sig:
+                # Filter data has changed (but not the filter type):
+                # Update fixpoint widgets from dict
+                self.dict2ui()
+
+            # =================== FX SIM ============================================
+            elif 'fx_sim' in dict_sig:
+                # --------------- init -------------------
+                if dict_sig['fx_sim'] == 'init':
+                    # fixpoint simulation has been started externally, e.g. by
+                    # `impz.impz_init()`
+                    if not self.fx_wdg_found:
+                        logger.error("No fixpoint widget found!")
+                        # process this in PlotImpz()
                         self.emit({'fx_sim': 'error'})
+                        return
+                    # initialize fixpoint filter and check for error during initialization
+                    err = self.fx_filt_init()
+                    if err != 0:  # returned an error
+                        # process this in PlotImpz()
+                        self.emit({'fx_sim': 'error'})
+                    else:
+                        # Reset overflow counter for input and output quantizer
+                        self.wdg_wq_input.Q.resetN()
+                        self.wdg_wq_output.Q.resetN()
+                        # Trigger fixpoint response calculation, passing a handle to the
+                        # fixpoint filter function in the emitted dict via signal-slot
+                        if hasattr(self.fx_filt_ui, 'fxfilter'):
+                            self.emit({'fx_sim': 'start_fx_response_calculation',
+                                    'fxfilter_func': self.fx_filt_ui.fxfilter})
+                        else:
+                            logger.error(
+                                "Couldn't find fixpoint filter definition\n"
+                                f"\t'{self.fx_filt_ui.__class__.__name__}.fxfilter'!")
+                            self.emit({'fx_sim': 'error'})
+
+                        # next, start fx response calculation in `plot_impz()`
+                        return
+
+                # --------------- finish --------------
+                elif dict_sig['fx_sim'] == 'finish':
+                    # update I/O widgets and dynamically instantiated filter widget with
+                    # number of overflows etc.
+                    self.wdg_wq_input.update_ovfl_cnt()
+                    self.wdg_wq_output.update_ovfl_cnt()
+                    if hasattr(self, 'fx_filt_ui') and hasattr(self.fx_filt_ui, 'update_ovfl_cnt_all'):
+                        self.fx_filt_ui.update_ovfl_cnt_all()
+                    else:
+                        logger.warning("No method 'fx_filt_ui.update_ovfl_cnt_all()'")
 
-                    # next, start fx response calculation in `plot_impz()`
-                    return
-
-            # --------------- finish --------------
-            elif dict_sig['fx_sim'] == 'finish':
-                # update I/O widgets and dynamically instantiated filter widget with
-                # number of overflows etc.
-                self.wdg_wq_input.update_disp()
-                self.wdg_wq_output.update_disp()
-                if hasattr(self, 'fx_filt_ui') and hasattr(self.fx_filt_ui, 'update'):
-                    self.fx_filt_ui.update_disp()
-                qstyle_widget(self.butSimFx, "normal")
-            # fixpoint specifications / quantization settings have been changed
-            # somewhere else, update UI and set run button to "changed" in wdg_dict2ui()
-
-            # --------------- fx specs_changed ------------
-            elif self.fx_specs_changed or\
-                    (dict_sig['fx_sim'] == 'specs_changed' and self.isVisible()):
-                # update wordlengths in UI and set RUN button to 'changed':
-                self.wdg_dict2ui()
-                self.fx_specs_changed = False
-                # self.emit(dict_sig)  # TODO: ???
-                return
-            elif dict_sig['fx_sim'] == 'specs_changed' and not self.isVisible():
+                # --------------- fx_sim : specs_changed ------------
+                elif dict_sig['fx_sim'] == 'specs_changed' and self.isVisible():
+                    self.dict2ui()  # update fixpoint widgets
+                    self.fx_specs_changed = False
+                elif dict_sig['fx_sim'] == 'specs_changed' and not self.isVisible():
+                    self.fx_specs_changed = True
+                else:
+                    logger.error('Unknown "fx_sim" command option "{0}"\n'
+                                '\treceived from "{1}".'
+                                .format(dict_sig['fx_sim'], dict_sig['class']))
+
+            # the next part is reached when fx_sim is active but no fx_sim command
+            # has been issued:
+            # =================== Previous Changes ====================================
+            # have fixpoint specs / filter been changed when widget was invisible
+            # or in float mode? If yes, update fixpoint topologies and UI from dict,
+            # set RUN button to 'changed' and resize fixpoint image.
+            if self.fx_filt_changed:
+                self.fx_filt_changed = False  # reset flag
+                self.fx_specs_changed = False  # reset flag
+                self._update_filter_cmb()
+
+            elif self.fx_specs_changed:
+                self.fx_specs_changed = False  # reset flag
+                self.dict2ui()  # update fixpoint widgets
+
+        # =============================================================================
+        else:  # fixpoint mode is not active
+            if 'data_changed' in dict_sig:
+                # Filter data has changed (but not the filter type):
+                # Reload UI from dict and
                 self.fx_specs_changed = True
 
-            else:
-                logger.error('Unknown "fx_sim" command option "{0}"\n'
-                             '\treceived from "{1}".'
-                             .format(dict_sig['fx_sim'], dict_sig['class']))
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self) -> None:
         """
         Intitialize the main UI, consisting of:
 
         - A combo box to select the filter topology and an image of the topology
@@ -274,17 +318,17 @@
         # The actual filter widget is instantiated / deleted in
         # `self._update_fixp_widget()` later on
 
         self.layH_fx_wdg = QHBoxLayout()
         # left and right: Zero margin, top and bottom: default margin
         self.layH_fx_wdg.setContentsMargins(0, margins[1], 0, margins[3])
         # self.layH_fx_wdg.setContentsMargins(*params['wdg_margins'])
-        wdg_fx = QWidget(self)
-        wdg_fx.setStyleSheet(".QWidget { background-color:none; }")
-        wdg_fx.setLayout(self.layH_fx_wdg)
+        wdg_fx_dyn = QWidget(self)
+        wdg_fx_dyn.setStyleSheet(".QWidget { background-color:none; }")
+        wdg_fx_dyn.setLayout(self.layH_fx_wdg)
 
 # ------------------------------------------------------------------------------
 #       Initialize fixpoint filter combobox, title and description
 # ------------------------------------------------------------------------------
         self.cmb_fx_wdg = QComboBox(self)
         self.cmb_fx_wdg.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
@@ -311,27 +355,28 @@
 #       Input and Output Quantizer
 # ------------------------------------------------------------------------------
 #       - instantiate widgets for input and output quantizer
 #       - pass the quantization dictionary to the constructor
 # ------------------------------------------------------------------------------
 
         self.wdg_wq_input = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QI'], wdg_name='wq_input',
+            fb.fil[0]['fxq']['QI'], objectName='fx_ui_wq_input',
             label='<b>Input Quantizer <i>Q<sub>X&nbsp;</sub></i>:</b>',
-            lock_vis='on')
+            lock_vis='on', cmb_w_vis='off')
         if HAS_DS:
             self.wdg_wq_input.cmbQuant.addItem('DSM', userData='dsm')
             self.wdg_wq_input.cmbQuant.setItemData(
                 self.wdg_wq_input.cmbQuant.count() - 1,
                 self.wdg_wq_input.cmbQuant.tr("Delta-Sigma Modulation"), Qt.ToolTipRole)
         self.wdg_wq_input.sig_tx.connect(self.sig_rx_local)
 
         self.wdg_wq_output = FX_UI_WQ(
-            fb.fil[0]['fxqc']['QO'], wdg_name='wq_output',
-            label='<b>Output Quantizer <i>Q<sub>Y&nbsp;</sub></i>:</b>')
+            fb.fil[0]['fxq']['QO'], objectName='fx_ui_wq_output',
+            label='<b>Output Quantizer <i>Q<sub>Y&nbsp;</sub></i>:</b>',
+            cmb_w_vis='off')
         self.wdg_wq_output.sig_tx.connect(self.sig_rx_local)
 
 # ------------------------------------------------------------------------------
 #       Dynamically updated image of filter topology (label as placeholder)
 # ------------------------------------------------------------------------------
         # allow setting background color
         # lbl_fixp_img_palette = QPalette()
@@ -351,39 +396,42 @@
         self.frmImg = QFrame(self)
         self.frmImg.setLayout(layHImg)
         self.frmImg.setContentsMargins(*params['wdg_margins'])
 
 # ------------------------------------------------------------------------------
 #       Simulation and export Buttons
 # ------------------------------------------------------------------------------
+        # choose float / fixpoint mode
+        self.cmb_qfrmt = QComboBox(self)
+        qcmb_box_populate(self.cmb_qfrmt, self.cmb_qfrmt_items,
+                          self.cmb_qfrmt_default)
+        self.cmb_qfrmt.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+
         self.butExportHDL = QPushButton(self)
         self.butExportHDL.setToolTip(
             "Create Verilog or VHDL netlist for fixpoint filter.")
         self.butExportHDL.setText("Create HDL")
 
-        self.butSimFx = QPushButton(self)
-        self.butSimFx.setToolTip("Start fixpoint simulation.")
-        self.butSimFx.setText("Sim. FX")
-
-        self.layHHdlBtns = QHBoxLayout()
-        self.layHHdlBtns.addWidget(self.butSimFx)
-        self.layHHdlBtns.addWidget(self.butExportHDL)
-        # This frame encompasses the HDL buttons sim and convert
+        # Wrap qfrmt combobox and HDL buttons sim and convert in one layout
+        layH_fx_btns = QHBoxLayout()
+        layH_fx_btns.addWidget(self.cmb_qfrmt)
+        layH_fx_btns.addWidget(self.butExportHDL)
+
         frmHdlBtns = QFrame(self)
-        frmHdlBtns.setLayout(self.layHHdlBtns)
+        frmHdlBtns.setLayout(layH_fx_btns)
         frmHdlBtns.setContentsMargins(*params['wdg_margins'])
 
 # -------------------------------------------------------------------
 #       Top level layout
 # -------------------------------------------------------------------
         layVMain = QVBoxLayout()
         layVMain.addWidget(self.frmTitle)
         layVMain.addWidget(frmHdlBtns)
         layVMain.addWidget(self.wdg_wq_input)
-        layVMain.addWidget(wdg_fx)
+        layVMain.addWidget(wdg_fx_dyn)
         layVMain.addWidget(self.wdg_wq_output)
         layVMain.addWidget(self.frmImg)
         layVMain.addStretch()
         layVMain.setContentsMargins(*params['wdg_margins'])
 
         self.setLayout(layVMain)
 
@@ -400,74 +448,95 @@
         #     self.fx_filt_ui.sig_tx.connect(self.sig_rx_local)
         # ----
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.cmb_fx_wdg.currentIndexChanged.connect(self._update_fixp_widget)
         self.butExportHDL.clicked.connect(self.exportHDL)
-        self.butSimFx.clicked.connect(self._start_fx_sim)
+        self.cmb_qfrmt.currentIndexChanged.connect(self.qfrmt2ui)
+
         # ----------------------------------------------------------------------
         # EVENT FILTER
         # ----------------------------------------------------------------------
         # # monitor events and generate sig_resize event when resized
         # self.lbl_fixp_img.installEventFilter(self)
         # # ... then redraw image when resized
         # self.sig_resize.connect(self.resize_img)
 
 # ------------------------------------------------------------------------------
-    def _start_fx_sim(self) -> None:
+    def load_fx_filter(self) -> None:
         """
-        Start fixpoint simulation by setting the global fixpoint flag
-        `fb.fil[0]['fx_sim'] = True` and emitting `{'fx_sim': 'start_fx_sim'}`.
+        A new filter has been loaded, create fixpoint filter from scratch.
+
+        (Re-)Read list of available fixpoint filters for a given filter class
+        every time a new filter has been designed or loaded.
+
+        Then try to import the fixpoint designs in the list and populate the
+        fixpoint implementation combo box `self.cmb_fx_wdg` with successfull
+        imports.
         """
-        fb.fil[0]['fx_sim'] = True
-        self.emit({'fx_sim': 'start_fx_sim'})
+        self._update_filter_cmb(fx_wdg=fb.fil[0]['fx_mod_class_name'])
+
+        self.dict2ui()  # update fixpoint widgets
 
 # ------------------------------------------------------------------------------
-    def _update_filter_cmb(self) -> str:
+    def _update_filter_cmb(self, fx_wdg: str = "") -> str:
         """
-        (Re-)Read list of available fixpoint filters for a given filter design
-        every time a new filter design is selected.
+        (Re-)Read list of available fixpoint filters for a given filter class
+        every time a new filter has been designed or loaded.
 
         Then try to import the fixpoint designs in the list and populate the
-        fixpoint implementation combo box `self.cmb_fx_wdg` when successfull.
+        fixpoint implementation combo box `self.cmb_fx_wdg` with successful
+        imports.
+
+        Try to set the combobox to the passed argument `fx_wdg` or (if empty), try
+        to use the last combobox setting. If both fail, use the first entry of the
+        combobox.
+
+        Parameters
+        ----------
+        fx_wdg: str
+          fully qualified name of fixpoint widget (optional)
 
         Returns
         -------
         inst_wdg_str: str
-          string with all fixpoint widgets that could be instantiated successfully
+          string with all fixpoint widgets that have been instantiated successfully.
         """
         inst_wdg_str = ""  # full names of successfully instantiated widgets for logging
         # remember last fx widget setting:
         last_fx_wdg = qget_cmb_box(self.cmb_fx_wdg, data=False)
-        self.cmb_fx_wdg.clear()
-        fc = fb.fil[0]['fc']
+        self.cmb_fx_wdg.clear()  # clear combobox
+        fc = fb.fil[0]['fc']  # get current filter class
 
         if 'fix' in fb.filter_classes[fc]:
             self.cmb_fx_wdg.blockSignals(True)
             for class_name in fb.filter_classes[fc]['fix']:  # get class name
                 try:   # construct module + class name ...
                     mod_class_name = fb.fixpoint_classes[class_name]['mod'] + '.'\
                         + class_name
                     # ... and display name
                     disp_name = fb.fixpoint_classes[class_name]['name']
                     self.cmb_fx_wdg.addItem(disp_name, mod_class_name)
                     inst_wdg_str += '\t' + class_name + ' : ' + mod_class_name + '\n'
                 except AttributeError as e:
                     logger.warning('Widget "{0}":\n{1}'.format(class_name, e))
                     self.embed_fixp_img(self.no_fx_filter_img)
-                    continue  # with next `class_name` of for loop
+                    continue  # with next `class_name` in for loop
                 except KeyError as e:
                     logger.warning("No fixpoint filter for filter type {0} available."
                                    .format(e))
                     self.embed_fixp_img(self.no_fx_filter_img)
-                    continue  # with next `class_name` of for loop
+                    continue  # with next `class_name` in for loop
 
-            # restore last fx widget if possible
-            idx = self.cmb_fx_wdg.findText(last_fx_wdg)
+            # set passed fx_widget or restore last fx widget if possible
+            if fx_wdg:
+                idx = self.cmb_fx_wdg.findText(fx_wdg)
+            else:
+                idx = self.cmb_fx_wdg.findText(last_fx_wdg)
             # set to idx 0 if not found (returned -1)
             self.cmb_fx_wdg.setCurrentIndex(max(idx, 0))
             self.cmb_fx_wdg.blockSignals(False)
         else:  # no fixpoint widget
             self.embed_fixp_img(self.no_fx_filter_img)
         self._update_fixp_widget()
         return inst_wdg_str
@@ -569,44 +638,43 @@
                     self.layH_fx_wdg.removeWidget(self.fx_filt_ui)
                     # delete QWidget when scope has been left
                     self.fx_filt_ui.deleteLater()
                 except AttributeError as e:
                     logger.error("Destructing UI failed!\n{0}".format(e))
 
             self.fx_wdg_found = False
-            self.butSimFx.setEnabled(False)
             self.butExportHDL.setVisible(False)
             self.img_fixp = self.embed_fixp_img(self.no_fx_filter_img)
             self.resize_img()
             self.lblTitle.setText("")
 
             self.fx_filt_ui = None
         # -----------------------------------------------------------
         _disable_fx_wdg(self)  # destruct old fixpoint widget instance:
 
         # instantiate new fixpoint widget class as self.fx_filt_ui
         cmb_wdg_fx_cur = qget_cmb_box(self.cmb_fx_wdg, data=False)
         if cmb_wdg_fx_cur:  # at least one valid fixpoint widget found
             self.fx_wdg_found = True
+            self.cmb_qfrmt.setEnabled(True)
             # get list [module name and path, class name]
             fx_mod_class_name = qget_cmb_box(self.cmb_fx_wdg, data=True).rsplit('.', 1)
             fx_mod = importlib.import_module(fx_mod_class_name[0])  # get module
             fx_filt_ui_class = getattr(fx_mod, fx_mod_class_name[1])  # get class
             logger.info("Instantiating new FX widget\n\t"
                         f"{fx_mod.__name__}.{fx_filt_ui_class.__name__}")
             # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
             self.fx_filt_ui = fx_filt_ui_class()  # instantiate the fixpoint widget
             # set lightblue background with transparency for fixpoint widget
             self.fx_filt_ui.setStyleSheet(
                ".QFrame { background-color: rgba(173, 216, 230, 25%)}")
             # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
             # and add it to layout:
             self.layH_fx_wdg.addWidget(self.fx_filt_ui, stretch=1)
-            self.fx_filt_ui.setVisible(True)
-            self.wdg_dict2ui()  # initialize the fixpoint subwidgets from the fxqc_dict
+            self.dict2ui()  # update fixpoint widgets from dictionary
 
             # ---- connect signals to fx_filt_ui ----
             if hasattr(self.fx_filt_ui, "sig_rx"):
                 self.sig_rx.connect(self.fx_filt_ui.sig_rx)
             if hasattr(self.fx_filt_ui, "sig_tx"):
                 self.fx_filt_ui.sig_tx.connect(self.sig_rx_local)
 
@@ -628,37 +696,90 @@
             self.lblTitle.setText(self.fx_filt_ui.title)
             if hasattr(self.fx_filt_ui, "description"):
                 self.lbl_descr.setVisible(True)
                 self.lbl_descr.setText(self.fx_filt_ui.description)
             else:
                 self.lbl_descr.setVisible(False)
 
+            # store fully qualified name of current fixpoint class:
+            fb.fil[0]['fx_mod_class_name'] = fx_mod_class_name[0]
             # Check which methods the fixpoint widget provides and enable
             # corresponding buttons:
             self.butExportHDL.setVisible(hasattr(self.fx_filt_ui, "to_hdl"))
-            self.butSimFx.setEnabled(hasattr(self.fx_filt_ui, "fxfilter"))
-            self.emit({'fx_sim': 'specs_changed'})
+
+        else:  # no fixpoint widget found
+            fb.fil[0]['fx_mod_class_name'] = ""
+            self.fx_wdg_found = False
+            # fb.fil[0]['fx_sim'] = False
+            self.lbl_descr.setVisible(False)
+            self.cmb_qfrmt.setEnabled(False)
+
+        self.emit({'fx_sim': 'specs_changed'})
 
 # ------------------------------------------------------------------------------
-    def wdg_dict2ui(self):
+    def qfrmt2ui(self):
         """
-        Trigger an update of the input, output and fixpoint widgets UI when view
-        (i.e. fixpoint coefficient format) or data have been changed outside this
-        class.
+        Triggered by by a change of index of the combo box `self.cmb_qfrmt`.
+
+        - Update UI (fixpoint format, visibility of fixpoint widgets) from combobox
+          `self.cmb_qfrmt` to `fb.fil[0]['fx_sim']` and `fb.fil[0]['qfrmt']`.
+
+        - Update fixpoint widget settings via `self.dict2ui()`
+
+        - Emit {'fx_sim': 'specs_changed'}.
+          """
+        fb.fil[0]['fx_sim'] = (qget_cmb_box(self.cmb_qfrmt) != 'float')
+        if fb.fil[0]['fx_sim']:
+            fb.fil[0]['qfrmt'] = qget_cmb_box(self.cmb_qfrmt)
 
-        Set the RUN button to "changed".
+        self.dict2ui()
+
+        self.emit({'fx_sim': 'specs_changed'})
+
+# ------------------------------------------------------------------------------
+    def dict2ui(self):
         """
-        self.wdg_wq_input.dict2ui()
-        self.wdg_wq_output.dict2ui()
+        Called during `__init__()` and from `process_sig_rx()`.
 
-#       The following should be connected via signal-slot
-#         if self.fx_wdg_found and hasattr(self.fx_filt_ui, "dict2ui"):
-#             self.fx_filt_ui.dict2ui()
+        Update UI from `fb.fil[0]['fx_sim']`, `fb.fil[0]['qfrmt']` and the fx filter
+        dict `fb.fil[0]['fxq']`. This affects the visibility and the fx settings of
+        input, output and dyn. filter widget via their `dict2ui()` methods.
+        The setting of the `self.cmb_qfrmt` combobox influencing float / fixpoint number
+        format is updated as well.
+        """
+        if not fb.fil[0]['fx_mod_class_name']:  # no fixpoint filter available
+            fb.fil[0]['fx_sim'] = False
+        is_fixp = fb.fil[0]['fx_sim']
+
+        # fixpoint widgets are only visible in fixpoint mode
+        self.frmTitle.setVisible(is_fixp)
+        self.wdg_wq_input.setVisible(is_fixp)
+        self.wdg_wq_output.setVisible(is_fixp)
+        self.frmImg.setVisible(is_fixp)
+        if self.fx_wdg_found:
+           self.fx_filt_ui.setVisible(is_fixp)
 
-        qstyle_widget(self.butSimFx, "changed")
+        if is_fixp:
+            # set combobox from dictionary
+            qset_cmb_box(self.cmb_qfrmt, fb.fil[0]['qfrmt'], data=True)
+            # refresh image in case of switching from float to fix
+            self.resize_img()
+            # update fixpoint widgets from the global filter dict:
+            # when loading a filter, a new instance of fb.fil[0] is created, requiring
+            # passing a hard update of the filter dict
+            self.wdg_wq_input.dict2ui(fb.fil[0]['fxq']['QI'])
+            self.wdg_wq_output.dict2ui(fb.fil[0]['fxq']['QO'])
+            try:
+                # this uses the global filter dict as well but it is reinstantiated
+                # when loading a filter, using the new instance
+                self.fx_filt_ui.dict2ui()
+            except AttributeError as e:
+                logger.error(f"Error using FX filter widget 'dict2ui()' method:\n{e}")
+        elif not fb.fil[0]['fx_sim']:
+            qset_cmb_box(self.cmb_qfrmt, 'float', data=True)
 
 # ------------------------------------------------------------------------------
     def exportHDL(self):
         """
         Synthesize HDL description of filter
         """
         dlg = QFileDialog(self)  # instantiate file dialog object
@@ -669,30 +790,17 @@
         dlg.setWindowTitle('Export Verilog')
         dlg.setNameFilter(file_types)
         dlg.setDirectory(dirs.last_file_dir)
         # set mode "save file" instead "open file":
         dlg.setAcceptMode(QFileDialog.AcceptSave)
         dlg.setOption(QFileDialog.DontConfirmOverwrite, False)
         if dlg.exec_() == QFileDialog.Accepted:
-            hdl_file = qstr(dlg.selectedFiles()[0])
-            # hdl_type = extract_file_ext(qstr(dlg.selectedNameFilter()))[0]
+            hdl_file = str(dlg.selectedFiles()[0])
+            # hdl_type = extract_file_ext(qstr(dlg.selectedNameFilter()))
 
-# =============================================================================
-#       # static method getSaveFileName_() is simple but unflexible
-#         hdl_file, hdl_filter = dlg.getSaveFileName_(
-#                 caption="Save Verilog netlist as (this also defines the module name)",
-#                 directory=dirs.last_file_dir, filter=file_types)
-#         hdl_file = qstr(hdl_file)
-#         if hdl_file != "": # "operation cancelled" returns an empty string
-#             # return '.v' or '.vhd' depending on filetype selection:
-#             # hdl_type = extract_file_ext(qstr(hdl_filter))[0]
-#             # sanitized dir + filename + suffix. The filename suffix is replaced
-#             # by `v` later.
-#             hdl_file = os.path.normpath(hdl_file) # complete path + file name
-# =============================================================================
             hdl_dir_name = os.path.dirname(hdl_file)  # extract the directory path
             if not os.path.isdir(hdl_dir_name):  # create directory if it doesn't exist
                 os.mkdir(hdl_dir_name)
             hdl_file_name = os.path.splitext(os.path.basename(hdl_file))[0]
             hdl_full_name = os.path.join(hdl_dir_name, hdl_file_name + ".v")
             dirs.last_file_name = hdl_full_name
             dirs.last_file_dir = hdl_dir_name  # make this directory the new default / base dir
@@ -722,22 +830,22 @@
         TODO: - Update the `fxqc_dict` containing all quantization information
 
         Returns
         -------
         error: int
             0 for sucessful fx widget construction, -1 for error
         """
-        try:
+        if True:
+        # try:
             # initialize fixpoint filter instance with fixpoint quantizer
-            # self.fx_filt_ui.init_filter()
-            self.fx_filt_ui.fx_filt.init(fb.fil[0]['fxqc'])
+            self.fx_filt_ui.fx_filt.init(fb.fil[0]['fxq'])
 
             return 0
-
-        except (ValueError, AttributeError) as e:
+        else:
+        # except (ValueError, AttributeError) as e:
             logger.error('Fixpoint filter reset or instantiation failed.'
                          '\nwith "{0} "'.format(e))
         return -1
 
 # ------------------------------------------------------------------------------
     def fx_sim_calc_response(self, dict_sig) -> None:
         """
@@ -747,58 +855,33 @@
           `fb.fx_results == None`
 
         Returns
         -------
         None
         """
         try:
-            # logger.info(
-            #     'Simulate fixpoint frame with "{0}" stimulus:\n\t{1}'.format(
-            #         dict_sig['class'],
-            #         pprint_log(dict_sig['fx_stimulus'], tab=" "),
-            #         ))
-
             # Run fixpoint simulation and store the results as integer values:
             fb.fx_results = self.fx_filt_ui.fxfilter(dict_sig['fx_stimulus'])
 
             if len(fb.fx_results) == 0:
                 logger.error("Fixpoint simulation returned empty results!")
-            # else:
-            #     # logger.debug("fx_results: {0}"\
-            #     #            .format(pprint_log(fb.fx_results, tab= " ")))
-            #     logger.info(
-            #         f'Fixpoint simulation successful for dict\n{pprint_log(dict_sig)}'
-            #         f'\tStimuli: Shape {np.shape(dict_sig["fx_stimulus"])}'
-            #         f' of type "{dict_sig["fx_stimulus"].dtype}"'
-            #         f'\n\tResponse: Shape {np.shape(fb.fx_results)}'
-            #         f' of type "{type(fb.fx_results).__name__} "'
-            #         f' ("{type(fb.fx_results[0]).__name__}")'
-            #     )
 
         except ValueError as e:
             logger.error("Simulator error {0}".format(e))
             fb.fx_results = None
 
         except AssertionError as e:
-            logger.error('Fixpoint simulation failed for dict\n{0}'
-                         '\twith msg. "{1}"\n\tStimuli: Shape {2} of type "{3}"'
-                         '\n\tResponse: Shape {4} of type "{5}"'.format(
-                            pprint_log(dict_sig), e,
-                            np.shape(dict_sig['fx_stimulus']),
-                            dict_sig['fx_stimulus'].dtype,
-                            np.shape(fb.fx_results),
-                            type(fb.fx_results)
-                                ))
+            logger.error(
+                f'Fixpoint simulation failed for dict\n{pprint_log(dict_sig)}'
+                f'\twith msg. "{e}"\n\tStimuli: Shape {np.shape(dict_sig["fx_stimulus"])} '
+                f'of type {dict_sig["fx_stimulus"].dtype}'
+                f'\n\tResponse: Shape {np.shape(fb.fx_results)} of type '
+                f'"{type(fb.fx_results)}"')
             fb.fx_results = None
 
-        if fb.fx_results is None:
-            qstyle_widget(self.butSimFx, "error")
-        else:
-            pass  # everything ok, return
-            # logger.debug("Sending fixpoint results")
         return
 
 
 ###############################################################################
 if __name__ == '__main__':
     """
     Run widget standalone with `python -m pyfda.input_widgets.input_fixpoint_specs`
@@ -810,15 +893,15 @@
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
 
     logging.basicConfig()  # setup a basic logger
 
     app = QApplication(sys.argv)
     app.setStyleSheet(rc.qss_rc)
-    # change initial settings to FIR (no IIR fixpoint filters available yet)
+    # change initial settings to FIR
     # fb.fil[0].update({'ft': 'FIR', 'fc': 'Equiripple'})
     # _ = Tree_Builder()  # TODO_ couldn't this be a function?
     fb.fil[0].update({'ft': 'IIR', 'fc': 'Ellip'})
     _ = Tree_Builder()  # TODO_ couldn't this be a function?
     mainw = Input_Fixpoint_Specs()
     app.setActiveWindow(mainw)
     mainw.show()
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_info.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_info.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_info_about.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_info_about.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_pz.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_pz.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pyfda.libs.compat import (
     QtCore, QWidget, QLineEdit, pyqtSignal, QEvent, QIcon,
     QBrush, QColor, QSize, QStyledItemDelegate, QApplication,
     QTableWidget, QTableWidgetItem, Qt, QVBoxLayout)
 
 from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qstyle_widget
-from pyfda.libs.pyfda_io_lib import qtable2csv, data2array, save_data_csv
+from pyfda.libs.pyfda_io_lib import qtable2csv, data2array, export_fil_data
 from pyfda.libs.pyfda_sig_lib import zeros_with_val, zpk2array
 
 import numpy as np
 from scipy.signal import freqz, zpk2tf
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
 from pyfda.libs.pyfda_lib import qstr, fil_save, safe_eval, pprint_log
@@ -204,18 +204,17 @@
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct the UI from the table widget and the control part (`self.ui`),
         initialize the widget and setup signal-slot connections and event filters
         """
-        self.tblPZ = QTableWidget(self)
+        self.tblPZ = QTableWidget(self, objectName="tblPZ")
 #        self.tblPZ.setEditTriggers(QTableWidget.AllEditTriggers) # make everything editable
         self.tblPZ.setAlternatingRowColors(True)  # alternating row colors)
-        self.tblPZ.setObjectName("tblPZ")
 
         # highlight when selected:
         self.tblPZ.horizontalHeader().setHighlightSections(True)
         self.tblPZ.horizontalHeader().setFont(self.ui.bfont)
 
         self.tblPZ.verticalHeader().setHighlightSections(True)
         self.tblPZ.verticalHeader().setFont(self.ui.bfont)
@@ -251,15 +250,15 @@
         self.ui.butSave.clicked.connect(self._save_entries)
         self.ui.cmbNorm.activated.connect(self._normalize_gain)
 
         self.ui.butDelCells.clicked.connect(self._delete_cells)
         self.ui.butAddCells.clicked.connect(self._add_rows)
         self.ui.butClear.clicked.connect(self._clear_table)
 
-        self.ui.butFromTable.clicked.connect(self._export)
+        self.ui.butFromTable.clicked.connect(self.export_table)
         self.ui.butToTable.clicked.connect(self._import)
 
         self.ui.butSetZero.clicked.connect(self._zero_PZ)
 
         self.ui.ledGain.installEventFilter(self)
         self.ui.ledEps.editingFinished.connect(self._set_eps)
 
@@ -460,15 +459,15 @@
 
         Format is: [array[zeros, ...], array[poles, ...], k]
         """
         if not type(fb.fil[0]['zpk']) is np.ndarray:
             logger.warning(f"fb.fil[0]['zpk'] is of type {type(fb.fil[0]['zpk'])} "
                            f"with len = {len(fb.fil[0]['zpk'])}")
 
-        zpk = list(fb.fil[0]['zpk'].copy())
+        zpk = list(fb.fil[0]['zpk']).copy()
 
         if len(zpk) == 3:  # number of rows
             if np.isscalar(zpk[2]):
                 logger.warning("Gain is scalar, converting to proper format!")
                 zpk[2] = zeros_with_val(len(zpk[0]), zpk[2])  # add a row gain
             elif len(zpk[2]) != len(zpk[0]):
                 zpk[2] = zeros_with_val(len(zpk[0]), zpk[2][0])
@@ -521,15 +520,15 @@
 
     # ------------------------------------------------------------------------------
     def _clear_table(self):
         """
         Clear & initialize table and zpk for two poles and zeros @ origin,
         P = Z = [0; 0], k = 1
         """
-        self.zpk = np.array([[0, 0], [0, 0], [1, 0]])
+        self.zpk = np.array([[0, 0], [0, 0], [1, 0]], dtype=complex)
         self.Hmax_last = 1.0
 
         qstyle_widget(self.ui.butSave, 'changed')
         self._refresh_table()
 
     # ------------------------------------------------------------------------------
     def _get_selected(self, table):
@@ -557,44 +556,50 @@
         - determining the indices of all selected cells in the P and Z arrays
         - deleting elements with those indices
         - equalizing the lengths of P and Z array by appending the required
           number of zeros.
         - deleting all P/Z pairs
         Finally, the table is refreshed from self.zpk.
         """
-        sel = self._get_selected(self.tblPZ)['idx']  # get all selected indices as 2D list
-        sel_z = [s[1] for s in sel if s[0] == 0]  # list with selected indices in 'Z' column
-        sel_p = [s[1] for s in sel if s[0] == 1]  # list with selected indices in 'P' column
+        sel = self._get_selected(self.tblPZ)['idx']  # get selected indices as 2D list
+        sel_z = [s[1] for s in sel if s[0] == 0]  # list with sel. indices in 'Z' column
+        sel_p = [s[1] for s in sel if s[0] == 1]  # list with sel. indices in 'P' column
 
         k = self.zpk[2][0]
 
         # Delete array entries with selected indices. If nothing is selected
-        # (Z and P are empty), delete the last row.
+        # (sel_z and sel_p are empty), delete the last row.
         if len(sel_z) < 1 and len(sel_p) < 1:
             sel_z = [len(self.zpk[0])-1]
             sel_p = [len(self.zpk[1])-1]
         zeros = np.delete(self.zpk[0], sel_z)
         poles = np.delete(self.zpk[1], sel_p)
 
-        # test and equalize if P and Z array have different lengths:
-        D = len(zeros) - len(poles)
-        if D > 0:
-            poles = np.append(poles, np.zeros(D))
-        elif D < 0:
-            zeros = np.append(zeros, np.zeros(-D))
+        # If resulting poles and zeros are empty, re-initialize using
+        # `self._clear_table()`. This also refreshes the table and marks
+        # the "Save" button as changed.
+        if len(zeros) == 0 and len(poles) == 0:
+            self._clear_table()
+        else:
+            # test and equalize if P and Z array have different lengths:
+            D = len(zeros) - len(poles)
+            if D > 0:
+                poles = np.append(poles, np.zeros(D))
+            elif D < 0:
+                zeros = np.append(zeros, np.zeros(-D))
 
-        gain = zeros_with_val(max(len(poles), len(zeros)), k)
+            gain = zeros_with_val(max(len(poles), len(zeros)), k)
 
-        # reconstruct array with new number of rows
-        self.zpk = np.array([zeros, poles, gain])
+            # reconstruct array with new number of rows
+            self.zpk = np.array([zeros, poles, gain])
 
-        self._delete_PZ_pairs()
-        self._normalize_gain()
-        qstyle_widget(self.ui.butSave, 'changed')
-        self._refresh_table()
+            self._delete_PZ_pairs()
+            self._normalize_gain()
+            qstyle_widget(self.ui.butSave, 'changed')
+            self._refresh_table()
 
     # ------------------------------------------------------------------------------
     def _add_rows(self):
         """
         Add the number of selected rows to the table and fill new cells with
         zeros. If nothing is selected, add one row.
         """
@@ -735,15 +740,15 @@
                     .format(r=r, p=phi, plcs=places, angle_char=self.angle_char,
                             pi_char=self.pi_char)
 
         else:
             logger.error("Unknown format {0}.".format(frmt))
 
     # ------------------------------------------------------------------------------
-    def frmt2cmplx(self, string, default=0.):
+    def frmt2cmplx(self, string: str, default: float = 0.) -> complex:
         """
         Convert string to real or complex, try to find out the format (cartesian,
         polar with various angle formats)
         """
         def str2angle_rad(string: str) -> float:
             """
             Try to convert `string` to a corresponding angle in rad
@@ -794,27 +799,28 @@
             if safe_eval.err > 0:
                 x = default.real
                 y = default.imag
                 logger.warning(f"Expression {string} could not be evaluated.")
             return x + 1j * y
 
     # --------------------------------------------------------------------------
-    def _export(self):
+    def export_table(self):
         """
         Export data from coefficient table `self.tblCoeff` to clipboard in CSV format
         or to file using a selected format
         """
         text = qtable2csv(
             self.tblPZ, self.zpk, zpk=True, formatted=self.ui.but_format.isChecked())
-        if params['CSV']['clipboard']:  # clipboard is selected as export target
+        if params['CSV']['destination'] == 'clipboard':
+            # clipboard is selected as export target
             fb.clipboard.setText(text)
         else:
             # pass csv formatted text, key for accessing data in ``*.npz`` file or
             # Matlab workspace (``*.mat``) and a title for the file export dialog
-            save_data_csv(self, text, 'zpk', title="Export Poles / Zeros")
+            export_fil_data(self, text, 'zpk', title="Export Poles / Zeros")
     # --------------------------------------------------------------------------
     def _import(self):
         """
         Import data from clipboard / file and copy it to `self.zpk` as array of complex
         # TODO: More checks for swapped row <-> col, single values, wrong data type ...
         """
         data_str = data2array(self, 'zpk', title="Import Poles / Zeros ",
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_pz_ui.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_pz_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 from pyfda.libs.compat import (
     pyqtSignal, Qt, QWidget, QLabel, QLineEdit, QComboBox, QPushButton,
     QFrame, QSpinBox, QFont, QIcon, QVBoxLayout, QHBoxLayout)
 
 from pyfda.libs.pyfda_qt_lib import qstyle_widget, qcmb_box_populate, PushButton
 from pyfda.libs.csv_option_box import CSV_option_box
-from pyfda.libs.pyfda_lib import to_html
+from pyfda.libs.pyfda_lib import to_html, first_item
 import pyfda.libs.pyfda_dirs as dirs
 from pyfda.pyfda_rc import params
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -55,31 +55,38 @@
             ('polar_pi', 'Polar (pi)',
              "<span>Polar coordinates (r * &ang; &Omega;) with &ang; in multiples "
              "of &pi;, type 'pi' instead of &pi;.</span>"),
             ('polar_deg', 'Polar (°)',
             "<span>Polar coordinates (r * &ang; &Omega;) with &ang; in degrees, "
             "use 'o' or '°' as the degree sign.</span>"),]
         # π: u'3C0, °: u'B0, ∠: u'2220
-        self.cmb_pz_frmt_init = 'polar_deg'  # initial setting
+        self.cmb_pz_frmt_init = 'cartesian'  # initial setting
 
         self._construct_UI()
 
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from the CSV pop-up window
         """
         # logger.debug("PROCESS_SIG_RX\n{0}".format(pprint_log(dict_sig)))
-
-        if 'closeEvent' in dict_sig:
+        if dict_sig['id'] == id(self):
+            logger.warning(
+                # this should not happen as the rx slot is not connected globally
+                f'Stopped infinite loop: "{first_item(dict_sig)}"')
+            return
+        elif 'closeEvent' in dict_sig:
             self._close_csv_win()
+            # send signal that pop-up box is closed
             self.emit({'ui_global_changed': 'csv'})
         elif 'ui_global_changed' in dict_sig:
             self._set_load_save_icons()  # update icons file <-> clipboard
-            # set state of CSV options button according to state of CSV popup handle
+            # signal change of CSV options to other widgets with current id
+            self.emit({'ui_global_changed': 'csv'})
+
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the widget, consisting of:
         - top chkbox row
         - coefficient table
@@ -103,17 +110,17 @@
         self.spnDigits.setRange(0, 16)
         self.spnDigits.setToolTip("Number of digits to display.")
         self.lblDigits = QLabel("Digits", self)
         self.lblDigits.setFont(self.bifont)
 
         self.but_format = QPushButton(QIcon(':/star.svg'), "", self)
         self.but_format.setToolTip(
-            "<span>Save and load poles, zeros and gain <i>k</i> with the table format "
-            "when activated, e.g. in polar coordinates, with the selected number of "
-            "digits etc.</span>"
+            "<span>Save and load poles, zeros and gain <i>k</i> formatted as in the "
+            "table when activated, e.g. in polar coordinates, with the selected number "
+            "of digits etc.</span>"
             )
         q_icon_size = self.but_format.iconSize()
         self.but_format.setCheckable(True)
 
         # self.cmbCausal = QComboBox(self)
         # causal_types = ['Causal', 'Acausal', 'Anticausal']
         # for cs in causal_types:
@@ -141,20 +148,19 @@
         self.cmbNorm = QComboBox(self)
         self.cmbNorm.addItems(["None", "1", "Max"])
         self.cmbNorm.setToolTip(
             "<span>Set the gain <i>k</i> so that H(f)<sub>max</sub> is "
             "either 1 or the max. of the previous system.</span>")
 
         self.lblGain = QLabel(to_html("k =", frmt='bi'), self)
-        self.ledGain = QLineEdit(self)
+        self.ledGain = QLineEdit(self, objectName="ledGain")
         self.ledGain.setToolTip(
             "<span>Specify gain factor <i>k</i>"
             " (only possible for Normalize = 'None').</span>")
         self.ledGain.setText(str(1.))
-        self.ledGain.setObjectName("ledGain")
 
         layHGain = QHBoxLayout()
         layHGain.addWidget(self.lblNorm)
         layHGain.addWidget(self.cmbNorm)
         layHGain.addWidget(self.lblGain)
         layHGain.addWidget(self.ledGain)
         layHGain.addStretch()
@@ -179,21 +185,21 @@
             "Use &lt;SHIFT&gt; or &lt;CTRL&gt; to select multiple cells. "
             "When nothing is selected, delete the last row.</span>")
 
         self.butSave = QPushButton(self)
         self.butSave.setIcon(QIcon(':/upload.svg'))
         self.butSave.setIconSize(q_icon_size)
         self.butSave.setToolTip(
-            "<span>Copy P/Z table to filter dict and update all plots and widgets."
+            "<span>Create filter from P/Z table and update all plots and widgets."
             "</span>")
 
         self.butLoad = QPushButton(self)
         self.butLoad.setIcon(QIcon(':/download.svg'))
         self.butLoad.setIconSize(q_icon_size)
-        self.butLoad.setToolTip("Reload P/Z table from filter dict.")
+        self.butLoad.setToolTip("<span>(Re)Load P/Z table from current filter.</span>")
 
         self.butClear = QPushButton(self)
         self.butClear.setIcon(QIcon(':/trash.svg'))
         self.butClear.setIconSize(q_icon_size)
         self.butClear.setToolTip("Clear all table entries.")
 
         self.butFromTable = QPushButton(self)
@@ -300,30 +306,30 @@
 
     # ------------------------------------------------------------------------------
     def _set_load_save_icons(self):
         """
         Set icons / tooltipps for loading and saving data to / from file or
         clipboard depending on selected options.
         """
-        if params['CSV']['clipboard']:
+        if params['CSV']['destination'] == 'clipboard':
             self.butFromTable.setIcon(QIcon(':/to_clipboard.svg'))
             self.butFromTable.setToolTip(
                 "<span>Copy table to clipboard in float format with full precision "
                 "when the &lt;FORMAT&gt; button is not selected.<br>"
                 "Otherwise, copy the table as displayed.</span>")
 
             self.butToTable.setIcon(QIcon(':/from_clipboard.svg'))
             self.butToTable.setToolTip(
                 "<span>Import table from clipboard in float format "
                 "when the &lt;FORMAT&gt; button is not selected.<br>"
-                "Otherwise, import the table as displayed.</span>")
+                "Otherwise, import the table in display format.</span>")
         else:
             self.butFromTable.setIcon(QIcon(':/save.svg'))
             self.butFromTable.setToolTip(
-                "<span>Save table to file in float format with full precision "
+                "<span>Export table to file in float format with full precision "
                 "when the &lt;FORMAT&gt; button is not selected.<br>"
                 "Otherwise, save the table as displayed.</span>")
 
             self.butToTable.setIcon(QIcon(':/file.svg'))
             self.butToTable.setToolTip(
                 "<span>Import table from file in float format. "
                 "when the &lt;FORMAT&gt; button is not selected.<br>"
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_specs.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 # (see file LICENSE in root directory for details)
 
 """
 Widget stacking all subwidgets for filter specification and design. The actual
 filter design is started here as well.
 """
 import sys
+import copy
 
 from pyfda.libs.compat import (
-    QWidget, QLabel, QFrame, QPushButton, pyqtSignal, QVBoxLayout, QHBoxLayout)
+    Qt, QWidget, QLabel, QFrame, QPushButton, QComboBox, QLineEdit, pyqtSignal,
+    QVBoxLayout, QHBoxLayout, QSizePolicy)
 
 import pyfda.filterbroker as fb
 import pyfda.filter_factory as ff
-from pyfda.libs.pyfda_lib import pprint_log
-from pyfda.libs.pyfda_qt_lib import qstyle_widget
+from pyfda.libs.pyfda_lib import pprint_log, to_html, first_item
+from pyfda.libs.pyfda_qt_lib import qstyle_widget, qcmb_box_populate, qget_cmb_box, qget_selected
 from pyfda.libs.pyfda_io_lib import load_filter, save_filter
 from pyfda.pyfda_rc import params
 
 from pyfda.input_widgets import (select_filter, amplitude_specs,
                                  freq_specs, freq_units,
                                  weight_specs, target_specs)
 import logging
@@ -38,125 +40,148 @@
     # class variables (shared between instances if more than one exists)
     sig_rx_local = pyqtSignal(object)  # incoming from subwidgets -> process_sig_rx_local
 
     sig_rx = pyqtSignal(object)  # incoming from subwidgets -> process_sig_rx
     sig_tx = pyqtSignal(object)  # from process_sig_rx: propagate local signals
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName="input_specs_inst"):
         super(Input_Specs, self).__init__(parent)
+        self.setObjectName(objectName)
         self.tab_label = "Specs"
         self.tool_tip = "Enter and view filter specifications."
 
+        self.cmb_filter_selection_items = [
+            "<span>Select file or memory location for saving or loading filters.</span>",
+            ("file", "File", "Save / load filter to / from file."),
+            ("1", "Mem 1", "Save / load to / from memory 1"),
+            ("2", "Mem 2", "Save / load to / from memory 2"),
+            ("3", "Mem 3", "Save / load to / from memory 3"),
+            ("4", "Mem 4", "Save / load to / from memory 4"),
+            ("5", "Mem 5", "Save / load to / from memory 5"),
+            ("6", "Mem 6", "Save / load to / from memory 6"),
+            ("7", "Mem 7", "Save / load to / from memory 7"),
+            ("8", "Mem 8", "Save / load to / from memory 8"),
+            ("9", "Mem 9", "Save / load to / from memory 9")
+        ]
+        self.cmb_filter_selection_default = "file"
+
         self._construct_UI()
 
     def process_sig_rx_local(self, dict_sig=None):
         """
-        Flag signals coming in from local subwidgets with `propagate=True` before
-        proceeding with processing in `process_sig_rx`.
+        Signals coming in from local subwidgets need to be propagated, so set
+        `propagate=True` and proceed with processing in `process_sig_rx`.
         """
         self.process_sig_rx(dict_sig, propagate=True)
 
-    def process_sig_rx(self, dict_sig=None, propagate=False):
+    def process_sig_rx(self, dict_sig, propagate=False):
         """
         Process signals coming in via subwidgets and sig_rx
 
         All signals terminate here unless the flag `propagate=True`.
 
         The sender name of signals coming in from local subwidgets is changed to
         its parent widget (`input_specs`) to prevent infinite loops.
 
         """
-        logger.debug(f"SIG_RX: {pprint_log(dict_sig)}")
+        # logger.warning(f"SIG_RX: {first_item(dict_sig)}")
         if dict_sig['id'] == id(self):
             # logger.warning(f"Stopped infinite loop:\n\tPropagate = {propagate}\
-            #               \n{pprint_log(dict_sig)}")
+            #               \n{first_item(dict_sig)}")
             return
-        elif 'view_changed' in dict_sig:
-            self.f_specs.load_dict()
-            self.t_specs.load_dict()
+
         elif 'specs_changed' in dict_sig:
-            self.f_specs.sort_dict_freqs()
-            self.t_specs.f_specs.sort_dict_freqs()
-            self.color_design_button("changed")
+            if dict_sig['specs_changed'] == 'f_sort':
+                # sort and update the frequency widgets
+                self.f_specs.sort_dict_freqs()
+                self.t_specs.f_specs.sort_dict_freqs()
+            self.color_design_button('changed')
         elif 'filt_changed' in dict_sig:
             # Changing the filter design requires updating UI because number or
             # kind of input fields changes -> call update_UI
             self.update_UI(dict_sig)
-        elif 'data_changed' in dict_sig:
-            if dict_sig['data_changed'] == 'filter_loaded':
-                """
-                Called when a new filter has been LOADED:
-                Pass new filter data from the global filter dict by
-                specifically calling SelectFilter.load_dict()
-                """
-                self.sel_fil.load_dict()  # update select_filter widget
-            # Pass new filter data from the global filter dict & set button = "ok"
-            self.load_dict()
+        elif 'data_changed' in dict_sig and dict_sig['data_changed'] == 'filter_loaded':
+                # Update info string from filter dict & set button = "ok"
+                # This is only triggered from global signals
+                self.load_dict()
 
         if propagate:
-            # local signals are propagated with the name of this widget,
+            # local signals are propagated with the class name and id of this widget,
             # global signals terminate here
-            dict_sig.update({'class': self.__class__.__name__})
+            dict_sig.update({'class': self.__class__.__name__, 'id': id(self)})
             self.emit(dict_sig)
 
     def _construct_UI(self):
         """
         Construct User Interface from all input subwidgets
         """
         self.butLoadFilt = QPushButton("LOAD FILTER", self)
-        self.butLoadFilt.setToolTip("Load filter from disk")
+        self.butLoadFilt.setToolTip("Load filter from disk or memory")
+        self.cmb_filter_selection = QComboBox(self)
+        qcmb_box_populate(self.cmb_filter_selection, self.cmb_filter_selection_items,
+                          self.cmb_filter_selection_default)
+        self.cmb_filter_selection.setSizePolicy(
+            QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.butSaveFilt = QPushButton("SAVE FILTER", self)
-        self.butSaveFilt.setToolTip("Save filter todisk")
-        layHButtons1 = QHBoxLayout()
-        layHButtons1.addWidget(self.butLoadFilt)  # <Load Filter> button
-        layHButtons1.addWidget(self.butSaveFilt)  # <Save Filter> button
-        layHButtons1.setContentsMargins(*params['wdg_margins_spc'])
+        self.butSaveFilt.setToolTip("Save filter to disk or memory")
+        self.lbl_info = QLabel(to_html("Info:", frmt='b'))
+        self.led_info = QLineEdit(fb.fil[0]['info'])
+        self.led_info.setToolTip("Add an info / comment for the filter")
+        lay_h_buttons_load_save_1 = QHBoxLayout()
+        lay_h_buttons_load_save_1.addWidget(self.butLoadFilt)  # <Load Filter> button
+        lay_h_buttons_load_save_1.addWidget(self.cmb_filter_selection) # File or memory
+        lay_h_buttons_load_save_1.addWidget(self.butSaveFilt)  # <Save Filter> button
+        lay_h_buttons_load_save_1.setContentsMargins(*params['wdg_margins_spc'])
+        lay_h_buttons_load_save_2 = QHBoxLayout()
+        lay_h_buttons_load_save_2.addWidget(self.lbl_info)
+        lay_h_buttons_load_save_2.addWidget(self.led_info)
+        lay_v_buttons_load_save = QVBoxLayout()
+        lay_v_buttons_load_save.addLayout(lay_h_buttons_load_save_1)
+        lay_v_buttons_load_save.addLayout(lay_h_buttons_load_save_2)
+        self.frm_buttons_load_save = QFrame()
+        self.frm_buttons_load_save.setLayout(lay_v_buttons_load_save)
+        self.frm_buttons_load_save.setContentsMargins(*params['wdg_margins'])
 
         self.butDesignFilt = QPushButton("DESIGN FILTER", self)
         self.butDesignFilt.setToolTip("Design filter with chosen specs")
         self.butQuit = QPushButton("Quit", self)
         self.butQuit.setToolTip("Exit pyfda tool")
         layHButtons2 = QHBoxLayout()
         layHButtons2.addWidget(self.butDesignFilt)  # <Design Filter> button
         layHButtons2.addWidget(self.butQuit)        # <Quit> button
         layHButtons2.setContentsMargins(*params['wdg_margins'])
 
         # Subwidget for selecting filter with response type rt (LP, ...),
         #    filter type ft (IIR, ...) and filter class fc (cheby1, ...)
-        self.sel_fil = select_filter.SelectFilter(self)
-        self.sel_fil.setObjectName("select_filter")
+        self.sel_fil = select_filter.SelectFilter(self, objectName="select_filter_inst")
 
         # Subwidget for selecting the frequency unit and range
-        self.f_units = freq_units.FreqUnits(self)
-        self.f_units.setObjectName("freq_units")
+        self.f_units = freq_units.FreqUnits(self, objectName="freq_units_inst")
 
         # Changing the frequency unit requires re-display of frequency specs
         # but it does not influence the actual specs (no specsChanged )
         # Activating the "Sort" button emits 'view_changed'?specs_changed'?, requiring
         # sorting and storing the frequency entries
 
         # Changing filter parameters / specs requires reloading of parameters
         # in other hierarchy levels, e.g. in the plot tabs
 
         # Subwidget for Frequency Specs
-        self.f_specs = freq_specs.FreqSpecs(self)
-        self.f_specs.setObjectName("freq_specs")
+        self.f_specs = freq_specs.FreqSpecs(self, objectName="freq_specs_corner")
 
         # Subwidget for Amplitude Specs
-        self.a_specs = amplitude_specs.AmplitudeSpecs(self)
-        self.a_specs.setObjectName("amplitude_specs")
+        self.a_specs = amplitude_specs.AmplitudeSpecs(self, objectName="amplitude_specs_general")
 
         # Subwidget for Weight Specs
-        self.w_specs = weight_specs.WeightSpecs(self)
-        self.w_specs.setObjectName("weight_specs")
+        self.w_specs = weight_specs.WeightSpecs(self, objectName="weight_specs_inst")
 
         # Subwidget for target specs (frequency and amplitude)
-        self.t_specs = target_specs.TargetSpecs(self, title="Target Specifications")
-        self.t_specs.setObjectName("target_specs")
+        self.t_specs = target_specs.TargetSpecs(self, title="Target Specifications",
+                                                objectName="target_specs_inst")
 
         # Subwidget for displaying infos on the design method
         self.lblMsg = QLabel(self)
         self.lblMsg.setWordWrap(True)
         layVMsg = QVBoxLayout()
         layVMsg.addWidget(self.lblMsg)
 
@@ -166,15 +191,16 @@
         layVFrm.addWidget(self.frmMsg)
         layVFrm.setContentsMargins(*params['wdg_margins'])
 
         # ----------------------------------------------------------------------
         # LAYOUT for input specifications and buttons
         # ----------------------------------------------------------------------
         layVMain = QVBoxLayout(self)
-        layVMain.addLayout(layHButtons1)  # <Load> & <Save> buttons
+        # layVMain.addLayout(lay_v_buttons_load_save)  # <Load> & <Save> buttons
+        layVMain.addWidget(self.frm_buttons_load_save)  # <Load> & <Save> buttons
         layVMain.addWidget(self.sel_fil)  # Design method (IIR - ellip, ...)
         layVMain.addLayout(layHButtons2)  # <Design> & <Quit> buttons
         layVMain.addWidget(self.f_units)  # Frequency units
         layVMain.addWidget(self.t_specs)  # Target specs
         layVMain.addWidget(self.f_specs)  # Freq. specifications
         layVMain.addWidget(self.a_specs)  # Amplitude specs
         layVMain.addWidget(self.w_specs)  # Weight specs
@@ -185,43 +211,56 @@
         layVMain.setContentsMargins(*params['wdg_margins'])
 
         self.setLayout(layVMain)  # main layout of widget
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
+        # connect incoming signals to process_sig_rx and other widgets?!
         self.sig_rx.connect(self.process_sig_rx)
-        self.sig_rx.connect(self.f_units.sig_rx)
+        # self.sig_rx.connect(self.f_units.sig_rx)
         self.sig_rx_local.connect(self.process_sig_rx_local)
 
+        # connect outgoing signal to receive slots of various subwidgets
+        self.sig_tx.connect(self.sel_fil.sig_rx)
         self.sig_tx.connect(self.f_specs.sig_rx)
         self.sig_tx.connect(self.t_specs.sig_rx)
+        self.sig_tx.connect(self.w_specs.sig_rx)
         self.sig_tx.connect(self.f_units.sig_rx)
 
         self.sel_fil.sig_tx.connect(self.sig_rx_local)
         self.f_specs.sig_tx.connect(self.sig_rx_local)
         self.a_specs.sig_tx.connect(self.sig_rx_local)
         self.t_specs.sig_tx.connect(self.sig_rx_local)
         self.w_specs.sig_tx.connect(self.sig_rx_local)
         self.f_units.sig_tx.connect(self.sig_rx_local)
 
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.butLoadFilt.clicked.connect(self._load_filter)
-        self.butSaveFilt.clicked.connect(lambda: save_filter(self))
+        self.butSaveFilt.clicked.connect(self._save_filter)
+        self.led_info.editingFinished.connect(self._save_info2dict)
         self.butDesignFilt.clicked.connect(self.start_design_filt)
+        self.cmb_filter_selection.currentIndexChanged.connect(self.update_info)
         self.butQuit.clicked.connect(self.quit_program)  # emit 'quit_program'
         # ----------------------------------------------------------------------
 
         self.update_UI()  # first time initialization
         self.start_design_filt()  # design first filter using default values
 
 # ------------------------------------------------------------------------------
-    def update_UI(self, dict_sig={}):
+    def _save_info2dict(self) -> None:
+        """
+        Update_filter dict every time the info field is changed
+        """
+        fb.fil[0]['info'] = self.led_info.text()
+
+# ------------------------------------------------------------------------------
+    def update_UI(self, dict_sig={}) -> None:
         """
         update_UI is called every time the filter design method or order
         (min / man) has been changed as this usually requires a different set of
         frequency and amplitude specs.
 
         At this time, the actual filter object instance has been created from
         the name of the design method (e.g. 'cheby1') in select_filter.py.
@@ -293,42 +332,63 @@
             self.frmMsg.setEnabled(all_widgets['msg'][0] != 'd')
             self.lblMsg.setText(all_widgets['msg'][1:][0])
         else:
             self.frmMsg.hide()
 
         # Update state of "DESIGN FILTER" button
         # It is disabled for "Manual_IIR" and "Manual_FIR" filter classes
-        self.color_design_button("changed")
+        self.color_design_button('changed')
 
 # ------------------------------------------------------------------------------
     def _load_filter(self):
-        ret = load_filter(self)
-        if ret == 0:
+        """
+        Load filter dict `fb.fil[0]` either from file or from memory and update the
+        widgets via `load_dict()` and via sig_tx: {'data_changed':'filter_loaded'}.
+        """
+        sel = qget_cmb_box(self.cmb_filter_selection)
+        if sel == "file":
+            ret = load_filter(self)
+            if ret == 0:
+                self.load_dict()
+                self.emit({'data_changed': 'filter_loaded'})
+            elif ret == -1:
+                return  # error occurred, do nothing
+            else:
+                logger.error(f'Unknown return code "{ret}"!')
+        else:
+            fb.fil[0] = copy.deepcopy(fb.fil[int(sel)])
             self.load_dict()
             self.emit({'data_changed': 'filter_loaded'})
-        elif ret == -1:
-            return  # error occurred, do nothing
+
+# ------------------------------------------------------------------------------
+    def _save_filter(self):
+        """ Save current filter fb.fil[0] either to file or to one of the memories"""
+        sel = qget_cmb_box(self.cmb_filter_selection)
+        if sel == "file":
+            save_filter(self)
         else:
-            logger.error(f'Unknown return code "{ret}"!')
+            fb.fil[int(sel)] = copy.deepcopy(fb.fil[0])
+            # set info string as new tool tip
+            self.cmb_filter_selection.setItemData(
+                int(sel), self.led_info.text(), Qt.ToolTipRole)
 
 # ------------------------------------------------------------------------------
     def load_dict(self):
         """
-        Reload all specs/parameters entries from global dict fb.fil[0],
-        using the "load_dict" methods of the individual classes
+        Reload info text from global dict `fb.fil[0]` and reset 'DESIGN' button
         """
-        self.sel_fil.load_dict()  # select filter widget
-        self.f_units.load_dict()  # frequency units widget
-        self.f_specs.load_dict()  # frequency specification widget
-        self.a_specs.load_dict()  # magnitude specs with unit
-        self.w_specs.load_dict()  # weight specification
-        self.t_specs.load_dict()  # target specs
-
+        self.led_info.setText(str(fb.fil[0]['info']))
         self.color_design_button("ok")
-
+# ------------------------------------------------------------------------------
+    def update_info(self):
+        """
+        Update the info field of the filter selection
+        """
+        self.led_info.setText(
+            str(fb.fil[self.cmb_filter_selection.currentIndex()]['info']))
 # ------------------------------------------------------------------------------
     def start_design_filt(self):
         """
         Start the actual filter design process:
 
         - store the entries of all input widgets in the global filter dict.
         - call the design method, passing the whole dictionary as the
@@ -363,41 +423,28 @@
             # -----------------------------------------------------------------------
 
             if err > 0:
                 self.color_design_button("error")
             elif err == -1:  # filter design cancelled by user
                 return
             else:
-                # Update filter order. weights and freq display in case they
-                # have been changed by the design algorithm
+                # Update filter order in case it has been changed by the
+                # design algorithm and emit {'data_changed': 'filter_designed'}
                 self.sel_fil.load_filter_order()
-                self.w_specs.load_dict()
-                self.f_specs.load_dict()
                 self.color_design_button("ok")
 
                 self.emit({'data_changed': 'filter_designed'})
                 logger.info(
-                    'Designed filter with order = {0}'.format(str(fb.fil[0]['N'])))
-# =============================================================================
-#                 logger.debug("Results:\n"
-#                     "F_PB = %s, F_SB = %s "
-#                     "Filter order N = %s\n"
-#                     "NDim fil[0]['ba'] = %s\n\n"
-#                     "b,a = %s\n\n"
-#                     "zpk = %s\n",
-#                     str(fb.fil[0]['F_PB']), str(fb.fil[0]['F_SB']), str(fb.fil[0]['N']),
-#                     str(np.ndim(fb.fil[0]['ba'])), pformat(fb.fil[0]['ba']),
-#                     pformat(fb.fil[0]['zpk']))
-#
-# =============================================================================
+                    f"Designed filter with order = {str(fb.fil[0]['N'])}")
+
         except Exception as e:
             if ('__doc__' in str(e)):
-                logger.warning("Filter design:\n %s\n %s\n", e.__doc__, e)
+                logger.warning(f"Filter design:\n {e.__doc__}\n{e}\n")
             else:
-                logger.warning("{0}".format(e))
+                logger.warning(f"{e}")
             self.color_design_button("error")
 
     def color_design_button(self, state):
         man = "manual" in fb.fil[0]['fc'].lower()
         self.butDesignFilt.setDisabled(man)
         if man:
             state = 'ok'
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/input_tab_widgets.py` & `pyfda-0.9.0b1/pyfda/input_widgets/input_tab_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,17 @@
     # signals as class variables (shared between instances if more than one exists)
     # incoming, connected here to individual senders, passed on to process sigmals
     sig_rx = pyqtSignal(object)
     # outgoing, connected in receiver (pyfdax -> plot_tab_widgets)
     sig_tx = pyqtSignal(object)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName='input_tab_widgets_inst'):
         super(InputTabWidgets, self).__init__(parent)
+        self.setObjectName(objectName)
         self._construct_UI()
 
     def _construct_UI(self):
         """
         Initialize UI with tabbed subwidgets: Instantiate dynamically each widget
         from the dict `fb.input_classes` and try to
 
@@ -144,15 +145,15 @@
 
 # ------------------------------------------------------------------------------
     def log_rx(self, dict_sig=None):
         """
         Enable `self.sig_rx.connect(self.log_rx)` above for debugging.
         """
         if type(dict_sig) == dict:
-            logger.warning("SIG_RX\n{0}".format(pprint_log(dict_sig)))
+            logger.warning(f"SIG_RX\n{pprint_log(dict_sig)}")
         else:
             logger.warning("empty dict")
 
 # ------------------------------------------------------------------------------
     def current_tab_changed(self):
         self.emit({'ui_global_changed': 'tab'})
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/select_filter.py` & `pyfda-0.9.0b1/pyfda/input_widgets/select_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import sys
 from pyfda.libs.compat import (
     QWidget, QLabel, QLineEdit, QComboBox, QFrame,
     QCheckBox, QVBoxLayout, QHBoxLayout, pyqtSignal)
 
 import pyfda.filterbroker as fb
 import pyfda.filter_factory as ff
-from pyfda.libs.pyfda_lib import safe_eval
+from pyfda.libs.pyfda_lib import safe_eval, first_item
 import pyfda.pyfda_rc as rc
 from pyfda.libs.pyfda_qt_lib import qget_cmb_box
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -39,26 +39,52 @@
     Every time a combo box is changed manually, the filter tree for the selected
     response resp. filter type is read and the combo box(es) further down in
     the hierarchy are populated according to the available combinations.
 
     sig_tx({'filt_changed'}) is emitted and propagated to input_filter_specs.py
     where it triggers the recreation of all subwidgets.
     """
+    # class variables (shared between instances if more than one exists)
+    sig_rx = pyqtSignal(object)  # incoming -> process_sig_rx
     sig_tx = pyqtSignal(object)  # outgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName="select_filter_inst"):
         super(SelectFilter, self).__init__(parent)
 
+        self.setObjectName(objectName)
         self.fc_last = ''  # previous filter class
-
         self._construct_UI()
-
         self._set_response_type()  # first time initialization
 
+    def process_sig_rx(self, dict_sig):
+        """
+        Process signals coming in via sig_rx
+
+        All signals terminate here.
+
+        The sender name of signals coming in from local subwidgets is changed to
+        its parent widget to prevent infinite loops.
+
+        """
+        # logger.warning(f"SIG_RX: {first_item(dict_sig)}")
+        if dict_sig['id'] == id(self):
+            # logger.warning(f"Stopped infinite loop:\n\tPropagate = {propagate}\
+            #               \n{first_item(dict_sig)}")
+            return
+
+        elif 'data_changed' in dict_sig:
+            if dict_sig['data_changed'] == 'filter_loaded':
+                """
+                Called when a new filter has been LOADED,
+                pass new filter data from the global filter dict to load_dict()
+                """
+            self.load_dict()
+
+
     def _construct_UI(self):
         """
         Construct UI with comboboxes for selecting filter:
 
         - cmbResponseType for selecting response type rt (LP, HP, ...)
 
         - cmbFilterType for selection of filter type (IIR, FIR, ...)
@@ -70,24 +96,21 @@
 
         See filterbroker.py for structure and content of "filterTree" dict
 
         """
         # ----------------------------------------------------------------------
         # Combo boxes for filter selection
         # ----------------------------------------------------------------------
-        self.cmbResponseType = QComboBox(self)
-        self.cmbResponseType.setObjectName("comboResponseType")
+        self.cmbResponseType = QComboBox(self, objectName="comboResponseType")
         self.cmbResponseType.setToolTip("Select filter response type.")
-        self.cmbFilterType = QComboBox(self)
-        self.cmbFilterType.setObjectName("comboFilterType")
+        self.cmbFilterType = QComboBox(self, objectName="comboFilterType")
         self.cmbFilterType.setToolTip(
           "<span>Choose filter type, either recursive (Infinite Impulse Response) "
           "or transversal (Finite Impulse Response).</span>")
-        self.cmbFilterClass = QComboBox(self)
-        self.cmbFilterClass.setObjectName("comboFilterClass")
+        self.cmbFilterClass = QComboBox(self, objectName="comboFilterClass")
         self.cmbFilterClass.setToolTip("Select the filter design class.")
 
         # Adapt comboboxes size dynamically to largest element
         self.cmbResponseType.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmbFilterType.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmbFilterClass.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
@@ -174,18 +197,22 @@
 
         layHMain = QHBoxLayout()
         layHMain.addWidget(frmMain)
         layHMain.setContentsMargins(*rc.params['wdg_margins'])
 
         self.setLayout(layHMain)
 
-# ==============================================================================
+        # ----------------------------------------------------------------------
+        # GLOBAL SIGNALS & SLOTs
+        # ----------------------------------------------------------------------
+        # connect incoming signals to process_sig_rx and other widgets?!
+        self.sig_rx.connect(self.process_sig_rx)
 
         # ------------------------------------------------------------
-        # SIGNALS & SLOTS
+        # LOCAL SIGNALS & SLOTS
         # ------------------------------------------------------------
         # Connect comboBoxes and setters, propgate change events hierarchically
         #  through all widget methods and emit 'filt_changed' in the end.
         self.cmbResponseType.currentIndexChanged.connect(
                 lambda: self._set_response_type(enb_signal=True))  # 'LP'
         self.cmbFilterType.currentIndexChanged.connect(
                 lambda: self._set_filter_type(enb_signal=True))  # 'IIR'
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/target_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/target_specs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # -*- coding: utf-8 -*-
 #
 # This file is part of the pyFDA project hosted at https://github.com/chipmuenk/pyfda
 #
 # Copyright © pyFDA Project Contributors
 # Licensed under the terms of the MIT License
 # (see file LICENSE in root directory for details)
@@ -12,14 +13,15 @@
 """
 import sys
 
 from pyfda.libs.compat import (
     QWidget, QLabel, QFont, QFrame, pyqtSignal, Qt, QHBoxLayout, QVBoxLayout)
 
 import pyfda.filterbroker as fb
+from pyfda.libs.pyfda_lib import pprint_log, first_item
 from pyfda.input_widgets import amplitude_specs, freq_specs
 from pyfda.pyfda_rc import params
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -27,47 +29,55 @@
     """
     Build and update widget for entering the target specifications (frequencies
     and amplitudes) like F_SB, F_PB, A_SB, etc.
     """
     # class variables (shared between instances if more than one exists)
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing
-    # from pyfda.libs.pyfda_qt_lib import emit
+    sig_tx_local = pyqtSignal(object)  # outgoing to lower hierarchies
+    from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None, title="Target Specs"):
+    def __init__(self, parent=None, title="Target Specs", objectName=""):
         super(TargetSpecs, self).__init__(parent)
 
         self.title = title
+        self.setObjectName(objectName)
 
         self._construct_UI()
 
 # =============================================================================
-# #------------------------------------------------------------------------------
-#     def process_sig_rx(self, dict_sig=None):
-#         """
-#         Process signals coming in via subwidgets and sig_rx
-#         """
-#         logger.warning("Processing {0}: {1}".format(type(dict_sig).__name__, dict_sig))
-#         if dict_sig['id'] == id(self):
-#           logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
-#           return
-#         elif 'view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S':
-#             # update target frequencies with new f_S
-#             self.f_specs.recalc_freqs()
-#
+#------------------------------------------------------------------------------
+    def process_sig_rx(self, dict_sig=None):
+        """
+        Process signals coming in via subwidgets and sig_rx
+        """
+        # logger.warning(f"SIG_RX: {first_item(dict_sig)}")
+        if dict_sig['id'] == id(self):
+          logger.warning("Stopped infinite loop.")
+          return
+        elif 'view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S':
+            # update target frequencies with new f_S
+            self.emit(dict_sig, sig_name='sig_tx_local')
+        elif 'data_changed' in dict_sig and dict_sig['data_changed'] == 'filter_loaded':
+            self.emit(dict_sig, sig_name='sig_tx_local')
+        else:
+            return
+
 # =============================================================================
 
     def _construct_UI(self):
         """
         Construct user interface
         """
         # subwidget for Frequency Specs
-        self.f_specs = freq_specs.FreqSpecs(self, title="Frequency")
+        self.f_specs = freq_specs.FreqSpecs(self, title="Frequency",
+                                            objectName="freq_specs_targ")
         # subwidget for Amplitude Specs
-        self.a_specs = amplitude_specs.AmplitudeSpecs(self, title="Ripple")
+        self.a_specs = amplitude_specs.AmplitudeSpecs(self, title="Ripple",
+                                                      objectName="amplitude_specs_targ")
         self.a_specs.setVisible(True)
         """
         LAYOUT
         """
         bfont = QFont()
         bfont.setBold(True)
         lblTitle = QLabel(self)  # field for widget title
@@ -97,18 +107,22 @@
         self.layVMain.setContentsMargins(*params['wdg_margins'])
 
         self.setLayout(self.layVMain)
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
-        # connect f_specs and a_specs subwidget to signalling
-        self.f_specs.sig_tx.connect(self.sig_tx)  # pass signal upwards
-        self.sig_rx.connect(self.f_specs.sig_rx)  # pass on received signals
-        self.a_specs.sig_tx.connect(self.sig_tx)  # pass signal upwards
+        # process incoming global signals
+        self.sig_rx.connect(self.process_sig_rx)
+        # connect signals from f_specs and a_specs subwidget to higher hierarchies
+        self.f_specs.sig_tx.connect(self.sig_tx)
+        self.a_specs.sig_tx.connect(self.sig_tx)
+        # pass on prefiltered received signals
+        self.sig_tx_local.connect(self.f_specs.sig_rx)
+        self.sig_tx_local.connect(self.a_specs.sig_rx)
 
         self.update_UI()  # first time initialization
 
 # ------------------------------------------------------------------------------
     def update_UI(self, new_labels=()):
         """
         Called when a new filter design algorithm has been selected
@@ -131,26 +145,14 @@
                 new_labels['amp'][0] != 'i'):
             self.a_specs.show()
             self.a_specs.setEnabled(new_labels['amp'][0] != 'd')
             self.a_specs.update_UI(new_labels=new_labels['amp'])
         else:
             self.a_specs.hide()
 
-        # self.emit({'changed_specs':'target'})
-
-# ------------------------------------------------------------------------------
-    def load_dict(self):
-        """
-        Update entries from global dict fb.fil[0]
-        parameters, using the "load_dict" methods of the classes
-        """
-        self.a_specs.load_dict()  # magnitude specs with unit
-        self.f_specs.load_dict()  # weight specification
-
-
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.input_widgets.target_specs` """
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
 
     app = QApplication(sys.argv)
```

### Comparing `pyfda-0.8.4/pyfda/input_widgets/weight_specs.py` & `pyfda-0.9.0b1/pyfda/input_widgets/weight_specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,57 @@
 import sys
 
 from pyfda.libs.compat import (
     QtCore, QWidget, QLabel, QLineEdit, QFrame, QFont, QToolButton,
     QVBoxLayout, QHBoxLayout, QGridLayout, pyqtSignal, QEvent)
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_lib import to_html, safe_eval
+from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log, first_item
 from pyfda.libs.pyfda_qt_lib import qstyle_widget
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
+import logging
+logger = logging.getLogger(__name__)
+
 class WeightSpecs(QWidget):
     """
     Build and update widget for entering the weight
     specifications like W_SB, W_PB etc.
     """
-    sig_tx = pyqtSignal(object)  # outgoing
+    sig_rx = pyqtSignal(object)  # receive signals from higher hierarchies
+    sig_tx = pyqtSignal(object)  # outgoing signals
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName=""):
         super(WeightSpecs, self).__init__(parent)
 
+        self.setObjectName(objectName)
         self.qlabels = []  # list with references to QLabel widgets
         self.qlineedit = []  # list with references to QLineEdit widgets
 
         self.spec_edited = False  # flag whether QLineEdit field has been edited
 
         self._construct_UI()
 
+# -------------------------------------------------------------
+    def process_sig_rx(self, dict_sig=None):
+        """
+        Process signals coming in via subwidgets and sig_rx
+        """
+        # logger.warning(
+        #     f"SIG RX: {first_item(dict_sig)}")
+        if dict_sig['id'] == id(self):
+            # logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
+            return
+        elif 'data_changed' in dict_sig:
+            if dict_sig['data_changed'] in {'filter_loaded', 'filter_designed'}:
+                self.load_dict()
+            # elif 'filt_changed' in dict_sig['data_changed'] == 'filter_designed':
+            #    self.update_UI()
+            # This needs to be called directly, passing labels etc.
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct User Interface
         """
         self.layGSpecs = QGridLayout()  # Sublayout for spec fields, populated
                                         # dynamically in _show_entries()
@@ -81,14 +102,19 @@
         # - Pass the list to setEntries which recreates the widget
         # ATTENTION: Entries need to be converted from QString to str for Py 2
         self.n_cur_labels = 0  # number of currently visible labels / qlineedits
         new_labels = [str(lbl) for lbl in fb.fil[0] if lbl[0] == 'W']
         self.update_UI(new_labels=new_labels)
 
         # ----------------------------------------------------------------------
+        # GLOBAL SIGNALS & SLOTs
+        # ----------------------------------------------------------------------
+        self.sig_rx.connect(self.process_sig_rx)
+
+        # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs / EVENT FILTER
         # ----------------------------------------------------------------------
         self.butReset.clicked.connect(self._reset_weights)
         #       ^ this also initializes the weight text fields
         # DYNAMIC EVENT MONITORING
         # Every time a field is edited, call self._store_entry and
         # self.load_dict. This is achieved by dynamically installing and
@@ -111,15 +137,15 @@
           `spec_edited`== True) and display the stored value in selected format
         """
         if isinstance(source, QLineEdit):  # could be extended for other widgets
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
                 self.load_dict()
                 # store current entry in case new value can't be evaluated:
-                fb.data_old = source.text()
+                self.data_prev = source.text()
             elif event.type() == QEvent.KeyPress:
                 self.spec_edited = True  # entry has been changed
                 key = event.key()
                 if key in {QtCore.Qt.Key_Return, QtCore.Qt.Key_Enter}:
                     self._store_entry(source)
                 elif key == QtCore.Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
@@ -190,15 +216,15 @@
     def _store_entry(self, widget):
         """
         When the textfield of `widget` has been edited (`self.spec_edited` =  True),
         store the weight spec in filter dict. This is triggered by `QEvent.focusOut`
         """
         if self.spec_edited:
             w_label = str(widget.objectName())
-            w_value = safe_eval(widget.text(), fb.data_old, sign='pos')
+            w_value = safe_eval(widget.text(), self.data_prev, sign='pos')
             if w_value < 1:
                 w_value = 1
             if w_value > 1.e6:
                 w_value = 1.e6
             fb.fil[0].update({w_label: w_value})
             self.emit({'specs_changed': 'w_specs'})
             self.spec_edited = False  # reset flag
```

### Comparing `pyfda-0.8.4/pyfda/libs/compat.py` & `pyfda-0.9.0b1/pyfda/libs/compat.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/libs/csv_option_box.py` & `pyfda-0.9.0b1/pyfda/libs/csv_option_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 Library with classes and functions for file and text IO
 """
 # TODO: import data from files doesn't update FIR / IIR and data changed
 
 from .pyfda_qt_lib import (qget_cmb_box, qset_cmb_box, qcmb_box_populate,
                            qwindow_stay_on_top)
+from .pyfda_lib import to_html
 from pyfda.pyfda_rc import params
 from .compat import (QLabel, QComboBox, QDialog, QPushButton, QRadioButton,
                      QCheckBox, QVBoxLayout, QGridLayout, pyqtSignal)
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -27,18 +28,19 @@
     Create a pop-up widget for setting CSV options. This is needed when storing /
     reading Comma-Separated Value (CSV) files containing coefficients or poles
     and zeros.
     """
     sig_tx = pyqtSignal(object)  # outgoing  # was: (dict)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent, has_cmsis=True):
+    def __init__(self, parent):
         super(CSV_option_box, self).__init__(parent)
 
-        self.has_cmsis = has_cmsis
+        # self.has_cmsis = has_cmsis
+        self.cmb_destination_default = "file"
         self.cmb_delimiter_default = "auto"
         self.cmb_terminator_default = "auto"
         self.cmb_orientation_default = "auto"
         self.cmb_header_default = "auto"
 
         self._construct_UI()
         qwindow_stay_on_top(self, True)
@@ -53,34 +55,41 @@
         self.emit({'closeEvent': ''})
         event.accept()
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """ initialize the User Interface """
         self.setWindowTitle("CSV Options")
-
-        lbl_delimiter = QLabel("CSV delimiter", self)
-        cmb_delimiter_items = ["<span>Select delimiter between data fields for im- and export."
-                       "</span>",
+        lbl_destination = QLabel(to_html("Import / export:", frmt='b'))
+        cmb_destination_items = ["<span>Select destination for import / export of data."
+                                 "</span>",
+                                 ("file", "File", "From / to file,"),
+                                 ("clipboard", "Clipboard", "From / to clipboard")]
+        self.cmb_destination = QComboBox(self)
+        qcmb_box_populate(self.cmb_destination, cmb_destination_items,
+                          self.cmb_destination_default)
+
+        lbl_delimiter = QLabel(to_html("CSV delimiter", frmt='b'), self)
+        cmb_delimiter_items = ["<span>Select delimiter between data fields for "
+                               "im- and export.</span>",
             ("auto", "Auto / ','", "<span>Detect the delimiter automatically for import, "
              "use ',' for exporting data.</span>"),
             (',', '< , >', "<span>Use ',' as delimiter between data fields.</span>"),
             (';', '< ; >', "<span>Use ';' as delimiter between data fields.</span>"),
             ( '\t', '<TAB>', "<span>Use &lt;TAB&gt; as delimiter between data fields."
              "</span>"),
             ( ' ', '<SPACE>', "<span>Use &lt;SPACE&gt; as delimiter between data "
              "fields.</span>"),
             ( '|', '< | >',"<span>Use '|' as delimiter between data fields.</span>")
             ]
         self.cmb_delimiter = QComboBox(self)
         qcmb_box_populate(self.cmb_delimiter, cmb_delimiter_items,
                           self.cmb_delimiter_default)
 
-
-        lbl_terminator = QLabel("Line terminator", self)
+        lbl_terminator = QLabel(to_html("Line terminator", frmt='b'), self)
         cmb_terminator_items = [
             "<span>Terminator at the end of a data row, depending on the operating "
             "system. 'None' can be used for a single row of data with added line breaks.</span>",
             ('auto', 'Auto',
              "<span>Use operating system's default line terminator.</span>"),
             ('\r\n', 'CRLF (Win)', 'Use &lt;CRLF&gt; as line terminator (Windows '
              'convention)</span>'),
@@ -93,100 +102,92 @@
         self.cmb_terminator = QComboBox(self)
         qcmb_box_populate(self.cmb_terminator, cmb_terminator_items,
                           self.cmb_terminator_default)
 
         butClose = QPushButton(self)
         butClose.setText("Close")
 
-        lbl_orientation = QLabel("Table mode", self)
+        lbl_orientation = QLabel(to_html("Table orientation", frmt='b'), self)
         cmb_orientation_items = [
-            "<span>Select row / column mode of table.</span>",
+            "<span>Select row / column orientation of table.</span>",
             ('auto', 'Auto/Cols.', "<span>Detect table orientation automatically "
              "during import; use column format for exporting data.</span>"),
             ('cols', 'Columns', "<span>Import / export data in columns.</span>"),
             ('rows', 'Rows', "<span>Import / export data in rows.</span>")
             ]
         self.cmb_orientation = QComboBox(self)
         qcmb_box_populate(self.cmb_orientation, cmb_orientation_items,
                           self.cmb_orientation_default)
 
-        lbl_header = QLabel("Use header", self)
+        lbl_header = QLabel(to_html("Use header", frmt='b'), self)
         cmb_header_items = [
             "<span>Interpret first row resp. column as header.</span>",
             ('auto', 'Auto/Off', "<span>Detect header automatically during import; "
              "turn off header during export.</span>"),
             ('on', 'On', "<span>Turn on header.</span>"),
             ('off', 'Off', "<span>Turn off.</span>")
             ]
         self.cmb_header = QComboBox(self)
         qcmb_box_populate(self.cmb_header, cmb_header_items,
                           self.cmb_header_default)
 
-        lbl_cmsis = QLabel("CMSIS SOS format", self)
-        lbl_cmsis.setVisible(self.has_cmsis)
-        self.chk_cmsis = QCheckBox()
-        self.chk_cmsis.setChecked(False)
-        self.chk_cmsis.setToolTip(
-            "<span>Use CMSIS DSP second-order sections format "
-            "(only for IIR coefficients).</span>")
-        self.chk_cmsis.setVisible(self.has_cmsis)
-
-        self.radClipboard = QRadioButton("Clipboard", self)
-        self.radClipboard.setChecked(False)
-        self.radFile = QRadioButton("File", self)
-        # setting is read later on from params['CSV']['clipboard']
-        self.radFile.setChecked(True)
+        # lbl_cmsis = QLabel("CMSIS SOS format", self)
+        # lbl_cmsis.setVisible(self.has_cmsis)
+        # self.chk_cmsis = QCheckBox()
+        # self.chk_cmsis.setChecked(False)
+        # self.chk_cmsis.setToolTip(
+        #     "<span>Use CMSIS DSP second-order sections format "
+        #     "(only for IIR coefficients).</span>")
+        # self.chk_cmsis.setVisible(self.has_cmsis)
 
         lay_grid = QGridLayout()
+        lay_grid.addWidget(lbl_destination, 0, 1)
+        lay_grid.addWidget(self.cmb_destination, 0, 2)
         lay_grid.addWidget(lbl_delimiter, 1, 1)
         lay_grid.addWidget(self.cmb_delimiter, 1, 2)
         lay_grid.addWidget(lbl_terminator, 2, 1)
         lay_grid.addWidget(self.cmb_terminator, 2, 2)
         lay_grid.addWidget(lbl_orientation, 3, 1)
         lay_grid.addWidget(self.cmb_orientation, 3, 2)
         lay_grid.addWidget(lbl_header, 4, 1)
         lay_grid.addWidget(self.cmb_header, 4, 2)
-        lay_grid.addWidget(lbl_cmsis, 5, 1)
-        lay_grid.addWidget(self.chk_cmsis, 5, 2)
-        lay_grid.addWidget(self.radClipboard, 6, 1)
-        lay_grid.addWidget(self.radFile, 6, 2)
+        # lay_grid.addWidget(lbl_cmsis, 5, 1)
+        # lay_grid.addWidget(self.chk_cmsis, 5, 2)
 
         layVMain = QVBoxLayout()
         # layVMain.setAlignment(Qt.AlignTop) # only affects first widget (intended here)
         layVMain.addLayout(lay_grid)
         layVMain.addWidget(butClose)
         layVMain.setContentsMargins(*params['wdg_margins'])
         self.setLayout(layVMain)
 
         self.load_settings()
 
         # ============== Signals & Slots ================================
         butClose.clicked.connect(self.close)
+        self.cmb_destination.currentIndexChanged.connect(self.store_settings)
         self.cmb_orientation.currentIndexChanged.connect(self.store_settings)
         self.cmb_delimiter.currentIndexChanged.connect(self.store_settings)
         self.cmb_terminator.currentIndexChanged.connect(self.store_settings)
         self.cmb_header.currentIndexChanged.connect(self.store_settings)
-        self.chk_cmsis.clicked.connect(self.store_settings)
-        self.radClipboard.clicked.connect(self.store_settings)
-        self.radFile.clicked.connect(self.store_settings)
+        # self.chk_cmsis.clicked.connect(self.store_settings)
 
     def store_settings(self):
         """
         Store settings of CSV options widget in ``pyfda_rc.params``.
         """
 
         try:
             params['CSV']['orientation'] = qget_cmb_box(self.cmb_orientation, data=True)
             params['CSV']['delimiter'] = qget_cmb_box(self.cmb_delimiter, data=True)
             params['CSV']['lineterminator'] = qget_cmb_box(self.cmb_terminator,
                                                            data=True)
             params['CSV']['header'] = qget_cmb_box(self.cmb_header, data=True)
-            params['CSV']['cmsis'] = self.chk_cmsis.isChecked()
-            params['CSV']['clipboard'] = self.radClipboard.isChecked()
-
+            # params['CSV']['cmsis'] = self.chk_cmsis.isChecked()
+            params['CSV']['destination'] = qget_cmb_box(self.cmb_destination, data=True)
             self.emit({'ui_global_changed': 'csv'})
 
         except KeyError as e:
             logger.error(e)
 
     def load_settings(self):
         """
@@ -194,18 +195,16 @@
         """
         try:
             qset_cmb_box(self.cmb_orientation, params['CSV']['orientation'], data=True)
             qset_cmb_box(self.cmb_delimiter, params['CSV']['delimiter'], data=True)
             qset_cmb_box(self.cmb_terminator, params['CSV']['lineterminator'],
                          data=True)
             qset_cmb_box(self.cmb_header, params['CSV']['header'], data=True)
-            self.chk_cmsis.setChecked(params['CSV']['cmsis'])
-
-            self.radClipboard.setChecked(params['CSV']['clipboard'])
-            self.radFile.setChecked(not params['CSV']['clipboard'])
+            # self.chk_cmsis.setChecked(params['CSV']['cmsis'])
+            qset_cmb_box(self.cmb_destination, params['CSV']['destination'], data=True)
 
         except KeyError as e:
             logger.error(f"Unknown key {e}")
 
 
 # ==============================================================================
 if __name__ == '__main__':
```

### Comparing `pyfda-0.8.4/pyfda/libs/frozendict.py` & `pyfda-0.9.0b1/pyfda/libs/frozendict.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_dirs.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_dirs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_fft_windows_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_fft_windows_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,18 +547,19 @@
     # instance. This is not a problem as signals are distinguished by the attached
     # dict with the payload
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing
 
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, win_dict):
+    def __init__(self, win_dict, objectName=""):
         super().__init__()
 
         self.win_dict = win_dict
+        self.setObjectName(objectName)
         self.err = False  # error flag for window calculation
         self._construct_UI()
         self.set_window_name()  # initialize win_dict
         self.ui2dict_win()
 
     # --------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
@@ -594,24 +595,22 @@
         # Variant of FFT window type (not implemented yet)
         self.cmb_win_fft_variant = QComboBox(self)
         self.cmb_win_fft_variant.setToolTip("FFT window variant.")
         self.cmb_win_fft_variant.setVisible(False)
 
         # First numeric parameter for FFT window
         self.lbl_win_par_0 = QLabel("Param1")
-        self.led_win_par_0 = QLineEdit(self)
+        self.led_win_par_0 = QLineEdit(self, objectName="ledWinPar1")
         self.led_win_par_0.setText("1")
-        self.led_win_par_0.setObjectName("ledWinPar1")
         self.cmb_win_par_0 = QComboBox(self)
 
         # Second numeric parameter for FFT window
         self.lbl_win_par_1 = QLabel("Param2")
-        self.led_win_par_1 = QLineEdit(self)
+        self.led_win_par_1 = QLineEdit(self, objectName="ledWinPar2")
         self.led_win_par_1.setText("2")
-        self.led_win_par_1.setObjectName("ledWinPar2")
         self.cmb_win_par_1 = QComboBox(self)
 
         layH_main = QHBoxLayout(self)
         layH_main.addWidget(self.cmb_win_fft)
         layH_main.addWidget(self.cmb_win_fft_variant)
         layH_main.addWidget(self.lbl_win_par_0)
         layH_main.addWidget(self.led_win_par_0)
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_fix_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_fix_lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,41 +9,43 @@
 """
 Fixpoint library for converting numpy scalars and arrays to quantized
 numpy values and formatting reals in various formats
 """
 # ===========================================================================
 import re
 import inspect
+import copy
 
+import pyfda.filterbroker as fb
 import numpy as np
 from numpy.lib.function_base import iterable
+from pyfda.libs.pyfda_lib import is_numeric, pprint_log
 try:
     import deltasigma as ds
     from deltasigma import simulateDSM, synthesizeNTF
     print("DS Backends:", ds.simulation_backends)
     DS = True
 except ImportError:
     DS = False
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 # TODO: Absolute value for WI is taken, no negative WI specifications possible
-# TODO: Vecorization for hex / csd functions (frmt2float)
 
 __version__ = 0.6
 
 
 def qstr(text):
     """ carefully replace qstr() function - only needed for Py2 compatibility """
     return str(text)
 
 
-def bin2hex(bin_str, WI=0):
+def bin2hex(bin_str: str, WI=0) -> str:
     """
     Convert number `bin_str` in binary format to hex formatted string.
     `bin_str` is prepended / appended with zeros until the number of bits before
     and after the radix point (position given by `WI`) is a multiple of 4.
     """
 
     wmap = {
@@ -100,14 +102,75 @@
     hex_str = "0" if len(hex_str) == 0 else hex_str
     return hex_str
 
 
 bin2hex_vec = np.vectorize(bin2hex)  # safer than frompyfunction()
 
 
+# ---------------------------------------------------------------------
+def bin2oct(bin_str: str, WI=0) -> str:
+    """
+    Convert number `bin_str` in binary format to octal formatted string.
+    `bin_str` is prepended / appended with zeros until the number of bits before
+    and after the radix point (position given by `WI`) is a multiple of 3.
+    """
+
+    wmap = {
+        '000': '0',
+        '001': '1',
+        '010': '2',
+        '011': '3',
+        '100': '4',
+        '101': '5',
+        '110': '6',
+        '111': '7',
+        }
+
+    oct_str = ""
+
+    # --- integer part ----------------------------
+    if WI > 0:
+        # slice string with integer bits and prepend with zeros to obtain a
+        # multiple of 3 length:
+        bin_i_str = bin_str[:WI+1]
+        while (len(bin_i_str) % 3 != 0):
+            bin_i_str = "0" + bin_i_str
+
+        i = 0
+        while (i < len(bin_i_str)):  # map chunks of 3 binary bits to one oct digit
+            oct_str = oct_str + wmap[bin_i_str[i:i + 3]]
+            i = i + 3
+    else:
+        oct_str = bin_str[0]  # copy MSB as sign bit
+
+    # --- fractional part -------------------------
+    WF = len(bin_str) - WI - 1
+    # slice string with fractional bits and append with zeros to obtain a
+    # multiple of 3 length:
+    if WF > 0:
+        oct_str = oct_str + '.'
+        bin_f_str = bin_str[WI+1:]
+
+        while (len(bin_f_str) % 3 != 0):
+            bin_f_str = bin_f_str + "0"
+
+        # map chunks of 3 binary bits to one octal digit
+        i = 0
+        while (i < len(bin_f_str)):
+            oct_str = oct_str + wmap[bin_f_str[i:i + 3]]
+            i = i + 3
+
+    # oct_str = oct_str.lstrip("0") # remove leading zeros
+    oct_str = "0" if len(oct_str) == 0 else oct_str
+    return oct_str
+
+
+bin2oct_vec = np.vectorize(bin2oct)  # safer than frompyfunction()
+
+
 # ------------------------------------------------------------------------------
 def dec2hex(val, nbits, WF=0):
     """
     --- currently not used, no unit test ---
 
     Return `val` in hex format with a wordlength of `nbits` in two's complement
     format. The built-in hex function returns args < 0 as negative values.
@@ -284,45 +347,37 @@
 csd2dec_vec = np.vectorize(csd2dec)  # safer than np.frompyfunc()
 
 
 # ------------------------------------------------------------------------
 class Fixed(object):
     """
     Implement binary quantization of signed scalar or array-like objects
-    in the form `Q = WI.WF` where WI and WF are the wordlength of integer resp.
+    in the form WI.WF where WI and WF are the wordlength of integer resp.
     fractional part; total wordlength is `W = WI + WF + 1` due to the sign bit.
 
     Examples
     --------
 
     Define a dictionary with the format options and pass it to the constructor:
 
-    >>> q_dict = {'WI':1, 'WF':14, 'ovfl':'sat', 'quant':'round'} # or
-    >>> q_dict = {'Q':'1.14', 'ovfl':'none', 'quant':'round'}
-    >>> myQ = Fixed(q_dict)
+    >>> q_dict = {'WI':1, 'WF':14, 'ovfl':'sat', 'quant':'round'}
+    >>> myQ = Fixed(q_dict)  # instantiate fixpoint quantizer
+    >>> WI = myQ.q_dict['WI']  # access quantizer parameters
+    >>> myQ.set_qdict({'WF': 13, 'WI': 2})  # update quantizer parameters
 
 
     Parameters
     ----------
     q_dict : dict
         define quantization options with the following keys
 
-    * **'WG'** : number of guard bits, default: 0
-
     * **'WI'** : number of integer bits, default: 0
 
     * **'WF'** : number of fractional bits; default: 15
 
-    * **'W'**  : total word length; WI + WF + 1 = W (1 sign bit). When WI and / or
-                 WF are missing, WI = W - 1 and WF = 0.
-
-    * **'Q'**  : Quantization format as string, e.g. '0.15', it is translated
-                 to`WI` and `WF`. When both `Q` and `WI` / `WF`
-                 are given, `Q` is ignored
-
     * **'quant'** : Quantization method, optional; default = 'floor'
 
       - 'floor': (default) largest integer `I` such that :math:`I \\le x`
                  (= binary truncation)
       - 'round': (binary) rounding
       - 'fix': round to nearest integer towards zero ('Betragsschneiden')
       - 'ceil': smallest integer `I`, such that :math:`I \\ge x`
@@ -331,129 +386,112 @@
 
     * **'ovfl'** : Overflow method, optional; default = 'wrap'
 
       - 'wrap': do a two's complement wrap-around
       - 'sat' : saturate at minimum / maximum value
       - 'none': no overflow; the integer word length is ignored
 
-    Additionally, the following keys define the base / display format for the
-    fixpoint number:
-
-    * **'fx_base'** : Output format, optional; default = 'float'
+    * **N_over** : integer
+        total number of overflows (should be considered as read-only)
 
-      - 'float' : (default)
-      - 'dec'  : decimal integer, scaled by :math:`2^{WF}`
-      - 'bin'  : binary string, scaled by :math:`2^{WF}`
-      - 'hex'  : hex string, scaled by :math:`2^{WF}`
-      - 'csd'  : canonically signed digit string, scaled by :math:`2^{WF}`
+    Additionally, the following keys from global dict `fb.fil[0]` define the
+    number base and quantization/overflow behaviour for fixpoint numbers:
 
-    * **'scale'** : Float or a keyword, the factor between the fixpoint integer
-            representation (FXP) and its "real world" floating point value (RWV).
-            If ``scale`` is a float, this value is used, RWV = FXP / scale.
-            By default, scale = 1 << WI.
+    * **`'fx_sim'`** : Flag for fixpoint mode, default = False (floating point)
 
-            Examples:
-                WI.WF = 3.0, FXP = "b0110." = 6,   scale = 8 -> RWV = 6 / 8   = 0.75
-                WI.WF = 1.2, FXP = "b01.10" = 1.5, scale = 2 -> RWV = 1.5 / 2 = 0.75
+    * **`'fx_base'`** : Display format for fixpoint number base; default = 'dec'
 
-            Alternatively, if:
+      - 'dec'   : decimal (base = 10)
+      - 'bin'   : binary (base = 2)
+      - 'hex'   : hexadecimal (base = 16)
+      - 'oct'   : octal (base = 8)
+      - 'csd'   : canonically signed digit (base = "3")
 
-                - ``q_dict['scale'] == 'int'``:   scale = 1 << self.q_dict['WF']
+    * **`'qfrmt'`** : Quantization / overflow behaviour, default = 'qfrac'
 
-                - ``q_dict['scale'] == 'norm'``:  scale = 2.**(-self.q_dict['WI'])
-    * **quant** : str
-        Quantization behaviour ('floor', 'round', ...)
-
-    * **'ovfl'**  : str
-        Overflow behaviour ('wrap', 'sat', ...)
-
-    * **'fx_base'** : str
-        target output format ('float', 'dec', 'bin', 'hex', 'csd')
+      - 'qint'   : fixpoint integer format
+      - 'qfrac'  : fractional fixpoint format
 
+    Attributes
+    ----------
+    q_dict : dict
+        A reference to the quantization dictionary passed during construction
+        (see above). This dictionary is updated here and can be accessed from
+        outside.
 
-    The following key: value pairs are calculated from other parameters and
-    can / should be considered as read-only.
+    LSB : float
+        value of LSB (smallest quantization step), `self.LSB = 2 ** -q_dict['WF']`
 
-    * **'places'** : integer
-        number of places required for printing in the selected number format.
-        For binary formats, this is the same as the wordlength. Calculated
-        from the numeric base 'self.base' (not used outside this class) and
-        the total word length 'W'.
+    MSB : float
+        value of most significant bit (MSB),  `self.MSB = 2 ** (q_dict['WI'] - 1)`
 
-    * **'LSB'** : float
-        value of LSB (smallest quantization step), calculated from `WI` and `WF`
+    MIN : float
+        most negative representable value, `self.MIN = -2 * self.MSB`
 
-    * **'MSB'** : float
-        value of most significant bit (MSB), calculated from `WI` and `WF`
+    MAX : float
+        largest representable value, `self.MAX = 2 * self.MSB - self.LSB`
 
-    * **'MIN'** : float
-        most negative representable value, calculated from `WI` and `WF`
+    N : integer
+        total number of simulation data points
 
-    * **'MAX'** : float
-        largest representable value, calculated from `WI` and `WF`
+    N_over_neg : integer
+        number of negative overflows
 
-    Overflow flags and counters are set in `self.fixp()` and reset in `self.reset_N()`
+    N_over_pos : integer
+        number of positive overflows
 
-    * **'ovr_flag'** : integer or integer array (same shape as input argument)
+    ovr_flag: integer or integer array (same shape as input argument)
         overflow flag, meaning:
 
-                        0 : no overflow
+            0 : no overflow
 
-                        +1: positive overflow
+            +1: positive overflow
 
-                        -1: negative overflow
+            -1: negative overflow
 
         has occured during last fixpoint conversion.
 
-    * **'N'** : integer
-        total number of simulation data points
-
-    * **'N_over'** : integer
-        total number of overflows
-
-    * **'N_over_neg'** : integer
-        number of negative overflows
-
-    * **'N_over_pos'** : integer
-        number of positive overflows
+    places : integer
+        number of places required for printing in the selected 'fx_base' format.
+        For binary formats, this is the same as the wordlength. Calculated
+        from the numeric base 'fx_base' and the total word length WI + WF + 1.
 
-    Attributes
-    ----------
-    q_dict : dict
-        A reference to the quantization dictionary passed during construction
-        (see above). This dictionary is updated here and can be accessed from
-        outside.
+    Overflow flags and counters are set in `self.fixp()` and reset in `self.reset_N()`
 
     Example
     -------
     class `Fixed()` can be used like Matlabs quantizer object / function from the
     fixpoint toolbox, see (Matlab) 'help round' and 'help quantizer/round' e.g.
 
-    >>> q_dsp = quantizer('fixed', 'round', [16 15], 'wrap'); % Matlab
+    MATLAB:
+    >>> q_dsp = quantizer('fixed', 'round', [16 15], 'wrap');
     >>> yq = quantize(q_dsp, y)
 
-    >>> q_dsp = {'Q':'0.15', 'quant':'round', 'ovfl':'wrap'} # Python
+    PYTHON
+    >>> q_dsp = {'WI':0, 'WF': 15, 'quant':'round', 'ovfl':'wrap'}
     >>> my_q = Fixed(q_dsp)
     >>> yq = my_q.fixp(y)
-
     """
 
     def __init__(self, q_dict):
         """
         Construct `Fixed` object with dict `q_dict`
         """
         # define valid keys and default values for quantization dict
         self.q_dict_default = {
-            'WG': 0, 'WI': 0, 'WF': 15, 'W': 16, 'Q': '0.15', 'quant': 'round',
-            'ovfl': 'sat', 'fx_base': 'float', 'qfrmt': 'qfrac', 'qfrmt_last': 'qfrac',
-            'scale': 1}
+            'WI': 0, 'WF': 15, 'w_a_m': 'm', 'quant': 'round', 'ovfl': 'sat',
         # these keys are calculated and should be regarded as read-only
-        self.q_dict_default_ro = {
-            'N': 0, 'ovr_flag': 0, 'N_over': 0, 'N_over_neg': 0, 'N_over_pos': 0,
-            'MSB': 1, 'LSB': 6, 'MAX': 2, 'MIN': -2, 'places': 4}
+            'N_over': 0}
+        # these attributes are calculated and should be regarded as read-only
+        self.LSB = 2. ** -self.q_dict_default['WF']
+        self.MSB = 2. ** (self.q_dict_default['WI'] - 1)
+        self.MAX = 2 * self.MSB - self.LSB
+        self.MIN = -2 * self.MSB
+
+        self.N = 0
 
         # test if all passed keys of quantizer object are valid
         self.verify_q_dict_keys(q_dict)
 
         # missing key-value pairs are taken from the default dict
         for k in self.q_dict_default.keys():  # loop over all defined keys
             if k not in q_dict.keys():  # key is not in passed dict, get k:v pair from ...
@@ -464,253 +502,260 @@
 
         self.set_qdict({})  # trigger calculation of parameters
         self.resetN()       # initialize overflow-counter
 
         # arguments for regex replacement with illegal characters
         # ^ means "not", | means "or" and \ escapes
         self.FRMT_REGEX = {
-                'bin': r'[^0|1|.|,|\-]',
-                'csd': r'[^0|\+|\-|.|,]',
                 'dec': r'[^0-9Ee|.|,|\-]',
-                'hex': r'[^0-9A-Fa-f|.|,|\-]'
+                'bin': r'[^0|1|.|,|\-]',
+                'oct': r'[^0-7|.|,|\-]',
+                'hex': r'[^0-9A-Fa-f|.|,|\-]',
+                'csd': r'[^0|\+|\-|.|,]'
                         }
-        # provide frmt2float function for arrays, swallow the `self` argument
+        # --------------------------------------------------------------------------
+        # vectorize frmt2float function for arrays, swallow the `self` argument
         self.frmt2float_vec = np.vectorize(self.frmt2float_scalar, excluded='self')
 
     def verify_q_dict_keys(self, q_dict: dict) -> None:
         """
-        Check against the merged `self.q_dict_default` and `self.q_dict_default_ro`
-        dictionaries whether all keys in the passed `q_dict` dictionary are valid.
+        Check against `self.q_dict_default` dictionary
+        whether all keys in the passed `q_dict` dictionary are valid.
 
-        Unknown keys throw an error message
+        Unknown keys throw an error message.
         """
         for k in q_dict.keys():
-            if k not in {**self.q_dict_default, **self.q_dict_default_ro}.keys():
+            if k not in self.q_dict_default:
                 logger.error(u'Unknown Key "{0:s}"!'.format(k))
 
+# ------------------------------------------------------------------------------
     def set_qdict(self, d: dict) -> None:
         """
-        Update the instance quantization dict `self.q_dict` from parameter `d`:
+        Update the instance quantization dict `self.q_dict` from passed dict `d`:
 
-        * Transform dict entries for `WF`, `WI`, `W` and `Q` into each other
-
-        * Calculate parameters `MSB`, `LSB`, `MIN` and `MAX` from quantization params
-
-        * Calculate number of places required for printing from `fx_base` and `W`
-
-        When the passed dictionary `d` is empty, update the quantization dict from
-        its `WF` and `WI` entries.
+        * Sanitize `WI` and `WF`
+        * Calculate attributes `MSB`, `LSB`, `MIN` and `MAX`
+        * Calculate number of places needed for printing from `qfrmt`,`fx_base` and `W`
+          and store it as attribute `self.places`
 
         Check the docstring of class `Fixed()` for details on quantization
         """
-        q_d = d.copy()  # create local copy to avoid modification of passed dict
-
-        self.verify_q_dict_keys(q_d)  # check whether all keys are valid
-
-        # Transform `WG`,  `WI`, `WF`, `W` and `Q` parameters into each other
-        if q_d == {}:
-            q_d['W'] = self.q_dict['WG'] + self.q_dict['WI'] + self.q_dict['WF'] + 1
-            q_d['Q'] = str(self.q_dict['WG'] + self.q_dict['WI']) + "."\
-                + str(self.q_dict['WF'])
-        elif 'WI' in q_d and 'WF' in q_d:
-            if 'WG' in q_d:
-                q_d['WG'] = abs(int(q_d['WG']))  # sanitize WG
-            else:
-                q_d['WG'] = 0
-            q_d['WI'] = int(q_d['WI'])  # sanitize WI
-            q_d['WF'] = abs(int(q_d['WF']))  # and WF
-            q_d['W'] = q_d['WG'] + q_d['WI'] + q_d['WF'] + 1
-            q_d['Q'] = str(q_d['WI']) + "." + str(q_d['WF'])
-        elif 'W' in q_d:
-            q_d['W'] = int(q_d['W'])  # sanitize W
-            q_d['WG'] = 0
-            q_d['WI'] = int(q_d['W']) - 1
-            q_d['WF'] = 0
-            q_d['Q'] = str(q_d['WI']) + ".0"
-        elif 'Q' in q_d:
-            Q_str = str(q_d['Q']).split('.', 1)  # split 'Q':'1.4'
-            q_d['WG'] = 0
-            q_d['WI'] = int(Q_str[0])
-            q_d['WF'] = abs(int(Q_str[1]))
-            q_d['W'] = q_d['WI'] + q_d['WF'] + 1
+        self.verify_q_dict_keys(d)  # check whether all keys are valid
+        self.q_dict.update(d)  # merge d into self.q_dict
 
-        self.q_dict.update(q_d)  # merge q_d into self.q_dict
+        # sanitize WI and WF
+        self.q_dict['WI'] = int(self.q_dict['WI'])
+        self.q_dict['WF'] = abs(int(self.q_dict['WF']))
 
         # Calculate min., max., LSB and MSB from word lengths
-        self.q_dict['LSB'] = 2. ** -self.q_dict['WF']
-        self.q_dict['MSB'] = 2. ** (self.q_dict['WG'] + self.q_dict['WI'] - 1)
+        if fb.fil[0]['qfrmt'] == 'qint':
+            # LSB = 1, MSB = 2 ** (W - 1)
+            self.LSB = 1
+            self.MSB = 2 ** (self.q_dict['WI'] + self.q_dict['WF']- 1)
+        else:
+            self.LSB = 2. ** -self.q_dict['WF']
+            self.MSB = 2. ** (self.q_dict['WI'] - 1)
 
-        self.q_dict['MAX'] =  2. * self.q_dict['MSB'] - self.q_dict['LSB']
-        self.q_dict['MIN'] = -2. * self.q_dict['MSB']
+        self.MAX =  2. * self.MSB - self.LSB
+        self.MIN = -2. * self.MSB
 
         # Calculate required number of places for different bases from total
         # number of bits:
-        if self.q_dict['fx_base'] == 'dec':
-            self.q_dict['places'] = int(
-                np.ceil(np.log10(self.q_dict['W']) * np.log10(2.))) + 1
-            self.base = 10
-        elif self.q_dict['fx_base'] == 'bin':
-            self.q_dict['places'] = self.q_dict['W'] + 1
-            self.base = 2
-        elif self.q_dict['fx_base'] == 'csd':
-            self.q_dict['places'] = self.q_dict['W'] + 1
-            self.base = 2
-        elif self.q_dict['fx_base'] == 'hex':
-            self.q_dict['places'] = int(np.ceil(self.q_dict['W'] / 4.)) + 1
-            self.base = 16
-        elif self.q_dict['fx_base'] == 'float':
-            self.q_dict['places'] = 4
-            self.base = 0
+        W = self.q_dict['WI'] + self.q_dict['WF'] + 1
+        #
+        if not fb.fil[0]['fx_sim']:  # float format
+            self.places = 4
+        elif fb.fil[0]['fx_base'] == 'dec':
+            self.places = int(
+                np.ceil(np.log10(W) * np.log10(2.))) + 1
+        elif fb.fil[0]['fx_base'] == 'bin':
+            self.places = W + 1
+        elif fb.fil[0]['fx_base'] == 'csd':
+            self.places = int(np.ceil(W / 1.5)) + 1
+        elif fb.fil[0]['fx_base'] == 'hex':
+            self.places = int(np.ceil(W / 4.)) + 1
+        elif fb.fil[0]['fx_base'] == 'oct':
+            self.places = int(np.ceil(W / 3.)) + 1
         else:
             raise Exception(
-                u'Unknown number format "{0:s}"!'.format(self.q_dict['fx_base']))
+                u'Unknown number format "{0:s}"!'.format(fb.fil[0]['fx_base']))
 
 # ------------------------------------------------------------------------------
-    def fixp(self, y, scaling='mult'):
+    def fixp(self, y, in_frmt: str = 'qfrac', out_frmt: str = 'qfrac'):
         """
-        Return fixed-point integer or fractional representation for `y`
-        (scalar or array-like) with the same shape as `y`.
+        Return a quantized copy `yq` for `y` (scalar or array-like) with the same
+        shape as `y`. The returned data is always in float format, use float2frmt()
+        to obtain different number formats.
+
+        This is used a.o. by the following methods / classes:
+
+        - frmt2float(): always returns a float with RWV
+        - float2frmt(): starts with RWV, passes on the scaling argument
+        - input_coeffs: uses both methods above when quantizing coefficients
 
         Saturation / two's complement wrapping happens outside the range +/- MSB,
         requantization (round, floor, fix, ...) is applied on the ratio `y / LSB`.
 
+        * Fractional number format WI.WF ('qfrmt':'qfrac'): *
+        `LSB =  2 ** -WF`
+
+        - Multiply float input by `1 / self.LSB = 2**WF`, obtaining integer scale
+        - Quantize
+        - Scale back by multiplying with `self.LSB` to restore fractional point
+        - Find pos. and neg. overflows and replace them by wrapped or saturated
+          values
+
+        * Integer number format W = 1 + WI + WF ('qfrmt':'qint'): *
+        `LSB = 1`
+
+        - Multiply float input by `2 ** WF` to obtain integer scale
+        - Quantize and treat overflows in integer scale
+
         Parameters
         ----------
-        y: scalar or array-like object
+        y: scalar or array-like object of float
             input value (floating point format) to be quantized
 
-        scaling: String
-            Determine the scaling before and after quantizing / saturation
+        in_frmt: str
+            Determine the scaling before quantizing / saturation
 
-            *'mult'* float in, int out:
-                `y` is multiplied by `self.q_dict['scale'])` *before* quantizing / saturating
-            **'div'**: int in, float out:
-                `y` is divided by `scale` *after* quantizing / saturating.
-            **'multdiv'**: float in, float out (default):
-                both of the above
+            *'qfrac'* (default): fractional float input
+                `y` is multiplied by `2 ** WF` *before* quantizing / saturating
+
+        out_frmt: str
+            Determine the scaling after quantizing / saturation
+            **'qfrac'** (default): fractional fixpoint output format
+                `y` is divided by `2 ** WF` *after* quantizing / saturating.
 
             For all other settings, `y` is transformed unscaled.
 
         Returns
         -------
-        float scalar or ndarray
+        yq: float scalar or ndarray
             with the same shape as `y`, in the range
-            `-2*self.q_dict['MSB']` ... `2*self.q_dict['MSB']-self.q_dict['LSB']`
+            `-2 * self.MSB` ... `2 * self.MSB - self.LSB`
 
         Examples
         --------
 
         >>> q_obj_a = {'WI':1, 'WF':6, 'ovfl':'sat', 'quant':'round'}
         >>> myQa = Fixed(q_obj_a) # instantiate fixed-point object myQa
         >>> myQa.resetN()  # reset overflow counter
         >>> a = np.arange(0,5, 0.05) # create input signal
 
-        >>> aq = myQa.fixed(a) # quantize input signal
+        >>> aq = myQa.fixp(a) # quantize input signal
         >>> plt.plot(a, aq) # plot quantized vs. original signal
         >>> print(myQa.q_dict('N_over'), "overflows!") # print number of overflows
 
         >>> # Convert output to same format as input:
         >>> b = np.arange(200, dtype = np.int16)
         >>> btype = np.result_type(b)
         >>> # MSB = 2**7, LSB = 2**(-2):
         >>> q_obj_b = {'WI':7, 'WF':2, 'ovfl':'wrap', 'quant':'round'}
         >>> myQb = Fixed(q_obj_b) # instantiate fixed-point object myQb
-        >>> bq = myQb.fixed(b)
+        >>> bq = myQb.fixp(b)
         >>> bq = bq.astype(btype) # restore original variable type
         """
 
         # ======================================================================
         # (1) : INITIALIZATION
         #       Convert input argument into proper floating point scalars /
         #       arrays and initialize flags
         # ======================================================================
-        scaling = scaling.lower()
-        # use values from dict for initialization
-        N_over_neg = self.q_dict['N_over_neg']
-        N_over_pos = self.q_dict['N_over_pos']
-        N = self.q_dict['N']
+        if not fb.fil[0]['fx_sim']:
+            logger.warning(
+                "fixp() should only be called for fixpoint number format - returning floats!")
+            return y
+
+        if not in_frmt in {'qfrac', 'qint'}:
+            logger.error(f"Unknown input format {in_frmt}")
+        if not out_frmt in {'qfrac', 'qint'}:
+            logger.error(f"Unknown output format {out_frmt}")
+
+        # logger.error(f"fixp in: y = {pprint_log(y, N=4)}")
 
         if np.shape(y):
             # Input is an array:
             #   Create empty arrays for result and overflows with same shape as y
             #   for speedup, test for invalid types
             SCALAR = False
             y = np.asarray(y)  # convert lists / tuples / ... to numpy arrays
             yq = np.zeros(y.shape)
             over_pos = over_neg = np.zeros(y.shape, dtype=bool)
-            ovr_flag = np.zeros(y.shape, dtype=int)
+            self.ovr_flag = np.zeros(y.shape, dtype=int)
 
-            if np.issubdtype(y.dtype, np.number):  # numpy number type
-                N += y.size
+            if np.issubdtype(y.dtype, np.number):
+                # numpy number type (usual case), proceed with test for complex value
+                self.N += y.size
             elif y.dtype.kind in {'U', 'S'}:  # string or unicode
                 try:
                     y = y.astype(np.float64)  # try to convert to float
-                    N += y.size
+                    self.N += y.size
                 except (TypeError, ValueError):
                     try:
                         np.char.replace(y, ' ', '')  # remove all whitespace
                         y = y.astype(complex)  # try to convert to complex
-                        N += y.size * 2
+                        self.N += y.size * 2
                     # try converting elements recursively:
-                    except (TypeError, ValueError):
-                        y = np.asarray(list(map(lambda y_scalar:
-                                            self.fixp(y_scalar, scaling=scaling), y)))
-                        N += y.size
+                    except (TypeError, ValueError) as e:
+                        yq = np.asarray(
+                            list(map(lambda y_scalar:\
+                                     self.fixp(y_scalar, in_frmt=in_frmt, out_frmt=out_frmt),
+                                     y)))
+                        self.N += y.size
+                        return yq
             else:
-                logger.error("Argument '{0}' is of type '{1}',\n"
-                             "cannot convert to float.".format(y, y.dtype))
+                logger.error(f"Argument '{y}' is of type '{y.dtype}',\n"
+                             "cannot convert to float or complex.")
                 y = np.zeros(y.shape)
         else:
             # Input is a scalar
             SCALAR = True
             # get rid of errors that have occurred upstream
             if y is None or str(y) == "":
                 y = 0
             # If y is not a number, remove whitespace and try to convert to
-            # to float and or to complex format:
+            # float and or to complex format:
             elif not np.issubdtype(type(y), np.number):
+                # logger.error(f"Quantize string {y}")
                 y = str(y)
                 y = y.replace(' ', '')  # remove all whitespace
                 try:
                     y = float(y)
                 except (TypeError, ValueError):
                     try:
                         y = complex(y)
                     except (TypeError, ValueError) as e:
                         logger.error(f"'{y}' cannot be converted to a number.")
                         y = 0.0
             over_pos = over_neg = yq = 0
-            ovr_flag = 0
-            N += 1
+            self.N += 1
 
-        # convert pseudo-complex (imag = 0) and complex values to real
+        # convert pseudo-complex (imag = 0) to real
         y = np.real_if_close(y)
+        # quantize complex values separately and recursively
         if np.iscomplexobj(y):
-            logger.warning("Casting complex values to real before quantization!")
-            # quantizing complex objects is not supported yet
-            y = y.real
+            yq = self.fixp(y.real, in_frmt=in_frmt, out_frmt=out_frmt) +\
+                 self.fixp(y.imag, in_frmt=in_frmt, out_frmt=out_frmt) * 1j
+            return yq
 
-        y_in = y  # y before scaling / quantizing
         # ======================================================================
-        # (2) : INPUT SCALING
-        #       Multiply by `scale` factor before requantization and saturation
-        #       when `scaling=='mult'`or 'multdiv'
-        # ======================================================================
-        if scaling in {'mult', 'multdiv'}:
-            y = y * self.q_dict['scale']
+        # logger.error(f"fixp: in_frmt = '{in_frmt}', out_frmt = '{out_frmt}'")
 
         # ======================================================================
-        # (3) : QUANTIZATION
-        #       Divide by LSB to obtain an intermediate format where the
-        #       quantization step size = 1.
+        # (2) : QUANTIZATION
+        #       For `in_frmt=='qfrac'`, multiply by 2**WF = 1/LSB to obtain an
+        #       intermediate format with quantization step size of 1.
         #       Next, apply selected quantization method to convert
         #       floating point inputs to "fixpoint integers".
-        #       Finally, multiply by LSB to restore original scale.
         # ======================================================================
-        y = y / self.q_dict['LSB']
+        if in_frmt == 'qfrac':
+            y = y * (2. ** self.q_dict['WF'])
+
+        # logger.error(f"fixp (in:scaled): {pprint_log(y, N=4)}")
 
         if self.q_dict['quant'] == 'floor':
             yq = np.floor(y)  # largest integer i, such that i <= x (= binary truncation)
         elif self.q_dict['quant'] == 'round':
             yq = np.round(y)  # rounding, also = binary rounding
         elif self.q_dict['quant'] == 'fix':
             yq = np.fix(y)  # round to nearest integer towards zero ("Betragsschneiden")
@@ -721,446 +766,680 @@
         elif self.q_dict['quant'] == 'dsm':
             if DS:
                 # Synthesize DSM loop filter,
                 # TODO: parameters should be adjustable via quantizer dict
                 H = synthesizeNTF(order=3, osr=64, opt=1)
                 # Calculate DSM stream and shift/scale it from -1 ... +1 to
                 # 0 ... 1 sequence
-                yq = (simulateDSM(y*self.q_dict['LSB'], H)[0]+1)/(2*self.q_dict['LSB'])
+                yq = (simulateDSM(y*self.LSB, H)[0]+1)/(2*self.LSB)
                 # returns four ndarrays:
                 # v: quantizer output (-1 or 1)
                 # xn: modulator states.
                 # xmax: maximum value that each state reached during simulation
                 # y: The quantizer input (ie the modulator output).
             else:
                 raise Exception('"deltasigma" Toolbox not found.\n'
                                 'Try installing it with "pip install deltasigma".')
         elif self.q_dict['quant'] == 'none':
             yq = y  # return unquantized value
         else:
             raise Exception(
                 f'''Unknown Requantization type "{self.q_dict['quant']:s}"!''')
-        yq = yq * self.q_dict['LSB']
-        # logger.debug("y_in={0} | y={1} | yq={2}".format(y_in, y, yq))
 
-        # ======================================================================
-        # (4) : Handle Overflow / saturation w.r.t. to the MSB, returning a
-        #       result in the range MIN = -2*MSB ... + 2*MSB-LSB = MAX
-        # ====================================================================
+        # ========================================================================
+        # (3) : OVERFLOW / SATURATION
+        #       Handle Overflow / saturation w.r.t. to the MSB = 2 ** (W - 2),
+        #       returning a result in the range MIN = -2*MSB ... + 2*MSB-LSB = MAX
+        # ========================================================================
+        LSB = 1
+        MSB = 1 << (self.q_dict['WI'] + self.q_dict['WF'] - 1)  # 2 ** (W - 2)
+        MAX = 2 * MSB - LSB  # 2 ** (W - 1) - 1
+        MIN = - 2 * MSB
+
         if self.q_dict['ovfl'] == 'none':
-            pass
+            # set all overflow flags to zero
+            self.N_over_neg = self.N_over_pos = self.N_over = 0
         else:
             # Bool. vectors with '1' for every neg./pos overflow:
-            over_neg = (yq < self.q_dict['MIN'])
-            over_pos = (yq > self.q_dict['MAX'])
+            over_neg = (yq < MIN)
+            over_pos = (yq > MAX)
             # create flag / array of flags for pos. / neg. overflows
-            ovr_flag = over_pos.astype(int) - over_neg.astype(int)
+            self.ovr_flag = over_pos.astype(int) - over_neg.astype(int)
             # No. of pos. / neg. / all overflows occured since last reset:
-            N_over_neg += np.sum(over_neg)
-            N_over_pos += np.sum(over_pos)
-            N_over = N_over_neg + N_over_pos
-
-            self.q_dict.update(
-               {'N_over_pos': N_over_pos, 'N_over_neg': N_over_neg, 'N_over': N_over,
-                'N': N, 'ovr_flag': ovr_flag})
+            self.N_over_neg += np.sum(over_neg)
+            self.N_over_pos += np.sum(over_pos)
+            self.N_over = self.N_over_neg + self.N_over_pos
 
             # Replace overflows with Min/Max-Values (saturation):
             if self.q_dict['ovfl'] == 'sat':
-                yq = np.where(over_pos, self.q_dict['MAX'], yq)  # (cond, true, false)
-                yq = np.where(over_neg, self.q_dict['MIN'], yq)
+                yq = np.where(over_pos, MAX, yq)  # (cond, true, false)
+                yq = np.where(over_neg, MIN, yq)
             # Replace overflows by two's complement wraparound (wrap)
             elif self.q_dict['ovfl'] == 'wrap':
                 yq = np.where(
-                    over_pos | over_neg,
-                    yq - 4. * self.q_dict['MSB'] * np.fix(
-                        (np.sign(yq) * 2 * self.q_dict['MSB'] + yq)
-                            / (4 * self.q_dict['MSB'])), yq)
+                    over_pos | over_neg, yq - 4. * MSB * np.fix(
+                        (np.sign(yq) * 2 * MSB + yq) / (4 * MSB)), yq)
             else:
                 raise Exception(
                     f"""Unknown overflow type "{self.q_dict['ovfl']:s}"!""")
 
+        self.q_dict.update({'N_over': self.N_over})
+
         # ======================================================================
-        # (5) : OUTPUT SCALING
-        #       Divide result by `scale` factor when `scaling=='div'`or 'multdiv'
-        #       to obtain correct scaling for floats
-        #       - frmt2float() always returns float
-        #       - input_coeffs when quantizing the coefficients
-        #       float2frmt passes on the scaling argument
+        # (4) : OUTPUT SCALING
+        #       Divide result by `2 ** WF` factor for `out_frmt=='qint'` to obtain
+        #       quantized fractional number
         # ======================================================================
+        if out_frmt == 'qfrac':
+            yq = yq / (2. ** self.q_dict['WF'])
 
-        if scaling in {'div', 'multdiv'}:
-            yq = yq / self.q_dict['scale']
+        # logger.error(f"fixp: (out:scaled) = {pprint_log(yq, N=4)}")
 
         if SCALAR and isinstance(yq, np.ndarray):
             yq = yq.item()  # convert singleton array to scalar
 
         return yq
 
     # --------------------------------------------------------------------------
     def resetN(self):
         """ Reset counters and overflow-flag of Fixed object """
         frm = inspect.stack()[1]
         logger.debug("'reset_N' called from {0}.{1}():{2}.".
                      format(inspect.getmodule(frm[0]).__name__.split('.')[-1],
                             frm[3], frm[2]))
-        self.q_dict.update(
-            {'N': 0, 'N_over': 0, 'N_over_neg': 0, 'N_over_pos': 0, 'ovr_flag' : 0})
+        self.q_dict.update({'N_over': 0})
+
+        self.ovr_flag = 0
+        self.N_over_pos = 0
+        self.N_over_neg = 0
+        self.N_over = 0
+        self.N = 0
 
     # --------------------------------------------------------------------------
-    def frmt2float(self, y, frmt=None):
+    def requant(self, x_i, QI):
+        """
+        Change word length of input signal `x_i` with fractional and integer widths
+        defined by 'QI' to the word format defined by `self.q_dict` using the
+        quantization and saturaion methods specified by `self.q_dict['quant']` and
+        `self.q_dict['ovfl']`.
+
+        **Input and output word are aligned at their binary points.**
+
+        Parameters
+        ----------
+        self: Fixed() object
+            `self.qdict()` is the quantizer dict that specifies the output word format
+            and the requantizing / saturation methods to be used.
+
+        x_i: int, float or complex scalar or array-like
+            signal to be requantized with quantization format defined in quantizer QI
+
+        QI: quantizer
+            Quantizer for input word, only the keys 'WI' and 'WF' for integer
+            and fractional wordlength are evaluated.
+            `QI.q_dict['WI'] = 2` and `QI.q_dict['WF'] = 13` e.g. define Q-Format '2.13'
+            with 2 integer, 13 fractional bits and 1 implied sign bit = 16 bits total.
+
+        Returns
+        -------
+
+        y: requantized output data with same shape as input data, quantized as specified
+            in `self.qdict`.
+
+        Documentation
+        -------------
+
+        The following shows an example of rescaling an input word from Q2.4 to Q0.3
+        using wrap-around and truncation. It's easy to see that for simple wrap-around
+        logic, the sign of the result may change.
+
+        ::
+
+        S | WI1 | WI0 * WF0 | WF1 | WF2 | WF3  :  WI = 2, WF = 4, W = 7
+        0 |  1  |  0  *  1  |  0  |  1  |  1   =  43 (dec) or 43/16 = 2 + 11/16 (float)
+                      *
+                |  S  * WF0 | WF1 | WF2        :  WI = 0, WF = 3, W = 4
+                   0  *  1  |  0  |  1         =  7 (dec) or 7/8 (float)
+
+
+        When the input is integer format, the fractional value is calculated as an
+        intermediate representation by multiplying the integer value by 2 ** (-WF).
+        Integer and fractional part are truncated / extended to the output
+        quantization specifications.
+
+        Changes in the number of integer bits `dWI` and fractional bits `dWF` are
+        handled separately.
+
+        When operating on bit level in hardware, the following operations are used:
+
+        Fractional Bits
+        ---------------
+
+        - For reducing the number of fractional bits by `dWF`, simply right-shift the
+          integer number by `dWF`. For rounding, add '1' to the bit below the truncation
+          point before right-shifting.
+
+        - Extend the number of fractional bits by left-shifting the integer by `dWF`,
+          LSB's are filled with zeros.
+
+        Integer Bits
+        ------------
+
+        - For reducing the number of integer bits by `dWI`, simply right-shift the
+          integer by `dWI`.
+
+        - The number of fractional bits is SIGN-EXTENDED by filling up the left-most
+          bits with the sign bit.
+        """
+
+        WI_F = QI.q_dict['WF']  # number of fractional bits of input signal
+
+        # Convert input signal to fractional format if needed for aligning at fractional point
+        if fb.fil[0]['qfrmt'] == 'qint':
+            x_i_frac = x_i / (1 << WI_F)
+        else:
+            x_i_frac = x_i
+
+        # Quantize and saturate / overflow based on fractional output format and return
+        # either fractional or integer format, depending on `fb.fil[0]['qfrmt']`.
+        return self.fixp(x_i_frac, out_frmt=fb.fil[0]['qfrmt'])
+
+    # --------------------------------------------------------------------------
+    def frmt2float(self, y):
         """
         Return floating point representation for fixpoint `y` (scalar or array)
-        given in format `frmt`.
+        given in format `fb.fil[0]['fx_base']`.
 
         When input format is float, return unchanged.
 
         Else:
 
         - Remove illegal characters and leading '0's
         - Count number of fractional places `frc_places` and remove radix point
         - Calculate decimal, fractional representation `y_dec` of string,
           using the base and the number of fractional places
         - Calculate two's complement for `W` bits (only for negative bin and hex numbers)
-        - Calculate fixpoint float representation `y_float = fixp(y_dec, scaling='div')`,
-          dividing the result by `scale`.
+        - Calculate fixpoint float representation `y_float = fixp(y_dec, out_frmt='qfrmt')`,
+          dividing the result by `2**WF`.
 
         Parameters
         ----------
-        y: scalar or string or array of scalars or strings in number format 'fx_base'
-
-        frmt: string (optional)
-            any of the formats `float`, `dec`, `bin`, `hex`, `csd`)
-            When `frmt` is unspecified, the instance parameter `self.q_dict['fx_base']`
-            is used.
+        y: scalar or string or array of scalars or strings in number format float or
+            `fb.fil[0]['fx_base']` ('dec', 'hex', 'oct', 'bin' or 'csd')
 
         Returns
         -------
         Quantized floating point (`dtype=np.float64`) representation of input string
         of same shape as `y`.
         """
 
-        # ----------------------------------------------------------------------
-        if frmt is None:
-            frmt = self.q_dict['fx_base']
-        frmt = frmt.lower()
-
         if y is None:
             return 0
         elif np.isscalar(y):
             if not y:
                 return 0
             else:
                 if np.all((y == "")):
                     return np.zeros_like(y)
         if isinstance(y, np.str_):
-            # logger.warning("Input format 'np.str_' not supported!\n\t{0}".format(y))
+            # Convert 'np.str_' to "regular" string
             y = str(y)
 
-        y_float = y_dec = None
+        y_float = None
 
-        if frmt == 'float32':
-            float_frmt = np.float32
-            # TODO: not implemented yet
-        elif frmt == 'float16':
-            # TODO: not implemented yet
-            float_frmt = np.float16
-
-        if frmt == 'float':
+        if not fb.fil[0]['fx_sim']:
             # this handles floats, np scalars + arrays and strings / string arrays
             try:
                 y_float = np.float64(y)
             except ValueError:
                 try:
                     y_float = np.complex(y)
                 except Exception:
                     y_float = 0.0
                     logger.warning(
                         f'\n\tCannot convert "{y}" of type "{type(y).__name__}" '
                         f'to float or complex, setting to zero.')
             return y_float
-
+        # Convert various fixpoint formats to float
         elif np.isscalar(y):
-            return self.frmt2float_scalar(y, frmt=frmt)
+            return self.frmt2float_scalar(y)
         else:
-            return self.frmt2float_vec(y, frmt=frmt)
+            return self.frmt2float_vec(y)
 
     # --------------------------------------------------------------------------
-    def frmt2float_scalar(self, y, frmt=None):
+    def frmt2float_scalar(self, y: str) -> float:
         """
-        Convert the formats 'dec', 'bin', 'hex', 'csd' to float
+        Convert a string in 'dec', 'bin', 'oct', 'hex', 'csd' numeric format
+        to float.
+
+        - format is taken from the global `fb.fil[0]['fx_base']`
+        - maximum wordlength is determined from the local quantization dict keys
+          `self.q_dict['WI']` and `self.q_dict['WF']`
+        - negative numbers can be represented by a '-' sign or in two's complement
+        - represented numbers may be fractional and / or complex.
+        - the result is divided by 2**WF for `fb.fil[0]['qfrmt'] == 'qint'` in `fixp()`
+
+        Parameters
+        ----------
+        y: str
+            A string formatted as a decimal, binary, octal, hex or csd
+            number representation. The number string may contain a '.'
+            or ',' to represent fractal numbers. When the string contains a 'j'm
+            it is tried to split the string into real and imaginary part.
+
+        Returns
+        --------
+        float or complex
+            The float / complex representation of the string
 
-        Find the number of places before the first radix point (if there is one)
-        and join integer and fractional parts
-        when returned string is empty, skip general conversions and rely on
-        error handling of individual routines,
-        remove illegal characters and trailing zeros
         """
-        val_str = re.sub(self.FRMT_REGEX[frmt], r'', str(y)).lstrip('0')
+        # -----------------------------------------------------
+        def split_complex_str(y: str) -> tuple:
+            """
+            Parameters
+            ----------
+            y: str
+                A string containing a 'j', indicating a complex number
+                representation. Format can be decimal, binary or hex.
+                csd is not supported.
+
+            Returns
+            --------
+            tuple of str: (y_re, y_im)
+
+            Split string `y` into two parts at the + or - sign, separating
+            real and imaginary part. The sign at the beginning of the string
+            is ignored. Real and imaginary part are returned as a tuple.
+            """
+            # only keep allowed characters incl. 'j' and '+',
+            # remove leading zero(s) and convert to lower case
+            y = re.sub(self.FRMT_REGEX[frmt].replace(']', '|j\+]'),
+                       r'', str(y)).lstrip('0').lower()
+
+            # (?!^) : any position other than start of string
+            # (...) split without deleting the delimiter
+            # (?= ...) Matches if ... matches next, but doesn’t consume any
+            #          of the string (lookahead assertion).
+            # [+-][\d]: +/-[0 ... 9 or A ... F or .]
+            y1 = re.split(r"(?!^)(?=[+-][\.\da-fA-F])", y)
+
+            if len(y1) == 2:
+                if not 'j' in y1[0] and 'j' in y1[1]:  # re + im
+                    return y1[0], y1[1].replace('j','')
+                elif 'j' in y1[0] and not 'j' in y1[1]:  # im + re
+                    return y1[1], y1[0].replace('j','')
+                else:  # both parts are imaginary, combine them
+                    y_im = self.frmt2float(y1[0].replace('j',''))\
+                        + self.frmt2float(y1[1].replace('j',''))
+                    return "0", self.float2frmt(y_im)
+            elif len(y1) == 1: # purely imaginary, return 0 for re part
+                return "0", y1[0].replace('j', '')
+            else:
+                logger.error(
+                    f"String split into {len(y1)} parts - that's too many!")
+                return "0", "0"
+        # -----------------------------------------
+        y = str(y)
+        frmt = fb.fil[0]['fx_base']
+        # ======================================================================
+        # (1) : COMPLEX NUMBERS
+        #       Split strings containing 'j' into real and imaginary part,
+        #       calling `frmt2float` recursively
+        # ======================================================================
+        if 'j' in y:
+            y_re, y_im = split_complex_str(y)
+            return self.frmt2float(y_re) + self.frmt2float(y_im) * 1j
+
+        # ======================================================================
+        # (2) : CLEAN UP INPUT STRING
+        #       - remove illegal characters (depending on selected number format
+        #         defined in FRMT_REGEX(frmt)) from input string
+        #       - remove all leading '0' to sanitize cases like '0001' or '00.23'
+        #       - replace ',' by '.' for German style numbers
+        # ======================================================================
+        val_str = re.sub(
+            self.FRMT_REGEX[frmt], r'', y).lstrip('0').replace(',', '.')
+
+        # ======================================================================
+        # (3) : FRACTIONAL PLACES
+        #       - prepend '0' if string starts with '.' and store as `val_str`
+        #       - store number of fractional places in `frc_places` (all number
+        #         formats)
+        #       - store fractional part as `frc_str` and whole string without '.'
+        #         as `raw_str`
+        # ======================================================================
         if len(val_str) > 0:
-            val_str = val_str.replace(',', '.')  # ',' -> '.' for German-style numbers
-            if val_str[0] == '.':  # prepend '0' when the number starts with '.'
+            if val_str[0] == '.':
                 val_str = '0' + val_str
 
             # count number of fractional places in string
             try:
                 # split into integer and fractional places
                 _, frc_str = val_str.split('.')
                 frc_places = len(frc_str)
             except ValueError:  # no fractional part
                 frc_places = 0
 
             raw_str = val_str.replace('.', '')  # join integer and fractional part
-
             # logger.debug(f"y={y}, val_str={val_str}, raw_str={raw_str}")
         else:
             return 0.0
 
-        # (1) calculate the decimal value of the input string using np.float64()
-        #     which takes the number of decimal places into account.
-        # (2) quantize and saturate
-        # (3) divide by scale
+        # ======================================================================
+        # (4a): CONVERSION (DEC)
+        #       - calculate the decimal value of `val_str` directly using `fixp()`
+        #         which quantizes and calculates overflows
+        #       - divide by scale
+        # ======================================================================
         if frmt == 'dec':
             # try to convert string -> float directly with decimal point position
             try:
-                y_dec = y_float = self.fixp(val_str, scaling='div')
+                y_dec = y_float = self.fixp(val_str, in_frmt=fb.fil[0]['qfrmt'])
             except Exception as e:
                 logger.warning(e)
+                return 0.0
 
-        elif frmt in {'hex', 'bin'}:
-            # - Glue integer and fractional part to a string without radix point
-            # - Check for a negative sign, use this information only in the end
-            # - Divide by <base> ** <number of fractional places> for correct scaling
-            # - Strip MSBs outside fixpoint range
-            # - Transform numbers in negative 2's complement to negative floats.
-            # - Calculate the fixpoint representation for correct saturation /
-            #   quantization
+        # ======================================================================
+        # (4b): CONVERSION (BIN, HEX, OCT)
+        #       - Use `raw_string` without radix point for calculation
+        #       - Check for a negative sign and remove it, use this information only
+        #         in the end
+        #       - Calculate decimal value of `raw_str` without '-' using
+        #        `int(raw_str, base)`
+        #       - divide by `base ** frc_places` for correct scaling
+        #       - calculate number of bits required for binary representation. If this
+        #         number exceeds word length, convert to binary string, strip
+        #         leading bits and convert back to float.
+        #       - transform numbers in negative 2's complement to negative floats.
+        #       - calculate the fixpoint representation using `fixp()` for correct
+        #            saturation / quantization
+        # TODO: Shouldn't `fixp()` be enough for handling number of bits etc?
+        # ======================================================================
+        elif frmt in {'hex', 'bin', 'oct'}:
             neg_sign = False
+            if fb.fil[0]['qfrmt'] == 'qint':
+                W = self.q_dict['WI'] + self.q_dict['WF'] + 1
+            else:
+                W = self.q_dict['WI'] + 1
             try:
                 if raw_str[0] == '-':
                     neg_sign = True
                     raw_str = raw_str.lstrip('-')
 
-                y_dec = abs(int(raw_str, self.base) / self.base**frc_places)
+                if frmt == 'hex':
+                    base = 16
+                elif frmt == 'oct':
+                    base = 8
+                else:  # 'bin'
+                    base = 2
+
+                y_dec = int(raw_str, base) / base ** frc_places
 
                 if y_dec == 0:  # avoid log2(0)
                     return 0
-
                 int_bits = max(int(np.floor(np.log2(y_dec))) + 1, 0)
+
                 # When number is outside fixpoint range, discard MSBs:
-                if int_bits > self.q_dict['WI'] + 1:
-                    if frmt == 'hex':
-                        raw_str = np.binary_repr(int(raw_str, 16))
+                if int_bits > W:
+                    # convert non-binary numbers to binary string for
+                    # discarding bits bit-wise
+                    if frmt != 'bin':
+                        raw_str = np.binary_repr(int(raw_str, base))
                     # discard the upper bits outside the valid range
-                    raw_str = raw_str[int_bits - self.q_dict['WI'] - 1:]
+                    raw_str = raw_str[int_bits - W:]
 
                     # recalculate y_dec for truncated string
-                    y_dec = int(raw_str, 2) / self.base**frc_places
+                    y_dec = int(raw_str, 2) / base ** frc_places
 
                     if y_dec == 0:  # avoid log2(0) error in code below
-                        return 0
-
+                        return 0.0
                     int_bits = max(int(np.floor(np.log2(y_dec))) + 1, 0)
+
                 # now, y_dec is in the correct range:
-                if int_bits <= self.q_dict['WI']:  # positive number
+                if int_bits <= W - 1:  # positive number
                     pass
-                elif int_bits == self.q_dict['WI'] + 1:
-                    # negative, calculate 2's complement
+                else: # int_bits == W -> negative, calculate 2's complement
+                    # int_bits > W has been treated above
                     y_dec = y_dec - (1 << int_bits)
                 # quantize / saturate / wrap & scale the integer value:
                 if neg_sign:
                     y_dec = -y_dec
-                y_float = self.fixp(y_dec, scaling='div')
+                y_float = self.fixp(y_dec, out_frmt='qfrac')
             except Exception as e:
                 logger.warning(e)
-                y_dec = y_float = None
+                return 0.0
 
-            # logger.debug(f"MSB={self.q_dict['MSB']} | LSB={self.q_dict['LSB']} | scale={self.q_dict['scale'])}")
-            # logger.debug(f"y_in={y} | y_dec={y_dec}")
-        # ----
+        # ======================================================================
+        # (4c): CONVERSION (CSD)
+        #       - use `raw_string` without radix point for calculation
+        #       - divide by 2 ** <number of fractional places> for correct scaling
+        #       - calculate the fixpoint representation using `fixp()` for correct
+        #            saturation / quantization
+        # ======================================================================
         elif frmt == 'csd':
-            # - Glue integer and fractional part to a string without radix point
-            # - Divide by 2 ** <number of fractional places> for correct scaling
-            # - Calculate fixpoint representation for saturation / overflow effects
-
             y_dec = csd2dec_vec(raw_str)  # csd -> integer
             if y_dec is not None:
-                y_float = self.fixp(y_dec / 2**frc_places, scaling='div')
+                y_float = self.fixp(y_dec / 2 ** frc_places, out_frmt='qfrac')
         # ----
         else:
             logger.error(f'Unknown output format "{frmt}"!')
-
-        # if frmt != "float":
-            # logger.debug("MSB={0:g} |  scale={1:g} | raw_str={2} | val_str={3}"\
-            #             .format(self.q_dict['MSB'], self.q_dict['scale']), raw_str, val_str))
-            # logger.debug("y={0} | y_dec = {1} | y_float={2}".format(y, y_dec, y_float))
+            return 0.0
 
         if y_float is not None:
             return y_float
         else:
             return 0.0
 
     # --------------------------------------------------------------------------
-    def float2frmt(self, y):
+    def float2frmt(self, y) -> str:
         """
+        Convert an array or single value of float / complex / string to a quantized
+        representation in one of the formats float / int / bin / hex / csd.
+
         Called a.o. by `itemDelegate.displayText()` for on-the-fly number
         conversion. Returns fixpoint representation for `y` (scalar or array-like)
-        with numeric format `self.frmt` and `self.q_dict['W']` bits. The result has the
-        same shape as `y`.
+        with numeric format `self.frmt` and a total wordlength of
+        `W = self.q_dict['WI'] + self.q_dict['WF'] + 1` bits.
+        The result has the same shape as `y`.
 
-        The float is multiplied by `self.q_dict['scale'])` and quantized / saturated
-        using `self.fixp()` for all formats before it is converted to different number
-        formats.
+        The float is always quantized / saturated using `self.fixp()` before it is
+        converted to different fixpoint number bases.
 
         Parameters
         ----------
         y: scalar or array-like
-            y has to be an integer or float decimal number either numeric or in
-            string format.
+            y has to be an integer, float or complex decimal number
 
         Returns
         -------
         A string, a float or an ndarray of float or string is returned in the
-        numeric format set in `self.q_dict['fx_base'])`. It has the same shape as `y`.
-         For all formats except `float` a fixpoint representation with
-         `self.q_dict['W']` binary digits is returned.
+        numeric format set in `fb.fil[0]['fx_base'])`. It has the same shape as `y`.
+        For all formats except `float` a fixpoint representation with
+        a total number of W = WI + WF + 1 binary digits is returned.
 
 
         Define vectorized functions using numpys automatic type casting:
         Vectorized functions for inserting binary point in string `bin_str`
         after position `pos`.
 
         Usage:  insert_binary_point(bin_str, pos)
 
         Parameters: bin_str : string
                     pos     : integer
         """
         insert_binary_point = np.vectorize(lambda bin_str, pos: (
                                     bin_str[:pos+1] + "." + bin_str[pos+1:]))
-
         binary_repr_vec = np.frompyfunc(np.binary_repr, 2, 1)
-        # ======================================================================
 
-        if self.q_dict['fx_base'] == 'float':  # return float input value unchanged (no string)
+        def binary_repr(y_int, W):
+            if type(y_int) in {np.ndarray, list, tuple}:
+                return binary_repr_vec(y_int, W).astype('U')
+            elif isinstance(y_int, (int, np.integer)):
+                return np.binary_repr(y_int, W)
+            else:
+                logger.error(f"Unsupported data type '{type(y_int)}'!")
+                return "0"
+
+        # ======================================================================
+        # logger.warning(f"float2frmt: y = {y}")
+        if not is_numeric(y):
+            logger.error(f"float2frmt() received a non-numeric argument '{y}'!")
+            return 0.0
+        if not fb.fil[0]['fx_sim']:  # return float input value unchanged (no string)
             return y
-        elif self.q_dict['fx_base'] == 'float32':
-            return np.float32(y)
-        elif self.q_dict['fx_base'] == 'float16':
-            return np.float16(y)
-
-        elif self.q_dict['fx_base'] in {'hex', 'bin', 'dec', 'csd'}:
-            # return a quantized & saturated / wrapped fixpoint (type float) for y
-            y_fix = self.fixp(y, scaling='mult')
-
-            if self.q_dict['fx_base'] == 'dec':
-                if self.q_dict['WF'] == 0:
-                    y_str = np.int64(y_fix)  # get rid of trailing zero
-                    # y_str = np.char.mod('%d', y_fix)
-                    # elementwise conversion from integer (%d) to string
-                    # see https://docs.scipy.org/doc/numpy/reference/routines.char.html
-                else:
-                    # y_str = np.char.mod('%f',y_fix)
-                    y_str = y_fix
-            elif self.q_dict['fx_base'] == 'csd':
-                y_str = dec2csd_vec(y_fix, self.q_dict['WF'])  # convert with WF fractional bits
-
-            else:  # bin or hex
-                # represent fixpoint number as integer in the range -2**(W-1) ... 2**(W-1)
-                y_fix_int = np.int64(np.round(y_fix / self.q_dict['LSB']))
-                # convert to (array of) string with 2's complement binary
-                y_bin_str = binary_repr_vec(y_fix_int, self.q_dict['W'])
-
-                if self.q_dict['fx_base'] == 'hex':
-                    y_str = bin2hex_vec(y_bin_str, self.q_dict['WI'])
-
-                else:  # self.q_dict['fx_base']t == 'bin':
-                    # insert radix point if required
-                    if self.q_dict['WF'] > 0:
-                        y_str = insert_binary_point(y_bin_str, self.q_dict['WI'])
-                    else:
-                        y_str = y_bin_str
 
-            if isinstance(y_str, np.ndarray) and np.ndim(y_str) < 1:
-                y_str = y_str.item()  # convert singleton array to scalar
+        if np.iscomplexobj(y):  # convert complex arguments recursively
+            y_re = self.float2frmt(y.real)
+            y_im = self.float2frmt(y.imag)
+            if fb.fil[0]['fx_base'] == 'csd':
+                logger.error(
+                    "Complex CSD coefficients are not supported yet, casting  to real. "
+                    "\n\tPlease create an issue if you need this feature.")
+                # CSD coefficients differ in length and require an array with dtype 'object'
+                # which does not support arithmetic or string operations.
+                return y_re
+            elif is_numeric(y_re) and is_numeric(y_im):  # return in numeric format
+                return y_re + y_im * 1j
+            elif not (is_numeric(y_re) or is_numeric(y_im)):  # return string (array)
+                # logger.error(
+                #     f"real part:\n{y_re}\n{type(y_re)} ({y_re.dtype})\n"
+                #     f"imag. part\n{y_im}\n{type(y_im)} ({y_im.dtype}).")
+                y_str = np.char.add(np.char.add(y_re, '+'), np.char.add(y_im,'j'))
+                # logger.warning(f"ystr={y_str}")
+                return y_str
+            else:
+                logger.error(f"Cannot combine real part ({y_re.dtype}) and imag. part ({y_im.dtype}).")
+                return "0"
+
+        # return a quantized & saturated / wrapped fixpoint (type float) for y (int or frac format)
+        y_fix = self.fixp(y, out_frmt=fb.fil[0]['qfrmt'])
+
+        if fb.fil[0]['fx_base'] == 'dec':
+            if self.q_dict['WF'] == 0 or fb.fil[0]['qfrmt'] == 'qint':
+                # TODO: need to convert to str?
+                y_str = np.int64(y_fix)  # get rid of trailing zero
+                # y_str = np.char.mod('%d', y_fix)
+                # elementwise conversion from integer (%d) to string
+                # see https://docs.scipy.org/doc/numpy/reference/routines.char.html
+            else:
+                # y_str = np.char.mod('%f',y_fix)
+                y_str = y_fix
+        elif fb.fil[0]['fx_base'] == 'csd':
+            if fb.fil[0]['qfrmt'] == 'qint':
+                # integer case, convert with 0 fractional bits
+                y_str = dec2csd_vec(y_fix, 0)
+            else:
+                # fractional case, convert with WF fractional bits
+                y_str = dec2csd_vec(y_fix, self.q_dict['WF'])
 
-            return y_str
+        elif fb.fil[0]['fx_base'] in {'bin', 'oct', 'hex'}:
+            # represent fixpoint number as integer in the range -2**(W-1) ... 2**(W-1)
+            y_fix_int = np.int64(np.round(y_fix / self.LSB))
+            W = self.q_dict['WI'] + self.q_dict['WF'] + 1
+            # convert to (array of) string with 2's complement binary
+            y_bin_str = binary_repr(y_fix_int, W)
+
+            if fb.fil[0]['qfrmt'] == 'qint':
+                WI = self.q_dict['WI'] + self.q_dict['WF'] + 1
+                # TODO: Is the "+ 1" correct?
+            else:
+                WI = self.q_dict['WI']
+            if fb.fil[0]['fx_base'] == 'hex':
+                y_str = bin2hex_vec(y_bin_str, WI)
+            elif fb.fil[0]['fx_base'] == 'oct':
+                y_str = bin2oct_vec(y_bin_str, WI)
+            else:  # 'bin'
+                # insert radix point if required
+                if fb.fil[0]['qfrmt'] == 'qint':
+                    y_str = y_bin_str
+                else:
+                    y_str = insert_binary_point(y_bin_str, WI)
         else:
-            raise Exception(f"""Unknown number format "{self.q_dict['fx_base']}"!""")
+            raise Exception(f"""Unknown number format "{fb.fil[0]['fx_base']}"!""")
+
+        if isinstance(y_str, np.ndarray) and np.ndim(y_str) < 1:
+            y_str = y_str.item()  # convert singleton array to scalar
+
+        # logger.warning(f"float2frmt: y_str = {y_str}")
+        return y_str
 
 ########################################
 
 # --------------------------------------------------------------------------
-def quant_coeffs(coeffs: iterable, QObj, recursive: bool = False) -> list:
+def quant_coeffs(coeffs: iterable, Q, recursive: bool = False) -> np.ndarray:
     """
     Quantize the coefficients, scale and convert them to a list of integers,
-    using the quantization settings of `Fixed()` instance QObj.
+    using the quantization settings of `Fixed()` instance `Q` and global setting
+    `fb.fil[0]['qfrmt']` (`'qfrac'` or `'qint'`) and `fb.fil[0]['fx_sim']` (`True`
+    or `False`)
 
     Parameters
     ----------
     coeffs: iterable
         a list or ndarray of coefficients to be quantized
 
-    QObj: dict
+    Q: dict
         instance of Fixed object containing quantization dict `q_dict`
 
     recursive: bool
         When `False` (default), process all coefficients. When `True`,
         The first coefficient is ignored (must be 1)
 
     Returns
     -------
-    A list of integer coeffcients, quantized and scaled with the settings
-    of the quantization object dict
+    A numpy array of integer coeffcients, quantized and scaled with the
+    settings of the quantization object dict.
 
     """
-    logger.debug("quant_coeffs")
+    disp_frmt_tmp = fb.fil[0]['fx_base']  # temporarily store fx display format and
     # always use decimal display format for coefficient quantization
-    disp_frmt_tmp = QObj.q_dict['fx_base']
-    QObj.q_dict['fx_base'] = 'dec'
-    QObj.resetN()  # reset all overflow counters
+    fb.fil[0]['fx_base'] = 'dec'
+    out_frmt=fb.fil[0]['qfrmt']
+    Q.resetN()  # reset all overflow counters
 
     if coeffs is None:
         logger.error("Coeffs empty!")
+        return None
+
     # quantize floating point coefficients with the selected scale (WI.WF),
-    # next convert array float  -> array of fixp
-    #                           -> list of int (scaled by 2^WF) when `to_int == True`
-    if QObj.q_dict['qfrmt'] == 'int':
-        QObj.q_dict['scale'] = 1 << QObj.q_dict['WF']
+    # next, convert array float  -> array of fixp
+    #                            -> list of int (scaled by 2^WF) when `'qfrmt':'qint'`
     if recursive:
-        # quantize coefficients except for first
-        coeff_q = [1] + list(QObj.fixp(coeffs[1:]))
+        # recursive coefficients: quantize coefficients except for first (= 1)
+        coeff_q = np.concatenate(([1], Q.fixp(coeffs[1:], out_frmt=out_frmt)))
     else:
         # quantize all coefficients
-        coeff_q = list(QObj.fixp(coeffs))
+        coeff_q = Q.fixp(coeffs, out_frmt=out_frmt)
 
-    # self.update_disp()  # update display of overflow counter and MSB / LSB
+    # self.update_ovfl_cnt()  # update display of overflow counter and MSB / LSB
 
-    QObj.q_dict['fx_base'] = disp_frmt_tmp  # restore previous display setting
+    fb.fil[0]['fx_base'] = disp_frmt_tmp  # restore previous display setting
     return coeff_q
 
 
 ########################################
 if __name__ == '__main__':
     """
     Run a simple test with python -m pyfda.libs.pyfda_fix_lib
     or a more elaborate one with
     python -m pyfda.tests.test_pyfda_fix_lib
     """
     import pprint
 
-    q_dict = {'WI': 0, 'WF': 3, 'ovfl': 'sat', 'quant': 'round', 'fx_base': 'dec', 'scale': 1}
+    q_dict = {'WI': 0, 'WF': 3, 'ovfl': 'sat', 'quant': 'round'}
     myQ = Fixed(q_dict)  # instantiate fixpoint object with settings above
     y_list = [-1.1, -1.0, -0.5, 0, 0.5, 0.99, 1.0]
 
     myQ.set_qdict(q_dict)
 
     print("\nTesting float2frmt()\n====================")
     pprint.pprint(q_dict)
     for y in y_list:
         print("y = {0}\t->\ty_fix = {1}".format(y, myQ.float2frmt(y)))
 
     print("\nTesting frmt2float()\n====================")
-    q_dict = {'WI': 3, 'WF': 3, 'ovfl': 'sat', 'quant': 'round', 'fx_base': 'dec', 'scale': 2}
+    q_dict = {'WI': 3, 'WF': 3, 'ovfl': 'sat', 'quant': 'round'}
     pprint.pprint(q_dict)
     myQ.set_qdict(q_dict)
     dec_list = [-9, -8, -7, -4.0, -3.578, 0, 0.5, 4, 7, 8]
     for dec in dec_list:
         print("y={0}\t->\ty_fix={1} ({2})".format(dec, myQ.frmt2float(dec), myQ.frmt))
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_io_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_io_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,55 +6,63 @@
 # Licensed under the terms of the MIT License
 # (see file LICENSE in root directory for details)
 
 """
 Library with classes and functions for file and text IO
 """
 import os, re, io
+import copy
 import csv
 import wave
 import datetime
 import warnings
 from typing import TextIO, Tuple  # replace by built-in tuple from Py 3.9
 
 import pickle
+import json
 
 import numpy as np
 from scipy.io import loadmat, savemat, wavfile
 
 try:
     import xlwt
 except ImportError:
     xlwt = None
 try:
     import xlsx
 except ImportError:
     xlsx = None
 
-from pyfda.libs.pyfda_lib import safe_eval, lin2unit, pprint_log, iter2ndarray
-from pyfda.libs.pyfda_qt_lib import qget_selected
+from pyfda.libs.pyfda_lib import (
+    safe_eval, lin2unit, pprint_log, iter2ndarray, sanitize_imported_dict)
+from pyfda.libs.pyfda_qt_lib import qget_selected, popup_warning
 
 import pyfda.libs.pyfda_fix_lib as fx
 from pyfda.pyfda_rc import params
 import pyfda.libs.pyfda_dirs as dirs
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
+from pyfda.version import __version__
 
 from .compat import QFileDialog
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 # ##############################################################################
+# Include this version number as `'_id': ('pyfda', FILTER_FILE_VERSION)` when saving
+# filter files and test for the version when loading filter files.
+FILTER_FILE_VERSION = 1
 
 # file filters for the QFileDialog object are constructed from this dict
 file_filters_dict = {
     'cmsis': 'CMSIS DSP FIR or IIR SOS coefficients',
     'coe': 'Xilinx FIR coefficients format',
     'csv': 'Comma / Tab Separated Values',
+    'json': 'Javascript Object Notation',
     'mat': 'Matlab-Workspace',
     'npy': 'Binary Numpy Array',
     'npz': 'Zipped Binary Numpy Array',
     'pkl': 'Pickled data',
     'txt': 'Microsemi FIR coefficient format',
     'vhd': 'VHDL package or architecture',
     'wav': 'WAV audio format',
@@ -103,38 +111,46 @@
     - '(' must be escaped as '\\\('
     """
 
     return re.sub('\([^\)]+\)', '', file_type)
 
 
 # ------------------------------------------------------------------------------
-def extract_file_ext(file_type: str) -> str:
+def extract_file_ext(file_type: str, return_list=False) -> str:
     """
     Extract list with file extension(s), e.g. '.vhd' from type description
     'VHDL (\*.vhd)' returned by QFileDialog. Depending on the OS, this may be the
     full file type description or just the extension like '(\*.vhd)'.
 
     When `file_type` contains no '(', the passed string is returned unchanged.
 
     For an explanation of the RegEx, see the docstring for `prune_file_ext`.
 
     Parameters
     ----------
     file_type : str
 
+    return_list: bool (default = False)
+       When True, return a list with file extensions (possibly empty or with only one
+       element), when False (default) only return the first element (a string)
+
     Returns
     -------
-    str
-        The file extension between ( ... ) or the unchanged input argument
-        `file_type` when no '('  was contained.
+    str or list of str
+        The file extension between ( ... ), e.g. 'csv' or the list of file extension
+        or the unchanged input argument `file_type` when no '('  was contained.
 
     """
     if "(" in file_type:
         ext_list = re.findall('\([^\)]+\)', file_type)  # extract '(*.txt)'
-        return [t.strip('(*)') for t in ext_list]  # remove '(*)'
+        file_type_list = [t.strip('(*.)') for t in ext_list]  # remove '(*.)'
+        if return_list:
+            return file_type_list
+        else:
+            return str(file_type_list[0])
     else:
         return file_type
 
 
 # ------------------------------------------------------------------------------
 def create_file_filters(file_types: tuple, file_filters: str = ""):
     """
@@ -209,14 +225,19 @@
 
     file_type: str
         File type, e.g. 'wav'. `None` when operation has been cancelled.
     """
 
     file_filters, last_file_filter = create_file_filters(file_types=file_types)
 
+    # check whether last file type is in the list of file types for the current
+    # operation, otherwise delete last_file_filter
+    if extract_file_ext(last_file_filter) not in file_types:
+        last_file_filter = ""
+
     dlg = QFileDialog(parent)  # create instance for QFileDialog
     dlg.setDirectory(dirs.last_file_dir)
     if mode in {"r", "rb"}:
         if title == "":
             title = "Import"
         dlg.setWindowTitle(title)
         dlg.setAcceptMode(QFileDialog.AcceptOpen)  # set dialog to "file open" mode
@@ -239,15 +260,15 @@
     if dlg.exec_() == QFileDialog.Accepted:
         file_name = dlg.selectedFiles()[0]  # pick only first selected file
         file_type = os.path.splitext(file_name)[-1].strip('.')
         sel_filt = dlg.selectedNameFilter()  # selected file filter
 
         if file_type == "":
             # No file type specified, add the type from the file filter
-            file_type = extract_file_ext(sel_filt)[0].strip('.')
+            file_type = extract_file_ext(sel_filt)
             file_name = file_name + '.' + file_type
 
         dirs.last_file_name = file_name
         dirs.last_file_dir = os.path.dirname(file_name)
         dirs.last_file_type = file_type
     else:  # operation cancelled
         file_name = None
@@ -299,21 +320,21 @@
             each entry or pair of entries which usually is not what you want.
             'auto' doesn't make much sense when writing, 'horiz' is used in this case.
 
     :'header': str (default: 'auto').
             When ``header='on'``, write the first row with 'b, a'.
 
     :'clipboard': bool (default: True),
-            when ``clipboard = True``, copy data to clipboard, else use a file.
+            when ``clipboard == True``, copy data to clipboard, else use a file.
 
     Returns
     -------
 
     None
-        Nothing, text is exported to clipboard or to file via ``save_data_csv``
+        Nothing, text is exported to clipboard or to file via ``export_fil_data``
     """
 
     text = ""
     if params['CSV']['header'] == 'on':
         use_header = True
     elif params['CSV']['header'] in {'off', 'auto'}:
         use_header = False
@@ -484,15 +505,15 @@
 
     :'clipboard': bool (default: True).
             When ``clipboard == True``, copy data from clipboard, else use a file
 
     Parameters that are 'auto', will be guessed by ``csv.Sniffer()``.
 
     """
-    if params['CSV']['clipboard']:  # data from clipboard
+    if params['CSV']['destination'] == 'clipboard':  # data from clipboard
         text = fb.clipboard.text()
         logger.debug(
             f"Importing data from clipboard:\n{np.shape(text)}\n{text}")
         # pass handle to text and convert to numpy array:
         data_arr = csv2array(io.StringIO(text))
 
     else:  # data from file
@@ -1140,49 +1161,57 @@
             f.writeframes(audio.tobytes())
         with open(file_name, 'w', encoding="utf8", newline='') as f:
                         f.write(data)
 
         logger.info(f'Filter saved as\n\t"{file_name}"')
 
     except IOError as e:
-        logger.error('Failed saving "{0}"!\n{1}\n'.format(file_name, e))
+        logger.error(f'Failed saving "{file_name}"!\n{e}\n')
 
 
 # ------------------------------------------------------------------------------
-def save_data_csv(parent: object, data: str, fkey: str = "", title: str = "Export",
+def export_fil_data(parent: object, data: str, fkey: str = "", title: str = "Export",
                 file_types: Tuple[str, ...] = ('csv', 'mat', 'npy', 'npz')):
     """
-    Export coefficients or pole/zero data in various formats
+    Export filter coefficients or pole/zero data in various formats, file name and type
+    are selected via the ui.
 
     Parameters
     ----------
     parent: handle to calling instance for creating file dialog instance
 
     data: str
         formatted as CSV data, i.e. rows of elements separated by 'delimiter',
-        terminated by 'lineterminator'
+        terminated by 'lineterminator'. Some data formats
 
     fkey: str
         Key for accessing data in ``*.npz`` or Matlab workspace (``*.mat``) file.
         When fkey == 'ba', exporting to FPGA coefficients format is enabled.
 
     title: str
         title string for the file dialog box (e.g. "filter coefficients ")
 
     file_types: tuple of strings
         file extension (e.g. `(csv)` or list of file extensions (e.g. `(csv, txt)`
         which are used to create a file filter.
     """
-    logger.debug(
-        f"export data: type{type(data)}|dim{np.ndim(data)}|"
-        f"shape{np.shape(data)}\n{data}")
-
-    # add file types for FIR filter coefficients
-    if fb.fil[0]['ft'] == 'FIR':
-        file_types += ('coe', 'vhd', 'txt')
+    # logger.debug(
+    #     f"export data: type{type(data)}|dim{np.ndim(data)}|"
+    #     f"shape{np.shape(data)}\n{data}")
+
+    # add file types for coefficients and a description text for messages.
+    if fkey == 'ba':
+        if fb.fil[0]['ft'] == 'FIR':
+            file_types += ('coe', 'vhd', 'txt')
+        else:
+            file_types += ('cmsis',)
+        description = "Coefficient"
+    else:
+        description = "Pole / zero"
+
     # Add file types when Excel modules are available:
     if xlwt is not None:
         file_types += ('xls',)
     if xlsx is not None:
         file_types += ('xlsx',)
 
     file_name, file_type = select_file(parent,title=title, mode='wb',
@@ -1192,31 +1221,33 @@
 
     err = False
 
     try:
         if file_type == 'csv':
             with open(file_name, 'w', encoding="utf8", newline='') as f:
                 f.write(data)
-        elif file_type in {'coe', 'txt', 'vhd'}:  # text / string format
+        elif file_type in {'coe', 'txt', 'vhd', 'cmsis'}:  # text / string formats
             with open(file_name, 'w', encoding="utf8") as f:
                 if file_type == 'coe':
                     err = export_coe_xilinx(f)
                 elif file_type == 'txt':
                     err = export_coe_microsemi(f)
-                elif file_type == '.vhd':
+                elif file_type == 'vhd':
                     err = export_coe_vhdl_package(f)
+                elif file_type == 'cmsis':
+                    err = export_coe_cmsis(f)
                 else:
                     logger.error(f'Unknown file extension "{file_type}')
                     return None
 
         else:  # binary formats, storing numpy arrays
             np_data = csv2array(io.StringIO(data))  # convert csv data to numpy array
             if isinstance(np_data, str):
                 # returned an error message instead of numpy data:
-                logger.error("Error converting coefficient data:\n{0}".format(np_data))
+                logger.error(f"Error converting {description.lower()} data:\n{np_data}")
                 return None
 
             with open(file_name, 'wb') as f:
                 if file_type == 'mat':
                     savemat(f, mdict={fkey: np_data})
                     # newline='\n', header='', footer='', comments='# ', fmt='%.18e'
                 elif file_type == 'npy':
@@ -1261,19 +1292,19 @@
 
                     # Insert an image - useful for documentation export ?!.
         #            worksheet.insert_image('B5', 'logo.png')
 
                     workbook.close()
 
                 else:
-                    logger.error('Unknown file type "{0}"'.format(file_type))
+                    logger.error(f'Unknown file type "{file_type}"')
                     err = True
 
         if not err:
-            logger.info(f'Filter saved as\n\t"{file_name}"')
+            logger.info(f'{description} data saved as\n\t"{file_name}"')
 
     except IOError as e:
         logger.error('Failed saving "{0}"!\n{1}\n'.format(file_name, e))
 
         # Download the Simple ods py module:
         # http://simple-odspy.sourceforge.net/
         # http://codextechnicanum.blogspot.de/2014/02/write-ods-for-libreoffice-calc-from_1.html
@@ -1361,16 +1392,16 @@
     unit = fb.fil[0]['plt_fUnit']
     if unit in {'f_S', 'f_Ny'}:
         f_S = ""
     else:
         f_S = fb.fil[0]["f_S"]
     header = (
         "-" * 85 + "\n\n"
-        "{0}".format(title) + "\n"
-        "Generated by pyFDA 0.6 (https://github.com/chipmuenk/pyfda)\n\n")
+        f"{title}\n"
+        f"Generated by pyfda {__version__} (https://github.com/chipmuenk/pyfda)\n\n")
     header += "Designed:\t{0}\n".format(
         datetime.datetime.fromtimestamp(
             int(fb.fil[0]['timestamp'])).strftime(date_frmt))
     header += "Saved:\t{0}\n\n".format(datetime.datetime.now().strftime(date_frmt))
     header += f"Filter type:\t{fb.fil[0]['rt']}, {fb.fil[0]['fc']} "
     header += f"(Order = {fb.fil[0]['N']})\n"
     header += f"Sample Frequency \tf_S = {f_S} {unit}\n\n"
@@ -1379,73 +1410,73 @@
         header += "\t" + lf + " = " + str(f) + " " + unit + " : " + la + " = "
         header += str(a) + " dB\n"
     header += "-" * 85 + "\n"
     return header
 
 
 # ------------------------------------------------------------------------------
-def export_coe_xilinx(f: TextIO) -> None:
+def export_coe_xilinx(f: TextIO) -> bool:
     """
     Save FIR filter coefficients in Xilinx coefficient format as file '\*.coe', specifying
     the number base and the quantized coefficients (decimal or hex integer).
+
+    Returns error status (False if the file was saved successfully)
     """
-    qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
-    logger.debug("scale = {0}, WF = {1}".format(qc.q_dict['scale'], qc.q_dict['WF']))
+    qc = fx.Fixed(fb.fil[0]['fxq']['QCB'])  # instantiate fixpoint object
 
-    if qc.q_dict['WF'] != 0:
-        # Set the fixpoint format to integer (WF=0) with the original wordlength
-        qc.set_qdict({'W': qc.q_dict['W'], 'scale': 1 << qc.q_dict['W']-1})
-        logger.warning("Fractional formats are not supported, using integer format.")
+    if qc.q_dict['WF'] != 0  and fb.fil[0]['qfrmt'] != 'qint':
+        logger.error("Fractional formats are not supported!")
+        return True
 
-    if qc.q_dict['fx_base'] == 'hex':  # select hex format
+    if fb.fil[0]['fx_base'] == 'hex':  # select hex format
         coe_radix = 16
-    if qc.q_dict['fx_base'] == 'bin':  # select binary format
+    if fb.fil[0]['fx_base'] == 'bin':  # select binary format
         coe_radix = 2
     else:
-        logger.warning('Coefficients in "{0}" format are not supported in COE files, '
-                       'using decimal format.')
-        qc.set_qdict({'fx_base': 'dec'})  # select decimal format in all other cases
+        logger.warning(f"Coefficients in {fb.fil[0]['fx_base']} format are "
+                       f'not supported in COE files, converting to decimal format.')
+        fb.fil[0]['fx_base'] =  'dec'  # select decimal format in all other cases
         coe_radix = 10
 
-    # Quantize coefficients to decimal / hex integer format, returning an array of strings
+    # Quantize coefficients to decimal / hex integer format, return an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
     exp_str = "; " + coe_header(
         "XILINX CORE Generator(tm) Distributed Arithmetic FIR filter coefficient (.COE) file").replace("\n", "\n; ")
 
     exp_str += "\nRadix = {0};\n".format(coe_radix)
-    exp_str += f"Coefficient_width = {qc.q_dict['W']};\n"  # quantized wordlength
+      # quantized wordlength
+    exp_str += f"Coefficient_width = {qc.q_dict['WI'] + qc.q_dict['WF'] + 1};\n"
     coeff_str = "CoefData = "
     for b in bq:
         coeff_str += str(b) + ",\n"
     exp_str += coeff_str[:-2] + ";"  # replace last "," by ";"
 
     f.write(exp_str)
 
     return False
 
 
 # ------------------------------------------------------------------------------
-def export_coe_microsemi(f: TextIO) -> None:
+def export_coe_microsemi(f: TextIO) -> bool:
     """
     Save FIR filter coefficients in Microsemi coefficient format as file '\*.txt'.
     Coefficients have to be in integer format, the last line has to be empty.
     For (anti)symmetric filter only one half of the coefficients must be
     specified?
     """
-    qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
+    qc = fx.Fixed(fb.fil[0]['fxq']['QCB'])  # instantiate fixpoint object
 
-    if qc.q_dict['WF'] != 0:
-        # Set the fixpoint format to integer (WF=0) with the original wordlength:
-        qc.set_qdict({'W': qc.q_dict['W'], 'scale': 1 << qc.q_dict['W']-1})
-        logger.warning("Fractional formats are not supported, using integer format.")
-
-    if qc.q_dict['fx_base'] != 'dec':
-        qc.set_qdict({'fx_base': 'dec'})  # select decimal format in all other cases
-        logger.warning('Switching to decimal coefficient format, other numeric formats '
+    if qc.q_dict['WF'] != 0  and fb.fil[0]['qfrmt'] != 'qint':
+        logger.error("Fractional formats are not supported!")
+        return True
+
+    if fb.fil[0]['fx_base'] != 'dec':
+        fb.fil[0]['fx_base'] = 'dec'  # select decimal format in all other cases
+        logger.warning('Converting to decimal coefficient format, other numeric formats '
                        'are not supported by Microsemi tools.')
 
     # Quantize coefficients to decimal integer format, returning an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
     coeff_str = "coefficient_set_1\n"
     for b in bq:
@@ -1453,60 +1484,62 @@
 
     f.write(coeff_str)
 
     return False
 
 
 # ------------------------------------------------------------------------------
-def export_coe_vhdl_package(f: TextIO) -> None:
+def export_coe_vhdl_package(f: TextIO) -> bool:
     """
     Save FIR filter coefficients as a VHDL package '\*.vhd', specifying
     the number base and the quantized coefficients (decimal or hex integer).
     """
-    qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
-    if not qc.q_dict['fx_base'] == 'float' and qc.q_dict['WF'] != 0:
-        # Set the fixpoint format to integer (WF=0) with the original wordlength
-        qc.set_qdict({'W': qc.q_dict['W'], 'scale': 1 << qc.q_dict['W']-1})
-        logger.warning("Fractional formats are not supported, using integer format.")
+    qc = fx.Fixed(fb.fil[0]['fxq']['QCB'])  # instantiate fixpoint object
+    if not fb.fil[0]['fx_sim'] or fb.fil[0]['qfrmt'] == 'qint'\
+        or fb.fil[0]['qfrmt'] == 'qfrac' and qc.q_dict['WF'] == 0:
+            pass
+    else:
+        logger.error("Fractional numbers are only supported for floats!")
+        return True
 
-    WO = fb.fil[0]['fxqc']['QO']['W']
+    WO = fb.fil[0]['fxq']['QO']['WI'] + fb.fil[0]['fxq']['QO']['WF'] + 1
 
-    if qc.q_dict['fx_base'] == 'hex':
+    if fb.fil[0]['fx_base'] == 'dec' or not fb.fil[0]['fx_sim']:
+        pre = ""
+        post = ""
+    elif fb.fil[0]['fx_base'] == 'hex':
         pre = "#16#"
         post = "#"
-    elif qc.q_dict['fx_base'] == 'bin':
+    elif fb.fil[0]['fx_base'] == 'bin':
         pre = "#2#"
         post = "#"
-    elif qc.q_dict['fx_base'] in {'dec', 'float'}:
-        pre = ""
-        post = ""
     else:
-        qc.set_qdict({'fx_base': 'dec'})  # select decimal format in all other cases
+        fb.fil[0]['fx_base'] = 'dec'  # select decimal format in all other cases
         pre = ""
         post = ""
-        logger.warning('Coefficients in "{0}" format are currently not supported, '
-                       'using decimal format.'.format(qc.q_dict['fx_base']))
+        logger.warning(f"Coefficients in {fb.fil[0]['fx_base']} format are "
+                       'not supported, converting to decimal format.')
 
     # Quantize coefficients to selected fixpoint format, returning an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
     exp_str = "-- " + coe_header(
         "VHDL FIR filter coefficient package file").replace("\n", "\n-- ")
 
     exp_str += "\nlibrary IEEE;\n"
-    if qc.q_dict['fx_base'] == 'float':
+    if not fb.fil[0]['fx_sim']:
         exp_str += "use IEEE.math_real.all;\n"
     exp_str += "USE IEEE.std_logic_1164.all;\n\n"
     exp_str += "package coeff_package is\n"
     exp_str += "constant n_taps: integer := {0:d};\n".format(len(bq)-1)
-    if qc.q_dict['fx_base'] == 'float':
+    if not fb.fil[0]['fx_sim']:
         exp_str += "type coeff_type is array(0 to n_taps) of real;\n"
     else:
         exp_str += "type coeff_type is array(0 to n_taps) of integer "
-        exp_str += "range {0} to {1};\n\n".format(-1 << WO-1, (1 << WO-1) - 1)
+        exp_str += f"range {-1 << WO-1} to {(1 << WO-1) - 1};\n\n"
     exp_str += "constant coeff : coeff_type := "
 
     coeff_str = "(\n"
     for b in bq:
         coeff_str += "\t" + pre + str(b) + post + ",\n"
     exp_str += coeff_str[:-2] + ");\n\n"  # replace last "," by ");"
 
@@ -1530,126 +1563,263 @@
     ...
 
     ** not implemented yet **
     """
     pass
 
 
+# ------------------------------------------------------------------------------
+def export_coe_cmsis(f: TextIO) -> None:
+    """
+    Get coefficients in SOS format and delete 4th column containing the
+    '1.0' of the recursive parts.
+
+    See https://www.keil.com/pack/doc/CMSIS/DSP/html/group__BiquadCascadeDF1.html
+    https://dsp.stackexchange.com/questions/79021/iir-design-scipy-cmsis-dsp-coefficient-format
+    https://github.com/docPhil99/DSP/blob/master/MatlabSOS2CMSIS.m
+
+    # TODO: check `scipy.signal.zpk2sos` for details concerning sos paring
+    """
+    sos_coeffs = np.delete(fb.fil[0]['sos'], 3, 1)
+
+    delim = params['CSV']['delimiter'].lower()
+    if delim == 'auto':  # 'auto' doesn't make sense when exporting
+        delim = ","
+    cr = params['CSV']['lineterminator']
+
+    text = ""
+    for r in range(np.shape(sos_coeffs)[0]):  # number of rows
+        for c in range(5):  # always has 5 columns
+            text += str(safe_eval(sos_coeffs[r][c], return_type='auto')) + delim
+        text = text.rstrip(delim) + cr
+    text = text.rstrip(cr)  # delete last CR
+
+    f.write(text)
+
+    return False
+
+
 # ==============================================================================
 def load_filter(self) -> int:
     """
     Load filter from zipped binary numpy array or (c)pickled object to
     filter dictionary
     """
     file_name, file_type = select_file(
-        self, title="Load Filter", mode="rb", file_types = ("npz", "pkl"))
+        self, title="Load Filter", mode="rb", file_types = ("json", "npz", "pkl"))
 
     if file_name is None:
         return -1  # operation cancelled or some other error
 
     err = False
-    fb.fil[1] = fb.fil[0].copy()  # backup filter dict
-    try:
-        with io.open(file_name, 'rb') as f:
-            if file_type == 'npz':
-                # array containing dict, dtype 'object':
-                a = np.load(f, allow_pickle=True)
-
-                logger.debug(f"Entries in {file_name}:\n{a.files}")
-                for key in sorted(a):
-                    logger.debug(
-                        f"key: {key}|{type(key).__name__}|"
-                        f"{type(a[key]).__name__}|{a[key]}")
-
-                    if np.ndim(a[key]) == 0:
-                        # scalar objects may be extracted with the item() method
-                        fb.fil[0][key] = a[key].item()
-                    else:
-                        # array objects are converted to list first
-                        fb.fil[0][key] = a[key].tolist()
-            elif file_type == 'pkl':
-                fb.fil[0] = pickle.load(f)
-            else:
-                logger.error('Unknown file type "{0}"'.format(file_type))
-                err = True
-            if not err:
-                # sanitize values in filter dictionary, keys are ok by now
-                for k in fb.fil[0]:
-                    # Bytes need to be decoded for py3 to be used as keys later on
-                    if type(fb.fil[0][k]) == bytes:
-                        fb.fil[0][k] = fb.fil[0][k].decode('utf-8')
-                    if fb.fil[0][k] is None:
-                        logger.warning("Entry fb.fil[0][{0}] is empty!".format(k))
-                if 'ba' not in fb.fil[0]\
-                    or type(fb.fil[0]['ba']) not in {list, np.ndarray}\
-                        or np.ndim(fb.fil[0]['ba']) != 2\
-                        or (np.shape(fb.fil[0]['ba'][0]) != 2
-                            and np.shape(fb.fil[0]['ba'])[1] < 3):
-                    logger.error("Missing key 'ba' or wrong data type!")
-                    return -1
-                elif 'zpk' not in fb.fil[0]:
-                    logger.error("Missing key 'zpk'!")
-                    return -1
-                elif 'sos' not in fb.fil[0]\
-                        or type(fb.fil[0]['sos']) not in {list, np.ndarray}:
-                    logger.error("Missing key 'sos' or wrong data type!")
-                    return -1
-                if type(fb.fil[0]['zpk']) == np.ndarray:
-                    if np.ndim(fb.fil[0]['zpk']) != 2:
-                        logger.error(
-                            f"Unsuitable dimension of 'zpk' data, ndim = {np.ndim(fb.fil[0]['zpk'])}")
-                    elif np.shape(fb.fil[0]['zpk'])[0] != 3:
-                        logger.error(
-                            f"Unsuitable shape {np.shape(fb.fil[0]['zpk'])} of 'zpk' data ")
-                elif type(fb.fil[0]['zpk']) == list:
-                    fb.fil[0]['zpk'] = iter2ndarray(fb.fil[0]['zpk'])
-
-                logger.info('Successfully loaded filter\n\t"{0}"'.format(file_name))
-                dirs.last_file_name = file_name
-                dirs.last_file_dir = os.path.dirname(file_name)  # update working dir
-                dirs.last_file_type = file_type  # save file type
-                return 0
+    fb.redo() # backup filter dict
 
-    except IOError as e:
-        logger.error("Failed loading {0}!\n{1}".format(file_name, e))
+    if file_type in {"npz", "pkl"}:
+        try:
+            with io.open(file_name, 'rb') as f:  # open in binary mode for npy and pkl
+                if file_type == 'npz':
+                    # array containing dict, dtype 'object':
+                    arr = np.load(f, allow_pickle=True)
+
+                    # convert arrays to lists and extract scalar objects
+                    for key in sorted(arr):
+                        if np.ndim(arr[key]) == 0:
+                            # scalar objects may be extracted with the item() method
+                            fb.fil[0][key] = arr[key].item()
+                        else:
+                            # array objects are converted to list first
+                            fb.fil[0][key] = arr[key].tolist()
+                else:  # file_type == 'pkl':
+                    fb.fil[0] = pickle.load(f)
+
+        except IOError as e:
+            logger.error(f"Failed loading {file_name}!\n{e}")
+            return -1
+
+    elif file_type == 'json':
+        try:
+            with io.open(file_name, 'r') as f:  # open in text mode for json files
+                fb.fil[0] = json.load(f)
+
+        except IOError as e:
+            logger.error(f"Failed loading {file_name}!\n{e}")
+            return -1
+    else:
+        logger.error(f'Unknown file type "{file_type}"')
+        err = True
+
+    if '_id' not in fb.fil[0] or len(fb.fil[0]['_id']) != 2\
+            or fb.fil[0]['_id'][0] != 'pyfda':
+        msg = "This is no pyfda filter or an outdated file format! Load anyway?"
+        err = not popup_warning(None, message=msg)
+
+    elif fb.fil[0]['_id'][1] != FILTER_FILE_VERSION:
+        msg = (
+            f"The filter file has version {str(fb.fil[0]['_id'][1])} instead of "
+            f"of required version {FILTER_FILE_VERSION}! Load anyway?")
+        err = not popup_warning(None, message=msg)
+
+    # Catch errors occurring during file opening
+    if err:
+        fb.undo()
         return -1
+
+# --------------------
+    try:
+        keys_missing, keys_unsupported = sanitize_imported_dict(fb.fil[0])
+        err_str = ""
+        if keys_missing != []:
+            # '\n'.join(...) converts list to multi-line string
+            err_str += (
+                f"The following {len(keys_missing)} key(s) have not been found in "
+                f"the loaded dict,\n"\
+                f"\tthey are copied with their values from the reference dict:\n"
+                    + "{0}".format('\n'.join(keys_missing))
+                )
+        if keys_unsupported != []:
+            err_str += (
+                f"\nThe following {len(keys_unsupported)} key(s) are not part of the "
+                f"reference dict and have been deleted:\n"
+                + "{0}".format('\n'.join(keys_unsupported))
+            )
+        if err_str != "":
+            logger.warning(err_str)
+
+        # sanitize *values* in filter dictionary, keys are ok by now
+        for k in fb.fil[0]:
+            # Bytes need to be decoded for py3 to be used as keys later on
+            if type(fb.fil[0][k]) == bytes:
+                fb.fil[0][k] = fb.fil[0][k].decode('utf-8')
+            if fb.fil[0][k] is None:
+                logger.warning(f"Entry fb.fil[0][{k}] is empty!")
+        if 'ba' not in fb.fil[0]\
+            or type(fb.fil[0]['ba']) not in {list, np.ndarray}\
+                or np.ndim(fb.fil[0]['ba']) != 2\
+                or (np.shape(fb.fil[0]['ba'][0]) != 2
+                    and np.shape(fb.fil[0]['ba'])[1] < 3):
+            logger.error("Missing key 'ba' or wrong data type!")
+            fb.undo()
+            return -1
+        elif 'zpk' not in fb.fil[0]:
+            logger.error("Missing key 'zpk'!")
+            fb.undo()
+            return -1
+        elif 'sos' not in fb.fil[0]\
+                or type(fb.fil[0]['sos']) not in {list, np.ndarray}:
+            logger.error("Missing key 'sos' or wrong data type!")
+            fb.undo()
+            return -1
+
+        if type(fb.fil[0]['ba']) == np.ndarray:
+            if np.ndim(fb.fil[0]['ba']) != 2:
+                logger.error(
+                    f"Unsuitable dimension of 'ba' data, ndim = {np.ndim(fb.fil[0]['ba'])}")
+            elif np.shape(fb.fil[0]['ba'])[0] != 2:
+                logger.error(
+                    f"Unsuitable shape {np.shape(fb.fil[0]['ba'])} of 'ba' data ")
+        elif type(fb.fil[0]['ba']) == list:
+            fb.fil[0]['ba'] = iter2ndarray(fb.fil[0]['ba'])
+
+        if type(fb.fil[0]['zpk']) == np.ndarray:
+            if np.ndim(fb.fil[0]['zpk']) != 2:
+                logger.error(
+                    f"Unsuitable dimension of 'zpk' data, ndim = {np.ndim(fb.fil[0]['zpk'])}")
+            elif np.shape(fb.fil[0]['zpk'])[0] != 3:
+                logger.error(
+                    f"Unsuitable shape {np.shape(fb.fil[0]['zpk'])} of 'zpk' data ")
+        elif type(fb.fil[0]['zpk']) == list:
+            fb.fil[0]['zpk'] = iter2ndarray(fb.fil[0]['zpk'])
+
+        logger.info(f'Successfully loaded filter\n\t"{file_name}"')
+        dirs.last_file_name = file_name
+        dirs.last_file_dir = os.path.dirname(file_name)  # update default working dir
+        dirs.last_file_type = file_type  # save new default file type
+        return 0
+
     except Exception as e:
-        logger.error("Unexpected error:\n{0}".format(e))
-        fb.fil[0] = fb.fil[1]  # restore backup
+        logger.error(f"Unexpected error:\n{e}")
+        fb.undo()
         return -1
 
 
 # ------------------------------------------------------------------------------
 def save_filter(self):
     """
-    Save filter as zipped binary numpy array or pickle object
+    Save filter as JSON formatted textfile, zipped binary numpy array or pickle object
     """
+    # provide an identifier with version number for pyfda files
+    fb.fil[0].update({'_id': ['pyfda', FILTER_FILE_VERSION]})
+
     file_name, file_type = select_file(
-        self, title="Save Filter", mode='wb', file_types = ("npz", "pkl"))
+        self, title="Save Filter", mode='w', file_types = ("json", "npz", "pkl"))
 
     if file_name is None:
         return -1  # operation cancelled or other error
     err = False
-    try:
-        with io.open(file_name, 'wb') as f:
-            if file_type == 'npz':
-                logger.warning(pprint_log(fb.fil[0]))
-                np.savez(f, **fb.fil[0])
-            elif file_type == 'pkl':
-                pickle.dump(fb.fil[0], f)  # save in default pickle version
-            else:
-                err = True
-                logger.error('Unknown file type "{0}"'.format(file_type))
+    if file_type in {"npz", "pkl"}:
+        try:
+            with io.open(file_name, 'wb') as f:  # open in binary mode
+                if file_type == 'npz':
+                    np.savez(f, **fb.fil[0])
+                else:  # file_type == 'pkl':
+                    pickle.dump(fb.fil[0], f)  # save in default pickle version
+
+        except IOError as e:
+            err = True
+            logger.error(f'Failed saving "{file_name}"!\n{e}')
 
-        if not err:
-            logger.info(f'Filter saved as\n\t"{file_name}"')
-            dirs.last_file_name = file_name
-            dirs.last_file_dir = os.path.dirname(file_name)  # save new dir
-            dirs.last_file_type = file_type  # save file type
+    elif file_type == 'json':
+        try:
+            with io.open(file_name, 'w') as f:  # open in text mode
+                # first, convert dict containing numpy arrays to a pure json string
+                fb_fil_0_json = json.dumps(fb.fil[0], cls=NumpyEncoder, indent=2,
+                                        ensure_ascii=False, sort_keys=True )
+                # next, dump the string to a file
+                f.write(fb_fil_0_json)
+
+        except IOError as e:
+            err = True
+            logger.error(f'Failed saving "{file_name}"!\n{e}')
+    else:
+        err = True
+        logger.error('Unknown file type "{0}"'.format(file_type))
 
-    except IOError as e:
-        logger.error('Failed saving "{0}"!\n{1}'.format(file_name, e))
+    if not err:
+        logger.info(f'Filter saved as\n\t"{file_name}"')
+        dirs.last_file_name = file_name
+        dirs.last_file_dir = os.path.dirname(file_name)  # save new default dir
+        dirs.last_file_type = file_type  # save new default file type
+
+
+# ------------------------------------------------------------------------------
+class NumpyEncoder(json.JSONEncoder):
+    """
+    Special json encoder for numpy and other non-supported types, building upon
+    https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable
+    """
+    def default(self, obj):
+        if isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        elif isinstance(obj, np.ndarray):
+            return obj.tolist()
+        elif isinstance(obj, complex):
+            if obj.imag < 0:
+                return str(obj.real) + str(obj.imag) + "j"
+            else:
+                return str(obj.real) + "+" + str(obj.imag) + "j"
+        elif callable(obj):
+            logger.warning(f"Object '{obj}' not JSON serializable as it is a function.")
+            return ""
+        else:
+            try:
+                return json.JSONEncoder.default(self, obj)
+            except TypeError as e:
+                logger.warning(
+                    f"Object of type '{type(obj)}' is not JSON serializable.\n{e}")
+                return ""
 
 
 # ==============================================================================
 if __name__ == '__main__':
     pass
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from numpy import ndarray, pi, log10, sin, cos
 import numexpr
 import markdown
 
 import scipy.signal as sig
 
 from distutils.version import LooseVersion
+import pyfda.filterbroker as fb
 import pyfda.libs.pyfda_dirs as dirs
 import pyfda.libs.pyfda_sig_lib as pyfda_sig_lib
 
 # ###### VERSIONS and related stuff ############################################
 # ================ Required Modules ============================
 # ==
 # == When one of the following imports fails, terminate the program
@@ -84,41 +85,41 @@
            }
 
 # ================ Optional Modules ============================
 try:
     from docutils import __version__ as V_DOC
     MODULES.update({'docutils': {'V_DOC': V_DOC}})
 except ImportError:
-    pass
+    MODULES.update({'docutils': {'V_DOC': "not found"}})
 
 try:
     from mplcursors import __version__ as V_CUR
     MODULES.update({'mplcursors': {'V_CUR': V_CUR}})
 except ImportError:
-    pass
+    MODULES.update({'mplcursors': {'V_CUR': "not found"}})
 
 MODULES.update({'yosys': {'V_YO': dirs.YOSYS_VER}})
 
 try:
     from xlwt import __version__ as V_XLWT
     MODULES.update({'xlwt': {'V_XLWT': V_XLWT}})
 except ImportError:
-    pass
+    MODULES.update({'xlwt': {'V_XLWT': "not found"}})
 
 try:
     from xlsxwriter import __version__ as V_XLSX
     MODULES.update({'xlsx': {'V_XLSX': V_XLSX}})
 except ImportError:
-    pass
+    MODULES.update({'xlsx': {'V_XLSX': "not found"}})
 
 try:
     from amaranth import __version__ as V_AM
     MODULES.update({'amaranth': {'V_AM': V_AM}})
 except ImportError:
-    pass
+    MODULES.update({'amaranth': {'V_AM': "not found"}})
 
 
 # Remove module names as keys and return a dict with items like
 #  {'V_MPL':'3.3.1', ...}
 MOD_VERSIONS = {}
 for k in MODULES.keys():
     MOD_VERSIONS.update(MODULES[k])
@@ -332,14 +333,34 @@
     """
     return str(text)  # this should be sufficient for Python 3 ?!
 
 ###############################################################################
 # General functions ###########################################################
 ###############################################################################
 
+def is_numeric(a) -> bool:
+    """
+    Return True when a or a.dtype is of a numeric type (complex, float, int, ...)
+
+    Parameters
+    ----------
+    a : array-like or scalar
+
+    Returns
+    -------
+    is_num : bool
+        True when dtype of a is a numeric subtype
+    """
+    if isinstance(a, np.ndarray):
+        is_num = np.issubdtype(a.dtype, np.number)
+    else:
+        is_num = np.issubdtype(type(a), np.number)
+    return is_num
+
+
 def np_type(a):
     """
     Return the python type of `a`, either of the parameter itself or (if it's a
     numpy array) of its items.
 
     Parameters
     ----------
@@ -407,28 +428,89 @@
             return np.nan_to_num(np.array(arrs, dtype=dtype))  # convert list of arrays to two-dimensional array
         else:
             logger.error(f"Unsupported type '{type(iterable)}' for conversion to ndarray.")
             return None
     except Exception as e:
         logger.error(f"Error '{e}'\nfor iterable =\n{iterable}")
         return None
+
+
 # -----------------------------------------------------------------------------
 def set_dict_defaults(d: dict, default_dict: dict) -> None:
     """
-    Add the key:value pairs of `default_dict` to dictionary `d` for all missing
-    keys
+    Add the key:value pairs of `default_dict` to dictionary `d` in-place for
+    all missing keys.
     """
-    if d is None or d == {}:
-        d = default_dict
+    # Create a list of keys to avoid "dictionary size changed" runtime error
+    for k in list(d.keys()):
+        if k not in default_dict:
+            d.pop(k)
+            logger.warning(f"Deleted key '{k}' (not part of default dict).")
+    if d == {}:
+        d.update(default_dict)
     else:
         for k, v in default_dict.items():
             if k not in d:
                 d[k] = v
 
 
+# -------------------------------------------------------------------------------
+def sanitize_imported_dict(new_dict: dict) -> list:
+
+    def compare_dictionaries(
+            ref_dict: dict, new_dict: dict, path: str = "") -> list:
+        """
+        Compare recursively a new dictionary `new_dict` to a reference dictionary `ref_dict`.
+        Keys in `new_dict` that are not contained in `ref_dict` are deleted from `new_dict`,
+        keys in `ref_dict` missing in `new_dict` are copied with their value to `new_dict`.
+
+        Params
+        ------
+        ref_dict: dict
+            reference dictionary
+        new_dict: dict
+            new dictionary
+        path: str
+            current path while traversing through the dictionaries
+
+        Returns
+        -------
+        key_errs: list
+            `key_errs[0]` contains all keys copied from `ref_dict` to `new_dict`.
+            `key_errs[1]` contains all discarded keys from `new_dict`.
+        """
+        key_errs = [[], []]
+        old_path = path
+
+        for k in ref_dict:
+            path = old_path + f"'{k}'"
+            if not k in new_dict:
+                key_errs[0].append(path)
+                new_dict.update({k: ref_dict[k]})
+            else:
+                if isinstance(ref_dict[k], dict) and isinstance(new_dict[k], dict):
+                    key_errs.append(compare_dictionaries(ref_dict[k], new_dict[k], path))
+
+        # emulate slightly inefficient Python 2 way of copying the dict keys to a list
+        # to avoid runtime error "dictionary changed size during iteration" due to new_dict.pop(k)
+        for k in list(new_dict):
+            path = old_path + f"'{k}'"
+            if not k in ref_dict:
+                key_errs[1].append(path)
+                new_dict.pop(k)
+
+        return key_errs
+    # ----------------------------------------
+    key_errs = compare_dictionaries(fb.fil_ref, new_dict)
+    key_errs[0].sort()
+    key_errs[1].sort()
+
+    return key_errs[0], key_errs[1]
+
+
 # -----------------------------------------------------------------------------
 def first_item(d: dict) -> str:
     """
     Return the first item of the dictionary as a string. This only works in a
     reproducible fashion for Python 3.7 and above.
     """
     k = next(iter(d))
@@ -486,20 +568,22 @@
         try:
             _ = np.asarray(d)
         except (TypeError, ValueError) as e:
             logger.warning(f"pprint_log(): Could not transform data to array:\n{e}")
             return ""
 
     if type(d) in {list, np.ndarray, tuple}:
-        if np.ndim(d) == 1:
-            s += (f'Type: {type(d).__name__} of {type(d[0]).__name__}, '
-                  f'shape =  ({len(d)},)' + cr + tab)
-            s += str(d[: min(N-1, len(d))])
+        if np.ndim(d) == 0: # iterable with a single element
+            s = str(d) + f' of type: {type(d).__name__}'
+        elif np.ndim(d) == 1:
+            s = cr + tab + str(d[: min(N-1, len(d))])
             if len(d) > N-1:
                 s += ' ...'
+            s += (cr + tab + f'Type: {type(d).__name__} of {type(d[0]).__name__}, '
+                  f'with shape = ({len(d)},)')
         elif np.ndim(d) == 2:
             rows, cols = np.shape(d)
             s += (f'Type: {type(d).__name__} of {type(d[0][0]).__name__}, '
                   f'shape = (r{rows} x c{cols})' + cr + tab)
             #  x.dtype.kind returns general information on numpy data (e.g. "iufc","SU")
             for r in range(min(N, rows)):
                 if not first:
@@ -519,17 +603,17 @@
         if type(d) is None:
             s += ('Type: None')
         elif type(d) is str:
             s += (f' Type: str, length = {len(d)}' +  cr + tab + d[: min(N-1, len(d))])
             if len(d) > N-1:
                 s += ' ...'
         elif np.isscalar(d):
-            s += (f'Type: {type(d).__name__}' + cr + tab + str(d))
+            s = str(d) + f' of type: {type(d).__name__}'
         else:
-            s += (f'Type: {type(d).__name__}')
+            s += 'Type: {type(d).__name__}'
     return s
 
 
 # ------------------------------------------------------------------------------
 def safe_numexpr_eval(expr: str, fallback=None,
                       local_dict: dict = {}) -> ndarray:
     """
@@ -627,15 +711,16 @@
     if not type(np_expr.item(0)) in {float, complex}:
         np_expr = np_expr.astype(float)
 
     return np_expr
 
 
 # ------------------------------------------------------------------------------
-def safe_eval(expr, alt_expr=0, return_type: str = "float", sign: str = None) -> str:
+def safe_eval(expr, alt_expr=0, return_type: str = "float", sign: str = None
+              ):  # -> complex|float|int: only works with py3.10 upawards
     """
     Try ... except wrapper around numexpr to catch various errors
     When evaluation fails or returns `None`, try evaluating `alt_expr`.
     When this also fails, return 0 to avoid errors further downstream.
 
     Parameters
     ----------
@@ -1445,15 +1530,15 @@
     elif format_in == 'zpk':
         format_error = False
         if isinstance(arg, np.ndarray) and np.ndim(arg) == 1:
             frmt = "nd1" #  one-dimensional numpy array
             logger.info(f"Format (zpk) is '{frmt}', shape = {np.shape(arg)}")
         elif isinstance(arg, np.ndarray) and np.ndim(arg) == 2:
             frmt = "nd2" #  two-dimensional numpy array
-            logger.info(f"Format (zpk) is '{frmt}', shape = {np.shape(arg)}")
+            # logger.info(f"Format (zpk) is '{frmt}', shape = {np.shape(arg)}")
         # elif any(isinstance(el, list) for el in arg):
         #     frmt = "lol"  # list or ndarray or tuple of lists
         elif any(isinstance(el, np.ndarray) for el in arg):
             frmt = "lon"  # list or tuple of ndarrays
             logger.warning(f"Format (zpk) is '{frmt}'.")
         else:
             format_error = True
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_log_template.conf` & `pyfda-0.9.0b1/pyfda/libs/pyfda_log_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_qt_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_qt_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,66 @@
     Qt, QtGui, QtCore, QFrame, QMessageBox, QPushButton, QLabel, QComboBox, QDialog,
     QFont, QSize, QFontMetrics, QIcon, QEvent)
 from .pyfda_dirs import OS, OS_VER
 
 import logging
 logger = logging.getLogger(__name__)
 
-
+DICT_SIG_KEYS = {'id', 'class', 'ttl', 'sender_name', 'object_name',
+                 'view_changed',   # view on the data (e.g. f_S) has changed
+                 'specs_changed',  # filter specs (corner freqs. etc.) have changed
+                 'data_changed',   # actual filter data (coeffs. etc.) has changed
+                 'filt_changed',   # the filter type (e.g. elliptic) has changed
+                 'ui_local_changed',  # some parameter in the local ui has changed
+                 'ui_global_changed', # this relates to resize, tab change or CSV options
+                 'fx_sim',         # parameters relating to fixpoint simulation
+                 'fxfilter_func',  # handle to filter function
+                 'close_event'     # propagate close event to finish some task upstream
+                }
 # ------------------------------------------------------------------------------
 def emit(self, dict_sig: dict = {}, sig_name: str = 'sig_tx') -> None:
     """
     Emit a signal `self.<sig_name>` (defined as a class attribute) with a
     dict `dict_sig` using Qt's `emit()`.
     - Add the keys `'id'` and `'class'` with id resp. class name of the calling
       instance if not contained in the dict
     - If key 'ttl' is in the dict and its value is less than one, terminate the
       signal. Otherwise, reduce the value by one.
     - If the sender has passed an objectName, add it with the key "sender_name"
       to the dict.
 
     """
-
+    for k in dict_sig:
+        if k not in DICT_SIG_KEYS:
+            logger.warning(f"Unknown entry '{k}':'{dict_sig[k]}' in 'dict_sig'!")
+            logger.warning(pprint_log(dict_sig))
+    # if self.sender() and self.sender().objectName():
+    #     logger.info(f"this_sender_name: {self.sender().objectName()}")
+    # logger.info(f"objectName = {self.objectName()}")
     if 'id' not in dict_sig:
         dict_sig.update({'id': id(self)})
     if 'class' not in dict_sig:
         dict_sig.update({'class': self.__class__.__name__})
     # Count down time-to-live counter and terminate the signal when ttl < 1
     if 'ttl' in dict_sig:
         if dict_sig['ttl'] < 1:
+            logger.warning("Terminated with ttl = 0")
             return
         else:
             dict_sig.update({'ttl': dict_sig['ttl'] - 1})
-    if self.sender() and self.sender().objectName():
+    else:
+        dict_sig.update({'ttl': 50})
+    if 'sender_name' not in dict_sig and\
+        self.sender() and self.sender().objectName():
         dict_sig.update({'sender_name': self.sender().objectName()})
+    if 'object_name' not in dict_sig:
+        dict_sig.update({'object_name': self.objectName()})
+
+    # logger.info(f"EMIT:{pprint_log(dict_sig)}")
+
     # Get signal (default name: `sig_tx`) from calling instance and emit it
     signal = getattr(self, sig_name)
     signal.emit(dict_sig)
 
 
 # # ------------------------------------------------------------------------------
 # def sig_loop(self, dict_sig: dict, logger, **kwargs) -> int:
@@ -122,28 +147,30 @@
 
     item_init: str
         data for initial positition of combobox. When data is not found,
         set combobox to first item.
 
     Returns
     -------
-    None
+    Index of `item_init`. If index == -1, `item_init` was not in `items_list`
     """
     cmb_box.clear()
     if type(items_list[0]) is str:  # combo box tool tipp (optional)
         cmb_box.setToolTip(cmb_box.tr(items_list[0]))
     for i in range(1, len(items_list)):
         if type(items_list[i][1]) == QtGui.QIcon:
             cmb_box.addItem("", items_list[i][0])
             cmb_box.setItemIcon(i-1, items_list[i][1])
         else:
             cmb_box.addItem(cmb_box.tr(items_list[i][1]), items_list[i][0])
         if len(items_list[i]) == 3:  # add item tool tip (optional)
             cmb_box.setItemData(i-1, cmb_box.tr(items_list[i][2]), Qt.ToolTipRole)
-    qset_cmb_box(cmb_box, item_init, data=True)
+    ret = qset_cmb_box(cmb_box, item_init, data=True)
+
+    return ret
 
     """ icon = QIcon('logo.png')
     # adding icon to the given index
     self.combo_box.setItemIcon(i, icon)
     size = QSize(10, 10)
     self.combo_box.setIconSize(size)  """
 
@@ -387,32 +414,32 @@
     """
     Apply the "state" defined in pyfda_rc.py to the widget, e.g.:
     Color the >> DESIGN FILTER << button according to the filter design state.
 
     This requires setting the property, "unpolishing" and "polishing" the widget
     and finally forcing an update.
 
-    - "normal": default, no color styling
-    - "ok":  green, filter has been designed, everything ok
-    - "changed": yellow, filter specs have been changed
-    - "running": orange, simulation is running
-    - "error" : red, an error has occurred during filter design
-    - "failed" : pink, filter fails to meet target specs (not used yet)
-    - "u" or "unused": grey text color
-    - "d" or "disabled": background color darkgrey
-    - "a" or "active": no special style defined
+    - 'normal' : default, no color styling
+    - 'ok':  green, filter has been designed, everything ok
+    - 'changed': yellow, filter specs have been changed
+    - 'running': orange, simulation is running
+    - 'error'  : red, an error has occurred during filter design
+    - 'failed' : pink, filter fails to meet target specs (not used yet)
+    - 'u' or 'unused'  : grey text color
+    - 'd' or 'disabled': background color darkgrey
+    - 'a' or 'active'  : no special style defined
     """
     state = str(state)
     if state == 'u':
-        state = "unused"
+        state = 'unused'
         # *[state="unused"], *[state="u"]{background-color:white; color:darkgrey}
     elif state == 'a':
-        state = "active"
+        state = 'active'
     elif state == 'd':
-        state = "disabled"
+        state = 'disabled'
         # QLineEdit:disabled{background-color:darkgrey;}
     # widget.setAttribute(Qt.WA_StyledBackground, True)
     widget.setProperty("state", state)
     widget.style().unpolish(widget)
     widget.style().polish(widget)
     widget.update()
 
@@ -456,25 +483,28 @@
     # rows = sorted(list({i[1] for i in idx}))
     cur = (table.currentColumn(), table.currentRow())
     # cur_idx_row = table.currentIndex().row()
     return {'idx': idx, 'sel': sel, 'cur': cur}  # 'rows':rows 'cols':cols, }
 
 
 # ----------------------------------------------------------------------------
-def qfilter_warning(self, N, fil_class):
+def popup_warning(self, param1: int = 0, param2: str = "", message: str = "") -> bool:
     """
-    Pop-up a warning box for very large filter orders
+    Pop-up a warning box and require a user prompt. When `message == ""`, warn of
+    very large filter orders, otherwise display the passed message
     """
+    if message == "":
+        message = (
+            f"<span><b><i>N</i> = {param1}</b> is a rather high order for<br />"
+            f"{param2} filters and may cause large <br />"
+            "numerical errors and compute times.<br />Continue?</span>")
+
     reply = QMessageBox.warning(
-        self, 'Warning',
-        ("<span><i><b>N = {0}</b></i> &nbsp; is a rather high order for<br />"
-         "an {1} filter and may cause large <br />"
-         "numerical errors and compute times.<br />"
-         "Continue?</span>".format(N, fil_class)),
-        QMessageBox.Yes, QMessageBox.No)
+        self, 'Warning', message, QMessageBox.Yes, QMessageBox.No)
+
     if reply == QMessageBox.Yes:
         return True
     else:
         return False
 
 
 # ----------------------------------------------------------------------------
@@ -662,17 +692,18 @@
     checkable : bool
         Whether button is checkable
 
     checked : bool
         Whether initial state is checked
     """
     def __init__(self, txt: str = "", icon: QIcon = None, N_x: int = 8,
-                 checkable: bool = True, checked: bool = False):
+                 checkable: bool = True, checked: bool = False, objectName=""):
         super(PushButton, self).__init__()
 
+        self.setObjectName(objectName)
         self.setCheckable(checkable)
         self.setChecked(checked)
         if icon is None:
             self.w = qtext_width(text=txt, N_x=N_x, font=self.font())
             self.h = super(PushButton, self).sizeHint().height()
             self.setText(txt.strip())
         else:
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_sig_lib.py` & `pyfda-0.9.0b1/pyfda/libs/pyfda_sig_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     if type(zpk) in {np.ndarray, list, tuple}:
         if len(zpk) == 3:  # dimensions are ok, but poles / gain could be empty
             if np.isscalar(zpk[2]) or zpk[2] == []:
                 if zpk[2] == 0:
                     zpk[2] = 1
             else:
-                logger.error(zpk[2])
+                # logger.error(zpk[2])
                 if zpk[2][0] in {0, None}:
                     zpk[2][0] = 1
 
         elif len(zpk) == 2:  # only poles and zeros given:
             zpk = list(zpk)
             zpk.append([1])  # set gain = 1
         elif len(zpk) == 1:  # only zeros given:
```

### Comparing `pyfda-0.8.4/pyfda/libs/pyfda_template.conf` & `pyfda-0.9.0b1/pyfda/libs/pyfda_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/libs/tree_builder.py` & `pyfda-0.9.0b1/pyfda/libs/tree_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .frozendict import freeze_hierarchical
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 # --------------------------------------------------------------------------
-def merge_dicts(d1, d2, path=None, mode='keep1'):
+def merge_dicts_hierarchically(d1, d2, path=None, mode='keep1'):
     """
     Merge the hierarchical dictionaries ``d1`` and ``d2``.  The dict ``d1`` is
     modified in place and returned
 
     Parameters
     ----------
     d1 : dict
@@ -59,21 +59,21 @@
     Returns
     -------
     d1 : dict
         a reference to the first dictionary, merged-in-place.
 
     Example
     -------
-    >>> merge_dicts(fil_tree, fil_tree_add, mode='add1')
+    >>> merge_dicts_hierarchically(fil_tree, fil_tree_add, mode='add1')
 
     Notes
     -----
     If you don't want to modify ``d1`` in place, call the function using:
 
-    >>> new_dict = merge_dicts(dict(d1), d2)
+    >>> new_dict = merge_dicts_hierarchically(dict(d1), d2)
 
     If you need to merge more than two dicts use:
 
     >>> from functools import reduce   # only for py3
     >>> reduce(merge, [d1, d2, d3...]) # add / merge all other dicts into d1
 
     Taken with some modifications from:
@@ -86,15 +86,15 @@
 
     if path is None:
         path = ""
     for key in d2:
         if key in d1:
             if isinstance(d1[key], dict) and isinstance(d2[key], dict):
                 # both entries are dicts, recurse one level deeper:
-                merge_dicts(d1[key], d2[key], path=path + str(key), mode=mode)
+                merge_dicts_hierarchically(d1[key], d2[key], path=path + str(key), mode=mode)
 # TODO:            elif <either d1[key] OR d2[key] is not a dict> -> exception
             elif d1[key] == d2[key] or mode == 'keep1':
                 pass  # keep item in dict1, discard item with same key in dict1
             elif mode == 'keep2':
                 d1[key] = d2[key]  # replace item in dict1 by item in dict2
             else:
                 try:
@@ -181,15 +181,15 @@
 
             # add attributes from dict to fil_tree for filter class fc
             fil_tree = self.build_fil_tree(fc, ff.fil_inst.rt_dict, fil_tree)
 
             # merge additional rt_dict (optional) into filter tree
             if hasattr(ff.fil_inst, 'rt_dict_add'):
                 fil_tree_add = self.build_fil_tree(fc, ff.fil_inst.rt_dict_add)
-                merge_dicts(fil_tree, fil_tree_add, mode='add1')
+                merge_dicts_hierarchically(fil_tree, fil_tree_add, mode='add1')
 
         # Make the dictionary and all sub-dictionaries read-only ("FrozenDict"):
         fb.fil_tree = freeze_hierarchical(fil_tree)
 
         # Test Immutatbility
 #        fil_tree_ref = fb.fil_tree['LP']['FIR']['Equiripple']['min']
 #        fil_tree_ref.update({'msg':("hallo",)}) # this changes  fb.fil_tree !!
@@ -699,15 +699,15 @@
 
             # now append all the individual 'min' / 'man'  subwidget infos to fc:
             fil_tree[rt][ft][fc].update(rt_dict[rt])
 
             if 'COM' in rt_dict:      # Now handle common info
                 for fo in rt_dict[rt]:  # iterate over 'min' / 'max'
                     if fo in rt_dict['COM']:  # and add common info first
-                        merge_dicts(fil_tree[rt][ft][fc][fo],
+                        merge_dicts_hierarchically(fil_tree[rt][ft][fc][fo],
                                     rt_dict['COM'][fo], mode='add2')
 
         return fil_tree
 
 
 # ==============================================================================
 if __name__ == "__main__":
```

### Comparing `pyfda-0.8.4/pyfda/license_info.md` & `pyfda-0.9.0b1/pyfda/license_info.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/module_versions.md` & `pyfda-0.9.0b1/pyfda/module_versions.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/mpl_widget.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/mpl_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_3d.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,72 +87,62 @@
 
         else:
             if 'data_changed' in dict_sig:
                 self.data_changed = True
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
-        self.but_log = PushButton("dB", checked=False)
-        self.but_log.setObjectName("but_log")
+        self.but_log = PushButton("dB", checked=False, objectName="but_log")
         self.but_log.setToolTip("Logarithmic scale")
 
-        self.but_plot_in_UC = PushButton("|z| < 1 ", checked=False)
-        self.but_plot_in_UC.setObjectName("but_plot_in_UC")
+        self.but_plot_in_UC = PushButton("|z| < 1 ", checked=False,
+                                         objectName="but_plot_in_UC")
         self.but_plot_in_UC.setToolTip("Only plot H(z) within the unit circle")
 
         self.lblBottom = QLabel(to_html("Bottom =", frmt='bi'), self)
-        self.ledBottom = QLineEdit(self)
-        self.ledBottom.setObjectName("ledBottom")
+        self.ledBottom = QLineEdit(self, objectName="ledBottom")
         self.ledBottom.setText(str(self.zmin))
         self.ledBottom.setToolTip("Minimum display value.")
         self.lblBottomdB = QLabel("dB", self)
         self.lblBottomdB.setVisible(self.but_log.isChecked())
 
         self.lblTop = QLabel(to_html("Top =", frmt='bi'), self)
-        self.ledTop = QLineEdit(self)
-        self.ledTop.setObjectName("ledTop")
+        self.ledTop = QLineEdit(self, objectName="ledTop")
         self.ledTop.setText(str(self.zmax))
         self.ledTop.setToolTip("Maximum display value.")
         self.lblTopdB = QLabel("dB", self)
         self.lblTopdB.setVisible(self.but_log.isChecked())
 
-        self.plt_UC = PushButton("UC", checked=True)
-        self.plt_UC.setObjectName("plt_UC")
+        self.plt_UC = PushButton("UC", checked=True, objectName="plt_UC")
         self.plt_UC.setToolTip("Plot unit circle")
 
-        self.but_PZ = PushButton("P/Z ", checked=True)
-        self.but_PZ.setObjectName("but_PZ")
+        self.but_PZ = PushButton("P/Z ", checked=True, objectName="but_PZ")
         self.but_PZ.setToolTip("Plot poles and zeros")
 
-        self.but_Hf = PushButton("H(f) ", checked=True)
-        self.but_Hf.setObjectName("but_Hf")
+        self.but_Hf = PushButton("H(f) ", checked=True, objectName="but_Hf")
         self.but_Hf.setToolTip("Plot H(f) along the unit circle")
 
         modes = ['None', 'Mesh', 'Surf', 'Contour']
-        self.cmbMode3D = QComboBox(self)
+        self.cmbMode3D = QComboBox(self, objectName="cmbShow3D")
         self.cmbMode3D.addItems(modes)
-        self.cmbMode3D.setObjectName("cmbShow3D")
         self.cmbMode3D.setToolTip("Select 3D-plot mode.")
         self.cmbMode3D.setCurrentIndex(0)
         self.cmbMode3D.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
-        self.but_colormap_r = PushButton("reverse", checked=True)
-        self.but_colormap_r.setObjectName("but_colormap_r")
+        self.but_colormap_r = PushButton("reverse", checked=True, objectName="but_colormap_r")
         self.but_colormap_r.setToolTip("reverse colormap")
 
         self.cmbColormap = QComboBox(self)
         self._init_cmb_colormap(cmap_init=self.cmap_default)
         self.cmbColormap.setToolTip("Select colormap")
 
-        self.but_colbar = PushButton("Colorbar ", checked=False)
-        self.but_colbar.setObjectName("chkColBar")
+        self.but_colbar = PushButton("Colorbar ", checked=False, objectName="chkColBar")
         self.but_colbar.setToolTip("Show colorbar")
 
-        self.but_lighting = PushButton("Lighting", checked=False)
-        self.but_lighting.setObjectName("but_lighting")
+        self.but_lighting = PushButton("Lighting", checked=False, objectName="but_lighting")
         self.but_lighting.setToolTip("Enable light source")
 
         self.lblAlpha = QLabel(to_html("Alpha", frmt='bi'), self)
         self.diaAlpha = QDial(self)
         self.diaAlpha.setRange(0, 10)
         self.diaAlpha.setValue(10)
         self.diaAlpha.setTracking(False)  # produce less events when turning
@@ -167,16 +157,16 @@
         self.diaHatch.setValue(5)
         self.diaHatch.setTracking(False)  # produce less events when turning
         self.diaHatch.setFixedHeight(30)
         self.diaHatch.setFixedWidth(30)
         self.diaHatch.setWrapping(False)
         self.diaHatch.setToolTip("Set line density for various plots.")
 
-        self.but_contour_2d = PushButton("Contour2D ", checked=False)
-        self.but_contour_2d.setObjectName("chkContour2D")
+        self.but_contour_2d = PushButton("Contour2D ", checked=False,
+                                         objectName="chkContour2D")
         self.but_contour_2d.setToolTip("Plot 2D-contours at z =0")
 
         # ----------------------------------------------------------------------
         # LAYOUT for UI widgets
         # ----------------------------------------------------------------------
         layGControls = QGridLayout()
         layGControls.addWidget(self.but_log, 0, 0)
@@ -204,16 +194,15 @@
         layGControls.addWidget(self.lblAlpha, 0, 15)
         layGControls.addWidget(self.diaAlpha, 0, 16)
 
         layGControls.addWidget(self.lblHatch, 1, 15)
         layGControls.addWidget(self.diaHatch, 1, 16)
 
         # This widget encompasses all control subwidgets
-        self.frmControls = QFrame(self)
-        self.frmControls.setObjectName("frmControls")
+        self.frmControls = QFrame(self, objectName="frmControls")
         self.frmControls.setLayout(layGControls)
 
         # ----------------------------------------------------------------------
         # mplwidget
         # ----------------------------------------------------------------------
         # This is the plot pane widget, encompassing the other widgets
         self.mplwidget = MplWidget(self)
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_fft_win.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_fft_win.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,28 +156,28 @@
         Intitialize the widget, consisting of:
         - Matplotlib widget with NavigationToolbar
         - Frame with control elements
         """
         self.bfont = QFont()
         self.bfont.setBold(True)
 
-        self.qfft_win_select = QFFTWinSelector(self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict, objectName='plot_fft_win_qfft')
 
         self.lbl_N = QLabel(to_html("N =", frmt='bi'))
         self.led_N = QLineEdit(self)
         self.led_N.setText(str(self.N_view))
         self.led_N.setMaximumWidth(qtext_width(N_x=8))
         self.led_N.setToolTip(
             "<span>Number of window data points to display.</span>")
 
         # By default, the enter key triggers the default 'dialog action' in QDialog
-        # widgets. This activates one of the pushbuttons.
-        self.but_log_t = QPushButton("dB", default=False, autoDefault=False)
+        # widgets. This would activate one of the pushbuttons if `default` wasn't False.
+        self.but_log_t = QPushButton("dB", default=False, autoDefault=False,
+                                     objectName="chk_log_time")
         self.but_log_t.setMaximumWidth(qtext_width(" dB "))
-        self.but_log_t.setObjectName("chk_log_time")
         self.but_log_t.setCheckable(True)
         self.but_log_t.setChecked(False)
         self.but_log_t.setToolTip("Display in dB")
 
         self.led_log_bottom_t = QLineEdit(self)
         self.led_log_bottom_t.setVisible(self.but_log_t.isChecked())
         self.led_log_bottom_t.setText(str(self.bottom_t))
@@ -200,17 +200,17 @@
         self.but_half_f.setChecked(True)
         self.but_half_f.setMaximumWidth(qtext_width(text=" 0...½ "))
         self.but_half_f.setToolTip(
             "Display window spectrum in the range 0 ... 0.5 f_S.")
 
         # By default, the enter key triggers the default 'dialog action' in QDialog
         # widgets. This activates one of the pushbuttons.
-        self.but_log_f = QPushButton("dB", default=False, autoDefault=False)
+        self.but_log_f = QPushButton("dB", default=False, autoDefault=False,
+                                     objectName="chk_log_freq")
         self.but_log_f.setMaximumWidth(qtext_width(" dB "))
-        self.but_log_f.setObjectName("chk_log_freq")
         self.but_log_f.setToolTip("<span>Display in dB.</span>")
         self.but_log_f.setCheckable(True)
         self.but_log_f.setChecked(True)
 
         self.lbl_log_bottom_f = QLabel(to_html("min =", frmt='bi'), self)
         self.lbl_log_bottom_f.setVisible(self.but_log_f.isChecked())
 
@@ -226,16 +226,15 @@
         #
         # This widget encompasses all control subwidgets
         # ----------------------------------------------------------------------
         layH_win_select = QHBoxLayout()
         layH_win_select.addWidget(self.qfft_win_select)
         layH_win_select.setContentsMargins(0, 0, 0, 0)
         layH_win_select.addStretch(1)
-        frmQFFT = QFrame(self)
-        frmQFFT.setObjectName("frmQFFT")
+        frmQFFT = QFrame(self, objectName="frmQFFT")
         frmQFFT.setLayout(layH_win_select)
 
         hline = QHLine()
 
         layHControls = QHBoxLayout()
         layHControls.addWidget(self.lbl_N)
         layHControls.addWidget(self.led_N)
@@ -255,16 +254,15 @@
         layHControls.addWidget(self.but_log_f)
 
         layVControls = QVBoxLayout()
         layVControls.addWidget(frmQFFT)
         layVControls.addWidget(hline)
         layVControls.addLayout(layHControls)
 
-        frmControls = QFrame(self)
-        frmControls.setObjectName("frmControls")
+        frmControls = QFrame(self, objectName="frmControls")
         frmControls.setLayout(layVControls)
 
         # ----------------------------------------------------------------------
         #               ### mplwidget ###
         #
         # Layout layVMainMpl (VBox) is defined within MplWidget, additional
         # widgets can be added below the matplotlib widget (here: frmControls)
@@ -303,16 +301,15 @@
 
         self.txtInfoBox = QTextBrowser(self)
 
         layVInfo = QVBoxLayout(self)
         layVInfo.addWidget(self.tbl_win_props)
         layVInfo.addWidget(self.txtInfoBox)
 
-        frmInfo = QFrame(self)
-        frmInfo.setObjectName("frmInfo")
+        frmInfo = QFrame(self, objectName="frmInfo")
         frmInfo.setLayout(layVInfo)
 
         # ----------------------------------------------------------------------
         #               ### splitter ###
         #
         # This widget encompasses all subwidgets
         # ----------------------------------------------------------------------
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_hf.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,27 +65,29 @@
         Process signals coming from the navigation toolbar and from sig_rx
         """
         # logger.debug("SIG_RX - needs_calc = {0}, vis = {1}\n{2}"\
         #              .format(self.needs_calc, self.isVisible(), pprint_log(dict_sig)))
 
         if self.isVisible():
             if 'data_changed' in dict_sig or 'specs_changed' in dict_sig\
+                    or 'filt_changed' in dict_sig\
                     or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home')\
                          or self.needs_calc:
                 self.draw()
                 self.needs_calc = False
                 self.needs_draw = False
             if 'view_changed' in dict_sig or self.needs_draw:
                 self.update_view()
                 self.needs_draw = False
             elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
                 self.frmControls.setVisible(dict_sig['value'] == 0)
 
         else:
-            if 'data_changed' in dict_sig or 'specs_changed' in dict_sig:
+            if 'data_changed' in dict_sig or 'specs_changed' in dict_sig\
+                    or 'filt_changed' in dict_sig:
                 self.needs_calc = True
             if 'view_changed' in dict_sig:
                 self.needs_draw = True
 
     def _construct_ui(self):
         """
         Define and construct the subwidgets
@@ -109,18 +111,17 @@
         layG_show_H.addWidget(self.lbl_show_H_im, 2, 0)
         layG_show_H.addWidget(self.chk_show_H_im, 2, 1)
         layG_show_H.setContentsMargins(0,0,10,0)
         layG_show_H.setSpacing(0)
 
         self.lblIn = QLabel(to_html("Unit:", frmt="b"), self)
 
-        self.cmb_units_a = QComboBox(self)
+        self.cmb_units_a = QComboBox(self, objectName="cmbUnitsA")
         qcmb_box_populate(self.cmb_units_a, self.cmb_units_a_items,
                           self.cmb_units_a_default)
-        self.cmb_units_a.setObjectName("cmbUnitsA")
 
         self.lbl_log_bottom = QLabel(to_html("min =", 'bi'), self)
         self.led_log_bottom = QLineEdit(self)
         self.led_log_bottom.setText(str(self.log_bottom))
         self.led_log_bottom.setMaximumWidth(qtext_width(N_x=8))
         self.led_log_bottom.setToolTip(
             "<span>Minimum display value for dB. scale.</span>")
@@ -130,17 +131,16 @@
 
         self.but_zerophase = PushButton(" Zero phase ", checked=False)
         self.but_zerophase.setToolTip(
             "<span>Remove linear phase calculated from filter order.\n"
             "Attention: This makes no sense for a non-linear phase system!</span>")
 
         self.lblInset = QLabel(to_html("Inset", "bi"), self)
-        self.cmbInset = QComboBox(self)
+        self.cmbInset = QComboBox(self, objectName="cmbInset")
         self.cmbInset.addItems(['off', 'edit', 'fixed'])
-        self.cmbInset.setObjectName("cmbInset")
         self.cmbInset.setToolTip("Display/edit second inset plot")
         self.cmbInset.setCurrentIndex(0)
         self.inset_idx = 0  # store previous index for comparison
 
         self.but_specs = PushButton("Specs ", checked=False)
         self.but_specs.setToolTip("Display filter specs as hatched regions")
 
@@ -174,16 +174,15 @@
         layHControls.addStretch(1)
         layHControls.addWidget(self.but_specs)
         layHControls.addStretch(1)
         layHControls.addWidget(self.but_phase)
         layHControls.addWidget(self.but_align)
         layHControls.addStretch(10)
 
-        self.frmControls = QFrame(self)
-        self.frmControls.setObjectName("frmControls")
+        self.frmControls = QFrame(self, objectName="frmControls")
         self.frmControls.setLayout(layHControls)
 
         # ----------------------------------------------------------------------
         #               ### mplwidget ###
         #
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_impz.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_impz.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # import matplotlib.lines as lines
 from matplotlib.ticker import AutoMinorLocator
 
 import pyfda.filterbroker as fb
 import pyfda.libs.pyfda_fix_lib as fx
 from pyfda.libs.pyfda_sig_lib import angle_zero
 from pyfda.libs.pyfda_lib import (
-    safe_eval, pprint_log, calc_ssb_spectrum, calc_Hcomplex)
+    safe_eval, pprint_log, calc_ssb_spectrum, calc_Hcomplex, first_item)
 from pyfda.libs.pyfda_qt_lib import (
     qget_cmb_box, qset_cmb_box, qstyle_widget, qcmb_box_add_item, qcmb_box_del_item)
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 from pyfda.plot_widgets.mpl_widget import MplWidget, stems, scatter
 
 from pyfda.plot_widgets.tran.plot_tran_stim import Plot_Tran_Stim
 from pyfda.plot_widgets.tran.tran_io import Tran_IO
@@ -47,33 +47,34 @@
     """
     Construct a widget for plotting impulse and general transient responses
     """
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing, e.g. when stimulus has been calculated
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self):
+    def __init__(self, objectName='plot_impz_inst'):
         super().__init__()
 
         # arrays that need to be passed to subwidgets
+        self.setObjectName(objectName)
         self.x = self.y = self.x_q = None
 
         # create the UI part with buttons etc.
         self.ui = PlotImpz_UI()
 
         # initial settings
         # ==================
         # flag whether specs have been changed and plots need to be recalculated
         self.needs_calc = True
         # same when fixpoint specs have been changed, only needed in Fixpoint mode
         self.needs_calc_fx = True
         self.needs_redraw = [True] * 2  # flag which plot needs to be redrawn
         self.error = False
         fb.fil[0]['fx_sim'] = False  # disable fixpoint mode initially
-        self.fx_sim_old = fb.fil[0]['fx_sim']
+        self.fx_mode_old = fb.fil[0]['fx_sim']
         self.tool_tip = "Impulse / transient response and their spectra"
         self.tab_label = "y[n]"
         self.active_tab = 0  # index for active tab
         # markersize=None, markeredgewidth=None, markeredgecolor=None,
         # markerfacecolor=None, markerfacecoloralt='none', fillstyle=None,
         self.fmt_mkr_size = 8
         self.fmt_plot_resp = {'color': 'red', 'linewidth': 2, 'alpha': 0.5}
@@ -88,18 +89,15 @@
         self.fmt_mkr_stmq = {'marker': 'D', 'color': 'darkgreen', 'alpha': 0.5,
                              'ms': self.fmt_mkr_size}
 
         self._construct_UI()
 
         # --------------------------------------------
         # initialize UI and `fb.fil[0]['fx_sim']` for fixpoint or float simulation
-        # self.update_fx_ui_settings(qget_cmb_box(self.ui.cmb_sim_select, data=False))
-        self.update_fx_ui_settings()
-        # store current state of `fb.fil[0]['fx_sim']``
-        # self.fx_sim_old = fb.fil[0]['fx_sim']
+        self.toggle_fx_settings()
 
         self.impz_init()  # initial calculation of stimulus and response and drawing
 
     def _construct_UI(self):
         """
         Create the top level UI of the widget, consisting of tabbed matplotlib widgets,
         tabbed stimuli and a control frame.
@@ -212,33 +210,33 @@
         # When user has selected a different local tab, trigger a redraw of current tab
         self.tab_mpl_w.currentChanged.connect(self.draw)  # passes # of active tab
         # ---------------------------------------------------------------------
         # UI SIGNALS & SLOTs
         # ---------------------------------------------------------------------
         self.tab_stim_w.currentChanged.connect(self.resize_stim_tab_widget)
         # --- run control ---
-        self.ui.cmb_sim_select.currentIndexChanged.connect(self.toggle_fx_setting)
+        self.ui.cmb_sim_select.currentIndexChanged.connect(self.toggle_fx_settings)
         self.ui.but_run.clicked.connect(self.impz_init)
         self.ui.but_auto_run.clicked.connect(self.calc_auto)
-        self.ui.but_fx_scale.clicked.connect(self.draw)
         self.stim_wdg.ui.but_file_io.clicked.connect(self.set_N_to_file_len)
         # --- time domain plotting --------------------------------------------
         self.ui.cmb_plt_time_resp.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_time_stim.currentIndexChanged.connect(self.draw)
         self.ui.chk_plt_time_stim_interp.clicked.connect(self.draw)
         self.ui.cmb_plt_time_stmq.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_time_spgr.currentIndexChanged.connect(self._spgr_cmb)
         self.ui.but_log_time.clicked.connect(self.draw)
         self.ui.led_log_bottom_time.editingFinished.connect(self.draw)
         self.ui.but_log_spgr_time.clicked.connect(self.draw)
         self.ui.led_time_nfft_spgr.editingFinished.connect(self._spgr_ui2params)
         self.ui.led_time_ovlp_spgr.editingFinished.connect(self._spgr_ui2params)
         self.ui.cmb_mode_spgr_time.currentIndexChanged.connect(self.draw)
         self.ui.chk_byfs_spgr_time.clicked.connect(self.draw)
-        self.ui.but_fx_range.clicked.connect(self.draw)
+        self.ui.but_fx_range_x.clicked.connect(self.draw)
+        self.ui.but_fx_range_y.clicked.connect(self.draw)
         self.ui.chk_win_time.clicked.connect(self.draw)
         # --- frequency domain plotting ---------------------------------------
         self.ui.cmb_plt_freq_resp.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_freq_stim.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_freq_stmq.currentIndexChanged.connect(self.draw)
         self.ui.but_Hf.clicked.connect(self.draw)
         self.ui.cmb_freq_display.currentIndexChanged.connect(self.draw)
@@ -317,64 +315,44 @@
         Process signals coming from
         - the navigation toolbars (time and freq.)
         - local widgets (impz_ui) and
         - plot_tab_widgets() (global signals)
         """
         # logger.warning(
         #     f"SIG_RX - needs_calc: {self.needs_calc} | vis: {self.isVisible()}\n"
-        #     f"{pprint_log(dict_sig)}\n")
-        # logger.debug(f'SIG_RX: "{first_item(dict_sig)}"')
+        #     f"{first_item(dict_sig)}")
 
         if dict_sig['id'] == id(self):
-            # logger.debug(f'Stopped infinite loop: "{first_item(dict_sig)}"')
+            # logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'fx_sim' in dict_sig:
-            # --------------- START (ext. widget) ------------
-            if dict_sig['fx_sim'] == 'start_fx_sim':
-                """
-                Fixpoint simulation started from external widget, e.g.
-                from 'input_fixpoint_specs' by pressing the "Sim FX" button
-                - Reset error flag and set 'needs_calc' flags
-                - Set fixpoint mode
-                - Update run button to "changed"
-                - Force-start simulation with `self.impz_init(True)`
-                """
-
-                self.needs_calc = True      # force recalculation
-                self.needs_calc_fx = True   # force fx recalculation
-                self.error = False          # reset error flag
-
-                self.update_fx_ui_settings("fixpoint")  # set fixpoint mode
-                qstyle_widget(self.ui.but_run, "changed")
-                self.ui.but_run.setIcon(QIcon(":/play.svg"))
-                self.impz_init(True)
-                return
             # --------------- specs changed ------------
-            elif dict_sig['fx_sim'] == 'specs_changed':
+            if dict_sig['fx_sim'] == 'specs_changed':
                 """
                 Fixpoint widget specs have been updated.
                 - set `self.needs_calc_fx = True`.
                 If fixpoint mode is active:
                 - Reset error flag
                 - Force recalculation (`self.needs_calc = True`)
-                - Update run button style to "changed"
-                - If widget is visible, initialize fixpoint widget and
-                    start simulation via `self.impz_init()`
+                - Update run button style to 'changed'
+                - If widget is visible and autorun is selected,
+                    initialize fixpoint widget and
+                    start simulation via `calc_auto` -> `self.impz_init()`
                 """
                 self.needs_calc_fx = True   # fx sim needs recalculation
+                self.needs_calc = True  # force recalculation
+                self.error = False      # reset error flag
+                # set cmb box for fixpoint / float simulation and update ui:
+                self.toggle_fx_settings()
 
-                if fb.fil[0]['fx_sim']:     # fixpoint mode is active
-                    self.error = False      # reset error flag
-                    self.needs_calc = True  # force recalculation
-
-                    qstyle_widget(self.ui.but_run, "changed")
-                    self.ui.but_run.setIcon(QIcon(":/play.svg"))
-                    if self.isVisible():
-                        self.impz_init()
+                qstyle_widget(self.ui.but_run, 'changed')
+                self.ui.but_run.setIcon(QIcon(":/play.svg"))
+                if self.isVisible():
+                    self.calc_auto() # call impz_init() if autorun is selected
 
             # --------------- 'start_fx_response_calculation' ---------
             elif dict_sig['fx_sim'] == 'start_fx_response_calculation':
                 """
                 The fixpoint widget has been initialized and starts the fx simulation
                 when the widget is visible via `self.impz()` and the handle to the
                 fixpoint simulation method handle passed in `dict_sig['fxfilter_func']`
@@ -416,15 +394,15 @@
                 # update number of data points in impz_ui and FFT window
                 # needed when e.g. FIR filter order has been changed, requiring
                 # a different number of data points for simulation. Don't emit a signal.
                 self.ui.update_N(emit=False)
                 self.needs_calc = True
                 # Highlight "RUN" button
                 self.ui.but_run.setIcon(QIcon(":/play.svg"))
-                qstyle_widget(self.ui.but_run, "changed")
+                qstyle_widget(self.ui.but_run, 'changed')
                 self.impz_init()
 
             elif 'mpl_toolbar' in dict_sig:
                 if dict_sig['mpl_toolbar'] == 'ui_level':
                     self.set_ui_level(dict_sig['value'])
                 elif dict_sig['mpl_toolbar'] == 'home':
                     self.zoom_home()
@@ -440,28 +418,26 @@
                 else:
                     # treat all other local UI events here
                     self.needs_calc = True
                     # make file data available to stimulus widget:
                     self.file_io()
                     self.impz_init()
 
-            elif 'view_changed' in dict_sig:
-                if 'f_S' in dict_sig['view_changed']:
-                    self.emit({'view_changed': 'f_S', 'id': id(self)})
+            elif 'view_changed' in dict_sig or any(self.needs_redraw):
                 self.draw()  # redraw a.o. changed axes scaling
 
         else:  # invisible
             if 'data_changed' in dict_sig:
                 self.needs_calc = True
-            elif 'view_changed' in dict_sig:
+            elif 'view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S':
+                self.needs_redraw = [True] * 2
                 # update frequency related widgets (visible or not)
-                if dict_sig['view_changed'] == 'f_S':
-                    self.emit({'view_changed': 'f_S', 'id': id(self)})
             elif 'ui_local_changed' in dict_sig:
-                self.needs_redraw = [True] * 2
+                # self.needs_redraw = [True] * 2
+                self.needs_calc = True
 
     # ------------------------------------------------------------------------------
     def set_N_to_file_len(self):
         """
         Check status of file_io widget:
         - if no file is loaded, do nothing. This shouldn't happen (check to be sure ...)
         - else set N_end = len(file_data) in the UI
@@ -500,15 +476,16 @@
                 qget_cmb_box(self.stim_wdg.ui.cmb_file_io) != "use")
 
     # =========================================================================
     # Simulation: Calculate stimulus, response and draw them
     # =========================================================================
     def calc_auto(self, autorun=None):
         """
-        Triggered when checkbox "Autorun" is clicked.
+        Triggered when checkbox "Autorun" is clicked or specs have been edited,
+        requiring a recalculation.
 
         When Autorun has been pushed (`but_auto_run.isChecked() == True`) and
         calculation is required, automatically run `impz_init()`.
         """
         if self.ui.but_auto_run.isChecked() and self.needs_calc:
             self.impz_init()
 
@@ -544,15 +521,15 @@
             )
         self.ui.but_freq_norm_impz.setVisible(self.stim_wdg.ui.cmb_stim == "impulse")
 
         self.error = False
         self.needs_redraw = [True] * 2
 
         # check for fixpoint setting (fb.fil[0]['fx_sim']) and update UI if needed
-        self.update_fx_ui_settings()
+        self.toggle_fx_settings()
 
         if type(arg) == bool:
             self.needs_calc = True  # but_run has been pressed -> force run
         elif not self.ui.but_auto_run.isChecked():  # "Auto" is not active, return
             return
 
         if self.needs_calc:
@@ -610,17 +587,17 @@
                  # initialize array for quantized stimulus
                 self.x_q = np.empty_like(self.x, dtype=np.float64)
                 if np.any(np.iscomplex(x_test)):
                     logger.warning(
                         "Complex stimulus: Only its real part is used for the "
                         "fixpoint filter!")
                 # setup and initialize input quantizer
-                self.q_i = fx.Fixed(fb.fil[0]['fxqc']['QI'])
+                self.q_i = fx.Fixed(fb.fil[0]['fxq']['QI'])
                 # always use integer decimal format for input quantizer
-                self.q_i.set_qdict({'fx_base': 'dec'})
+                # self.q_i.set_qdict({'fx_base': 'dec'})
 
                 # initialize FX filter and get a handle for `fxfilter()` function
                 self.emit({'fx_sim': 'init'})
                 return  # process_sig_rx() directly calls impz() in next step
             else:
                 # Initialize filter memory with zeros, for either cascaded structure (sos)
                 # or direct form
@@ -654,30 +631,33 @@
             #             f"{int(np.ceil(self.ui.N_end / self.ui.N_frame))}")
             # The last frame could be shorter than self.ui.N_frame:
             L_frame = min(self.ui.N_frame, self.ui.N_end - self.N_first)
             # Define slicing expression for the current frame
             frame = slice(self.N_first, self.N_first + L_frame)
 
             # ------------------------------------------------------------------
-            # ---- calculate stimuli for current frame -------------------------
+            # ---- calculate stimuli for current frame inplace -----------------
             # ------------------------------------------------------------------
             # self.x[frame] = self.stim_wdg.calc_stimulus_frame(
             self.stim_wdg.calc_stimulus_frame(
                 self.x, N_first=self.N_first, N_frame=L_frame, N_end=self.ui.N_end)
 
             # ------------------------------------------------------------------
             # ---- calculate fixpoint or floating point response for current frame
             # ------------------------------------------------------------------
             if fb.fil[0]['fx_sim']:  # fixpoint filter
-                self.x_q[frame] = self.q_i.fixp(self.x[frame].real)  # quantize stimulus
+                # Quantize stimulus:
+                self.x_q[frame] = self.q_i.fixp(self.x[frame].real,
+                                                out_frmt=fb.fil[0]['qfrmt'])
                 # --------------------------------------------------------------
                 # ---- Get fixpoint response for current frame -----------------
                 # --------------------------------------------------------------
                 try:
                     self.y[frame] = np.asarray(self.fxfilter(self.x_q[frame]))
+                    # logger.warning(f"y_frame = {pprint_log(self.y[frame])}")
 
                 except ValueError as e:
                     if self.fxfilter(self.x_q[frame]) is None:
                         logger.error("Fixpoint simulation returned empty results!")
                     else:
                         logger.error("Simulator error {0}".format(e))
                         fb.fx_results = None
@@ -753,77 +733,82 @@
         qstyle_widget(self.ui.but_run, "normal")
         # update Tran_IO ui, depending on complex and fixpoint status
         self.file_io_wdg.ui.update_ui(cmplx=self.cmplx, fx=fb.fil[0]['fx_sim'])
 
         if fb.fil[0]['fx_sim']:
             self.emit({'fx_sim': 'finish'})
 
-# =============================================================================
-    def toggle_fx_setting(self):
-        """ Triggered by changing `self.ui.cmb_sim_select` """
-
-        fb.fil[0]['fx_sim'] = (qget_cmb_box(self.ui.cmb_sim_select) == "fixpoint")
-        self.update_fx_ui_settings()
-        self.impz_init()
-
     # --------------------------------------------------------------------------
-    def update_fx_ui_settings(self, fx=None):
+    def toggle_fx_settings(self, arg=None):
         """
-        Select between fixpoint and floating point simulation and update FX UI
-        settings.
-
-        Parameter `fx` can be:
+        `arg` can be the following arguments, triggered by:
 
-        - str "fixpoint", "float" or `None` when called directly. "fixpoint"
-          or "float" updates the combobox setting correspondingly. `None`
-          only upcates the UI.
-
-        - int 0 or 1 when triggered by changing the index of combobox
-          `self.ui.cmb_sim_select` (signal-slot-connection)
+            - arg `None`: from `__init__()`, `impz_init()` or `process_sig_rx()` when
+              {dict_sig['fx_sim'] == 'specs_changed'} was received. Read the state of
+              `fb.fil[0]['fx_sim']` and update combobox correspondingly
+            - arg int 0 or 1 from `self.ui.cmb_sim_select` when index was changed
+              (signal-slot-connection), update `fb.fil[0]['fx_sim']` correspondingly,
+              fire signal {'fx_sim': 'specs_changed'} and start simulation
+            - arg "fixpoint" or "float" from a direct call with (not used currently),
+              update ui and combobox `self.ui.cmb_sim_select` correspondingly
 
         When fixpoint simulation is selected, all corresponding widgets are made
         visible and `fb.fil[0]['fx_sim']` is set to True.
 
         If `fb.fil[0]['fx_sim']` has been changed since last time, `self.needs_calc`
-        is set to True and the run button is set to "changed".
+        is set to True and the run button is set to 'changed'.
         """
-        if fx in {"float", "fixpoint"}:
-            # Function call with argument: Set UI and fb.fil[0]['fx_sim'] accord. to `fx`
-            qset_cmb_box(self.ui.cmb_sim_select, fx, data=True)
-            fb.fil[0]['fx_sim'] = (fx == "fixpoint")
-        elif fb.fil[0]['fx_sim']:
-            qset_cmb_box(self.ui.cmb_sim_select, "fixpoint", data=True)
-        else:
-            qset_cmb_box(self.ui.cmb_sim_select, "float", data=True)
-
-        # plot styles for quantized stimulus signal
-        self.ui.cmb_plt_freq_stmq.setVisible(fb.fil[0]['fx_sim'])  # cmb box freq. domain
-        self.ui.lbl_plt_freq_stmq.setVisible(fb.fil[0]['fx_sim'])  # label freq. domain
-        self.ui.cmb_plt_time_stmq.setVisible(fb.fil[0]['fx_sim'])  # cmb box time domain
-        self.ui.lbl_plt_time_stmq.setVisible(fb.fil[0]['fx_sim'])  # cmb box time domain
-        self.ui.but_fx_scale.setVisible(fb.fil[0]['fx_sim'])  # fx scale int
-        self.ui.but_fx_range.setVisible(fb.fil[0]['fx_sim'])  # display fx range limits
+        # Function call with argument: Set UI and fb.fil[0]['fx_sim'] accord. to `arg`
+        # if arg in {"float", "fixpoint"}:
+        #     qset_cmb_box(self.ui.cmb_sim_select, arg, data=True)
+        #     fb.fil[0]['fx_sim'] = (arg == "fixpoint")
+
+        # Direct call with no argument, set combobox according to fb.fil[0]['fx_sim']
+        if arg is None:
+            if fb.fil[0]['fx_sim']:
+                qset_cmb_box(self.ui.cmb_sim_select, "fixpoint", data=True)
+            else:
+                qset_cmb_box(self.ui.cmb_sim_select, "float", data=True)
+        # Combobox modified, set fb.fil[0]['fx_sim'] according to combobox and start sim
+        elif type(arg) == int:
+            fb.fil[0]['fx_sim'] = (qget_cmb_box(self.ui.cmb_sim_select) == 'fixpoint')
+            self.emit({'fx_sim': 'specs_changed'})
+            self.needs_calc = True
+            self.calc_auto()  # run simulation if autostart has been selected
+        else:
+            logger.error(f"Unknown argument '{arg}'!")
+            return
+
+        fx_mode = fb.fil[0]['fx_sim']
+        # enable plot widgets for quantized stimulus signal
+        self.ui.cmb_plt_freq_stmq.setVisible(fx_mode)  # cmb box freq. domain
+        self.ui.lbl_plt_freq_stmq.setVisible(fx_mode)  # label freq. domain
+        self.ui.cmb_plt_time_stmq.setVisible(fx_mode)  # cmb box time domain
+        self.ui.lbl_plt_time_stmq.setVisible(fx_mode)  # cmb box time domain
+        self.ui.lbl_fx_range.setVisible(fx_mode)  # display fx range limits
+        self.ui.but_fx_range_x.setVisible(fx_mode)  # display fx range limits
+        self.ui.but_fx_range_y.setVisible(fx_mode)  # display fx range limits
 
         # add / delete fixpoint entry to / from spectrogram combo box and set
         # `fx_str = "fixpoint"`` or `""``
-        if fb.fil[0]['fx_sim']:
+        if fx_mode:
             qcmb_box_add_item(self.ui.cmb_plt_time_spgr, ["xqn", "x_q[n]", ""])
             self.fx_str = "fixpoint "
         else:
             qcmb_box_del_item(self.ui.cmb_plt_time_spgr, "x_q[n]")
             self.fx_str = ""
 
-        if fb.fil[0]['fx_sim'] != self.fx_sim_old:
+        if fx_mode != self.fx_mode_old:
             self.ui.but_run.setIcon(QIcon(":/play.svg"))
-            qstyle_widget(self.ui.but_run, "changed")
+            qstyle_widget(self.ui.but_run, 'changed')
             # force recalculation of stimulus and response when switching
             # between float and fixpoint
             self.needs_calc = True
 
-        self.fx_sim_old = fb.fil[0]['fx_sim']
+        self.fx_mode_old = fb.fil[0]['fx_sim']
 
     # ------------------------------------------------------------------------
     def calc_fft(self):
         """
         (Re-)calculate FFTs of stimulus `self.X`, quantized stimulus `self.X_q`
         and response `self.Y` using the window function from `self.ui.win_dict['win']`.
         """
@@ -884,37 +869,48 @@
         if type(arg) is not None:
             self.needs_redraw = [True] * 2
 
         if not hasattr(self, 'cmplx'):  # has response been calculated yet?
             logger.error("Response should have been calculated by now!")
             return
 
-        self.scale_i = self.scale_o = 1
-        self.fx_min = -1.
-        self.fx_max = 1.
+        self.scale_i = self.scale_iq = self.scale_o = 1
+        self.fx_min_x = self.fx_min_y = -1.
+        self.fx_max_x = self.fx_max_y = 1.
         if fb.fil[0]['fx_sim']:
             # fixpoint simulation enabled -> scale stimulus and response
             try:
-                if self.ui.but_fx_scale.isChecked():
-                    # display stimulus and response as integer values:
-                    # - multiply stimulus and response by 2 ** WF
-                    self.scale_i = 1 << fb.fil[0]['fxqc']['QI']['WF']
-                    self.scale_o = 1 << fb.fil[0]['fxqc']['QO']['WF']
-                    self.fx_min = - (1 << fb.fil[0]['fxqc']['QO']['W']-1)
-                    self.fx_max = -self.fx_min - 1
-                else:
+                if fb.fil[0]['qfrmt'] == 'qint':
+                    # display stimulus and response as integer values
+                    # in the range +/- 2 ** (WI + WF)
+                    self.scale_i = 1 << fb.fil[0]['fxq']['QI']['WF']
+                    self.scale_iq = 1
+                    self.scale_o = 1 << fb.fil[0]['fxq']['QO']['WF']
+
+                    self.fx_min_x = - (1 << (fb.fil[0]['fxq']['QI']['WI']
+                                     + fb.fil[0]['fxq']['QI']['WF']))
+                    self.fx_max_x = -self.fx_min_x - 1
+                    self.fx_min_y = - (1 << (fb.fil[0]['fxq']['QO']['WI']
+                                     + fb.fil[0]['fxq']['QO']['WF']))
+                    self.fx_max_y = -self.fx_min_y - 1
+                elif fb.fil[0]['qfrmt'] == 'qfrac':
                     # display values scaled as "real world (float) values"
-                    self.fx_min = -(1 << fb.fil[0]['fxqc']['QO']['WI'])
-                    self.fx_max = -self.fx_min - 1. / (1 << fb.fil[0]['fxqc']['QO']['WF'])
+                    self.scale_i = self.scale_iq = self.scale_o = 1
+                    self.fx_min_x = -(1 << fb.fil[0]['fxq']['QI']['WI'])
+                    self.fx_max_x = -self.fx_min_x\
+                        - 1. / (1 << fb.fil[0]['fxq']['QI']['WF'])
+                    self.fx_min_y = -(1 << fb.fil[0]['fxq']['QO']['WI'])
+                    self.fx_max_y = -self.fx_min_y -\
+                        1. / (1 << fb.fil[0]['fxq']['QO']['WF'])
 
             except AttributeError as e:
                 logger.error("Attribute error: {0}".format(e))
             except TypeError as e:
                 logger.error(
-                    "Type error: 'fxqc_dict'={0},\n{1}".format(fb.fil[0]['fxqc'], e))
+                    "Type error: 'fxqc_dict'={0},\n{1}".format(fb.fil[0]['fxq'], e))
             except ValueError as e:
                 logger.error("Value error: {0}".format(e))
 
         idx = self.tab_mpl_w.currentIndex()
 
         if idx == 0 and self.needs_redraw[0]\
                 and self.mplwidget_t.mplToolbar.plot_enabled:
@@ -1142,37 +1138,35 @@
             fmt_mkr_stmq = {'marker': ''}
 
         if "*" in qget_cmb_box(self.ui.cmb_plt_time_resp):
             fmt_mkr_resp = self.fmt_mkr_resp
         else:
             fmt_mkr_resp = {'marker': ''}
 
-        # fixpoint simulation enabled -> scale stimulus and response
+        # fixpoint simulation enabled -> assign frame to x_q
         if fb.fil[0]['fx_sim'] and hasattr(self, 'x_q'):
-            x_q = self.x_q[self.ui.N_start:N_end] * self.scale_i
+            x_q = self.x_q[self.ui.N_start:N_end]
             if self.ui.but_log_time.isChecked():
                 x_q = np.maximum(20 * np.log10(abs(x_q)), self.ui.bottom_t)
-
-            # logger.warning("self.scale I:{0} O:{1}".format(self.scale_i, self.scale_o))
         else:
             x_q = None
 
         # Create finer grid for plotting interpolated waveforms
         if self.ui.chk_plt_time_stim_interp.isChecked():
             I = 20
             # self.t_interp = np.linspace(self.t[0], self.t[-1], (len(self.t) - 1) * I + 1)
             # self.x_interp = np.interp(self.t_interp, self.t, self.x, left=None, right=None,
             #                      period=None)
             self.x_interp = sig.resample_poly(self.x, I, 1, axis=0, window=('kaiser', 5.0),
                                               padtype='line', cval=None)
             self.t_interp = np.linspace(self.n[0], self.n[-1] + 1, len(self.n) * I, endpoint=False) * fb.fil[0]['T_S']
 
         t = self.t[N_start:N_end]
-        x = self.x[N_start:N_end] * self.scale_i
-        y = self.y[N_start:N_end] * self.scale_o
+        x = self.x[N_start:N_end] * self.scale_i  # obtain same scaling for x as for quantized signals
+        y = self.y[N_start:N_end]
         win = self.ui.qfft_win_select.get_window(self.ui.N)
         if self.cmplx:
             x_r = x.real
             x_i = x.imag
             y_r = y.real
             y_i = y.imag
             lbl_x_r = "$x_r[n]$"
@@ -1200,29 +1194,34 @@
                 x_i = np.maximum(20 * np.log10(abs(x_i)), self.ui.bottom_t)
                 y_i = np.maximum(20 * np.log10(abs(y_i)), self.ui.bottom_t)
                 H_i_str = r'$|\Im\{$' + H_str + r'$\}|$' + ' in dBV'
                 H_str = r'$|\Re\{$' + H_str + r'$\}|$' + ' in dBV'
             else:
                 H_str = '$|$' + H_str + '$|$ in dBV'
 
-            fx_min = 20*np.log10(abs(self.fx_min))
-            fx_max = fx_min
+            fx_min_x = fx_max_x = 20*np.log10(abs(self.fx_min_x))
+            fx_min_y = fx_max_y = 20*np.log10(abs(self.fx_min_y))
         else:
             bottom_t = 0
-            fx_max = self.fx_max
-            fx_min = self.fx_min
+            fx_max_x = self.fx_max_x
+            fx_min_x = self.fx_min_x
+            fx_max_y = self.fx_max_y
+            fx_min_y = self.fx_min_y
             if self.cmplx:
                 H_i_str = r'$\Im\{$' + H_str + r'$\}$ in V'
                 H_str = r'$\Re\{$' + H_str + r'$\}$ in V'
             else:
                 H_str = H_str + ' in V'
 
-        if self.ui.but_fx_range.isChecked() and fb.fil[0]['fx_sim']:
-            self.ax_r.axhline(fx_max, 0, 1, color='k', linestyle='--')
-            self.ax_r.axhline(fx_min, 0, 1, color='k', linestyle='--')
+        if self.ui.but_fx_range_x.isChecked() and fb.fil[0]['fx_sim']:
+            self.ax_r.axhline(fx_max_x, 0, 1, color='k', linestyle='--')
+            self.ax_r.axhline(fx_min_x, 0, 1, color='k', linestyle='--')
+        if self.ui.but_fx_range_y.isChecked() and fb.fil[0]['fx_sim']:
+            self.ax_r.axhline(fx_max_y, 0, 1, color='k', linestyle='-.')
+            self.ax_r.axhline(fx_min_y, 0, 1, color='k', linestyle='-.')
 
         h_r = []  # plot handles (real part)
         h_i = []  # plot handles (imag. part)
         l_r = []  # labels (real part)
         l_i = []  # labels (imag. part)
 
         # --------------- Stimulus plot --------------------------------------
@@ -1569,14 +1568,18 @@
             if self.ui.but_Hf.isChecked():
                 H_F_str += r'$H_{id}$, '
             H_F_str = H_F_str.rstrip(', ') + ejO_str
 
             F_range = fb.fil[0]['freqSpecsRange']
 
             if fb.fil[0]['freq_specs_unit'] == 'k':
+                """
+                "'<i>k</i>' specifies frequencies w.r.t. " + to_html("f_S", frmt = 'i') +
+                " but plots graphs over the frequency index <i>k</i>.</span>",
+                """
                 # By default, k = params['N_FFT'] which is used for the calculation
                 # of the non-transient tabs and for F_id / H_id here.
                 # Here, the frequency axes must be scaled to fit the number of
                 # frequency points self.ui.N
                 F_range = [f * self.ui.N / fb.fil[0]['f_max'] for f in F_range]
                 f_max = self.ui.N
             else:
@@ -1607,34 +1610,35 @@
             else:
                 freq_resp = False
                 scale_impz = 1.
 
             # scale with window NENBW for correct power calculation
             P_scale = scale_impz / nenbw
             if plt_stimulus:
-                # scale display of frequency response
+                # scale display of stimulus: `self.x` is unscaled, hence X needs
+                # to be multiplied by self.scale_i
                 Px = np.sum(np.square(np.abs(self.X))) * P_scale
                 if fb.fil[0]['freqSpecsRangeType'] == 'half' and not freq_resp:
-                    X = calc_ssb_spectrum(self.X) * self.scale_i * scale_impz
+                    X = calc_ssb_spectrum(self.X) * scale_impz
                 else:
-                    X = self.X * self.scale_i * scale_impz
+                    X = self.X * scale_impz
 
             if plt_stimulus_q:
                 Pxq = np.sum(np.square(np.abs(self.X_q))) * P_scale
                 if fb.fil[0]['freqSpecsRangeType'] == 'half' and not freq_resp:
-                    X_q = calc_ssb_spectrum(self.X_q) * self.scale_i * scale_impz
+                    X_q = calc_ssb_spectrum(self.X_q) / self.scale_iq * scale_impz
                 else:
-                    X_q = self.X_q * self.scale_i * scale_impz
+                    X_q = self.X_q / self.scale_iq * scale_impz
 
             if plt_response:
                 Py = np.sum(np.square(np.abs(self.Y * self.scale_o))) * P_scale
                 if fb.fil[0]['freqSpecsRangeType'] == 'half' and not freq_resp:
-                    Y = calc_ssb_spectrum(self.Y) * self.scale_o * scale_impz
+                    Y = calc_ssb_spectrum(self.Y) / self.scale_o * scale_impz
                 else:
-                    Y = self.Y * self.scale_o * scale_impz
+                    Y = self.Y / self.scale_o * scale_impz
 
             # ----------------------------------------------------------------
             # Scale and shift frequency range
             # ----------------------------------------------------------------
             if fb.fil[0]['freqSpecsRangeType'] == 'sym':
                 # display -f_S/2 ... f_S/2 ->  shift X, Y and F using fftshift()
                 if plt_response:
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_impz_ui.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_impz_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         if 'id' in dict_sig and dict_sig['id'] == id(self):
             logger.warning("Stopped infinite loop:\n{0}".format(
                 pprint_log(dict_sig)))
             return
 
         # --- signals coming from the FFT window widget or the FFT window selector
         if dict_sig['class'] in {'Plot_FFT_win', 'QFFTWinSelector'}:
+            logger.error(f"FFT: pprint_log(dict_sig)")
             if 'closeEvent' in dict_sig:   # hide FFT window widget and return
                 self.hide_fft_wdg()
                 return
             else:
                 # check for value 'fft_win*':
                 if 'view_changed' in dict_sig and 'fft_win' in dict_sig['view_changed']:
                     # local connection to FFT window widget and qfft_win_select
@@ -166,15 +167,14 @@
             ("psd", "PSD",
              "<span>Power Spectral Density, either per bin or referred to "
              "<i>f<sub>S</sub></i></span>"),
             ("magnitude", "Mag.", "Signal magnitude"),
             ("angle", "Angle", "Phase, wrapped to &pm; &pi;"),
             ("phase", "Phase", "Phase (unwrapped)")
         ]
-#        self.N
 
         self.cmb_freq_display_items = [
             "<span>Select how to display the spectrum.</span>",
             ("mag", "Magnitude", "<span>Spectral magnitude</span>"),
             ("mag_phi", "Mag. / Phase", "<span>Magnitude and phase.</span>"),
             ("re_im", "Re. / Imag.", "<span>Real and imaginary part of spectrum.</span>")
         ]
@@ -184,17 +184,15 @@
         self.update_N(emit=False)  # also updates window function and win_dict
 #        self._update_noi()
 
     def _construct_UI(self):
         # ----------- ---------------------------------------------------
         # Run control widgets
         # ---------------------------------------------------------------
-        # self.but_auto_run = QPushButtonRT(text=to_html("Auto", frmt="b"), margin=0)
-        self.but_auto_run = QPushButton(" Auto", self)
-        self.but_auto_run.setObjectName("but_auto_run")
+        self.but_auto_run = QPushButton(" Auto", objectName="but_auto_run")
         self.but_auto_run.setToolTip("<span>Update response automatically when "
                                      "parameters have been changed.</span>")
         # self.but_auto_run.setMaximumWidth(qtext_width(text=" Auto "))
         self.but_auto_run.setCheckable(True)
         self.but_auto_run.setChecked(True)
 
         but_height = self.but_auto_run.sizeHint().height()
@@ -260,25 +258,23 @@
         self.but_fft_wdg.setIconSize(QSize(but_height, but_height))
         self.but_fft_wdg.setFixedSize(QSize(int(1.5 * but_height), but_height))
         self.but_fft_wdg.setToolTip('<span>Show / hide FFT widget (select window type '
                                     ' and display its properties).</span>')
         self.but_fft_wdg.setCheckable(True)
         self.but_fft_wdg.setChecked(False)
 
-        self.qfft_win_select = QFFTWinSelector(self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict, objectName='win_select_qfft')
 
-        self.but_fx_scale = PushButton(" FX:Int ")
-        self.but_fx_scale.setObjectName("but_fx_scale")
-        self.but_fx_scale.setToolTip(
-            "<span>Display data with integer (fixpoint) scale.</span>")
-
-        self.but_fx_range = PushButton(" FX:Range")
-        self.but_fx_range.setObjectName("but_fx_limits")
-        self.but_fx_range.setToolTip(
-            "<span>Display limits of fixpoint range.</span>")
+        self.lbl_fx_range = QLabel(to_html("FX Range:", frmt='b'))
+        self.but_fx_range_x = QCheckBox("X", objectName="but_fx_range_x")
+        self.but_fx_range_x.setToolTip(
+             "<span>Display stimulus fixpoint range (---).</span>")
+        self.but_fx_range_y = QCheckBox("Y", objectName="but_fx_range_y")
+        self.but_fx_range_y.setToolTip(
+             "<span>Display response fixpoint range (-.-).</span>")
 
         layH_ctrl_run = QHBoxLayout()
         layH_ctrl_run.addWidget(self.but_auto_run)
         layH_ctrl_run.addWidget(self.but_run)
         layH_ctrl_run.addWidget(self.cmb_sim_select)
         layH_ctrl_run.addWidget(self.prg_wdg)
         layH_ctrl_run.addSpacing(10)
@@ -291,50 +287,41 @@
         layH_ctrl_run.addWidget(self.frm_file_io)
         layH_ctrl_run.addSpacing(5)
         layH_ctrl_run.addWidget(self.lbl_stim_cmplx_warn)
         layH_ctrl_run.addSpacing(20)
         layH_ctrl_run.addWidget(self.but_fft_wdg)
         layH_ctrl_run.addWidget(self.qfft_win_select)
         layH_ctrl_run.addSpacing(20)
-        layH_ctrl_run.addWidget(self.but_fx_scale)
-        layH_ctrl_run.addWidget(self.but_fx_range)
+        layH_ctrl_run.addWidget(self.lbl_fx_range)
+        layH_ctrl_run.addWidget(self.but_fx_range_x)
+        layH_ctrl_run.addWidget(self.but_fx_range_y)
         layH_ctrl_run.addStretch(10)
 
         # layH_ctrl_run.setContentsMargins(*params['wdg_margins'])
 
         self.wdg_ctrl_run = QWidget(self)
         self.wdg_ctrl_run.setLayout(layH_ctrl_run)
         # --- end of run control ----------------------------------------
 
         # ----------- ---------------------------------------------------
         # Controls for time domain
         # ---------------------------------------------------------------
-        self.lbl_title_plot_time = QLabel("Plots:")
-        self.lbl_title_plot_time.setObjectName("large")
-
-        # setting up background color and border
-        # self.lbl_title_plot_time.setStyleSheet("font-size:14")
-        # self.lbl_title_plot_time.setFont(QFont('Arial', 10))
-        # self.lbl_title_plot_time.resize(200, 20)
-        # color_effect = QGraphicsColorizeEffect()
-        # color_effect.setColor(Qt.darkGreen)
-        # self.lbl_title_plot_time.setGraphicsEffect(color_effect)
+        self.lbl_title_plot_time = QLabel("Plots:", objectName="large")
 
         self.lbl_plt_time_stim = QLabel(to_html("Stim. x", frmt='bi'), self)
         self.cmb_plt_time_stim = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_stim, self.plot_styles_list, self.plt_time_stim)
         self.cmb_plt_time_stim.setToolTip(
             "<span>Plot style for stimulus.</span>")
 
         self.lbl_plt_time_stim_interp = QLabel(
             to_html("&nbsp;&nbsp;x(t)", frmt='bi'), self)
-        self.chk_plt_time_stim_interp = QCheckBox(self)
+        self.chk_plt_time_stim_interp = QCheckBox(self, objectName="chk_plt_time_stim_interp")
         self.chk_plt_time_stim_interp.setChecked(False)
-        self.chk_plt_time_stim_interp.setObjectName("chk_plt_time_stim_interp")
         self.chk_plt_time_stim_interp.setToolTip(
             '<span>Plot interpolated pseudo-analog stimulus "<i>x</i>(<i>t</i>)", '
             'valid up to approx. 0.4 <i>f<sub>S</sub></i>.</span>')
 
         self.lbl_plt_time_stmq = QLabel(to_html(
             "&nbsp;&nbsp;FX Stim. x_Q", frmt='bi'), self)
         self.cmb_plt_time_stmq = QComboBox(self)
@@ -357,39 +344,36 @@
         self.chk_win_time.setToolTip(
             '<span>Plot FFT windowing function.</span>')
         self.chk_win_time.setChecked(False)
 
         line1 = QVLine()
         line2 = QVLine(width=5)
 
-        self.but_log_time = PushButton(" dB")
-        self.but_log_time.setObjectName("but_log_time")
+        self.but_log_time = PushButton(" dB", objectName="but_log_time")
         self.but_log_time.setToolTip(
             "<span>Logarithmic scale for y-axis.</span>")
 
-        lbl_plt_time_spgr = QLabel(to_html("Spectrogram", frmt='bi'), self)
+        lbl_plt_time_spgr = QLabel(to_html("Spectrogram", frmt='bi'))
         self.cmb_plt_time_spgr = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_spgr, self.cmb_time_spgr_items, self.plt_time_spgr)
 
         self.cmb_mode_spgr_time = QComboBox(self)
         qcmb_box_populate(
             self.cmb_mode_spgr_time, self.cmb_mode_spgr_time_items, self.mode_spgr_time)
 
         self.lbl_byfs_spgr_time = QLabel(
             to_html("&nbsp;per f_S", frmt='b'), self)
-        self.chk_byfs_spgr_time = QCheckBox(self)
-        self.chk_byfs_spgr_time.setObjectName("chk_log_spgr")
+        self.chk_byfs_spgr_time = QCheckBox(self, objectName="chk_log_spgr")
         self.chk_byfs_spgr_time.setToolTip("<span>Display spectral density "
                                            "i.e. scale by f_S</span>")
         self.chk_byfs_spgr_time.setChecked(True)
 
-        self.but_log_spgr_time = QPushButton("dB")
+        self.but_log_spgr_time = QPushButton("dB", objectName="but_log_spgr")
         self.but_log_spgr_time.setMaximumWidth(qtext_width(text=" dB"))
-        self.but_log_spgr_time.setObjectName("but_log_spgr")
         self.but_log_spgr_time.setToolTip(
             "<span>Logarithmic scale for spectrogram.</span>")
         self.but_log_spgr_time.setCheckable(True)
         self.but_log_spgr_time.setChecked(True)
 
         self.lbl_time_nfft_spgr = QLabel(
             to_html("&nbsp;N_FFT =", frmt='bi'), self)
@@ -485,28 +469,26 @@
         layG_ctrl_time = QGridLayout()
         layG_ctrl_time.addWidget(self.wdg_ctrl_time_0, 0, 0, 2, 1)
         layG_ctrl_time.addWidget(self.wdg_ctrl_time_1, 0, 1)
         layG_ctrl_time.addWidget(self.wdg_ctrl_time_spgr, 1, 1)
         layG_ctrl_time.setContentsMargins(0, 0, 0, 0)
         layG_ctrl_time.setVerticalSpacing(0)
 
-        self.wdg_ctrl_time = QWidget(self)
+        self.wdg_ctrl_time = QWidget(self, objectName="transparent")
         self.wdg_ctrl_time.setLayout(layG_ctrl_time)
-        self.wdg_ctrl_time.setObjectName("transparent")
         self.wdg_ctrl_time.setContentsMargins(0, 0, 0, 0) # (*rc.params['wdg_margins'])
 
         self.wdg_ctrl_time_spgr.setVisible(self.plt_time_spgr != "none")
 
         # ---- end time domain ------------------
 
         # ---------------------------------------------------------------
         # Controls for frequency domain
         # ---------------------------------------------------------------
-        self.lbl_title_plot_freq = QLabel("Plots:")
-        self.lbl_title_plot_freq.setObjectName("large")
+        self.lbl_title_plot_freq = QLabel("Plots:", objectName="large")
         #
         self.lbl_plt_freq_stim = QLabel(to_html("Stim. X", frmt='bi'), self)
         self.cmb_plt_freq_stim = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_freq_stim, self.plot_styles_list, self.plt_freq_stim)
         self.cmb_plt_freq_stim.setToolTip(
             "<span>Plot style for stimulus.</span>")
@@ -523,17 +505,16 @@
             to_html("&nbsp;Resp. Y", frmt='bi'), self)
         self.cmb_plt_freq_resp = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_freq_resp, self.plot_styles_list, self.plt_freq_resp)
         self.cmb_plt_freq_resp.setToolTip(
             "<span>Plot style for response.</span>")
 
-        self.but_log_freq = QPushButton("dB")
+        self.but_log_freq = QPushButton("dB", objectName="but_log_freq")
         self.but_log_freq.setMaximumWidth(qtext_width(" dB"))
-        self.but_log_freq.setObjectName(".but_log_freq")
         self.but_log_freq.setToolTip(
             "<span>Logarithmic scale for y-axis.</span>")
         self.but_log_freq.setCheckable(True)
         self.but_log_freq.setChecked(True)
 
         self.lbl_log_bottom_freq = QLabel(to_html("min =", frmt='bi'), self)
         self.lbl_log_bottom_freq.setVisible(self.but_log_freq.isChecked())
@@ -543,18 +524,17 @@
         self.led_log_bottom_freq.setToolTip(
             "<span>Minimum display value for log. scale.</span>")
         self.led_log_bottom_freq.setVisible(self.but_log_freq.isChecked())
 
         if not self.but_log_freq.isChecked():
             self.bottom_f = 0
 
-        self.cmb_freq_display = QComboBox(self)
+        self.cmb_freq_display = QComboBox(self, objectName="cmb_re_im_freq")
         qcmb_box_populate(self.cmb_freq_display, self.cmb_freq_display_items,
                           self.cmb_freq_display_item)
-        self.cmb_freq_display.setObjectName("cmb_re_im_freq")
 
         self.but_Hf = QPushButtonRT(self, to_html("H_id", frmt="bi"), margin=5)
         self.but_Hf.setObjectName("chk_Hf")
         self.but_Hf.setToolTip("<span>Show ideal frequency response, calculated "
                                "from the filter coefficients.</span>")
         self.but_Hf.setChecked(False)
         self.but_Hf.setCheckable(True)
@@ -566,17 +546,16 @@
             "to an energy <i>E<sub>X</sub></i> = 1. For a dirac pulse, this yields "
             "|<i>Y(f)</i>| = |<i>H(f)</i>|. DC, Noise and file I/O need to be "
             "turned off, window should be <b>Rectangular</b>.</span>")
         self.but_freq_norm_impz.setCheckable(True)
         self.but_freq_norm_impz.setChecked(True)
         self.but_freq_norm_impz.setObjectName("freq_norm_impz")
 
-        self.but_freq_show_info = QPushButton("Info", self)
+        self.but_freq_show_info = QPushButton("Info", objectName="but_show_info_freq")
         self.but_freq_show_info.setMaximumWidth(qtext_width(" Info "))
-        self.but_freq_show_info.setObjectName("but_show_info_freq")
         self.but_freq_show_info.setToolTip(
             "<span>Show signal power in legend.</span>")
         self.but_freq_show_info.setCheckable(True)
         self.but_freq_show_info.setChecked(False)
 
         layH_ctrl_freq_0 = QHBoxLayout()
         layH_ctrl_freq_0.addWidget(self.lbl_title_plot_freq)
@@ -616,17 +595,16 @@
         self.wdg_ctrl_freq_1.setContentsMargins(0, 0, 0, 0)
         layG_ctrl_freq = QGridLayout()
         layG_ctrl_freq.addWidget(self.wdg_ctrl_freq_0, 0, 0)
         layG_ctrl_freq.addWidget(self.wdg_ctrl_freq_1, 0, 1)
         layG_ctrl_freq.setContentsMargins(0, 0, 0, 0)
         layG_ctrl_freq.setVerticalSpacing(0)
 
-        self.wdg_ctrl_freq = QWidget(self)
+        self.wdg_ctrl_freq = QWidget(self, objectName="transparent")
         self.wdg_ctrl_freq.setLayout(layG_ctrl_freq)
-        self.wdg_ctrl_freq.setObjectName("transparent")
         self.wdg_ctrl_freq.setContentsMargins(0, 0, 0, 0)  # (*rc.params['wdg_margins'])
         # ---- end Frequency Domain ------------------
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         # connect FFT widget to qfft_selector and vice versa and to and signals upstream:
@@ -752,16 +730,16 @@
         settling time.
         """
         if N_user == 0:  # set number of data points automatically
             if fb.fil[0]['ft'] == 'IIR':
                 # IIR: No algorithm yet, set N = 100
                 N = 100
             else:
-                # FIR: N = number of coefficients (max. 100)
-                N = min(len(fb.fil[0]['ba'][0]), 100)
+                # FIR: N = number of coefficients (min. 25, max. 100)
+                N = max(min(len(fb.fil[0]['ba'][0]), 100), 25)
         else:
             N = N_user
 
         return N
 
 
 # ------------------------------------------------------------------------------
@@ -771,15 +749,15 @@
 
     app = QApplication(sys.argv)
 
     mainw = PlotImpz_UI(None)
     layVMain = QVBoxLayout()
     layVMain.addWidget(mainw.wdg_ctrl_time)
     layVMain.addWidget(mainw.wdg_ctrl_freq)
-    layVMain.addWidget(mainw.wdg_ctrl_stim)
+    # layVMain.addWidget(mainw.wdg_ctrl_stim)
     layVMain.addWidget(mainw.wdg_ctrl_run)
     # (left, top, right, bottom)
     layVMain.setContentsMargins(*params['wdg_margins'])
 
     mainw.setLayout(layVMain)
 
     app.setActiveWindow(mainw)
@@ -796,13 +774,13 @@
     app = QApplication(sys.argv)
     app.setStyleSheet(rc.qss_rc)
     mainw = PlotImpz_UI()
 
     layVMain = QVBoxLayout()
     layVMain.addWidget(mainw.wdg_ctrl_time)
     layVMain.addWidget(mainw.wdg_ctrl_freq)
-    layVMain.addWidget(mainw.wdg_ctrl_stim)
+    # layVMain.addWidget(mainw.wdg_ctrl_stim)
     layVMain.addWidget(mainw.wdg_ctrl_run)
     mainw.setLayout(layVMain)
     app.setActiveWindow(mainw)
     mainw.show()
     sys.exit(app.exec_())
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_phi.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_phi.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,20 +75,19 @@
     def _construct_UI(self):
         """
         Intitialize the widget, consisting of:
         - Matplotlib widget with NavigationToolbar
         - Frame with control elements
         """
 
-        self.cmbUnitsPhi = QComboBox(self)
+        self.cmbUnitsPhi = QComboBox(self, objectName="cmbUnitsA")
         units = ["rad", "rad/pi",  "deg"]
         scales = [1.,   1. / np.pi, 180./np.pi]
         for unit, scale in zip(units, scales):
             self.cmbUnitsPhi.addItem(unit, scale)
-        self.cmbUnitsPhi.setObjectName("cmbUnitsA")
         self.cmbUnitsPhi.setToolTip("Set unit for phase.")
         self.cmbUnitsPhi.setCurrentIndex(0)
         self.cmbUnitsPhi.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.but_wrap = PushButton("wrapped ", checked=False)
         self.but_wrap.setToolTip("Plot phase wrapped to +/- pi")
 
@@ -98,16 +97,15 @@
         layHControls.addStretch(10)
 
         # ----------------------------------------------------------------------
         #               ### frmControls ###
         #
         # This widget encompasses all control subwidgets
         # ----------------------------------------------------------------------
-        self.frmControls = QFrame(self)
-        self.frmControls.setObjectName("frmControls")
+        self.frmControls = QFrame(self, objectName="frmControls")
         self.frmControls.setLayout(layHControls)
 
         # ----------------------------------------------------------------------
         #               ### mplwidget ###
         #
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_pz.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_pz.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 #
 # This file is part of the pyFDA project hosted at https://github.com/chipmuenk/pyfda
 #
 # Copyright © pyFDA Project Contributors
 # Licensed under the terms of the MIT License
 # (see file LICENSE in root directory for details)
 
+# TODO: Make P/Z draggable -> Bercher, Journey in Signal Processing with Jupyter, 2018.
+# TODO: Highlight P/Z selected in P/Z editor
+
 """
 Widget for plotting poles and zeros
 """
 from pyfda.libs.compat import (
     QWidget, QLabel, QFrame, QDial, QHBoxLayout, pyqtSignal, QComboBox, QLineEdit)
 import numpy as np
 import scipy.signal as sig
@@ -100,41 +103,38 @@
         - Frame with control elements
         """
         self.lbl_overlay = QLabel(to_html("Overlay:", frmt='bi'), self)
         self.cmb_overlay = QComboBox(self)
         qcmb_box_populate(
             self.cmb_overlay, self.cmb_overlay_items, self.cmb_overlay_default)
 
-        self.but_log = PushButton(" Log.", checked=True)
-        self.but_log.setObjectName("but_log")
+        self.but_log = PushButton(" Log.", checked=True, objectName="but_log")
         self.but_log.setToolTip("<span>Log. scale for overlays.</span>")
 
         self.diaRad_Hf = QDial(self)
         self.diaRad_Hf.setRange(2, 10)
         self.diaRad_Hf.setValue(2)
         self.diaRad_Hf.setTracking(False)  # produce less events when turning
         self.diaRad_Hf.setFixedHeight(30)
         self.diaRad_Hf.setFixedWidth(30)
         self.diaRad_Hf.setWrapping(False)
         self.diaRad_Hf.setToolTip("<span>Set max. radius for |H(f)| plot.</span>")
 
         self.lblRad_Hf = QLabel("Radius", self)
 
         self.lblBottom = QLabel(to_html("Bottom =", frmt='bi'), self)
-        self.ledBottom = QLineEdit(self)
-        self.ledBottom.setObjectName("ledBottom")
+        self.ledBottom = QLineEdit(self, objectName="ledBottom")
         self.ledBottom.setText(str(self.zmin))
         self.ledBottom.setMaximumWidth(qtext_width(N_x=8))
         self.ledBottom.setToolTip("Minimum display value.")
         self.lblBottomdB = QLabel("dB", self)
         self.lblBottomdB.setVisible(self.but_log.isChecked())
 
         self.lblTop = QLabel(to_html("Top =", frmt='bi'), self)
-        self.ledTop = QLineEdit(self)
-        self.ledTop.setObjectName("ledTop")
+        self.ledTop = QLineEdit(self, objectName="ledTop")
         self.ledTop.setText(str(self.zmax))
         self.ledTop.setToolTip("Maximum display value.")
         self.ledTop.setMaximumWidth(qtext_width(N_x=8))
         self.lblTopdB = QLabel("dB", self)
         self.lblTopdB.setVisible(self.but_log.isChecked())
 
         self.but_fir_poles = PushButton(" FIR Poles ", checked=True)
@@ -156,16 +156,15 @@
         layHControls.addWidget(self.but_fir_poles)
 
         # ----------------------------------------------------------------------
         #               ### frmControls ###
         #
         # This widget encompasses all control subwidgets
         # ----------------------------------------------------------------------
-        self.frmControls = QFrame(self)
-        self.frmControls.setObjectName("frmControls")
+        self.frmControls = QFrame(self, objectName="frmControls")
         self.frmControls.setLayout(layHControls)
 
         # ----------------------------------------------------------------------
         #               ### mplwidget ###
         #
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_tab_widgets.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_tab_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 
     # incoming, connected to input_tab_widget.sig_tx in pyfdax
     sig_rx = pyqtSignal(object)
     # outgoing: emitted by process_sig_rx
     sig_tx = pyqtSignal(object)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, objectName="plot_tab_widgets_inst"):
         super(PlotTabWidgets, self).__init__(parent)
+        self.setObjectName(objectName)
         self._construct_UI()
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Initialize UI with tabbed subwidgets: Instantiate dynamically each widget
         from the dict `fb.plot_classes` and try to
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/plot_tau_g.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/plot_tau_g.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,15 @@
         layHControls = QHBoxLayout()
         layHControls.addStretch(10)
         layHControls.addWidget(self.chkWarnings)
         # layHControls.addWidget(self.chkScipy)
         layHControls.addWidget(self.cmbAlgorithm)
 
         # This widget encompasses all control subwidgets:
-        self.frmControls = QFrame(self)
-        self.frmControls.setObjectName("frmControls")
+        self.frmControls = QFrame(self, objectName="frmControls")
         self.frmControls.setLayout(layHControls)
 
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['mpl_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_tau_g.html"
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/tran/plot_tran_stim.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/tran/plot_tran_stim.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     """
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing, e.g. when stimulus has been calculated
     from pyfda.libs.pyfda_qt_lib import emit
 
     def __init__(self):
         super().__init__()
-        self.ui = Plot_Tran_Stim_UI()  # create the UI part with buttons etc.
+        # create the UI part with buttons etc.
+        self.ui = Plot_Tran_Stim_UI(objectName='plot_tran_stim_ui_inst')
 
         # initial settings
         self.needs_calc = True   # flag whether plots need to be recalculated
         self.needs_redraw = [True] * 2  # flag which plot needs to be redrawn
         self.error = False
         self.x_file = None  # data mapped from file io in Plot_Impz.file_io()
 
@@ -252,15 +253,15 @@
             self.rad_phi2 = self.ui.phi2 / 180 * pi
         # -------------------------------------------------------------------
         # Initialization for current frame
         # -------------------------------------------------------------------
         N_last = N_first + N_frame  # calculate last element index
         frm_slc = slice(N_first, N_last)  # current slice
         n = np.arange(N_first, N_last)  #  create frame index vector
-        t = n / fb.fil[0]['f_S']  # create time vector
+        t = n * fb.fil[0]['T_S']  # create time vector
         noi = 0  # fallback when no noise is selected
         # ====================================================================
 
         # #####################################################################
         #
         # calculate stimuli x[n]
         #
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/tran/plot_tran_stim_ui.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/tran/plot_tran_stim_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,25 @@
                 pprint_log(dict_sig)))
             return
         elif 'view_changed' in dict_sig:
             if dict_sig['view_changed'] == 'f_S':
                 self.normalize_freqs()
 
 # ------------------------------------------------------------------------------
-    def __init__(self):
+    def __init__(self, objectName='plot_tran_stim_ui_inst'):
         super().__init__()
 
         """
         Intitialize the widget, consisting of:
         - top chkbox row
         - coefficient table
         - two bottom rows with action buttons
         """
         # initial settings
+        self.setObjectName(objectName)
         self.N_FFT = 0  # TODO: FFT value needs to be passed here somehow?
 
         # stimuli
         self.cmb_stim_item = "impulse"
         self.cmb_stim_periodic_item = "rect_per"
         self.cmb_stim_modulation_item = "am"
         self.stim = "dirac"
@@ -84,15 +85,15 @@
 
         self.f1 = 0.02
         self.f2 = 0.03
         self.A1 = 1.0
         self.A2 = 0.0
         self.phi1 = self.phi2 = 0
         self.T1 = self.T2 = 0
-        self.TW1 = self.TW2 = 1
+        self.TW1 = self.TW2 = 10
         self.BW1 = self.BW2 = 0.5
         self.N1 = self.N2 = 5
         self.noi = 0.1
         self.noise = "none"
         self.mls_b = 8
         self.DC = 0.0
         self.stim_formula = "A1 * abs(sin(2 * pi * f1 * n))"
@@ -236,37 +237,34 @@
         self._update_noi()
 
     def _construct_UI(self):
         # =====================================================================
         # Controls for stimuli
         # =====================================================================
 
-        self.lbl_title_stim = QLabel("Stim:")
-        self.lbl_title_stim.setObjectName("large")
+        self.lbl_title_stim = QLabel("Stim:", objectName="large")
         #
         self.cmbStimulus = QComboBox(self)
         qcmb_box_populate(self.cmbStimulus,
                           self.cmb_stim_items, self.cmb_stim_item)
 
         self.lblStimPar1 = QLabel(to_html("&alpha; =", frmt='b'), self)
-        self.ledStimPar1 = QLineEdit(self)
+        self.ledStimPar1 = QLineEdit(self, objectName="ledStimPar1")
         self.ledStimPar1.setText("0.5")
         self.ledStimPar1.setToolTip("Duty Cycle, 0 ... 1")
-        self.ledStimPar1.setObjectName("ledStimPar1")
 
-        self.but_stim_bl = QPushButton(self)
+        self.but_stim_bl = QPushButton(self, objectName="stim_bl")
         self.but_stim_bl.setText("BL")
         self.but_stim_bl.setToolTip(
             "<span>Bandlimit the signal to the Nyquist "
             "frequency to avoid aliasing. However, this is much slower "
             "to calculate especially for a large number of points.</span>")
         self.but_stim_bl.setMaximumWidth(qtext_width(text="BL "))
         self.but_stim_bl.setCheckable(True)
         self.but_stim_bl.setChecked(True)
-        self.but_stim_bl.setObjectName("stim_bl")
 
         # -------------------------------------
         self.cmbChirpType = QComboBox(self)
         qcmb_box_populate(self.cmbChirpType,
                           self.cmb_stim_chirp_items, self.chirp_type)
 
         self.cmbImpulseType = QComboBox(self)
@@ -283,28 +281,26 @@
 
         self.cmbModulationType = QComboBox(self)
         qcmb_box_populate(
             self.cmbModulationType, self.cmb_stim_modulation_items,
             self.cmb_stim_modulation_item)
 
         # -------------------------------------
-        self.chk_step_err = QPushButton("Error", self)
+        self.chk_step_err = QPushButton("Error", objectName="stim_step_err")
         self.chk_step_err.setToolTip(
             "<span>Display the step response error.</span>")
         self.chk_step_err.setMaximumWidth(qtext_width(text="Error "))
         self.chk_step_err.setCheckable(True)
         self.chk_step_err.setChecked(False)
-        self.chk_step_err.setObjectName("stim_step_err")
         #
         self.but_file_io = PushButton("<", checkable=False)
         self.but_file_io.setToolTip(
             "<span>Use file length as number of data points.</span>")
         self.lbl_file_io = QLabel(to_html("&nbsp;File IO", frmt='bi'))
-        self.cmb_file_io = QComboBox(self)
-        self.cmb_file_io.setObjectName("cmb_file_io")
+        self.cmb_file_io = QComboBox(self, objectName="cmb_file_io")
         qcmb_box_populate(
             self.cmb_file_io, self.cmb_file_io_items, self.cmb_file_io_default)
 
         # TODO: layH_file_io is instantiated in plot_impz, this is very hacky
         self.layH_file_io = QHBoxLayout()
         self.layH_file_io.addWidget(self.but_file_io)
         self.layH_file_io.addWidget(self.lbl_file_io)
@@ -321,157 +317,142 @@
         layHCmbStim.addWidget(self.cmbModulationType)
         layHCmbStim.addWidget(self.but_stim_bl)
         layHCmbStim.addWidget(self.lblStimPar1)
         layHCmbStim.addWidget(self.ledStimPar1)
         layHCmbStim.addWidget(self.chk_step_err)
 
         self.lblDC = QLabel(to_html("DC =", frmt='bi'), self)
-        self.ledDC = QLineEdit(self)
+        self.ledDC = QLineEdit(self, objectName="stimDC")
         self.ledDC.setText(str(self.DC))
         self.ledDC.setToolTip("DC Level")
-        self.ledDC.setObjectName("stimDC")
 
         layHStimDC = QHBoxLayout()
         layHStimDC.addWidget(self.lblDC)
         layHStimDC.addWidget(self.ledDC)
 
         # ======================================================================
         self.lblAmp1 = QLabel(to_html("&nbsp;A_1", frmt='bi') + " =", self)
-        self.ledAmp1 = QLineEdit(self)
+        self.ledAmp1 = QLineEdit(self, objectName="stimAmp1")
         self.ledAmp1.setText(str(self.A1))
         self.ledAmp1.setToolTip(
-            "Stimulus amplitude, complex values like 3j - 1 are allowed")
-        self.ledAmp1.setObjectName("stimAmp1")
+            "Stimulus amplitude; complex values like 3j - 1 are allowed")
 
         self.lblAmp2 = QLabel(to_html("&nbsp;A_2", frmt='bi') + " =", self)
-        self.ledAmp2 = QLineEdit(self)
+        self.ledAmp2 = QLineEdit(self, objectName="stimAmp2")
         self.ledAmp2.setText(str(self.A2))
         self.ledAmp2.setToolTip(
-            "Stimulus amplitude 2, complex values like 3j - 1 are allowed")
-        self.ledAmp2.setObjectName("stimAmp2")
+            "Stimulus amplitude 2; complex values like 3j - 1 are allowed")
         # ----------------------------------------------
         self.lblPhi1 = QLabel(to_html("&nbsp;&phi;_1", frmt='bi') + " =", self)
-        self.ledPhi1 = QLineEdit(self)
+        self.ledPhi1 = QLineEdit(self, objectName="stimPhi1")
         self.ledPhi1.setText(str(self.phi1))
         self.ledPhi1.setToolTip("Stimulus phase 1 in degrees")
-        self.ledPhi1.setObjectName("stimPhi1")
         self.lblPhU1 = QLabel(to_html("&deg;", frmt='i'), self)
 
         self.lblPhi2 = QLabel(to_html("&nbsp;&phi;_2", frmt='bi') + " =", self)
-        self.ledPhi2 = QLineEdit(self)
+        self.ledPhi2 = QLineEdit(self, objectName="stimPhi2")
         self.ledPhi2.setText(str(self.phi2))
         self.ledPhi2.setToolTip("Stimulus phase 2 in degrees")
-        self.ledPhi2.setObjectName("stimPhi2")
         self.lblPhU2 = QLabel(to_html("&deg;", frmt='i'), self)
         # ----------------------------------------------
         self.lbl_T1 = QLabel(to_html("&nbsp;T_1", frmt='bi') + " =", self)
-        self.led_T1 = QLineEdit(self)
+        self.led_T1 = QLineEdit(self, objectName="led_T1")
         self.led_T1.setText(str(self.T1))
         self.led_T1.setToolTip("Time shift 1")
-        self.led_T1.setObjectName("led_T1")
         self.lbl_TU1 = QLabel(to_html("T_S", frmt='i'), self)
 
         self.lbl_T2 = QLabel(to_html("&nbsp;T_2", frmt='bi') + " =", self)
-        self.led_T2 = QLineEdit(self)
+        self.led_T2 = QLineEdit(self, objectName="led_T2")
         self.led_T2.setText(str(self.T2))
         self.led_T2.setToolTip("Time shift 2")
-        self.led_T2.setObjectName("led_T2")
         self.lbl_TU2 = QLabel(to_html("T_S", frmt='i'), self)
 
         # ----------------------------------------------
         self.lbl_N1 = QLabel(to_html("&nbsp;N_1", frmt='bi') + " =", self)
-        self.led_N1 = QLineEdit(self)
+        self.led_N1 = QLineEdit(self, objectName="stimN1")
         self.led_N1.setText(str(self.N1))
         self.led_N1.setToolTip("Parameter N1")
-        self.led_N1.setObjectName("stimN1")
 
         self.lbl_N2 = QLabel(to_html("&nbsp;N_2", frmt='bi') + " =", self)
-        self.led_N2 = QLineEdit(self)
+        self.led_N2 = QLineEdit(self, objectName="stimN2")
         self.led_N2.setText(str(self.N2))
         self.led_N2.setToolTip("Parameter N2")
-        self.led_N2.setObjectName("stimN2")
         # ---------------------------------------------
         self.lbl_TW1 = QLabel(
             to_html("&nbsp;&Delta;T_1", frmt='bi') + " =", self)
-        self.led_TW1 = QLineEdit(self)
+        self.led_TW1 = QLineEdit(self, objectName="led_TW1")
         self.led_TW1.setText(str(self.TW1))
         self.led_TW1.setToolTip("Time width")
-        self.led_TW1.setObjectName("led_TW1")
         self.lbl_TWU1 = QLabel(to_html("T_S", frmt='i'), self)
 
         self.lbl_TW2 = QLabel(
             to_html("&nbsp;&Delta;T_2", frmt='bi') + " =", self)
-        self.led_TW2 = QLineEdit(self)
+        self.led_TW2 = QLineEdit(self, objectName="led_TW2")
         self.led_TW2.setText(str(self.TW2))
         self.led_TW2.setToolTip("Time width 2")
-        self.led_TW2.setObjectName("led_TW2")
         self.lbl_TWU2 = QLabel(to_html("T_S", frmt='i'), self)
         # ----------------------------------------------
         self.txtFreq1_f = to_html("&nbsp;f_1", frmt='bi') + " ="
+        self.txtFreq1_F = to_html("&nbsp;F_1", frmt='bi') + " ="
         self.txtFreq1_k = to_html("&nbsp;k_1", frmt='bi') + " ="
         self.lblFreq1 = QLabel(self.txtFreq1_f, self)
-        self.led_f1 = QLineEdit(self)
+        self.led_f1 = QLineEdit(self, objectName="led_f1")
         self.led_f1.setText(str(self.f1))
         self.led_f1.setToolTip("Stimulus frequency")
-        self.led_f1.setObjectName("led_f1")
         self.lblFreqUnit1 = QLabel(to_html("f_S", frmt='i'), self)
 
         self.txtFreq2_f = to_html("&nbsp;f_2", frmt='bi') + " ="
+        self.txtFreq2_F = to_html("&nbsp;F_2", frmt='bi') + " ="
         self.txtFreq2_k = to_html("&nbsp;k_2", frmt='bi') + " ="
         self.lblFreq2 = QLabel(self.txtFreq2_f, self)
-        self.led_f2 = QLineEdit(self)
+        self.led_f2 = QLineEdit(self, objectName="led_f2")
         self.led_f2.setText(str(self.f2))
         self.led_f2.setToolTip("Stimulus frequency 2")
-        self.led_f2.setObjectName("led_f2")
         self.lblFreqUnit2 = QLabel(to_html("f_S", frmt='i'), self)
         # ----------------------------------------------
         self.lbl_BW1 = QLabel(
             to_html(self.tr("&nbsp;BW_1"), frmt='bi') + " =", self)
-        self.led_BW1 = QLineEdit(self)
+        self.led_BW1 = QLineEdit(self, objectName="stimBW1")
         self.led_BW1.setText(str(self.BW1))
         self.led_BW1.setToolTip(self.tr("Relative bandwidth"))
-        self.led_BW1.setObjectName("stimBW1")
 
         self.lbl_BW2 = QLabel(
             to_html(self.tr("&nbsp;BW_2"), frmt='bi') + " =", self)
-        self.led_BW2 = QLineEdit(self)
+        self.led_BW2 = QLineEdit(self, objectName="stimBW2")
         self.led_BW2.setText(str(self.BW2))
         self.led_BW2.setToolTip(self.tr("Relative bandwidth 2"))
-        self.led_BW2.setObjectName("stimBW2")
         # ----------------------------------------------
         self.lblNoise = QLabel(to_html("&nbsp;Noise", frmt='bi'), self)
         self.cmb_stim_noise = QComboBox(self)
         qcmb_box_populate(self.cmb_stim_noise, self.cmb_stim_noise_items, self.noise)
 
         line2 = QVLine()
         self.lblNoi = QLabel("not initialized", self)
-        self.ledNoi = QLineEdit(self)
+        self.ledNoi = QLineEdit(self, objectName="stimNoi")
         self.ledNoi.setMaximumWidth(self.cmb_stim_noise.width())
         self.ledNoi.setText(str(self.noi))
         self.ledNoi.setToolTip("not initialized")
-        self.ledNoi.setObjectName("stimNoi")
         self.lblNoi_par = QLabel("not initialized", self)
         self.ledNoi_par = QLineEdit(self)
         self.ledNoi_par.setMaximumWidth(qtext_width(N_x=4))
         layH_noi_params = QHBoxLayout()
         layH_noi_params.addWidget(self.ledNoi)
         layH_noi_params.addWidget(self.lblNoi_par)
         layH_noi_params.addWidget(self.ledNoi_par)
 
         # ----------------------------------------------
         # Widget and Layout containing formula editor
         self.lblStimFormula = QLabel(to_html("x =", frmt='bi'), self)
-        self.ledStimFormula = QLineEdit(self)
+        self.ledStimFormula = QLineEdit(self, objectName="stimFormula")
         self.ledStimFormula.setText(str(self.stim_formula))
         self.ledStimFormula.setToolTip(
             "<span>Enter formula for stimulus in numexpr syntax, using the index "
             "<i>n</i> or the time vector <i>t</i> and the following UI settings: "
             + to_html("A_1, A_2, phi_1, phi_2, f_1, f_2, T_1, T_2, BW_1, BW_2",
                       frmt='i') + ".</span>")
-        self.ledStimFormula.setObjectName("stimFormula")
 
         layH_formula_stim = QHBoxLayout()
         layH_formula_stim.addWidget(self.lblStimFormula)
         layH_formula_stim.addWidget(self.ledStimFormula)
         layH_formula_stim.setContentsMargins(0, 0, 0, 0)
         self.wdg_formula_stim = QWidget(self)
         self.wdg_formula_stim.setLayout(layH_formula_stim)
@@ -566,16 +547,15 @@
         self.wdg_ctrl_stim.setLayout(layG_ctrl_stim)
 
         layH_stim = QHBoxLayout()
         layH_stim.addWidget(self.wdg_title_stim)
         layH_stim.addWidget(self.wdg_ctrl_stim)
         layH_stim.setContentsMargins(0, 0, 0, 0)
 
-        self.wdg_stim = QWidget(self)
-        self.wdg_stim.setObjectName("transparent")
+        self.wdg_stim = QWidget(self, objectName="transparent")
         self.wdg_stim.setLayout(layH_stim)
         self.wdg_stim.setContentsMargins(0, 0, 0, 0)
 
         # ----------------------------------------------------------------------
         # Initialization
         # ----------------------------------------------------------------------
         self.normalize_freqs()  # set f_scale and t_scale factors
@@ -641,21 +621,24 @@
             f_unit = ''
             t_unit = ''
             self.lblFreq1.setText(self.txtFreq1_k)
             self.lblFreq2.setText(self.txtFreq2_k)
         else:
             f_unit = fb.fil[0]['plt_fUnit']
             t_unit = fb.fil[0]['plt_tUnit'].replace(r"$\mu$", "&mu;")
-            self.lblFreq1.setText(self.txtFreq1_f)
-            self.lblFreq2.setText(self.txtFreq2_f)
-
-        if f_unit in {"f_S", "f_Ny"}:
-            unit_frmt = "i"  # italic
-        else:
-            unit_frmt = None  # don't print units like kHz in italic
+            if fb.fil[0]['freq_specs_unit'] in {'f_S', 'f_Ny'}:
+                # Normalized frequency labels with capital F
+                self.lblFreq1.setText(self.txtFreq1_F)
+                self.lblFreq2.setText(self.txtFreq2_F)
+                unit_frmt = "i"  # print 'f_S' and 'f_Ny' in italic
+            else:
+                # absolute frequencies with lower case f
+                self.lblFreq1.setText(self.txtFreq1_f)
+                self.lblFreq2.setText(self.txtFreq2_f)
+                unit_frmt = None  # don't print units like kHz in italic
 
         self.lblFreqUnit1.setText(to_html(f_unit, frmt=unit_frmt))
         self.lblFreqUnit2.setText(to_html(f_unit, frmt=unit_frmt))
         self.lbl_TU1.setText(to_html(t_unit, frmt=unit_frmt))
         self.lbl_TU2.setText(to_html(t_unit, frmt=unit_frmt))
 
 # ------------------------------------------------------------------------------
@@ -744,14 +727,15 @@
                 _store_entry(source)
 
         # Call base class method to continue normal event processing:
         return super(Plot_Tran_Stim_UI, self).eventFilter(source, event)
 
     # -------------------------------------------------------------
     def normalize_freqs(self):
+        # TODO: move this to plot_tran_stim and update N_FFT
         """
         Update normalized frequencies and periods if required.
 
         `normalize_freqs()` is called when sampling frequency has been changed
         via signal ['view_changed':'f_S'] from plot_impz.process_sig_rx
 
         Frequency and time related entries are always stored normalized w.r.t. f_S
@@ -762,15 +746,15 @@
           values for frequency entries are updated with f_S, not the normalized freqs.
 
         - When the `f_S` lock button is checked, the absolute frequency values in
           the widget fields are kept constant, and the normalized freqs are updated.
         """
 
         f_corr = 1
-        if fb.fil[0]['freq_locked'] and fb.fil[0]['freq_specs_unit'] != 'k':
+        if fb.fil[0]['freq_locked']:
             f_corr = fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']
             self.f1 *= f_corr
             self.f2 *= f_corr
             self.T1 /= f_corr
             self.T2 /= f_corr
             self.TW1 /= f_corr
             self.TW2 /= f_corr
@@ -806,15 +790,15 @@
             else:
                 qstyle_widget(led, 'normal')
 
         self.update_freq_units()
 
         # emit a signal if normalized frequencies have changed due to an update
         # of f_S
-        if fb.fil[0]['freq_locked'] and fb.fil[0]['freq_specs_unit'] != 'k':
+        if fb.fil[0]['freq_locked']:
             self.emit({'ui_local_changed': 'f1_f2'})
 
     # -------------------------------------------------------------
     def _enable_stim_widgets(self):
         """ Enable / disable widgets depending on the selected stimulus """
 
         self.cmb_stim = qget_cmb_box(self.cmbStimulus)
```

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/tran/tran_io.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/tran/tran_io.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/plot_widgets/tran/tran_io_ui.py` & `pyfda-0.9.0b1/pyfda/plot_widgets/tran/tran_io_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,15 @@
         self._construct_UI()
 
     # -------------------------------------------------------------------------
     def _construct_UI(self):
         # =====================================================================
         # Controls
         # =====================================================================
-        self.lbl_title_io_file = QLabel("File:")
-        self.lbl_title_io_file.setObjectName("large")
+        self.lbl_title_io_file = QLabel("File:", objectName="large")
         # ----------------------------------------------------------------------
         # Main Widget
         # ----------------------------------------------------------------------
         self.cmb_file_format = QComboBox()
         qcmb_box_populate(self.cmb_file_format, self.cmb_file_format_items,
                           self.cmb_file_format_init)
         self.but_csv_options = PushButton(self, icon=QIcon(':/settings.svg'),
@@ -145,24 +144,22 @@
 
         layH_lbl_led_f_s_wav = QHBoxLayout()
         layH_lbl_led_f_s_wav.addWidget(self.lbl_f_s_wav)
         layH_lbl_led_f_s_wav.addWidget(self.led_f_s_wav)
 
         # ----------- LOAD ------------------------------------------------------------
         line1 = QVLine(width=10)
-        self.but_select = PushButton("Select", checkable=False)
-        self.but_select.setObjectName("large")
+        self.but_select = PushButton("Select", checkable=False, objectName="large")
         self.but_select.setSizePolicy(QSizePolicy.Expanding,
                                     QSizePolicy.Expanding)
         self.but_select.setToolTip(
             self.tr("<span>Select file, get its shape and size but don't load "
                     "it yet.</span>"))
 
-        self.but_load = QPushButton("Load:")
-        self.but_load.setObjectName("large")
+        self.but_load = QPushButton("Load:", objectName="large")
         self.but_load.setSizePolicy(QSizePolicy.Expanding,
                                     QSizePolicy.Expanding)
         self.but_load.setToolTip(
             self.tr("<span>Load / unload selected file.</span>"))
         self.but_load.setEnabled(False)
 
         self.lbl_file = QLabel(to_html("Name:", frmt="b"))
@@ -213,16 +210,15 @@
         self.led_normalize.setText(str(self.led_normalize_default))
         self.led_normalize.setEnabled(False)
         self.led_normalize.setMaximumWidth(qtext_width(N_x=8))
         # self.led_normalize.setFixedWidth(self.but_normalize.sizeHint().width())
 
         # ----------- SAVE ------------------------------------------------------------
         line3 = QVLine(width=5)
-        self.but_save = QPushButton("Save:")
-        self.but_save.setObjectName("large")
+        self.but_save = QPushButton("Save:", objectName="large")
         self.but_save.setSizePolicy(QSizePolicy.Expanding,
                                       QSizePolicy.Expanding)
         self.but_save.setToolTip(
             self.tr("<span>Save selected signals to R/L file channels.</span>"))
         self.lbl_chan_export_l = QLabel(to_html("L:", frmt="b"))
         self.cmb_chan_export_l = QComboBox(self)
         self.lbl_chan_export_r = QLabel(to_html("R:", frmt="b"))
@@ -309,16 +305,15 @@
         self.wdg_ctrl_io_file.setContentsMargins(0, 0, 0, 0)
 
         layH_io = QHBoxLayout()
         layH_io.addWidget(self.wdg_title_io_file)
         layH_io.addWidget(self.wdg_ctrl_io_file)
         layH_io.setContentsMargins(0, 0, 0, 0)
 
-        self.wdg_top = QWidget(self)
-        self.wdg_top.setObjectName("transparent")
+        self.wdg_top = QWidget(self, objectName="transparent")
         self.wdg_top.setLayout(layH_io)
         self.wdg_top.setContentsMargins(0, 0, 0, 0)
         self.wdg_top.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
         # ------ Local signal-slot-connections
         self.cmb_file_format.currentIndexChanged.connect(self.set_ui_visibility)
         self.cmb_data_format.currentIndexChanged.connect(self.set_ui_visibility)
         self.but_f_s_wav_auto.clicked.connect(self.set_ui_visibility)
```

### Comparing `pyfda-0.8.4/pyfda/pyfda.qrc` & `pyfda-0.9.0b1/pyfda/pyfda.qrc`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/pyfda_class.py` & `pyfda-0.9.0b1/pyfda/pyfda_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,19 @@
         Construct the main GUI, consisting of:
             - Tabbed input widgets (left side)
             - Tabbed plot widgets (right side)
             - Logger window (right side, below plot tab)
         """
 
         # ============== UI Layout with H and V-Splitter =====================
-
-        inputTabWidgets = input_tab_widgets.InputTabWidgets(self)  # input widgets
-        pltTabWidgets = plot_tab_widgets.PlotTabWidgets(self)  # plot widgets
+        # create tab widgets for input and plot widgets
+        inputTabWidgets = input_tab_widgets.InputTabWidgets(
+            self, objectName='input_tab_widgets_inst')
+        pltTabWidgets = plot_tab_widgets.PlotTabWidgets(
+            self, objectName='plot_tab_widgets_inst')
         self.loggerWin = QPlainTextEdit(self)  # logger window
         self.loggerWin.setReadOnly(True)
         # set custom right-button context menu policy
         self.loggerWin.setContextMenuPolicy(Qt.CustomContextMenu)
         self.loggerWin.customContextMenuRequested.connect(self.logger_win_context_menu)
         # create context menu and define actions and shortcuts
         self.popMenu = QMenu(self)
```

### Comparing `pyfda-0.8.4/pyfda/pyfda_rc.py` & `pyfda-0.9.0b1/pyfda/pyfda_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     'N_FFT':  2048,   # number of FFT points for plot commands (freqz etc.)
     'FMT': '{:.3g}',  # format string for QLineEdit fields
     'CSV': {  # format options and parameters for CSV-files and clipboard
             'delimiter': 'auto',  # default delimiter
             'lineterminator': CRLF,  # OS-dependent line break from pyfda_lib
             'orientation': 'auto',  # 'auto', 'vert', 'horiz'# table orientation
             'header': 'auto',  # 'auto', 'on', 'off'
-            'cmsis' : False,  # True, False
-            'clipboard': False  # source/target is QClipboard or file
+            # 'cmsis' : False,  # True, False
+            'destination': False  # source/target is 'clipboard' or 'file'
             },
     'screen': { # screen properties, filled with values in pyfdax.py
         'ref_dpi': None, 'scaling': None, # dpi for scaling = 1 and scaling factor
         'height': None, 'width': None}, # height and width in pixels
     'FMT_ba': 4,      # number of digits for coefficient table
     'FMT_pz': 5,      # number of digits for Pole/Zero table
     'P_Marker': [mpl_ms, 'r'],  # size and color for poles' marker
```

### Comparing `pyfda-0.8.4/pyfda/pyfdax.py` & `pyfda-0.9.0b1/pyfda/pyfdax.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/qrc_resources.py` & `pyfda-0.9.0b1/pyfda/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/widget_templates/filter_widgets/my_filter_widget.py` & `pyfda-0.9.0b1/pyfda/widget_templates/filter_widgets/my_filter_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from pyfda.libs.compat import QWidget, QLabel, QLineEdit, pyqtSignal, QVBoxLayout, QHBoxLayout
 
 import scipy.signal as sig
 import numpy as np
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_qt_lib import popup_warning
 from pyfda.libs.pyfda_lib import fil_save, safe_eval
 
 __version__ = "1.0"
 
 classes = {'AllpPZ':'Allpass (P)'} #: Dict containing class name : display name
 
 class AllpPZ(QWidget):
@@ -160,15 +160,15 @@
         logger.info(fil_dict['zpk'])
         
     def _test_poles(self):
         """
         Warn the user if one of the poles is outside the unit circle
         """
         if abs(self.p[0]) >= 1 or abs(self.p[1])  >=1:
-            return qfilter_warning(self, self.p[0], "Delay")
+            return popup_warning(self, self.p[0], "Delay")
         else:
             return True
 
     def _save(self, fil_dict, arg=None):
         """
         Convert between poles / zeros / gain, filter coefficients (polynomes)
         and second-order sections and store all available formats in the passed
```

### Comparing `pyfda-0.8.4/pyfda/widget_templates/input_widgets/my_input_widget.py` & `pyfda-0.9.0b1/pyfda/widget_templates/input_widgets/my_input_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda/widget_templates/plot_widgets/myplot.py` & `pyfda-0.9.0b1/pyfda/widget_templates/plot_widgets/myplot.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/pyfda.egg-info/PKG-INFO` & `pyfda-0.9.0b1/pyfda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.8.4
+Version: 0.9.0b1
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
@@ -26,15 +26,15 @@
 License-File: AUTHORS.md
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.2.0
 Requires-Dist: matplotlib>=3.1
 Requires-Dist: pyqt5
 Requires-Dist: docutils
 Requires-Dist: mplcursors
-Requires-Dist: numexpr<=2.8.4
+Requires-Dist: numexpr>=2.8.8
 Requires-Dist: markdown
 
 pyfda
 ======
 ## Python Filter Design Analysis Tool
 
 pyfda is a GUI based tool in Python / Qt for analysing and designing discrete time filters. Fixpoint implementations (for some filter types) can be simulated.
```

### Comparing `pyfda-0.8.4/pyfda.egg-info/SOURCES.txt` & `pyfda-0.9.0b1/pyfda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 pyfda/fixpoint_widgets/fir_df/fir_df.png
 pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
 pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
 pyfda/fixpoint_widgets/iir_df1/iir_df1.png
 pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
 pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
 pyfda/fixpoint_widgets/old/fixpoint_helpers.py
-pyfda/fixpoint_widgets/old/fixpoint_helpers_nmigen.py
 pyfda/fixpoint_widgets/old/delay/delay.png
 pyfda/fixpoint_widgets/old/delay/fx_delay.py
 pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen.py
 pyfda/fixpoint_widgets/old/fir_df/fir_df_nmigen_ui.py
 pyfda/images/icons/fft.svg
 pyfda/images/icons/plot_style-line-mkr.png
 pyfda/images/icons/plot_style-line.png
@@ -167,14 +166,15 @@
 pyfda/libs/__init__.py
 pyfda/libs/compat.py
 pyfda/libs/csv_option_box.py
 pyfda/libs/frozendict.py
 pyfda/libs/pyfda_dirs.py
 pyfda/libs/pyfda_fft_windows_lib.py
 pyfda/libs/pyfda_fix_lib.py
+pyfda/libs/pyfda_fix_lib_amaranth.py
 pyfda/libs/pyfda_io_lib.py
 pyfda/libs/pyfda_lib.py
 pyfda/libs/pyfda_log_template.conf
 pyfda/libs/pyfda_qt_lib.py
 pyfda/libs/pyfda_sig_lib.py
 pyfda/libs/pyfda_template.conf
 pyfda/libs/tree_builder.py
```

### Comparing `pyfda-0.8.4/pyfdax.spec` & `pyfda-0.9.0b1/pyfdax.spec`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.4/setup.py` & `pyfda-0.9.0b1/setup.py`

 * *Files identical despite different names*

