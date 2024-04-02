# Comparing `tmp/PyQtUIkit-1.6.0.tar.gz` & `tmp/PyQtUIkit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-1.6.0.tar", last modified: Sun Mar 31 14:33:33 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.0.0.tar", last modified: Tue Apr  2 12:08:43 2024, max compression
```

## Comparing `PyQtUIkit-1.6.0.tar` & `PyQtUIkit-2.0.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.941294 PyQtUIkit-1.6.0/
--rw-rw-rw-   0        0        0     1090 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-03-31 14:33:33.941294 PyQtUIkit-1.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.910042 PyQtUIkit-1.6.0/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3969 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.910042 PyQtUIkit-1.6.0/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       90 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0      113 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/core/font_size.py
--rw-rw-rw-   0        0        0     1019 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4361 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.925668 PyQtUIkit-1.6.0/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.925668 PyQtUIkit-1.6.0/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     3740 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     2591 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559111 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1207 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1121 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.941294 PyQtUIkit-1.6.0/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1469 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3115 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1413 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     3622 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2318 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9655 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7012 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5810 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     3264 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0      938 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1184 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     2131 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3245 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     6891 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2503 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6380 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3882 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     6920 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    11840 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2122 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4358 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    15985 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     3265 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:33:33.910042 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2380 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-31 14:33:33.000000 PyQtUIkit-1.6.0/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 14:33:33.941294 PyQtUIkit-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-03-31 14:33:02.000000 PyQtUIkit-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3969 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4478 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.044005 PyQtUIkit-2.0.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.044005 PyQtUIkit-2.0.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     1845 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559111 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1207 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1469 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     3857 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2594 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0     9950 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4142 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1240 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     2130 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6585 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     7014 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    11841 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4411 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    15985 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4441 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:08:43.028327 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 12:08:42.000000 PyQtUIkit-2.0.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:08:43.059557 PyQtUIkit-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-02 12:07:54.000000 PyQtUIkit-2.0.0/setup.py
```

### Comparing `PyQtUIkit-1.6.0/LICENSE` & `PyQtUIkit-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PKG-INFO` & `PyQtUIkit-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 1.6.0
+Version: 2.0.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/_icons.py` & `PyQtUIkit-2.0.0/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.0.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.0.0/PyQtUIkit/core/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum
 from uuid import uuid4
 
+from PyQt6.QtCore import pyqtSignal
 from PyQt6.QtGui import QColor
 
+from PyQtUIkit.core.font import KitFont
 from PyQtUIkit.core.icon import KitIcon
 from PyQtUIkit.themes import KitPalette, icons
 
 
 class IntProperty(property):
     def __init__(self, name='', default=0):
         self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
@@ -73,59 +75,47 @@
         def setter(obj, value: str | KitIcon):
             setattr(obj, self._id, value)
             obj._apply_theme()
 
         super().__init__(getter, setter)
 
 
-class _Color(QColor):
-    def __str__(self):
-        return self.name()
-
-
-class ColorProperty(property):
-    def __init__(self, name='', default='#00000000'):
+class PaletteProperty(property):
+    def __init__(self, name='', default='Main'):
         self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
 
-        def getter(obj) -> _Color:
+        def getter(obj) -> KitPalette:
             try:
                 res = getattr(obj, self._id)
             except AttributeError:
                 res = default
             if isinstance(res, str):
-                if res.startswith('#'):
-                    res = _Color(res)
-                else:
-                    res = obj.theme_manager.get(res)
+                res = obj.theme_manager.palette(res)
             return res
 
-        def setter(obj, value: str | _Color | QColor):
-            if isinstance(value, QColor):
-                value = _Color(value.name())
+        def setter(obj, value: str | KitPalette):
             setattr(obj, self._id, value)
 
         super().__init__(getter, setter)
 
 
-class PaletteProperty(property):
-    def __init__(self, name='', default='Main'):
-        if name == 'Main':
-            raise Exception
+class FontProperty(property):
+    def __init__(self, name='', default='default'):
         self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
 
-        def getter(obj) -> KitPalette:
+        def getter(obj) -> KitFont:
             try:
                 res = getattr(obj, self._id)
             except AttributeError:
                 res = default
             if isinstance(res, str):
-                res = obj.theme_manager.get(res)
+                res = obj.theme_manager.font(res)
             return res
 
-        def setter(obj, value: str | KitPalette):
+        def setter(obj, value: str | KitFont):
             setattr(obj, self._id, value)
 
         super().__init__(getter, setter)
 
 
 class EnumProperty(property):
     def __init__(self, name, enum, default=0):
@@ -141,7 +131,21 @@
 
         def setter(obj, value: str):
             if value not in self._enum:
                 raise ValueError(f"Invalid value: {name} must be one of {repr(list(self._enum))}")
             setattr(obj, self._id, value)
 
         super().__init__(getter, setter)
