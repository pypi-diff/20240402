# Comparing `tmp/eo_man-0.1.8.tar.gz` & `tmp/eo_man-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_man-0.1.8.tar", last modified: Tue Feb 20 22:43:29 2024, max compression
+gzip compressed data, was "eo_man-0.1.9.tar", last modified: Thu Feb 22 23:01:08 2024, max compression
```

## Comparing `eo_man-0.1.8.tar` & `eo_man-0.1.9.tar`

### file list

```diff
@@ -1,66 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.967529 eo_man-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-20 22:43:12.000000 eo_man-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-02-20 22:43:29.967529 eo_man-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-20 22:43:12.000000 eo_man-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.959529 eo_man-0.1.8/eo_man/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.959529 eo_man-0.1.8/eo_man/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/controller/app_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/controller/esp3_serial_com.py
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/controller/serial_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.963529 eo_man-0.1.8/eo_man/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/app_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/application_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/data_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/ha_config_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.963529 eo_man-0.1.8/eo_man/data/homeassistant/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/data/homeassistant/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.963529 eo_man-0.1.8/eo_man/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Breathe-about.png
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Faenza-system-search.png
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Gnome-help-faq.png
--rw-r--r--   0 runner    (1001) docker     (127)    58874 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Home_Assistant_Logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Oxygen480-actions-document-save-as.png
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Oxygen480-actions-document-save.png
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Oxygen480-actions-help.png
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Oxygen480-status-folder-open.png
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/Software-update-available.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49380 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/export_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/github_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/image_gallary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/paypal_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/paypal_me_badge.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/icons/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.967529 eo_man-0.1.8/eo_man/view/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/about_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    54995 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/checklistcombobox.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/device_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/device_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/donation_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/filter_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/log_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/main_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/menu_presenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/serial_communication_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/status_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-20 22:43:12.000000 eo_man-0.1.8/eo_man/view/tool_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.967529 eo_man-0.1.8/eo_man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-02-20 22:43:29.000000 eo_man-0.1.8/eo_man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-20 22:43:29.000000 eo_man-0.1.8/eo_man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 22:43:29.000000 eo_man-0.1.8/eo_man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-20 22:43:29.000000 eo_man-0.1.8/eo_man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 22:43:29.000000 eo_man-0.1.8/eo_man.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 22:43:29.967529 eo_man-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-20 22:43:12.000000 eo_man-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:43:29.967529 eo_man-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-20 22:43:12.000000 eo_man-0.1.8/tests/test_app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.878840 eo_man-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-22 23:00:48.000000 eo_man-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-22 23:01:08.878840 eo_man-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-02-22 23:00:48.000000 eo_man-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.870840 eo_man-0.1.9/eo_man/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.870840 eo_man-0.1.9/eo_man/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/controller/app_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/controller/esp3_serial_com.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23423 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/controller/serial_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.870840 eo_man-0.1.9/eo_man/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/app_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/application_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/data_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/ha_config_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.870840 eo_man-0.1.9/eo_man/data/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/data/homeassistant/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.874840 eo_man-0.1.9/eo_man/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Breathe-about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20886 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Faenza-system-search.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Faenza-system-search.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Faenza-system-search.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Gnome-help-faq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58874 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Home_Assistant_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Oxygen480-actions-document-save-as.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Oxygen480-actions-document-save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Oxygen480-actions-help.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Oxygen480-status-folder-open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/Software-update-available.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/blank.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49380 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/export_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/fam-usb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/fam-usb2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/fam14.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   246846 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/fam14.png
+-rw-r--r--   0 runner    (1001) docker     (127)   170989 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/fgw14-usb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/github_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/image_gallary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/paypal_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/paypal_me_badge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43746 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/usb300.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24425 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/wireless-network-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36175 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/wireless-network-colored.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/icons/wireless.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.878840 eo_man-0.1.9/eo_man/view/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/about_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54995 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/checklistcombobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/device_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/device_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/donation_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/filter_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/log_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/main_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/menu_presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/serial_communication_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/status_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-02-22 23:00:48.000000 eo_man-0.1.9/eo_man/view/tool_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.878840 eo_man-0.1.9/eo_man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-22 23:01:08.000000 eo_man-0.1.9/eo_man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-22 23:01:08.000000 eo_man-0.1.9/eo_man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 23:01:08.000000 eo_man-0.1.9/eo_man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 23:01:08.000000 eo_man-0.1.9/eo_man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 23:01:08.000000 eo_man-0.1.9/eo_man.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 23:01:08.878840 eo_man-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-22 23:00:48.000000 eo_man-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:01:08.878840 eo_man-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-22 23:00:48.000000 eo_man-0.1.9/tests/test_app_config.py
```

### Comparing `eo_man-0.1.8/LICENSE` & `eo_man-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/PKG-INFO` & `eo_man-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo_man
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to managed EnOcean Devices and to generate Home Assistant Configuration.
 Home-page: https://github.com/grimmpp/enocean-device-manager
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
         
@@ -25,15 +25,17 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eltako14bus==0.0.45
+Requires-Dist: eltako14bus==0.0.46
+Requires-Dist: requests==2.31.0
+Requires-Dist: enocean==0.60.1
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio
 Requires-Dist: aiocoap
 Requires-Dist: pyyaml
 Requires-Dist: termcolor
 Requires-Dist: strenum
 Requires-Dist: pillow
@@ -51,15 +53,15 @@
 # WORK IN PROGRESS!!! NOT YET RELEASE READY!!!
 
 This client application allows you to **inventory all EnOcean devices**. It can **automatically read and detect devices** from the RS485 bus or from wireless network. After the devices are listed in the EnOcean Device Manager **you can enricht device information** like changing the name, comment or adapt parameters like timeframes, thresholds, units, ... .
 Furthermore, it automatically can detect default settings for Home Assistant configuration which can be adjust as well and it allows you to **generate and export the configuration for Home Assistant**. 
 (The exported Home Assistant configuration is intended for the [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako/))
 
 ## Preview
-<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot.png" /> 
+<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot2.png" /> 
 What you can see here can automatically detected by reading the memory of the bus devices via FAM14. Telegrams of sensors and decentralized devices will be received and additionally added. 
 Additional info for Home Assistant is automatically added. The configuration for Home Assistant can be generated by the detected information.
 For further steps it is planned to extend the support for changing the data which was collected so that a proper management of the devices can be supported.
 
 ## System Requirements / Where to install and how to use it?
 This tool is a desktop application (not browser based) and it runs independent of Home Assistant. Install it directly on a Windows, Linux or Max. (So far only Windows has been tested but all three operating systems should be supported.) Your PC requires Python pre-installed and you should be able to connect it to your EnOcean devices, either via USB cable (Eltako FAM14, FGW14-USB, ...) or wireless transceiver (Eltako FAM-USB). Support for the wireless transceiver 'EnOcean USB300' is planned for future releases.
```

### Comparing `eo_man-0.1.8/README.md` & `eo_man-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WORK IN PROGRESS!!! NOT YET RELEASE READY!!!
 
 This client application allows you to **inventory all EnOcean devices**. It can **automatically read and detect devices** from the RS485 bus or from wireless network. After the devices are listed in the EnOcean Device Manager **you can enricht device information** like changing the name, comment or adapt parameters like timeframes, thresholds, units, ... .
 Furthermore, it automatically can detect default settings for Home Assistant configuration which can be adjust as well and it allows you to **generate and export the configuration for Home Assistant**. 
 (The exported Home Assistant configuration is intended for the [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako/))
 
 ## Preview
-<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot.png" /> 
+<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot2.png" /> 
 What you can see here can automatically detected by reading the memory of the bus devices via FAM14. Telegrams of sensors and decentralized devices will be received and additionally added. 
 Additional info for Home Assistant is automatically added. The configuration for Home Assistant can be generated by the detected information.
 For further steps it is planned to extend the support for changing the data which was collected so that a proper management of the devices can be supported.
 
 ## System Requirements / Where to install and how to use it?
 This tool is a desktop application (not browser based) and it runs independent of Home Assistant. Install it directly on a Windows, Linux or Max. (So far only Windows has been tested but all three operating systems should be supported.) Your PC requires Python pre-installed and you should be able to connect it to your EnOcean devices, either via USB cable (Eltako FAM14, FGW14-USB, ...) or wireless transceiver (Eltako FAM-USB). Support for the wireless transceiver 'EnOcean USB300' is planned for future releases.
