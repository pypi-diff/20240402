# Comparing `tmp/reflex-0.4.6a3.tar.gz` & `tmp/reflex-0.4.6a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.4.6a3.tar", max compression
+gzip compressed data, was "reflex-0.4.6a4.tar", max compression
```

## Comparing `reflex-0.4.6a3.tar` & `reflex-0.4.6a4.tar`

### file list

```diff
@@ -1,522 +1,522 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.6a3/LICENSE
--rw-r--r--   0        0        0     9171 2024-03-29 16:58:00.709441 reflex-0.4.6a3/README.md
--rw-r--r--   0        0        0     2957 2024-04-01 19:07:40.608726 reflex-0.4.6a3/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.6a3/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.6a3/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      838 2024-03-20 23:54:55.828973 reflex-0.4.6a3/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.6a3/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.6a3/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.6a3/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.6a3/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.6a3/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.6a3/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.6a3/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.6a3/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.6a3/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.6a3/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.6a3/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.6a3/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.6a3/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0     2392 2024-03-20 23:54:55.830719 reflex-0.4.6a3/reflex/.templates/apps/sidebar/README.md
--rw-r--r--   0        0        0     4286 2023-11-22 05:49:24.665793 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-22 05:49:24.665902 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/github.svg
--rw-r--r--   0        0        0     5403 2023-11-22 05:49:24.666131 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-22 05:49:24.666228 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/paneleft.svg
--rw-r--r--   0        0        0     1899 2024-03-20 23:54:55.831004 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/reflex_black.svg
--rw-r--r--   0        0        0      908 2024-03-20 23:54:55.831285 reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/reflex_white.svg
--rw-r--r--   0        0        0       32 2023-11-22 05:49:24.666441 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 05:49:24.666586 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/components/__init__.py
--rw-r--r--   0        0        0     3906 2024-03-20 23:54:55.831486 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/components/sidebar.py
--rw-r--r--   0        0        0       89 2023-11-22 05:49:24.666931 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/pages/__init__.py
--rw-r--r--   0        0        0      490 2024-03-20 23:54:55.831633 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/pages/dashboard.py
--rw-r--r--   0        0        0      436 2023-11-22 05:49:24.667170 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/pages/index.py
--rw-r--r--   0        0        0     1571 2024-03-20 23:54:55.831956 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/pages/settings.py
--rw-r--r--   0        0        0      270 2024-02-06 00:51:31.970017 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/sidebar.py
--rw-r--r--   0        0        0     1570 2024-03-20 23:54:55.832516 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/styles.py
--rw-r--r--   0        0        0       43 2024-03-20 23:54:55.832690 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/templates/__init__.py
--rw-r--r--   0        0        0     3904 2024-03-20 23:54:55.832868 reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/templates/template.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.6a3/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.6a3/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.6a3/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.6a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      615 2024-03-29 13:41:30.688966 reflex-0.4.6a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2262 2024-03-20 23:54:55.833729 reflex-0.4.6a3/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.6a3/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      412 2024-03-28 16:38:22.949259 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      461 2024-03-28 16:38:22.949386 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.6a3/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.6a3/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.6a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.6a3/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.6a3/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.6a3/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.6a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.6a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.6a3/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.6a3/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.6a3/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.6a3/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.6a3/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.6a3/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.6a3/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0    21563 2024-03-29 16:58:00.711812 reflex-0.4.6a3/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5676 2024-03-29 16:58:00.711989 reflex-0.4.6a3/reflex/__init__.py
--rw-r--r--   0        0        0     7565 2024-03-29 16:58:00.712124 reflex-0.4.6a3/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.6a3/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.6a3/reflex/admin.py
--rw-r--r--   0        0        0    44631 2024-03-29 16:58:00.712540 reflex-0.4.6a3/reflex/app.py
--rw-r--r--   0        0        0     4928 2024-03-20 23:54:55.837030 reflex-0.4.6a3/reflex/app.pyi
--rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.6a3/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4250 2024-03-29 16:58:00.713739 reflex-0.4.6a3/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.6a3/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17012 2024-03-28 16:38:22.949522 reflex-0.4.6a3/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.6a3/reflex/compiler/templates.py
--rw-r--r--   0        0        0    13997 2024-03-29 16:58:00.713923 reflex-0.4.6a3/reflex/compiler/utils.py
--rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.6a3/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.6a3/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.6a3/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-03-29 16:58:00.714454 reflex-0.4.6a3/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-03-29 16:58:00.714593 reflex-0.4.6a3/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.6a3/reflex/components/base/body.py
--rw-r--r--   0        0        0     3277 2024-03-29 16:58:00.714744 reflex-0.4.6a3/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.6a3/reflex/components/base/document.py
--rw-r--r--   0        0        0    14587 2024-03-29 16:58:00.714887 reflex-0.4.6a3/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.6a3/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3289 2024-03-29 16:58:00.715025 reflex-0.4.6a3/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.6a3/reflex/components/base/head.py
--rw-r--r--   0        0        0     6073 2024-03-29 16:58:00.715201 reflex-0.4.6a3/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.6a3/reflex/components/base/link.py
--rw-r--r--   0        0        0     7132 2024-03-29 16:58:00.715592 reflex-0.4.6a3/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.6a3/reflex/components/base/meta.py
--rw-r--r--   0        0        0    13088 2024-03-29 16:58:00.715862 reflex-0.4.6a3/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.6a3/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-03-29 16:58:00.716023 reflex-0.4.6a3/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.6a3/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.6a3/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    11059 2024-03-29 16:58:00.716548 reflex-0.4.6a3/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.6a3/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.6a3/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3725 2024-03-29 16:58:00.716690 reflex-0.4.6a3/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.6a3/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3300 2024-03-29 16:58:00.716857 reflex-0.4.6a3/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.6a3/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     4005 2024-03-29 16:58:00.717106 reflex-0.4.6a3/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.6a3/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3322 2024-03-29 16:58:00.717227 reflex-0.4.6a3/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.6a3/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    13065 2024-03-29 16:58:00.717356 reflex-0.4.6a3/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.6a3/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17816 2024-03-29 16:58:00.717520 reflex-0.4.6a3/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.6a3/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27536 2024-03-29 16:58:00.717709 reflex-0.4.6a3/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.6a3/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    16018 2024-03-29 16:58:00.717856 reflex-0.4.6a3/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.6a3/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.6a3/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    16087 2024-03-29 16:58:00.718197 reflex-0.4.6a3/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.6a3/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18809 2024-03-29 16:58:00.718354 reflex-0.4.6a3/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.6a3/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20429 2024-03-29 16:58:00.718551 reflex-0.4.6a3/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.6a3/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3329 2024-03-29 16:58:00.718696 reflex-0.4.6a3/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.6a3/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.6a3/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12594 2024-03-29 16:58:00.718821 reflex-0.4.6a3/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.6a3/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7708 2024-03-29 16:58:00.718976 reflex-0.4.6a3/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.6a3/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4349 2024-03-29 16:58:00.719131 reflex-0.4.6a3/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.6a3/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10903 2024-03-29 16:58:00.719257 reflex-0.4.6a3/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.6a3/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4178 2024-03-29 16:58:00.719399 reflex-0.4.6a3/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.6a3/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.6a3/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10687 2024-03-29 16:58:00.719754 reflex-0.4.6a3/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.6a3/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10443 2024-03-29 16:58:00.720133 reflex-0.4.6a3/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.6a3/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18530 2024-03-29 16:58:00.720262 reflex-0.4.6a3/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.6a3/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-03-29 16:58:00.720401 reflex-0.4.6a3/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.6a3/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-03-29 16:58:00.720529 reflex-0.4.6a3/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.6a3/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13623 2024-03-29 16:58:00.720743 reflex-0.4.6a3/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.6a3/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-03-29 16:58:00.720895 reflex-0.4.6a3/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.6a3/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20832 2024-03-29 16:58:00.721043 reflex-0.4.6a3/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.6a3/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4739 2024-03-29 16:58:00.721237 reflex-0.4.6a3/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.6a3/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21869 2024-03-29 16:58:00.721368 reflex-0.4.6a3/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.6a3/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.6a3/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18377 2024-03-29 16:58:00.721513 reflex-0.4.6a3/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.6a3/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-03-29 16:58:00.721666 reflex-0.4.6a3/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6501 2024-02-07 21:48:43.279255 reflex-0.4.6a3/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9432 2024-03-29 16:58:00.721794 reflex-0.4.6a3/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3176 2024-02-07 21:48:43.279649 reflex-0.4.6a3/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8414 2024-03-29 16:58:00.721926 reflex-0.4.6a3/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4547 2024-02-07 21:48:43.279975 reflex-0.4.6a3/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    14156 2024-03-29 16:58:00.722060 reflex-0.4.6a3/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.6a3/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-03-29 16:58:00.722172 reflex-0.4.6a3/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.6a3/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17745 2024-03-29 16:58:00.722496 reflex-0.4.6a3/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.6a3/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6602 2024-03-29 16:58:00.722723 reflex-0.4.6a3/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.6a3/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-03-29 16:58:00.722906 reflex-0.4.6a3/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.6a3/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-03-29 16:58:00.723061 reflex-0.4.6a3/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.6a3/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.6a3/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3450 2024-03-29 16:58:00.723207 reflex-0.4.6a3/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.6a3/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3733 2024-03-29 16:58:00.723333 reflex-0.4.6a3/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.6a3/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    14063 2024-03-29 16:58:00.723473 reflex-0.4.6a3/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.6a3/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8905 2024-03-29 16:58:00.723622 reflex-0.4.6a3/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.6a3/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3502 2024-03-29 16:58:00.723745 reflex-0.4.6a3/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.6a3/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4209 2024-03-29 16:58:00.723875 reflex-0.4.6a3/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.6a3/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    14066 2024-03-29 16:58:00.724005 reflex-0.4.6a3/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.6a3/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3301 2024-03-29 16:58:00.724121 reflex-0.4.6a3/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.6a3/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12432 2024-03-29 16:58:00.724241 reflex-0.4.6a3/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.6a3/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     7014 2024-03-29 16:58:00.724378 reflex-0.4.6a3/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.6a3/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.6a3/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10658 2024-03-29 16:58:00.724498 reflex-0.4.6a3/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.6a3/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6342 2024-03-29 16:58:00.724631 reflex-0.4.6a3/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.6a3/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-03-29 16:58:00.724932 reflex-0.4.6a3/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.6a3/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.6a3/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13646 2024-03-29 16:58:00.725095 reflex-0.4.6a3/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.6a3/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-03-29 16:58:00.725268 reflex-0.4.6a3/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.6a3/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6375 2024-03-29 16:58:00.725401 reflex-0.4.6a3/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.6a3/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    28490 2024-03-29 16:58:00.725535 reflex-0.4.6a3/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.6a3/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.6a3/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    24411 2024-03-29 16:58:00.725691 reflex-0.4.6a3/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.6a3/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25832 2024-03-29 16:58:00.725823 reflex-0.4.6a3/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.6a3/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    29108 2024-03-29 16:58:00.725942 reflex-0.4.6a3/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.6a3/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23975 2024-03-29 16:58:00.726063 reflex-0.4.6a3/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.6a3/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    30461 2024-03-29 16:58:00.726195 reflex-0.4.6a3/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.6a3/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6131 2024-03-29 16:58:00.726350 reflex-0.4.6a3/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.6a3/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.6a3/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3777 2024-03-29 16:58:00.726564 reflex-0.4.6a3/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.6a3/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3716 2024-03-29 16:58:00.726676 reflex-0.4.6a3/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.6a3/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3443 2024-03-29 16:58:00.726810 reflex-0.4.6a3/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.6a3/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3667 2024-03-29 16:58:00.727239 reflex-0.4.6a3/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    66152 2024-03-29 16:58:00.727489 reflex-0.4.6a3/reflex/components/component.py
--rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.6a3/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5937 2024-03-29 16:58:00.727967 reflex-0.4.6a3/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-03-29 16:58:00.728201 reflex-0.4.6a3/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.6a3/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6406 2024-03-29 16:58:00.728357 reflex-0.4.6a3/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.6a3/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6291 2024-03-28 16:38:22.950227 reflex-0.4.6a3/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.6a3/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4149 2024-03-29 16:58:00.728487 reflex-0.4.6a3/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.6a3/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.6a3/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-03-29 16:58:00.728640 reflex-0.4.6a3/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.6a3/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.6a3/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-03-28 16:38:22.951005 reflex-0.4.6a3/reflex/components/core/responsive.py
--rw-r--r--   0        0        0     8993 2024-03-20 23:54:55.842640 reflex-0.4.6a3/reflex/components/core/upload.py
--rw-r--r--   0        0        0     8667 2024-03-29 16:58:00.728756 reflex-0.4.6a3/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      334 2024-02-17 20:02:02.418838 reflex-0.4.6a3/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11227 2024-03-28 16:38:22.951420 reflex-0.4.6a3/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31107 2024-03-29 16:58:00.729100 reflex-0.4.6a3/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.6a3/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-03-29 16:58:00.729235 reflex-0.4.6a3/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.6a3/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.6a3/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.6a3/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.6a3/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.6a3/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.6a3/reflex/components/el/element.py
--rw-r--r--   0        0        0     3284 2024-03-29 16:58:00.729521 reflex-0.4.6a3/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.6a3/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.6a3/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6411 2024-03-29 16:58:00.729666 reflex-0.4.6a3/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20046 2024-03-29 13:41:30.691703 reflex-0.4.6a3/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0   100523 2024-03-29 16:58:00.729893 reflex-0.4.6a3/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.6a3/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   166595 2024-03-29 16:58:00.730238 reflex-0.4.6a3/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.6a3/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    94561 2024-03-29 16:58:00.730453 reflex-0.4.6a3/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.6a3/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28386 2024-03-29 16:58:00.730622 reflex-0.4.6a3/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.6a3/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42530 2024-03-29 16:58:00.730823 reflex-0.4.6a3/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.6a3/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19828 2024-03-29 16:58:00.731098 reflex-0.4.6a3/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.6a3/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    88307 2024-03-29 16:58:00.731379 reflex-0.4.6a3/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.6a3/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    62559 2024-03-29 16:58:00.731561 reflex-0.4.6a3/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.6a3/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    90180 2024-03-29 16:58:00.732029 reflex-0.4.6a3/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.6a3/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.6a3/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7124 2024-03-29 16:58:00.732267 reflex-0.4.6a3/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.6a3/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.6a3/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34206 2024-03-28 16:38:22.952671 reflex-0.4.6a3/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    38019 2024-03-29 16:58:00.732739 reflex-0.4.6a3/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.6a3/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    11348 2024-03-20 23:54:55.845491 reflex-0.4.6a3/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5387 2024-03-29 16:58:00.732913 reflex-0.4.6a3/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.6a3/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.6a3/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.6a3/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.6a3/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-03-29 16:58:00.733083 reflex-0.4.6a3/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.6a3/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.6a3/reflex/components/next/base.py
--rw-r--r--   0        0        0     3304 2024-03-29 16:58:00.733205 reflex-0.4.6a3/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.6a3/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-03-29 16:58:00.733348 reflex-0.4.6a3/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.6a3/reflex/components/next/link.py
--rw-r--r--   0        0        0     3532 2024-03-29 16:58:00.733475 reflex-0.4.6a3/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.6a3/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-03-29 16:58:00.733692 reflex-0.4.6a3/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.6a3/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.6a3/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     7007 2024-03-29 16:58:00.733965 reflex-0.4.6a3/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.6a3/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.6a3/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.6a3/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    26956 2024-03-29 16:58:00.734654 reflex-0.4.6a3/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.6a3/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6620 2024-03-29 16:58:00.734830 reflex-0.4.6a3/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.6a3/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34981 2024-03-29 16:58:00.734989 reflex-0.4.6a3/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.6a3/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48365 2024-03-29 16:58:00.735164 reflex-0.4.6a3/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.6a3/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22997 2024-03-29 16:58:00.735320 reflex-0.4.6a3/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.6a3/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    17052 2024-03-29 16:58:00.735456 reflex-0.4.6a3/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.6a3/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.6a3/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    24216 2024-03-29 16:58:00.735792 reflex-0.4.6a3/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.6a3/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    21283 2024-03-29 16:58:00.735967 reflex-0.4.6a3/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.6a3/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.6a3/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-03-29 16:58:00.736179 reflex-0.4.6a3/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.6a3/reflex/components/radix/themes/components/alertdialog.pyi
--rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.6a3/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-03-29 16:58:00.736340 reflex-0.4.6a3/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.6a3/reflex/components/radix/themes/components/aspectratio.pyi
--rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.6a3/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-03-29 16:58:00.736598 reflex-0.4.6a3/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.6a3/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9315 2024-03-29 16:58:00.736718 reflex-0.4.6a3/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.6a3/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11758 2024-03-29 16:58:00.736942 reflex-0.4.6a3/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.6a3/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-03-29 16:58:00.737085 reflex-0.4.6a3/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.6a3/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-03-29 16:58:00.737329 reflex-0.4.6a3/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.6a3/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-03-29 16:58:00.737593 reflex-0.4.6a3/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.6a3/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-03-29 16:58:00.737853 reflex-0.4.6a3/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.6a3/reflex/components/radix/themes/components/contextmenu.pyi
--rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.6a3/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-03-29 16:58:00.738034 reflex-0.4.6a3/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.6a3/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-03-29 16:58:00.738238 reflex-0.4.6a3/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.6a3/reflex/components/radix/themes/components/dropdownmenu.pyi
--rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.6a3/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-03-29 16:58:00.738395 reflex-0.4.6a3/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.6a3/reflex/components/radix/themes/components/hovercard.pyi
--rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.6a3/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    11916 2024-03-29 16:58:00.738544 reflex-0.4.6a3/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.6a3/reflex/components/radix/themes/components/iconbutton.pyi
--rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.6a3/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-03-29 16:58:00.738713 reflex-0.4.6a3/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.6a3/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-03-29 16:58:00.739092 reflex-0.4.6a3/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.6a3/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-03-29 16:58:00.739287 reflex-0.4.6a3/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.6a3/reflex/components/radix/themes/components/radiogroup.pyi
--rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.6a3/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-03-29 16:58:00.739462 reflex-0.4.6a3/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.6a3/reflex/components/radix/themes/components/scrollarea.pyi
--rw-r--r--   0        0        0     7906 2024-03-20 23:54:55.856284 reflex-0.4.6a3/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-03-29 16:58:00.739642 reflex-0.4.6a3/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.6a3/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-03-29 16:58:00.739823 reflex-0.4.6a3/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.6a3/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-03-29 16:58:00.739978 reflex-0.4.6a3/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.6a3/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-03-29 16:58:00.740131 reflex-0.4.6a3/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.6a3/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-03-29 16:58:00.740269 reflex-0.4.6a3/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.6a3/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    17321 2024-03-29 16:58:00.740387 reflex-0.4.6a3/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.6a3/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-03-29 16:58:00.740542 reflex-0.4.6a3/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.6a3/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    43043 2024-03-29 16:58:00.740692 reflex-0.4.6a3/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.6a3/reflex/components/radix/themes/components/textfield.pyi
--rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.6a3/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-03-29 16:58:00.740851 reflex-0.4.6a3/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-03-20 23:54:55.859034 reflex-0.4.6a3/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.6a3/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7643 2024-03-29 16:58:00.741107 reflex-0.4.6a3/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.6a3/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-03-29 16:58:00.741251 reflex-0.4.6a3/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.6a3/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8245 2024-03-29 16:58:00.741366 reflex-0.4.6a3/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.6a3/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     6779 2024-03-29 16:58:00.741604 reflex-0.4.6a3/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.6a3/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-03-29 16:58:00.741735 reflex-0.4.6a3/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.6a3/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-03-29 16:58:00.741865 reflex-0.4.6a3/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4889 2024-03-29 13:41:30.694246 reflex-0.4.6a3/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    29367 2024-03-29 16:58:00.741991 reflex-0.4.6a3/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.6a3/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-03-29 16:58:00.742213 reflex-0.4.6a3/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.6a3/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8245 2024-03-29 16:58:00.742320 reflex-0.4.6a3/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.6a3/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-03-29 16:58:00.742471 reflex-0.4.6a3/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.6a3/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.6a3/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.6a3/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-03-29 16:58:00.742613 reflex-0.4.6a3/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.6a3/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-03-29 16:58:00.742714 reflex-0.4.6a3/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.6a3/reflex/components/radix/themes/typography/em.pyi
--rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.6a3/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-03-29 16:58:00.742817 reflex-0.4.6a3/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.6a3/reflex/components/radix/themes/typography/kbd.pyi
--rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.6a3/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12063 2024-03-29 16:58:00.743022 reflex-0.4.6a3/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.6a3/reflex/components/radix/themes/typography/quote.pyi
--rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.6a3/reflex/components/radix/themes/typography/strong.pyi
--rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.6a3/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-03-29 16:58:00.743196 reflex-0.4.6a3/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.6a3/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.6a3/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4398 2024-03-29 16:58:00.743344 reflex-0.4.6a3/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.6a3/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4425 2024-03-29 16:58:00.743461 reflex-0.4.6a3/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.6a3/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4398 2024-03-29 16:58:00.743580 reflex-0.4.6a3/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.6a3/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.6a3/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    85500 2024-03-29 16:58:00.743745 reflex-0.4.6a3/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.6a3/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-03-29 16:58:00.743902 reflex-0.4.6a3/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.6a3/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    23071 2024-03-29 16:58:00.744013 reflex-0.4.6a3/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.6a3/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24752 2024-03-29 16:58:00.744142 reflex-0.4.6a3/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.6a3/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8606 2024-03-29 16:58:00.744267 reflex-0.4.6a3/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.6a3/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.6a3/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-03-29 16:58:00.744395 reflex-0.4.6a3/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.6a3/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.6a3/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.6a3/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.6a3/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.6a3/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.6a3/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    11089 2024-03-29 16:58:00.744513 reflex-0.4.6a3/reflex/config.py
--rw-r--r--   0        0        0     3325 2024-03-20 23:54:55.864565 reflex-0.4.6a3/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-03-20 23:54:55.864713 reflex-0.4.6a3/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5818 2024-03-20 23:54:55.864858 reflex-0.4.6a3/reflex/constants/base.py
--rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.6a3/reflex/constants/colors.py
--rw-r--r--   0        0        0     3852 2024-03-20 23:54:55.865208 reflex-0.4.6a3/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.6a3/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.6a3/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.6a3/reflex/constants/event.py
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.865387 reflex-0.4.6a3/reflex/constants/installer.py
--rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.6a3/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.6a3/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.6a3/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    32037 2024-04-01 18:35:29.811716 reflex-0.4.6a3/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    26634 2024-03-29 13:41:30.696386 reflex-0.4.6a3/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.6a3/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.6a3/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.6a3/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13091 2024-03-20 23:54:55.866065 reflex-0.4.6a3/reflex/model.py
--rw-r--r--   0        0        0     1922 2024-02-07 21:48:43.327922 reflex-0.4.6a3/reflex/page.py
--rw-r--r--   0        0        0    18257 2024-03-29 13:41:30.696694 reflex-0.4.6a3/reflex/reflex.py
--rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.6a3/reflex/route.py
--rw-r--r--   0        0        0   105642 2024-03-29 16:58:00.744911 reflex-0.4.6a3/reflex/state.py
--rw-r--r--   0        0        0     8820 2024-02-17 20:02:02.451439 reflex-0.4.6a3/reflex/style.py
--rw-r--r--   0        0        0    29811 2024-03-28 16:38:22.954494 reflex-0.4.6a3/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.6a3/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.6a3/reflex/utils/build.py
--rw-r--r--   0        0        0     4941 2024-03-28 16:38:22.954713 reflex-0.4.6a3/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.6a3/reflex/utils/exceptions.py
--rw-r--r--   0        0        0     9414 2024-03-20 23:54:55.867670 reflex-0.4.6a3/reflex/utils/exec.py
--rw-r--r--   0        0        0     2454 2024-02-06 00:51:32.032368 reflex-0.4.6a3/reflex/utils/export.py
--rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.6a3/reflex/utils/format.py
--rw-r--r--   0        0        0     1919 2023-12-01 04:51:31.117478 reflex-0.4.6a3/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.6a3/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    38849 2024-03-28 16:38:22.955049 reflex-0.4.6a3/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     8279 2024-03-28 16:38:22.955216 reflex-0.4.6a3/reflex/utils/processes.py
--rw-r--r--   0        0        0    27674 2024-03-29 16:58:00.745050 reflex-0.4.6a3/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     8538 2024-03-20 23:54:55.868965 reflex-0.4.6a3/reflex/utils/serializers.py
--rw-r--r--   0        0        0     3760 2024-03-20 23:54:55.869231 reflex-0.4.6a3/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    13585 2024-03-29 16:58:00.745225 reflex-0.4.6a3/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.6a3/reflex/utils/watch.py
--rw-r--r--   0        0        0    67145 2024-03-28 16:38:22.956455 reflex-0.4.6a3/reflex/vars.py
--rw-r--r--   0        0        0     5575 2024-03-20 23:54:55.869763 reflex-0.4.6a3/reflex/vars.pyi
--rw-r--r--   0        0        0    11367 1970-01-01 00:00:00.000000 reflex-0.4.6a3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.6a4/LICENSE
+-rw-r--r--   0        0        0     9171 2024-03-29 16:58:00.709441 reflex-0.4.6a4/README.md
+-rw-r--r--   0        0        0     2922 2024-04-01 22:59:11.356406 reflex-0.4.6a4/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.6a4/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.6a4/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      838 2024-03-20 23:54:55.828973 reflex-0.4.6a4/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.6a4/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.6a4/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.6a4/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.6a4/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.6a4/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.6a4/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.6a4/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.6a4/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.6a4/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.6a4/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.6a4/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.6a4/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.6a4/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0     2392 2024-03-20 23:54:55.830719 reflex-0.4.6a4/reflex/.templates/apps/sidebar/README.md
+-rw-r--r--   0        0        0     4286 2023-11-22 05:49:24.665793 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-22 05:49:24.665902 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/github.svg
+-rw-r--r--   0        0        0     5403 2023-11-22 05:49:24.666131 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-22 05:49:24.666228 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/paneleft.svg
+-rw-r--r--   0        0        0     1899 2024-03-20 23:54:55.831004 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/reflex_black.svg
+-rw-r--r--   0        0        0      908 2024-03-20 23:54:55.831285 reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/reflex_white.svg
+-rw-r--r--   0        0        0       32 2023-11-22 05:49:24.666441 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-22 05:49:24.666586 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/components/__init__.py
+-rw-r--r--   0        0        0     3906 2024-03-20 23:54:55.831486 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/components/sidebar.py
+-rw-r--r--   0        0        0       89 2023-11-22 05:49:24.666931 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/pages/__init__.py
+-rw-r--r--   0        0        0      490 2024-03-20 23:54:55.831633 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/pages/dashboard.py
+-rw-r--r--   0        0        0      436 2023-11-22 05:49:24.667170 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/pages/index.py
+-rw-r--r--   0        0        0     1571 2024-03-20 23:54:55.831956 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/pages/settings.py
+-rw-r--r--   0        0        0      270 2024-02-06 00:51:31.970017 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/sidebar.py
+-rw-r--r--   0        0        0     1570 2024-03-20 23:54:55.832516 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/styles.py
+-rw-r--r--   0        0        0       43 2024-03-20 23:54:55.832690 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/templates/__init__.py
+-rw-r--r--   0        0        0     3904 2024-03-20 23:54:55.832868 reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/templates/template.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.6a4/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.6a4/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.6a4/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.6a4/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      615 2024-03-29 13:41:30.688966 reflex-0.4.6a4/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2262 2024-03-20 23:54:55.833729 reflex-0.4.6a4/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.6a4/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      412 2024-03-28 16:38:22.949259 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      461 2024-03-28 16:38:22.949386 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.6a4/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.6a4/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.6a4/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.6a4/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.6a4/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.6a4/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.6a4/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.6a4/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.6a4/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.6a4/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.6a4/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.6a4/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.6a4/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.6a4/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.6a4/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0    21563 2024-03-29 16:58:00.711812 reflex-0.4.6a4/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5676 2024-03-29 16:58:00.711989 reflex-0.4.6a4/reflex/__init__.py
+-rw-r--r--   0        0        0     7565 2024-03-29 16:58:00.712124 reflex-0.4.6a4/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.6a4/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.6a4/reflex/admin.py
+-rw-r--r--   0        0        0    44631 2024-03-29 16:58:00.712540 reflex-0.4.6a4/reflex/app.py
+-rw-r--r--   0        0        0     4928 2024-03-20 23:54:55.837030 reflex-0.4.6a4/reflex/app.pyi
+-rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.6a4/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4250 2024-03-29 16:58:00.713739 reflex-0.4.6a4/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.6a4/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17012 2024-03-28 16:38:22.949522 reflex-0.4.6a4/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.6a4/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    13997 2024-03-29 16:58:00.713923 reflex-0.4.6a4/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.6a4/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.6a4/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.6a4/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-03-29 16:58:00.714454 reflex-0.4.6a4/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-03-29 16:58:00.714593 reflex-0.4.6a4/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.6a4/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3277 2024-03-29 16:58:00.714744 reflex-0.4.6a4/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.6a4/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14587 2024-03-29 16:58:00.714887 reflex-0.4.6a4/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.6a4/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3289 2024-03-29 16:58:00.715025 reflex-0.4.6a4/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.6a4/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6073 2024-03-29 16:58:00.715201 reflex-0.4.6a4/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.6a4/reflex/components/base/link.py
+-rw-r--r--   0        0        0     7132 2024-03-29 16:58:00.715592 reflex-0.4.6a4/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.6a4/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    13088 2024-03-29 16:58:00.715862 reflex-0.4.6a4/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.6a4/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-03-29 16:58:00.716023 reflex-0.4.6a4/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.6a4/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.6a4/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    11059 2024-03-29 16:58:00.716548 reflex-0.4.6a4/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.6a4/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.6a4/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3725 2024-03-29 16:58:00.716690 reflex-0.4.6a4/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.6a4/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3300 2024-03-29 16:58:00.716857 reflex-0.4.6a4/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.6a4/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     4005 2024-03-29 16:58:00.717106 reflex-0.4.6a4/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.6a4/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3322 2024-03-29 16:58:00.717227 reflex-0.4.6a4/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.6a4/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    13065 2024-03-29 16:58:00.717356 reflex-0.4.6a4/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.6a4/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17816 2024-03-29 16:58:00.717520 reflex-0.4.6a4/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.6a4/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27536 2024-03-29 16:58:00.717709 reflex-0.4.6a4/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.6a4/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    16018 2024-03-29 16:58:00.717856 reflex-0.4.6a4/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.6a4/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.6a4/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    16087 2024-03-29 16:58:00.718197 reflex-0.4.6a4/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.6a4/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18809 2024-03-29 16:58:00.718354 reflex-0.4.6a4/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.6a4/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20429 2024-03-29 16:58:00.718551 reflex-0.4.6a4/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.6a4/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3329 2024-03-29 16:58:00.718696 reflex-0.4.6a4/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.6a4/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.6a4/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12594 2024-03-29 16:58:00.718821 reflex-0.4.6a4/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.6a4/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7708 2024-03-29 16:58:00.718976 reflex-0.4.6a4/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.6a4/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4349 2024-03-29 16:58:00.719131 reflex-0.4.6a4/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.6a4/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10903 2024-03-29 16:58:00.719257 reflex-0.4.6a4/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.6a4/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4178 2024-03-29 16:58:00.719399 reflex-0.4.6a4/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.6a4/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.6a4/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10687 2024-03-29 16:58:00.719754 reflex-0.4.6a4/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.6a4/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10443 2024-03-29 16:58:00.720133 reflex-0.4.6a4/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.6a4/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18530 2024-03-29 16:58:00.720262 reflex-0.4.6a4/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.6a4/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-03-29 16:58:00.720401 reflex-0.4.6a4/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.6a4/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-03-29 16:58:00.720529 reflex-0.4.6a4/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.6a4/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13623 2024-03-29 16:58:00.720743 reflex-0.4.6a4/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.6a4/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-03-29 16:58:00.720895 reflex-0.4.6a4/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.6a4/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20832 2024-03-29 16:58:00.721043 reflex-0.4.6a4/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.6a4/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4739 2024-03-29 16:58:00.721237 reflex-0.4.6a4/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.6a4/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21869 2024-03-29 16:58:00.721368 reflex-0.4.6a4/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.6a4/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.6a4/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18377 2024-03-29 16:58:00.721513 reflex-0.4.6a4/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.6a4/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-03-29 16:58:00.721666 reflex-0.4.6a4/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6501 2024-02-07 21:48:43.279255 reflex-0.4.6a4/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9432 2024-03-29 16:58:00.721794 reflex-0.4.6a4/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3176 2024-02-07 21:48:43.279649 reflex-0.4.6a4/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8414 2024-03-29 16:58:00.721926 reflex-0.4.6a4/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4547 2024-02-07 21:48:43.279975 reflex-0.4.6a4/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    14156 2024-03-29 16:58:00.722060 reflex-0.4.6a4/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.6a4/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-03-29 16:58:00.722172 reflex-0.4.6a4/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.6a4/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17745 2024-03-29 16:58:00.722496 reflex-0.4.6a4/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.6a4/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6602 2024-03-29 16:58:00.722723 reflex-0.4.6a4/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.6a4/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-03-29 16:58:00.722906 reflex-0.4.6a4/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.6a4/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-03-29 16:58:00.723061 reflex-0.4.6a4/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.6a4/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.6a4/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3450 2024-03-29 16:58:00.723207 reflex-0.4.6a4/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.6a4/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3733 2024-03-29 16:58:00.723333 reflex-0.4.6a4/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.6a4/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    14063 2024-03-29 16:58:00.723473 reflex-0.4.6a4/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.6a4/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8905 2024-03-29 16:58:00.723622 reflex-0.4.6a4/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.6a4/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3502 2024-03-29 16:58:00.723745 reflex-0.4.6a4/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.6a4/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4209 2024-03-29 16:58:00.723875 reflex-0.4.6a4/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.6a4/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    14066 2024-03-29 16:58:00.724005 reflex-0.4.6a4/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.6a4/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3301 2024-03-29 16:58:00.724121 reflex-0.4.6a4/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.6a4/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12432 2024-03-29 16:58:00.724241 reflex-0.4.6a4/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.6a4/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     7014 2024-03-29 16:58:00.724378 reflex-0.4.6a4/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.6a4/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.6a4/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10658 2024-03-29 16:58:00.724498 reflex-0.4.6a4/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.6a4/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6342 2024-03-29 16:58:00.724631 reflex-0.4.6a4/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.6a4/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-03-29 16:58:00.724932 reflex-0.4.6a4/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.6a4/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.6a4/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13646 2024-03-29 16:58:00.725095 reflex-0.4.6a4/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.6a4/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-03-29 16:58:00.725268 reflex-0.4.6a4/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.6a4/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6375 2024-03-29 16:58:00.725401 reflex-0.4.6a4/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.6a4/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    28490 2024-03-29 16:58:00.725535 reflex-0.4.6a4/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.6a4/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.6a4/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    24411 2024-03-29 16:58:00.725691 reflex-0.4.6a4/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.6a4/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25832 2024-03-29 16:58:00.725823 reflex-0.4.6a4/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.6a4/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    29108 2024-03-29 16:58:00.725942 reflex-0.4.6a4/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.6a4/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23975 2024-03-29 16:58:00.726063 reflex-0.4.6a4/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.6a4/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    30461 2024-03-29 16:58:00.726195 reflex-0.4.6a4/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.6a4/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6131 2024-03-29 16:58:00.726350 reflex-0.4.6a4/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.6a4/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.6a4/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3777 2024-03-29 16:58:00.726564 reflex-0.4.6a4/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.6a4/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3716 2024-03-29 16:58:00.726676 reflex-0.4.6a4/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.6a4/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3443 2024-03-29 16:58:00.726810 reflex-0.4.6a4/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.6a4/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3667 2024-03-29 16:58:00.727239 reflex-0.4.6a4/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    65276 2024-04-01 22:58:36.881174 reflex-0.4.6a4/reflex/components/component.py
+-rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.6a4/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5937 2024-03-29 16:58:00.727967 reflex-0.4.6a4/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-03-29 16:58:00.728201 reflex-0.4.6a4/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.6a4/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6406 2024-03-29 16:58:00.728357 reflex-0.4.6a4/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.6a4/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6291 2024-03-28 16:38:22.950227 reflex-0.4.6a4/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.6a4/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4149 2024-03-29 16:58:00.728487 reflex-0.4.6a4/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.6a4/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.6a4/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-03-29 16:58:00.728640 reflex-0.4.6a4/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.6a4/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.6a4/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-03-28 16:38:22.951005 reflex-0.4.6a4/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0     8993 2024-03-20 23:54:55.842640 reflex-0.4.6a4/reflex/components/core/upload.py
+-rw-r--r--   0        0        0     8667 2024-03-29 16:58:00.728756 reflex-0.4.6a4/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      334 2024-02-17 20:02:02.418838 reflex-0.4.6a4/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11227 2024-03-28 16:38:22.951420 reflex-0.4.6a4/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31107 2024-03-29 16:58:00.729100 reflex-0.4.6a4/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.6a4/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-03-29 16:58:00.729235 reflex-0.4.6a4/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.6a4/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.6a4/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.6a4/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.6a4/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.6a4/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.6a4/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3284 2024-03-29 16:58:00.729521 reflex-0.4.6a4/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.6a4/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.6a4/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6411 2024-03-29 16:58:00.729666 reflex-0.4.6a4/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20046 2024-03-29 13:41:30.691703 reflex-0.4.6a4/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0   100523 2024-03-29 16:58:00.729893 reflex-0.4.6a4/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.6a4/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   166595 2024-03-29 16:58:00.730238 reflex-0.4.6a4/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.6a4/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    94561 2024-03-29 16:58:00.730453 reflex-0.4.6a4/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.6a4/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28386 2024-03-29 16:58:00.730622 reflex-0.4.6a4/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.6a4/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42530 2024-03-29 16:58:00.730823 reflex-0.4.6a4/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.6a4/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19828 2024-03-29 16:58:00.731098 reflex-0.4.6a4/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.6a4/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    88307 2024-03-29 16:58:00.731379 reflex-0.4.6a4/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.6a4/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    62559 2024-03-29 16:58:00.731561 reflex-0.4.6a4/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.6a4/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    90180 2024-03-29 16:58:00.732029 reflex-0.4.6a4/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.6a4/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.6a4/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7124 2024-03-29 16:58:00.732267 reflex-0.4.6a4/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.6a4/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.6a4/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34206 2024-03-28 16:38:22.952671 reflex-0.4.6a4/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    38019 2024-03-29 16:58:00.732739 reflex-0.4.6a4/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.6a4/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    11348 2024-03-20 23:54:55.845491 reflex-0.4.6a4/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5387 2024-03-29 16:58:00.732913 reflex-0.4.6a4/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.6a4/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.6a4/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.6a4/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.6a4/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-03-29 16:58:00.733083 reflex-0.4.6a4/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.6a4/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.6a4/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3304 2024-03-29 16:58:00.733205 reflex-0.4.6a4/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.6a4/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-03-29 16:58:00.733348 reflex-0.4.6a4/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.6a4/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3532 2024-03-29 16:58:00.733475 reflex-0.4.6a4/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.6a4/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-03-29 16:58:00.733692 reflex-0.4.6a4/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.6a4/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.6a4/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     7007 2024-03-29 16:58:00.733965 reflex-0.4.6a4/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.6a4/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.6a4/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.6a4/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    26956 2024-03-29 16:58:00.734654 reflex-0.4.6a4/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.6a4/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6620 2024-03-29 16:58:00.734830 reflex-0.4.6a4/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.6a4/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34981 2024-03-29 16:58:00.734989 reflex-0.4.6a4/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.6a4/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48365 2024-03-29 16:58:00.735164 reflex-0.4.6a4/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.6a4/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22997 2024-03-29 16:58:00.735320 reflex-0.4.6a4/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.6a4/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    17052 2024-03-29 16:58:00.735456 reflex-0.4.6a4/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.6a4/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.6a4/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    24216 2024-03-29 16:58:00.735792 reflex-0.4.6a4/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.6a4/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    21283 2024-03-29 16:58:00.735967 reflex-0.4.6a4/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.6a4/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.6a4/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-03-29 16:58:00.736179 reflex-0.4.6a4/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.6a4/reflex/components/radix/themes/components/alertdialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.6a4/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-03-29 16:58:00.736340 reflex-0.4.6a4/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.6a4/reflex/components/radix/themes/components/aspectratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.6a4/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-03-29 16:58:00.736598 reflex-0.4.6a4/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.6a4/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9315 2024-03-29 16:58:00.736718 reflex-0.4.6a4/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.6a4/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11758 2024-03-29 16:58:00.736942 reflex-0.4.6a4/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.6a4/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-03-29 16:58:00.737085 reflex-0.4.6a4/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.6a4/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-03-29 16:58:00.737329 reflex-0.4.6a4/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.6a4/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-03-29 16:58:00.737593 reflex-0.4.6a4/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.6a4/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-03-29 16:58:00.737853 reflex-0.4.6a4/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.6a4/reflex/components/radix/themes/components/contextmenu.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.6a4/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-03-29 16:58:00.738034 reflex-0.4.6a4/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.6a4/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-03-29 16:58:00.738238 reflex-0.4.6a4/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.6a4/reflex/components/radix/themes/components/dropdownmenu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.6a4/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-03-29 16:58:00.738395 reflex-0.4.6a4/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.6a4/reflex/components/radix/themes/components/hovercard.pyi
+-rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.6a4/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    11916 2024-03-29 16:58:00.738544 reflex-0.4.6a4/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.6a4/reflex/components/radix/themes/components/iconbutton.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.6a4/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-03-29 16:58:00.738713 reflex-0.4.6a4/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.6a4/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-03-29 16:58:00.739092 reflex-0.4.6a4/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.6a4/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-03-29 16:58:00.739287 reflex-0.4.6a4/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.6a4/reflex/components/radix/themes/components/radiogroup.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.6a4/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-03-29 16:58:00.739462 reflex-0.4.6a4/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.6a4/reflex/components/radix/themes/components/scrollarea.pyi
+-rw-r--r--   0        0        0     7906 2024-03-20 23:54:55.856284 reflex-0.4.6a4/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-03-29 16:58:00.739642 reflex-0.4.6a4/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.6a4/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-03-29 16:58:00.739823 reflex-0.4.6a4/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.6a4/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-03-29 16:58:00.739978 reflex-0.4.6a4/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.6a4/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-03-29 16:58:00.740131 reflex-0.4.6a4/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.6a4/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-03-29 16:58:00.740269 reflex-0.4.6a4/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.6a4/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    17321 2024-03-29 16:58:00.740387 reflex-0.4.6a4/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.6a4/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-03-29 16:58:00.740542 reflex-0.4.6a4/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.6a4/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    43043 2024-03-29 16:58:00.740692 reflex-0.4.6a4/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.6a4/reflex/components/radix/themes/components/textfield.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.6a4/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-03-29 16:58:00.740851 reflex-0.4.6a4/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-03-20 23:54:55.859034 reflex-0.4.6a4/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.6a4/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7643 2024-03-29 16:58:00.741107 reflex-0.4.6a4/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.6a4/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-03-29 16:58:00.741251 reflex-0.4.6a4/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.6a4/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8245 2024-03-29 16:58:00.741366 reflex-0.4.6a4/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.6a4/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     6779 2024-03-29 16:58:00.741604 reflex-0.4.6a4/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.6a4/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-03-29 16:58:00.741735 reflex-0.4.6a4/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.6a4/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-03-29 16:58:00.741865 reflex-0.4.6a4/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4889 2024-03-29 13:41:30.694246 reflex-0.4.6a4/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29367 2024-03-29 16:58:00.741991 reflex-0.4.6a4/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.6a4/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-03-29 16:58:00.742213 reflex-0.4.6a4/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.6a4/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8245 2024-03-29 16:58:00.742320 reflex-0.4.6a4/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.6a4/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-03-29 16:58:00.742471 reflex-0.4.6a4/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.6a4/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.6a4/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.6a4/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-03-29 16:58:00.742613 reflex-0.4.6a4/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.6a4/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-03-29 16:58:00.742714 reflex-0.4.6a4/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.6a4/reflex/components/radix/themes/typography/em.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.6a4/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-03-29 16:58:00.742817 reflex-0.4.6a4/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.6a4/reflex/components/radix/themes/typography/kbd.pyi
+-rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.6a4/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12063 2024-03-29 16:58:00.743022 reflex-0.4.6a4/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.6a4/reflex/components/radix/themes/typography/quote.pyi
+-rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.6a4/reflex/components/radix/themes/typography/strong.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.6a4/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-03-29 16:58:00.743196 reflex-0.4.6a4/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.6a4/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.6a4/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4398 2024-03-29 16:58:00.743344 reflex-0.4.6a4/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.6a4/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4425 2024-03-29 16:58:00.743461 reflex-0.4.6a4/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.6a4/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4398 2024-03-29 16:58:00.743580 reflex-0.4.6a4/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.6a4/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.6a4/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    85500 2024-03-29 16:58:00.743745 reflex-0.4.6a4/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.6a4/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-03-29 16:58:00.743902 reflex-0.4.6a4/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.6a4/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    23071 2024-03-29 16:58:00.744013 reflex-0.4.6a4/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.6a4/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24752 2024-03-29 16:58:00.744142 reflex-0.4.6a4/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.6a4/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8606 2024-03-29 16:58:00.744267 reflex-0.4.6a4/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.6a4/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.6a4/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-03-29 16:58:00.744395 reflex-0.4.6a4/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.6a4/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.6a4/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.6a4/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.6a4/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.6a4/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.6a4/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    11089 2024-03-29 16:58:00.744513 reflex-0.4.6a4/reflex/config.py
+-rw-r--r--   0        0        0     3325 2024-03-20 23:54:55.864565 reflex-0.4.6a4/reflex/config.pyi
+-rw-r--r--   0        0        0     2036 2024-03-20 23:54:55.864713 reflex-0.4.6a4/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5818 2024-03-20 23:54:55.864858 reflex-0.4.6a4/reflex/constants/base.py
+-rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.6a4/reflex/constants/colors.py
+-rw-r--r--   0        0        0     3852 2024-03-20 23:54:55.865208 reflex-0.4.6a4/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.6a4/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.6a4/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.6a4/reflex/constants/event.py
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.865387 reflex-0.4.6a4/reflex/constants/installer.py
+-rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.6a4/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.6a4/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.6a4/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    32037 2024-04-01 18:35:29.811716 reflex-0.4.6a4/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    26634 2024-03-29 13:41:30.696386 reflex-0.4.6a4/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.6a4/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.6a4/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.6a4/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13091 2024-03-20 23:54:55.866065 reflex-0.4.6a4/reflex/model.py
+-rw-r--r--   0        0        0     1922 2024-02-07 21:48:43.327922 reflex-0.4.6a4/reflex/page.py
+-rw-r--r--   0        0        0    18257 2024-03-29 13:41:30.696694 reflex-0.4.6a4/reflex/reflex.py
+-rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.6a4/reflex/route.py
+-rw-r--r--   0        0        0   105642 2024-03-29 16:58:00.744911 reflex-0.4.6a4/reflex/state.py
+-rw-r--r--   0        0        0     8820 2024-02-17 20:02:02.451439 reflex-0.4.6a4/reflex/style.py
+-rw-r--r--   0        0        0    29811 2024-03-28 16:38:22.954494 reflex-0.4.6a4/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.6a4/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.6a4/reflex/utils/build.py
+-rw-r--r--   0        0        0     4941 2024-03-28 16:38:22.954713 reflex-0.4.6a4/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.6a4/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0     9414 2024-03-20 23:54:55.867670 reflex-0.4.6a4/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2454 2024-02-06 00:51:32.032368 reflex-0.4.6a4/reflex/utils/export.py
+-rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.6a4/reflex/utils/format.py
+-rw-r--r--   0        0        0     1919 2023-12-01 04:51:31.117478 reflex-0.4.6a4/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.6a4/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    38849 2024-03-28 16:38:22.955049 reflex-0.4.6a4/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     8279 2024-03-28 16:38:22.955216 reflex-0.4.6a4/reflex/utils/processes.py
+-rw-r--r--   0        0        0    27674 2024-03-29 16:58:00.745050 reflex-0.4.6a4/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     8538 2024-03-20 23:54:55.868965 reflex-0.4.6a4/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     3760 2024-03-20 23:54:55.869231 reflex-0.4.6a4/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    13585 2024-03-29 16:58:00.745225 reflex-0.4.6a4/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.6a4/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67145 2024-03-28 16:38:22.956455 reflex-0.4.6a4/reflex/vars.py
+-rw-r--r--   0        0        0     5575 2024-03-20 23:54:55.869763 reflex-0.4.6a4/reflex/vars.pyi
+-rw-r--r--   0        0        0    11367 1970-01-01 00:00:00.000000 reflex-0.4.6a4/PKG-INFO
```

### Comparing `reflex-0.4.6a3/LICENSE` & `reflex-0.4.6a4/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/README.md` & `reflex-0.4.6a4/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/pyproject.toml` & `reflex-0.4.6a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.4.6a3"
+version = "0.4.6a4"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
@@ -81,15 +81,14 @@
 pillow = [
     {version = ">=10.0.0,<11.0", python = ">=3.8,<4.0"}
 ]
 plotly = ">=5.13.0,<6.0"
 asynctest = ">=0.13.0,<1.0"
 pre-commit = {version = ">=3.2.1", python = ">=3.8,<4.0"}
 selenium = ">=4.11.0,<5.0"