+
+
+class SignalProperty(property):
+    def __init__(self, name, signal: str):
+        self._id = '_' + (str(name) or str(uuid4()).replace('-', '_'))
+        self._signal = signal
+
+        def getter(obj):
+            return None
+
+        def setter(obj, value: str):
+            getattr(obj, self._signal).connect(value)
+
+        super().__init__(getter, setter)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.0.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.0.0/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.0.0/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/_widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+from typing import Callable
+
+from PyQtUIkit.builder import BUILDER
 from PyQtUIkit.core.properties import PaletteProperty, IntProperty
 from PyQtUIkit.themes import ThemeManager
 
 
 class _KitWidget:
     main_palette = PaletteProperty('main_palette')
+    border_palette = PaletteProperty('border_palette', 'Border')
 
     def __init__(self):
         self._tm: ThemeManager = None
+        self._add_child_func = lambda x: None
+
+    def _build_from_kui(self):
+        BUILDER.build_from_file(self, self._add_child_func)
+
+    def _build_from_kui_as_child(self, _class, vars):
+        BUILDER.build(_class, self, self._add_child_func, vars)
 
     def _set_tm(self, tm: ThemeManager):
         self._tm = tm
         if tm and tm.active:
             self._apply_theme()
 
     @property
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 
 def except_hook(cls, exception, traceback):
     sys.__excepthook__(cls, exception, traceback)
 
 
 class KitApplication(QApplication):
     def __init__(self, window: Callable[[], KitMainWindow]):
-        print(0)
         super().__init__([])
-        print(1)
         self._window = window()
         self._window.show()
         sys.excepthook = except_hook
-        print(2)
 
 
 try:
     import qasync
 except ImportError:
     class KitAsyncApplication:
         def __init__(self):
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/button.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout
 
-from PyQtUIkit.core import IconProperty, EnumProperty, IntProperty, PaletteProperty, FontSize
+from PyQtUIkit.core import IconProperty, EnumProperty, IntProperty, PaletteProperty, KitFont, FontProperty, \
+    SignalProperty
 from PyQtUIkit.themes import ThemeManager
 from PyQtUIkit.widgets import KitIconWidget
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    on_click = SignalProperty('on_click', 'clicked')
 
     def __init__(self, text='', icon=None):
         super().__init__()
         self.__widgets = []
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
         self.setText(text)
         self._icon = icon
 