```

### Comparing `eo_man-0.1.8/eo_man/__main__.py` & `eo_man-0.1.9/eo_man/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .data.app_info import ApplicationInfo
 from .data.data_manager import DataManager
 from .data.ha_config_generator import HomeAssistantConfigurationGenerator
 from .view.main_panel import MainPanel
 from .controller.app_bus import AppBus, AppBusEventType
 
 import logging
-from tkinter import *
 
 
 def cli_argument():
     p = argparse.ArgumentParser(
         description=
 """EnOcean Device Manager (https://github.com/grimmpp/enocean-device-manager) allows you to managed your EnOcean devices and to generate 
 Home Assistant Configurations for the Home Assistant Eltako Integration (https://github.com/grimmpp/home-assistant-eltako).""")
@@ -74,12 +73,11 @@
        e = {'msg': f"Invalid filename {opts.app_config}. It must end with '.eodm'", 'color': 'darkred'}
        app_bus.fire_event(AppBusEventType.LOG_MESSAGE, e)
 
     # generate home assistant config instead of starting GUI
     if opts.app_config and opts.app_config.endswith('.eodm') and opts.ha_config:
         HomeAssistantConfigurationGenerator(app_bus, data_manager).save_as_yaml_to_file(opts.ha_config)
     else:
-        root = Tk()
-        MainPanel(root, app_bus, data_manager)
+        MainPanel(app_bus, data_manager)
 
 if __name__ == "__main__":
     main()
```

### Comparing `eo_man-0.1.8/eo_man/controller/app_bus.py` & `eo_man-0.1.9/eo_man/controller/app_bus.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/controller/serial_controller.py` & `eo_man-0.1.9/eo_man/controller/serial_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,59 +9,55 @@
 import logging
 import threading
 
 from eltakobus import *
 from eltakobus.device import *
 from eltakobus.locking import buslocked, UNLOCKED
 from eltakobus.message import Regular4BSMessage
-from controller.esp3_serial_com import ESP3SerialCommunicator
+from .esp3_serial_com import ESP3SerialCommunicator
 
-from data.device import Device
+from ..data import data_helper
+from ..data.device import Device
+from ..data.const import GatewayDeviceType
 
 from .app_bus import AppBusEventType, AppBus
 
 
 class SerialController():
 
     def __init__(self, app_bus:AppBus) -> None:
         self.app_bus = app_bus
         self._serial_bus = None
         self.current_base_id:str = None
+        self.port_mapping = None
 
         self.app_bus.add_event_handler(AppBusEventType.WINDOW_CLOSED, self.on_window_closed)
     
 
     def on_window_closed(self, data) -> None:
         self.kill_serial_connection_before_exit()
 
-    def get_serial_ports(self, device_type:str) ->list[str]:
+
+    def get_serial_ports(self, device_type:str, force_reload:bool=False) ->list[str]:
+        if force_reload or self.port_mapping is None:
+            self.port_mapping = self._get_gateway2serial_port_mapping()
+
         if device_type == 'FAM14':
-            return self.get_serial_ports_for_fam14()
+            return self.port_mapping[GatewayDeviceType.GatewayEltakoFAM14.value]
         elif device_type == 'FGW14-USB':
-            return self.get_serial_ports_for_fgw14usb()
+            return self.port_mapping[GatewayDeviceType.GatewayEltakoFGW14USB.value]
         elif device_type == 'FAM-USB':
-            return self.get_serial_ports_for_famusb()
+            return self.port_mapping[GatewayDeviceType.GatewayEltakoFAMUSB.value]
         elif device_type == 'USB300':
-            return self.get_serial_ports_for_usb300()
+            return self.port_mapping[GatewayDeviceType.GatewayEnOceanUSB300.value]
         else:
             return []
-
-    def get_serial_ports_for_fam14(self) -> list[str]:
-        return self._get_serial_ports(baudrate=57600, test_fam14=True)
-    
-    def get_serial_ports_for_fgw14usb(self) -> list[str]:
-        return self._get_serial_ports(baudrate=57600, test_fam14=False)
     
-    def get_serial_ports_for_famusb(self) -> list[str]:
-        return self._get_serial_ports(baudrate=9600, test_fam14=False, test_famusb=True)
 
-    def get_serial_ports_for_usb300(self) -> list[str]:
-        return self._get_serial_ports(baudrate=57600, test_fam14=False, test_usb300=True)
-
-    def _get_serial_ports(self, baudrate:int=57600, test_fam14:bool=True, test_famusb:bool=False, test_usb300:bool=False) -> list[str]:
+    def _get_gateway2serial_port_mapping(self) -> dict[str:list[str]]:
         """ Lists serial port names
 
             :raises EnvironmentError:
                 On unsupported or unknown platforms
             :returns:
                 A list of the serial ports available on the system
         """
@@ -73,56 +69,89 @@
             # this excludes your current terminal "/dev/tty"
             ports = glob.glob('/dev/tty[A-Za-z]*')
         elif sys.platform.startswith('darwin'):
             ports = glob.glob('/dev/tty.*')
         else:
             raise EnvironmentError('Unsupported platform')
 
-        result = []
-        for port in ports:
-            try:
-                s = serial.Serial(port, baudrate=baudrate, timeout=0.2)
-                if not test_usb300: s.rs485_mode = serial.rs485.RS485Settings()
-
-                # test fam14
-                fam14_test_request = b'\xff\x00\xff' * 5
-                s.write(fam14_test_request)
-                fam14_test_response = s.read_until(fam14_test_request)
-
-                # test fam-usb and fgw14-usb
-                famusb_test_request = ESP2Message(b'\xAB\x58\x00\x00\x00\x00\x00\x00\x00\x00\x00').serialize()
-                famusb_expected_response = b'\xa5Z\x8b\x98'
-                s.write(famusb_test_request)
-                famusb_test_response = s.read_until(famusb_expected_response)
-                
-                if test_fam14 and fam14_test_request == fam14_test_response: 
-                    result.append(port)
-                    self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FAM14 detected on serial port {port},(baudrate: {baudrate})", 'color':'lightgreen'})
-                elif fam14_test_request == fam14_test_response: 
-                    continue
-
-                if test_famusb and famusb_test_response == famusb_expected_response:
-                    result.append(port)
-                    self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FAM-USB detected on serial port {port},(baudrate: {baudrate})", 'color':'lightgreen'})
-                elif test_famusb:
-                    continue
+        fam14 = GatewayDeviceType.GatewayEltakoFAM14.value
+        usb300 = GatewayDeviceType.GatewayEnOceanUSB300.value
+        famusb = GatewayDeviceType.GatewayEltakoFAMUSB.value
+        fgw14usb = GatewayDeviceType.GatewayEltakoFGW14USB.value
+        result = { fam14: [], usb300: [], famusb: [], fgw14usb: [], 'all': [] }
+
+        count = 0
+        for baud_rate in [9600, 57600]:
+            for port in ports:
+                count += 1
+                # take in 10 as one step and start with 10 to see directly process is running
+                progress = min(round((count/(2*256.0))*10)*10 + 10, 100)
+                self.app_bus.fire_event(AppBusEventType.DEVICE_ITERATION_PROGRESS, progress) 
+
+                try:
+                    # is faster to precheck with serial
+                    s = serial.Serial(port, baudrate=baud_rate, timeout=0.2)
+                    s.rs485_mode = serial.rs485.RS485Settings()
+                    s.close()
+
+                    # test usb300
+                    if baud_rate == 57600:
+                        s = ESP3SerialCommunicator(port, auto_reconnect=False)
+                        s.start()
+                        s.is_serial_connected.wait()
+
+                        if s.base_id and isinstance(s.base_id, list) and port not in result['all']:
+                            result[usb300].append(port)
+                            result['all'].append(port)
+                            self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"USB300 detected on serial port {port},(baudrate: {baud_rate})", 'color':'lightgreen'})
+                            s.stop()
+                            continue
+
+                        s.stop()
+                    
+                    # test fam14, fgw14-usb and fam-usb
+                    s = RS485SerialInterfaceV2(port, baud_rate=baud_rate, delay_message=0.2, auto_reconnect=False)
+                    s.start()
+                    s.is_serial_connected.wait()
+
+                    # test fam14
+                    if s.suppress_echo and port not in result['all']:
+                        result[fam14].append(port)
+                        result['all'].append(port)
+                        self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FAM14 detected on serial port {port},(baudrate: {baud_rate})", 'color':'lightgreen'})
+                        s.stop()
+                        continue
+
+                    # test fam-usb
+                    if baud_rate == 9600:
+                        # try to get base id of fam-usb to test if device is fam-usb
+                        base_id = asyncio.run( self.async_get_base_id_for_fam_usb(s, None) )
+                        # fam14 can answer on both baud rates but fam-usb cannot echo
+                        if base_id is not None and base_id != '00-00-00-00' and not s.suppress_echo and port not in result['all']:
+                            result[famusb].append(port)
+                            result['all'].append(port)
+                            self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FAM-USB detected on serial port {port},(baudrate: {baud_rate})", 'color':'lightgreen'})
+                            s.stop()
+                            continue
+
+                    # fgw14-usb
+                    if baud_rate == 57600:
+                        if not s.suppress_echo and port not in result['all']:
+                            result[fgw14usb].append(port)
+                            result['all'].append(port)
+                            self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FGW14-USB could be on serial port {port},(baudrate: {baud_rate})", 'color':'lightgreen'})
+                            s.stop()
+                            continue
                 
