# Comparing `tmp/django_smartbase_admin-0.2.3.tar.gz` & `tmp/django_smartbase_admin-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_smartbase_admin-0.2.3.tar", max compression
+gzip compressed data, was "django_smartbase_admin-0.2.4.tar", max compression
```

## Comparing `django_smartbase_admin-0.2.3.tar` & `django_smartbase_admin-0.2.4.tar`

### file list

```diff
@@ -1,630 +1,630 @@
--rw-r--r--   0        0        0     1078 2024-03-27 14:29:27.238664 django_smartbase_admin-0.2.3/LICENSE.md
--rw-r--r--   0        0        0       65 2024-03-27 14:29:27.238664 django_smartbase_admin-0.2.3/README.md
--rw-r--r--   0        0        0      536 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/actions/__init__.py
--rw-r--r--   0        0        0    12723 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/actions/admin_action_list.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/__init__.py
--rw-r--r--   0        0        0    31010 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/admin_base.py
--rw-r--r--   0        0        0     6783 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/site.py
--rw-r--r--   0        0        0    12119 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/widgets.py
--rw-r--r--   0        0        0      479 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/apps.py
--rw-r--r--   0        0        0      342 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/compilemessages.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/__init__.py
--rw-r--r--   0        0        0      658 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/actions.py
--rw-r--r--   0        0        0    21953 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_base_view.py
--rw-r--r--   0        0        0      624 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_entrypoint_view.py
--rw-r--r--   0        0        0     4238 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_view.py
--rw-r--r--   0        0        0     5985 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/configuration.py
--rw-r--r--   0        0        0     1942 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/const.py
--rw-r--r--   0        0        0    23660 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/dashboard.py
--rw-r--r--   0        0        0     4630 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/fake_inline.py
--rw-r--r--   0        0        0     8795 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/field.py
--rw-r--r--   0        0        0     1294 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/field_formatter.py
--rw-r--r--   0        0        0    18605 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/filter_widgets.py
--rw-r--r--   0        0        0      249 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/global_filter_form.py
--rw-r--r--   0        0        0     2936 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/menu_item.py
--rw-r--r--   0        0        0     2588 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/request.py
--rw-r--r--   0        0        0    14647 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15583 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      381 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/makemessages.py
--rw-r--r--   0        0        0     1154 2024-03-27 14:29:27.254664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0001_initial.py
--rw-r--r--   0        0        0      631 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py
--rw-r--r--   0        0        0      552 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py
--rw-r--r--   0        0        0      648 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/__init__.py
--rw-r--r--   0        0        0      743 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/models.py
--rw-r--r--   0        0        0      833 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py
--rw-r--r--   0        0        0      385 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/querysets.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/__init__.py
--rw-r--r--   0        0        0      712 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/configuration.py
--rw-r--r--   0        0        0      156 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/data.py
--rw-r--r--   0        0        0      642 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/thread_local.py
--rw-r--r--   0        0        0     5606 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/translations.py
--rw-r--r--   0        0        0     7338 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/views.py
--rw-r--r--   0        0        0     8911 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/xlsx_export.py
--rw-r--r--   0        0        0      610 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js
--rw-r--r--   0        0        0     2369 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js
--rw-r--r--   0        0        0     1015 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js
--rw-r--r--   0        0        0      342 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/screens.js
--rw-r--r--   0        0        0     1341 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js
--rw-r--r--   0        0        0      851 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js
--rw-r--r--   0        0        0      247 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/webpack.analyze.js
--rw-r--r--   0        0        0     2540 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js
--rw-r--r--   0        0        0      176 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/webpack.dev.js
--rw-r--r--   0        0        0      294 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/webpack.prod.js
--rw-r--r--   0        0        0     6037 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css
--rw-r--r--   0        0        0     1646 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css
--rw-r--r--   0        0        0   204560 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/chart.js
--rw-r--r--   0        0        0      257 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/chart.js.LICENSE.txt
--rw-r--r--   0        0        0   375193 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main.js
--rw-r--r--   0        0        0     5600 2024-03-27 14:29:27.258664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt
--rw-r--r--   0        0        0   145701 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main_style.css
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main_style.js
--rw-r--r--   0        0        0   457031 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/table.js
--rw-r--r--   0        0        0      125 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/table.js.LICENSE.txt
--rw-r--r--   0        0        0      567 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/translations.js
--rw-r--r--   0        0        0    18172 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0    50085 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     7398 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0      261 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/browserconfig.xml
--rw-r--r--   0        0        0     1213 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png
--rw-r--r--   0        0        0     2044 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico
--rw-r--r--   0        0        0     3716 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png
--rw-r--r--   0        0        0     3914 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png
--rw-r--r--   0        0        0     4332 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png
--rw-r--r--   0        0        0     8565 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png
--rw-r--r--   0        0        0     2781 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png
--rw-r--r--   0        0        0     4925 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg
--rw-r--r--   0        0        0      456 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/site.webmanifest
--rw-r--r--   0        0        0    56968 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2
--rw-r--r--   0        0        0    37924 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2
--rw-r--r--   0        0        0       43 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/blank.gif
--rw-r--r--   0        0        0      364 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ad.png
--rw-r--r--   0        0        0      333 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ae.png
--rw-r--r--   0        0        0      478 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/af.png
--rw-r--r--   0        0        0      827 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png
--rw-r--r--   0        0        0      843 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png
--rw-r--r--   0        0        0      614 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/al.png
--rw-r--r--   0        0        0      269 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/am.png
--rw-r--r--   0        0        0      503 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/an.png
--rw-r--r--   0        0        0      497 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ao.png
--rw-r--r--   0        0        0      383 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ar.png
--rw-r--r--   0        0        0      308 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/at.png
--rw-r--r--   0        0        0      877 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/au.png
--rw-r--r--   0        0        0      419 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/aw.png
--rw-r--r--   0        0        0      323 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ax.png
--rw-r--r--   0        0        0      367 2024-03-27 14:29:27.262664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/az.png
--rw-r--r--   0        0        0      600 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png
--rw-r--r--   0        0        0      509 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bb.png
--rw-r--r--   0        0        0      516 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png
--rw-r--r--   0        0        0      275 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/be.png
--rw-r--r--   0        0        0      437 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bf.png
--rw-r--r--   0        0        0      306 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bg.png
--rw-r--r--   0        0        0      393 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bh.png
--rw-r--r--   0        0        0      826 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png
--rw-r--r--   0        0        0      309 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bj.png
--rw-r--r--   0        0        0      870 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png
--rw-r--r--   0        0        0      709 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png
--rw-r--r--   0        0        0      275 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bo.png
--rw-r--r--   0        0        0      863 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/br.png
--rw-r--r--   0        0        0      618 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png
--rw-r--r--   0        0        0      365 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bt.png
--rw-r--r--   0        0        0      280 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bw.png
--rw-r--r--   0        0        0      362 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/by.png
--rw-r--r--   0        0        0      685 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png
--rw-r--r--   0        0        0      494 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ca.png
--rw-r--r--   0        0        0      616 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png
--rw-r--r--   0        0        0      793 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png
--rw-r--r--   0        0        0     1067 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png
--rw-r--r--   0        0        0      783 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png
--rw-r--r--   0        0        0      569 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png
--rw-r--r--   0        0        0      665 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png
--rw-r--r--   0        0        0      313 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ch.png
--rw-r--r--   0        0        0      326 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ci.png
--rw-r--r--   0        0        0      454 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cl.png
--rw-r--r--   0        0        0      446 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cm.png
--rw-r--r--   0        0        0      585 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png
--rw-r--r--   0        0        0      721 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png
--rw-r--r--   0        0        0      276 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/co.png
--rw-r--r--   0        0        0      914 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png
--rw-r--r--   0        0        0      309 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cr.png
--rw-r--r--   0        0        0      463 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cs.png
--rw-r--r--   0        0        0      567 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png
--rw-r--r--   0        0        0      599 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png
--rw-r--r--   0        0        0      594 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png
--rw-r--r--   0        0        0      688 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png
--rw-r--r--   0        0        0      463 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cz.png
--rw-r--r--   0        0        0      278 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/de.png
--rw-r--r--   0        0        0      583 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png
--rw-r--r--   0        0        0      327 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dk.png
--rw-r--r--   0        0        0      677 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png
--rw-r--r--   0        0        0      446 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/do.png
--rw-r--r--   0        0        0      738 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png
--rw-r--r--   0        0        0      491 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ec.png
--rw-r--r--   0        0        0      314 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ee.png
--rw-r--r--   0        0        0      427 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/eg.png
--rw-r--r--   0        0        0     1025 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/en.png
--rw-r--r--   0        0        0      821 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/er.png
--rw-r--r--   0        0        0      473 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/es.png
--rw-r--r--   0        0        0      579 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/et.png
--rw-r--r--   0        0        0      582 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png
--rw-r--r--   0        0        0      326 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fi.png
--rw-r--r--   0        0        0      900 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png
--rw-r--r--   0        0        0      949 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png
--rw-r--r--   0        0        0      599 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png
--rw-r--r--   0        0        0      330 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fr.png
--rw-r--r--   0        0        0      273 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ga.png
--rw-r--r--   0        0        0     1025 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png
--rw-r--r--   0        0        0      806 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png
--rw-r--r--   0        0        0      397 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ge.png
--rw-r--r--   0        0        0      539 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png
--rw-r--r--   0        0        0      393 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gh.png
--rw-r--r--   0        0        0      472 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gi.png
--rw-r--r--   0        0        0      279 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gm.png
--rw-r--r--   0        0        0      278 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gn.png
--rw-r--r--   0        0        0      574 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png
--rw-r--r--   0        0        0      453 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gr.png
--rw-r--r--   0        0        0      491 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gt.png
--rw-r--r--   0        0        0      453 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gw.png
--rw-r--r--   0        0        0      677 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png
--rw-r--r--   0        0        0      657 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png
--rw-r--r--   0        0        0      419 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hn.png
--rw-r--r--   0        0        0      638 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png
--rw-r--r--   0        0        0      568 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png
--rw-r--r--   0        0        0      308 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hu.png
--rw-r--r--   0        0        0      295 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/id.png
--rw-r--r--   0        0        0      328 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ie.png
--rw-r--r--   0        0        0      527 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/il.png
--rw-r--r--   0        0        0      642 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/im.png
--rw-r--r--   0        0        0      375 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/in.png
--rw-r--r--   0        0        0      428 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/iq.png
--rw-r--r--   0        0        0      553 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png
--rw-r--r--   0        0        0      328 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/is.png
--rw-r--r--   0        0        0      329 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/it.png
--rw-r--r--   0        0        0     1133 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/je.png
--rw-r--r--   0        0        0      779 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png
--rw-r--r--   0        0        0      602 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png
--rw-r--r--   0        0        0      614 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png
--rw-r--r--   0        0        0      573 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png
--rw-r--r--   0        0        0      725 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png
--rw-r--r--   0        0        0      459 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kh.png
--rw-r--r--   0        0        0      729 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/km.png
--rw-r--r--   0        0        0     1020 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png
--rw-r--r--   0        0        0      512 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png
--rw-r--r--   0        0        0      845 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png
--rw-r--r--   0        0        0      474 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kw.png
--rw-r--r--   0        0        0      931 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png
--rw-r--r--   0        0        0      883 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png
--rw-r--r--   0        0        0      411 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/la.png
--rw-r--r--   0        0        0      442 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lb.png
--rw-r--r--   0        0        0      542 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png
--rw-r--r--   0        0        0      263 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/li.png
--rw-r--r--   0        0        0      799 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png
--rw-r--r--   0        0        0      659 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png
--rw-r--r--   0        0        0      401 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ls.png
--rw-r--r--   0        0        0      274 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lt.png
--rw-r--r--   0        0        0      314 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lu.png
--rw-r--r--   0        0        0      285 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lv.png
--rw-r--r--   0        0        0      352 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ly.png
--rw-r--r--   0        0        0      513 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png
--rw-r--r--   0        0        0      295 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mc.png
--rw-r--r--   0        0        0      375 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/md.png
--rw-r--r--   0        0        0      810 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/me.png
--rw-r--r--   0        0        0      334 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mg.png
--rw-r--r--   0        0        0     1071 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png
--rw-r--r--   0        0        0      277 2024-03-27 14:29:27.266664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ml.png
--rw-r--r--   0        0        0      548 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png
--rw-r--r--   0        0        0      390 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mn.png
--rw-r--r--   0        0        0      620 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png
--rw-r--r--   0        0        0      579 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png
--rw-r--r--   0        0        0      900 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png
--rw-r--r--   0        0        0      438 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mt.png
--rw-r--r--   0        0        0      279 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mu.png
--rw-r--r--   0        0        0      506 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mv.png
--rw-r--r--   0        0        0      389 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mw.png
--rw-r--r--   0        0        0      523 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png
--rw-r--r--   0        0        0      686 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/my.png
--rw-r--r--   0        0        0      590 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png
--rw-r--r--   0        0        0      897 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/na.png
--rw-r--r--   0        0        0      380 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ne.png
--rw-r--r--   0        0        0      317 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ng.png
--rw-r--r--   0        0        0      405 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ni.png
--rw-r--r--   0        0        0      307 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/nl.png
--rw-r--r--   0        0        0      402 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/no.png
--rw-r--r--   0        0        0      866 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/np.png
--rw-r--r--   0        0        0      784 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png
--rw-r--r--   0        0        0      473 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/om.png
--rw-r--r--   0        0        0      604 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png
--rw-r--r--   0        0        0      319 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pe.png
--rw-r--r--   0        0        0      534 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png
--rw-r--r--   0        0        0      754 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png
--rw-r--r--   0        0        0      629 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png
--rw-r--r--   0        0        0      682 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png
--rw-r--r--   0        0        0      290 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pl.png
--rw-r--r--   0        0        0      678 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png
--rw-r--r--   0        0        0      545 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png
--rw-r--r--   0        0        0      508 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pw.png
--rw-r--r--   0        0        0      371 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/py.png
--rw-r--r--   0        0        0      392 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/qa.png
--rw-r--r--   0        0        0      273 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ro.png
--rw-r--r--   0        0        0      525 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png
--rw-r--r--   0        0        0      306 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ru.png
--rw-r--r--   0        0        0      385 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/rw.png
--rw-r--r--   0        0        0      676 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png
--rw-r--r--   0        0        0     1126 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png
--rw-r--r--   0        0        0      974 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png
--rw-r--r--   0        0        0      523 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png
--rw-r--r--   0        0        0      284 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/se.png
--rw-r--r--   0        0        0      592 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png
--rw-r--r--   0        0        0     1253 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png
--rw-r--r--   0        0        0      430 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/si.png
--rw-r--r--   0        0        0      772 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png
--rw-r--r--   0        0        0      308 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sl.png
--rw-r--r--   0        0        0      503 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sm.png
--rw-r--r--   0        0        0      404 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sn.png
--rw-r--r--   0        0        0      506 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/so.png
--rw-r--r--   0        0        0      446 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sr.png
--rw-r--r--   0        0        0      650 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/st.png
--rw-r--r--   0        0        0      438 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sv.png
--rw-r--r--   0        0        0      495 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sy.png
--rw-r--r--   0        0        0      535 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png
--rw-r--r--   0        0        0      919 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png
--rw-r--r--   0        0        0      274 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/td.png
--rw-r--r--   0        0        0      481 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tg.png
--rw-r--r--   0        0        0      307 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/th.png
--rw-r--r--   0        0        0      399 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tj.png
--rw-r--r--   0        0        0      739 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png
--rw-r--r--   0        0        0      786 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png
--rw-r--r--   0        0        0      678 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png
--rw-r--r--   0        0        0      522 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/to.png
--rw-r--r--   0        0        0      649 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png
--rw-r--r--   0        0        0     1025 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png
--rw-r--r--   0        0        0      423 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tw.png
--rw-r--r--   0        0        0      767 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png
--rw-r--r--   0        0        0      260 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ua.png
--rw-r--r--   0        0        0      598 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png
--rw-r--r--   0        0        0      627 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/us.png
--rw-r--r--   0        0        0      588 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png
--rw-r--r--   0        0        0      494 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/uz.png
--rw-r--r--   0        0        0      485 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vc.png
--rw-r--r--   0        0        0      364 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ve.png
--rw-r--r--   0        0        0      997 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png
--rw-r--r--   0        0        0      503 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vn.png
--rw-r--r--   0        0        0      666 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png
--rw-r--r--   0        0        0      428 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ws.png
--rw-r--r--   0        0        0      744 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png
--rw-r--r--   0        0        0      308 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ye.png
--rw-r--r--   0        0        0      802 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/za.png
--rw-r--r--   0        0        0      501 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/zm.png
--rw-r--r--   0        0        0      620 2024-03-27 14:29:27.270664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png
--rw-r--r--   0        0        0  1664449 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/login.jpg
--rw-r--r--   0        0        0    92962 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/login.webp
--rw-r--r--   0        0        0     6363 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/logo.svg
--rw-r--r--   0        0        0     2354 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/sk.svg
--rw-r--r--   0        0        0   170535 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js
--rw-r--r--   0        0        0     4819 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js
--rw-r--r--   0        0        0     1323 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js
--rw-r--r--   0        0        0    39433 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js
--rw-r--r--   0        0        0    87461 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js
--rw-r--r--   0        0        0     3063 2024-03-27 14:29:27.274664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js
--rw-r--r--   0        0        0     7770 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js
--rw-r--r--   0        0        0     1698 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js
--rw-r--r--   0        0        0     1914 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/prices.js
--rw-r--r--   0        0        0      932 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/remove-me.js
--rw-r--r--   0        0        0   387673 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js
--rw-r--r--   0        0        0      527 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg
--rw-r--r--   0        0        0      682 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg
--rw-r--r--   0        0        0      386 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-one.svg
--rw-r--r--   0        0        0      826 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg
--rw-r--r--   0        0        0      444 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-three.svg
--rw-r--r--   0        0        0      477 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Aiming.svg
--rw-r--r--   0        0        0      677 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg
--rw-r--r--   0        0        0      732 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg
--rw-r--r--   0        0        0      734 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg
--rw-r--r--   0        0        0     1138 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg
--rw-r--r--   0        0        0     1238 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg
--rw-r--r--   0        0        0     1209 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg
--rw-r--r--   0        0        0      509 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-down.svg
--rw-r--r--   0        0        0      522 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg
--rw-r--r--   0        0        0      524 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg
--rw-r--r--   0        0        0      511 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-up.svg
--rw-r--r--   0        0        0      737 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg
--rw-r--r--   0        0        0      988 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg
--rw-r--r--   0        0        0      538 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg
--rw-r--r--   0        0        0      524 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg
--rw-r--r--   0        0        0      304 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card.svg
--rw-r--r--   0        0        0      622 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg
--rw-r--r--   0        0        0      532 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg
--rw-r--r--   0        0        0      824 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg
--rw-r--r--   0        0        0      540 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg
--rw-r--r--   0        0        0      583 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg
--rw-r--r--   0        0        0      979 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg
--rw-r--r--   0        0        0      281 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-small.svg
--rw-r--r--   0        0        0      280 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check.svg
--rw-r--r--   0        0        0      544 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg
--rw-r--r--   0        0        0      318 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-small.svg
--rw-r--r--   0        0        0      318 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close.svg
--rw-r--r--   0        0        0      429 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Column.svg
--rw-r--r--   0        0        0      361 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-left.svg
--rw-r--r--   0        0        0      347 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-right.svg
--rw-r--r--   0        0        0     1231 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg
--rw-r--r--   0        0        0     2040 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg
--rw-r--r--   0        0        0      611 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg
--rw-r--r--   0        0        0      454 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete.svg
--rw-r--r--   0        0        0      439 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-down.svg
--rw-r--r--   0        0        0      433 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-left.svg
--rw-r--r--   0        0        0      430 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-right.svg
--rw-r--r--   0        0        0      439 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-up.svg
--rw-r--r--   0        0        0      504 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-c.svg
--rw-r--r--   0        0        0      296 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-small.svg
--rw-r--r--   0        0        0      280 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down.svg
--rw-r--r--   0        0        0      984 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg
--rw-r--r--   0        0        0      386 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download.svg
--rw-r--r--   0        0        0      898 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg
--rw-r--r--   0        0        0      529 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg
--rw-r--r--   0        0        0      442 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Excel-one.svg
--rw-r--r--   0        0        0      636 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg
--rw-r--r--   0        0        0     1432 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg
--rw-r--r--   0        0        0      683 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg
--rw-r--r--   0        0        0      575 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg
--rw-r--r--   0        0        0      527 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg
--rw-r--r--   0        0        0      570 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg
--rw-r--r--   0        0        0      264 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Hamburger-button.svg
--rw-r--r--   0        0        0      653 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg
--rw-r--r--   0        0        0     1300 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg
--rw-r--r--   0        0        0      536 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg
--rw-r--r--   0        0        0      756 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg
--rw-r--r--   0        0        0     1039 2024-03-27 14:29:27.278664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg
--rw-r--r--   0        0        0      501 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-c.svg
--rw-r--r--   0        0        0      247 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-down.svg
--rw-r--r--   0        0        0      235 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-up.svg
--rw-r--r--   0        0        0      301 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small.svg
--rw-r--r--   0        0        0      272 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left.svg
--rw-r--r--   0        0        0      852 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg
--rw-r--r--   0        0        0      856 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg
--rw-r--r--   0        0        0      714 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg
--rw-r--r--   0        0        0      566 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg
--rw-r--r--   0        0        0      403 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lock.svg
--rw-r--r--   0        0        0      381 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Login.svg
--rw-r--r--   0        0        0      376 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Logout.svg
--rw-r--r--   0        0        0      887 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg
--rw-r--r--   0        0        0      574 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg
--rw-r--r--   0        0        0      666 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg
--rw-r--r--   0        0        0      647 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg
--rw-r--r--   0        0        0      418 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail.svg
--rw-r--r--   0        0        0     1757 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg
--rw-r--r--   0        0        0      555 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg
--rw-r--r--   0        0        0      487 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus-the-top.svg
--rw-r--r--   0        0        0      148 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus.svg
--rw-r--r--   0        0        0      541 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg
--rw-r--r--   0        0        0      810 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg
--rw-r--r--   0        0        0      771 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg
--rw-r--r--   0        0        0      547 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg
--rw-r--r--   0        0        0     1528 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg
--rw-r--r--   0        0        0      638 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg
--rw-r--r--   0        0        0      874 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg
--rw-r--r--   0        0        0      656 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg
--rw-r--r--   0        0        0      940 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg
--rw-r--r--   0        0        0      891 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg
--rw-r--r--   0        0        0     1485 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg
--rw-r--r--   0        0        0      242 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Plus.svg
--rw-r--r--   0        0        0     2587 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg
--rw-r--r--   0        0        0      938 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg
--rw-r--r--   0        0        0     2362 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg
--rw-r--r--   0        0        0      745 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg
--rw-r--r--   0        0        0      362 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Reduce-one.svg
--rw-r--r--   0        0        0      899 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg
--rw-r--r--   0        0        0      507 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Return.svg
--rw-r--r--   0        0        0      299 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora Filled.svg
--rw-r--r--   0        0        0      504 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora.svg
--rw-r--r--   0        0        0      501 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-c.svg
--rw-r--r--   0        0        0      280 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-down.svg
--rw-r--r--   0        0        0      243 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-up.svg
--rw-r--r--   0        0        0      294 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small.svg
--rw-r--r--   0        0        0      272 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right.svg
--rw-r--r--   0        0        0      687 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg
--rw-r--r--   0        0        0      461 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Search.svg
--rw-r--r--   0        0        0      534 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg
--rw-r--r--   0        0        0      328 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-config.svg
--rw-r--r--   0        0        0     2761 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg
--rw-r--r--   0        0        0     1380 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg
--rw-r--r--   0        0        0     2218 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg
--rw-r--r--   0        0        0      812 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg
--rw-r--r--   0        0        0      940 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg
--rw-r--r--   0        0        0      497 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort Alt.svg
--rw-r--r--   0        0        0      311 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-down.svg
--rw-r--r--   0        0        0      334 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-up.svg
--rw-r--r--   0        0        0      360 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-one.svg
--rw-r--r--   0        0        0      479 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-three.svg
--rw-r--r--   0        0        0      809 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg
--rw-r--r--   0        0        0     1175 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg
--rw-r--r--   0        0        0     1876 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg
--rw-r--r--   0        0        0      323 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Switch.svg
--rw-r--r--   0        0        0      525 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg
--rw-r--r--   0        0        0      806 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg
--rw-r--r--   0        0        0      485 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag.svg
--rw-r--r--   0        0        0      490 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tips-one.svg
--rw-r--r--   0        0        0      312 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/To-top.svg
--rw-r--r--   0        0        0      476 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Transfer-data.svg
--rw-r--r--   0        0        0     2485 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg
--rw-r--r--   0        0        0     1003 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg
--rw-r--r--   0        0        0      860 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg
--rw-r--r--   0        0        0     1074 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg
--rw-r--r--   0        0        0      592 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg
--rw-r--r--   0        0        0      393 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Unlock.svg
--rw-r--r--   0        0        0      504 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-c.svg
--rw-r--r--   0        0        0      299 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-small.svg
--rw-r--r--   0        0        0      279 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up.svg
--rw-r--r--   0        0        0      988 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg
--rw-r--r--   0        0        0      385 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload.svg
--rw-r--r--   0        0        0      777 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg
--rw-r--r--   0        0        0      888 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg
--rw-r--r--   0        0        0      680 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg
--rw-r--r--   0        0        0      584 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg
--rw-r--r--   0        0        0      490 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-out.svg
--rw-r--r--   0        0        0     1840 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_base.css
--rw-r--r--   0        0        0     1889 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css
--rw-r--r--   0        0        0     2825 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css
--rw-r--r--   0        0        0    12213 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_components.css
--rw-r--r--   0        0        0    14025 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css
--rw-r--r--   0        0        0     4096 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css
--rw-r--r--   0        0        0     5587 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css
--rw-r--r--   0        0        0    18294 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css
--rw-r--r--   0        0        0       58 2024-03-27 14:29:27.282664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_tailwind_base.css
--rw-r--r--   0        0        0      901 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css
--rw-r--r--   0        0        0     4665 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css
--rw-r--r--   0        0        0     1763 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css
--rw-r--r--   0        0        0    10276 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css
--rw-r--r--   0        0        0     4316 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css
--rw-r--r--   0        0        0      719 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css
--rw-r--r--   0        0        0    10087 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css
--rw-r--r--   0        0        0     2388 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css
--rw-r--r--   0        0        0     2485 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css
--rw-r--r--   0        0        0      361 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/style.css
--rw-r--r--   0        0        0    12215 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js
--rw-r--r--   0        0        0     4736 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/chart.js
--rw-r--r--   0        0        0     4615 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/choices.js
--rw-r--r--   0        0        0      486 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/code.js
--rw-r--r--   0        0        0    14259 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js
--rw-r--r--   0        0        0     9131 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/main.js
--rw-r--r--   0        0        0     3354 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js
--rw-r--r--   0        0        0     1733 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/range.js
--rw-r--r--   0        0        0     1570 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js
--rw-r--r--   0        0        0     1186 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js
--rw-r--r--   0        0        0     9952 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table.js
--rw-r--r--   0        0        0      507 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/base_module.js
--rw-r--r--   0        0        0    10561 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js
--rw-r--r--   0        0        0      929 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js
--rw-r--r--   0        0        0      686 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js
--rw-r--r--   0        0        0     4016 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js
--rw-r--r--   0        0        0     7694 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js
--rw-r--r--   0        0        0     6403 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js
--rw-r--r--   0        0        0    11157 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js
--rw-r--r--   0        0        0     2383 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js
--rw-r--r--   0        0        0      954 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/translations.js
--rw-r--r--   0        0        0     4245 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/utils.js
--rw-r--r--   0        0        0    10987 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html
--rw-r--r--   0        0        0     3200 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html
--rw-r--r--   0        0        0      272 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/dashboard.html
--rw-r--r--   0        0        0     3205 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html
--rw-r--r--   0        0        0     2248 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html
--rw-r--r--   0        0        0     9442 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/list.html
--rw-r--r--   0        0        0      122 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/media.html
--rw-r--r--   0        0        0     1905 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html
--rw-r--r--   0        0        0      109 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/partials/open_modal_attrs.html
--rw-r--r--   0        0        0      857 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html
--rw-r--r--   0        0        0     4542 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html
--rw-r--r--   0        0        0      587 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html
--rw-r--r--   0        0        0      334 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations-list.html
--rw-r--r--   0        0        0     1285 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations.html
--rw-r--r--   0        0        0       50 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/auth/user/add_form.html
--rw-r--r--   0        0        0     2398 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/login.html
--rw-r--r--   0        0        0      864 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html
--rw-r--r--   0        0        0      496 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/logout.html
--rw-r--r--   0        0        0      485 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_done.html
--rw-r--r--   0        0        0     1905 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html
--rw-r--r--   0        0        0      503 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_complete.html
--rw-r--r--   0        0        0     1310 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html
--rw-r--r--   0        0        0      666 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html
--rw-r--r--   0        0        0      621 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html
--rw-r--r--   0        0        0     1397 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html
--rw-r--r--   0        0        0       76 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/blank_base.html
--rw-r--r--   0        0        0     1982 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/buttons.html
--rw-r--r--   0        0        0      959 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/columns.html
--rw-r--r--   0        0        0     2654 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/filters.html
--rw-r--r--   0        0        0    10938 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/inputs.html
--rw-r--r--   0        0        0     4543 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/config/view.html
--rw-r--r--   0        0        0      900 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html
--rw-r--r--   0        0        0     1096 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html
--rw-r--r--   0        0        0      141 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/list_widget.html
--rw-r--r--   0        0        0      720 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html
--rw-r--r--   0        0        0     1071 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html
--rw-r--r--   0        0        0      548 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html
--rw-r--r--   0        0        0      645 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html
--rw-r--r--   0        0        0      648 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html
--rw-r--r--   0        0        0     1243 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html
--rw-r--r--   0        0        0     1162 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html
--rw-r--r--   0        0        0      614 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html
--rw-r--r--   0        0        0     1212 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html
--rw-r--r--   0        0        0      548 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html
--rw-r--r--   0        0        0     1121 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/fonts.html
--rw-r--r--   0        0        0      165 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/attrs.html
--rw-r--r--   0        0        0      172 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/change_form_title.html
--rw-r--r--   0        0        0    18710 2024-03-27 14:29:27.286664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/components.html
--rw-r--r--   0        0        0      229 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/fieldset.html
--rw-r--r--   0        0        0     2227 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html
--rw-r--r--   0        0        0      287 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/loading.html
--rw-r--r--   0        0        0      304 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/loading_absolute.html
--rw-r--r--   0        0        0      771 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html
--rw-r--r--   0        0        0     7592 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html
--rw-r--r--   0        0        0    15127 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html
--rw-r--r--   0        0        0     3046 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html
--rw-r--r--   0        0        0    18190 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html
--rw-r--r--   0        0        0      308 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/cms/translations_status_row.html
--rw-r--r--   0        0        0     3002 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html
--rw-r--r--   0        0        0    18834 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html
--rw-r--r--   0        0        0     1909 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html
--rw-r--r--   0        0        0    15189 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html
--rw-r--r--   0        0        0     9195 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/navigation.html
--rw-r--r--   0        0        0      825 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html
--rw-r--r--   0        0        0      121 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_close.html
--rw-r--r--   0        0        0      276 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_error.html
--rw-r--r--   0        0        0      268 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_info.html
--rw-r--r--   0        0        0      323 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_success.html
--rw-r--r--   0        0        0      323 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_warning.html
--rw-r--r--   0        0        0     1507 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html
--rw-r--r--   0        0        0      505 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sb_admin_base.html
--rw-r--r--   0        0        0     3253 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html
--rw-r--r--   0        0        0      817 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html
--rw-r--r--   0        0        0    59910 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg
--rw-r--r--   0        0        0     3254 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/submit_line.html
--rw-r--r--   0        0        0      577 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html
--rw-r--r--   0        0        0     2815 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/array.html
--rw-r--r--   0        0        0      172 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/attrs.html
--rw-r--r--   0        0        0     2434 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html
--rw-r--r--   0        0        0      232 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox.html
--rw-r--r--   0        0        0       51 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_option.html
--rw-r--r--   0        0        0     1578 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html
--rw-r--r--   0        0        0      542 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html
--rw-r--r--   0        0        0     2340 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html
--rw-r--r--   0        0        0      345 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/code.html
--rw-r--r--   0        0        0      160 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/date.html
--rw-r--r--   0        0        0       44 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/datetime.html
--rw-r--r--   0        0        0       43 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/email.html
--rw-r--r--   0        0        0       44 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/file.html
--rw-r--r--   0        0        0       44 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/hidden.html
--rw-r--r--   0        0        0      148 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/includes/field_label.html
--rw-r--r--   0        0        0      148 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/includes/help_text.html
--rw-r--r--   0        0        0      443 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/includes/simple_field_label.html
--rw-r--r--   0        0        0      185 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/input.html
--rw-r--r--   0        0        0      209 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/input_option.html
--rw-r--r--   0        0        0       50 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/multiple_hidden.html
--rw-r--r--   0        0        0      329 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/multiwidget.html
--rw-r--r--   0        0        0      159 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/number.html
--rw-r--r--   0        0        0      585 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/password.html
--rw-r--r--   0        0        0      363 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/radio.html
--rw-r--r--   0        0        0       51 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/radio_option.html
--rw-r--r--   0        0        0      216 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/read_only_password_hash.html
--rw-r--r--   0        0        0      496 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/select.html
--rw-r--r--   0        0        0       50 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/select_date.html
--rw-r--r--   0        0        0      123 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/select_option.html
--rw-r--r--   0        0        0       50 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/splitdatetime.html
--rw-r--r--   0        0        0       50 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/splithiddendatetime.html
--rw-r--r--   0        0        0      160 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/text.html
--rw-r--r--   0        0        0      257 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/textarea.html
--rw-r--r--   0        0        0      160 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/time.html
--rw-r--r--   0        0        0      280 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/toggle.html
--rw-r--r--   0        0        0      160 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/url.html
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templatetags/__init__.py
--rw-r--r--   0        0        0     1520 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templatetags/base.py
--rw-r--r--   0        0        0     4125 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/templatetags/sb_admin_tags.py
--rw-r--r--   0        0        0       17 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/urls.py
--rw-r--r--   0        0        0     1343 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/utils.py
--rw-r--r--   0        0        0        0 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/__init__.py
--rw-r--r--   0        0        0     1495 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/dashboard_view.py
--rw-r--r--   0        0        0      954 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/global_filter_view.py
--rw-r--r--   0        0        0      292 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/media_view.py
--rw-r--r--   0        0        0    20254 2024-03-27 14:29:27.290664 django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/translations_view.py
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 django_smartbase_admin-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-02 09:54:00.455182 django_smartbase_admin-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0       65 2024-04-02 09:54:00.455182 django_smartbase_admin-0.2.4/README.md
+-rw-r--r--   0        0        0      536 2024-04-02 09:54:00.471182 django_smartbase_admin-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.471182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.471182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/actions/__init__.py
+-rw-r--r--   0        0        0    12723 2024-04-02 09:54:00.471182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/actions/admin_action_list.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.471182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/__init__.py
+-rw-r--r--   0        0        0    31113 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/admin_base.py
+-rw-r--r--   0        0        0     6783 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/site.py
+-rw-r--r--   0        0        0    12138 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/widgets.py
+-rw-r--r--   0        0        0      479 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/apps.py
+-rw-r--r--   0        0        0      342 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/compilemessages.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/__init__.py
+-rw-r--r--   0        0        0      658 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/actions.py
+-rw-r--r--   0        0        0    21953 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_base_view.py
+-rw-r--r--   0        0        0      624 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_entrypoint_view.py
+-rw-r--r--   0        0        0     4238 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_view.py
+-rw-r--r--   0        0        0     5985 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/configuration.py
+-rw-r--r--   0        0        0     1942 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/const.py
+-rw-r--r--   0        0        0    23660 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/dashboard.py
+-rw-r--r--   0        0        0     4630 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/fake_inline.py
+-rw-r--r--   0        0        0     8795 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/field.py
+-rw-r--r--   0        0        0     1294 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/field_formatter.py
+-rw-r--r--   0        0        0    18605 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/filter_widgets.py
+-rw-r--r--   0        0        0      249 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/global_filter_form.py
+-rw-r--r--   0        0        0     2936 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/menu_item.py
+-rw-r--r--   0        0        0     2588 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/request.py
+-rw-r--r--   0        0        0    14647 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15583 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      381 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/makemessages.py
+-rw-r--r--   0        0        0     1154 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0001_initial.py
+-rw-r--r--   0        0        0      631 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py
+-rw-r--r--   0        0        0      552 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py
+-rw-r--r--   0        0        0      648 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/models.py
+-rw-r--r--   0        0        0      833 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py
+-rw-r--r--   0        0        0      385 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/querysets.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/configuration.py
+-rw-r--r--   0        0        0      156 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/data.py
+-rw-r--r--   0        0        0      642 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/thread_local.py
+-rw-r--r--   0        0        0     5606 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/translations.py
+-rw-r--r--   0        0        0     7338 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/views.py
+-rw-r--r--   0        0        0     8911 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/xlsx_export.py
+-rw-r--r--   0        0        0      610 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js
+-rw-r--r--   0        0        0     2369 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js
+-rw-r--r--   0        0        0     1015 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js
+-rw-r--r--   0        0        0      342 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/screens.js
+-rw-r--r--   0        0        0     1341 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js
+-rw-r--r--   0        0        0      851 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js
+-rw-r--r--   0        0        0      247 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/webpack.analyze.js
+-rw-r--r--   0        0        0     2540 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js
+-rw-r--r--   0        0        0      176 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/webpack.dev.js
+-rw-r--r--   0        0        0      294 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/webpack.prod.js
+-rw-r--r--   0        0        0     6037 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css
+-rw-r--r--   0        0        0     1646 2024-04-02 09:54:00.475182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css
+-rw-r--r--   0        0        0   204560 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/chart.js
+-rw-r--r--   0        0        0      257 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/chart.js.LICENSE.txt
+-rw-r--r--   0        0        0   375193 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main.js
+-rw-r--r--   0        0        0     5600 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt
+-rw-r--r--   0        0        0   145701 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main_style.css
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.479182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main_style.js
+-rw-r--r--   0        0        0   457031 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/table.js
+-rw-r--r--   0        0        0      125 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/table.js.LICENSE.txt
+-rw-r--r--   0        0        0      567 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/translations.js
+-rw-r--r--   0        0        0    18172 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0    50085 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7398 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0      261 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/browserconfig.xml
+-rw-r--r--   0        0        0     1213 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png
+-rw-r--r--   0        0        0     2044 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico
+-rw-r--r--   0        0        0     3716 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png
+-rw-r--r--   0        0        0     3914 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png
+-rw-r--r--   0        0        0     4332 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png
+-rw-r--r--   0        0        0     8565 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png
+-rw-r--r--   0        0        0     2781 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png
+-rw-r--r--   0        0        0     4925 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      456 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/site.webmanifest
+-rw-r--r--   0        0        0    56968 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2
+-rw-r--r--   0        0        0    37924 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2
+-rw-r--r--   0        0        0       43 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/blank.gif
+-rw-r--r--   0        0        0      364 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ad.png
+-rw-r--r--   0        0        0      333 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ae.png
+-rw-r--r--   0        0        0      478 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/af.png
+-rw-r--r--   0        0        0      827 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png
+-rw-r--r--   0        0        0      843 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png
+-rw-r--r--   0        0        0      614 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/al.png
+-rw-r--r--   0        0        0      269 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/am.png
+-rw-r--r--   0        0        0      503 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/an.png
+-rw-r--r--   0        0        0      497 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ao.png
+-rw-r--r--   0        0        0      383 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ar.png
+-rw-r--r--   0        0        0      308 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/at.png
+-rw-r--r--   0        0        0      877 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/au.png
+-rw-r--r--   0        0        0      419 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/aw.png
+-rw-r--r--   0        0        0      323 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ax.png
+-rw-r--r--   0        0        0      367 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/az.png
+-rw-r--r--   0        0        0      600 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png
+-rw-r--r--   0        0        0      509 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bb.png
+-rw-r--r--   0        0        0      516 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png
+-rw-r--r--   0        0        0      275 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/be.png
+-rw-r--r--   0        0        0      437 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bf.png
+-rw-r--r--   0        0        0      306 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bg.png
+-rw-r--r--   0        0        0      393 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bh.png
+-rw-r--r--   0        0        0      826 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png
+-rw-r--r--   0        0        0      309 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bj.png
+-rw-r--r--   0        0        0      870 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png
+-rw-r--r--   0        0        0      709 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png
+-rw-r--r--   0        0        0      275 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bo.png
+-rw-r--r--   0        0        0      863 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/br.png
+-rw-r--r--   0        0        0      618 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png
+-rw-r--r--   0        0        0      365 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bt.png
+-rw-r--r--   0        0        0      280 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bw.png
+-rw-r--r--   0        0        0      362 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/by.png
+-rw-r--r--   0        0        0      685 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png
+-rw-r--r--   0        0        0      494 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ca.png
+-rw-r--r--   0        0        0      616 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png
+-rw-r--r--   0        0        0      793 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png
+-rw-r--r--   0        0        0     1067 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png
+-rw-r--r--   0        0        0      783 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png
+-rw-r--r--   0        0        0      569 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png
+-rw-r--r--   0        0        0      665 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png
+-rw-r--r--   0        0        0      313 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ch.png
+-rw-r--r--   0        0        0      326 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ci.png
+-rw-r--r--   0        0        0      454 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cl.png
+-rw-r--r--   0        0        0      446 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cm.png
+-rw-r--r--   0        0        0      585 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png
+-rw-r--r--   0        0        0      721 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png
+-rw-r--r--   0        0        0      276 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/co.png
+-rw-r--r--   0        0        0      914 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png
+-rw-r--r--   0        0        0      309 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cr.png
+-rw-r--r--   0        0        0      463 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cs.png
+-rw-r--r--   0        0        0      567 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png
+-rw-r--r--   0        0        0      599 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png
+-rw-r--r--   0        0        0      594 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png
+-rw-r--r--   0        0        0      688 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png
+-rw-r--r--   0        0        0      463 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cz.png
+-rw-r--r--   0        0        0      278 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/de.png
+-rw-r--r--   0        0        0      583 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png
+-rw-r--r--   0        0        0      327 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dk.png
+-rw-r--r--   0        0        0      677 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png
+-rw-r--r--   0        0        0      446 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/do.png
+-rw-r--r--   0        0        0      738 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png
+-rw-r--r--   0        0        0      491 2024-04-02 09:54:00.483182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ec.png
+-rw-r--r--   0        0        0      314 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ee.png
+-rw-r--r--   0        0        0      427 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/eg.png
+-rw-r--r--   0        0        0     1025 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/en.png
+-rw-r--r--   0        0        0      821 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/er.png
+-rw-r--r--   0        0        0      473 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/es.png
+-rw-r--r--   0        0        0      579 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/et.png
+-rw-r--r--   0        0        0      582 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png
+-rw-r--r--   0        0        0      326 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fi.png
+-rw-r--r--   0        0        0      900 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png
+-rw-r--r--   0        0        0      949 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png
+-rw-r--r--   0        0        0      599 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png
+-rw-r--r--   0        0        0      330 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fr.png
+-rw-r--r--   0        0        0      273 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ga.png
+-rw-r--r--   0        0        0     1025 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png
+-rw-r--r--   0        0        0      806 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png
+-rw-r--r--   0        0        0      397 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ge.png
+-rw-r--r--   0        0        0      539 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png
+-rw-r--r--   0        0        0      393 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gh.png
+-rw-r--r--   0        0        0      472 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gi.png
+-rw-r--r--   0        0        0      279 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gm.png
+-rw-r--r--   0        0        0      278 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gn.png
+-rw-r--r--   0        0        0      574 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png
+-rw-r--r--   0        0        0      453 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gr.png
+-rw-r--r--   0        0        0      491 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gt.png
+-rw-r--r--   0        0        0      453 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gw.png
+-rw-r--r--   0        0        0      677 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png
+-rw-r--r--   0        0        0      657 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png
+-rw-r--r--   0        0        0      419 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hn.png
+-rw-r--r--   0        0        0      638 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png
+-rw-r--r--   0        0        0      568 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png
+-rw-r--r--   0        0        0      308 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hu.png
+-rw-r--r--   0        0        0      295 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/id.png
+-rw-r--r--   0        0        0      328 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ie.png
+-rw-r--r--   0        0        0      527 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/il.png
+-rw-r--r--   0        0        0      642 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/im.png
+-rw-r--r--   0        0        0      375 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/in.png
+-rw-r--r--   0        0        0      428 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/iq.png
+-rw-r--r--   0        0        0      553 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png
+-rw-r--r--   0        0        0      328 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/is.png
+-rw-r--r--   0        0        0      329 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/it.png
+-rw-r--r--   0        0        0     1133 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/je.png
+-rw-r--r--   0        0        0      779 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png
+-rw-r--r--   0        0        0      602 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png
+-rw-r--r--   0        0        0      614 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png
+-rw-r--r--   0        0        0      573 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png
+-rw-r--r--   0        0        0      725 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png
+-rw-r--r--   0        0        0      459 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kh.png
+-rw-r--r--   0        0        0      729 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/km.png
+-rw-r--r--   0        0        0     1020 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png
+-rw-r--r--   0        0        0      512 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png
+-rw-r--r--   0        0        0      845 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png
+-rw-r--r--   0        0        0      474 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kw.png
+-rw-r--r--   0        0        0      931 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png
+-rw-r--r--   0        0        0      883 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png
+-rw-r--r--   0        0        0      411 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/la.png
+-rw-r--r--   0        0        0      442 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lb.png
+-rw-r--r--   0        0        0      542 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png
+-rw-r--r--   0        0        0      263 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/li.png
+-rw-r--r--   0        0        0      799 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png
+-rw-r--r--   0        0        0      659 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png
+-rw-r--r--   0        0        0      401 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ls.png
+-rw-r--r--   0        0        0      274 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lt.png
+-rw-r--r--   0        0        0      314 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lu.png
+-rw-r--r--   0        0        0      285 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lv.png
+-rw-r--r--   0        0        0      352 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ly.png
+-rw-r--r--   0        0        0      513 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png
+-rw-r--r--   0        0        0      295 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mc.png
+-rw-r--r--   0        0        0      375 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/md.png
+-rw-r--r--   0        0        0      810 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/me.png
+-rw-r--r--   0        0        0      334 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mg.png
+-rw-r--r--   0        0        0     1071 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png
+-rw-r--r--   0        0        0      277 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ml.png
+-rw-r--r--   0        0        0      548 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png
+-rw-r--r--   0        0        0      390 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mn.png
+-rw-r--r--   0        0        0      620 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png
+-rw-r--r--   0        0        0      579 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png
+-rw-r--r--   0        0        0      900 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png
+-rw-r--r--   0        0        0      438 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mt.png
+-rw-r--r--   0        0        0      279 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mu.png
+-rw-r--r--   0        0        0      506 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mv.png
+-rw-r--r--   0        0        0      389 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mw.png
+-rw-r--r--   0        0        0      523 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png
+-rw-r--r--   0        0        0      686 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/my.png
+-rw-r--r--   0        0        0      590 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png
+-rw-r--r--   0        0        0      897 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/na.png
+-rw-r--r--   0        0        0      380 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ne.png
+-rw-r--r--   0        0        0      317 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ng.png
+-rw-r--r--   0        0        0      405 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ni.png
+-rw-r--r--   0        0        0      307 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/nl.png
+-rw-r--r--   0        0        0      402 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/no.png
+-rw-r--r--   0        0        0      866 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/np.png
+-rw-r--r--   0        0        0      784 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png
+-rw-r--r--   0        0        0      473 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/om.png
+-rw-r--r--   0        0        0      604 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png
+-rw-r--r--   0        0        0      319 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pe.png
+-rw-r--r--   0        0        0      534 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png
+-rw-r--r--   0        0        0      754 2024-04-02 09:54:00.487182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png
+-rw-r--r--   0        0        0      629 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png
+-rw-r--r--   0        0        0      682 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png
+-rw-r--r--   0        0        0      290 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pl.png
+-rw-r--r--   0        0        0      678 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png
+-rw-r--r--   0        0        0      545 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png
+-rw-r--r--   0        0        0      508 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pw.png
+-rw-r--r--   0        0        0      371 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/py.png
+-rw-r--r--   0        0        0      392 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/qa.png
+-rw-r--r--   0        0        0      273 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ro.png
+-rw-r--r--   0        0        0      525 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png
+-rw-r--r--   0        0        0      306 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ru.png
+-rw-r--r--   0        0        0      385 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/rw.png
+-rw-r--r--   0        0        0      676 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png
+-rw-r--r--   0        0        0     1126 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png
+-rw-r--r--   0        0        0      974 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png
+-rw-r--r--   0        0        0      523 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png
+-rw-r--r--   0        0        0      284 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/se.png
+-rw-r--r--   0        0        0      592 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png
+-rw-r--r--   0        0        0     1253 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png
+-rw-r--r--   0        0        0      430 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/si.png
+-rw-r--r--   0        0        0      772 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png
+-rw-r--r--   0        0        0      308 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sl.png
+-rw-r--r--   0        0        0      503 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sm.png
+-rw-r--r--   0        0        0      404 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sn.png
+-rw-r--r--   0        0        0      506 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/so.png
+-rw-r--r--   0        0        0      446 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sr.png
+-rw-r--r--   0        0        0      650 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/st.png
+-rw-r--r--   0        0        0      438 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sv.png
+-rw-r--r--   0        0        0      495 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sy.png
+-rw-r--r--   0        0        0      535 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png
+-rw-r--r--   0        0        0      919 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png
+-rw-r--r--   0        0        0      274 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/td.png
+-rw-r--r--   0        0        0      481 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tg.png
+-rw-r--r--   0        0        0      307 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/th.png
+-rw-r--r--   0        0        0      399 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tj.png
+-rw-r--r--   0        0        0      739 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png
+-rw-r--r--   0        0        0      786 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png
+-rw-r--r--   0        0        0      678 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png
+-rw-r--r--   0        0        0      522 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/to.png
+-rw-r--r--   0        0        0      649 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png
+-rw-r--r--   0        0        0     1025 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png
+-rw-r--r--   0        0        0      423 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tw.png
+-rw-r--r--   0        0        0      767 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png
+-rw-r--r--   0        0        0      260 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ua.png
+-rw-r--r--   0        0        0      598 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png
+-rw-r--r--   0        0        0      627 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/us.png
+-rw-r--r--   0        0        0      588 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png
+-rw-r--r--   0        0        0      494 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/uz.png
+-rw-r--r--   0        0        0      485 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vc.png
+-rw-r--r--   0        0        0      364 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ve.png
+-rw-r--r--   0        0        0      997 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png
+-rw-r--r--   0        0        0      503 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vn.png
+-rw-r--r--   0        0        0      666 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png
+-rw-r--r--   0        0        0      428 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ws.png
+-rw-r--r--   0        0        0      744 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png
+-rw-r--r--   0        0        0      308 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ye.png
+-rw-r--r--   0        0        0      802 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/za.png
+-rw-r--r--   0        0        0      501 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/zm.png
+-rw-r--r--   0        0        0      620 2024-04-02 09:54:00.491182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png
+-rw-r--r--   0        0        0  1664449 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/login.jpg
+-rw-r--r--   0        0        0    92962 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/login.webp
+-rw-r--r--   0        0        0     6363 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/logo.svg
+-rw-r--r--   0        0        0     2354 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/sk.svg
+-rw-r--r--   0        0        0   170535 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js
+-rw-r--r--   0        0        0     4819 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js
+-rw-r--r--   0        0        0     1323 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js
+-rw-r--r--   0        0        0    39433 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js
+-rw-r--r--   0        0        0    87461 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js
+-rw-r--r--   0        0        0     3063 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js
+-rw-r--r--   0        0        0     7770 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js
+-rw-r--r--   0        0        0     1698 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js
+-rw-r--r--   0        0        0     1914 2024-04-02 09:54:00.495182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/prices.js
+-rw-r--r--   0        0        0      932 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/remove-me.js
+-rw-r--r--   0        0        0   387673 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js
+-rw-r--r--   0        0        0      527 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg
+-rw-r--r--   0        0        0      682 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg
+-rw-r--r--   0        0        0      386 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-one.svg
+-rw-r--r--   0        0        0      826 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg
+-rw-r--r--   0        0        0      444 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-three.svg
+-rw-r--r--   0        0        0      477 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Aiming.svg
+-rw-r--r--   0        0        0      677 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg
+-rw-r--r--   0        0        0      732 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg
+-rw-r--r--   0        0        0      734 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg
+-rw-r--r--   0        0        0     1138 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg
+-rw-r--r--   0        0        0     1238 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg
+-rw-r--r--   0        0        0     1209 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg
+-rw-r--r--   0        0        0      509 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-down.svg
+-rw-r--r--   0        0        0      522 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg
+-rw-r--r--   0        0        0      524 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg
+-rw-r--r--   0        0        0      511 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-up.svg
+-rw-r--r--   0        0        0      737 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg
+-rw-r--r--   0        0        0      988 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg
+-rw-r--r--   0        0        0      538 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg
+-rw-r--r--   0        0        0      524 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg
+-rw-r--r--   0        0        0      304 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card.svg
+-rw-r--r--   0        0        0      622 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg
+-rw-r--r--   0        0        0      532 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg
+-rw-r--r--   0        0        0      824 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg
+-rw-r--r--   0        0        0      540 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg
+-rw-r--r--   0        0        0      583 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg
+-rw-r--r--   0        0        0      979 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg
+-rw-r--r--   0        0        0      281 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-small.svg
+-rw-r--r--   0        0        0      280 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check.svg
+-rw-r--r--   0        0        0      544 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg
+-rw-r--r--   0        0        0      318 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-small.svg
+-rw-r--r--   0        0        0      318 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close.svg
+-rw-r--r--   0        0        0      429 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Column.svg
+-rw-r--r--   0        0        0      361 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-left.svg
+-rw-r--r--   0        0        0      347 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-right.svg
+-rw-r--r--   0        0        0     1231 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg
+-rw-r--r--   0        0        0     2040 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg
+-rw-r--r--   0        0        0      611 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg
+-rw-r--r--   0        0        0      454 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete.svg
+-rw-r--r--   0        0        0      439 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-down.svg
+-rw-r--r--   0        0        0      433 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-left.svg
+-rw-r--r--   0        0        0      430 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-right.svg
+-rw-r--r--   0        0        0      439 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-up.svg
+-rw-r--r--   0        0        0      504 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-c.svg
+-rw-r--r--   0        0        0      296 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-small.svg
+-rw-r--r--   0        0        0      280 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down.svg
+-rw-r--r--   0        0        0      984 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg
+-rw-r--r--   0        0        0      386 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download.svg
+-rw-r--r--   0        0        0      898 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg
+-rw-r--r--   0        0        0      529 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg
+-rw-r--r--   0        0        0      442 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Excel-one.svg
+-rw-r--r--   0        0        0      636 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg
+-rw-r--r--   0        0        0     1432 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg
+-rw-r--r--   0        0        0      683 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg
+-rw-r--r--   0        0        0      575 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg
+-rw-r--r--   0        0        0      527 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg
+-rw-r--r--   0        0        0      570 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg
+-rw-r--r--   0        0        0      264 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Hamburger-button.svg
+-rw-r--r--   0        0        0      653 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg
+-rw-r--r--   0        0        0     1300 2024-04-02 09:54:00.499183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg
+-rw-r--r--   0        0        0      536 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg
+-rw-r--r--   0        0        0      756 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg
+-rw-r--r--   0        0        0     1039 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg
+-rw-r--r--   0        0        0      501 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-c.svg
+-rw-r--r--   0        0        0      247 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-down.svg
+-rw-r--r--   0        0        0      235 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-up.svg
+-rw-r--r--   0        0        0      301 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small.svg
+-rw-r--r--   0        0        0      272 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left.svg
+-rw-r--r--   0        0        0      852 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg
+-rw-r--r--   0        0        0      856 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg
+-rw-r--r--   0        0        0      714 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg
+-rw-r--r--   0        0        0      566 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg
+-rw-r--r--   0        0        0      403 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lock.svg
+-rw-r--r--   0        0        0      381 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Login.svg
+-rw-r--r--   0        0        0      376 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Logout.svg
+-rw-r--r--   0        0        0      887 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg
+-rw-r--r--   0        0        0      574 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg
+-rw-r--r--   0        0        0      666 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg
+-rw-r--r--   0        0        0      647 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg
+-rw-r--r--   0        0        0      418 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail.svg
+-rw-r--r--   0        0        0     1757 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg
+-rw-r--r--   0        0        0      555 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg
+-rw-r--r--   0        0        0      487 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus-the-top.svg
+-rw-r--r--   0        0        0      148 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus.svg
+-rw-r--r--   0        0        0      541 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg
+-rw-r--r--   0        0        0      810 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg
+-rw-r--r--   0        0        0      771 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg
+-rw-r--r--   0        0        0      547 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg
+-rw-r--r--   0        0        0     1528 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg
+-rw-r--r--   0        0        0      638 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg
+-rw-r--r--   0        0        0      874 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg
+-rw-r--r--   0        0        0      656 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg
+-rw-r--r--   0        0        0      940 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg
+-rw-r--r--   0        0        0      891 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg
+-rw-r--r--   0        0        0     1485 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg
+-rw-r--r--   0        0        0      242 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Plus.svg
+-rw-r--r--   0        0        0     2587 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg
+-rw-r--r--   0        0        0      938 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg
+-rw-r--r--   0        0        0     2362 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg
+-rw-r--r--   0        0        0      745 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg
+-rw-r--r--   0        0        0      362 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Reduce-one.svg
+-rw-r--r--   0        0        0      899 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg
+-rw-r--r--   0        0        0      507 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Return.svg
+-rw-r--r--   0        0        0      299 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora Filled.svg
+-rw-r--r--   0        0        0      504 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora.svg
+-rw-r--r--   0        0        0      501 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-c.svg
+-rw-r--r--   0        0        0      280 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-down.svg
+-rw-r--r--   0        0        0      243 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-up.svg
+-rw-r--r--   0        0        0      294 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small.svg
+-rw-r--r--   0        0        0      272 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right.svg
+-rw-r--r--   0        0        0      687 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg
+-rw-r--r--   0        0        0      461 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Search.svg
+-rw-r--r--   0        0        0      534 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg
+-rw-r--r--   0        0        0      328 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-config.svg
+-rw-r--r--   0        0        0     2761 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg
+-rw-r--r--   0        0        0     1380 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg
+-rw-r--r--   0        0        0     2218 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg
+-rw-r--r--   0        0        0      812 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg
+-rw-r--r--   0        0        0      940 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg
+-rw-r--r--   0        0        0      497 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort Alt.svg
+-rw-r--r--   0        0        0      311 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-down.svg
+-rw-r--r--   0        0        0      334 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-up.svg
+-rw-r--r--   0        0        0      360 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-one.svg
+-rw-r--r--   0        0        0      479 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-three.svg
+-rw-r--r--   0        0        0      809 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg
+-rw-r--r--   0        0        0     1175 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg
+-rw-r--r--   0        0        0     1876 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg
+-rw-r--r--   0        0        0      323 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Switch.svg
+-rw-r--r--   0        0        0      525 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg
+-rw-r--r--   0        0        0      806 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg
+-rw-r--r--   0        0        0      485 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag.svg
+-rw-r--r--   0        0        0      490 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tips-one.svg
+-rw-r--r--   0        0        0      312 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/To-top.svg
+-rw-r--r--   0        0        0      476 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Transfer-data.svg
+-rw-r--r--   0        0        0     2485 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg
+-rw-r--r--   0        0        0     1003 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg
+-rw-r--r--   0        0        0      860 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg
+-rw-r--r--   0        0        0     1074 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg
+-rw-r--r--   0        0        0      592 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg
+-rw-r--r--   0        0        0      393 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Unlock.svg
+-rw-r--r--   0        0        0      504 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-c.svg
+-rw-r--r--   0        0        0      299 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-small.svg
+-rw-r--r--   0        0        0      279 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up.svg
+-rw-r--r--   0        0        0      988 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg
+-rw-r--r--   0        0        0      385 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload.svg
+-rw-r--r--   0        0        0      777 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg
+-rw-r--r--   0        0        0      888 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg
+-rw-r--r--   0        0        0      680 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg
+-rw-r--r--   0        0        0      584 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg
+-rw-r--r--   0        0        0      490 2024-04-02 09:54:00.503183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-out.svg
+-rw-r--r--   0        0        0     1840 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_base.css
+-rw-r--r--   0        0        0     1889 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css
+-rw-r--r--   0        0        0     2825 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css
+-rw-r--r--   0        0        0    12213 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_components.css
+-rw-r--r--   0        0        0    14025 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css
+-rw-r--r--   0        0        0     4096 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css
+-rw-r--r--   0        0        0     5587 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css
+-rw-r--r--   0        0        0    18294 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css
+-rw-r--r--   0        0        0       58 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_tailwind_base.css
+-rw-r--r--   0        0        0      901 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css
+-rw-r--r--   0        0        0     4665 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css
+-rw-r--r--   0        0        0     1763 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css
+-rw-r--r--   0        0        0    10276 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css
+-rw-r--r--   0        0        0     4316 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css
+-rw-r--r--   0        0        0      719 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css
+-rw-r--r--   0        0        0    10087 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css
+-rw-r--r--   0        0        0     2388 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css
+-rw-r--r--   0        0        0     2485 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css
+-rw-r--r--   0        0        0      361 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/style.css
+-rw-r--r--   0        0        0    12215 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js
+-rw-r--r--   0        0        0     4736 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/chart.js
+-rw-r--r--   0        0        0     4615 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/choices.js
+-rw-r--r--   0        0        0      486 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/code.js
+-rw-r--r--   0        0        0    14259 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js
+-rw-r--r--   0        0        0     9131 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/main.js
+-rw-r--r--   0        0        0     3354 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js
+-rw-r--r--   0        0        0     1733 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/range.js
+-rw-r--r--   0        0        0     1570 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js
+-rw-r--r--   0        0        0     1186 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js
+-rw-r--r--   0        0        0     9952 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table.js
+-rw-r--r--   0        0        0      507 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/base_module.js
+-rw-r--r--   0        0        0    10561 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js
+-rw-r--r--   0        0        0      929 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js
+-rw-r--r--   0        0        0      686 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js
+-rw-r--r--   0        0        0     4016 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js
+-rw-r--r--   0        0        0     7694 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js
+-rw-r--r--   0        0        0     6403 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js
+-rw-r--r--   0        0        0    11157 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js
+-rw-r--r--   0        0        0     2383 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js
+-rw-r--r--   0        0        0      954 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/translations.js
+-rw-r--r--   0        0        0     4245 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/utils.js
+-rw-r--r--   0        0        0    10987 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html
+-rw-r--r--   0        0        0     3200 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html
+-rw-r--r--   0        0        0      272 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/dashboard.html
+-rw-r--r--   0        0        0     3205 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html
+-rw-r--r--   0        0        0     2248 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     9442 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/list.html
+-rw-r--r--   0        0        0      122 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/media.html
+-rw-r--r--   0        0        0     1905 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html
+-rw-r--r--   0        0        0      109 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/partials/open_modal_attrs.html
+-rw-r--r--   0        0        0      857 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html
+-rw-r--r--   0        0        0     4542 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html
+-rw-r--r--   0        0        0      587 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html
+-rw-r--r--   0        0        0      334 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations-list.html
+-rw-r--r--   0        0        0     1285 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations.html
+-rw-r--r--   0        0        0       50 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     2398 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/login.html
+-rw-r--r--   0        0        0      864 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html
+-rw-r--r--   0        0        0      496 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/logout.html
+-rw-r--r--   0        0        0      485 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_done.html
+-rw-r--r--   0        0        0     1905 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html
+-rw-r--r--   0        0        0      503 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_complete.html
+-rw-r--r--   0        0        0     1310 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html
+-rw-r--r--   0        0        0      666 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html
+-rw-r--r--   0        0        0      621 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html
+-rw-r--r--   0        0        0     1397 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html
+-rw-r--r--   0        0        0       76 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/blank_base.html
+-rw-r--r--   0        0        0     1982 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/buttons.html
+-rw-r--r--   0        0        0      959 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/columns.html
+-rw-r--r--   0        0        0     2654 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/filters.html
+-rw-r--r--   0        0        0    10938 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/inputs.html
+-rw-r--r--   0        0        0     4543 2024-04-02 09:54:00.507182 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/config/view.html
+-rw-r--r--   0        0        0      900 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html
+-rw-r--r--   0        0        0     1096 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html
+-rw-r--r--   0        0        0      141 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/list_widget.html
+-rw-r--r--   0        0        0      720 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html
+-rw-r--r--   0        0        0     1071 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html
+-rw-r--r--   0        0        0      548 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html
+-rw-r--r--   0        0        0      645 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html
+-rw-r--r--   0        0        0      648 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html
+-rw-r--r--   0        0        0     1243 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html
+-rw-r--r--   0        0        0     1162 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html
+-rw-r--r--   0        0        0      614 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html
+-rw-r--r--   0        0        0     1212 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html
+-rw-r--r--   0        0        0      548 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html
+-rw-r--r--   0        0        0     1121 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/fonts.html
+-rw-r--r--   0        0        0      165 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/attrs.html
+-rw-r--r--   0        0        0      172 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/change_form_title.html
+-rw-r--r--   0        0        0    18710 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/components.html
+-rw-r--r--   0        0        0      229 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/fieldset.html
+-rw-r--r--   0        0        0     2227 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html
+-rw-r--r--   0        0        0      287 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/loading.html
+-rw-r--r--   0        0        0      304 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/loading_absolute.html
+-rw-r--r--   0        0        0      771 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html
+-rw-r--r--   0        0        0     7592 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html
+-rw-r--r--   0        0        0    15127 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html
+-rw-r--r--   0        0        0     3046 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html
+-rw-r--r--   0        0        0    18190 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html
+-rw-r--r--   0        0        0      308 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/cms/translations_status_row.html
+-rw-r--r--   0        0        0     3002 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html
+-rw-r--r--   0        0        0    18834 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html
+-rw-r--r--   0        0        0     1909 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html
+-rw-r--r--   0        0        0    15189 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html
+-rw-r--r--   0        0        0     9195 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/navigation.html
+-rw-r--r--   0        0        0      825 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html
+-rw-r--r--   0        0        0      121 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_close.html
+-rw-r--r--   0        0        0      276 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_error.html
+-rw-r--r--   0        0        0      268 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_info.html
+-rw-r--r--   0        0        0      323 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_success.html
+-rw-r--r--   0        0        0      323 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_warning.html
+-rw-r--r--   0        0        0     1507 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html
+-rw-r--r--   0        0        0      505 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sb_admin_base.html
+-rw-r--r--   0        0        0     3253 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html
+-rw-r--r--   0        0        0      817 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html
+-rw-r--r--   0        0        0    59910 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg
+-rw-r--r--   0        0        0     3254 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/submit_line.html
+-rw-r--r--   0        0        0      577 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html
+-rw-r--r--   0        0        0     2815 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/array.html
+-rw-r--r--   0        0        0      172 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/attrs.html
+-rw-r--r--   0        0        0     2434 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html
+-rw-r--r--   0        0        0      232 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox.html
+-rw-r--r--   0        0        0       51 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_option.html
+-rw-r--r--   0        0        0     1578 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html
+-rw-r--r--   0        0        0      542 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html
+-rw-r--r--   0        0        0     2340 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html
+-rw-r--r--   0        0        0      345 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/code.html
+-rw-r--r--   0        0        0      160 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/date.html
+-rw-r--r--   0        0        0       44 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/datetime.html
+-rw-r--r--   0        0        0       43 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/email.html
+-rw-r--r--   0        0        0       44 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/file.html
+-rw-r--r--   0        0        0       44 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/hidden.html
+-rw-r--r--   0        0        0      148 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/includes/field_label.html
+-rw-r--r--   0        0        0      148 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/includes/help_text.html
+-rw-r--r--   0        0        0      443 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/includes/simple_field_label.html
+-rw-r--r--   0        0        0      185 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/input.html
+-rw-r--r--   0        0        0      209 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/input_option.html
+-rw-r--r--   0        0        0       50 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/multiple_hidden.html
+-rw-r--r--   0        0        0      329 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/multiwidget.html
+-rw-r--r--   0        0        0      159 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/number.html
+-rw-r--r--   0        0        0      585 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/password.html
+-rw-r--r--   0        0        0      363 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/radio.html
+-rw-r--r--   0        0        0       51 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/radio_option.html
+-rw-r--r--   0        0        0      216 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/read_only_password_hash.html
+-rw-r--r--   0        0        0      496 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/select.html
+-rw-r--r--   0        0        0       50 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/select_date.html
+-rw-r--r--   0        0        0      123 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/select_option.html
+-rw-r--r--   0        0        0       50 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/splitdatetime.html
+-rw-r--r--   0        0        0       50 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/splithiddendatetime.html
+-rw-r--r--   0        0        0      160 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/text.html
+-rw-r--r--   0        0        0      257 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/textarea.html
+-rw-r--r--   0        0        0      160 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/time.html
+-rw-r--r--   0        0        0      280 2024-04-02 09:54:00.511183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/toggle.html
+-rw-r--r--   0        0        0      160 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/url.html
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templatetags/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templatetags/base.py
+-rw-r--r--   0        0        0     4125 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/templatetags/sb_admin_tags.py
+-rw-r--r--   0        0        0       17 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/urls.py
+-rw-r--r--   0        0        0     1343 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/dashboard_view.py
+-rw-r--r--   0        0        0      954 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/global_filter_view.py
+-rw-r--r--   0        0        0      292 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/media_view.py
+-rw-r--r--   0        0        0    20254 2024-04-02 09:54:00.515183 django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/translations_view.py
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 django_smartbase_admin-0.2.4/PKG-INFO
```

### Comparing `django_smartbase_admin-0.2.3/LICENSE.md` & `django_smartbase_admin-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/pyproject.toml` & `django_smartbase_admin-0.2.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-smartbase-admin"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["SmartBase <info@smartbase.sk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = ">= 4.1, < 6.0"
```

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/actions/admin_action_list.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/actions/admin_action_list.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/admin_base.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/admin_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,16 @@
 
 class SBAdminBaseFormInit(SBAdminFormFieldWidgetsMixin):
     threadsafe_request = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for field in self.fields:
+            if not hasattr(self.fields[field].widget, 'init_widget_dynamic'):
+                continue
             self.fields[field].widget.init_widget_dynamic(
                 self,
                 self.fields[field],
                 field,
                 self.view,
                 self.threadsafe_request,
             )
```

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/site.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/admin/widgets.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/admin/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
     def __init__(self, form_field=None, attrs=None):
         super().__init__(
             form_field, attrs={"class": "input js-datetimepicker", **(attrs or {})}
         )
 
 
