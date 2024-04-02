# Comparing `tmp/ftrack_qt-2.0.1.tar.gz` & `tmp/ftrack_qt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_qt-2.0.1.tar", max compression
+gzip compressed data, was "ftrack_qt-2.1.0.tar", max compression
```

## Comparing `ftrack_qt-2.0.1.tar` & `ftrack_qt-2.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    10176 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0       50 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/README.md
--rw-r--r--   0        0        0     1195 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      895 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/__init__.py
--rw-r--r--   0        0        0       57 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/__init__.py
--rw-r--r--   0        0        0       74 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/decorators/__init__.py
--rw-r--r--   0        0        0      369 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/decorators/threading.py
--rw-r--r--   0        0        0      988 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/layout/__init__.py
--rw-r--r--   0        0        0     1018 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/theme/__init__.py
--rw-r--r--   0        0        0     1186 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/threading/__init__.py
--rw-r--r--   0        0        0     3802 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/utils/widget/__init__.py
--rw-r--r--   0        0        0       57 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/__init__.py
--rw-r--r--   0        0        0       77 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/accordion/__init__.py
--rw-r--r--   0        0        0     8688 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/accordion/accordion_widget.py
--rw-r--r--   0        0        0      132 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/browsers/__init__.py
--rw-r--r--   0        0        0    30910 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/browsers/entity_browser.py
--rw-r--r--   0        0        0     1887 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/browsers/file_browser.py
--rw-r--r--   0        0        0      257 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/__init__.py
--rw-r--r--   0        0        0     1519 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/circular_button.py
--rw-r--r--   0        0        0     4058 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/options_button.py
--rw-r--r--   0        0        0     7456 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/progress_button.py
--rw-r--r--   0        0        0      168 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/delegate/__init__.py
--rw-r--r--   0        0        0     1612 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
--rw-r--r--   0        0        0      346 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0      927 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/file_dialog.py
--rw-r--r--   0        0        0     4942 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/modal_dialog.py
--rw-r--r--   0        0        0     6357 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
--rw-r--r--   0        0        0     3145 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/styled_dialog.py
--rw-r--r--   0        0        0     3411 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/tab_dialog.py
--rw-r--r--   0        0        0      249 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/__init__.py
--rw-r--r--   0        0        0     2470 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/asset_version_creation.py
--rw-r--r--   0        0        0     3987 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/asset_version_selection.py
--rw-r--r--   0        0        0     2871 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/new_asset_input.py
--rw-r--r--   0        0        0      160 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/headers/__init__.py
--rw-r--r--   0        0        0     5412 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/headers/accordion_header_widget.py
--rw-r--r--   0        0        0     2963 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/headers/session_header.py
--rw-r--r--   0        0        0      207 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/__init__.py
--rw-r--r--   0        0        0      647 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/arrow_icon.py
--rw-r--r--   0        0        0     2244 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/material_icon.py
--rw-r--r--   0        0        0     2807 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/status_icon.py
--rw-r--r--   0        0        0       58 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/info/__init__.py
--rw-r--r--   0        0        0     2598 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/info/entity_info.py
--rw-r--r--   0        0        0       59 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/lines/__init__.py
--rw-r--r--   0        0        0     1124 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/lines/line_widget.py
--rw-r--r--   0        0        0       57 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/lists/__init__.py
--rw-r--r--   0        0        0     3764 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/lists/asset_list.py
--rw-r--r--   0        0        0       59 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/logos/__init__.py
--rw-r--r--   0        0        0     1059 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/logos/ftrack_logo.py
--rw-r--r--   0        0        0      118 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/models/__init__.py
--rw-r--r--   0        0        0     3461 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/models/table_model.py
--rw-r--r--   0        0        0      257 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/__init__.py
--rw-r--r--   0        0        0     3085 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/busy_indicator.py
--rw-r--r--   0        0        0     6504 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/overlay_widget.py
--rw-r--r--   0        0        0      964 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/shaded_widget.py
--rw-r--r--   0        0        0      128 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/progress/__init__.py
--rw-r--r--   0        0        0     9602 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/progress/progress_widget.py
--rw-r--r--   0        0        0       70 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/search/__init__.py
--rw-r--r--   0        0        0     3540 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/search/collapsable_search_box.py
--rw-r--r--   0        0        0      392 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/__init__.py
--rw-r--r--   0        0        0     7861 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/asset_selector.py
--rw-r--r--   0        0        0     7908 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/context_selector.py
--rw-r--r--   0        0        0     3450 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/list_selector.py
--rw-r--r--   0        0        0     1507 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/status_selector.py
--rw-r--r--   0        0        0     1450 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/version_selector.py
--rw-r--r--   0        0        0      408 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/__init__.py
--rw-r--r--   0        0        0      806 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/asset_version.py
--rw-r--r--   0        0        0     5530 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/base.py
--rw-r--r--   0        0        0     1827 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/context.py
--rw-r--r--   0        0        0      859 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/ellipse.py
--rw-r--r--   0        0        0     5599 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/session_base.py
--rw-r--r--   0        0        0     1139 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/user.py
--rw-r--r--   0        0        0      116 2024-03-08 11:14:07.091586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/user/__init__.py
--rw-r--r--   0        0        0     2422 2024-03-08 11:14:07.095586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/user/ftrack_user.py
--rw-r--r--   0        0        0      115 2024-03-08 11:14:07.095586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/views/__init__.py
--rw-r--r--   0        0        0     1567 2024-03-08 11:14:07.095586 ftrack_qt-2.0.1/source/ftrack_qt/widgets/views/table_view.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 ftrack_qt-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      168 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/README.md
+-rw-r--r--   0        0        0     1249 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/decorators/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/decorators/threading.py
+-rw-r--r--   0        0        0      988 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/layout/__init__.py
+-rw-r--r--   0        0        0     1018 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/theme/__init__.py
+-rw-r--r--   0        0        0     1186 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/threading/__init__.py
+-rw-r--r--   0        0        0     3802 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/widget/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/__init__.py
+-rw-r--r--   0        0        0     8688 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/accordion_widget.py
+-rw-r--r--   0        0        0      267 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/__init__.py
+-rw-r--r--   0        0        0     3616 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py
+-rw-r--r--   0        0        0     3987 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py
+-rw-r--r--   0        0        0     4105 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py
+-rw-r--r--   0        0        0      132 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/__init__.py
+-rw-r--r--   0        0        0    30910 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/entity_browser.py
+-rw-r--r--   0        0        0     1887 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/file_browser.py
+-rw-r--r--   0        0        0      257 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/__init__.py
+-rw-r--r--   0        0        0     1519 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/circular_button.py
+-rw-r--r--   0        0        0     4058 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/options_button.py
+-rw-r--r--   0        0        0     7456 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/progress_button.py
+-rw-r--r--   0        0        0      168 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/__init__.py
+-rw-r--r--   0        0        0     1612 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
+-rw-r--r--   0        0        0      346 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0      927 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/file_dialog.py
+-rw-r--r--   0        0        0     4942 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py
+-rw-r--r--   0        0        0     6357 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
+-rw-r--r--   0        0        0     3103 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py
+-rw-r--r--   0        0        0     3411 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py
+-rw-r--r--   0        0        0      167 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/__init__.py
+-rw-r--r--   0        0        0     5412 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py
+-rw-r--r--   0        0        0     2963 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/session_header_widget.py
+-rw-r--r--   0        0        0      207 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/__init__.py
+-rw-r--r--   0        0        0      647 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/arrow_icon.py
+-rw-r--r--   0        0        0     2244 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/material_icon.py
+-rw-r--r--   0        0        0     2807 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/status_icon.py
+-rw-r--r--   0        0        0       58 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/entity_info.py
+-rw-r--r--   0        0        0       59 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/__init__.py
+-rw-r--r--   0        0        0     1124 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/line_widget.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/__init__.py
+-rw-r--r--   0        0        0     5294 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/asset_list.py
+-rw-r--r--   0        0        0       59 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/__init__.py
+-rw-r--r--   0        0        0     1059 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/ftrack_logo.py
+-rw-r--r--   0        0        0      118 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/table_model.py
+-rw-r--r--   0        0        0      264 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/__init__.py
+-rw-r--r--   0        0        0     3085 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py
+-rw-r--r--   0        0        0     6504 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/overlay_widget.py
+-rw-r--r--   0        0        0      964 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/shaded_widget.py
+-rw-r--r--   0        0        0      128 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/__init__.py
+-rw-r--r--   0        0        0     9602 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/progress_widget.py
+-rw-r--r--   0        0        0       70 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3540 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/collapsable_search_box.py
+-rw-r--r--   0        0        0      392 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/__init__.py
+-rw-r--r--   0        0        0     8610 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/asset_selector.py
+-rw-r--r--   0        0        0     7908 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/context_selector.py
+-rw-r--r--   0        0        0     3450 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/list_selector.py
+-rw-r--r--   0        0        0     1507 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/status_selector.py
+-rw-r--r--   0        0        0     1450 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/version_selector.py
+-rw-r--r--   0        0        0      486 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/__init__.py
+-rw-r--r--   0        0        0      816 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py
+-rw-r--r--   0        0        0     5530 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py
+-rw-r--r--   0        0        0     1846 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py
+-rw-r--r--   0        0        0      878 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py
+-rw-r--r--   0        0        0     5599 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py
+-rw-r--r--   0        0        0     1149 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py
+-rw-r--r--   0        0        0      116 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/ftrack_user.py
+-rw-r--r--   0        0        0      115 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/__init__.py
+-rw-r--r--   0        0        0     1567 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/table_view.py
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 ftrack_qt-2.1.0/PKG-INFO
```

### Comparing `ftrack_qt-2.0.1/LICENSE.txt` & `ftrack_qt-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/pyproject.toml` & `ftrack_qt-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-qt"
-version = "2.0.1"
+version = "2.1.0"
 description='ftrack qt library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_qt", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/qt"