-                if not test_famusb and not test_fam14 and famusb_test_response == famusb_expected_response:
-                    result.append(port)
-                    self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"FGW14-USB detected on serial port {port},(baudrate: {baudrate})", 'color':'lightgreen'})
-
-                # TODO needs to be fixed. just for testing!!!
-                if test_usb300:
-                    result.append(port)
-                    self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"USB300 detected on serial port {port},(baudrate: {baudrate})", 'color':'lightgreen'})
+                    s.stop()
 
-                s.close()
+                except (OSError, serial.SerialException) as e:
+                    pass
 
-            except (OSError, serial.SerialException) as e:
-                pass
+        self.app_bus.fire_event(AppBusEventType.DEVICE_ITERATION_PROGRESS, 0)
         return result
     
     def is_serial_connection_active(self) -> bool:
         return self._serial_bus is not None and self._serial_bus.is_active()
     
     def is_fam14_connection_active(self) -> bool:
         return self.is_serial_connection_active() and self._serial_bus.suppress_echo
@@ -137,17 +166,24 @@
             baudrate = 9600
         elif device_type == 'FAM14':
             delay_message = .001
 
         try:
             if not self.is_serial_connection_active():
                 if device_type == 'USB300':
-                    self._serial_bus = ESP3SerialCommunicator(serial_port, callback=lambda msg: self._send_serial_event(ESP3SerialCommunicator.convert_esp3_to_esp2_message(msg)))
+                    self._serial_bus = ESP3SerialCommunicator(serial_port, 
+                                                              callback=self._send_serial_event,
+                                                              esp2_translation_enabled=True,
+                                                              auto_reconnect=False
+                                                              )
                 else:
-                    self._serial_bus = RS485SerialInterfaceV2(serial_port, baud_rate=baudrate, callback=self._send_serial_event, delay_message=delay_message)
+                    self._serial_bus = RS485SerialInterfaceV2(serial_port, 
+                                                              baud_rate=baudrate, 
+                                                              callback=self._send_serial_event, 
+                                                              delay_message=delay_message)
                 self._serial_bus.start()
                 self._serial_bus.is_serial_connected.wait(timeout=10)
                 
                 if not self._serial_bus.is_active():
                     self._serial_bus.stop()
                 
                 if self._serial_bus.is_active():
@@ -194,15 +230,32 @@
 
         except Exception as e:
             msg = 'Failed to get information about USB300!!!'
             self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': msg, 'log-level': 'ERROR', 'color': 'red'})
             logging.exception(msg, exc_info=True)
             raise e
         finally:
-            self._serial_bus.set_callback( lambda msg: self._send_serial_event(ESP3SerialCommunicator.convert_esp3_to_esp2_message(msg)) )                    
+            self._serial_bus.set_callback( self._send_serial_event )                    
+
+    async def async_get_base_id_for_fam_usb(self, fam_usb:RS485SerialInterfaceV2, callback) -> str:
+        base_id:str = None
+        try:
+            fam_usb.set_callback( None )
+            
+            # get base id
+            data = b'\xAB\x58\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+            # timeout really requires for this command sometimes 1sec!
+            response:ESP2Message = await fam_usb.exchange(ESP2Message(bytes(data)), ESP2Message, retries=3, timeout=1)
+            base_id = b2s(response.body[2:6])
+        except:
+            pass
+        finally:
+            fam_usb.set_callback( callback )
+
+        return base_id
 
     async def async_create_fam_usb_device(self):
         try:
             self._serial_bus.set_callback( None )
             
             # get base id
             data = b'\xAB\x58\x00\x00\x00\x00\x00\x00\x00\x00\x00'
```

### Comparing `eo_man-0.1.8/eo_man/data/app_info.py` & `eo_man-0.1.9/eo_man/data/app_info.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/application_data.py` & `eo_man-0.1.9/eo_man/data/application_data.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/const.py` & `eo_man-0.1.9/eo_man/data/const.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/data_helper.py` & `eo_man-0.1.9/eo_man/data/data_helper.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/data_manager.py` & `eo_man-0.1.9/eo_man/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/device.py` & `eo_man-0.1.9/eo_man/data/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,33 +56,33 @@
         self.name = name
         self.comment = comment
         self.base_id = base_id
         self.use_in_ha = use_in_ha
         self.memory_entries = memory_entries
 
     def is_fam14(self) -> bool:
-        return FAM14.__name__ in self.device_type
+        return self.device_type is not None and FAM14.__name__ in self.device_type
 
     def is_fam_usb(self) -> bool:
-        return 'FAM-USB' in self.device_type or 'FAM_USB' in self.device_type
+        return self.device_type is not None and ('FAM-USB' in self.device_type or 'FAM_USB' in self.device_type)
     
     def is_fgw14_usb(self) -> bool:
-        return 'FGW14_USB' in self.device_type
+        return self.device_type is not None and 'FGW14_USB' in self.device_type
 
     def is_usb300(self) -> bool:
-        return 'USB300' in self.device_type
+        return self.device_type is not None and 'USB300' in self.device_type
 
     def is_gateway(self) -> bool:
         return self.is_wired_gateway() or self.is_wireless_tranceiver()
     
     def is_wired_gateway(self) -> bool:
         return self.is_fam14() or self.is_fgw14_usb()
 
     def is_wireless_tranceiver(self) -> bool:
-        return self.is_usb300() or self.is_fam_usb() or 'Wireless Tranceiver' in self.device_type
+        return self.is_usb300() or self.is_fam_usb() or (self.device_type is not None and 'Wireless Tranceiver' in self.device_type)
     
     def is_bus_device(self) -> bool:
         return self.bus_device
         # return self.address.startswith('00-00-00-')            
 
     @classmethod
     def merge_devices(cls, device1, device2):
```

### Comparing `eo_man-0.1.8/eo_man/data/filter.py` & `eo_man-0.1.9/eo_man/data/filter.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/ha_config_generator.py` & `eo_man-0.1.9/eo_man/data/ha_config_generator.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/data/homeassistant/const.py` & `eo_man-0.1.9/eo_man/data/homeassistant/const.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Breathe-about.png` & `eo_man-0.1.9/eo_man/icons/Breathe-about.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Faenza-system-search.png` & `eo_man-0.1.9/eo_man/icons/Faenza-system-search.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Gnome-help-faq.png` & `eo_man-0.1.9/eo_man/icons/Gnome-help-faq.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Home_Assistant_Logo.png` & `eo_man-0.1.9/eo_man/icons/Home_Assistant_Logo.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Oxygen480-actions-document-save-as.png` & `eo_man-0.1.9/eo_man/icons/Oxygen480-actions-document-save-as.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Oxygen480-actions-document-save.png` & `eo_man-0.1.9/eo_man/icons/Oxygen480-actions-document-save.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Oxygen480-actions-help.png` & `eo_man-0.1.9/eo_man/icons/Oxygen480-actions-help.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Oxygen480-status-folder-open.png` & `eo_man-0.1.9/eo_man/icons/Oxygen480-status-folder-open.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/Software-update-available.png` & `eo_man-0.1.9/eo_man/icons/Software-update-available.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/export_icon.png` & `eo_man-0.1.9/eo_man/icons/export_icon.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/github_icon.png` & `eo_man-0.1.9/eo_man/icons/github_icon.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/image_gallary.py` & `eo_man-0.1.9/eo_man/icons/image_gallary.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,36 @@
 from PIL import Image, ImageTk
 
 # icon list
 # https://commons.wikimedia.org/wiki/Comparison_of_icon_sets
 
 class ImageGallery():
 