-class SBAdminSplitDateTimeWidget(forms.SplitDateTimeWidget):
+class SBAdminSplitDateTimeWidget(SBAdminBaseWidget, forms.SplitDateTimeWidget):
     template_name = "sb_admin/widgets/splitdatetime.html"
 
     def __init__(self, form_field=None, attrs=None):
         self.form_field = form_field
         widgets = [SBAdminDateWidget, SBAdminTimeWidget]
         # init of forms.MultiWidget with form_field attribute during widget instancing
         if isinstance(widgets, dict):
```

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/actions.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/actions.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_base_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_base_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_entrypoint_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_entrypoint_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/admin_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/admin_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/configuration.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/configuration.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/const.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/const.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/dashboard.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/dashboard.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/fake_inline.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/fake_inline.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/field.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/field.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/field_formatter.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/field_formatter.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/filter_widgets.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/filter_widgets.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/menu_item.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/menu_item.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/engine/request.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/engine/request.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0001_initial.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/models.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/models.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/configuration.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/configuration.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/thread_local.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/thread_local.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/translations.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/translations.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/views.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/views.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/services/xlsx_export.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/services/xlsx_export.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/chart.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/chart.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/main_style.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/main_style.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/table.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/table.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/dist/translations.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/dist/translations.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/al.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/al.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/au.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/au.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/br.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/br.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/en.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/en.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/er.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/er.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/et.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/et.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/il.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/il.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/im.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/im.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/je.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/je.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/km.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/km.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/me.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/me.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/my.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/my.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/na.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/na.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/np.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/np.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/st.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/st.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/to.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/to.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/us.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/us.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/za.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/za.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/login.jpg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/login.jpg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/login.webp` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/login.webp`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/logo.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/images/sk.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/images/sk.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/prices.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/prices.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/remove-me.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/remove-me.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_base.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_base.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_components.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_components.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/chart.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/choices.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/choices.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/main.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/main.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/range.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/range.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/translations.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/translations.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/static/sb_admin/src/js/utils.js` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/static/sb_admin/src/js/utils.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/list.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/actions/translations.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/actions/translations.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/login.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/login.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/buttons.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/buttons.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/columns.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/columns.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/filters.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/filters.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/components/inputs.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/components/inputs.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/config/view.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/config/view.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/fonts.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/fonts.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/components.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/components.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/navigation.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/navigation.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/submit_line.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/array.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/array.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templates/sb_admin/widgets/password.html` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templates/sb_admin/widgets/password.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templatetags/base.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templatetags/base.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/templatetags/sb_admin_tags.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/templatetags/sb_admin_tags.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/utils.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/utils.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/dashboard_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/global_filter_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/global_filter_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/src/django_smartbase_admin/views/translations_view.py` & `django_smartbase_admin-0.2.4/src/django_smartbase_admin/views/translations_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.3/PKG-INFO` & `django_smartbase_admin-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-smartbase-admin
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: SmartBase
 Author-email: info@smartbase.sk
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