@@ -20,14 +20,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 3.12"
+# TODO: PySide will be implemented in future versions
 PySide2 = { version = "^5.13.2", optional = true } #python = "<3.10", optional = true }
 #PySide6 = { version = "^6.5",  python = ">=3.10", optional = true }
 "Qt.py" = ">=1.0.0, < 2"
 #ftrack
 ftrack-constants= {  version = "^2.0.0", optional = true }
 ftrack-utils = {  version = "^2.0.0", optional = true }
 ftrack-qt-style = {  version = "^2.0.0", optional = true }
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/__init__.py` & `ftrack_qt-2.1.0/source/ftrack_qt/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/utils/layout/__init__.py` & `ftrack_qt-2.1.0/source/ftrack_qt/utils/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/utils/theme/__init__.py` & `ftrack_qt-2.1.0/source/ftrack_qt/utils/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/utils/threading/__init__.py` & `ftrack_qt-2.1.0/source/ftrack_qt/utils/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/utils/widget/__init__.py` & `ftrack_qt-2.1.0/source/ftrack_qt/utils/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/accordion/accordion_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/accordion_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/browsers/entity_browser.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/entity_browser.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/browsers/file_browser.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/file_browser.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/circular_button.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/circular_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/options_button.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/options_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/buttons/progress_button.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/progress_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/file_dialog.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/file_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/modal_dialog.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/styled_dialog.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     '''
 
     DEFAULT_STYLE = qt_constants.theme.DEFAULT_STYLE
 
     # Allow child classes to override the default theme and background style
     theme = qt_constants.theme.DEFAULT_THEME
     background_style = qt_constants.theme.DEFAULT_BACKGROUND_STYLE
-    docked = False
 
     @property
     def darken(self):
         return self._darken
 
     @darken.setter
     def darken(self, value):
@@ -47,16 +46,15 @@
         super(StyledDialog, self).__init__(parent=parent)
         self._darken = False
         self._shaded_widget = None
 
         if background_style:
             self.background_style = background_style
 
-        if docked:
-            self.docked = docked
+        self.docked = docked
 
         # Apply theme and with DCC specific properties
         # TODO: This has been deactivated as it makes the filebrowser dialog
         #  crash after selecting a file. If this needs to be activated in the
         #  future for DCC reasons: 1- Double check file browser dialog still
         #  working after selecting a file in standalone ui mode. 2- if not
         #  working, find another way to simulate the tool property in PySide2.
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/dialogs/tab_dialog.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/asset_version_creation.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,22 +17,49 @@
         return self._versions[-1]
 
     @property
     def asset_id(self):
         '''Return the id of the asset.'''
         return self._asset_id
 
+    @property
+    def active(self):
+        '''Return the active state of the widget.'''
+        return self._active
+
+    @active.setter
+    def active(self, value):
+        '''Change active state of the widget - greys out the widget if False.'''
+        if value == self._active:
+            return
+        self._active = value
+        self._asset_name_widget.style().unpolish(self._asset_name_widget)
+        self._create_label.style().unpolish(self._create_label)
+        self._version_label.style().unpolish(self._version_label)
+        if value:
+            self._asset_name_widget.setObjectName('')
+            self._create_label.setObjectName('gray')
+            self._version_label.setObjectName('color-primary')
+        else:
+            self._asset_name_widget.setObjectName('gray-dark')
+            self._create_label.setObjectName('gray-darker')
+            self._version_label.setObjectName('gray-darker')
+        self._asset_name_widget.style().polish(self._asset_name_widget)
+        self._create_label.style().polish(self._create_label)
+        self._version_label.style().polish(self._version_label)
+
     def __init__(self, asset_name, asset_id, versions, server_url):
         '''Initialize the AssetVersionCreation widget.'''
         super(AssetVersionCreation, self).__init__()
 
         self._asset_id = asset_id
         self._asset_name = asset_name
         self._versions = versions
         self._server_url = server_url
+        self._active = True
 
         self._thumbnail_widget = None
         self._asset_name_widget = None
         self._create_label = None
         self._version_label = None
 
         self.pre_build()
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/frames/asset_version_selection.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/headers/accordion_header_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/headers/session_header.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/session_header_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/arrow_icon.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/arrow_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/material_icon.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/material_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/icons/status_icon.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/status_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/info/entity_info.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/entity_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/lines/line_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/line_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/lists/asset_list.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/asset_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from Qt import QtWidgets, QtCore, QtGui
 
 
 class AssetList(QtWidgets.QListWidget):
     '''Widget presenting list of existing assets'''
 
+    active_changed = QtCore.Signal(object)
+    '''Signal emitted when the list is activated or deactivated, with active as argument.'''
+
     version_changed = QtCore.Signal(object)
     '''Signal emitted when version is changed, with assetversion entity as 
     argument (version select mode)'''
 
     assets_added = QtCore.Signal(object)
     '''Signal emitted when assets are added to the list'''
 
@@ -20,35 +23,68 @@
     '''Signal emitted when selected item is changed with arguments containing 
     the index of the current version, the version dictionary and the asset_id'''
 
     @property
     def latest_published_asset_item(self):
         return self._latest_published_asset_item
 
-    def __init__(self, asset_list_widget_item, parent=None):
+    @property
+    def active(self):
+        '''Return if list is active - focus or not'''
+        return self._active
+
+    @active.setter
+    def active(self, value):
+        '''Set active state of the list'''
+        if value == self._active:
+            return
+        self._active = value
+        # Activate or deactivate the list items
+        for idx in range(self.count()):
+            item = self.item(idx)
+            widget = self.itemWidget(item)
+            if hasattr(widget, 'active'):
+                widget.active = value
+        if value:
+            # Must have something selected
+            if self.currentRow() == -1:
+                self.setCurrentItem(self.item(0))
+        else:
+            self.blockSignals(True)
+            self.setCurrentRow(-1)  # Make sure list is deselected
+            self.blockSignals(False)
+        self.active_changed.emit(value)
+
+    def __init__(self, asset_list_widget_item_class, parent=None):
         '''Initialize AssetList'''
         super(AssetList, self).__init__(parent=parent)
         self.logger = logging.getLogger(
             __name__ + '.' + self.__class__.__name__
         )
-        self.asset_list_widget_item = asset_list_widget_item
+        self.asset_list_widget_item_class = asset_list_widget_item_class
         self._latest_published_asset_item = None
+        self._active = True
 
         self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.verticalScrollBar().setDisabled(True)
+        self.setAutoScroll(False)
         self.setSpacing(1)
         self.assets = []
-        self.currentItemChanged.connect(self._on_item_changed)
+        self.currentItemChanged.connect(self.on_item_changed_callback)
 
     def set_assets(self, assets):
         '''Set assets for the list'''
+        self.currentItemChanged.disconnect()
+        self._latest_published_asset_item = None
+        self.clear()
         self.assets = assets
 
         for asset_id, asset_dict in self.assets.items():
-            widget = self.asset_list_widget_item(
+            widget = self.asset_list_widget_item_class(
                 asset_name=asset_dict['name'],
                 asset_id=asset_id,
                 versions=asset_dict['versions'],
                 server_url=asset_dict['server_url'],
             )
 
             if hasattr(widget, 'version_changed'):
@@ -73,25 +109,31 @@
                     widget.version['date']
                     > self.itemWidget(
                         self._latest_published_asset_item
                     ).version['date']
                 ):
                     self._latest_published_asset_item = list_item
         self.assets_added.emit(assets)
+        self.currentItemChanged.connect(self.on_item_changed_callback)
         # Pre select the latest published asset version.
         self.setCurrentItem(self._latest_published_asset_item)
 
     def _on_version_changed_callback(self, version):
         '''Handle version changed callback'''
         self.version_changed.emit(version)
 
-    def _on_item_changed(self, current_item, previous_item):
+    def on_item_changed_callback(self, current_item, previous_item):
         '''Handle item changed event'''
         if hasattr(self.itemWidget(current_item), 'enable_version_select'):
             if previous_item:
                 self.itemWidget(previous_item).enable_version_select = False
             self.itemWidget(current_item).enable_version_select = True
         self.selected_item_changed.emit(
             self.indexFromItem(current_item),
             self.itemWidget(current_item).version,
             self.itemWidget(current_item).asset_id,
         )
+
+    def mousePressEvent(self, event):
+        '''Override mouse press to emit signal.'''
+        super(AssetList, self).mousePressEvent(event)
+        self.active = True
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/logos/ftrack_logo.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/ftrack_logo.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/models/table_model.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/table_model.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/busy_indicator.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/overlay_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/overlay_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/overlay/shaded_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/shaded_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/progress/progress_widget.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/progress_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/search/collapsable_search_box.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/collapsable_search_box.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/asset_selector.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/asset_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 import logging
 
 from Qt import QtWidgets, QtCore, QtGui
 
-from ftrack_qt.widgets.frames import (
+from ftrack_qt.widgets.asset import (
     AssetVersionCreation,
     AssetVersionSelection,
     NewAssetInput,
 )
 from ftrack_qt.widgets.lists import AssetList
 
 
-class OpenAssetSelector(QtWidgets.QWidget):
-    '''This widget allows the user to select an existing asset and asset version,
-    or input an asset name for creating a new asset, depending on the mode.'''
+class AssetSelectorBase(QtWidgets.QWidget):
+    '''This widget allows the user to select an existing asset and asset version.'''
 
     assets_added = QtCore.Signal(object)
     '''This signal is emitted when assets are added. It sends a list of assets 
     dictionaries as an argument'''
 
     version_changed = QtCore.Signal(object)
     '''This signal is emitted when the version is changed. It sends the version 