+    # is needed to keep a reference to the images otherwise they will not displayed in the icons
+    _images:dict[str:ImageTk.PhotoImage] = {}
+
+    @classmethod
+    def get_image(cls, filename, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        id = f"{filename}_{size[0]}_{size[0]}"
+        if id not in cls._images:
+            with Image.open(os.path.join(os.path.dirname(__file__), filename)) as img:
+                if size is not None:
+                    _img = img.resize(size, Image.LANCZOS)
+                img = ImageTk.PhotoImage(_img)
+                cls._images[id] = img
+
+        return cls._images[id]
+
+    @classmethod
+    def get_eo_man_logo(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("Faenza-system-search.png", size)
+
     @classmethod
-    def get_image(cls, filename, size:tuple[int:int]=(32,32)):
-        img = Image.open(os.path.join(os.path.dirname(__file__), filename))
-        if size is not None:
-            img = img.resize(size, Image.LANCZOS)
-        return ImageTk.PhotoImage(img)
+    def get_blank(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("blank.png", size)
 
     @classmethod
     def get_ha_logo(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
         return ImageGallery.get_image("Home_Assistant_Logo.png", size)
     
     @classmethod
     def get_open_folder_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
@@ -47,8 +63,36 @@
 
     @classmethod
     def get_github_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
         return ImageGallery.get_image("github_icon.png", size)
     
     @classmethod
     def get_software_update_available_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
-        return ImageGallery.get_image("Software-update-available.png", size)
+        return ImageGallery.get_image("Software-update-available.png", size)
+    
+    @classmethod
+    def get_fam14_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("fam14.png", size)
+    
+    @classmethod
+    def get_usb300_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("usb300.png", size)
+    
+    @classmethod
+    def get_fam_usb_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("fam-usb2.png", size)
+    
+    @classmethod
+    def get_fgw14_usb_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("fgw14-usb.png", size)
+    
+    @classmethod
+    def get_wireless_network_in_color_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("wireless-network-colored.png", size)
+    
+    @classmethod
+    def get_wireless_network_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("wireless-network-bw.png", size)
+    
+    @classmethod
+    def get_wireless_icon(cls, size:tuple[int:int]=(32,32)) -> ImageTk.PhotoImage:
+        return ImageGallery.get_image("wireless.png", size)
```

### Comparing `eo_man-0.1.8/eo_man/icons/paypal_icon.png` & `eo_man-0.1.9/eo_man/icons/paypal_icon.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/icons/paypal_me_badge.png` & `eo_man-0.1.9/eo_man/icons/paypal_me_badge.png`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/view/about_window.py` & `eo_man-0.1.9/eo_man/view/about_window.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/view/checklistcombobox.py` & `eo_man-0.1.9/eo_man/view/checklistcombobox.py`

 * *Files identical despite different names*

### Comparing `eo_man-0.1.8/eo_man/view/device_details.py` & `eo_man-0.1.9/eo_man/view/device_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         self.app_bus = app_bus
         self.data_manager = data_manager
         self.current_device = None
 
         self.app_bus.add_event_handler(AppBusEventType.SELECTED_DEVICE, self.selected_device_handler)
 
         # main
-        main_frame = Frame(main, width=370)
+        main_frame = Frame(main, width=350)
         main_frame.pack(fill=BOTH, expand=1)
 
         # canvas
-        canvas = Canvas(main_frame, width=250)
+        canvas = Canvas(main_frame, width=350)
         canvas.pack(side=LEFT, fill=BOTH, expand=1)
 
         # scrollbar
         scrollbar = tk.Scrollbar(main_frame, orient=VERTICAL, command=canvas.yview)
         scrollbar.pack(side=RIGHT, fill=Y)
 
         # configure the canvas
@@ -56,63 +56,64 @@
 
         c_row = 0
 
         # name
         l = Label(f, text="Name")
         l.grid(row=0, column=0, sticky=W, padx=3)
 
-        self.text_name = Entry(f)
+        self.text_name = ttk.Entry(f)
         self.text_name.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_name, device.name, NORMAL)
         self.text_name.bind('<Return>', lambda e, d=device: self.update_device(d))
         
 
         # address
         c_row += 1
         l = Label(f, text="Address")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
 
-        self.text_address = Entry(f)
+        self.text_address = ttk.Entry(f)
         self.text_address.insert(END, "00-00-00-00")
-        self.text_address.config(state=DISABLED)
+        self.text_address.config(state=NORMAL)
         self.text_address.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_address, device.address)
-        self.text_address.bind('<Return>', lambda e, d=device: self.update_device(d))
+        # self.text_address.bind('<Return>', lambda e, d=device: self.update_device(d))
+        self.text_address.bind_all('<Key>', lambda e: [])
 
         # base id
         c_row += 1
         l = Label(f, text="Base Id")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
 
-        self.text_address = Entry(f)
+        self.text_address = ttk.Entry(f)
         self.text_address.insert(END, "00-00-00-00")
         self.text_address.config(state=DISABLED)
         self.text_address.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_address, device.base_id)
         # self.text_address.bind('<Return>', lambda e, d=device: self.update_device(d))
 
         # external address
         c_row += 1
         l = Label(f, text="External Id")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
 
-        self.text_ext_address = Entry(f)
+        self.text_ext_address = ttk.Entry(f)
         self.text_ext_address.insert(END, "00-00-00-00")
         self.text_ext_address.config(state=DISABLED)
         self.text_ext_address.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_ext_address, device.external_id)
         self.text_ext_address.bind('<Return>', lambda e, d=device: self.update_device(d))
 
 
         # version
         c_row += 1
         l = Label(f, text="Version")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
 
-        self.text_version = Entry(f)
+        self.text_version = ttk.Entry(f)
         self.text_version.config(state=DISABLED)
         self.text_version.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_version, device.version)
         self.text_version.bind('<Return>', lambda e, d=device: self.update_device(d))
 
 
         # device type
@@ -144,15 +145,15 @@
 
 
         # comment
         c_row += 1
         l = Label(f, text="Comment")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
 
-        self.text_comment = Entry(f)
+        self.text_comment = ttk.Entry(f)
         self.text_comment.grid(row=c_row, column=1, sticky=W+E)
         self._update_text_field(self.text_comment, device.comment, NORMAL)
         self.text_comment.bind('<Return>', lambda e, d=device: self.update_device(d))
 
         c_row += 1
         l = Label(f, text="Device EEP")
         l.grid(row=c_row, column=0, sticky=W, padx=3)
@@ -164,15 +165,15 @@
         self.cb_device_eep.set(device.eep if device.eep else '')
         self.cb_device_eep.bind('<Return>', lambda e, d=device: self.update_device(d))
 
 
         # in HA
         c_row += 1
         self.cb_export_ha_var = tk.IntVar()
-        cb = Checkbutton(f, text="Export to HA Config", variable=self.cb_export_ha_var)
+        cb = ttk.Checkbutton(f, text="Export to HA Config", variable=self.cb_export_ha_var)
         cb.grid(row=c_row, column=0, columnspan=2, padx=3, sticky=W)
         self.cb_export_ha_var.set(1 if device.use_in_ha else 0)
         cb.bind('<Return>', lambda e, d=device: self.update_device(d))
 
         # HA platform
         c_row += 1
         l = Label(f, text="HA Platform")
```

### Comparing `eo_man-0.1.8/eo_man/view/device_table.py` & `eo_man-0.1.9/eo_man/view/device_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import threading
 import time
-import tkinter as tk
-import os
-from pathlib import Path
 from tkinter import *
 from tkinter import ttk
-from tkinter import filedialog
-from tkinter.tix import IMAGETEXT
-from PIL import Image, ImageTk
-from idlelib.tooltip import Hovertip
 
 from ..controller.app_bus import AppBus, AppBusEventType
 from ..data.const import *
 from ..data.homeassistant.const import CONF_ID, CONF_NAME
 from ..data.filter import DataFilter
 from ..data.data_manager import DataManager, Device
 from ..data import data_helper
+from ..icons.image_gallary import ImageGallery
 
 from eltakobus.util import b2s
-from eltakobus.eep import EEP
 from eltakobus.message import EltakoMessage, RPSMessage, Regular1BSMessage, Regular4BSMessage, EltakoWrappedRPS
 
 
 class DeviceTable():
 
+    ICON_SIZE = (20,20)
     NON_BUS_DEVICE_LABEL:str="Distributed Devices"
 
     def __init__(self, main: Tk, app_bus:AppBus, data_manager:DataManager):
         
         self.blinking_enabled = True
         self.pane = ttk.Frame(main, padding=2)
         # self.pane.grid(row=0, column=0, sticky=W+E+N+S)
