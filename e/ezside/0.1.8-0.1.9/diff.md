# Comparing `tmp/ezside-0.1.8.tar.gz` & `tmp/ezside-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezside-0.1.8.tar", last modified: Fri Mar 22 11:36:44 2024, max compression
+gzip compressed data, was "ezside-0.1.9.tar", last modified: Fri Mar 22 11:44:50 2024, max compression
```

## Comparing `ezside-0.1.8.tar` & `ezside-0.1.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-22 11:36:34.000000 ezside-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 11:36:44.461896 ezside-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 11:36:34.000000 ezside-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-22 11:36:40.000000 ezside-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-22 11:36:44.461896 ezside-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.449896 ezside-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.449896 ezside-0.1.8/src/eznum/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-22 11:36:34.000000 ezside-0.1.8/src/eznum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-22 11:36:34.000000 ezside-0.1.8/src/eznum/_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-22 11:36:34.000000 ezside-0.1.8/src/eznum/_eznum_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.449896 ezside-0.1.8/src/ezside/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.453896 ezside-0.1.8/src/ezside/core/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_brush.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_brush_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_color_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_font_family.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_parse_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_pen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_pen_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/core/_qt_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.457896 ezside-0.1.8/src/ezside/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_base_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_border_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_box_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_client_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_corner_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_data_roll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_data_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_data_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_filled_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_grid_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_horizontal_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_horizontal_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_layout_OLD.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_plot_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_radio_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_spacer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_text_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_vertical_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_vertical_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_vertical_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_white_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/widgets/_wrap_viewOLD.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.457896 ezside-0.1.8/src/ezside/windows/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/_base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/_layout_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/_main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/_test_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.457896 ezside-0.1.8/src/ezside/windows/bars/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/bars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/bars/_menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/bars/_status_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/ezside/windows/menus/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_abstract_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_debug_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_edit_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_files_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/_help_menu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/ezside/windows/menus/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/icons/_get_icon_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/icons/_load_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/ezside/windows/menus/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-22 11:36:34.000000 ezside-0.1.8/src/ezside/windows/menus/shortcuts/_get_shortcut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/ezside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 11:36:44.000000 ezside-0.1.8/src/ezside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-22 11:36:44.000000 ezside-0.1.8/src/ezside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:36:44.000000 ezside-0.1.8/src/ezside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-22 11:36:44.000000 ezside-0.1.8/src/ezside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/moreutils/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-22 11:36:34.000000 ezside-0.1.8/src/moreutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-22 11:36:34.000000 ezside-0.1.8/src/moreutils/_int_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:36:44.461896 ezside-0.1.8/src/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-22 11:36:34.000000 ezside-0.1.8/src/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-22 11:36:34.000000 ezside-0.1.8/src/settings/_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-22 11:36:34.000000 ezside-0.1.8/src/settings/_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.603319 ezside-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-22 11:44:39.000000 ezside-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 11:44:50.603319 ezside-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 11:44:39.000000 ezside-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-22 11:44:46.000000 ezside-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-22 11:44:50.603319 ezside-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.591319 ezside-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.591319 ezside-0.1.9/src/eznum/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-22 11:44:39.000000 ezside-0.1.9/src/eznum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-22 11:44:39.000000 ezside-0.1.9/src/eznum/_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-22 11:44:39.000000 ezside-0.1.9/src/eznum/_eznum_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.591319 ezside-0.1.9/src/ezside/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.595319 ezside-0.1.9/src/ezside/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_brush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_brush_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_color_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_font_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_parse_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_pen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_pen_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/core/_qt_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_border_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_box_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_client_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_corner_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_data_roll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_data_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_data_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_filled_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_grid_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_horizontal_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_horizontal_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_layout_OLD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_plot_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_radio_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_spacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_text_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_vertical_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_vertical_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_vertical_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_white_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/widgets/_wrap_viewOLD.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/_base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/_layout_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/_test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/windows/bars/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/bars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/bars/_menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/bars/_status_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/windows/menus/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_abstract_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_debug_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_edit_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_files_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/_help_menu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/windows/menus/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/icons/_get_icon_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/icons/_load_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.599319 ezside-0.1.9/src/ezside/windows/menus/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-22 11:44:39.000000 ezside-0.1.9/src/ezside/windows/menus/shortcuts/_get_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.603319 ezside-0.1.9/src/ezside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 11:44:50.000000 ezside-0.1.9/src/ezside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-22 11:44:50.000000 ezside-0.1.9/src/ezside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:44:50.000000 ezside-0.1.9/src/ezside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-22 11:44:50.000000 ezside-0.1.9/src/ezside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.603319 ezside-0.1.9/src/moreutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-22 11:44:39.000000 ezside-0.1.9/src/moreutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-22 11:44:39.000000 ezside-0.1.9/src/moreutils/_int_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:44:50.603319 ezside-0.1.9/src/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-22 11:44:39.000000 ezside-0.1.9/src/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-22 11:44:39.000000 ezside-0.1.9/src/settings/_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-22 11:44:39.000000 ezside-0.1.9/src/settings/_icons.py
```

### Comparing `ezside-0.1.8/LICENSE` & `ezside-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/PKG-INFO` & `ezside-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezside
-Version: 0.1.8
+Version: 0.1.9
 Summary: ezside provides examples and utilities for PySide6.
 Home-page: https://github.com/AsgerJon/ezside
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/ezside
 Project-URL: Bug Tracker, https://github.com/AsgerJon/ezside
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezside-0.1.8/pyproject.toml` & `ezside-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=68.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "ezside"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "ezside provides examples and utilities for PySide6."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ezside-0.1.8/setup.cfg` & `ezside-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ezside
-version = 0.1.8
+version = 0.1.9
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = ezside provides examples and utilities for PySide6
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AsgerJon/ezside
 classifiers =