@@ -32,22 +31,20 @@
     def __init__(
         self,
         parent=None,
     ):
         '''
         This method initialises the asset selector widget.
         '''
-        super(OpenAssetSelector, self).__init__(parent=parent)
+        super(AssetSelectorBase, self).__init__(parent=parent)
         self.logger = logging.getLogger(
             __name__ + '.' + self.__class__.__name__
         )
 
-        self._list_and_input = None
         self._asset_list = None
-        self._new_asset_input = None
 
         self.selected_index = None
 
         self.pre_build()
         self.build()
         self.post_build()
 
@@ -65,58 +62,64 @@
         self.layout().addWidget(self._asset_list)
 
     def post_build(self):
         '''This method connects signals to slots after building the widget.'''
         self._asset_list.assets_added.connect(self._on_assets_added)
         self._asset_list.version_changed.connect(self._on_version_changed)
         self._asset_list.selected_item_changed.connect(
-            self._on_selected_item_changed
+            self._on_selected_item_changed_callback
         )
 
     def _on_assets_added(self, assets):
         '''This method emits the assets_added signal with the given assets.'''
         self.assets_added.emit(assets)
 
     def set_assets(self, assets):
         '''This method sets the assets in the asset list and shows or hides it
         based on the presence of assets.'''
-        if not assets:
-            self._asset_list.hide()
-        else:
-            self._asset_list.show()
         self._asset_list.set_assets(assets)
 
     def _on_version_changed(self, version):
         '''This method emits the version_changed signal with the given version.'''
         self.version_changed.emit(version)
 