@@ -40,14 +34,15 @@
         xscrollbar = ttk.Scrollbar(self.pane, orient=HORIZONTAL)
         xscrollbar.pack(side=BOTTOM, fill=X)
 
         # Treeview
         columns = ("Address", "External Address", "Device Type", "Key Function", "Comment", "Export to HA Config", "HA Platform", "Device EEP", "Sender Address", "Sender EEP")
         self.treeview = ttk.Treeview(
             self.pane,
+            show="tree headings", 
             selectmode="browse",
             yscrollcommand=yscrollbar.set,
             xscrollcommand=xscrollbar.set,
             columns=(0,1,2,3,4,5,6,7,8,9),
             height=10,
         )
         self.treeview.pack(expand=True, fill=BOTH)
@@ -110,29 +105,32 @@
         # initial loading
         if self.data_manager.selected_data_filter_name is not None:
             self._set_data_filter_handler(self.data_manager.data_fitlers[self.data_manager.selected_data_filter_name])
         for d in self.data_manager.devices.values():
             parent = self.NON_BUS_DEVICE_LABEL if not d.is_bus_device() else None
             self.update_device_handler(d, parent)
 
+
     def _set_data_filter_handler(self, filter):
         self.current_data_filter = filter
 
         self._reset(None)
         for d in self.data_manager.devices.values():
             if d.bus_device:
                 self.update_device_handler(d)
             else:
                 self.update_device_handler(d, parent=self.NON_BUS_DEVICE_LABEL)
 
+
     def _reset(self, data):
         for item in self.treeview.get_children():
             self.treeview.delete(item)
         self.check_if_wireless_network_exists()
 
+
     def on_selected(self, event):
         device_external_id = self.treeview.focus()
         device = self.data_manager.get_device_by_id(device_external_id)
         if device is not None:
             self.app_bus.fire_event(AppBusEventType.SELECTED_DEVICE, device)
 
         self.mark_related_elements(device_external_id)
@@ -150,17 +148,19 @@
 
     def show_context_menu(self, event):
         try:
             self.menu.tk_popup(event.x_root, event.y_root)
         finally:
             self.menu.grab_release()
 
+
     def insert_device(self, device:Device):
         v=("", b2s(device.address[0]), "", "")
         self.treeview.insert(parent="", index="end", text=device.id_string, values=v)
+
         
     def device_scan_status_handler(self, status:str):
         if status in ['STARTED']:
             #TODO: disable treeview or menue of it
             # self.treeview.config(state=DISABLED)
             pass
         elif status in ['FINISHED']:
@@ -173,23 +173,39 @@
         if d.is_fam14():
             if not self.treeview.exists(d.base_id):
                 text = ""
                 comment = ""
                 text = d.name
                 comment = d.comment if d.comment is not None else "" 
                 in_ha = d.use_in_ha
-                self.treeview.insert(parent="", index=0, iid=d.external_id, text=text, values=("", "", "", "", comment, in_ha, "", "", ""), open=True)
+                self.treeview.insert(parent="", 
+                                     index=0, 
+                                     iid=d.external_id, 
+                                     text=" " + text, 
+                                     values=("", "", "", "", comment, in_ha, "", "", ""),
+                                     image=ImageGallery.get_fam14_icon(self.ICON_SIZE),
+                                     open=True)
             else:
-                self.treeview.item(d.base_id, text=d.name, values=("", "", "", "", d.comment, d.use_in_ha, "", "", "") )
+                self.treeview.item(d.base_id, 
+                                   text=" " + d.name, 
+                                   values=("", "", "", "", d.comment, d.use_in_ha, "", "", ""),
+                                   image=ImageGallery.get_fam14_icon(self.ICON_SIZE), 
+                                   open=True)
 
 
     def check_if_wireless_network_exists(self):
         id = self.NON_BUS_DEVICE_LABEL
         if not self.treeview.exists(id):
-            self.treeview.insert(parent="", index="end", iid=id, text=self.NON_BUS_DEVICE_LABEL, values=("", "", "", "", "", "", "", "", ""), open=True)
+            self.treeview.insert(parent="", 
+                                 index="end", 
+                                 iid=id, 
+                                 text=" " + self.NON_BUS_DEVICE_LABEL, 
+                                 values=("", "", "", "", "", "", "", "", ""), 
+                                 image=ImageGallery.get_wireless_icon(self.ICON_SIZE),
+                                 open=True)
 
 
     def update_device_representation_handler(self, d:Device):
         self.update_device_handler(d)
 
 
     def update_device_handler(self, d:Device, parent:str=None):
@@ -202,27 +218,47 @@
             ha_pl = "" if d.ha_platform is None else d.ha_platform
             eep = "" if d.eep is None else d.eep
             device_type = "" if d.device_type is None else d.device_type
             key_func = "" if d.key_function is None else d.key_function
             comment = "" if d.comment is None else d.comment
             sender_adr = "" if 'sender' not in d.additional_fields else d.additional_fields['sender'][CONF_ID]
             sender_eep = "" if 'sender' not in d.additional_fields else d.additional_fields['sender'][CONF_EEP]
+            
+            if d.is_usb300():
+                image = ImageGallery.get_usb300_icon(self.ICON_SIZE)
+            elif d.is_fam_usb():
+                image = ImageGallery.get_fam_usb_icon(self.ICON_SIZE)
+            elif d.is_fgw14_usb():
+                image = ImageGallery.get_fgw14_usb_icon(self.ICON_SIZE)
+            else:
+                image = ImageGallery.get_blank(self.ICON_SIZE)
+
             _parent = d.base_id if parent is None else parent
             if not self.treeview.exists(_parent): self.add_fam14(self.data_manager.devices[_parent])
             if not self.treeview.exists(d.external_id):
-                self.treeview.insert(parent=_parent, index="end", iid=d.external_id, text=d.name, values=(d.address, d.external_id, device_type, key_func, comment, in_ha, ha_pl, eep, sender_adr, sender_eep), open=True)
+                self.treeview.insert(parent=_parent, 
+                                     index="end", 
+                                     iid=d.external_id, 
+                                     text=" " + d.name, 
+                                     values=(d.address, d.external_id, device_type, key_func, comment, in_ha, ha_pl, eep, sender_adr, sender_eep), 
+                                     open=True)
+                self.treeview.item(d.external_id, image=image)
             else:
                 # update device
-                self.treeview.item(d.external_id, text=d.name, values=(d.address, d.external_id, device_type, key_func, comment, in_ha, ha_pl, eep, sender_adr, sender_eep), open=True)
+                self.treeview.item(d.external_id, 
+                                   text=" " + d.name, 
+                                   values=(d.address, d.external_id, device_type, key_func, comment, in_ha, ha_pl, eep, sender_adr, sender_eep), 
+                                   image=image,
+                                   open=True)
                 if self.treeview.parent(d.external_id) != _parent:
                     self.treeview.move(d.external_id, _parent, 0)
         else:
             self.add_fam14(d)
-
         # self.trigger_blinking(d.external_id)
+            
 
     def _serial_callback_handler(self, data:dict):
         message:EltakoMessage = data['msg']
         current_base_id:str = data['base_id']
 
         if type(message) in [RPSMessage, Regular1BSMessage, Regular4BSMessage, EltakoWrappedRPS]:
             if isinstance(message.address, int):
@@ -233,14 +269,15 @@
             if not adr.startswith('00-00-00-'):
                 self.trigger_blinking(adr)
             elif current_base_id is not None:
                 d:Device = self.data_manager.find_device_by_local_address(adr, current_base_id)
                 if d is not None:
                     self.trigger_blinking(d.external_id)
 
+
     def trigger_blinking(self, external_id:str):
         if not self.blinking_enabled:
             return
         
         def blink(ext_id:str):
             for i in range(0,2):
                 if self.treeview.exists(ext_id):
```

### Comparing `eo_man-0.1.8/eo_man/view/donation_button.py` & `eo_man-0.1.9/eo_man/view/donation_button.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import os
 from tkinter import *
-from PIL import Image, ImageTk
+from tkinter import ttk
 import webbrowser
 from idlelib.tooltip import Hovertip
 
 from ..icons.image_gallary import ImageGallery
 
-class DonationButton(Button):
+class DonationButton(ttk.Button):
 
     def __init__(self, master=None, cnf={}, **kw):
         if 'small_icon' in kw and kw['small_icon']:
             image = ImageGallery.get_paypal_icon()
         else:
             image = ImageGallery.get_paypal_me_icon()
         
