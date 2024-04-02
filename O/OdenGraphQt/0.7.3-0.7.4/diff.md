# Comparing `tmp/OdenGraphQt-0.7.3.tar.gz` & `tmp/OdenGraphQt-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OdenGraphQt-0.7.3.tar", last modified: Wed Feb 14 02:08:01 2024, max compression
+gzip compressed data, was "OdenGraphQt-0.7.4.tar", last modified: Tue Apr  2 10:05:51 2024, max compression
```

## Comparing `OdenGraphQt-0.7.3.tar` & `OdenGraphQt-0.7.4.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.973804 OdenGraphQt-0.7.3/
--rw-rw-rw-   0        0        0     1132 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/LICENSE.md
--rw-rw-rw-   0        0        0       49 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.935805 OdenGraphQt-0.7.3/OdenGraphQt/
--rw-rw-rw-   0        0        0     2507 2024-02-13 09:00:37.000000 OdenGraphQt-0.7.3/OdenGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.942805 OdenGraphQt-0.7.3/OdenGraphQt/base/
--rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    15872 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/factory.py
--rw-rw-rw-   0        0        0   106778 2024-02-14 02:03:13.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     9613 2024-02-13 10:01:22.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    22527 2024-02-13 09:48:55.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15557 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/node.py
--rw-rw-rw-   0        0        0    17810 2024-02-13 08:01:12.000000 OdenGraphQt-0.7.3/OdenGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7609 2024-02-14 02:03:12.000000 OdenGraphQt-0.7.3/OdenGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.944805 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0      699 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    12101 2024-02-13 08:52:11.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4809 2024-02-13 08:52:14.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.950805 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3608 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     5650 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_extra.py
--rw-rw-rw-   0        0        0     2471 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     5050 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6675 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2951 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2789 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    30753 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      763 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7357 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.954806 OdenGraphQt-0.7.3/OdenGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4674 2024-02-13 08:45:29.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    29668 2024-02-13 09:57:33.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5786 2024-02-13 08:27:07.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      156 2024-02-14 02:05:29.000000 OdenGraphQt-0.7.3/OdenGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.961805 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7467 2024-02-13 09:16:14.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    11550 2024-02-13 09:16:14.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    38059 2024-02-13 09:22:35.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21084 2024-02-13 08:47:24.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12528 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4287 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8227 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8226 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3875 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    23930 2024-02-13 08:16:26.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    14714 2024-02-05 05:25:56.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2950 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.966805 OdenGraphQt-0.7.3/OdenGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3959 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1875 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.967806 OdenGraphQt-0.7.3/OdenGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4552 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    19701 2024-02-13 09:57:33.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5383 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11833 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    62922 2024-02-13 08:49:29.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6983 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/OdenGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.972805 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/
--rw-rw-rw-   0        0        0     4082 2024-02-14 02:08:01.000000 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2024-02-14 02:08:01.000000 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 02:08:01.000000 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-02-14 02:08:01.000000 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-14 02:08:01.000000 OdenGraphQt-0.7.3/OdenGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4082 2024-02-14 02:08:01.973804 OdenGraphQt-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1782 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.929805 OdenGraphQt-0.7.3/examples/
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.968806 OdenGraphQt-0.7.3/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.3/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6316 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2024-02-14 02:08:01.972805 OdenGraphQt-0.7.3/examples/nodes/
--rw-rw-rw-   0        0        0        0 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.3/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2320 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3699 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.3/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     4633 2024-02-13 09:58:00.000000 OdenGraphQt-0.7.3/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1273 2024-01-24 05:16:41.000000 OdenGraphQt-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       26 2023-12-27 03:02:26.000000 OdenGraphQt-0.7.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 02:08:01.973804 OdenGraphQt-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.553547 OdenGraphQt-0.7.4/
+-rw-rw-rw-   0        0        0     1132 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.516547 OdenGraphQt-0.7.4/OdenGraphQt/
+-rw-rw-rw-   0        0        0     2507 2024-02-13 09:00:37.000000 OdenGraphQt-0.7.4/OdenGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.524548 OdenGraphQt-0.7.4/OdenGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    15872 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0   106883 2024-02-14 05:57:16.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     9613 2024-02-13 10:01:22.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    22527 2024-02-13 09:48:55.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15557 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    17810 2024-02-13 08:01:12.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     1225 2024-02-14 06:07:08.000000 OdenGraphQt-0.7.4/OdenGraphQt/base/types.py
+-rw-rw-rw-   0        0        0     7609 2024-02-14 02:03:12.000000 OdenGraphQt-0.7.4/OdenGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.526547 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0      699 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    12101 2024-02-13 08:52:11.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4809 2024-02-13 08:52:14.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.532547 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3608 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     5650 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_extra.py
+-rw-rw-rw-   0        0        0     2471 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     5050 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6675 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2951 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2789 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    30753 2024-02-14 01:49:48.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      763 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7357 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.535549 OdenGraphQt-0.7.4/OdenGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4674 2024-02-13 08:45:29.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    29668 2024-02-13 09:57:33.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5786 2024-02-13 08:27:07.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      156 2024-04-02 10:04:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.542547 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7467 2024-02-13 09:16:14.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    11550 2024-02-13 09:16:14.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    38059 2024-02-13 09:22:35.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21084 2024-02-13 08:47:24.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12528 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4287 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8227 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8226 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3875 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    23930 2024-02-13 08:16:26.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    14714 2024-02-05 05:25:56.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2950 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.548547 OdenGraphQt-0.7.4/OdenGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3959 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1875 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.548547 OdenGraphQt-0.7.4/OdenGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4552 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    19798 2024-02-14 02:53:52.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5383 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11833 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    62922 2024-02-13 08:49:29.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6983 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/OdenGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.552547 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     4123 2024-04-02 10:05:51.000000 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2024-04-02 10:05:51.000000 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:05:51.000000 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-02 10:05:51.000000 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 10:05:51.000000 OdenGraphQt-0.7.4/OdenGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4123 2024-04-02 10:05:51.553547 OdenGraphQt-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.510547 OdenGraphQt-0.7.4/examples/
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.549547 OdenGraphQt-0.7.4/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.4/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6316 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:05:51.552547 OdenGraphQt-0.7.4/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.4/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2320 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3699 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2024-01-24 05:06:49.000000 OdenGraphQt-0.7.4/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4633 2024-02-13 09:58:00.000000 OdenGraphQt-0.7.4/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1273 2024-02-14 05:42:11.000000 OdenGraphQt-0.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2024-02-14 06:14:57.000000 OdenGraphQt-0.7.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:05:51.553547 OdenGraphQt-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-12-22 04:10:35.000000 OdenGraphQt-0.7.4/setup.py
```

### Comparing `OdenGraphQt-0.7.3/LICENSE.md` & `OdenGraphQt-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/__init__.py` & `OdenGraphQt-0.7.4/OdenGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/commands.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/factory.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/graph.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     PortConnectedCmd,
 )
 from OdenGraphQt.base.factory import NodeFactory
 from OdenGraphQt.base.menu import NodeGraphMenu, NodesMenu
 from OdenGraphQt.base.model import NodeGraphModel
 from OdenGraphQt.base.node import NodeObject
 from OdenGraphQt.base.port import Port