+        self._build_from_kui()
+
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm['Border'].main};
+    border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
     padding: 3px 8px 3px 8px;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::disabled {{
     color: {self.main_palette.main};
-    border-color: {self._tm['Border'].main};
+    border-color: {self.border_palette.main};
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::menu-indicator {{
     image: none;
     subcontrol-origin: padding;
     padding-right: 5px;
     subcontrol-position: right;
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
+    text = property(QPushButton.text, QPushButton.setText)
+
 
 class KitIconButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     size = IntProperty('size', 24)
     icon = IconProperty('icon')
 
     def __init__(self, icon=''):
@@ -83,27 +90,27 @@
         self._icon_label.icon = self.icon
         self._icon_label._main_palette = self._main_palette
         self.setFixedSize(self.size, self.size)
         self.__layout.setContentsMargins(*[self.size // 5] * 4)
         self.setStyleSheet(f"""
 QPushButton {{
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm['Border'].main};
+    border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
     padding: 3px 8px 3px 8px;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::disabled {{
     color: {self.main_palette.main};
-    border-color: {self._tm['Border'].main};
+    border-color: {self.border_palette.main};
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::menu-indicator {{
     image: none;
     subcontrol-position: right;
 }}""")
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/checkbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, FontSize
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.button import KitIconButton
 
 
 class KitCheckBox(QWidget, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     stateChanged = pyqtSignal(bool)
 
     def __init__(self, text=''):
         super().__init__()
         self.__state = False
         self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Minimum)
@@ -39,30 +40,39 @@
         self.__on_state_changed()
 
     def __on_state_changed(self):
         self.__button.icon = 'solid-check' if self.__state else ''
         self.__button.setChecked(self.__state)
         self.stateChanged.emit(self.__state)
 
-    def state(self):
+    def isChecked(self):
         return self.__state
 
-    def setState(self, state):
+    def setChecked(self, state):
         self.__state = bool(state)
         self.__on_state_changed()
 
+    def setText(self, text):
+        self.__label.setText(text)
+
+    def getText(self):
+        return self.__label.text()
+
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__button._set_tm(tm)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.__button.main_palette = self.main_palette
         self.__button._apply_theme()
-        self.__label.setFont(self._tm.font(self.font_size))
+        self.__label.setFont(self.font.get(self.font_size))
         self.__label.setStyleSheet(f"""
         QPushButton {{
             color: {self.main_palette.text};
             background-color: transparent;
             text-align: left;
         }}""")
+
+    state = property(isChecked, setChecked)
+    text = property(getText, setText)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/combo_box.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from PyQt6.QtCore import pyqtSignal, Qt, QPoint, QPropertyAnimation, QEasingCurve, QSize, QParallelAnimationGroup
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QMenu, QHBoxLayout, QApplication
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontSize
+from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
     selected = pyqtSignal(object)
     icon = IconProperty('icon')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
-    def __init__(self, name, value=None, icon=''):
+    def __init__(self, name='', value=None, icon=''):
         super().__init__()
         self._name = name
         self._value = value or name
         self._icon = icon
         self.setCheckable(True)
         self.clicked.connect(self._on_clicked)
         self.setText(self._name)
@@ -33,39 +34,42 @@
     @property
     def value(self):
         return self._value
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font_medium)
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: 0px solid {self._tm['Border'].main};
+    border: 0px solid {self.border_palette.main};
     border-radius: 5px;
     padding: 3px 5px 3px 5px;
     text-align: left;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
+    name = property(QPushButton.text, QPushButton.setText)
+
 
 class KitComboBox(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     type = IntProperty('type', 1)
     icon = IconProperty('icon')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentIndexChanged = pyqtSignal(object)
     currentValueChanged = pyqtSignal(object)
 
     def __init__(self, *values: str | tuple | KitComboBoxItem):
         super().__init__()
         self.__widgets: list[KitComboBoxItem] = []
@@ -83,14 +87,17 @@
         self._arrow._use_text_only = False
         self._arrow.setFixedSize(16, 12)
         layout.addWidget(self._arrow)
 
         for el in values:
             self.addItem(el)
 
+        self._add_child_func = self.addItem
+        self._build_from_kui()
+
     def addItem(self, item: str | KitComboBoxItem, value=None):
         if not isinstance(item, KitComboBoxItem):
             item = KitComboBoxItem(item, value)
         item.selected.connect(self._on_item_selected)
         self.__widgets.append(item)
         self.__menu.add_item(item)
         if len(self.__widgets) == 1:
@@ -152,44 +159,45 @@
     def resizeEvent(self, a0) -> None:
         super().resizeEvent(a0)
         self.__menu.setFixedWidth(self.width())
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm['Border'].main};
+    border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
     padding: 3px 8px 3px 8px;
     text-align: left;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::disabled {{
     color: {self.main_palette.main};
-    border-color: {self._tm['Border'].main};
+    border-color: {self.border_palette.main};
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}""")
         if self.__current is not None and self.__widgets[self.__current].icon is not None:
             self.setIcon(self.__widgets[self.__current].icon.icon(self.main_palette.text))
         self.__menu._apply_theme()
         self._arrow._apply_theme()
 
 
 class _ComboBoxMenu(QMenu, _KitWidget):
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self):
         super().__init__()
         main_layout = QVBoxLayout()
         main_layout.setContentsMargins(2, 2, 1, 2)
         self.setLayout(main_layout)
 
@@ -229,15 +237,15 @@
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.setStyleSheet(f"""
 QMenu {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: 1px solid {self._tm['Border'].main};
+    border: 1px solid {self.border_palette.main};
     border-radius: 5px;
     spacing: 4px;
     padding: 3px;
 }}""")
         self._scroll_area._apply_theme()
 
     def open(self, pos: QPoint, type=1):
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.__button_close.setHidden(not self.button_close)
         self.__label.setHidden(not self.name)
         self.__top_widget.setHidden(not self.button_close and not self.name)
 
         self.__label.setText(self.name)
         css = f"""color: {self.main_palette.text};
                   background-color: {self.main_palette.main};
-                  border: 1px solid {self._tm['Border'].main};
+                  border: 1px solid {self.border_palette.main};
                   border-radius: 5px;"""
         self.setStyleSheet(css)
 
         self.__top_widget._set_tm(self._parent._tm)
         self.__widget._set_tm(self._parent._tm)
         super()._apply_theme()
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/flow_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def _apply_theme(self):
         for el in self.__widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
         self.setStyleSheet(f"""
         QWidget {{
             background-color: {self.main_palette.main};
-            border: {self.border}px solid {self._tm.get('Border').main};
+            border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
 
 
 class _FlowLayout(QLayout):
     def __init__(self, parent=None, margin=-1, hspacing=-1, vspacing=-1):
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/hbox_layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         strange_layout.addWidget(strange_widget)
 
         self.__layout = QHBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.__layout.setSpacing(0)
         strange_widget.setLayout(self.__layout)
 
+        self._add_child_func = self.addWidget
+        self._build_from_kui()
+
     def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.addWidget(widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.addWidget(widget, stretch)
         else:
             self.__layout.addWidget(widget)
@@ -55,23 +58,42 @@
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
             self.__layout.takeAt(0).widget().setParent(None)
         self._widgets.clear()
 
-    def setAlignment(self, a) -> bool:
-        return self.__layout.setAlignment(a)
+    def setAlignment(self, a):
+        self.__layout.setAlignment(a)
+
+    def getAlignment(self):
+        return self.__layout.alignment()
 
     def setSpacing(self, spacing):
         self.__layout.setSpacing(spacing)
 
+    def getSpacing(self):
+        return self.__layout.spacing()
+
     def setContentsMargins(self, left: int, top: int, right: int, bottom: int) -> None:
         self.__layout.setContentsMargins(left, top, right, bottom)
 
+    def getContentsMargins(self):
+        return self.__layout.contentsMargins()
+
+    def _set_margins(self, margins):
+        if len(margins) == 1:
+            self.__layout.setContentsMargins(margins[0], margins[0], margins[0], margins[0])
+        elif len(margins) == 2:
+            self.__layout.setContentsMargins(margins[0], margins[1], margins[0], margins[1])
+        elif len(margins) == 4:
+            self.__layout.setContentsMargins(*margins)
+        else:
+            raise ValueError
+
     def contentsMargins(self) -> QMargins:
         return self.__layout.contentsMargins()
 
     def count(self):
         return self.__layout.count()
 
     def _set_tm(self, tm):
@@ -85,11 +107,15 @@
             return
         for el in self._widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
         self.setStyleSheet(f"""
         QWidget {{
             background-color: {self.main_palette.main};
-            border: {self.border}px solid {self._tm.get('Border').main};
+            border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
+
+    padding = property(getContentsMargins, _set_margins)
+    spacing = property(getSpacing, setSpacing)
+    alignment = property(getAlignment, setAlignment)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from PyQt6.QtWidgets import QLabel
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, FontSize
+from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitLabel(QLabel, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Transparent')
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, text=''):
         super().__init__(text)
         self._use_text_only = True
+        self._build_from_kui()
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
         QWidget {{
             color: {self.main_palette.text_only if self._use_text_only else self.main_palette.text};
             background-color: transparent;
             border: none;
         }}""")
+
+    text = property(QLabel.text, QLabel.setText)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/line_edit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from PyQt6.QtWidgets import QLineEdit
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, FontSize
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitLineEdit(QLineEdit, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, text=''):
         super().__init__(text)
         self.__widgets = []
         self.border = 1
         self.radius = 4
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QLineEdit {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm.get('Border').main};
+    border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
 }}
 QLineEdit:hover {{
-    border: {self.border}px solid {self._tm.get('Border').hover};
+    border: {self.border}px solid {self.border_palette.hover};
     background-color: {self.main_palette.hover};
 }}
 QLineEdit:focus {{
-    border: {self.border}px solid {self._tm.get('Border').selected};
+    border: {self.border}px solid {self.border_palette.selected};
     background-color: {self.main_palette.hover};
 }}""")
+
+    text = property(QLineEdit.text, QLineEdit.setText)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/list_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.__widgets = []
 
     def _apply_theme(self):
         self.setStyleSheet(f"""
 QListWidget {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm.get('Border').main};
+    border: {self.border}px solid {self.border_palette.main};
     border-radius: {self.radius}px;
 }}
 QListWidget::item {{
     border-radius: 6px;
 }}
 QListWidget::item:hover {{
     background-color: {self.main_palette.hover};
@@ -42,25 +42,25 @@
     background: {self.main_palette.main};
     border-bottom-left-radius: 4px;
     border-bottom-right-radius: 4px;
     height: 12px;
     margin: 0px;
 }}
 QListWidget QScrollBar::handle::vertical {{
-    background-color: {self._tm['Border'].main};
+    background-color: {self.border_palette.main};
     margin: 2px 2px 2px 6px;
     border-radius: 2px;
     min-height: 20px;
 }}
 QListWidget QScrollBar::handle::vertical:hover {{
     margin: 2px;
     border-radius: 4px;
 }}
 QListWidget QScrollBar::handle::horizontal {{
-    background-color: {self._tm['Border'].main};
+    background-color: {self.border_palette.main};
     margin: 6px 2px 2px 2px;
     border-radius: 2px;
     min-width: 20px;
 }}
 QListWidget QScrollBar::handle::horizontal:hover {{
     margin: 2px;
     border-radius: 4px;
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 
 from PyQt6 import QtGui
 from PyQt6.QtGui import QAction
 from PyQt6.QtWidgets import QMenu
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontSize
+from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class _KitMenuAction:
     def __init__(self, action, icon):
         self.__action = action
         self.__icon = icon
@@ -44,15 +44,16 @@
 
 
 class KitMenu(QMenu, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
     icon = IconProperty('icon')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, parent):
         super().__init__()
         self.__parent = parent
         self.__actions = []
 
     def showEvent(self, a0: typing.Optional[QtGui.QShowEvent]) -> None:
@@ -70,41 +71,41 @@
         menu = _KitMenu(menu, icon)
         self.__actions.append(menu)
         return menu
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QMenu {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: 1px solid {self._tm['Border'].main};
+    border: 1px solid {self.border_palette.main};
     border-radius: 6px;
     spacing: 4px;
     padding: 3px;
 }}
 
 QMenu::item {{
-    border: 0px solid {self._tm['Border'].main};
+    border: 0px solid {self.border_palette.main};
     background-color: transparent;
     border-radius: 8px;
     padding: 4px 16px;
 }}
 
 QMenu::icon {{
     padding-left: 6px;
 }}
 
 QMenu::item:selected {{
     background-color: {self.main_palette.hover};
 }}
 QMenu::separator {{
     height: 1px;
-    background: {self._tm['Border'].main};
+    background: {self.border_palette.main};
     margin: 4px 10px;
 }}""")
         if self.icon:
             self.setIcon(self._tm.icon(self.icon, self.main_palette.text))
         for el in self.__actions:
             el._apply_icon(self._tm, self.main_palette)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from PyQt6.QtCore import Qt, QPropertyAnimation, QEasingCurve, pyqtSignal
 from PyQt6.QtGui import QFontMetrics
 from PyQt6.QtWidgets import QLabel, QPushButton, QHBoxLayout, QSizePolicy
 
 from PyQtUIkit.core.icon import KitIcon
-from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontSize
+from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets import KitVBoxLayout, KitIconButton, KitIconWidget
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitNavigationButton(QPushButton, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     selected = pyqtSignal()
 
     def __init__(self, text='', icon=None):
         super().__init__()
         self.__widgets = []
         self._radius = 4
@@ -62,20 +63,21 @@
         super()._set_tm(tm)
         self.__icon._set_tm(tm)
 
     def _apply_theme(self):
         self._set_expanded(not self.__label.isHidden())
         self.setFixedHeight(self._size)
         self.__icon.setFixedSize(self._size - 8, self._size - 8)
-        self.__label.setFont(self._tm.font(self.font_size))
+        self.__icon._main_palette = self._main_palette
+        self.__label.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: 0px solid {self._tm['Border'].main};
+    border: 0px solid {self.border_palette.main};
     border-radius: {self._radius}px;
     padding: 3px 8px 3px 8px;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
 }}
 QPushButton::checked {{
@@ -85,15 +87,16 @@
         if self.icon is not None:
             self.__icon.icon = self.icon
 
 
 class KitNavigation(KitVBoxLayout):
     button_size = IntProperty('button_size', 30)
     button_radius = IntProperty('button_radius', 4)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentChanged = pyqtSignal(int)
 
     def __init__(self):
         super().__init__()
         self._main_palette = 'Menu'
         self._radius = 0
@@ -181,11 +184,12 @@
 
     def _apply_theme(self):
         self.setMaximumWidth(self.button_size + self.contentsMargins().left() + self.contentsMargins().right())
         self.__button.main_palette = self._main_palette
         self.__button.size = self.button_size
         for el in self.__tabs:
             el.main_palette = self.main_palette
+            el.font = self.font
             el.font_size = self.font_size
             el._size = self.button_size
             el._radius = self.button_radius
         super()._apply_theme()
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if self.mode == KitProgressBar.Mode.LARGE:
             self.setFixedHeight(24)
             self.setTextVisible(self.__text_visible)
             self.setStyleSheet(f"""
 QProgressBar {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm['Border'].main};
+    border: {self.border}px solid {self.border_palette.main};
     border-radius: {self.radius}px;
     text-align: center;
 }}
 QProgressBar::chunk {{
     background-color: {self.main_palette.selected};
     border-radius: {self.radius}px;
 }}
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/radio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtGui import QFontMetrics
 from PyQt6.QtWidgets import QLabel, QPushButton, QHBoxLayout, QSizePolicy
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, FontSize, EnumProperty
+from PyQtUIkit.core import IntProperty, PaletteProperty, KitFont, EnumProperty, FontProperty
 from PyQtUIkit.widgets import KitVBoxLayout, KitHBoxLayout
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitRadioButton(QPushButton, _KitWidget):
     main_palette = PaletteProperty('Bg')
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     selected = pyqtSignal()
 
     def __init__(self, text=''):
         super().__init__()
         self.__widgets = []
         self._size = 30
@@ -42,42 +43,43 @@
     def _set_selected(self, flag):
         self.__selected = flag
         self.__button.setChecked(flag)
         if flag:
             self.selected.emit()
 
     def _apply_theme(self):
-        self.__label.setFont(self._tm.font(self.font_size))
+        self.__label.setFont(self.font.get(self.font_size))
         fm = QFontMetrics(self.__label.font())
         fm.size(0, self.__label.text())
         self.setFixedWidth(34 + fm.size(0, self.__label.text()).width())
 
         self.setFixedHeight(self._size)
         self.__button.setFixedSize(self._size - 8, self._size - 8)
         self.__button.setStyleSheet(f"""
 QPushButton {{
     background-color: {self.main_palette.main};
-    border: 1px solid {self._tm['Border'].main};
+    border: 1px solid {self.border_palette.main};
     border-radius: {(self._size - 8) // 2}px;
     padding: 3px 8px 3px 8px;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
-    border: 1px solid {self._tm['Border'].selected};
+    border: 1px solid {self.border_palette.selected};
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.main};
-    border: {(self._size - 8) // 4}px solid {self._tm['Border'].selected};
+    border: {(self._size - 8) // 4}px solid {self.border_palette.selected};
 }}""")
         self.__label.setStyleSheet(f"color: {self.main_palette.text}; border: none; background-color: transparent")
 
 
 class KitVRadio(KitVBoxLayout):
     button_height = IntProperty('button_size', 24)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentChanged = pyqtSignal(int)
 
     def __init__(self):
         super().__init__()
         self._main_palette = 'Bg'
         self.__items = []
@@ -120,22 +122,24 @@
 
     def currentIndex(self):
         return self.__items.index(self.__current)
 
     def _apply_theme(self):
         for el in self.__items:
             el.main_palette = self.main_palette
+            el.font = self.font
             el.font_size = self.font_size
             el._size = self.button_height
         super()._apply_theme()
 
 
 class KitHRadio(KitHBoxLayout):
     button_height = IntProperty('button_size', 24)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentChanged = pyqtSignal(int)
 
     def __init__(self):
         super().__init__()
         self._main_palette = 'Bg'
         self.__items = []
@@ -178,10 +182,11 @@
 
     def currentIndex(self):
         return self.__items.index(self.__current)
 
     def _apply_theme(self):
         for el in self.__items:
             el.main_palette = self.main_palette
+            el.font = self.font
             el.font_size = self.font_size
             el._size = self.button_height
         super()._apply_theme()
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/scroll_area.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.setStyleSheet(f"""
 QScrollArea {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm.get('Border').main};
+    border: {self.border}px solid {self.border_palette.main};
     border-radius: {self.radius}px;
 }}
 QScrollArea QScrollBar:vertical {{
     background: {self.main_palette.main};
     border-top-right-radius: 4px;
     border-bottom-right-radius: 4px;
     width: 12px;
@@ -83,25 +83,25 @@
     background: {self.main_palette.main};
     border-bottom-left-radius: 4px;
     border-bottom-right-radius: 4px;
     height: 12px;
     margin: 0px;
 }}
 QScrollArea QScrollBar::handle::vertical {{
-    background-color: {self._tm['Border'].main};
+    background-color: {self.border_palette.main};
     margin: 2px 2px 2px 6px;
     border-radius: 2px;
     min-height: 20px;
 }}
 QScrollArea QScrollBar::handle::vertical:hover {{
     margin: 2px;
     border-radius: 4px;
 }}
 QScrollArea QScrollBar::handle::horizontal {{
-    background-color: {self._tm['Border'].main};
+    background-color: {self.border_palette.main};
     margin: 6px 2px 2px 2px;
     border-radius: 2px;
     min-width: 20px;
 }}
 QScrollArea QScrollBar::handle::horizontal:hover {{
     margin: 2px;
     border-radius: 4px;
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/spin_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from PyQt6.QtCore import pyqtSignal, Qt
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QLineEdit, QVBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import IntProperty, EnumProperty, FontSize
+from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem, KitGroup as _KitGroup
 
 
 class KitSpinBox(QWidget, _KitGroupItem):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
     valueChanged = pyqtSignal(object)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, func=int):
         super().__init__()
         self._min = 0
         self._max = 100
         self._step = 1
         self._func = func
@@ -106,60 +107,62 @@
         self._max = maximum
         self._on_text_edited()
 
     def setValue(self, value):
         self._line_edit.setText(str(value))
         self._on_text_edited()
 
-    def value(self):
+    def getValue(self):
         if not self._line_edit.text():
             return 0
         return self._func(self._line_edit.text())
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         orientation, position = self._group()
         self._line_edit.setFixedHeight(self.height())
-        self._line_edit.setFont(self._tm.font(self.font_size))
+        self._line_edit.setFont(self.font.get(self.font_size))
         self._line_edit.setStyleSheet(f"""
         QLineEdit {{
             color: {self.main_palette.text};
             background-color: {self.main_palette.main};
-            border: {self.border}px solid {self._tm.get('Border').main};
+            border: {self.border}px solid {self.border_palette.main};
             border-top-left-radius: {self.radius if orientation == _KitGroup.NO_GROUP or position == _KitGroup.FIRST else 0}px;
             border-bottom-left-radius: {self.radius if orientation == _KitGroup.NO_GROUP or
                                                        orientation == _KitGroup.VERTICAL and position == _KitGroup.LAST or
                                                        orientation == _KitGroup.HORIZONTAL and position == _KitGroup.FIRST else 0}px;
             border-top-right-radius: 0px;
             border-bottom-right-radius: 0px;
         }}
         QLineEdit:hover {{
-            border: {self.border}px solid {self._tm.get('Border').hover};
+            border: {self.border}px solid {self.border_palette.hover};
             background-color: {self.main_palette.hover};
         }}
         QLineEdit:focus {{
-            border: {self.border}px solid {self._tm.get('Border').selected};
+            border: {self.border}px solid {self.border_palette.selected};
             background-color: {self.main_palette.hover};
         }}""")
         self._button_up.setIcon(self._tm.icon('solid-angle-up', self.main_palette.text))
         self._button_down.setIcon(self._tm.icon('solid-angle-down', self.main_palette.text))
         css = f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm['Border'].main};
+    border: {self.border}px solid {self.border_palette.main};
     border-top-left-radius: 0px;
     border-bottom-left-radius: 0px;
     border-top-right-radius: 0px;
     border-bottom-right-radius: 0px;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self._tm['Border'].selected};
+    border: {self.border}px solid {self.border_palette.selected};
 }}"""
         radius = self.radius if orientation == _KitGroup.NO_GROUP or \
                                 orientation == _KitGroup.VERTICAL and position == _KitGroup.FIRST or \
                                 orientation == _KitGroup.HORIZONTAL and position == _KitGroup.LAST else 0
         self._button_up.setStyleSheet(css.replace("top-right-radius: 0px;", f"top-right-radius: {radius}px;"))
         radius = self.radius if orientation == _KitGroup.NO_GROUP or position == _KitGroup.LAST else 0
         self._button_down.setStyleSheet(css.replace("bottom-right-radius: 0px;", f"bottom-right-radius: {radius}px;"))
+
+    value = property(getValue, setValue)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tab_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.__button_close.main_palette = KitPalette('#00000000', self.main_palette.main,
                                                       text=self.main_palette.text)
         self.__label.setFont(self._tm.font_medium)
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main if not self.__checked else self.main_palette.selected};
-    border: 0px solid {self._tm['Border'].main};
+    border: 0px solid {self.border_palette.main};
     border-top-left-radius: {self.radius_top}px;
     border-top-right-radius: {self.radius_top}px;
     border-bottom-left-radius: {self.radius_bottom}px;
     border-bottom-right-radius: {self.radius_bottom}px;
     padding: 3px 5px 3px 5px;
     text-align: left;
 }}
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/text_edit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from PyQt6.QtWidgets import QTextEdit
 
-from PyQtUIkit.core import FontSize
-from PyQtUIkit.core.properties import IntProperty, PaletteProperty, EnumProperty
+from PyQtUIkit.core import KitFont
+from PyQtUIkit.core.properties import IntProperty, PaletteProperty, EnumProperty, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitTextEdit(QTextEdit, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
-    font_size = EnumProperty('font_size', FontSize, FontSize.MEDIUM)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self):
         super().__init__()
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self.setFont(self._tm.font(self.font_size))
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QTextEdit {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
-    border: {self.border}px solid {self._tm.get('Border').main};
+    border: {self.border}px solid {self.border_palette.main};
     border-radius: {self.radius}px;
 }}
 QTextEdit QScrollBar:vertical {{
     background: {self.main_palette.main};
     border-top-right-radius: 5px;
     border-bottom-right-radius: 5px;
     width: 12px;
@@ -36,25 +37,25 @@
     background: {self.main_palette.main};
     border-bottom-left-radius: 5px;
     border-bottom-right-radius: 5px;
     height: 12px;
     margin: 0px;
 }}
 QTextEdit QScrollBar::handle::horizontal {{
-    background-color: {self._tm.get('Border').main};
+    background-color: {self.border_palette.main};
     margin: 6px 2px 2px 2px;
     border-radius: 2px;
     min-width: 20px;
 }}
 QTextEdit QScrollBar::handle::horizontal:hover {{
     margin: 2px;
     border-radius: 4px;
 }}
 QTextEdit QScrollBar::handle::vertical {{
-    background-color: {self._tm.get('Border').main};
+    background-color: {self.border_palette.main};
     margin: 2px 2px 2px 6px;
     border-radius: 2px;
     min-height: 20px;
 }}
 QTextEdit QScrollBar::handle::vertical:hover {{
     margin: 2px;
     border-radius: 4px;
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/toggle.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,18 +75,18 @@
                                 QPoint(self.__button_x, self.__button_y))
         self.__anim.setDuration(200)
         self.__anim.setEasingCurve(QEasingCurve.Type.OutCubic)
         self.__anim.start()
 
         self._apply_theme()
 
-    def state(self):
+    def isChecked(self):
         return self.__state
 
-    def setState(self, state):
+    def setChecked(self, state):
         self.__state = bool(state)
         self.__on_state_changed()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__button._set_tm(tm)
 
@@ -110,11 +110,13 @@
         self.__button.move(self.__button_x_r if self.__state else self.__button_x, self.__button_y)
 
         self.__button.main_palette = self.main_palette
         self.__button._apply_theme()
         self.__rail.setStyleSheet(f"""
         QWidget {{
             color: {self.main_palette.text};
-            background-color: {self.rail_palette.selected if self.__state else self.main_palette.main};
+            background-color: {self.rail_palette.selected if self.__state else self.rail_palette.main};
             border: 0px solid black;
             border-radius: {sizes['rail_size'][1] // 2}px;
         }}""")
+
+    state = property(isChecked, setChecked)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.0.0/PyQtUIkit/widgets/vbox_layout.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         strange_layout.addWidget(strange_widget)
 
         self.__layout = QVBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.__layout.setSpacing(0)
         strange_widget.setLayout(self.__layout)
 
+        self._add_child_func = self.addWidget
+        self._build_from_kui()
+
     def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.addWidget(widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.addWidget(widget, stretch)
         else:
             self.__layout.addWidget(widget)
@@ -55,23 +58,42 @@
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
             self.__layout.takeAt(0).widget().setParent(None)
         self._widgets.clear()
 
-    def setAlignment(self, a) -> bool:
-        return self.__layout.setAlignment(a)
+    def setAlignment(self, a):
+        self.__layout.setAlignment(a)
+
+    def getAlignment(self):
+        return self.__layout.alignment()
 
     def setSpacing(self, spacing):
         self.__layout.setSpacing(spacing)
 
+    def getSpacing(self):
+        return self.__layout.spacing()
+
     def setContentsMargins(self, left: int, top: int, right: int, bottom: int) -> None:
         self.__layout.setContentsMargins(left, top, right, bottom)
 
+    def getContentsMargins(self):
+        return self.__layout.contentsMargins()
+
+    def _set_margins(self, margins):
+        if len(margins) == 1:
+            self.__layout.setContentsMargins(margins[0], margins[0], margins[0], margins[0])
+        elif len(margins) == 2:
+            self.__layout.setContentsMargins(margins[0], margins[1], margins[0], margins[1])
+        elif len(margins) == 4:
+            self.__layout.setContentsMargins(*margins)
+        else:
+            raise ValueError
+
     def contentsMargins(self) -> QMargins:
         return self.__layout.contentsMargins()
 
     def count(self):
         return self.__layout.count()
 
     def _set_tm(self, tm):
@@ -85,11 +107,19 @@
             return
         for el in self._widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
         self.setStyleSheet(f"""
         QWidget {{
             background-color: {self.main_palette.main};
-            border: {self.border}px solid {self._tm.get('Border').main};
+            border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
+
+    padding = property(getContentsMargins, _set_margins)
+    spacing = property(getSpacing, setSpacing)
+    alignment = property(getAlignment, setAlignment)
+    max_width = property(QWidget.maximumWidth, QWidget.setMaximumWidth)
+    min_width = property(QWidget.minimumWidth, QWidget.setMinimumWidth)
+    max_height = property(QWidget.maximumHeight, QWidget.setMaximumHeight)
+    min_height = property(QWidget.minimumHeight, QWidget.setMinimumHeight)
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.0.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 1.6.0
+Version: 2.0.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-1.6.0/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.0.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 PyQtUIkit/_icons.py
 PyQtUIkit.egg-info/PKG-INFO
 PyQtUIkit.egg-info/SOURCES.txt
 PyQtUIkit.egg-info/dependency_links.txt
 PyQtUIkit.egg-info/entry_points.txt
 PyQtUIkit.egg-info/requires.txt
 PyQtUIkit.egg-info/top_level.txt
+PyQtUIkit/builder/__init__.py
+PyQtUIkit/builder/builder_class.py
+PyQtUIkit/builder/builder_module.py
 PyQtUIkit/core/__init__.py
 PyQtUIkit/core/_version.py
-PyQtUIkit/core/font_size.py
+PyQtUIkit/core/font.py
 PyQtUIkit/core/icon.py
 PyQtUIkit/core/properties.py
 PyQtUIkit/fonts/Roboto-Black.ttf
 PyQtUIkit/fonts/Roboto-BlackItalic.ttf
 PyQtUIkit/fonts/Roboto-Bold.ttf
 PyQtUIkit/fonts/Roboto-BoldItalic.ttf
 PyQtUIkit/fonts/Roboto-Italic.ttf
```

### Comparing `PyQtUIkit-1.6.0/setup.py` & `PyQtUIkit-2.0.0/setup.py`

 * *Files identical despite different names*