-        super().__init__(master, image=image, relief=kw.get('relief', FLAT), cursor="hand2", command=self.open_payapl_me)
+        super().__init__(master, image=image, cursor="hand2", command=self.open_payapl_me) # , relief=kw.get('relief', FLAT))
         self.image = image
 
         Hovertip(self,"Donate to support this project!",300)
 
         self.bind('<Return>', lambda e: self.open_payapl_me())
 
     def open_payapl_me(self):
```

### Comparing `eo_man-0.1.8/eo_man/view/filter_bar.py` & `eo_man-0.1.9/eo_man/view/filter_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,50 +28,50 @@
         l.grid(row=0, column=col, padx=(3,3), sticky=W)
 
         self.cb_filtername = ttk.Combobox(f, width="14") 
         self.cb_filtername.grid(row=1, column=col, padx=(0,3) )
         self.cb_filtername.bind('<Return>', lambda e: [self.load_filter(), self.add_filter(False), self.apply_filter(e, True)] )
 
         col += 1
-        self.btn_save_filter = Button(f, text="Load", command=self.load_filter)
+        self.btn_save_filter = ttk.Button(f, text="Load", command=self.load_filter)
         self.btn_save_filter.grid(row=1, column=col, padx=(0,3))
 
         col += 1
-        self.btn_save_filter = Button(f, text="Remove", command=self.remove_filter)
+        self.btn_save_filter = ttk.Button(f, text="Remove", command=self.remove_filter)
         self.btn_save_filter.grid(row=0, column=col, padx=(0,3) )
 
-        self.btn_save_filter = Button(f, text="Add", command=self.add_filter)
+        self.btn_save_filter = ttk.Button(f, text="Add", command=self.add_filter)
         self.btn_save_filter.grid(row=1, column=col, padx=(0,3), sticky=W+E )
 
         # global filter
         col += 1
         l = Label(f, text="Global Filter:")
         l.grid(row=0, column=col, padx=(0,3), sticky=W)
 
-        self.global_filter = Entry(f, width="14") 
+        self.global_filter = ttk.Entry(f, width="14") 
         self.global_filter.grid(row=1, column=col, padx=(0,3) )
         self.global_filter.bind('<Return>', self.apply_filter)
         self.global_filter.bind("<KeyRelease>", lambda e: self.cb_filtername.set('') )
 
         # address
         col += 1
         l = Label(f, text="Address:")
         l.grid(row=0, column=col, padx=(0,3), sticky=W)
 
-        self.cb_device_address = Entry(f, width="14") 
+        self.cb_device_address = ttk.Entry(f, width="14") 
         self.cb_device_address.grid(row=1, column=col, padx=(0,3) )
         self.cb_device_address.bind('<Return>', self.apply_filter)
         self.cb_device_address.bind("<KeyRelease>", lambda e: self.cb_filtername.set('') )
 
         # external address
         col += 1
         l = Label(f, text="External Address:")
         l.grid(row=0, column=col, padx=(0,3), sticky=W)
 
-        self.cb_external_address = Entry(f, width="14") 
+        self.cb_external_address = ttk.Entry(f, width="14") 
         self.cb_external_address.grid(row=1, column=col, padx=(0,3) )
         self.cb_external_address.bind('<Return>', self.apply_filter)
         self.cb_external_address.bind("<KeyRelease>", lambda e: self.cb_filtername.set('') )
 
         # device type
         col += 1
         l = Label(f, text="Device Type:")
@@ -102,19 +102,19 @@
         self.cb_in_ha.grid(row=1, column=col, padx=(0,3) )
         self.cb_in_ha.bind('<Return>', self.apply_filter)
         self.cb_in_ha.bind('<Button-1>', lambda e: self.cb_filtername.set('') )
 
 
         # button reset
         col += 1
-        self.btn_clear_filter = Button(f, text="Reset", command=self.reset_filter)
+        self.btn_clear_filter = ttk.Button(f, text="Reset", command=self.reset_filter)
         self.btn_clear_filter.grid(row=1, column=col, padx=(0,3) )
 
         col += 1
-        self.btn_apply_filter = Button(f, text="Apply", command=self.apply_filter)
+        self.btn_apply_filter = ttk.Button(f, text="Apply", command=self.apply_filter)
         self.btn_apply_filter.grid(row=1, column=col, padx=(0,3) )
 
         self.app_bus.add_event_handler(AppBusEventType.SET_DATA_TABLE_FILTER, self.on_set_filter_handler)
         self.app_bus.add_event_handler(AppBusEventType.ADDED_DATA_TABLE_FILTER, self.on_filter_added_handler)
         self.app_bus.add_event_handler(AppBusEventType.REMOVED_DATA_TABLE_FILTER, self.on_filter_removed_handler)
 
         ## initiall add all filters
```

### Comparing `eo_man-0.1.8/eo_man/view/log_output.py` & `eo_man-0.1.9/eo_man/view/log_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.app_bus = app_bus
         self.data_manager = data_manager
 
         pane = ttk.Frame(main, padding=2, height=100)
         # pane.grid(row=2, column=0, sticky="nsew", columnspan=3)
         self.root = pane
 
-        self.st = ScrolledText.ScrolledText(pane, border=3, height=10, state='disabled', bg='black', fg='lightgrey', font=('Arial', 14), padx=5, pady=5)
+        self.st = ScrolledText.ScrolledText(pane, border=3, height=10, state=DISABLED, bg='black', fg='lightgrey', font=('Arial', 14), padx=5, pady=5)
         self.st.configure(font='TkFixedFont')
         self.st.pack(expand=True, fill="both")
         # self.st.grid(row=2, column=0, sticky="nsew", columnspan=3)
 
         app_bus.add_event_handler(AppBusEventType.SERIAL_CALLBACK, self.serial_callback)
         app_bus.add_event_handler(AppBusEventType.LOG_MESSAGE, self.receive_log_message)
```

### Comparing `eo_man-0.1.8/eo_man/view/main_panel.py` & `eo_man-0.1.9/eo_man/view/main_panel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
-import os
-import sys
-import copy
 
-import tkinter as tk
 from tkinter import *
 from tkinter import ttk
 
+from ..icons.image_gallary import ImageGallery
+
 from ..controller.app_bus import AppBus, AppBusEventType
 
 from ..data.data_manager import DataManager
 
 from ..view import DEFAULT_WINDOW_TITLE
 from ..view.device_details import DeviceDetails
 from ..view.device_table import DeviceTable
@@ -19,44 +17,42 @@
 from ..view.menu_presenter import MenuPresenter
 from ..view.serial_communication_bar import SerialConnectionBar
 from ..view.status_bar import StatusBar
 from ..view.tool_bar import ToolBar
 
 class MainPanel():
 
-    def __init__(self, main: Tk, app_bus:AppBus, data_manager: DataManager):
-        self.main = main
+    def __init__(self, app_bus:AppBus, data_manager: DataManager):
+        self.main = Tk()
         self.app_bus = app_bus
         ## init main window
         self._init_window()
 
-        self.main
-
         ## define grid
         row_button_bar = 0
         row_serial_con_bar = 1
         row_filter_bar = 2
         row_main_area = 3
         row_status_bar = 4
-        main.rowconfigure(row_button_bar, weight=0, minsize=38)      # button bar
-        main.rowconfigure(row_serial_con_bar, weight=0, minsize=38)      # serial connection bar
-        main.rowconfigure(row_filter_bar, weight=0, minsize=38)      # table filter bar
-        main.rowconfigure(row_main_area, weight=5, minsize=100)     # treeview
+        self.main.rowconfigure(row_button_bar, weight=0, minsize=38)      # button bar
+        self.main.rowconfigure(row_serial_con_bar, weight=0, minsize=38)      # serial connection bar
+        self.main.rowconfigure(row_filter_bar, weight=0, minsize=38)      # table filter bar
+        self.main.rowconfigure(row_main_area, weight=5, minsize=100)     # treeview
         # main.rowconfigure(2, weight=1, minsize=30)    # logview
-        main.rowconfigure(row_status_bar, weight=0, minsize=30)      # status bar
-        main.columnconfigure(0, weight=1, minsize=100)
+        self.main.rowconfigure(row_status_bar, weight=0, minsize=30)      # status bar
+        self.main.columnconfigure(0, weight=1, minsize=100)
 
         ## init presenters
-        mp = MenuPresenter(main, app_bus, data_manager)
+        mp = MenuPresenter(self.main, app_bus, data_manager)
         