+from OdenGraphQt.base.types import TSerializedData
 from OdenGraphQt.constants import (
     LayoutDirectionEnum,
     MIME_TYPE,
     PipeLayoutEnum,
     PortTypeEnum,
     URI_SCHEME,
     URN_SCHEME,
@@ -1736,26 +1737,26 @@
                     p.set_locked(False, connected_ports=False)
 
                 p.clear_connections()
 
         self._undo_stack.clear()
         self._model = NodeGraphModel()
 
-    def _serialize(self, nodes):
+    def _serialize(self, nodes) -> TSerializedData:
         """
         serialize nodes to a dict.
         (used internally by the node graph)
 
         Args:
             nodes (list[OdenGraphQt.Nodes]): list of node instances.
 
         Returns:
             dict: serialized data.
         """
-        serial_data = {'graph': {}, 'nodes': {}, 'connections': []}
+        serial_data: TSerializedData = {'graph': {}, 'nodes': {}, 'connections': []}
         nodes_data = {}
 
         # serialize graph session.
         serial_data['graph']['layout_direction'] = self.layout_direction()
         serial_data['graph']['acyclic'] = self.acyclic()
         serial_data['graph']['pipe_collision'] = self.pipe_collision()
         serial_data['graph']['pipe_slicing'] = self.pipe_slicing()
@@ -1801,15 +1802,15 @@
                             serial_data['connections'].append(pipe)
 
         if not serial_data['connections']:
             serial_data.pop('connections')
 
         return serial_data
 
-    def _deserialize(self, data, relative_pos=False, pos=None):
+    def _deserialize(self, data: TSerializedData, relative_pos=False, pos=None):
         """
         deserialize node data.
         (used internally by the node graph)
 
         Args:
             data (dict): node data.
             relative_pos (bool): position node relative to the cursor.
```

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/menu.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/model.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/node.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/base/port.py` & `OdenGraphQt-0.7.4/OdenGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/constants.py` & `OdenGraphQt-0.7.4/OdenGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/__init__.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/nodes_palette.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/nodes_tree.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_extra.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_extra.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `OdenGraphQt-0.7.4/OdenGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/nodes/backdrop_node.py` & `OdenGraphQt-0.7.4/OdenGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/nodes/base_node.py` & `OdenGraphQt-0.7.4/OdenGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/nodes/base_node_circle.py` & `OdenGraphQt-0.7.4/OdenGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/nodes/group_node.py` & `OdenGraphQt-0.7.4/OdenGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/nodes/port_node.py` & `OdenGraphQt-0.7.4/OdenGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_abstract.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_backdrop.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_base.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_circle.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_group.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_overlay_disabled.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_port_in.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_port_out.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/node_text_item.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/pipe.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/port.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/qgraphics/slicer.py` & `OdenGraphQt-0.7.4/OdenGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/actions.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/dialogs.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/icons/node_base.png` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/node_graph.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/node_widgets.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/node_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     def __init__(self, label: str, parent=None):
         super().__init__(parent)
         layout = QtWidgets.QVBoxLayout(self)
         layout.setSpacing(1)
         self.setTitle(label)
 
-    def setTitle(self, text):
+    def setTitle(self, text: str):
         margin = (0, 2, 0, 0) if text else (0, 0, 0, 0)
         self.layout().setContentsMargins(*margin)
         super().setTitle(text)
 
     def setTitleAlign(self, align='center'):
         text_color = tuple(
             map(
@@ -36,15 +36,15 @@
                 'padding-left': '1px',
                 'padding-right': '1px',
                 'font-size': '8pt',
             },
             'QGroupBox::title': {
                 'subcontrol-origin': 'margin',
                 'subcontrol-position': 'top center',
-                'color': 'rgba({0}, {1}, {2}, 100)'.format(*text_color),
+                'color': 'rgba({0}, {1}, {2}, 200)'.format(*text_color),
                 'padding': '0px',
             }
         }
 
         if self.title():
             style_dict['QGroupBox']['padding-top'] = '14px'
         else:
@@ -65,18 +65,18 @@
             for elm_name, elm_val in css.items():
                 style += '  {}:{};\n'.format(elm_name, elm_val)
             style += '}\n'
             stylesheet += style
 
         self.setStyleSheet(stylesheet)
 
-    def add_node_widget(self, widget):
+    def add_node_widget(self, widget: QtWidgets.QWidget):
         self.layout().addWidget(widget)
 
-    def get_node_widget(self):
+    def get_node_widget(self) -> QtWidgets.QWidget:
         return self.layout().itemAt(0).widget()
 
 
 class NodeBaseWidget(QtWidgets.QGraphicsProxyWidget):
     """
     This is the main wrapper class that allows a ``QtWidgets.QWidget`` to be
     added in a :class:`OdenGraphQt.BaseNode` object.
@@ -212,26 +212,27 @@
     def get_custom_widget(self):
         """
         Returns the embedded QWidget used in the node.
 
         Returns:
             QtWidgets.QWidget: nested QWidget
         """
-        widget = self.widget()
+        widget: _NodeGroupBox = self.widget()
         return widget.get_node_widget()
 
     def set_custom_widget(self, widget):
         """
         Set the custom QWidget used in the node.
 
         Args:
             widget (QtWidgets.QWidget): custom.
         """
         if self.widget():
             raise NodeWidgetError('Custom node widget already set.')
+
         group = _NodeGroupBox(self._label)
         # TODO: Need to handle setting minimum width for custom widget
         group.add_node_widget(widget)
         self.setWidget(group)
 
     def get_label(self):
         """
@@ -245,16 +246,18 @@
     def set_label(self, label=''):
         """
         Sets the label text above the embedded widget.
 
         Args:
             label (str): new label ext.
         """
-        if self.widget():
-            self.widget().setTitle(label)
+        widget: _NodeGroupBox = self.widget()
+        if widget:
+            widget.setTitle(label)
+
         self._label = label
 
 
 class NodeComboBox(NodeBaseWidget):
     """
     Displays as a ``QComboBox`` in a node.
```

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/scene.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/tab_search.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/viewer.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt/widgets/viewer_nav.py` & `OdenGraphQt-0.7.4/OdenGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt.egg-info/PKG-INFO` & `OdenGraphQt-0.7.4/OdenGraphQt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OdenGraphQt
-Version: 0.7.3
+Version: 0.7.4
 Summary: Node graph framework for PySide6/PyQt6 that can be implemented and re-purposed into applications.
 Author: Huey Yeng, Johnny Chan
 Maintainer: Huey Yeng
 License: MIT License
         ===========
         
         Copyright (c) 2024 Huey Yeng
@@ -38,14 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: PySide6>=6.5.0
 Requires-Dist: qtpy>=2.3.1
 
 # OdenGraphQt
 
 OdenGraphQt is a fork of jchanvfx [NodeGraphQt](https://github.com/jchanvfx/NodeGraphQt), a node graph UI framework
 for `PySide6` that can be implemented and re-purposed into applications.
```

### Comparing `OdenGraphQt-0.7.3/OdenGraphQt.egg-info/SOURCES.txt` & `OdenGraphQt-0.7.4/OdenGraphQt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 OdenGraphQt/base/commands.py
 OdenGraphQt/base/factory.py
 OdenGraphQt/base/graph.py
 OdenGraphQt/base/menu.py
 OdenGraphQt/base/model.py
 OdenGraphQt/base/node.py
 OdenGraphQt/base/port.py
+OdenGraphQt/base/types.py
 OdenGraphQt/custom_widgets/__init__.py
 OdenGraphQt/custom_widgets/nodes_palette.py
 OdenGraphQt/custom_widgets/nodes_tree.py
 OdenGraphQt/custom_widgets/properties_bin/__init__.py
 OdenGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
 OdenGraphQt/custom_widgets/properties_bin/custom_widget_extra.py
 OdenGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
```

### Comparing `OdenGraphQt-0.7.3/PKG-INFO` & `OdenGraphQt-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OdenGraphQt
-Version: 0.7.3
+Version: 0.7.4
 Summary: Node graph framework for PySide6/PyQt6 that can be implemented and re-purposed into applications.
 Author: Huey Yeng, Johnny Chan
 Maintainer: Huey Yeng
 License: MIT License
         ===========
         
         Copyright (c) 2024 Huey Yeng
@@ -38,14 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: PySide6>=6.5.0
 Requires-Dist: qtpy>=2.3.1
 
 # OdenGraphQt
 
 OdenGraphQt is a fork of jchanvfx [NodeGraphQt](https://github.com/jchanvfx/NodeGraphQt), a node graph UI framework
 for `PySide6` that can be implemented and re-purposed into applications.
```

### Comparing `OdenGraphQt-0.7.3/README.md` & `OdenGraphQt-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/examples/hotkeys/hotkey_functions.py` & `OdenGraphQt-0.7.4/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/examples/nodes/basic_nodes.py` & `OdenGraphQt-0.7.4/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/examples/nodes/custom_ports_node.py` & `OdenGraphQt-0.7.4/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/examples/nodes/widget_nodes.py` & `OdenGraphQt-0.7.4/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `OdenGraphQt-0.7.3/pyproject.toml` & `OdenGraphQt-0.7.4/pyproject.toml`

 * *Files identical despite different names*

