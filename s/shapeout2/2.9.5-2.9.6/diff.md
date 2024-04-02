# Comparing `tmp/shapeout2-2.9.5.tar.gz` & `tmp/shapeout2-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapeout2-2.9.5.tar", last modified: Wed Feb 16 22:31:08 2022, max compression
+gzip compressed data, was "shapeout2-2.9.6.tar", last modified: Thu Feb 17 14:57:12 2022, max compression
```

## Comparing `shapeout2-2.9.5.tar` & `shapeout2-2.9.6.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.323883 shapeout2-2.9.5/
--rw-r--r--   0 runner     (501) staff       (20)    11830 2022-02-16 22:30:22.000000 shapeout2-2.9.5/CHANGELOG
--rw-r--r--   0 runner     (501) staff       (20)    35149 2022-02-16 22:30:22.000000 shapeout2-2.9.5/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      202 2022-02-16 22:30:22.000000 shapeout2-2.9.5/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3376 2022-02-16 22:31:08.324125 shapeout2-2.9.5/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2298 2022-02-16 22:30:22.000000 shapeout2-2.9.5/README.rst
--rw-r--r--   0 runner     (501) staff       (20)       73 2022-02-16 22:31:08.324819 shapeout2-2.9.5/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1498 2022-02-16 22:30:22.000000 shapeout2-2.9.5/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.081162 shapeout2-2.9.5/shapeout2/
--rw-r--r--   0 runner     (501) staff       (20)       59 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1209 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     7095 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/_version.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2022-02-16 22:30:34.000000 shapeout2-2.9.5/shapeout2/_version_save.py
--rw-r--r--   0 runner     (501) staff       (20)     9523 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/extensions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.094828 shapeout2-2.9.5/shapeout2/gui/
--rw-r--r--   0 runner     (501) staff       (20)       78 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.110541 shapeout2-2.9.5/shapeout2/gui/analysis/
--rw-r--r--   0 runner     (501) staff       (20)      233 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13538 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_filter.py
--rw-r--r--   0 runner     (501) staff       (20)    11172 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_filter.ui
--rw-r--r--   0 runner     (501) staff       (20)     6628 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_meta.py
--rw-r--r--   0 runner     (501) staff       (20)     3841 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_meta.ui
--rw-r--r--   0 runner     (501) staff       (20)    26506 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_plot.py
--rw-r--r--   0 runner     (501) staff       (20)    32171 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_plot.ui
--rw-r--r--   0 runner     (501) staff       (20)    18536 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_slot.py
--rw-r--r--   0 runner     (501) staff       (20)    18446 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_slot.ui
--rw-r--r--   0 runner     (501) staff       (20)     1678 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_view.py
--rw-r--r--   0 runner     (501) staff       (20)     4982 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/ana_view.ui
--rw-r--r--   0 runner     (501) staff       (20)     1825 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/dlg_slot_reorder.py
--rw-r--r--   0 runner     (501) staff       (20)     3478 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/analysis/dlg_slot_reorder.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.112307 shapeout2-2.9.5/shapeout2/gui/bulk/
--rw-r--r--   0 runner     (501) staff       (20)       67 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/bulk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4639 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/bulk/bulk_emodulus.py
--rw-r--r--   0 runner     (501) staff       (20)     5907 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/bulk/bulk_emodulus.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.126219 shapeout2-2.9.5/shapeout2/gui/compute/
--rw-r--r--   0 runner     (501) staff       (20)      106 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3713 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4.py
--rw-r--r--   0 runner     (501) staff       (20)     5077 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4.ui
--rw-r--r--   0 runner     (501) staff       (20)     1789 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2163 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_dataset.ui
--rw-r--r--   0 runner     (501) staff       (20)     3829 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_results.py
--rw-r--r--   0 runner     (501) staff       (20)     7791 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_results.ui
--rw-r--r--   0 runner     (501) staff       (20)     7600 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     5013 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/compute/comp_stats.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.127396 shapeout2-2.9.5/shapeout2/gui/dcor/
--rw-r--r--   0 runner     (501) staff       (20)    10551 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/dcor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2947 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/dcor/dcor.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.131768 shapeout2-2.9.5/shapeout2/gui/export/
--rw-r--r--   0 runner     (501) staff       (20)      139 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5417 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2data.py
--rw-r--r--   0 runner     (501) staff       (20)     4628 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2data.ui
--rw-r--r--   0 runner     (501) staff       (20)     3021 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2filter.py
--rw-r--r--   0 runner     (501) staff       (20)     3514 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2filter.ui
--rw-r--r--   0 runner     (501) staff       (20)     3254 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2plot.py
--rw-r--r--   0 runner     (501) staff       (20)     4351 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/export/e2plot.ui
--rw-r--r--   0 runner     (501) staff       (20)      346 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/idiom.py
--rw-r--r--   0 runner     (501) staff       (20)    38247 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/main.py
--rw-r--r--   0 runner     (501) staff       (20)    15560 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/main.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.141937 shapeout2-2.9.5/shapeout2/gui/matrix/
--rw-r--r--   0 runner     (501) staff       (20)      206 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5289 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/block_matrix.py
--rw-r--r--   0 runner     (501) staff       (20)     6017 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/block_matrix.ui
--rw-r--r--   0 runner     (501) staff       (20)    21243 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/data_matrix.py
--rw-r--r--   0 runner     (501) staff       (20)     4084 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)    10245 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_dataset.ui
--rw-r--r--   0 runner     (501) staff       (20)     3668 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_element.py
--rw-r--r--   0 runner     (501) staff       (20)     4313 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_element.ui
--rw-r--r--   0 runner     (501) staff       (20)     3594 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_filter.py
--rw-r--r--   0 runner     (501) staff       (20)     8290 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/dm_filter.ui
--rw-r--r--   0 runner     (501) staff       (20)    11192 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/plot_matrix.py
--rw-r--r--   0 runner     (501) staff       (20)     1333 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/pm_element.py
--rw-r--r--   0 runner     (501) staff       (20)     2592 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/pm_plot.py
--rw-r--r--   0 runner     (501) staff       (20)     7107 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/matrix/pm_plot.ui
--rw-r--r--   0 runner     (501) staff       (20)    27341 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/pipeline_plot.py
--rw-r--r--   0 runner     (501) staff       (20)     1617 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/pipeline_plot.ui
--rw-r--r--   0 runner     (501) staff       (20)    12364 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/preferences.py
--rw-r--r--   0 runner     (501) staff       (20)    13607 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/preferences.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.144577 shapeout2-2.9.5/shapeout2/gui/quick_view/
--rw-r--r--   0 runner     (501) staff       (20)       45 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/quick_view/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    30873 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/quick_view/qv_main.py
--rw-r--r--   0 runner     (501) staff       (20)    29802 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/quick_view/qv_main.ui
--rw-r--r--   0 runner     (501) staff       (20)     9726 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/quick_view/qv_scatter.py
--rw-r--r--   0 runner     (501) staff       (20)      150 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/quick_view/qv_style.css
--rw-r--r--   0 runner     (501) staff       (20)     3252 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/update.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.163864 shapeout2-2.9.5/shapeout2/gui/widgets/
--rw-r--r--   0 runner     (501) staff       (20)      599 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      737 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/bg_thread.py
--rw-r--r--   0 runner     (501) staff       (20)     2603 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/bulk_list.py
--rw-r--r--   0 runner     (501) staff       (20)     2194 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/bulk_list.ui
--rw-r--r--   0 runner     (501) staff       (20)     2138 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/double_spin_box_nan.py
--rw-r--r--   0 runner     (501) staff       (20)      184 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/key_value_table_widget.css
--rw-r--r--   0 runner     (501) staff       (20)     2943 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/key_value_table_widget.py
--rw-r--r--   0 runner     (501) staff       (20)      407 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/mdi_subwindow_wo_close.py
--rw-r--r--   0 runner     (501) staff       (20)     8002 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/qrangeslider.py
--rw-r--r--   0 runner     (501) staff       (20)     8116 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/rangecontrol.py
--rw-r--r--   0 runner     (501) staff       (20)     2540 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/rangecontrol.ui
--rw-r--r--   0 runner     (501) staff       (20)     1575 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/simple_image_view.py
--rw-r--r--   0 runner     (501) staff       (20)     4105 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/simple_plot_widget.py
--rw-r--r--   0 runner     (501) staff       (20)     1233 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/so_colorbaritem.py
--rw-r--r--   0 runner     (501) staff       (20)     1069 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/gui/widgets/wait_cursor.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.170793 shapeout2-2.9.5/shapeout2/img/
--rw-r--r--   0 runner     (501) staff       (20)      161 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      117 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.171959 shapeout2-2.9.5/shapeout2/img/icon-theme/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.173398 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/
--rw-r--r--   0 runner     (501) staff       (20)     9362 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/COPYING-ICONS
--rw-r--r--   0 runner     (501) staff       (20)    26527 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/COPYING.LIB
--rw-r--r--   0 runner     (501) staff       (20)      271 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/README
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.066190 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.206957 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/
--rw-r--r--   0 runner     (501) staff       (20)      457 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)     1207 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/code-context.svg
--rw-r--r--   0 runner     (501) staff       (20)      766 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      626 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      422 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      504 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      504 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      603 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      603 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      733 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      577 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)     1150 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/draw-watercolor.svg
--rw-r--r--   0 runner     (501) staff       (20)     1336 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-clear-all.svg
--rw-r--r--   0 runner     (501) staff       (20)      673 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      612 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-paste.svg
--rw-r--r--   0 runner     (501) staff       (20)    20688 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/globe.svg
--rw-r--r--   0 runner     (501) staff       (20)      989 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      490 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/list-add.svg
--rw-r--r--   0 runner     (501) staff       (20)      633 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)      552 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-columns.svg
--rw-r--r--   0 runner     (501) staff       (20)      711 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-order-lower.svg
--rw-r--r--   0 runner     (501) staff       (20)      552 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-rows.svg
--rw-r--r--   0 runner     (501) staff       (20)     1255 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/office-chart-ring.svg
--rw-r--r--   0 runner     (501) staff       (20)      967 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/office-chart-scatter.svg
--rw-r--r--   0 runner     (501) staff       (20)      610 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/path-mode-polyline.svg
--rw-r--r--   0 runner     (501) staff       (20)     1060 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/preferences-activities.svg
--rw-r--r--   0 runner     (501) staff       (20)      361 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/remove.svg
--rw-r--r--   0 runner     (501) staff       (20)      684 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/search.svg
--rw-r--r--   0 runner     (501) staff       (20)      656 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/show-grid.svg
--rw-r--r--   0 runner     (501) staff       (20)      898 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/special_paste.svg
--rw-r--r--   0 runner     (501) staff       (20)      497 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/tools-wizard.svg
--rw-r--r--   0 runner     (501) staff       (20)      575 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/view-filter.svg
--rw-r--r--   0 runner     (501) staff       (20)      445 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/view-statistics.svg
--rw-r--r--   0 runner     (501) staff       (20)     1447 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/visibility.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.241663 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/
--rw-r--r--   0 runner     (501) staff       (20)      447 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)     1258 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/code-context.svg
--rw-r--r--   0 runner     (501) staff       (20)      962 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      487 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      467 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      567 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      567 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      472 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      472 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      788 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      640 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)     1275 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/draw-watercolor.svg
--rw-r--r--   0 runner     (501) staff       (20)     1182 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-clear-all.svg
--rw-r--r--   0 runner     (501) staff       (20)      663 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      608 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-paste.svg
--rw-r--r--   0 runner     (501) staff       (20)    24227 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/globe.svg
--rw-r--r--   0 runner     (501) staff       (20)      904 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      441 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/list-add.svg
--rw-r--r--   0 runner     (501) staff       (20)      637 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)      560 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-columns.svg
--rw-r--r--   0 runner     (501) staff       (20)      916 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-order-lower.svg
--rw-r--r--   0 runner     (501) staff       (20)      622 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-rows.svg
--rw-r--r--   0 runner     (501) staff       (20)     1614 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/office-chart-ring.svg
--rw-r--r--   0 runner     (501) staff       (20)     1268 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/office-chart-scatter.svg
--rw-r--r--   0 runner     (501) staff       (20)      677 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/path-mode-polyline.svg
--rw-r--r--   0 runner     (501) staff       (20)     1087 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/preferences-activities.svg
--rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/remove.svg
--rw-r--r--   0 runner     (501) staff       (20)      908 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/special_paste.svg
--rw-r--r--   0 runner     (501) staff       (20)      870 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/tools-wizard.svg
--rw-r--r--   0 runner     (501) staff       (20)      684 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/view-filter.svg
--rw-r--r--   0 runner     (501) staff       (20)      452 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/view-statistics.svg
--rw-r--r--   0 runner     (501) staff       (20)     1062 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/visibility.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.277435 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/
--rw-r--r--   0 runner     (501) staff       (20)      481 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)     1292 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/code-context.svg
--rw-r--r--   0 runner     (501) staff       (20)      996 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      521 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      501 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      601 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      601 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      506 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      506 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      822 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      674 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)     1309 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/draw-watercolor.svg
--rw-r--r--   0 runner     (501) staff       (20)     1216 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-clear-all.svg
--rw-r--r--   0 runner     (501) staff       (20)      697 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      642 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-paste.svg
--rw-r--r--   0 runner     (501) staff       (20)    24261 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/globe.svg
--rw-r--r--   0 runner     (501) staff       (20)      938 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      475 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/list-add.svg
--rw-r--r--   0 runner     (501) staff       (20)      671 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)      594 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-columns.svg
--rw-r--r--   0 runner     (501) staff       (20)      950 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-order-lower.svg
--rw-r--r--   0 runner     (501) staff       (20)      656 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-rows.svg
--rw-r--r--   0 runner     (501) staff       (20)     1648 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/office-chart-ring.svg
--rw-r--r--   0 runner     (501) staff       (20)     1302 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/office-chart-scatter.svg
--rw-r--r--   0 runner     (501) staff       (20)      711 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/path-mode-polyline.svg
--rw-r--r--   0 runner     (501) staff       (20)     1074 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/preferences-activities.svg
--rw-r--r--   0 runner     (501) staff       (20)      389 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/remove.svg
--rw-r--r--   0 runner     (501) staff       (20)      942 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/special_paste.svg
--rw-r--r--   0 runner     (501) staff       (20)      904 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/tools-wizard.svg
--rw-r--r--   0 runner     (501) staff       (20)      718 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/view-filter.svg
--rw-r--r--   0 runner     (501) staff       (20)      486 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/view-statistics.svg
--rw-r--r--   0 runner     (501) staff       (20)     1096 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/visibility.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.282528 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/
--rw-r--r--   0 runner     (501) staff       (20)      421 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)      733 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      375 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      391 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      665 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      728 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      918 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/object-order-lower.svg
--rw-r--r--   0 runner     (501) staff       (20)      820 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/view-filter.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.067452 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.284795 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/16/
--rw-r--r--   0 runner     (501) staff       (20)      818 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/16/folder-cloud.svg
--rw-r--r--   0 runner     (501) staff       (20)      609 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/16/folder.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.285897 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/22/
--rw-r--r--   0 runner     (501) staff       (20)      780 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/22/folder-cloud.svg
--rw-r--r--   0 runner     (501) staff       (20)      654 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/22/folder.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.286903 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/24/
--rw-r--r--   0 runner     (501) staff       (20)      814 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/24/folder-cloud.svg
--rw-r--r--   0 runner     (501) staff       (20)      688 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/24/folder.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.287872 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/32/
--rw-r--r--   0 runner     (501) staff       (20)     5337 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/32/folder-cloud.svg
--rw-r--r--   0 runner     (501) staff       (20)     1831 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/32/folder.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.289013 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/64/
--rw-r--r--   0 runner     (501) staff       (20)     6595 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/64/folder-cloud.svg
--rw-r--r--   0 runner     (501) staff       (20)     2116 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/64/folder.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.068509 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.289509 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/16/
--rw-r--r--   0 runner     (501) staff       (20)      529 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/16/dialog-information.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.291751 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/
--rw-r--r--   0 runner     (501) staff       (20)      525 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)      473 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)      680 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)      329 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-warning.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.294224 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/
--rw-r--r--   0 runner     (501) staff       (20)      559 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)      507 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)      714 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)      363 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-warning.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.301569 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/
--rw-r--r--   0 runner     (501) staff       (20)     2991 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)     2726 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)     3645 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)     2892 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-warning.svg
--rw-r--r--   0 runner     (501) staff       (20)     3349 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/collect_icons.py
--rw-r--r--   0 runner     (501) staff       (20)     1020 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/index.theme
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.307064 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/
--rw-r--r--   0 runner     (501) staff       (20)     7277 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/dcor.png
--rw-r--r--   0 runner     (501) staff       (20)      522 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/edit-copy-anew.svg
--rw-r--r--   0 runner     (501) staff       (20)     2279 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/emodulus.svg
--rw-r--r--   0 runner     (501) staff       (20)     2873 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/region_channel.svg
--rw-r--r--   0 runner     (501) staff       (20)     2997 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/region_reservoir.svg
--rw-r--r--   0 runner     (501) staff       (20)     4187 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/rlang.svg
--rw-r--r--   0 runner     (501) staff       (20)     4126 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/statistical_significance.svg
--rw-r--r--   0 runner     (501) staff       (20)     5422 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon.png
--rw-r--r--   0 runner     (501) staff       (20)    21701 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/icon.svg
--rw-r--r--   0 runner     (501) staff       (20)    42784 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/img/splash.png
--rw-r--r--   0 runner     (501) staff       (20)     2826 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/meta_tool.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.310744 shapeout2-2.9.5/shapeout2/pipeline/
--rw-r--r--   0 runner     (501) staff       (20)      212 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    19466 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/core.py
--rw-r--r--   0 runner     (501) staff       (20)     8045 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/dataslot.py
--rw-r--r--   0 runner     (501) staff       (20)     5417 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/filter.py
--rw-r--r--   0 runner     (501) staff       (20)     5791 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/filter_ray.py
--rw-r--r--   0 runner     (501) staff       (20)     5893 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/pipeline/plot.py
--rw-r--r--   0 runner     (501) staff       (20)     2252 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/plot_cache.py
--rw-r--r--   0 runner     (501) staff       (20)    13818 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/session.py
--rw-r--r--   0 runner     (501) staff       (20)     1722 2022-02-16 22:30:22.000000 shapeout2-2.9.5/shapeout2/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.084353 shapeout2-2.9.5/shapeout2.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3376 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    12641 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       51 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      113 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2022-02-16 22:31:07.000000 shapeout2-2.9.5/shapeout2.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.322914 shapeout2-2.9.5/tests/
--rw-r--r--   0 runner     (501) staff       (20)     1365 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-16 22:31:08.323469 shapeout2-2.9.5/tests/data/
--rw-r--r--   0 runner     (501) staff       (20)     1104 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/data/ext_feat_anc_plugin_ca.py
--rw-r--r--   0 runner     (501) staff       (20)     6769 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_extensions.py
--rw-r--r--   0 runner     (501) staff       (20)     2037 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_basic.py
--rw-r--r--   0 runner     (501) staff       (20)     6343 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_bulk_emodulus.py
--rw-r--r--   0 runner     (501) staff       (20)     3618 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_compute_lme4.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_compute_stats.py
--rw-r--r--   0 runner     (501) staff       (20)    10250 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_emodulus.py
--rw-r--r--   0 runner     (501) staff       (20)     3265 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_export_data.py
--rw-r--r--   0 runner     (501) staff       (20)     1637 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_export_plot.py
--rw-r--r--   0 runner     (501) staff       (20)     8824 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_filter.py
--rw-r--r--   0 runner     (501) staff       (20)     2678 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_matrix.py
--rw-r--r--   0 runner     (501) staff       (20)     2344 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_pipeline_plot.py
--rw-r--r--   0 runner     (501) staff       (20)     9241 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_plotting.py
--rw-r--r--   0 runner     (501) staff       (20)    14691 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_quickview.py
--rw-r--r--   0 runner     (501) staff       (20)     1534 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_reorder_datasets.py
--rw-r--r--   0 runner     (501) staff       (20)     1061 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_gui_update.py
--rw-r--r--   0 runner     (501) staff       (20)     3484 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_pipeline_core.py
--rw-r--r--   0 runner     (501) staff       (20)     3736 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_pipeline_filter_ray.py
--rw-r--r--   0 runner     (501) staff       (20)     9437 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_session.py
--rw-r--r--   0 runner     (501) staff       (20)      452 2022-02-16 22:30:22.000000 shapeout2-2.9.5/tests/test_util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.382580 shapeout2-2.9.6/
+-rw-r--r--   0 runner     (501) staff       (20)    11899 2022-02-17 14:56:37.000000 shapeout2-2.9.6/CHANGELOG
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2022-02-17 14:56:37.000000 shapeout2-2.9.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      202 2022-02-17 14:56:37.000000 shapeout2-2.9.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2022-02-17 14:57:12.382801 shapeout2-2.9.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2298 2022-02-17 14:56:37.000000 shapeout2-2.9.6/README.rst
+-rw-r--r--   0 runner     (501) staff       (20)       73 2022-02-17 14:57:12.383515 shapeout2-2.9.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1498 2022-02-17 14:56:37.000000 shapeout2-2.9.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.257711 shapeout2-2.9.6/shapeout2/
+-rw-r--r--   0 runner     (501) staff       (20)       59 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1209 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7095 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2022-02-17 14:56:49.000000 shapeout2-2.9.6/shapeout2/_version_save.py
+-rw-r--r--   0 runner     (501) staff       (20)     9523 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/extensions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.264972 shapeout2-2.9.6/shapeout2/gui/
+-rw-r--r--   0 runner     (501) staff       (20)       78 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.271206 shapeout2-2.9.6/shapeout2/gui/analysis/
+-rw-r--r--   0 runner     (501) staff       (20)      233 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13538 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_filter.py
+-rw-r--r--   0 runner     (501) staff       (20)    11172 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_filter.ui
+-rw-r--r--   0 runner     (501) staff       (20)     6628 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_meta.py
+-rw-r--r--   0 runner     (501) staff       (20)     3841 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_meta.ui
+-rw-r--r--   0 runner     (501) staff       (20)    26506 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)    32171 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_plot.ui
+-rw-r--r--   0 runner     (501) staff       (20)    18536 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_slot.py
+-rw-r--r--   0 runner     (501) staff       (20)    18446 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_slot.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1678 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_view.py
+-rw-r--r--   0 runner     (501) staff       (20)     4982 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/ana_view.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1825 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/dlg_slot_reorder.py
+-rw-r--r--   0 runner     (501) staff       (20)     3478 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/analysis/dlg_slot_reorder.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.272625 shapeout2-2.9.6/shapeout2/gui/bulk/
+-rw-r--r--   0 runner     (501) staff       (20)       67 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/bulk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4639 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/bulk/bulk_emodulus.py
+-rw-r--r--   0 runner     (501) staff       (20)     5907 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/bulk/bulk_emodulus.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.276930 shapeout2-2.9.6/shapeout2/gui/compute/
+-rw-r--r--   0 runner     (501) staff       (20)      106 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3713 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4.py
+-rw-r--r--   0 runner     (501) staff       (20)     5077 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1789 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2163 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_dataset.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3829 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_results.py
+-rw-r--r--   0 runner     (501) staff       (20)     7791 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_results.ui
+-rw-r--r--   0 runner     (501) staff       (20)     7600 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     5013 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/compute/comp_stats.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.277897 shapeout2-2.9.6/shapeout2/gui/dcor/
+-rw-r--r--   0 runner     (501) staff       (20)    10551 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/dcor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2947 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/dcor/dcor.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.281349 shapeout2-2.9.6/shapeout2/gui/export/
+-rw-r--r--   0 runner     (501) staff       (20)      139 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5417 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2data.py
+-rw-r--r--   0 runner     (501) staff       (20)     4628 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2data.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3021 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2filter.py
+-rw-r--r--   0 runner     (501) staff       (20)     3514 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2filter.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3254 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     4351 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/export/e2plot.ui
+-rw-r--r--   0 runner     (501) staff       (20)      346 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/idiom.py
+-rw-r--r--   0 runner     (501) staff       (20)    38242 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/main.py
+-rw-r--r--   0 runner     (501) staff       (20)    15560 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/main.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.287717 shapeout2-2.9.6/shapeout2/gui/matrix/
+-rw-r--r--   0 runner     (501) staff       (20)      206 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5289 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/block_matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)     6017 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/block_matrix.ui
+-rw-r--r--   0 runner     (501) staff       (20)    21243 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/data_matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)     4084 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)    10245 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_dataset.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3668 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_element.py
+-rw-r--r--   0 runner     (501) staff       (20)     4313 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_element.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3594 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_filter.py
+-rw-r--r--   0 runner     (501) staff       (20)     8290 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/dm_filter.ui
+-rw-r--r--   0 runner     (501) staff       (20)    11192 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/plot_matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)     1333 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/pm_element.py
+-rw-r--r--   0 runner     (501) staff       (20)     2592 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/pm_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     7107 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/matrix/pm_plot.ui
+-rw-r--r--   0 runner     (501) staff       (20)    27341 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/pipeline_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     1617 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/pipeline_plot.ui
+-rw-r--r--   0 runner     (501) staff       (20)    12364 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/preferences.py
+-rw-r--r--   0 runner     (501) staff       (20)    13607 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/preferences.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.290125 shapeout2-2.9.6/shapeout2/gui/quick_view/
+-rw-r--r--   0 runner     (501) staff       (20)       45 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/quick_view/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    30873 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/quick_view/qv_main.py
+-rw-r--r--   0 runner     (501) staff       (20)    29802 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/quick_view/qv_main.ui
+-rw-r--r--   0 runner     (501) staff       (20)     9726 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/quick_view/qv_scatter.py
+-rw-r--r--   0 runner     (501) staff       (20)      150 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/quick_view/qv_style.css
+-rw-r--r--   0 runner     (501) staff       (20)     3252 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/update.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.297512 shapeout2-2.9.6/shapeout2/gui/widgets/
+-rw-r--r--   0 runner     (501) staff       (20)      599 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      737 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/bg_thread.py
+-rw-r--r--   0 runner     (501) staff       (20)     2603 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/bulk_list.py
+-rw-r--r--   0 runner     (501) staff       (20)     2194 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/bulk_list.ui
+-rw-r--r--   0 runner     (501) staff       (20)     2138 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/double_spin_box_nan.py
+-rw-r--r--   0 runner     (501) staff       (20)      184 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/key_value_table_widget.css
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/key_value_table_widget.py
+-rw-r--r--   0 runner     (501) staff       (20)      407 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/mdi_subwindow_wo_close.py
+-rw-r--r--   0 runner     (501) staff       (20)     8002 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/qrangeslider.py
+-rw-r--r--   0 runner     (501) staff       (20)     8116 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/rangecontrol.py
+-rw-r--r--   0 runner     (501) staff       (20)     2540 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/rangecontrol.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1575 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/simple_image_view.py
+-rw-r--r--   0 runner     (501) staff       (20)     4105 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/simple_plot_widget.py
+-rw-r--r--   0 runner     (501) staff       (20)     1233 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/so_colorbaritem.py
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/gui/widgets/wait_cursor.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.300039 shapeout2-2.9.6/shapeout2/img/
+-rw-r--r--   0 runner     (501) staff       (20)      161 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      117 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.301058 shapeout2-2.9.6/shapeout2/img/icon-theme/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.302505 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/
+-rw-r--r--   0 runner     (501) staff       (20)     9362 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/COPYING-ICONS
+-rw-r--r--   0 runner     (501) staff       (20)    26527 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/COPYING.LIB
+-rw-r--r--   0 runner     (501) staff       (20)      271 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/README
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.245902 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.319166 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/
+-rw-r--r--   0 runner     (501) staff       (20)      457 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1207 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/code-context.svg
+-rw-r--r--   0 runner     (501) staff       (20)      766 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      626 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      422 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      504 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      504 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      603 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      603 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      733 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      577 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1150 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/draw-watercolor.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1336 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-clear-all.svg
+-rw-r--r--   0 runner     (501) staff       (20)      673 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      612 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)    20688 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/globe.svg
+-rw-r--r--   0 runner     (501) staff       (20)      989 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      490 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/list-add.svg
+-rw-r--r--   0 runner     (501) staff       (20)      633 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)      552 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-columns.svg
+-rw-r--r--   0 runner     (501) staff       (20)      711 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-order-lower.svg
+-rw-r--r--   0 runner     (501) staff       (20)      552 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-rows.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/office-chart-ring.svg
+-rw-r--r--   0 runner     (501) staff       (20)      967 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/office-chart-scatter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      610 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/path-mode-polyline.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1060 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/preferences-activities.svg
+-rw-r--r--   0 runner     (501) staff       (20)      361 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/remove.svg
+-rw-r--r--   0 runner     (501) staff       (20)      684 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/search.svg
+-rw-r--r--   0 runner     (501) staff       (20)      656 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/show-grid.svg
+-rw-r--r--   0 runner     (501) staff       (20)      898 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/special_paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)      497 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/tools-wizard.svg
+-rw-r--r--   0 runner     (501) staff       (20)      575 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/view-filter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      445 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/view-statistics.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1447 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/visibility.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.334354 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/
+-rw-r--r--   0 runner     (501) staff       (20)      447 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/code-context.svg
+-rw-r--r--   0 runner     (501) staff       (20)      962 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      487 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      467 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      567 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      567 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      472 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      472 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      788 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      640 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1275 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/draw-watercolor.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1182 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-clear-all.svg
+-rw-r--r--   0 runner     (501) staff       (20)      663 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      608 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)    24227 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/globe.svg
+-rw-r--r--   0 runner     (501) staff       (20)      904 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      441 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/list-add.svg
+-rw-r--r--   0 runner     (501) staff       (20)      637 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)      560 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-columns.svg
+-rw-r--r--   0 runner     (501) staff       (20)      916 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-order-lower.svg
+-rw-r--r--   0 runner     (501) staff       (20)      622 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-rows.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1614 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/office-chart-ring.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1268 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/office-chart-scatter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      677 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/path-mode-polyline.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/preferences-activities.svg
+-rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/remove.svg
+-rw-r--r--   0 runner     (501) staff       (20)      908 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/special_paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)      870 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/tools-wizard.svg
+-rw-r--r--   0 runner     (501) staff       (20)      684 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/view-filter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      452 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/view-statistics.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1062 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/visibility.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.349367 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/
+-rw-r--r--   0 runner     (501) staff       (20)      481 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1292 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/code-context.svg
+-rw-r--r--   0 runner     (501) staff       (20)      996 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      521 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      501 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      601 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      601 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      506 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      506 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      822 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      674 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1309 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/draw-watercolor.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1216 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-clear-all.svg
+-rw-r--r--   0 runner     (501) staff       (20)      697 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      642 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)    24261 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/globe.svg
+-rw-r--r--   0 runner     (501) staff       (20)      938 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      475 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/list-add.svg
+-rw-r--r--   0 runner     (501) staff       (20)      671 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)      594 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-columns.svg
+-rw-r--r--   0 runner     (501) staff       (20)      950 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-order-lower.svg
+-rw-r--r--   0 runner     (501) staff       (20)      656 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-rows.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/office-chart-ring.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1302 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/office-chart-scatter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      711 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/path-mode-polyline.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1074 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/preferences-activities.svg
+-rw-r--r--   0 runner     (501) staff       (20)      389 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/remove.svg
+-rw-r--r--   0 runner     (501) staff       (20)      942 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/special_paste.svg
+-rw-r--r--   0 runner     (501) staff       (20)      904 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/tools-wizard.svg
+-rw-r--r--   0 runner     (501) staff       (20)      718 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/view-filter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      486 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/view-statistics.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1096 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/visibility.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.354045 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/
+-rw-r--r--   0 runner     (501) staff       (20)      421 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)      733 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      375 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      355 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      391 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      665 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      728 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      918 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/object-order-lower.svg
+-rw-r--r--   0 runner     (501) staff       (20)      820 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/view-filter.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.247663 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.355017 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/16/
+-rw-r--r--   0 runner     (501) staff       (20)      818 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/16/folder-cloud.svg
+-rw-r--r--   0 runner     (501) staff       (20)      609 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/16/folder.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.355870 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/22/
+-rw-r--r--   0 runner     (501) staff       (20)      780 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/22/folder-cloud.svg
+-rw-r--r--   0 runner     (501) staff       (20)      654 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/22/folder.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.356718 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/24/
+-rw-r--r--   0 runner     (501) staff       (20)      814 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/24/folder-cloud.svg
+-rw-r--r--   0 runner     (501) staff       (20)      688 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/24/folder.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.357714 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/32/
+-rw-r--r--   0 runner     (501) staff       (20)     5337 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/32/folder-cloud.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1831 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/32/folder.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.358601 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/64/
+-rw-r--r--   0 runner     (501) staff       (20)     6595 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/64/folder-cloud.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2116 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/64/folder.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.248988 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.359125 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/16/
+-rw-r--r--   0 runner     (501) staff       (20)      529 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/16/dialog-information.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.360979 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/
+-rw-r--r--   0 runner     (501) staff       (20)      525 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)      473 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)      680 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)      329 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-warning.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.362996 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/
+-rw-r--r--   0 runner     (501) staff       (20)      559 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)      507 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)      714 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)      363 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-warning.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.364905 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/
+-rw-r--r--   0 runner     (501) staff       (20)     2991 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2726 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)     3645 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2892 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)     3349 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/collect_icons.py
+-rw-r--r--   0 runner     (501) staff       (20)     1020 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/index.theme
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.368566 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/
+-rw-r--r--   0 runner     (501) staff       (20)     7277 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/dcor.png
+-rw-r--r--   0 runner     (501) staff       (20)      522 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/edit-copy-anew.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2279 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/emodulus.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2873 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/region_channel.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2997 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/region_reservoir.svg
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/rlang.svg
+-rw-r--r--   0 runner     (501) staff       (20)     4126 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/statistical_significance.svg
+-rw-r--r--   0 runner     (501) staff       (20)     5422 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon.png
+-rw-r--r--   0 runner     (501) staff       (20)    21701 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/icon.svg
+-rw-r--r--   0 runner     (501) staff       (20)    42784 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/img/splash.png
+-rw-r--r--   0 runner     (501) staff       (20)     2826 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/meta_tool.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.371523 shapeout2-2.9.6/shapeout2/pipeline/
+-rw-r--r--   0 runner     (501) staff       (20)      212 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    19466 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/core.py
+-rw-r--r--   0 runner     (501) staff       (20)     8045 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/dataslot.py
+-rw-r--r--   0 runner     (501) staff       (20)     5417 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/filter.py
+-rw-r--r--   0 runner     (501) staff       (20)     5791 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/filter_ray.py
+-rw-r--r--   0 runner     (501) staff       (20)     5893 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/pipeline/plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     2252 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/plot_cache.py
+-rw-r--r--   0 runner     (501) staff       (20)    13818 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/session.py
+-rw-r--r--   0 runner     (501) staff       (20)     1722 2022-02-17 14:56:37.000000 shapeout2-2.9.6/shapeout2/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.260342 shapeout2-2.9.6/shapeout2.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2022-02-17 14:57:11.000000 shapeout2-2.9.6/shapeout2.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12641 2022-02-17 14:57:12.000000 shapeout2-2.9.6/shapeout2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-17 14:57:11.000000 shapeout2-2.9.6/shapeout2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       51 2022-02-17 14:57:11.000000 shapeout2-2.9.6/shapeout2.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      113 2022-02-17 14:57:11.000000 shapeout2-2.9.6/shapeout2.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2022-02-17 14:57:11.000000 shapeout2-2.9.6/shapeout2.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.381521 shapeout2-2.9.6/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     1365 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-17 14:57:12.382085 shapeout2-2.9.6/tests/data/
+-rw-r--r--   0 runner     (501) staff       (20)     1104 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/data/ext_feat_anc_plugin_ca.py
+-rw-r--r--   0 runner     (501) staff       (20)     6769 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_extensions.py
+-rw-r--r--   0 runner     (501) staff       (20)     2037 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_basic.py
+-rw-r--r--   0 runner     (501) staff       (20)     6343 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_bulk_emodulus.py
+-rw-r--r--   0 runner     (501) staff       (20)     3618 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_compute_lme4.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_compute_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)    10250 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_emodulus.py
+-rw-r--r--   0 runner     (501) staff       (20)     3265 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_export_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     1637 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_export_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     8824 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_filter.py
+-rw-r--r--   0 runner     (501) staff       (20)     2678 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)     2344 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_pipeline_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     9241 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_plotting.py
+-rw-r--r--   0 runner     (501) staff       (20)    14691 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_quickview.py
+-rw-r--r--   0 runner     (501) staff       (20)     1534 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_reorder_datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_gui_update.py
+-rw-r--r--   0 runner     (501) staff       (20)     3484 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_pipeline_core.py
+-rw-r--r--   0 runner     (501) staff       (20)     3736 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_pipeline_filter_ray.py
+-rw-r--r--   0 runner     (501) staff       (20)     9437 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_session.py
+-rw-r--r--   0 runner     (501) staff       (20)      452 2022-02-17 14:56:37.000000 shapeout2-2.9.6/tests/test_util.py
```

### Comparing `shapeout2-2.9.5/CHANGELOG` & `shapeout2-2.9.6/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+2.9.6
+ - fix: extensions not loaded during startup on Windows (#117)
 2.9.5
  - fix: polygon translation via drag-n-drop in polygon edit mode
    was not taken into account (#115)
  - enh: add (de-)select all button for lists in ComputeStatistics (#116)
  - enh: convert all selectable lists in dialogs to new BulkList class
  - setup: bump dclab from 0.39.13 to 0.39.15
 2.9.4
```

### Comparing `shapeout2-2.9.5/LICENSE` & `shapeout2-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/PKG-INFO` & `shapeout2-2.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: shapeout2
-Version: 2.9.5
+Version: 2.9.6
 Summary: User interface for real-time deformability cytometry (RT-DC)
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/ShapeOut2
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Description: |ShapeOut2|
         ===========
```

### Comparing `shapeout2-2.9.5/README.rst` & `shapeout2-2.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/setup.py` & `shapeout2-2.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/__main__.py` & `shapeout2-2.9.6/shapeout2/__main__.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/_version.py` & `shapeout2-2.9.6/shapeout2/_version.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/extensions.py` & `shapeout2-2.9.6/shapeout2/extensions.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_filter.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_filter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_filter.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_filter.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_meta.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_meta.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_meta.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_meta.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_plot.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_plot.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_plot.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_slot.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_slot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_slot.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_slot.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_view.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_view.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/ana_view.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/ana_view.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/dlg_slot_reorder.py` & `shapeout2-2.9.6/shapeout2/gui/analysis/dlg_slot_reorder.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/analysis/dlg_slot_reorder.ui` & `shapeout2-2.9.6/shapeout2/gui/analysis/dlg_slot_reorder.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/bulk/bulk_emodulus.py` & `shapeout2-2.9.6/shapeout2/gui/bulk/bulk_emodulus.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/bulk/bulk_emodulus.ui` & `shapeout2-2.9.6/shapeout2/gui/bulk/bulk_emodulus.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4.py` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4.ui` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_dataset.py` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_dataset.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_dataset.ui` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_dataset.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_results.py` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_results.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_lme4_results.ui` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_lme4_results.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_stats.py` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_stats.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/compute/comp_stats.ui` & `shapeout2-2.9.6/shapeout2/gui/compute/comp_stats.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/dcor/__init__.py` & `shapeout2-2.9.6/shapeout2/gui/dcor/__init__.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/dcor/dcor.ui` & `shapeout2-2.9.6/shapeout2/gui/dcor/dcor.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2data.py` & `shapeout2-2.9.6/shapeout2/gui/export/e2data.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2data.ui` & `shapeout2-2.9.6/shapeout2/gui/export/e2data.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2filter.py` & `shapeout2-2.9.6/shapeout2/gui/export/e2filter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2filter.ui` & `shapeout2-2.9.6/shapeout2/gui/export/e2filter.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2plot.py` & `shapeout2-2.9.6/shapeout2/gui/export/e2plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/export/e2plot.ui` & `shapeout2-2.9.6/shapeout2/gui/export/e2plot.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/main.py` & `shapeout2-2.9.6/shapeout2/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         api_key = self.settings.value("dcor/api key", "")
         dclab.rtdc_dataset.fmt_dcor.APIHandler.add_api_key(api_key)
         #: Analysis pipeline
         self.pipeline = pipeline.Pipeline()
         #: Extensions
         store_path = os_path.join(
             QStandardPaths.writableLocation(
-                QStandardPaths.AppLocalDataLocation), "extensions")
+                QStandardPaths.AppDataLocation), "extensions")
         try:
             self.extensions = ExtensionManager(store_path)
         except BaseException:
             QtWidgets.QMessageBox.warning(
                 self,
                 "Extensions automatically disabled",
                 "Some extensions could not be loaded and were disabled:\n\n"
```

### Comparing `shapeout2-2.9.5/shapeout2/gui/main.ui` & `shapeout2-2.9.6/shapeout2/gui/main.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/block_matrix.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/block_matrix.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/block_matrix.ui` & `shapeout2-2.9.6/shapeout2/gui/matrix/block_matrix.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/data_matrix.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/data_matrix.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_dataset.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_dataset.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_dataset.ui` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_dataset.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_element.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_element.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_element.ui` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_element.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_filter.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_filter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/dm_filter.ui` & `shapeout2-2.9.6/shapeout2/gui/matrix/dm_filter.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/plot_matrix.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/pm_element.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/pm_element.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/pm_plot.py` & `shapeout2-2.9.6/shapeout2/gui/matrix/pm_plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/matrix/pm_plot.ui` & `shapeout2-2.9.6/shapeout2/gui/matrix/pm_plot.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/pipeline_plot.py` & `shapeout2-2.9.6/shapeout2/gui/pipeline_plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/pipeline_plot.ui` & `shapeout2-2.9.6/shapeout2/gui/pipeline_plot.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/preferences.py` & `shapeout2-2.9.6/shapeout2/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/preferences.ui` & `shapeout2-2.9.6/shapeout2/gui/preferences.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/quick_view/qv_main.py` & `shapeout2-2.9.6/shapeout2/gui/quick_view/qv_main.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/quick_view/qv_main.ui` & `shapeout2-2.9.6/shapeout2/gui/quick_view/qv_main.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/quick_view/qv_scatter.py` & `shapeout2-2.9.6/shapeout2/gui/quick_view/qv_scatter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/update.py` & `shapeout2-2.9.6/shapeout2/gui/update.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/__init__.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/bg_thread.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/bg_thread.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/bulk_list.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/bulk_list.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/bulk_list.ui` & `shapeout2-2.9.6/shapeout2/gui/widgets/bulk_list.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/double_spin_box_nan.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/double_spin_box_nan.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/key_value_table_widget.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/key_value_table_widget.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/qrangeslider.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/qrangeslider.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/rangecontrol.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/rangecontrol.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/rangecontrol.ui` & `shapeout2-2.9.6/shapeout2/gui/widgets/rangecontrol.ui`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/simple_image_view.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/simple_image_view.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/simple_plot_widget.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/simple_plot_widget.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/so_colorbaritem.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/so_colorbaritem.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/gui/widgets/wait_cursor.py` & `shapeout2-2.9.6/shapeout2/gui/widgets/wait_cursor.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/COPYING-ICONS` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/COPYING-ICONS`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/COPYING.LIB` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/COPYING.LIB`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/code-context.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/code-context.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-cancel.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/dialog-close.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-open-folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-open-folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-open.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/document-save.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/documentinfo.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/draw-watercolor.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/draw-watercolor.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-clear-all.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-clear-all.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-clear.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/edit-paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/edit-paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/globe.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/globe.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/gtk-preferences.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/messagebox_warning.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-columns.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-columns.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-order-lower.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-order-lower.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/object-rows.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/object-rows.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/office-chart-ring.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/office-chart-ring.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/office-chart-scatter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/office-chart-scatter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/path-mode-polyline.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/path-mode-polyline.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/preferences-activities.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/search.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/search.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/show-grid.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/show-grid.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/special_paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/special_paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/view-filter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/view-filter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/16/visibility.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/16/visibility.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/code-context.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/code-context.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-cancel.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/document-save.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/documentinfo.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/draw-watercolor.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/draw-watercolor.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-clear-all.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-clear-all.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-clear.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/edit-paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/edit-paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/globe.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/globe.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/gtk-preferences.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/messagebox_warning.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-columns.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-columns.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-order-lower.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-order-lower.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/object-rows.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/object-rows.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/office-chart-ring.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/office-chart-ring.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/office-chart-scatter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/office-chart-scatter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/path-mode-polyline.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/path-mode-polyline.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/preferences-activities.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/special_paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/special_paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/tools-wizard.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/tools-wizard.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/view-filter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/view-filter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/22/visibility.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/22/visibility.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/code-context.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/code-context.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-cancel.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-close.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/document-save.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/documentinfo.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/draw-watercolor.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/draw-watercolor.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-clear-all.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-clear-all.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-clear.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/edit-paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/edit-paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/globe.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/globe.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/gtk-preferences.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/messagebox_warning.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-columns.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-columns.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-order-lower.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-order-lower.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/object-rows.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/object-rows.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/office-chart-ring.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/office-chart-ring.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/office-chart-scatter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/office-chart-scatter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/path-mode-polyline.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/path-mode-polyline.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/preferences-activities.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/special_paste.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/special_paste.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/tools-wizard.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/tools-wizard.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/view-filter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/view-filter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/24/visibility.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/24/visibility.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/dialog-cancel.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/document-save.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/gtk-preferences.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/object-order-lower.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/object-order-lower.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/actions/32/view-filter.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/actions/32/view-filter.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/16/folder-cloud.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/16/folder-cloud.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/16/folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/16/folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/22/folder-cloud.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/22/folder-cloud.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/22/folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/22/folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/24/folder-cloud.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/24/folder-cloud.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/24/folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/24/folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/32/folder-cloud.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/32/folder-cloud.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/32/folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/32/folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/64/folder-cloud.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/64/folder-cloud.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/places/64/folder.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/places/64/folder.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/16/dialog-information.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/16/dialog-information.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-error.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/22/dialog-question.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/22/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-error.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/24/dialog-question.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/24/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-error.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-information.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-information.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-question.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/breeze/status/64/dialog-warning.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/breeze/status/64/dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/collect_icons.py` & `shapeout2-2.9.6/shapeout2/img/icon-theme/collect_icons.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/index.theme` & `shapeout2-2.9.6/shapeout2/img/icon-theme/index.theme`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/dcor.png` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/dcor.png`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/edit-copy-anew.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/edit-copy-anew.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/emodulus.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/emodulus.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/region_channel.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/region_channel.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/region_reservoir.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/region_reservoir.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/rlang.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/rlang.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon-theme/shapeout2/statistical_significance.svg` & `shapeout2-2.9.6/shapeout2/img/icon-theme/shapeout2/statistical_significance.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon.png` & `shapeout2-2.9.6/shapeout2/img/icon.png`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/icon.svg` & `shapeout2-2.9.6/shapeout2/img/icon.svg`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/img/splash.png` & `shapeout2-2.9.6/shapeout2/img/splash.png`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/meta_tool.py` & `shapeout2-2.9.6/shapeout2/meta_tool.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/pipeline/core.py` & `shapeout2-2.9.6/shapeout2/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/pipeline/dataslot.py` & `shapeout2-2.9.6/shapeout2/pipeline/dataslot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/pipeline/filter.py` & `shapeout2-2.9.6/shapeout2/pipeline/filter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/pipeline/filter_ray.py` & `shapeout2-2.9.6/shapeout2/pipeline/filter_ray.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/pipeline/plot.py` & `shapeout2-2.9.6/shapeout2/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/plot_cache.py` & `shapeout2-2.9.6/shapeout2/plot_cache.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/session.py` & `shapeout2-2.9.6/shapeout2/session.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2/util.py` & `shapeout2-2.9.6/shapeout2/util.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/shapeout2.egg-info/PKG-INFO` & `shapeout2-2.9.6/shapeout2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: shapeout2
-Version: 2.9.5
+Version: 2.9.6
 Summary: User interface for real-time deformability cytometry (RT-DC)
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/ShapeOut2
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Description: |ShapeOut2|
         ===========
```

### Comparing `shapeout2-2.9.5/shapeout2.egg-info/SOURCES.txt` & `shapeout2-2.9.6/shapeout2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/conftest.py` & `shapeout2-2.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/data/ext_feat_anc_plugin_ca.py` & `shapeout2-2.9.6/tests/data/ext_feat_anc_plugin_ca.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_extensions.py` & `shapeout2-2.9.6/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_basic.py` & `shapeout2-2.9.6/tests/test_gui_basic.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_bulk_emodulus.py` & `shapeout2-2.9.6/tests/test_gui_bulk_emodulus.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_compute_lme4.py` & `shapeout2-2.9.6/tests/test_gui_compute_lme4.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_compute_stats.py` & `shapeout2-2.9.6/tests/test_gui_compute_stats.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_emodulus.py` & `shapeout2-2.9.6/tests/test_gui_emodulus.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_export_data.py` & `shapeout2-2.9.6/tests/test_gui_export_data.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_export_plot.py` & `shapeout2-2.9.6/tests/test_gui_export_plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_filter.py` & `shapeout2-2.9.6/tests/test_gui_filter.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_matrix.py` & `shapeout2-2.9.6/tests/test_gui_matrix.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_pipeline_plot.py` & `shapeout2-2.9.6/tests/test_gui_pipeline_plot.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_plotting.py` & `shapeout2-2.9.6/tests/test_gui_plotting.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_quickview.py` & `shapeout2-2.9.6/tests/test_gui_quickview.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_reorder_datasets.py` & `shapeout2-2.9.6/tests/test_gui_reorder_datasets.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_gui_update.py` & `shapeout2-2.9.6/tests/test_gui_update.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_pipeline_core.py` & `shapeout2-2.9.6/tests/test_pipeline_core.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_pipeline_filter_ray.py` & `shapeout2-2.9.6/tests/test_pipeline_filter_ray.py`

 * *Files identical despite different names*

### Comparing `shapeout2-2.9.5/tests/test_session.py` & `shapeout2-2.9.6/tests/test_session.py`

 * *Files identical despite different names*