-        ToolBar(main, mp, row=row_button_bar)
-        SerialConnectionBar(main, app_bus, data_manager, row=row_serial_con_bar)
-        FilterBar(main, app_bus, data_manager, row=row_filter_bar)
+        ToolBar(self.main, mp, row=row_button_bar)
+        SerialConnectionBar(self.main, app_bus, data_manager, row=row_serial_con_bar)
+        FilterBar(self.main, app_bus, data_manager, row=row_filter_bar)
         # main area
-        main_split_area = ttk.PanedWindow(main, orient="vertical")
+        main_split_area = ttk.PanedWindow(self.main, orient="vertical")
         main_split_area.grid(row=row_main_area, column=0, sticky="nsew", columnspan=4)
         
         data_split_area = ttk.PanedWindow(main_split_area, orient="horizontal")
         # data_split_area = Frame(main_split_area)
         # data_split_area.columnconfigure(0, weight=5)
         # data_split_area.columnconfigure(0, weight=0, minsize=100)
         
@@ -68,39 +64,50 @@
         main_split_area.add(lo.root, weight=1)
 
         data_split_area.add(dt.root, weight=5)
         data_split_area.add(dd.root, weight=0)
         # dt.root.grid(row=0, column=0, sticky="nsew")
         # dd.root.grid(row=0, column=1, sticky="nsew")
 
-        StatusBar(main, app_bus, data_manager, row=row_status_bar)
+        StatusBar(self.main, app_bus, data_manager, row=row_status_bar)
 
-        main.after(1, lambda: main.focus_force())
+        self.main.after(1, lambda: self.main.focus_force())
 
         ## start main loop
-        main.mainloop()
+        self.main.mainloop()
 
         
         
 
 
     def _init_window(self):
         self.main.title(DEFAULT_WINDOW_TITLE)
+
+        #style
+        style = ttk.Style()
+        style_theme = 'xpnative' # 'clam'
+        self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"Available style themes: {ttk.Style().theme_names()}", 'log-level': 'DEBUG'})
+        try:
+            style.theme_use(style_theme)
+        except:
+            self.app_bus.fire_event(AppBusEventType.LOG_MESSAGE, {'msg': f"Cannot load style theme {style_theme}!", 'log-level': 'WARNING'})
+
         self.main.geometry("1400x600")  # set starting size of window
         # self.main.attributes('-fullscreen', True)
         # self.main.state('zoomed') # opens window maximized
+
         self.main.config(bg="lightgrey")
         self.main.protocol("WM_DELETE_WINDOW", self.on_closing)
-        filename = os.path.join(os.path.dirname(__file__), '..', 'icons', 'Faenza-system-search.png')
+
         # icon next to title in window frame
-        # self.main.wm_iconphoto(False, tk.PhotoImage(file=filename))
+        self.main.wm_iconphoto(False, ImageGallery.get_eo_man_logo())
+
         # icon in taskbar
-        icon = tk.PhotoImage(file=filename)
+        icon = ImageGallery.get_eo_man_logo()
         self.main.iconphoto(True, icon, icon)
-        # self.main.iconbitmap(bitmap=filename.replace('.png', '.icon'))
 
     def on_loaded(self) -> None:
         self.app_bus.fire_event(AppBusEventType.WINDOW_LOADED, {})
 
     def on_closing(self) -> None:
         self.app_bus.fire_event(AppBusEventType.WINDOW_CLOSED, {})
         logging.info("Close Application eo-man")
```

### Comparing `eo_man-0.1.8/eo_man/view/menu_presenter.py` & `eo_man-0.1.9/eo_man/view/menu_presenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import threading
 from tkinter import *
+from tkinter import ttk
 from tkinter import filedialog
 import logging
 from tkinter import messagebox
 import webbrowser
 
 from ..controller.app_bus import AppBus, AppBusEventType
```

### Comparing `eo_man-0.1.8/eo_man/view/serial_communication_bar.py` & `eo_man-0.1.9/eo_man/view/serial_communication_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from idlelib.tooltip import Hovertip
 import threading
 
 from eo_man import LOGGER
 
 from ..controller.app_bus import AppBus, AppBusEventType
 from ..controller.serial_controller import SerialController
-from ..data.data_manager import DataManager, Device
+from ..data.data_manager import DataManager
 
 class SerialConnectionBar():
 
     def __init__(self, main: Tk, app_bus:AppBus, data_manager:DataManager, row:int):
         self.main = main
         self.app_bus = app_bus
         self.data_manager = data_manager
         self.serial_cntr = SerialController(app_bus)
 
         f = LabelFrame(main, text="Serial Connection", bd=1)#, relief=SUNKEN)
         f.grid(row=row, column=0, columnspan=1, sticky=W+E+N+S, pady=(0,2), padx=2)
 
-        self.b_detect = Button(f, text="Detect Serial Ports")
+        self.b_detect = ttk.Button(f, text="Detect Serial Ports")
         self.b_detect.pack(side=tk.LEFT, padx=(5, 5), pady=5)
-        self.b_detect.config(command=self.detect_serial_ports_command)
+        self.b_detect.config(command=lambda : self.detect_serial_ports_command(force_reload=True) )
         Hovertip(self.b_detect,"Serial port detection is sometime unstable. Please try again if device was not detected.",300)
 
         l = Label(f, text="Gateway Type: ")
         l.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         self.cb_device_type = ttk.Combobox(f, state="readonly", width="12") 
         self.cb_device_type.pack(side=tk.LEFT, padx=(0, 5), pady=5)
@@ -37,31 +37,31 @@
 
         l = Label(f, text="Serial Port: ")
         l.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         self.cb_serial_ports = ttk.Combobox(f, state="readonly", width="10") 
         self.cb_serial_ports.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
-        self.b_connect = Button(f, text="Connect", state=DISABLED, command=self.toggle_serial_connection_command)
+        self.b_connect = ttk.Button(f, text="Connect", state=DISABLED, command=self.toggle_serial_connection_command)
         self.b_connect.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         s = ttk.Separator(f, orient=VERTICAL )
         s.pack(side=tk.LEFT, padx=(0,5), pady=0, fill="y")
 
-        self.b_scan = Button(f, text="Scan for devices", state=DISABLED, command=self.scan_for_devices)
+        self.b_scan = ttk.Button(f, text="Scan for devices", state=DISABLED, command=self.scan_for_devices)
         self.b_scan.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         self.overwrite = tk.BooleanVar()
-        self.cb_overwrite = Checkbutton(f, text="Overwrite existing values", variable=self.overwrite)
+        self.cb_overwrite = ttk.Checkbutton(f, text="Overwrite existing values", variable=self.overwrite)
         self.cb_overwrite.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         s = ttk.Separator(f, orient=VERTICAL )
         s.pack(side=tk.LEFT, padx=(0,5), pady=0, fill="y")
 
-        self.b_sync_ha_sender = Button(f, text="Write HA senders to devices", state=DISABLED, command=self.write_ha_senders_to_devices)
+        self.b_sync_ha_sender = ttk.Button(f, text="Write HA senders to devices", state=DISABLED, command=self.write_ha_senders_to_devices)
         Hovertip(self.b_sync_ha_sender,"Ensures sender configuration for Home Assistant is written into device memory.",300)
         self.b_sync_ha_sender.pack(side=tk.LEFT, padx=(0, 5), pady=5)
 
         self.app_bus.add_event_handler(AppBusEventType.CONNECTION_STATUS_CHANGE, self.is_connected_handler)
         self.app_bus.add_event_handler(AppBusEventType.DEVICE_SCAN_STATUS, self.device_scan_status_handler)
         self.app_bus.add_event_handler(AppBusEventType.WRITE_SENDER_IDS_TO_DEVICES_STATUS, self.device_scan_status_handler)
         self.app_bus.add_event_handler(AppBusEventType.WINDOW_LOADED, self.on_window_loaded)
@@ -142,21 +142,25 @@
             self.cb_serial_ports.config(state="readonly")
             self.cb_device_type.config(state="readonly")
             self.b_scan.config(state=DISABLED)
             self.b_sync_ha_sender.config(state=DISABLED)
             if not skipp_serial_port_detection: self.detect_serial_ports_command()
 
 
-    def detect_serial_ports_command(self):
+    def detect_serial_ports_command(self, force_reload:bool=False):
 
         def detect_serial_ports():
             try:
                 self.main.config(cursor="watch")    #set cursor for waiting
                 self.b_detect.config(state=DISABLED)