```

### Comparing `ezside-0.1.8/src/eznum/_eznum_meta.py` & `ezside-0.1.9/src/eznum/_eznum_meta.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/__init__.py` & `ezside-0.1.9/src/ezside/__init__.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/__init__.py` & `ezside-0.1.9/src/ezside/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_brush.py` & `ezside-0.1.9/src/ezside/core/_brush.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_brush_factory.py` & `ezside-0.1.9/src/ezside/core/_brush_factory.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_color_factory.py` & `ezside-0.1.9/src/ezside/core/_color_factory.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_colors.py` & `ezside-0.1.9/src/ezside/core/_colors.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_font_family.py` & `ezside-0.1.9/src/ezside/core/_font_family.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_parse_parent.py` & `ezside-0.1.9/src/ezside/core/_parse_parent.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_pen.py` & `ezside-0.1.9/src/ezside/core/_pen.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_pen_factory.py` & `ezside-0.1.9/src/ezside/core/_pen_factory.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/core/_qt_names.py` & `ezside-0.1.9/src/ezside/core/_qt_names.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/__init__.py` & `ezside-0.1.9/src/ezside/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_base_widget.py` & `ezside-0.1.9/src/ezside/widgets/_base_widget.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_border_rect.py` & `ezside-0.1.9/src/ezside/widgets/_border_rect.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_box_layout.py` & `ezside-0.1.9/src/ezside/widgets/_box_layout.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_client_info.py` & `ezside-0.1.9/src/ezside/widgets/_client_info.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_control_widget.py` & `ezside-0.1.9/src/ezside/widgets/_control_widget.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_corner_panel.py` & `ezside-0.1.9/src/ezside/widgets/_corner_panel.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_data_roll.py` & `ezside-0.1.9/src/ezside/widgets/_data_roll.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_data_series.py` & `ezside-0.1.9/src/ezside/widgets/_data_series.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_data_view.py` & `ezside-0.1.9/src/ezside/widgets/_data_view.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_data_widget.py` & `ezside-0.1.9/src/ezside/widgets/_data_widget.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_equalizer.py` & `ezside-0.1.9/src/ezside/widgets/_equalizer.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_filled_rect.py` & `ezside-0.1.9/src/ezside/widgets/_filled_rect.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_grid_layout.py` & `ezside-0.1.9/src/ezside/widgets/_grid_layout.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_horizontal_panel.py` & `ezside-0.1.9/src/ezside/widgets/_horizontal_panel.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_layout_OLD.py` & `ezside-0.1.9/src/ezside/widgets/_layout_OLD.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_plot_envelope.py` & `ezside-0.1.9/src/ezside/widgets/_plot_envelope.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_spacer.py` & `ezside-0.1.9/src/ezside/widgets/_spacer.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_spinbox.py` & `ezside-0.1.9/src/ezside/widgets/_spinbox.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_text_label.py` & `ezside-0.1.9/src/ezside/widgets/_text_label.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_timer.py` & `ezside-0.1.9/src/ezside/widgets/_timer.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_vertical_panel.py` & `ezside-0.1.9/src/ezside/widgets/_vertical_panel.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_vertical_slider.py` & `ezside-0.1.9/src/ezside/widgets/_vertical_slider.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_white_noise.py` & `ezside-0.1.9/src/ezside/widgets/_white_noise.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/widgets/_wrap_viewOLD.py` & `ezside-0.1.9/src/ezside/widgets/_wrap_viewOLD.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/_base_window.py` & `ezside-0.1.9/src/ezside/windows/_base_window.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/_layout_window.py` & `ezside-0.1.9/src/ezside/windows/_layout_window.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/_main_window.py` & `ezside-0.1.9/src/ezside/windows/_main_window.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/_test_window.py` & `ezside-0.1.9/src/ezside/windows/_test_window.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/bars/_menu_bar.py` & `ezside-0.1.9/src/ezside/windows/bars/_menu_bar.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/bars/_status_bar.py` & `ezside-0.1.9/src/ezside/windows/bars/_status_bar.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_abstract_menu.py` & `ezside-0.1.9/src/ezside/windows/menus/_abstract_menu.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_action.py` & `ezside-0.1.9/src/ezside/windows/menus/_action.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_debug_menu.py` & `ezside-0.1.9/src/ezside/windows/menus/_debug_menu.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_edit_menu.py` & `ezside-0.1.9/src/ezside/windows/menus/_edit_menu.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_files_menu.py` & `ezside-0.1.9/src/ezside/windows/menus/_files_menu.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/_help_menu.py` & `ezside-0.1.9/src/ezside/windows/menus/_help_menu.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/icons/_get_icon_path.py` & `ezside-0.1.9/src/ezside/windows/menus/icons/_get_icon_path.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/icons/_load_icon.py` & `ezside-0.1.9/src/ezside/windows/menus/icons/_load_icon.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside/windows/menus/shortcuts/_get_shortcut.py` & `ezside-0.1.9/src/ezside/windows/menus/shortcuts/_get_shortcut.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/ezside.egg-info/PKG-INFO` & `ezside-0.1.9/src/ezside.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezside
-Version: 0.1.8
+Version: 0.1.9
 Summary: ezside provides examples and utilities for PySide6.
 Home-page: https://github.com/AsgerJon/ezside
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/ezside
 Project-URL: Bug Tracker, https://github.com/AsgerJon/ezside
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezside-0.1.8/src/ezside.egg-info/SOURCES.txt` & `ezside-0.1.9/src/ezside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/moreutils/_int_field.py` & `ezside-0.1.9/src/moreutils/_int_field.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/settings/_default.py` & `ezside-0.1.9/src/settings/_default.py`

 * *Files identical despite different names*

### Comparing `ezside-0.1.8/src/settings/_icons.py` & `ezside-0.1.9/src/settings/_icons.py`

 * *Files identical despite different names*

