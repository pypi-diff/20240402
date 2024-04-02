# Comparing `tmp/PyQtUIkit-2.0.0.tar.gz` & `tmp/PyQtUIkit-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.0.0.tar", last modified: Tue Apr  2 12:08:43 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.0.1.tar", last modified: Tue Apr  2 13:34:06 2024, max compression
```

## Comparing `PyQtUIkit-2.0.0.tar` & `PyQtUIkit-2.0.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/
--rw-rw-rw-   0        0        0     1090 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3969 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4478 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.044005 PyQtUIkit-2.0.0/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.044005 PyQtUIkit-2.0.0/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     1845 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559111 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1207 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1469 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     3857 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2594 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9950 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4142 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1240 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     2130 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6585 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     7014 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    11841 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4411 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    15985 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4441 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4478 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.453929 PyQtUIkit-2.0.1/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.453929 PyQtUIkit-2.0.1/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     1845 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559111 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1207 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1469 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     3857 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2594 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0     9950 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4142 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1287 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     2130 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6585 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     7014 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    11841 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4411 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    15985 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4441 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/setup.py
```

### Comparing `PyQtUIkit-2.0.0/LICENSE` & `PyQtUIkit-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PKG-INFO` & `PyQtUIkit-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.0
+Version: 2.0.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/_icons.py` & `PyQtUIkit-2.0.1/PyQtUIkit/_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         item.setText(key)
         self.list_widget.addItem(item)
 
     def update_icons(self):
         self.list_widget.clear()
         if isinstance(self.__searcher, QThread):
             self.__searcher.terminate()
-        search = self.line_edit.text()
+        search = self.line_edit.text
         self.__searcher = Searcher(search, icons.keys())
         self.__searcher.find.connect(self._add_icon)
         self.__searcher.finished.connect(self._on_search_finished)
 
         self._spinner.resume()
         self._spinner.show()
         self._icon.hide()
```

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.0.1/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/core/font.py` & `PyQtUIkit-2.0.1/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.0.1/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.0.1/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.0.1/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.0.1/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.0.1/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.0.1/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.0.1/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/line_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from PyQt6.QtWidgets import QLineEdit
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitLineEdit(QLineEdit, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    font = FontProperty('font')
 
     def __init__(self, text=''):
         super().__init__(text)
         self.__widgets = []
         self.border = 1
         self.radius = 4
```

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.0.1/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.0.1/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.0
+Version: 2.0.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.0/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.0.1/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.0/setup.py` & `PyQtUIkit-2.0.1/setup.py`

 * *Files identical despite different names*