-    def _on_selected_item_changed(self, index, version, asset_id):
+    def _on_selected_item_changed_callback(self, index, version, asset_id):
         '''This method updates the selected index and emits the
         selected_item_changed signal with the given version.'''
         self.selected_index = index
         self.selected_item_changed.emit(version, asset_id)
 
 
-class PublishAssetSelector(OpenAssetSelector):
-    '''This widget allows the user to select an existing asset and asset version,
-    or input an asset name for creating a new asset.'''
+class OpenAssetSelector(AssetSelectorBase):
+    '''Asset selector tailored for open.'''
+
+    def __init__(self):
+        '''This method initialises the open asset selector widget.'''
+        super(OpenAssetSelector, self).__init__()
+
+
+class PublishAssetSelector(AssetSelectorBase):
+    '''Asset selector tailored for publish, allows user to select and existing
+    asset or input an asset name for creating a new asset.'''
 
     VALID_ASSET_NAME = QtCore.QRegExp('[A-Za-z0-9_]+')
 
     new_asset = QtCore.Signal(object)
     '''This signal is emitted when a new asset is selected. It sends the
     new asset_name as argument.'''
 
     def __init__(
         self,
         parent=None,
     ):
         '''
-        This method initialises the asset selector widget.
+        This method initialises the publish asset selector widget.
         '''