-types-tabulate = ">=0.9.0.3,<0.10"
 pytest-benchmark = ">=4.0.0,<5.0"
 
 [tool.poetry.scripts]
 reflex = "reflex.reflex:cli"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
```

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.4.6a4/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.4.6a4/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.4.6a4/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.4.6a4/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.4.6a4/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.4.6a4/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.4.6a4/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.4.6a4/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/README.md` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/favicon.ico` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/github.svg` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/logo.svg` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/paneleft.svg` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/reflex_black.svg` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/reflex_black.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/assets/reflex_white.svg` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/assets/reflex_white.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/components/sidebar.py` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/pages/settings.py` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/pages/settings.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/styles.py` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/apps/sidebar/code/templates/template.py` & `reflex-0.4.6a4/reflex/.templates/apps/sidebar/code/templates/template.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.4.6a4/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.4.6a4/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.4.6a4/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.4.6a4/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.4.6a4/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.4.6a4/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/.templates/web/utils/state.js` & `reflex-0.4.6a4/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/__init__.py` & `reflex-0.4.6a4/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/__init__.pyi` & `reflex-0.4.6a4/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/app.py` & `reflex-0.4.6a4/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/app.pyi` & `reflex-0.4.6a4/reflex/app.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/app_module_for_backend.py` & `reflex-0.4.6a4/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/base.py` & `reflex-0.4.6a4/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/compiler/compiler.py` & `reflex-0.4.6a4/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/compiler/templates.py` & `reflex-0.4.6a4/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/compiler/utils.py` & `reflex-0.4.6a4/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/__init__.py` & `reflex-0.4.6a4/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/app_wrap.py` & `reflex-0.4.6a4/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/app_wrap.pyi` & `reflex-0.4.6a4/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/bare.py` & `reflex-0.4.6a4/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/body.pyi` & `reflex-0.4.6a4/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/document.py` & `reflex-0.4.6a4/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/document.pyi` & `reflex-0.4.6a4/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/fragment.pyi` & `reflex-0.4.6a4/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/head.pyi` & `reflex-0.4.6a4/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/link.py` & `reflex-0.4.6a4/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/link.pyi` & `reflex-0.4.6a4/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/meta.py` & `reflex-0.4.6a4/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/meta.pyi` & `reflex-0.4.6a4/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/script.py` & `reflex-0.4.6a4/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/base/script.pyi` & `reflex-0.4.6a4/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/__init__.py` & `reflex-0.4.6a4/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/base.py` & `reflex-0.4.6a4/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/base.pyi` & `reflex-0.4.6a4/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/list.py` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/table.py` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.4.6a4/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/transition.py` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.4.6a4/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/alert.py` & `reflex-0.4.6a4/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.4.6a4/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.4.6a4/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.4.6a4/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/progress.py` & `reflex-0.4.6a4/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.4.6a4/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.4.6a4/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.4.6a4/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/spinner.py` & `reflex-0.4.6a4/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.4.6a4/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/__init__.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/button.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/button.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/checkbox.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/editable.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/editable.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/email.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/form.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/form.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/input.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/input.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/multiselect.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/numberinput.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/password.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/pininput.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/radio.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/radio.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/select.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/select.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/slider.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/slider.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/switch.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/switch.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/textarea.py` & `reflex-0.4.6a4/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.4.6a4/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/box.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/box.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/card.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/card.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/center.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/container.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/flex.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/flex.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/grid.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/grid.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/stack.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/stack.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/wrap.py` & `reflex-0.4.6a4/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.4.6a4/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/avatar.py` & `reflex-0.4.6a4/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/avatar.pyi` & `reflex-0.4.6a4/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/icon.py` & `reflex-0.4.6a4/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/icon.pyi` & `reflex-0.4.6a4/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/image.py` & `reflex-0.4.6a4/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/media/image.pyi` & `reflex-0.4.6a4/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.4.6a4/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.4.6a4/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/link.py` & `reflex-0.4.6a4/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/link.pyi` & `reflex-0.4.6a4/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.4.6a4/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.4.6a4/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/stepper.py` & `reflex-0.4.6a4/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.4.6a4/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/__init__.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/drawer.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/menu.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/modal.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/popover.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.4.6a4/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.4.6a4/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/typography/heading.pyi` & `reflex-0.4.6a4/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/typography/highlight.py` & `reflex-0.4.6a4/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.4.6a4/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/typography/span.pyi` & `reflex-0.4.6a4/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/chakra/typography/text.pyi` & `reflex-0.4.6a4/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/component.py` & `reflex-0.4.6a4/reflex/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1025,24 +1025,14 @@
                 {
                     ImportVar(tag="useRef"),
                     ImportVar(tag="useEffect"),
                 },
             )
         return _imports
 
