# Comparing `tmp/spine_items-0.8.0.tar.gz` & `tmp/spine_items-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_items-0.8.0.tar", last modified: Fri Sep  3 11:44:49 2021, max compression
+gzip compressed data, was "spine_items-0.9.0.tar", last modified: Wed Sep  8 12:31:44 2021, max compression
```

## Comparing `spine_items-0.8.0.tar` & `spine_items-0.9.0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.638792 spine_items-0.8.0/
--rw-rw-rw-   0        0        0    35823 2021-04-27 13:13:28.000000 spine_items-0.8.0/COPYING
--rw-rw-rw-   0        0        0     7815 2021-04-27 13:13:28.000000 spine_items-0.8.0/COPYING.LESSER
--rw-rw-rw-   0        0        0     2129 2021-09-03 11:44:49.638792 spine_items-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2021-06-29 14:12:36.000000 spine_items-0.8.0/README.md
--rw-rw-rw-   0        0        0      111 2021-04-27 13:13:28.000000 spine_items-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      828 2021-09-03 11:44:49.640823 spine_items-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1163 2021-06-29 14:12:36.000000 spine_items-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:47.786670 spine_items-0.8.0/spine_items/
--rw-rw-rw-   0        0        0     1086 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/__init__.py
--rw-rw-rw-   0        0        0     4907 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/animations.py
--rw-rw-rw-   0        0        0     1712 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/category.py
--rw-rw-rw-   0        0        0     5883 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/commands.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:47.881420 spine_items-0.8.0/spine_items/data_connection/
--rw-rw-rw-   0        0        0     1059 2021-01-15 07:37:16.000000 spine_items-0.8.0/spine_items/data_connection/__init__.py
--rw-rw-rw-   0        0        0     2223 2021-01-15 07:37:16.000000 spine_items-0.8.0/spine_items/data_connection/commands.py
--rw-rw-rw-   0        0        0    21329 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/data_connection/data_connection.py
--rw-rw-rw-   0        0        0     2628 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/data_connection/data_connection_factory.py
--rw-rw-rw-   0        0        0     3730 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/data_connection/data_connection_icon.py
--rw-rw-rw-   0        0        0     2751 2021-04-27 13:18:58.000000 spine_items-0.8.0/spine_items/data_connection/executable_item.py
--rw-rw-rw-   0        0        0     1404 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_connection/item_info.py
--rw-rw-rw-   0        0        0     1956 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/data_connection/output_resources.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:47.898373 spine_items-0.8.0/spine_items/data_connection/ui/
--rw-rw-rw-   0        0        0     1096 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_connection/ui/__init__.py
--rw-rw-rw-   0        0        0    12125 2021-04-14 09:24:28.000000 spine_items-0.8.0/spine_items/data_connection/ui/data_connection_properties.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:47.932332 spine_items-0.8.0/spine_items/data_connection/widgets/
--rw-rw-rw-   0        0        0     1083 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_connection/widgets/__init__.py
--rw-rw-rw-   0        0        0     2140 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_connection/widgets/add_data_connection_widget.py
--rw-rw-rw-   0        0        0     3179 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_connection/widgets/custom_menus.py
--rw-rw-rw-   0        0        0     5327 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/data_connection/widgets/data_connection_properties_widget.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.015063 spine_items-0.8.0/spine_items/data_store/
--rw-rw-rw-   0        0        0     1054 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/__init__.py
--rw-rw-rw-   0        0        0     1854 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/commands.py
--rw-rw-rw-   0        0        0    24876 2021-08-11 10:17:04.000000 spine_items-0.8.0/spine_items/data_store/data_store.py
--rw-rw-rw-   0        0        0     2545 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/data_store/data_store_factory.py
--rw-rw-rw-   0        0        0     1901 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/data_store/data_store_icon.py
--rw-rw-rw-   0        0        0     3558 2021-02-12 12:55:40.000000 spine_items-0.8.0/spine_items/data_store/do_work.py
--rw-rw-rw-   0        0        0     4971 2021-08-25 05:49:43.000000 spine_items-0.8.0/spine_items/data_store/executable_item.py
--rw-rw-rw-   0        0        0     1389 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/item_info.py
--rw-rw-rw-   0        0        0     1661 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/data_store/output_resources.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.032018 spine_items-0.8.0/spine_items/data_store/ui/
--rw-rw-rw-   0        0        0     1091 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/ui/__init__.py
--rw-rw-rw-   0        0        0    21923 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/data_store/ui/data_store_properties.py
--rw-rw-rw-   0        0        0     3411 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/data_store/utils.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.056987 spine_items-0.8.0/spine_items/data_store/widgets/
--rw-rw-rw-   0        0        0     1078 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/widgets/__init__.py
--rw-rw-rw-   0        0        0     2115 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_store/widgets/add_data_store_widget.py
--rw-rw-rw-   0        0        0     1947 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_store/widgets/data_store_properties_widget.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.164668 spine_items-0.8.0/spine_items/data_transformer/
--rw-rw-rw-   0        0        0     1060 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/__init__.py
--rw-rw-rw-   0        0        0     6511 2021-06-08 11:40:38.000000 spine_items-0.8.0/spine_items/data_transformer/commands.py
--rw-rw-rw-   0        0        0     9001 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/data_transformer.py
--rw-rw-rw-   0        0        0     3067 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/data_transformer/data_transformer_factory.py
--rw-rw-rw-   0        0        0     1872 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/data_transformer/data_transformer_icon.py
--rw-rw-rw-   0        0        0     3719 2021-04-14 07:30:23.000000 spine_items-0.8.0/spine_items/data_transformer/data_transformer_specification.py
--rw-rw-rw-   0        0        0     3659 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/executable_item.py
--rw-rw-rw-   0        0        0     1459 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/filter_config_path.py
--rw-rw-rw-   0        0        0     1402 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/item_info.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.206579 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/
--rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     5096 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/class_renames_table_model.py
--rw-rw-rw-   0        0        0     2243 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/parameter_drop_target_table_model.py
--rw-rw-rw-   0        0        0     4612 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/parameter_renames_table_model.py
--rw-rw-rw-   0        0        0     5719 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/mvcmodels/value_transformations_table_model.py
--rw-rw-rw-   0        0        0     2652 2021-04-21 09:41:26.000000 spine_items-0.8.0/spine_items/data_transformer/output_resources.py
--rw-rw-rw-   0        0        0     7269 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/settings.py
--rw-rw-rw-   0        0        0     1748 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/specification_factory.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.256424 spine_items-0.8.0/spine_items/data_transformer/ui/
--rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/ui/__init__.py
--rw-rw-rw-   0        0        0     5618 2021-06-11 13:28:55.000000 spine_items-0.8.0/spine_items/data_transformer/ui/class_renamer_editor.py
--rw-rw-rw-   0        0        0     8429 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/data_transformer/ui/data_transformer_properties.py
--rw-rw-rw-   0        0        0     5482 2021-06-11 13:28:55.000000 spine_items-0.8.0/spine_items/data_transformer/ui/parameter_renamer_editor.py
--rw-rw-rw-   0        0        0    26672 2021-06-11 13:28:55.000000 spine_items-0.8.0/spine_items/data_transformer/ui/specification_editor_widget.py
--rw-rw-rw-   0        0        0     9058 2021-06-11 13:28:56.000000 spine_items-0.8.0/spine_items/data_transformer/ui/value_transformer_editor.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.357182 spine_items-0.8.0/spine_items/data_transformer/widgets/
--rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/__init__.py
--rw-rw-rw-   0        0        0     2212 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/add_data_transformer_widget.py
--rw-rw-rw-   0        0        0     5581 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/class_rename.py
--rw-rw-rw-   0        0        0     2559 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/class_tree_widget.py
--rw-rw-rw-   0        0        0     6092 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/copy_paste.py
--rw-rw-rw-   0        0        0     1874 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/data_transformer_properties_widget.py
--rw-rw-rw-   0        0        0     1516 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/drop_target_table.py
--rw-rw-rw-   0        0        0    16390 2021-06-08 11:40:38.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/instructions_editor.py
--rw-rw-rw-   0        0        0     6042 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/parameter_rename.py
--rw-rw-rw-   0        0        0     3132 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/parameter_tree_widget.py
--rw-rw-rw-   0        0        0     8128 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/specification_editor_window.py
--rw-rw-rw-   0        0        0     6683 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/data_transformer/widgets/value_transformation.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.440970 spine_items-0.8.0/spine_items/exporter/
--rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/__init__.py
--rw-rw-rw-   0        0        0    12876 2021-04-26 06:19:04.000000 spine_items-0.8.0/spine_items/exporter/commands.py
--rw-rw-rw-   0        0        0     5587 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/do_work.py
--rw-rw-rw-   0        0        0     5994 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/executable_item.py
--rw-rw-rw-   0        0        0     7217 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/exporter.py
--rw-rw-rw-   0        0        0     3085 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/exporter/exporter_factory.py
--rw-rw-rw-   0        0        0     2199 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/exporter/exporter_icon.py
--rw-rw-rw-   0        0        0     1382 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/item_info.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.489801 spine_items-0.8.0/spine_items/exporter/mvcmodels/
--rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0    23167 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/mapping_editor_table_model.py
--rw-rw-rw-   0        0        0    13921 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/mappings_table_model.py
--rw-rw-rw-   0        0        0     2162 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/mappings_table_proxy.py
--rw-rw-rw-   0        0        0     5286 2021-04-26 06:19:04.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/preview_table_model.py
--rw-rw-rw-   0        0        0     7801 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/exporter/mvcmodels/preview_tree_model.py
--rw-rw-rw-   0        0        0     2340 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/preview_table_writer.py
--rw-rw-rw-   0        0        0     8201 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/exporter/specification.py
--rw-rw-rw-   0        0        0     1673 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/specification_factory.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.541691 spine_items-0.8.0/spine_items/exporter/ui/
--rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/ui/__init__.py
--rw-rw-rw-   0        0        0     3236 2021-06-11 13:28:56.000000 spine_items-0.8.0/spine_items/exporter/ui/default_filter_editor.py
--rw-rw-rw-   0        0        0     3834 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/ui/export_list_item.py
--rw-rw-rw-   0        0        0    10092 2021-04-14 09:24:28.000000 spine_items-0.8.0/spine_items/exporter/ui/exporter_properties.py
--rw-rw-rw-   0        0        0    25724 2021-06-11 13:28:56.000000 spine_items-0.8.0/spine_items/exporter/ui/specification_editor.py
--rw-rw-rw-   0        0        0     4138 2021-06-11 13:28:56.000000 spine_items-0.8.0/spine_items/exporter/ui/value_type_filter_editor.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.615495 spine_items-0.8.0/spine_items/exporter/widgets/
--rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/widgets/__init__.py
--rw-rw-rw-   0        0        0     2176 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/widgets/add_exporter_widget.py
--rw-rw-rw-   0        0        0     2689 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/widgets/export_list_item.py
--rw-rw-rw-   0        0        0     1892 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/widgets/exporter_properties.py
--rw-rw-rw-   0        0        0     3540 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/widgets/filter_edit_delegate.py
--rw-rw-rw-   0        0        0     3514 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/widgets/position_edit_delegate.py
--rw-rw-rw-   0        0        0    22596 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/exporter/widgets/preview_updater.py
--rw-rw-rw-   0        0        0    44323 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/exporter/widgets/specification_editor_window.py
--rw-rw-rw-   0        0        0     1255 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/exporter/widgets/specification_menu.py
--rw-rw-rw-   0        0        0     5338 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/exporter_executable_item_base.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.717224 spine_items-0.8.0/spine_items/gdx_exporter/
--rw-rw-rw-   0        0        0     1071 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/__init__.py
--rw-rw-rw-   0        0        0     2342 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/gdx_exporter/commands.py
--rw-rw-rw-   0        0        0     3212 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/gdx_exporter/do_work.py
--rw-rw-rw-   0        0        0     5700 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/gdx_exporter/executable_item.py
--rw-rw-rw-   0        0        0    15635 2021-06-08 11:40:38.000000 spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter.py
--rw-rw-rw-   0        0        0     2636 2021-06-08 11:40:38.000000 spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter_factory.py
--rw-rw-rw-   0        0        0     2205 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter_icon.py
--rw-rw-rw-   0        0        0     1389 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/item_info.py
--rw-rw-rw-   0        0        0     2880 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/list_utils.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.779033 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/
--rw-rw-rw-   0        0        0     1100 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     2515 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/domain_name_list_model.py
--rw-rw-rw-   0        0        0     9541 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/indexing_domain_list_model.py
--rw-rw-rw-   0        0        0     9125 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/indexing_table_model.py
--rw-rw-rw-   0        0        0     4591 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/parameter_name_list_model.py
--rw-rw-rw-   0        0        0     4188 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/record_list_model.py
--rw-rw-rw-   0        0        0    12084 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/set_list_model.py
--rw-rw-rw-   0        0        0     4379 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/gdx_exporter/settings_pack.py
--rw-rw-rw-   0        0        0     1471 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/settings_state.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.842862 spine_items-0.8.0/spine_items/gdx_exporter/ui/
--rw-rw-rw-   0        0        0     1077 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/__init__.py
--rw-rw-rw-   0        0        0    13418 2021-02-12 13:06:54.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/gdx_export_settings.py
--rw-rw-rw-   0        0        0     8205 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/gdx_exporter_properties.py
--rw-rw-rw-   0        0        0     7479 2021-02-12 13:06:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_index_settings.py
--rw-rw-rw-   0        0        0     9584 2021-02-12 13:06:57.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_index_settings_window.py
--rw-rw-rw-   0        0        0     8779 2021-02-12 13:06:58.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_merging_settings.py
--rw-rw-rw-   0        0        0     3973 2021-02-12 13:07:00.000000 spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_merging_settings_window.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.924381 spine_items-0.8.0/spine_items/gdx_exporter/widgets/
--rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/__init__.py
--rw-rw-rw-   0        0        0     2168 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/add_gdx_exporter_widget.py
--rw-rw-rw-   0        0        0    18380 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/gdx_export_settings.py
--rw-rw-rw-   0        0        0     1818 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/gdx_exporter_properties.py
--rw-rw-rw-   0        0        0     1354 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/merging_error_flag.py
--rw-rw-rw-   0        0        0    11414 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_index_settings.py
--rw-rw-rw-   0        0        0    19686 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_index_settings_window.py
--rw-rw-rw-   0        0        0     9888 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_merging_settings.py
--rw-rw-rw-   0        0        0    10120 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_merging_settings_window.py
--rw-rw-rw-   0        0        0     6698 2021-02-15 13:26:55.000000 spine_items-0.8.0/spine_items/gdx_exporter/worker.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:48.992202 spine_items-0.8.0/spine_items/gimlet/
--rw-rw-rw-   0        0        0     1068 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/__init__.py
--rw-rw-rw-   0        0        0     4010 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/commands.py
--rw-rw-rw-   0        0        0     9301 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/gimlet/executable_item.py
--rw-rw-rw-   0        0        0    17343 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/gimlet/gimlet.py
--rw-rw-rw-   0        0        0     2467 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/gimlet/gimlet_factory.py
--rw-rw-rw-   0        0        0     1499 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/gimlet/gimlet_icon.py
--rw-rw-rw-   0        0        0     1376 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/item_info.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.010152 spine_items-0.8.0/spine_items/gimlet/ui/
--rw-rw-rw-   0        0        0     1090 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/ui/__init__.py
--rw-rw-rw-   0        0        0    13242 2021-04-14 09:24:29.000000 spine_items-0.8.0/spine_items/gimlet/ui/gimlet_properties.py
--rw-rw-rw-   0        0        0     1146 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/utils.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.043064 spine_items-0.8.0/spine_items/gimlet/widgets/
--rw-rw-rw-   0        0        0     1077 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/widgets/__init__.py
--rw-rw-rw-   0        0        0     2170 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/gimlet/widgets/add_gimlet_widget.py
--rw-rw-rw-   0        0        0     1760 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/widgets/custom_menus.py
--rw-rw-rw-   0        0        0     1927 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/gimlet/widgets/gimlet_properties_widget.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.148449 spine_items-0.8.0/spine_items/importer/
--rw-rw-rw-   0        0        0     1052 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/__init__.py
--rw-rw-rw-   0        0        0    30568 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/importer/commands.py
--rw-rw-rw-   0        0        0    14703 2021-06-11 08:51:27.000000 spine_items-0.8.0/spine_items/importer/connection_manager.py
--rw-rw-rw-   0        0        0     6770 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/do_work.py
--rw-rw-rw-   0        0        0     6325 2021-04-27 13:18:58.000000 spine_items-0.8.0/spine_items/importer/executable_item.py
--rw-rw-rw-   0        0        0    16537 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/importer/importer.py
--rw-rw-rw-   0        0        0     2708 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/importer/importer_factory.py
--rw-rw-rw-   0        0        0     2222 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/importer/importer_icon.py
--rw-rw-rw-   0        0        0     3579 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/importer_specification.py
--rw-rw-rw-   0        0        0     1383 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/item_info.py
--rw-rw-rw-   0        0        0     1158 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/mapping_colors.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.198320 spine_items-0.8.0/spine_items/importer/mvcmodels/
--rw-rw-rw-   0        0        0     1076 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     6591 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/mvcmodels/mapping_list_model.py
--rw-rw-rw-   0        0        0    40090 2021-08-25 05:49:43.000000 spine_items-0.8.0/spine_items/importer/mvcmodels/mapping_specification_model.py
--rw-rw-rw-   0        0        0    14920 2021-06-11 08:51:27.000000 spine_items-0.8.0/spine_items/importer/mvcmodels/source_data_table_model.py
--rw-rw-rw-   0        0        0     7780 2021-04-23 13:26:19.000000 spine_items-0.8.0/spine_items/importer/mvcmodels/source_table_list_model.py
--rw-rw-rw-   0        0        0     1719 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/specification_factory.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.225758 spine_items-0.8.0/spine_items/importer/ui/
--rw-rw-rw-   0        0        0     1089 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/ui/__init__.py
--rw-rw-rw-   0        0        0    23336 2021-06-10 15:00:05.000000 spine_items-0.8.0/spine_items/importer/ui/import_editor_window.py
--rw-rw-rw-   0        0        0     9603 2021-04-14 09:24:30.000000 spine_items-0.8.0/spine_items/importer/ui/importer_properties.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.326491 spine_items-0.8.0/spine_items/importer/widgets/
--rw-rw-rw-   0        0        0     1076 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/importer/widgets/__init__.py
--rw-rw-rw-   0        0        0     2181 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/importer/widgets/add_importer_widget.py
--rw-rw-rw-   0        0        0     5057 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/widgets/custom_menus.py
--rw-rw-rw-   0        0        0    17132 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/importer/widgets/import_editor_window.py
--rw-rw-rw-   0        0        0    27561 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/importer/widgets/import_mapping_options.py
--rw-rw-rw-   0        0        0    12835 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/importer/widgets/import_mappings.py
--rw-rw-rw-   0        0        0    19706 2021-06-29 14:12:36.000000 spine_items-0.8.0/spine_items/importer/widgets/import_sources.py
--rw-rw-rw-   0        0        0     3291 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/widgets/importer_properties_widget.py
--rw-rw-rw-   0        0        0     2078 2021-04-23 13:26:19.000000 spine_items-0.8.0/spine_items/importer/widgets/multi_checkable_tree_view.py
--rw-rw-rw-   0        0        0    10657 2021-04-12 13:56:32.000000 spine_items-0.8.0/spine_items/importer/widgets/options_widget.py
--rw-rw-rw-   0        0        0    20858 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/importer/widgets/table_view_with_button_header.py
--rw-rw-rw-   0        0        0    14744 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/item_base.py
--rw-rw-rw-   0        0        0    24075 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/models.py
--rw-rw-rw-   0        0        0   114515 2021-08-20 08:29:28.000000 spine_items-0.8.0/spine_items/resources_icons_rc.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.411363 spine_items-0.8.0/spine_items/tool/
--rw-rw-rw-   0        0        0     1048 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/tool/__init__.py
--rw-rw-rw-   0        0        0     2542 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/tool/commands.py
--rw-rw-rw-   0        0        0    32856 2021-08-25 05:49:43.000000 spine_items-0.8.0/spine_items/tool/executable_item.py
--rw-rw-rw-   0        0        0     1371 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/tool/item_info.py
--rw-rw-rw-   0        0        0     2772 2021-04-12 13:56:33.000000 spine_items-0.8.0/spine_items/tool/output_resources.py
--rw-rw-rw-   0        0        0     1686 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/tool/specification_factory.py
--rw-rw-rw-   0        0        0    26258 2021-07-02 16:09:40.000000 spine_items-0.8.0/spine_items/tool/tool.py
--rw-rw-rw-   0        0        0     4339 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/tool/tool_factory.py
--rw-rw-rw-   0        0        0     3995 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/tool/tool_icon.py
--rw-rw-rw-   0        0        0    11781 2021-09-03 07:14:07.000000 spine_items-0.8.0/spine_items/tool/tool_instance.py
--rw-rw-rw-   0        0        0    24378 2021-08-18 12:14:10.000000 spine_items-0.8.0/spine_items/tool/tool_specifications.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.461266 spine_items-0.8.0/spine_items/tool/ui/
--rw-rw-rw-   0        0        0     1085 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/tool/ui/__init__.py
--rw-rw-rw-   0        0        0     9674 2021-02-12 13:07:05.000000 spine_items-0.8.0/spine_items/tool/ui/add_tool.py
--rw-rw-rw-   0        0        0     5269 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/tool/ui/julia_options.py
--rw-rw-rw-   0        0        0     8932 2021-08-27 13:58:22.000000 spine_items-0.8.0/spine_items/tool/ui/python_kernel_spec_options.py
--rw-rw-rw-   0        0        0    16410 2021-08-20 08:29:27.000000 spine_items-0.8.0/spine_items/tool/ui/tool_properties.py
--rw-rw-rw-   0        0        0    23514 2021-08-20 08:29:27.000000 spine_items-0.8.0/spine_items/tool/ui/tool_specification_form.py
--rw-rw-rw-   0        0        0     5061 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/tool/utils.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.526091 spine_items-0.8.0/spine_items/tool/widgets/
--rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/tool/widgets/__init__.py
--rw-rw-rw-   0        0        0     2197 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/tool/widgets/add_tool_widget.py
--rw-rw-rw-   0        0        0     3941 2021-04-12 13:56:33.000000 spine_items-0.8.0/spine_items/tool/widgets/custom_menus.py
--rw-rw-rw-   0        0        0     5842 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/tool/widgets/main_program_text_edit.py
--rw-rw-rw-   0        0        0    17495 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/tool/widgets/options_widgets.py
--rw-rw-rw-   0        0        0     2005 2021-06-23 14:51:54.000000 spine_items-0.8.0/spine_items/tool/widgets/tool_properties_widget.py
--rw-rw-rw-   0        0        0    10293 2021-08-09 14:40:32.000000 spine_items-0.8.0/spine_items/tool/widgets/tool_spec_optional_widgets.py
--rw-rw-rw-   0        0        0    55784 2021-09-03 07:14:07.000000 spine_items-0.8.0/spine_items/tool/widgets/tool_specification_editor_window.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.534099 spine_items-0.8.0/spine_items/ui/
--rw-rw-rw-   0        0        0     1090 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/ui/__init__.py
--rw-rw-rw-   0        0        0    11619 2021-08-25 05:49:43.000000 spine_items-0.8.0/spine_items/utils.py
--rw-rw-rw-   0        0        0     1054 2021-09-03 08:59:10.000000 spine_items-0.8.0/spine_items/version.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.585931 spine_items-0.8.0/spine_items/view/
--rw-rw-rw-   0        0        0     1048 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/__init__.py
--rw-rw-rw-   0        0        0     1583 2021-04-27 13:18:58.000000 spine_items-0.8.0/spine_items/view/executable_item.py
--rw-rw-rw-   0        0        0     1371 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/item_info.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.603886 spine_items-0.8.0/spine_items/view/ui/
--rw-rw-rw-   0        0        0     1085 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/ui/__init__.py
--rw-rw-rw-   0        0        0     7810 2021-02-15 09:22:32.000000 spine_items-0.8.0/spine_items/view/ui/view_properties.py
--rw-rw-rw-   0        0        0     7315 2021-05-25 09:51:15.000000 spine_items-0.8.0/spine_items/view/view.py
--rw-rw-rw-   0        0        0     2426 2021-04-21 09:41:14.000000 spine_items-0.8.0/spine_items/view/view_factory.py
--rw-rw-rw-   0        0        0     1508 2021-04-19 13:01:13.000000 spine_items-0.8.0/spine_items/view/view_icon.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:49.636832 spine_items-0.8.0/spine_items/view/widgets/
--rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/widgets/__init__.py
--rw-rw-rw-   0        0        0     1948 2021-06-04 14:34:51.000000 spine_items-0.8.0/spine_items/view/widgets/add_view_widget.py
--rw-rw-rw-   0        0        0     1774 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/widgets/custom_menus.py
--rw-rw-rw-   0        0        0     3007 2021-01-15 07:37:17.000000 spine_items-0.8.0/spine_items/view/widgets/view_properties_widget.py
--rw-rw-rw-   0        0        0     5586 2021-04-27 13:13:28.000000 spine_items-0.8.0/spine_items/widgets.py
-drwxrwxrwx   0        0        0        0 2021-09-03 11:44:47.817624 spine_items-0.8.0/spine_items.egg-info/
--rw-rw-rw-   0        0        0     2129 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10617 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-09-03 11:44:47.000000 spine_items-0.8.0/spine_items.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.812797 spine_items-0.9.0/
+-rw-rw-rw-   0        0        0    35823 2021-04-27 13:13:28.000000 spine_items-0.9.0/COPYING
+-rw-rw-rw-   0        0        0     7815 2021-04-27 13:13:28.000000 spine_items-0.9.0/COPYING.LESSER
+-rw-rw-rw-   0        0        0     2131 2021-09-08 12:31:44.812797 spine_items-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2021-06-29 14:12:36.000000 spine_items-0.9.0/README.md
+-rw-rw-rw-   0        0        0      111 2021-04-27 13:13:28.000000 spine_items-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      970 2021-09-08 12:31:44.812797 spine_items-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2021-06-29 14:12:36.000000 spine_items-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.579322 spine_items-0.9.0/spine_items/
+-rw-rw-rw-   0        0        0     1086 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/__init__.py
+-rw-rw-rw-   0        0        0     4907 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/animations.py
+-rw-rw-rw-   0        0        0     1712 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/category.py
+-rw-rw-rw-   0        0        0     5883 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/commands.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.662398 spine_items-0.9.0/spine_items/data_connection/
+-rw-rw-rw-   0        0        0     1059 2021-01-15 07:37:16.000000 spine_items-0.9.0/spine_items/data_connection/__init__.py
+-rw-rw-rw-   0        0        0     2223 2021-01-15 07:37:16.000000 spine_items-0.9.0/spine_items/data_connection/commands.py
+-rw-rw-rw-   0        0        0    21329 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/data_connection/data_connection.py
+-rw-rw-rw-   0        0        0     2628 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/data_connection/data_connection_factory.py
+-rw-rw-rw-   0        0        0     3730 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/data_connection/data_connection_icon.py
+-rw-rw-rw-   0        0        0     2751 2021-04-27 13:18:58.000000 spine_items-0.9.0/spine_items/data_connection/executable_item.py
+-rw-rw-rw-   0        0        0     1404 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_connection/item_info.py
+-rw-rw-rw-   0        0        0     1956 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/data_connection/output_resources.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.662398 spine_items-0.9.0/spine_items/data_connection/ui/
+-rw-rw-rw-   0        0        0     1096 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_connection/ui/__init__.py
+-rw-rw-rw-   0        0        0    12125 2021-04-14 09:24:28.000000 spine_items-0.9.0/spine_items/data_connection/ui/data_connection_properties.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.696085 spine_items-0.9.0/spine_items/data_connection/widgets/
+-rw-rw-rw-   0        0        0     1083 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_connection/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2140 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_connection/widgets/add_data_connection_widget.py
+-rw-rw-rw-   0        0        0     3179 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_connection/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0     5327 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/data_connection/widgets/data_connection_properties_widget.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.745709 spine_items-0.9.0/spine_items/data_store/
+-rw-rw-rw-   0        0        0     1054 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/__init__.py
+-rw-rw-rw-   0        0        0     1854 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/commands.py
+-rw-rw-rw-   0        0        0    24876 2021-08-11 10:17:04.000000 spine_items-0.9.0/spine_items/data_store/data_store.py
+-rw-rw-rw-   0        0        0     2545 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/data_store/data_store_factory.py
+-rw-rw-rw-   0        0        0     1901 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/data_store/data_store_icon.py
+-rw-rw-rw-   0        0        0     3558 2021-02-12 12:55:40.000000 spine_items-0.9.0/spine_items/data_store/do_work.py
+-rw-rw-rw-   0        0        0     4971 2021-08-25 05:49:43.000000 spine_items-0.9.0/spine_items/data_store/executable_item.py
+-rw-rw-rw-   0        0        0     1389 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/item_info.py
+-rw-rw-rw-   0        0        0     1661 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/data_store/output_resources.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.762338 spine_items-0.9.0/spine_items/data_store/ui/
+-rw-rw-rw-   0        0        0     1091 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/ui/__init__.py
+-rw-rw-rw-   0        0        0    21923 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/data_store/ui/data_store_properties.py
+-rw-rw-rw-   0        0        0     3411 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/data_store/utils.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.779056 spine_items-0.9.0/spine_items/data_store/widgets/
+-rw-rw-rw-   0        0        0     1078 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2115 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_store/widgets/add_data_store_widget.py
+-rw-rw-rw-   0        0        0     1947 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_store/widgets/data_store_properties_widget.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.845656 spine_items-0.9.0/spine_items/data_transformer/
+-rw-rw-rw-   0        0        0     1060 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/__init__.py
+-rw-rw-rw-   0        0        0     6511 2021-06-08 11:40:38.000000 spine_items-0.9.0/spine_items/data_transformer/commands.py
+-rw-rw-rw-   0        0        0     9001 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/data_transformer.py
+-rw-rw-rw-   0        0        0     3067 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/data_transformer/data_transformer_factory.py
+-rw-rw-rw-   0        0        0     1872 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/data_transformer/data_transformer_icon.py
+-rw-rw-rw-   0        0        0     3719 2021-04-14 07:30:23.000000 spine_items-0.9.0/spine_items/data_transformer/data_transformer_specification.py
+-rw-rw-rw-   0        0        0     3659 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/executable_item.py
+-rw-rw-rw-   0        0        0     1459 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/filter_config_path.py
+-rw-rw-rw-   0        0        0     1402 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/item_info.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.862367 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/
+-rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     5096 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/class_renames_table_model.py
+-rw-rw-rw-   0        0        0     2243 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/parameter_drop_target_table_model.py
+-rw-rw-rw-   0        0        0     4612 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/parameter_renames_table_model.py
+-rw-rw-rw-   0        0        0     5719 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/mvcmodels/value_transformations_table_model.py
+-rw-rw-rw-   0        0        0     2652 2021-04-21 09:41:26.000000 spine_items-0.9.0/spine_items/data_transformer/output_resources.py
+-rw-rw-rw-   0        0        0     7269 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/settings.py
+-rw-rw-rw-   0        0        0     1748 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/specification_factory.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.896020 spine_items-0.9.0/spine_items/data_transformer/ui/
+-rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/ui/__init__.py
+-rw-rw-rw-   0        0        0     5618 2021-06-11 13:28:55.000000 spine_items-0.9.0/spine_items/data_transformer/ui/class_renamer_editor.py
+-rw-rw-rw-   0        0        0     8429 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/data_transformer/ui/data_transformer_properties.py
+-rw-rw-rw-   0        0        0     5482 2021-06-11 13:28:55.000000 spine_items-0.9.0/spine_items/data_transformer/ui/parameter_renamer_editor.py
+-rw-rw-rw-   0        0        0    26672 2021-06-11 13:28:55.000000 spine_items-0.9.0/spine_items/data_transformer/ui/specification_editor_widget.py
+-rw-rw-rw-   0        0        0     9058 2021-06-11 13:28:56.000000 spine_items-0.9.0/spine_items/data_transformer/ui/value_transformer_editor.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.962644 spine_items-0.9.0/spine_items/data_transformer/widgets/
+-rw-rw-rw-   0        0        0      975 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2212 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/add_data_transformer_widget.py
+-rw-rw-rw-   0        0        0     5581 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/class_rename.py
+-rw-rw-rw-   0        0        0     2559 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/class_tree_widget.py
+-rw-rw-rw-   0        0        0     6092 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/copy_paste.py
+-rw-rw-rw-   0        0        0     1874 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/data_transformer_properties_widget.py
+-rw-rw-rw-   0        0        0     1516 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/drop_target_table.py
+-rw-rw-rw-   0        0        0    16390 2021-06-08 11:40:38.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/instructions_editor.py
+-rw-rw-rw-   0        0        0     6042 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/parameter_rename.py
+-rw-rw-rw-   0        0        0     3132 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/parameter_tree_widget.py
+-rw-rw-rw-   0        0        0     8128 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/specification_editor_window.py
+-rw-rw-rw-   0        0        0     6683 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/data_transformer/widgets/value_transformation.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.028215 spine_items-0.9.0/spine_items/exporter/
+-rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/__init__.py
+-rw-rw-rw-   0        0        0    12876 2021-04-26 06:19:04.000000 spine_items-0.9.0/spine_items/exporter/commands.py
+-rw-rw-rw-   0        0        0     5587 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/do_work.py
+-rw-rw-rw-   0        0        0     5994 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/executable_item.py
+-rw-rw-rw-   0        0        0     7217 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/exporter.py
+-rw-rw-rw-   0        0        0     3085 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/exporter/exporter_factory.py
+-rw-rw-rw-   0        0        0     2199 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/exporter/exporter_icon.py
+-rw-rw-rw-   0        0        0     1382 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/item_info.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.045850 spine_items-0.9.0/spine_items/exporter/mvcmodels/
+-rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0    23167 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/mapping_editor_table_model.py
+-rw-rw-rw-   0        0        0    13921 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/mappings_table_model.py
+-rw-rw-rw-   0        0        0     2162 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/mappings_table_proxy.py
+-rw-rw-rw-   0        0        0     5286 2021-04-26 06:19:04.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/preview_table_model.py
+-rw-rw-rw-   0        0        0     7801 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/exporter/mvcmodels/preview_tree_model.py
+-rw-rw-rw-   0        0        0     2340 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/preview_table_writer.py
+-rw-rw-rw-   0        0        0     8201 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/exporter/specification.py
+-rw-rw-rw-   0        0        0     1673 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/specification_factory.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.062480 spine_items-0.9.0/spine_items/exporter/ui/
+-rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/ui/__init__.py
+-rw-rw-rw-   0        0        0     3236 2021-06-11 13:28:56.000000 spine_items-0.9.0/spine_items/exporter/ui/default_filter_editor.py
+-rw-rw-rw-   0        0        0     3834 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/ui/export_list_item.py
+-rw-rw-rw-   0        0        0    10092 2021-04-14 09:24:28.000000 spine_items-0.9.0/spine_items/exporter/ui/exporter_properties.py
+-rw-rw-rw-   0        0        0    25724 2021-06-11 13:28:56.000000 spine_items-0.9.0/spine_items/exporter/ui/specification_editor.py
+-rw-rw-rw-   0        0        0     4138 2021-06-11 13:28:56.000000 spine_items-0.9.0/spine_items/exporter/ui/value_type_filter_editor.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.112365 spine_items-0.9.0/spine_items/exporter/widgets/
+-rw-rw-rw-   0        0        0      975 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2176 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/widgets/add_exporter_widget.py
+-rw-rw-rw-   0        0        0     2689 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/widgets/export_list_item.py
+-rw-rw-rw-   0        0        0     1892 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/widgets/exporter_properties.py
+-rw-rw-rw-   0        0        0     3540 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/widgets/filter_edit_delegate.py
+-rw-rw-rw-   0        0        0     3514 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/widgets/position_edit_delegate.py
+-rw-rw-rw-   0        0        0    22596 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/exporter/widgets/preview_updater.py
+-rw-rw-rw-   0        0        0    44323 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/exporter/widgets/specification_editor_window.py
+-rw-rw-rw-   0        0        0     1255 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/exporter/widgets/specification_menu.py
+-rw-rw-rw-   0        0        0     5978 2021-09-08 12:09:13.000000 spine_items-0.9.0/spine_items/exporter_executable_item_base.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.179086 spine_items-0.9.0/spine_items/gdx_exporter/
+-rw-rw-rw-   0        0        0     1071 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2342 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/gdx_exporter/commands.py
+-rw-rw-rw-   0        0        0     3212 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/gdx_exporter/do_work.py
+-rw-rw-rw-   0        0        0     5700 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/gdx_exporter/executable_item.py
+-rw-rw-rw-   0        0        0    15635 2021-06-08 11:40:38.000000 spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter.py
+-rw-rw-rw-   0        0        0     2636 2021-06-08 11:40:38.000000 spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter_factory.py
+-rw-rw-rw-   0        0        0     2205 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter_icon.py
+-rw-rw-rw-   0        0        0     1389 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/item_info.py
+-rw-rw-rw-   0        0        0     2880 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/list_utils.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.212315 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/
+-rw-rw-rw-   0        0        0     1100 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     2515 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/domain_name_list_model.py
+-rw-rw-rw-   0        0        0     9541 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/indexing_domain_list_model.py
+-rw-rw-rw-   0        0        0     9125 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/indexing_table_model.py
+-rw-rw-rw-   0        0        0     4591 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/parameter_name_list_model.py
+-rw-rw-rw-   0        0        0     4188 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/record_list_model.py
+-rw-rw-rw-   0        0        0    12084 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/set_list_model.py
+-rw-rw-rw-   0        0        0     4379 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/gdx_exporter/settings_pack.py
+-rw-rw-rw-   0        0        0     1471 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/settings_state.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.267291 spine_items-0.9.0/spine_items/gdx_exporter/ui/
+-rw-rw-rw-   0        0        0     1077 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/__init__.py
+-rw-rw-rw-   0        0        0    13418 2021-02-12 13:06:54.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/gdx_export_settings.py
+-rw-rw-rw-   0        0        0     8205 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/gdx_exporter_properties.py
+-rw-rw-rw-   0        0        0     7479 2021-02-12 13:06:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_index_settings.py
+-rw-rw-rw-   0        0        0     9584 2021-02-12 13:06:57.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_index_settings_window.py
+-rw-rw-rw-   0        0        0     8779 2021-02-12 13:06:58.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_merging_settings.py
+-rw-rw-rw-   0        0        0     3973 2021-02-12 13:07:00.000000 spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_merging_settings_window.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.312470 spine_items-0.9.0/spine_items/gdx_exporter/widgets/
+-rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2168 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/add_gdx_exporter_widget.py
+-rw-rw-rw-   0        0        0    18380 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/gdx_export_settings.py
+-rw-rw-rw-   0        0        0     1818 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/gdx_exporter_properties.py
+-rw-rw-rw-   0        0        0     1354 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/merging_error_flag.py
+-rw-rw-rw-   0        0        0    11414 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_index_settings.py
+-rw-rw-rw-   0        0        0    19686 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_index_settings_window.py
+-rw-rw-rw-   0        0        0     9888 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_merging_settings.py
+-rw-rw-rw-   0        0        0    10120 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_merging_settings_window.py
+-rw-rw-rw-   0        0        0     6698 2021-02-15 13:26:55.000000 spine_items-0.9.0/spine_items/gdx_exporter/worker.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.375932 spine_items-0.9.0/spine_items/gimlet/
+-rw-rw-rw-   0        0        0     1068 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/__init__.py
+-rw-rw-rw-   0        0        0     4010 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/commands.py
+-rw-rw-rw-   0        0        0     9301 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/gimlet/executable_item.py
+-rw-rw-rw-   0        0        0    17343 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/gimlet/gimlet.py
+-rw-rw-rw-   0        0        0     2467 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/gimlet/gimlet_factory.py
+-rw-rw-rw-   0        0        0     1499 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/gimlet/gimlet_icon.py
+-rw-rw-rw-   0        0        0     1376 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/item_info.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.389986 spine_items-0.9.0/spine_items/gimlet/ui/
+-rw-rw-rw-   0        0        0     1090 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/ui/__init__.py
+-rw-rw-rw-   0        0        0    13242 2021-04-14 09:24:29.000000 spine_items-0.9.0/spine_items/gimlet/ui/gimlet_properties.py
+-rw-rw-rw-   0        0        0     1146 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/utils.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.396075 spine_items-0.9.0/spine_items/gimlet/widgets/
+-rw-rw-rw-   0        0        0     1077 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2170 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/gimlet/widgets/add_gimlet_widget.py
+-rw-rw-rw-   0        0        0     1760 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0     1927 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/gimlet/widgets/gimlet_properties_widget.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.446062 spine_items-0.9.0/spine_items/importer/
+-rw-rw-rw-   0        0        0     1052 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/__init__.py
+-rw-rw-rw-   0        0        0    30568 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/importer/commands.py
+-rw-rw-rw-   0        0        0    14703 2021-06-11 08:51:27.000000 spine_items-0.9.0/spine_items/importer/connection_manager.py
+-rw-rw-rw-   0        0        0     6770 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/do_work.py
+-rw-rw-rw-   0        0        0     6325 2021-04-27 13:18:58.000000 spine_items-0.9.0/spine_items/importer/executable_item.py
+-rw-rw-rw-   0        0        0    16537 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/importer/importer.py
+-rw-rw-rw-   0        0        0     2708 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/importer/importer_factory.py
+-rw-rw-rw-   0        0        0     2222 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/importer/importer_icon.py
+-rw-rw-rw-   0        0        0     3579 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/importer_specification.py
+-rw-rw-rw-   0        0        0     1383 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/item_info.py
+-rw-rw-rw-   0        0        0     1158 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/mapping_colors.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.479410 spine_items-0.9.0/spine_items/importer/mvcmodels/
+-rw-rw-rw-   0        0        0     1076 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     6591 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/mvcmodels/mapping_list_model.py
+-rw-rw-rw-   0        0        0    40090 2021-08-25 05:49:43.000000 spine_items-0.9.0/spine_items/importer/mvcmodels/mapping_specification_model.py
+-rw-rw-rw-   0        0        0    14920 2021-06-11 08:51:27.000000 spine_items-0.9.0/spine_items/importer/mvcmodels/source_data_table_model.py
+-rw-rw-rw-   0        0        0     7780 2021-04-23 13:26:19.000000 spine_items-0.9.0/spine_items/importer/mvcmodels/source_table_list_model.py
+-rw-rw-rw-   0        0        0     1719 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/specification_factory.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.512693 spine_items-0.9.0/spine_items/importer/ui/
+-rw-rw-rw-   0        0        0     1089 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/ui/__init__.py
+-rw-rw-rw-   0        0        0    23336 2021-06-10 15:00:05.000000 spine_items-0.9.0/spine_items/importer/ui/import_editor_window.py
+-rw-rw-rw-   0        0        0     9603 2021-04-14 09:24:30.000000 spine_items-0.9.0/spine_items/importer/ui/importer_properties.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.579419 spine_items-0.9.0/spine_items/importer/widgets/
+-rw-rw-rw-   0        0        0     1076 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/importer/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2181 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/importer/widgets/add_importer_widget.py
+-rw-rw-rw-   0        0        0     5057 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0    17132 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/importer/widgets/import_editor_window.py
+-rw-rw-rw-   0        0        0    27561 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/importer/widgets/import_mapping_options.py
+-rw-rw-rw-   0        0        0    12835 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/importer/widgets/import_mappings.py
+-rw-rw-rw-   0        0        0    19706 2021-06-29 14:12:36.000000 spine_items-0.9.0/spine_items/importer/widgets/import_sources.py
+-rw-rw-rw-   0        0        0     3291 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/widgets/importer_properties_widget.py
+-rw-rw-rw-   0        0        0     2078 2021-04-23 13:26:19.000000 spine_items-0.9.0/spine_items/importer/widgets/multi_checkable_tree_view.py
+-rw-rw-rw-   0        0        0    10657 2021-04-12 13:56:32.000000 spine_items-0.9.0/spine_items/importer/widgets/options_widget.py
+-rw-rw-rw-   0        0        0    20858 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/importer/widgets/table_view_with_button_header.py
+-rw-rw-rw-   0        0        0    14744 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/item_base.py
+-rw-rw-rw-   0        0        0    24075 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/models.py
+-rw-rw-rw-   0        0        0   114515 2021-08-20 08:29:28.000000 spine_items-0.9.0/spine_items/resources_icons_rc.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.662604 spine_items-0.9.0/spine_items/tool/
+-rw-rw-rw-   0        0        0     1048 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/tool/__init__.py
+-rw-rw-rw-   0        0        0     2542 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/tool/commands.py
+-rw-rw-rw-   0        0        0    32856 2021-08-25 05:49:43.000000 spine_items-0.9.0/spine_items/tool/executable_item.py
+-rw-rw-rw-   0        0        0     1371 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/tool/item_info.py
+-rw-rw-rw-   0        0        0     2772 2021-04-12 13:56:33.000000 spine_items-0.9.0/spine_items/tool/output_resources.py
+-rw-rw-rw-   0        0        0     1686 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/tool/specification_factory.py
+-rw-rw-rw-   0        0        0    26258 2021-07-02 16:09:40.000000 spine_items-0.9.0/spine_items/tool/tool.py
+-rw-rw-rw-   0        0        0     4339 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/tool/tool_factory.py
+-rw-rw-rw-   0        0        0     3995 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/tool/tool_icon.py
+-rw-rw-rw-   0        0        0    11781 2021-09-03 07:14:07.000000 spine_items-0.9.0/spine_items/tool/tool_instance.py
+-rw-rw-rw-   0        0        0    24378 2021-08-18 12:14:10.000000 spine_items-0.9.0/spine_items/tool/tool_specifications.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.696065 spine_items-0.9.0/spine_items/tool/ui/
+-rw-rw-rw-   0        0        0     1085 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/tool/ui/__init__.py
+-rw-rw-rw-   0        0        0     9674 2021-02-12 13:07:05.000000 spine_items-0.9.0/spine_items/tool/ui/add_tool.py
+-rw-rw-rw-   0        0        0     5269 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/tool/ui/julia_options.py
+-rw-rw-rw-   0        0        0     8932 2021-08-27 13:58:22.000000 spine_items-0.9.0/spine_items/tool/ui/python_kernel_spec_options.py
+-rw-rw-rw-   0        0        0    16410 2021-08-20 08:29:27.000000 spine_items-0.9.0/spine_items/tool/ui/tool_properties.py
+-rw-rw-rw-   0        0        0    23514 2021-08-20 08:29:27.000000 spine_items-0.9.0/spine_items/tool/ui/tool_specification_form.py
+-rw-rw-rw-   0        0        0     5061 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/tool/utils.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.729360 spine_items-0.9.0/spine_items/tool/widgets/
+-rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/tool/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2197 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/tool/widgets/add_tool_widget.py
+-rw-rw-rw-   0        0        0     3941 2021-04-12 13:56:33.000000 spine_items-0.9.0/spine_items/tool/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0     5842 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/tool/widgets/main_program_text_edit.py
+-rw-rw-rw-   0        0        0    17495 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/tool/widgets/options_widgets.py
+-rw-rw-rw-   0        0        0     2005 2021-06-23 14:51:54.000000 spine_items-0.9.0/spine_items/tool/widgets/tool_properties_widget.py
+-rw-rw-rw-   0        0        0    10293 2021-08-09 14:40:32.000000 spine_items-0.9.0/spine_items/tool/widgets/tool_spec_optional_widgets.py
+-rw-rw-rw-   0        0        0    55784 2021-09-03 07:14:07.000000 spine_items-0.9.0/spine_items/tool/widgets/tool_specification_editor_window.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.745990 spine_items-0.9.0/spine_items/ui/
+-rw-rw-rw-   0        0        0     1090 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/ui/__init__.py
+-rw-rw-rw-   0        0        0    11592 2021-09-08 12:09:13.000000 spine_items-0.9.0/spine_items/utils.py
+-rw-rw-rw-   0        0        0     1054 2021-09-08 10:47:58.000000 spine_items-0.9.0/spine_items/version.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.779374 spine_items-0.9.0/spine_items/view/
+-rw-rw-rw-   0        0        0     1048 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/__init__.py
+-rw-rw-rw-   0        0        0     1583 2021-04-27 13:18:58.000000 spine_items-0.9.0/spine_items/view/executable_item.py
+-rw-rw-rw-   0        0        0     1371 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/item_info.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.796124 spine_items-0.9.0/spine_items/view/ui/
+-rw-rw-rw-   0        0        0     1085 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/ui/__init__.py
+-rw-rw-rw-   0        0        0     7810 2021-02-15 09:22:32.000000 spine_items-0.9.0/spine_items/view/ui/view_properties.py
+-rw-rw-rw-   0        0        0     7315 2021-05-25 09:51:15.000000 spine_items-0.9.0/spine_items/view/view.py
+-rw-rw-rw-   0        0        0     2426 2021-04-21 09:41:14.000000 spine_items-0.9.0/spine_items/view/view_factory.py
+-rw-rw-rw-   0        0        0     1508 2021-04-19 13:01:13.000000 spine_items-0.9.0/spine_items/view/view_icon.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:44.812797 spine_items-0.9.0/spine_items/view/widgets/
+-rw-rw-rw-   0        0        0     1072 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1948 2021-06-04 14:34:51.000000 spine_items-0.9.0/spine_items/view/widgets/add_view_widget.py
+-rw-rw-rw-   0        0        0     1774 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0     3007 2021-01-15 07:37:17.000000 spine_items-0.9.0/spine_items/view/widgets/view_properties_widget.py
+-rw-rw-rw-   0        0        0     5586 2021-04-27 13:13:28.000000 spine_items-0.9.0/spine_items/widgets.py
+drwxrwxrwx   0        0        0        0 2021-09-08 12:31:43.595840 spine_items-0.9.0/spine_items.egg-info/
+-rw-rw-rw-   0        0        0     2131 2021-09-08 12:31:43.000000 spine_items-0.9.0/spine_items.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10617 2021-09-08 12:31:43.000000 spine_items-0.9.0/spine_items.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-08 12:31:43.000000 spine_items-0.9.0/spine_items.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-03 11:44:47.000000 spine_items-0.9.0/spine_items.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      167 2021-09-08 12:31:43.000000 spine_items-0.9.0/spine_items.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-09-08 12:31:43.000000 spine_items-0.9.0/spine_items.egg-info/top_level.txt
```

### Comparing `spine_items-0.8.0/COPYING` & `spine_items-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/COPYING.LESSER` & `spine_items-0.9.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/PKG-INFO` & `spine_items-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spine_items
-Version: 0.8.0
+Version: 0.9.0
 Summary: Spine project items
 Home-page: https://github.com/Spine-project/spine-items
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.9,>=3.6
+Requires-Python: <3.9,>=3.7.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 # Spine Items
 
 [![Python](https://img.shields.io/badge/python-3.7%20|%203.8-blue.svg)](https://www.python.org/downloads/release/python-379/)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: spine_items Version: 0.8.0 Summary: Spine project
+Metadata-Version: 2.1 Name: spine_items Version: 0.9.0 Summary: Spine project
 items Home-page: https://github.com/Spine-project/spine-items Author: Spine
 Project consortium Author-email: spine_info@vtt.fi License: LGPL-3.0-or-later
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: <3.9,>=3.6
+Classifier: Operating System :: OS Independent Requires-Python: <3.9,>=3.7.1
 Description-Content-Type: text/markdown License-File: COPYING License-File:
 COPYING.LESSER # Spine Items [![Python](https://img.shields.io/badge/python-
 3.7%20|%203.8-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Unit tests](https://github.com/Spine-project/spine-items/workflows/
 Unit%20tests/badge.svg)](https://github.com/Spine-project/spine-items/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/Spine-
 project/spine-items/branch/master/graph/badge.svg)](https://codecov.io/gh/
```

### Comparing `spine_items-0.8.0/README.md` & `spine_items-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/setup.cfg` & `spine_items-0.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -31,22 +31,31 @@
 000001e0: 2028 4c47 504c 7633 290d 0a09 4f70 6572   (LGPLv3)...Oper
 000001f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
 00000200: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
 00000210: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
 00000220: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a7a  kages = find:..z
 00000230: 6970 5f73 6166 6520 3d20 4661 6c73 650d  ip_safe = False.
 00000240: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000250: 7320 3d20 0d0a 0973 7069 6e65 6462 5f61  s = ...spinedb_a
-00000260: 7069 203d 3d20 302e 3133 2e30 0d0a 0973  pi == 0.13.0...s
-00000270: 7069 6e65 5f65 6e67 696e 6520 3d3d 2030  pine_engine == 0
-00000280: 2e31 312e 300d 0a09 7370 696e 6574 6f6f  .11.0...spinetoo
-00000290: 6c62 6f78 203d 3d20 302e 362e 330d 0a69  lbox == 0.6.3..i
-000002a0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-000002b0: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
-000002c0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000002d0: 332e 362c 203c 332e 390d 0a0d 0a5b 6f70  3.6, <3.9....[op
-000002e0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002f0: 696e 645d 0d0a 6578 636c 7564 6520 3d20  ind]..exclude = 
-00000300: 7465 7374 732c 2074 6573 7473 2e2a 0d0a  tests, tests.*..
-00000310: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000320: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000330: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000250: 7320 3d20 0d0a 0970 7973 6964 6532 203e  s = ...pyside2 >
+00000260: 3d20 352e 3134 2c20 3c20 352e 3135 0d0a  = 5.14, < 5.15..
+00000270: 0970 796f 6462 6320 3e3d 2034 2e30 2c20  .pyodbc >= 4.0, 
+00000280: 3c20 342e 310d 0a09 7371 6c61 6c63 6865  < 4.1...sqlalche
+00000290: 6d79 203e 3d20 312e 332c 203c 2031 2e34  my >= 1.3, < 1.4
+000002a0: 0d0a 0970 7967 6d65 6e74 7320 3e3d 2032  ...pygments >= 2
+000002b0: 2e38 2c20 3c20 322e 3131 0d0a 096e 756d  .8, < 2.11...num
+000002c0: 7079 203e 3d20 312e 3230 2e32 2c20 3c20  py >= 1.20.2, < 
+000002d0: 312e 3232 0d0a 0973 7069 6e65 6462 5f61  1.22...spinedb_a
+000002e0: 7069 203e 3d20 302e 3134 2c20 3c20 302e  pi >= 0.14, < 0.
+000002f0: 3135 0d0a 0973 7069 6e65 5f65 6e67 696e  15...spine_engin
+00000300: 6520 3e3d 2030 2e31 322c 203c 2030 2e31  e >= 0.12, < 0.1
+00000310: 330d 0a09 7370 696e 6574 6f6f 6c62 6f78  3...spinetoolbox
+00000320: 203d 3d20 302e 362e 350d 0a69 6e63 6c75   == 0.6.5..inclu
+00000330: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000340: 3d20 5472 7565 0d0a 7079 7468 6f6e 5f72  = True..python_r
+00000350: 6571 7569 7265 7320 3d20 3e3d 332e 372e  equires = >=3.7.
+00000360: 312c 203c 332e 390d 0a0d 0a5b 6f70 7469  1, <3.9....[opti
+00000370: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000380: 645d 0d0a 6578 636c 7564 6520 3d20 7465  d]..exclude = te
+00000390: 7374 732c 2074 6573 7473 2e2a 0d0a 0d0a  sts, tests.*....
+000003a0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000003b0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000003c0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `spine_items-0.8.0/setup.py` & `spine_items-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/__init__.py` & `spine_items-0.9.0/spine_items/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/animations.py` & `spine_items-0.9.0/spine_items/animations.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/category.py` & `spine_items-0.9.0/spine_items/category.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/commands.py` & `spine_items-0.9.0/spine_items/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/__init__.py` & `spine_items-0.9.0/spine_items/data_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/commands.py` & `spine_items-0.9.0/spine_items/data_connection/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/data_connection.py` & `spine_items-0.9.0/spine_items/data_connection/data_connection.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/data_connection_factory.py` & `spine_items-0.9.0/spine_items/data_connection/data_connection_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/data_connection_icon.py` & `spine_items-0.9.0/spine_items/data_connection/data_connection_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/executable_item.py` & `spine_items-0.9.0/spine_items/data_connection/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/item_info.py` & `spine_items-0.9.0/spine_items/data_connection/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/output_resources.py` & `spine_items-0.9.0/spine_items/data_connection/output_resources.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/ui/__init__.py` & `spine_items-0.9.0/spine_items/data_connection/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/ui/data_connection_properties.py` & `spine_items-0.9.0/spine_items/data_connection/ui/data_connection_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/widgets/__init__.py` & `spine_items-0.9.0/spine_items/data_connection/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/widgets/add_data_connection_widget.py` & `spine_items-0.9.0/spine_items/data_connection/widgets/add_data_connection_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/widgets/custom_menus.py` & `spine_items-0.9.0/spine_items/data_connection/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_connection/widgets/data_connection_properties_widget.py` & `spine_items-0.9.0/spine_items/data_connection/widgets/data_connection_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/__init__.py` & `spine_items-0.9.0/spine_items/data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/commands.py` & `spine_items-0.9.0/spine_items/data_store/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/data_store.py` & `spine_items-0.9.0/spine_items/data_store/data_store.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/data_store_factory.py` & `spine_items-0.9.0/spine_items/data_store/data_store_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/data_store_icon.py` & `spine_items-0.9.0/spine_items/data_store/data_store_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/do_work.py` & `spine_items-0.9.0/spine_items/data_store/do_work.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/executable_item.py` & `spine_items-0.9.0/spine_items/data_store/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/item_info.py` & `spine_items-0.9.0/spine_items/data_store/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/output_resources.py` & `spine_items-0.9.0/spine_items/data_store/output_resources.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/ui/__init__.py` & `spine_items-0.9.0/spine_items/data_store/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/ui/data_store_properties.py` & `spine_items-0.9.0/spine_items/data_store/ui/data_store_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/utils.py` & `spine_items-0.9.0/spine_items/data_store/utils.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/widgets/__init__.py` & `spine_items-0.9.0/spine_items/data_store/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/widgets/add_data_store_widget.py` & `spine_items-0.9.0/spine_items/data_store/widgets/add_data_store_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_store/widgets/data_store_properties_widget.py` & `spine_items-0.9.0/spine_items/data_store/widgets/data_store_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/__init__.py` & `spine_items-0.9.0/spine_items/data_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/commands.py` & `spine_items-0.9.0/spine_items/data_transformer/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/data_transformer.py` & `spine_items-0.9.0/spine_items/data_transformer/data_transformer.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/data_transformer_factory.py` & `spine_items-0.9.0/spine_items/data_transformer/data_transformer_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/data_transformer_icon.py` & `spine_items-0.9.0/spine_items/data_transformer/data_transformer_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/data_transformer_specification.py` & `spine_items-0.9.0/spine_items/data_transformer/data_transformer_specification.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/executable_item.py` & `spine_items-0.9.0/spine_items/data_transformer/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/filter_config_path.py` & `spine_items-0.9.0/spine_items/data_transformer/filter_config_path.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/item_info.py` & `spine_items-0.9.0/spine_items/data_transformer/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/mvcmodels/__init__.py` & `spine_items-0.9.0/spine_items/data_transformer/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/mvcmodels/class_renames_table_model.py` & `spine_items-0.9.0/spine_items/data_transformer/mvcmodels/class_renames_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/mvcmodels/parameter_drop_target_table_model.py` & `spine_items-0.9.0/spine_items/data_transformer/mvcmodels/parameter_drop_target_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/mvcmodels/parameter_renames_table_model.py` & `spine_items-0.9.0/spine_items/data_transformer/mvcmodels/parameter_renames_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/mvcmodels/value_transformations_table_model.py` & `spine_items-0.9.0/spine_items/data_transformer/mvcmodels/value_transformations_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/output_resources.py` & `spine_items-0.9.0/spine_items/data_transformer/output_resources.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/settings.py` & `spine_items-0.9.0/spine_items/data_transformer/settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/specification_factory.py` & `spine_items-0.9.0/spine_items/data_transformer/specification_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/__init__.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/class_renamer_editor.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/class_renamer_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/data_transformer_properties.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/data_transformer_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/parameter_renamer_editor.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/parameter_renamer_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/specification_editor_widget.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/specification_editor_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/ui/value_transformer_editor.py` & `spine_items-0.9.0/spine_items/data_transformer/ui/value_transformer_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/__init__.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/add_data_transformer_widget.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/add_data_transformer_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/class_rename.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/class_rename.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/class_tree_widget.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/class_tree_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/copy_paste.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/copy_paste.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/data_transformer_properties_widget.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/data_transformer_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/drop_target_table.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/drop_target_table.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/instructions_editor.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/instructions_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/parameter_rename.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/parameter_rename.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/parameter_tree_widget.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/parameter_tree_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/specification_editor_window.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/data_transformer/widgets/value_transformation.py` & `spine_items-0.9.0/spine_items/data_transformer/widgets/value_transformation.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/__init__.py` & `spine_items-0.9.0/spine_items/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/commands.py` & `spine_items-0.9.0/spine_items/exporter/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/do_work.py` & `spine_items-0.9.0/spine_items/exporter/do_work.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/executable_item.py` & `spine_items-0.9.0/spine_items/exporter/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/exporter.py` & `spine_items-0.9.0/spine_items/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/exporter_factory.py` & `spine_items-0.9.0/spine_items/exporter/exporter_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/exporter_icon.py` & `spine_items-0.9.0/spine_items/exporter/exporter_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/item_info.py` & `spine_items-0.9.0/spine_items/exporter/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/__init__.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/mapping_editor_table_model.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/mapping_editor_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/mappings_table_model.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/mappings_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/mappings_table_proxy.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/mappings_table_proxy.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/preview_table_model.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/preview_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/mvcmodels/preview_tree_model.py` & `spine_items-0.9.0/spine_items/exporter/mvcmodels/preview_tree_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/preview_table_writer.py` & `spine_items-0.9.0/spine_items/exporter/preview_table_writer.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/specification.py` & `spine_items-0.9.0/spine_items/exporter/specification.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/specification_factory.py` & `spine_items-0.9.0/spine_items/exporter/specification_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/__init__.py` & `spine_items-0.9.0/spine_items/exporter/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/default_filter_editor.py` & `spine_items-0.9.0/spine_items/exporter/ui/default_filter_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/export_list_item.py` & `spine_items-0.9.0/spine_items/exporter/ui/export_list_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/exporter_properties.py` & `spine_items-0.9.0/spine_items/exporter/ui/exporter_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/specification_editor.py` & `spine_items-0.9.0/spine_items/exporter/ui/specification_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/ui/value_type_filter_editor.py` & `spine_items-0.9.0/spine_items/exporter/ui/value_type_filter_editor.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/__init__.py` & `spine_items-0.9.0/spine_items/exporter/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/add_exporter_widget.py` & `spine_items-0.9.0/spine_items/exporter/widgets/add_exporter_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/export_list_item.py` & `spine_items-0.9.0/spine_items/exporter/widgets/export_list_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/exporter_properties.py` & `spine_items-0.9.0/spine_items/exporter/widgets/exporter_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/filter_edit_delegate.py` & `spine_items-0.9.0/spine_items/exporter/widgets/filter_edit_delegate.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/position_edit_delegate.py` & `spine_items-0.9.0/spine_items/exporter/widgets/position_edit_delegate.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/preview_updater.py` & `spine_items-0.9.0/spine_items/exporter/widgets/preview_updater.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/specification_editor_window.py` & `spine_items-0.9.0/spine_items/exporter/widgets/specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter/widgets/specification_menu.py` & `spine_items-0.9.0/spine_items/exporter/widgets/specification_menu.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/exporter_executable_item_base.py` & `spine_items-0.9.0/spine_items/exporter_executable_item_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,20 +11,24 @@
 
 """
 Contains base classes for executable items.
 
 :authors: A. Soininen (VTT)
 :date:    10.2.2021
 """
+import json
 import os.path
+from pathlib import Path
+
+from spine_engine.project_item.project_item_resource import file_resource_in_pack
 from spinedb_api import clear_filter_configs, load_filters
 from spinedb_api.filters.tools import filter_configs, name_from_dict
 from spinedb_api.spine_io import gdx_utils
 from spine_engine.project_item.executable_item_base import ExecutableItemBase
-from .utils import exported_files_as_resources
+from .utils import exported_files_as_resources, EXPORTER_EXECUTION_MANIFEST_FILE_PREFIX
 
 
 class ExporterExecutableItemBase(ExecutableItemBase):
     """Base class for exporter executable items."""
 
     def __init__(self, name, databases, output_time_stamps, cancel_on_error, gams_path, project_dir, logger):
         """
@@ -56,17 +60,25 @@
         super().stop_execution()
         if self._process is not None:
             self._process.terminate()
             self._process = None
 
     def exclude_execution(self, forward_resources, backward_resources):
         """See base class."""
-        database_urls = [r.url for r in forward_resources if r.type_ == "database"]
-        _, forks = self._databases_and_forks(database_urls)
-        self._forks.update(forks)
+        manifest_file_name = (
+            (EXPORTER_EXECUTION_MANIFEST_FILE_PREFIX + self.filter_id)
+            if self.filter_id
+            else EXPORTER_EXECUTION_MANIFEST_FILE_PREFIX
+        ) + ".json"
+        manifest_file_path = Path(self._data_dir, manifest_file_name)
+        if not manifest_file_path.exists():
+            return
+        with open(Path(self._data_dir, manifest_file_name)) as manifest_file:
+            manifest = json.load(manifest_file)
+        self._result_files = {label: set(files) for label, files in manifest.items()}
 
     def _databases_and_forks(self, database_urls):
         """
         Connects output file names to scenario and tool filters.
 
         Args:
             database_urls (Iterable of str): database URLs.
@@ -94,17 +106,19 @@
                 filter_name = name_from_dict(config)
                 if filter_name is not None:
                     forks[url].append(filter_name)
         return databases, forks
 
     def _output_resources_forward(self):
         """See base class."""
-        resources, self._result_files = exported_files_as_resources(
-            self.name, self._result_files, self._data_dir, self._databases
-        )
+        if self._result_files is None:
+            return []
+        resources = list()
+        for label, output_files in self._result_files.items():
+            resources += [file_resource_in_pack(self.name, label, f) for f in output_files]
         return resources
 
     def _resolve_gams_system_directory(self):
         """Returns GAMS system path from Toolbox settings or None if GAMS default is to be used.
 
         Returns:
             str: GAMS system path
```

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/__init__.py` & `spine_items-0.9.0/spine_items/gdx_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/commands.py` & `spine_items-0.9.0/spine_items/gdx_exporter/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/do_work.py` & `spine_items-0.9.0/spine_items/gdx_exporter/do_work.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/executable_item.py` & `spine_items-0.9.0/spine_items/gdx_exporter/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter.py` & `spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter_factory.py` & `spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/gdx_exporter_icon.py` & `spine_items-0.9.0/spine_items/gdx_exporter/gdx_exporter_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/item_info.py` & `spine_items-0.9.0/spine_items/gdx_exporter/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/list_utils.py` & `spine_items-0.9.0/spine_items/gdx_exporter/list_utils.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/__init__.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/domain_name_list_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/domain_name_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/indexing_domain_list_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/indexing_domain_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/indexing_table_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/indexing_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/parameter_name_list_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/parameter_name_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/record_list_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/record_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/mvcmodels/set_list_model.py` & `spine_items-0.9.0/spine_items/gdx_exporter/mvcmodels/set_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/settings_pack.py` & `spine_items-0.9.0/spine_items/gdx_exporter/settings_pack.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/settings_state.py` & `spine_items-0.9.0/spine_items/gdx_exporter/settings_state.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/__init__.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/gdx_export_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/gdx_export_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/gdx_exporter_properties.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/gdx_exporter_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_index_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_index_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_index_settings_window.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_index_settings_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_merging_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_merging_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/ui/parameter_merging_settings_window.py` & `spine_items-0.9.0/spine_items/gdx_exporter/ui/parameter_merging_settings_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/__init__.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/add_gdx_exporter_widget.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/add_gdx_exporter_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/gdx_export_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/gdx_export_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/gdx_exporter_properties.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/gdx_exporter_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/merging_error_flag.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/merging_error_flag.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_index_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_index_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_index_settings_window.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_index_settings_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_merging_settings.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_merging_settings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/widgets/parameter_merging_settings_window.py` & `spine_items-0.9.0/spine_items/gdx_exporter/widgets/parameter_merging_settings_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gdx_exporter/worker.py` & `spine_items-0.9.0/spine_items/gdx_exporter/worker.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/__init__.py` & `spine_items-0.9.0/spine_items/gimlet/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/commands.py` & `spine_items-0.9.0/spine_items/gimlet/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/executable_item.py` & `spine_items-0.9.0/spine_items/gimlet/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/gimlet.py` & `spine_items-0.9.0/spine_items/gimlet/gimlet.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/gimlet_factory.py` & `spine_items-0.9.0/spine_items/gimlet/gimlet_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/gimlet_icon.py` & `spine_items-0.9.0/spine_items/gimlet/gimlet_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/item_info.py` & `spine_items-0.9.0/spine_items/gimlet/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/ui/__init__.py` & `spine_items-0.9.0/spine_items/gimlet/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/ui/gimlet_properties.py` & `spine_items-0.9.0/spine_items/gimlet/ui/gimlet_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/utils.py` & `spine_items-0.9.0/spine_items/gimlet/utils.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/widgets/__init__.py` & `spine_items-0.9.0/spine_items/gimlet/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/widgets/add_gimlet_widget.py` & `spine_items-0.9.0/spine_items/gimlet/widgets/add_gimlet_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/widgets/custom_menus.py` & `spine_items-0.9.0/spine_items/gimlet/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/gimlet/widgets/gimlet_properties_widget.py` & `spine_items-0.9.0/spine_items/gimlet/widgets/gimlet_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/__init__.py` & `spine_items-0.9.0/spine_items/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/commands.py` & `spine_items-0.9.0/spine_items/importer/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/connection_manager.py` & `spine_items-0.9.0/spine_items/importer/connection_manager.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/do_work.py` & `spine_items-0.9.0/spine_items/importer/do_work.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/executable_item.py` & `spine_items-0.9.0/spine_items/importer/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/importer.py` & `spine_items-0.9.0/spine_items/importer/importer.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/importer_factory.py` & `spine_items-0.9.0/spine_items/importer/importer_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/importer_icon.py` & `spine_items-0.9.0/spine_items/importer/importer_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/importer_specification.py` & `spine_items-0.9.0/spine_items/importer/importer_specification.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/item_info.py` & `spine_items-0.9.0/spine_items/importer/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mapping_colors.py` & `spine_items-0.9.0/spine_items/importer/mapping_colors.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mvcmodels/__init__.py` & `spine_items-0.9.0/spine_items/importer/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mvcmodels/mapping_list_model.py` & `spine_items-0.9.0/spine_items/importer/mvcmodels/mapping_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mvcmodels/mapping_specification_model.py` & `spine_items-0.9.0/spine_items/importer/mvcmodels/mapping_specification_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mvcmodels/source_data_table_model.py` & `spine_items-0.9.0/spine_items/importer/mvcmodels/source_data_table_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/mvcmodels/source_table_list_model.py` & `spine_items-0.9.0/spine_items/importer/mvcmodels/source_table_list_model.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/specification_factory.py` & `spine_items-0.9.0/spine_items/importer/specification_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/ui/__init__.py` & `spine_items-0.9.0/spine_items/importer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/ui/import_editor_window.py` & `spine_items-0.9.0/spine_items/importer/ui/import_editor_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/ui/importer_properties.py` & `spine_items-0.9.0/spine_items/importer/ui/importer_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/__init__.py` & `spine_items-0.9.0/spine_items/importer/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/add_importer_widget.py` & `spine_items-0.9.0/spine_items/importer/widgets/add_importer_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/custom_menus.py` & `spine_items-0.9.0/spine_items/importer/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/import_editor_window.py` & `spine_items-0.9.0/spine_items/importer/widgets/import_editor_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/import_mapping_options.py` & `spine_items-0.9.0/spine_items/importer/widgets/import_mapping_options.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/import_mappings.py` & `spine_items-0.9.0/spine_items/importer/widgets/import_mappings.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/import_sources.py` & `spine_items-0.9.0/spine_items/importer/widgets/import_sources.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/importer_properties_widget.py` & `spine_items-0.9.0/spine_items/importer/widgets/importer_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/multi_checkable_tree_view.py` & `spine_items-0.9.0/spine_items/importer/widgets/multi_checkable_tree_view.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/options_widget.py` & `spine_items-0.9.0/spine_items/importer/widgets/options_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/importer/widgets/table_view_with_button_header.py` & `spine_items-0.9.0/spine_items/importer/widgets/table_view_with_button_header.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/item_base.py` & `spine_items-0.9.0/spine_items/item_base.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/models.py` & `spine_items-0.9.0/spine_items/models.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/resources_icons_rc.py` & `spine_items-0.9.0/spine_items/resources_icons_rc.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/__init__.py` & `spine_items-0.9.0/spine_items/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/commands.py` & `spine_items-0.9.0/spine_items/tool/commands.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/executable_item.py` & `spine_items-0.9.0/spine_items/tool/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/item_info.py` & `spine_items-0.9.0/spine_items/tool/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/output_resources.py` & `spine_items-0.9.0/spine_items/tool/output_resources.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/specification_factory.py` & `spine_items-0.9.0/spine_items/tool/specification_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/tool.py` & `spine_items-0.9.0/spine_items/tool/tool.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/tool_factory.py` & `spine_items-0.9.0/spine_items/tool/tool_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/tool_icon.py` & `spine_items-0.9.0/spine_items/tool/tool_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/tool_instance.py` & `spine_items-0.9.0/spine_items/tool/tool_instance.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/tool_specifications.py` & `spine_items-0.9.0/spine_items/tool/tool_specifications.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/__init__.py` & `spine_items-0.9.0/spine_items/tool/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/add_tool.py` & `spine_items-0.9.0/spine_items/tool/ui/add_tool.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/julia_options.py` & `spine_items-0.9.0/spine_items/tool/ui/julia_options.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/python_kernel_spec_options.py` & `spine_items-0.9.0/spine_items/tool/ui/python_kernel_spec_options.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/tool_properties.py` & `spine_items-0.9.0/spine_items/tool/ui/tool_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/ui/tool_specification_form.py` & `spine_items-0.9.0/spine_items/tool/ui/tool_specification_form.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/utils.py` & `spine_items-0.9.0/spine_items/tool/utils.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/__init__.py` & `spine_items-0.9.0/spine_items/tool/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/add_tool_widget.py` & `spine_items-0.9.0/spine_items/tool/widgets/add_tool_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/custom_menus.py` & `spine_items-0.9.0/spine_items/tool/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/main_program_text_edit.py` & `spine_items-0.9.0/spine_items/tool/widgets/main_program_text_edit.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/options_widgets.py` & `spine_items-0.9.0/spine_items/tool/widgets/options_widgets.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/tool_properties_widget.py` & `spine_items-0.9.0/spine_items/tool/widgets/tool_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/tool_spec_optional_widgets.py` & `spine_items-0.9.0/spine_items/tool/widgets/tool_spec_optional_widgets.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/tool/widgets/tool_specification_editor_window.py` & `spine_items-0.9.0/spine_items/tool/widgets/tool_specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/ui/__init__.py` & `spine_items-0.9.0/spine_items/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/utils.py` & `spine_items-0.9.0/spine_items/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,14 @@
         dict: mapping from output label to list of file paths, or None if no manifest files were found
     """
     manifests = None
     for path in Path(data_dir).iterdir():
         if path.name.startswith(EXPORTER_EXECUTION_MANIFEST_FILE_PREFIX) and path.suffix == ".json":
             with open(path) as manifest_file:
                 manifest = json.load(manifest_file)
-            path.unlink()
             for out_file_name, paths in manifest.items():
                 if manifests is None:
                     manifests = dict()
                 path_list = manifests.setdefault(out_file_name, list())
                 path_list += paths
     return manifests
```

### Comparing `spine_items-0.8.0/spine_items/version.py` & `spine_items-0.9.0/spine_items/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 # Spine Items is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 # NOTE: Required other package versions in setup.cfg
```

### Comparing `spine_items-0.8.0/spine_items/view/__init__.py` & `spine_items-0.9.0/spine_items/view/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/executable_item.py` & `spine_items-0.9.0/spine_items/view/executable_item.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/item_info.py` & `spine_items-0.9.0/spine_items/view/item_info.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/ui/__init__.py` & `spine_items-0.9.0/spine_items/view/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/ui/view_properties.py` & `spine_items-0.9.0/spine_items/view/ui/view_properties.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/view.py` & `spine_items-0.9.0/spine_items/view/view.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/view_factory.py` & `spine_items-0.9.0/spine_items/view/view_factory.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/view_icon.py` & `spine_items-0.9.0/spine_items/view/view_icon.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/widgets/__init__.py` & `spine_items-0.9.0/spine_items/view/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/widgets/add_view_widget.py` & `spine_items-0.9.0/spine_items/view/widgets/add_view_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/widgets/custom_menus.py` & `spine_items-0.9.0/spine_items/view/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/view/widgets/view_properties_widget.py` & `spine_items-0.9.0/spine_items/view/widgets/view_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items/widgets.py` & `spine_items-0.9.0/spine_items/widgets.py`

 * *Files identical despite different names*

### Comparing `spine_items-0.8.0/spine_items.egg-info/PKG-INFO` & `spine_items-0.9.0/spine_items.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spine-items
-Version: 0.8.0
+Version: 0.9.0
 Summary: Spine project items
 Home-page: https://github.com/Spine-project/spine-items
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.9,>=3.6
+Requires-Python: <3.9,>=3.7.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 # Spine Items
 
 [![Python](https://img.shields.io/badge/python-3.7%20|%203.8-blue.svg)](https://www.python.org/downloads/release/python-379/)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: spine-items Version: 0.8.0 Summary: Spine project
+Metadata-Version: 2.1 Name: spine-items Version: 0.9.0 Summary: Spine project
 items Home-page: https://github.com/Spine-project/spine-items Author: Spine
 Project consortium Author-email: spine_info@vtt.fi License: LGPL-3.0-or-later
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: <3.9,>=3.6
+Classifier: Operating System :: OS Independent Requires-Python: <3.9,>=3.7.1
 Description-Content-Type: text/markdown License-File: COPYING License-File:
 COPYING.LESSER # Spine Items [![Python](https://img.shields.io/badge/python-
 3.7%20|%203.8-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Unit tests](https://github.com/Spine-project/spine-items/workflows/
 Unit%20tests/badge.svg)](https://github.com/Spine-project/spine-items/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/Spine-
 project/spine-items/branch/master/graph/badge.svg)](https://codecov.io/gh/
```

### Comparing `spine_items-0.8.0/spine_items.egg-info/SOURCES.txt` & `spine_items-0.9.0/spine_items.egg-info/SOURCES.txt`

 * *Files identical despite different names*