+        self._list_and_input = None
+        self._new_asset_input = None
         self.validator = QtGui.QRegExpValidator(self.VALID_ASSET_NAME)
         self.placeholder_name = "Asset Name..."
 
         super(PublishAssetSelector, self).__init__(parent=parent)
 
     def build(self):
         '''This method builds the asset list and new asset input and adds them
@@ -134,23 +137,38 @@
         self._list_and_input.add_asset_input(self._new_asset_input)
 
         self.layout().addWidget(self._list_and_input)
 
     def post_build(self):
         '''This method connects signals to slots after building the widget.'''
         super(PublishAssetSelector, self).post_build()
-        self._new_asset_input.text_changed.connect(self._on_new_asset)
+        self._asset_list.active_changed.connect(
+            self._on_asset_list_active_changed_callback
+        )
+        self._new_asset_input.active_changed.connect(
+            self._on_new_asset_active_changed_callback
+        )
+        self._new_asset_input.text_changed.connect(
+            self._on_new_asset_name_changed_callback
+        )
+
+    def _on_asset_list_active_changed_callback(self, active):
+        if active:
+            # Deactivate new input
+            self._new_asset_input.active = False
 
-    def _on_new_asset(self, asset_name):
+    def _on_new_asset_active_changed_callback(self, active):
         '''This method handles changes to the new asset name input.'''
-        self._asset_list.blockSignals(True)
-        self._asset_list.setCurrentRow(-1)  # Make sure list is deselected
-        self._asset_list.blockSignals(False)
-        self.selected_index = None
-        self.selected_item_changed.emit(None, None)
+        if active:
+            # Deactivate list
+            self._asset_list.active = False
+            self.selected_index = None
+            self.selected_item_changed.emit(None, None)
+
+    def _on_new_asset_name_changed_callback(self, asset_name):
         is_valid_name = self.validate_name(asset_name)
         if is_valid_name:
             self.new_asset.emit(asset_name)
         else:
             self.new_asset.emit(None)
 
     def validate_name(self, asset_name):
@@ -173,14 +191,20 @@
 
     def set_default_new_asset_name(self, name):
         '''This method sets the default name for the new asset input.'''
         self._new_asset_input.set_default_name(name)
 
     def set_assets(self, assets):
         super(PublishAssetSelector, self).set_assets(assets)
+        if not assets:
+            self._asset_list.hide()
+            self._new_asset_input.active = True
+        else:
+            self._asset_list.show()
+            self._new_asset_input.active = False
         # Make sure widget expands properly to fit list
         self._list_and_input.size_changed()
 
 
 class AssetListAndInput(QtWidgets.QWidget):
     '''This is a compound widget containing an asset list and a new asset input'''
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/context_selector.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/context_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/list_selector.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/list_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/status_selector.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/status_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/selectors/version_selector.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/version_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/asset_version.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 from Qt import QtCore, QtGui, QtWidgets
 
-from ftrack_qt.widgets.thumbnails.base import ThumbnailBase
+from ftrack_qt.widgets.thumbnails.base_thumbnail import ThumbnailBase
 
 
 class AssetVersionThumbnail(ThumbnailBase):
     '''Asset version thumbnail widget'''
 
     def _download(self, url):
         '''Return thumbnail from *reference*.'''
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/base.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/context.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
 
 import urllib.request, urllib.parse, urllib.error
 
 from Qt import QtCore, QtGui, QtWidgets
 
-from ftrack_qt.widgets.thumbnails.session_base import SessionThumbnailBase
+from ftrack_qt.widgets.thumbnails.session_base_thumbnail import (
+    SessionThumbnailBase,
+)
 
 
 class ContextThumbnail(SessionThumbnailBase):
     '''Context thumbnail widget'''
 
     def _download(self, reference):
         '''Return thumbnail from *reference*.'''
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/ellipse.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
 
 from Qt import QtCore, QtGui, QtWidgets
 
-from ftrack_qt.widgets.thumbnails.session_base import SessionThumbnailBase
+from ftrack_qt.widgets.thumbnails.session_base_thumbnail import (
+    SessionThumbnailBase,
+)
 
 
 class EllipseThumbnailBase(SessionThumbnailBase):
     '''Thumbnail which is drawn as an ellipse.'''
 
     def paintEvent(self, event):
         '''Override paint event to make round thumbnails.'''
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/session_base.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/thumbnails/user.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
 
 import urllib.request, urllib.parse, urllib.error
 
-from ftrack_qt.widgets.thumbnails.ellipse import EllipseThumbnailBase
+from ftrack_qt.widgets.thumbnails.ellipse_thumbnail import EllipseThumbnailBase
 
 
 class UserThumbnail(EllipseThumbnailBase):
     '''User(avatar) thumbnail widget'''
 
     def _download(self, reference):
         '''Return thumbnail from *reference*.'''
```

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/user/ftrack_user.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/ftrack_user.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/source/ftrack_qt/widgets/views/table_view.py` & `ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/table_view.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.0.1/PKG-INFO` & `ftrack_qt-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-qt
-Version: 2.0.1
+Version: 2.1.0
 Summary: ftrack qt library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,9 +22,10 @@
 Requires-Dist: ftrack-qt-style (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-utils (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/qt
 Description-Content-Type: text/markdown
 
 # Qt
 
-This is the ftrack integrations Qt library.
+This is the ftrack integrations Qt library. 
+All custom widgets and dialogs used around the framework and other ftrack integrations plugins should be found here.
```