-    def add_imports(
-        self,
-    ) -> Dict[str, Union[str, ImportVar, List[str | ImportVar]]]:
-        """User defined imports for the component. Need to be overriden in subclass.
-
-        Returns:
-            The user defined imports as a dict.
-        """
-        return {}
-
     def _get_imports(self) -> imports.ImportDict:
         """Get all the libraries and fields that are used by the component.
 
         Returns:
             The imports needed by the component.
         """
         _imports = {}
@@ -1055,37 +1045,20 @@
         event_imports = Imports.EVENTS if self.event_triggers else {}
 
         # Collect imports from Vars used directly by this component.
         var_imports = [
             var._var_data.imports for var in self._get_vars() if var._var_data
         ]
 
-        # If the subclass implements add_imports, merge the imports.
-        def _make_list(
-            value: str | ImportVar | list[str | ImportVar],
-        ) -> list[str | ImportVar]:
-            if isinstance(value, (str, ImportVar)):
-                return [value]
-            return value
-
-        added_imports = {
-            package: [
-                ImportVar(tag=tag) if not isinstance(tag, ImportVar) else tag
-                for tag in _make_list(maybe_tags)
-            ]
-            for package, maybe_tags in self.add_imports().items()
-        }
-
         return imports.merge_imports(
             *self._get_props_imports(),
             self._get_dependencies_imports(),
             self._get_hooks_imports(),
             _imports,
             event_imports,
-            added_imports,
             *var_imports,
         )
 
     def get_imports(self, collapse: bool = False) -> imports.ImportDict:
         """Get all the libraries and fields that are used by the component and its children.
 
         Args:
```

### Comparing `reflex-0.4.6a3/reflex/components/core/__init__.py` & `reflex-0.4.6a4/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/banner.py` & `reflex-0.4.6a4/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/banner.pyi` & `reflex-0.4.6a4/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/client_side_routing.py` & `reflex-0.4.6a4/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/client_side_routing.pyi` & `reflex-0.4.6a4/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/colors.py` & `reflex-0.4.6a4/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/cond.py` & `reflex-0.4.6a4/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/debounce.py` & `reflex-0.4.6a4/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/debounce.pyi` & `reflex-0.4.6a4/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/foreach.py` & `reflex-0.4.6a4/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/html.py` & `reflex-0.4.6a4/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/html.pyi` & `reflex-0.4.6a4/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/match.py` & `reflex-0.4.6a4/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/responsive.py` & `reflex-0.4.6a4/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/upload.py` & `reflex-0.4.6a4/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/core/upload.pyi` & `reflex-0.4.6a4/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/datadisplay/code.py` & `reflex-0.4.6a4/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/datadisplay/code.pyi` & `reflex-0.4.6a4/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/datadisplay/dataeditor.py` & `reflex-0.4.6a4/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.4.6a4/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/constants/html.py` & `reflex-0.4.6a4/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/constants/react.py` & `reflex-0.4.6a4/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/constants/reflex.py` & `reflex-0.4.6a4/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/element.pyi` & `reflex-0.4.6a4/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/__init__.py` & `reflex-0.4.6a4/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/base.py` & `reflex-0.4.6a4/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/base.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/forms.py` & `reflex-0.4.6a4/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/forms.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/inline.py` & `reflex-0.4.6a4/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/inline.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/media.py` & `reflex-0.4.6a4/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/media.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/metadata.py` & `reflex-0.4.6a4/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/metadata.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/other.py` & `reflex-0.4.6a4/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/other.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/scripts.py` & `reflex-0.4.6a4/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/scripts.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/sectioning.py` & `reflex-0.4.6a4/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/sectioning.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/tables.py` & `reflex-0.4.6a4/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/tables.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/typography.py` & `reflex-0.4.6a4/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/el/elements/typography.pyi` & `reflex-0.4.6a4/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/gridjs/datatable.py` & `reflex-0.4.6a4/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/gridjs/datatable.pyi` & `reflex-0.4.6a4/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/lucide/icon.py` & `reflex-0.4.6a4/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/lucide/icon.pyi` & `reflex-0.4.6a4/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/markdown/markdown.py` & `reflex-0.4.6a4/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/markdown/markdown.pyi` & `reflex-0.4.6a4/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/moment/moment.py` & `reflex-0.4.6a4/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/moment/moment.pyi` & `reflex-0.4.6a4/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/base.pyi` & `reflex-0.4.6a4/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/image.py` & `reflex-0.4.6a4/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/image.pyi` & `reflex-0.4.6a4/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/link.pyi` & `reflex-0.4.6a4/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/video.py` & `reflex-0.4.6a4/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/next/video.pyi` & `reflex-0.4.6a4/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/plotly/plotly.py` & `reflex-0.4.6a4/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/plotly/plotly.pyi` & `reflex-0.4.6a4/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/accordion.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/base.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/base.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/drawer.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/form.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/form.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/progress.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/progress.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/slider.py` & `reflex-0.4.6a4/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/primitives/slider.pyi` & `reflex-0.4.6a4/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/base.py` & `reflex-0.4.6a4/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/base.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/color_mode.py` & `reflex-0.4.6a4/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/__init__.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/alertdialog.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/aspectratio.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/aspectratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/avatar.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/badge.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/button.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/button.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/callout.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/card.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/card.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/contextmenu.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/contextmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/dialog.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/dropdownmenu.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/dropdownmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/hovercard.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/hovercard.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/iconbutton.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/inset.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/popover.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/radiogroup.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/radiogroup.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/scrollarea.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/scrollarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/select.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/select.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/separator.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/slider.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/switch.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/table.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/table.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/tabs.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/text_area.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/text_field.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/textfield.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/textfield.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.4.6a4/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/base.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/container.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/flex.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/grid.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/list.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/stack.py` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/code.py` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/em.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/em.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/heading.py` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/kbd.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/kbd.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/link.py` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/quote.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/quote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/strong.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/strong.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/text.py` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.4.6a4/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/react_player/audio.pyi` & `reflex-0.4.6a4/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/react_player/react_player.py` & `reflex-0.4.6a4/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/react_player/react_player.pyi` & `reflex-0.4.6a4/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/react_player/video.pyi` & `reflex-0.4.6a4/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/__init__.py` & `reflex-0.4.6a4/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/cartesian.py` & `reflex-0.4.6a4/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/cartesian.pyi` & `reflex-0.4.6a4/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/charts.py` & `reflex-0.4.6a4/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/charts.pyi` & `reflex-0.4.6a4/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/general.py` & `reflex-0.4.6a4/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/general.pyi` & `reflex-0.4.6a4/reflex/components/recharts/general.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/polar.py` & `reflex-0.4.6a4/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/polar.pyi` & `reflex-0.4.6a4/reflex/components/recharts/polar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/recharts.py` & `reflex-0.4.6a4/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/recharts/recharts.pyi` & `reflex-0.4.6a4/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/suneditor/editor.py` & `reflex-0.4.6a4/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/suneditor/editor.pyi` & `reflex-0.4.6a4/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/tags/iter_tag.py` & `reflex-0.4.6a4/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/tags/tag.py` & `reflex-0.4.6a4/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/components/tags/tagless.py` & `reflex-0.4.6a4/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/config.py` & `reflex-0.4.6a4/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/config.pyi` & `reflex-0.4.6a4/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/__init__.py` & `reflex-0.4.6a4/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/base.py` & `reflex-0.4.6a4/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/colors.py` & `reflex-0.4.6a4/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/compiler.py` & `reflex-0.4.6a4/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/config.py` & `reflex-0.4.6a4/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/custom_components.py` & `reflex-0.4.6a4/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/event.py` & `reflex-0.4.6a4/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/installer.py` & `reflex-0.4.6a4/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/route.py` & `reflex-0.4.6a4/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/constants/style.py` & `reflex-0.4.6a4/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/custom_components/custom_components.py` & `reflex-0.4.6a4/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/event.py` & `reflex-0.4.6a4/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/middleware/hydrate_middleware.py` & `reflex-0.4.6a4/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/middleware/middleware.py` & `reflex-0.4.6a4/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/model.py` & `reflex-0.4.6a4/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/page.py` & `reflex-0.4.6a4/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/reflex.py` & `reflex-0.4.6a4/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/route.py` & `reflex-0.4.6a4/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/state.py` & `reflex-0.4.6a4/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/style.py` & `reflex-0.4.6a4/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/testing.py` & `reflex-0.4.6a4/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/build.py` & `reflex-0.4.6a4/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/console.py` & `reflex-0.4.6a4/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/exec.py` & `reflex-0.4.6a4/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/export.py` & `reflex-0.4.6a4/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/format.py` & `reflex-0.4.6a4/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/imports.py` & `reflex-0.4.6a4/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/path_ops.py` & `reflex-0.4.6a4/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/prerequisites.py` & `reflex-0.4.6a4/reflex/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/processes.py` & `reflex-0.4.6a4/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/pyi_generator.py` & `reflex-0.4.6a4/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/serializers.py` & `reflex-0.4.6a4/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/telemetry.py` & `reflex-0.4.6a4/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/types.py` & `reflex-0.4.6a4/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/utils/watch.py` & `reflex-0.4.6a4/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/vars.py` & `reflex-0.4.6a4/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/reflex/vars.pyi` & `reflex-0.4.6a4/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.6a3/PKG-INFO` & `reflex-0.4.6a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.4.6a3
+Version: 0.4.6a4
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