-                serial_ports = self.serial_cntr.get_serial_ports(self.cb_device_type.get())
+                self.cb_device_type.config(state=DISABLED)
+                self.cb_serial_ports.config(state=DISABLED)
+                serial_ports = self.serial_cntr.get_serial_ports(self.cb_device_type.get(), force_reload)
+                self.cb_device_type.config(state=NORMAL)
+                self.cb_device_type.config(state=NORMAL)
                 self.cb_serial_ports['values'] = serial_ports
                 if len(self.cb_serial_ports['values']) > 0:
                     self.cb_serial_ports.set(self.cb_serial_ports['values'][0])
                     self.b_connect.config(state=NORMAL)
                 else:
                     self.b_connect.config(state=DISABLED)
                     self.cb_serial_ports.set('')
```

### Comparing `eo_man-0.1.8/eo_man/view/status_bar.py` & `eo_man-0.1.9/eo_man/view/status_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, main: Tk, app_bus:AppBus, data_manager:DataManager, row:int):
         self.app_bus = app_bus
         self.data_manager = data_manager
         
         f = Frame(main, bd=1, relief=SUNKEN)
         f.grid(row=row, column=0, columnspan=1, sticky=W+E+N+S)
 
-        self.l_connected = Label(f, bd=1)
+        self.l_connected = Label(f, borderwidth=1)
         self.l_connected.pack(side=tk.RIGHT, padx=(5, 5), pady=2)
         self.is_connected_handler({'connected':False})
 
         self.pb = ttk.Progressbar(f, orient=tk.HORIZONTAL, length=160, maximum=100)
         self.pb.pack(side=tk.RIGHT, padx=(5, 0), pady=2)
         self.pb.step(0)
```

### Comparing `eo_man-0.1.8/eo_man/view/tool_bar.py` & `eo_man-0.1.9/eo_man/view/tool_bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import threading
 import tkinter as tk
+from tkinter import ttk
 import os
 from tkinter import *
 from tkinter import messagebox
 from PIL import Image, ImageTk
 from idlelib.tooltip import Hovertip
 import webbrowser
 import subprocess
@@ -41,15 +42,15 @@
         if not AppInfo.is_version_up_to_date():
             new_v = AppInfo.get_lastest_available_version()
             b = self._create_img_button(f, f"New Software Version 'v{new_v}' is available.", ImageGallery.get_software_update_available_icon(), self.show_how_to_update)
             b.pack(side=RIGHT, padx=(0,2), pady=2)
 
 
     def _create_img_button(self, f:Frame, tooltip:str, image:ImageTk.PhotoImage, command) -> Button:
-        b = Button(f, image=image, relief=GROOVE, cursor="hand2", command=command)
+        b = ttk.Button(f, image=image, cursor="hand2", command=command) #, relief=GROOVE)
         Hovertip(b,tooltip,300)
         b.image = image
         b.pack(side=LEFT, padx=(2,0), pady=2)
         return b
     
     def show_how_to_update(self):
         base_path = os.environ.get('VIRTUAL_ENV', '')
```

### Comparing `eo_man-0.1.8/eo_man.egg-info/PKG-INFO` & `eo_man-0.1.9/eo_man.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo_man
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to managed EnOcean Devices and to generate Home Assistant Configuration.
 Home-page: https://github.com/grimmpp/enocean-device-manager
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
         
@@ -25,15 +25,17 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eltako14bus==0.0.45
+Requires-Dist: eltako14bus==0.0.46
+Requires-Dist: requests==2.31.0
+Requires-Dist: enocean==0.60.1
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio
 Requires-Dist: aiocoap
 Requires-Dist: pyyaml
 Requires-Dist: termcolor
 Requires-Dist: strenum
 Requires-Dist: pillow
@@ -51,15 +53,15 @@
 # WORK IN PROGRESS!!! NOT YET RELEASE READY!!!
 
 This client application allows you to **inventory all EnOcean devices**. It can **automatically read and detect devices** from the RS485 bus or from wireless network. After the devices are listed in the EnOcean Device Manager **you can enricht device information** like changing the name, comment or adapt parameters like timeframes, thresholds, units, ... .
 Furthermore, it automatically can detect default settings for Home Assistant configuration which can be adjust as well and it allows you to **generate and export the configuration for Home Assistant**. 
 (The exported Home Assistant configuration is intended for the [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako/))
 
 ## Preview
-<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot.png" /> 
+<img src="https://github.com/grimmpp/enocean-device-manager/blob/main/screenshot2.png" /> 
 What you can see here can automatically detected by reading the memory of the bus devices via FAM14. Telegrams of sensors and decentralized devices will be received and additionally added. 
 Additional info for Home Assistant is automatically added. The configuration for Home Assistant can be generated by the detected information.
 For further steps it is planned to extend the support for changing the data which was collected so that a proper management of the devices can be supported.
 
 ## System Requirements / Where to install and how to use it?
 This tool is a desktop application (not browser based) and it runs independent of Home Assistant. Install it directly on a Windows, Linux or Max. (So far only Windows has been tested but all three operating systems should be supported.) Your PC requires Python pre-installed and you should be able to connect it to your EnOcean devices, either via USB cable (Eltako FAM14, FGW14-USB, ...) or wireless transceiver (Eltako FAM-USB). Support for the wireless transceiver 'EnOcean USB300' is planned for future releases.
```

### Comparing `eo_man-0.1.8/eo_man.egg-info/SOURCES.txt` & `eo_man-0.1.9/eo_man.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,29 +20,40 @@
 eo_man/data/data_manager.py
 eo_man/data/device.py
 eo_man/data/filter.py
 eo_man/data/ha_config_generator.py
 eo_man/data/homeassistant/__init__.py
 eo_man/data/homeassistant/const.py
 eo_man/icons/Breathe-about.png
+eo_man/icons/Faenza-system-search.bmp
+eo_man/icons/Faenza-system-search.ico
 eo_man/icons/Faenza-system-search.png
 eo_man/icons/Gnome-help-faq.png
 eo_man/icons/Home_Assistant_Logo.png
 eo_man/icons/Oxygen480-actions-document-save-as.png
 eo_man/icons/Oxygen480-actions-document-save.png
 eo_man/icons/Oxygen480-actions-help.png
 eo_man/icons/Oxygen480-status-folder-open.png
 eo_man/icons/Software-update-available.png
 eo_man/icons/__init__.py
+eo_man/icons/blank.png
 eo_man/icons/export_icon.png
+eo_man/icons/fam-usb.png
+eo_man/icons/fam-usb2.png
+eo_man/icons/fam14.jpg
+eo_man/icons/fam14.png
+eo_man/icons/fgw14-usb.png
 eo_man/icons/github_icon.png
 eo_man/icons/image_gallary.py
 eo_man/icons/paypal_icon.png
 eo_man/icons/paypal_me_badge.png
-eo_man/icons/test.py
+eo_man/icons/usb300.png
+eo_man/icons/wireless-network-bw.png
+eo_man/icons/wireless-network-colored.png
+eo_man/icons/wireless.png
 eo_man/view/__init__.py
 eo_man/view/about_window.py
 eo_man/view/checklistcombobox.py
 eo_man/view/device_details.py
 eo_man/view/device_table.py
 eo_man/view/donation_button.py
 eo_man/view/filter_bar.py
```

### Comparing `eo_man-0.1.8/setup.py` & `eo_man-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 with open('README.md', encoding="utf-8") as f:
     long_description = f.read()
 
 # with open(os.path.join(base_dir, 'LICENSE'), encoding="utf-8") as f:
 with open('LICENSE', encoding="utf-8") as f:
     license = f.read()
 
-required = ['eltako14bus==0.0.45', 'pyserial', 'pyserial-asyncio', 'aiocoap', 
+required = ['eltako14bus==0.0.46', 'requests==2.31.0', 'enocean==0.60.1', 'pyserial', 'pyserial-asyncio', 'aiocoap', 
             # 'homeassistant', 
             'pyyaml', 
             'termcolor', 'strenum', 'pillow', 'numpy',
             # 'tzlocal', 
             'tkinterhtml']
 
+
+
 setup(
     name='eo_man',
-    version='0.1.8',
+    version='0.1.9',
     package_dir={'eo_man':"eo_man"},
     # packages=find_packages("./eo-man"),
     #package_data={'': ['*.png']},
     package_data={'': ['icons/*']},
     package=["eo_man"],
     include_package_data=True,
     install_requires=required,
```

### Comparing `eo_man-0.1.8/tests/test_app_config.py` & `eo_man-0.1.9/tests/test_app_config.py`

 * *Files identical despite different names*

