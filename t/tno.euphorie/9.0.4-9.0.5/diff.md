# Comparing `tmp/tno.euphorie-9.0.4.tar.gz` & `tmp/tno.euphorie-9.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tno.euphorie-9.0.4.tar", last modified: Tue Feb 28 14:28:19 2023, max compression
+gzip compressed data, was "tno.euphorie-9.0.5.tar", last modified: Wed Mar 22 10:26:13 2023, max compression
```

## Comparing `tno.euphorie-9.0.4.tar` & `tno.euphorie-9.0.5.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/
--rw-rw-r--   0 ale       (1000) ale       (1000)      702 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      293 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)    16550 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1094 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/README.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)     1885 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/base.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     6023 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/bootstrap.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      697 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/devel.cfg
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/docs/
--rw-rw-r--   0 ale       (1000) ale       (1000)     5586 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)     7321 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/api.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)    14684 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/changes.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)     8278 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/conf.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      787 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/index.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)      384 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/docs/installation.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)     1234 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/picked-versions.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)       40 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/requirements.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      422 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1616 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/
--rw-rw-r--   0 ale       (1000) ale       (1000)      245 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/
--rw-rw-r--   0 ale       (1000) ale       (1000)      336 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/assets/
--rw-rw-r--   0 ale       (1000) ale       (1000)    16396 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/assets/od-logo.png
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/client/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4319 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/company.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3370 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     9652 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/docx_reports.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      298 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/module.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/overrides/
--rw-rw-r--   0 ale       (1000) ale       (1000)     8657 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/overrides/euphorie.client.browser.templates.conditions-bare.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)      322 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/report.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      356 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/risk.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     8643 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/session.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/
--rw-rw-r--   0 ale       (1000) ale       (1000)    19498 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/measures_overview.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)    11344 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/report_company.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     8526 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/report_landing.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)    22365 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/rie.docx
--rw-rw-r--   0 ale       (1000) ale       (1000)     1150 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/client.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      375 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/client/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1069 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/configure.zcml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/content/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      407 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      107 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/survey.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/templates/
--rw-rw-r--   0 ale       (1000) ale       (1000)     2916 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/browser/templates/survey_view.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)      206 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/content/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      684 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/interfaces.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/locales/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/locales/nl/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 ale       (1000) ale       (1000)    13103 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/locales/nl/LC_MESSAGES/euphorie.po
--rw-rw-r--   0 ale       (1000) ale       (1000)     3104 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/model.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      920 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      412 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/interfaces.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/
--rw-rw-r--   0 ale       (1000) ale       (1000)     2284 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/error_unauthorized.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1101 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/largetextarea_input.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1376 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/wysiwyg_input.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1556 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/nuplone/widget.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno/euphorie/profiles/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/
--rw-rw-r--   0 ale       (1000) ale       (1000)      141 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/browserlayer.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)       88 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/mailhost.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      170 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/metadata.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      192 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/properties.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      136 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/profiles/default/skins.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      796 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/schema.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/templates/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1930 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/templates/upload.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1777 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/testing.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      291 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_client.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7219 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_company.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3482 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_module.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      787 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_report.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5352 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_risk.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4731 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_session.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4129 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_survey.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      396 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/tests/test_testing.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1998 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/env.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      494 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/script.py.mako
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/versions/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1584 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/versions/203_.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      750 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/versions/204_.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2374 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/configure.zcml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/to_204/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1251 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/to_204/registry.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      598 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/v1.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1357 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/v2.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      171 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno/euphorie/upgrade/v3.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.282305 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)    16550 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     3198 2023-02-28 14:28:19.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        4 2023-02-28 14:28:19.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/namespace_packages.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      189 2023-02-28 14:28:19.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        4 2023-02-28 14:28:19.000000 tno.euphorie-9.0.4/src/tno.euphorie.egg-info/top_level.txt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-02-28 14:28:19.286305 tno.euphorie-9.0.4/templates/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1327 2023-02-28 14:28:18.000000 tno.euphorie-9.0.4/templates/euphorie.ini
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      702 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)      293 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)    16990 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1094 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/README.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1885 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/base.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6023 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/bootstrap.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      697 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/devel.cfg
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/docs/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5586 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7321 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/api.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)    15124 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/changes.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8270 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/conf.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      787 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/index.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)      384 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/docs/installation.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1234 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/picked-versions.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)       40 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/requirements.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      422 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1616 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.885789 tno.euphorie-9.0.5/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      245 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      337 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/assets/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    16396 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/assets/od-logo.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/client/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4277 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/company.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3369 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9656 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/docx_reports.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      298 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/module.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/overrides/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8657 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/overrides/euphorie.client.browser.templates.conditions-bare.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      319 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/report.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      356 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/risk.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8637 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/session.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    19498 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/measures_overview.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11344 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/report_company.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8526 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/report_landing.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    22365 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/rie.docx
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1150 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/client.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      375 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/client/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1069 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/configure.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/content/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      407 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      107 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/survey.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3000 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/browser/templates/survey_view.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      206 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/content/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      684 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/interfaces.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.885789 tno.euphorie-9.0.5/src/tno/euphorie/locales/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.885789 tno.euphorie-9.0.5/src/tno/euphorie/locales/nl/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13103 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/locales/nl/LC_MESSAGES/euphorie.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3104 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/model.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      920 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      412 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/interfaces.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2284 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/error_unauthorized.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1101 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/largetextarea_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1376 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/wysiwyg_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1554 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/nuplone/widget.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.885789 tno.euphorie-9.0.5/src/tno/euphorie/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      141 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/browserlayer.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       88 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/mailhost.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      170 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      192 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/properties.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      136 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/profiles/default/skins.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      796 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/schema.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1930 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/templates/upload.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1777 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      291 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_client.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7219 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_company.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3482 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_module.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      776 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_report.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5352 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_risk.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4730 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_session.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4129 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_survey.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      396 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/tests/test_testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1998 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/env.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      494 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/script.py.mako
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/versions/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1582 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/versions/203_.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      750 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/versions/204_.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2374 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/configure.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/to_204/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1251 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/to_204/registry.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      598 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/v1.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1357 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/v2.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      172 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/src/tno/euphorie/upgrade/v3.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    16990 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3198 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        4 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      189 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        4 2023-03-22 10:26:13.000000 tno.euphorie-9.0.5/src/tno.euphorie.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-22 10:26:13.889788 tno.euphorie-9.0.5/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1327 2023-03-22 10:26:12.000000 tno.euphorie-9.0.5/templates/euphorie.ini
```

### Comparing `tno.euphorie-9.0.4/MANIFEST.in` & `tno.euphorie-9.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/PKG-INFO` & `tno.euphorie-9.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.euphorie
-Version: 9.0.4
+Version: 9.0.5
 Summary: TNO specific extensions for Euphorie
 Home-page: http://readthedocs.org/docs/tnoeuphorie/en/latest/
 Author: Wichert Akkerman and Syslab.com
 Author-email: info@syslab.com
 License: GPL
 Keywords: Euphorie OIRA RIE
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,28 @@
 If you do not already have Euphorie installed it will be installed
 automatically.
 
 
 Changelog
 =========
 
+9.0.5 (2023-03-22)
+------------------
+
+- Adapt the survey-view template to the latest Euphorie
+  [ale-rt]
+- Fix for prioritiy risks being displayed though they were answered N/A.
+  https://github.com/syslabcom/scrum/issues/1020
+  [reinhardt]
+- Fix the ``@@plan_van_aanpak.docx`` report to display some numerical number as zeros and not
+  as not provided values.
+  Fixes `#1054 <https://github.com/syslabcom/scrum/issues/1054>`_
+  [ale-rt]
+
+
 9.0.4 (2023-02-28)
 ------------------
 
 - Add custom terms of service and condition (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
 - Hide the organisation tab (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
@@ -181,15 +195,15 @@
 - Switch to Plone5
 
 
 6.0.15 (2018-07-13)
 -------------------
 
 - Bugfix for the "measures" report: Do not rely on the pre-computed
-  list of modules, since this can fail for a scenario with 
+  list of modules, since this can fail for a scenario with
   module->module->Optional module
 
 6.0.14 (2017-11-01)
 -------------------
 
 - Another bugfix for the "measures" report. Correctly compute the
   future months
```

### Comparing `tno.euphorie-9.0.4/README.rst` & `tno.euphorie-9.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/base.cfg` & `tno.euphorie-9.0.5/base.cfg`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/bootstrap.py` & `tno.euphorie-9.0.5/bootstrap.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/devel.cfg` & `tno.euphorie-9.0.5/devel.cfg`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/docs/Makefile` & `tno.euphorie-9.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/docs/api.rst` & `tno.euphorie-9.0.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/docs/changes.rst` & `tno.euphorie-9.0.5/docs/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+9.0.5 (2023-03-22)
+------------------
+
+- Adapt the survey-view template to the latest Euphorie
+  [ale-rt]
+- Fix for prioritiy risks being displayed though they were answered N/A.
+  https://github.com/syslabcom/scrum/issues/1020
+  [reinhardt]
+- Fix the ``@@plan_van_aanpak.docx`` report to display some numerical number as zeros and not
+  as not provided values.
+  Fixes `#1054 <https://github.com/syslabcom/scrum/issues/1054>`_
+  [ale-rt]
+
+
 9.0.4 (2023-02-28)
 ------------------
 
 - Add custom terms of service and condition (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
 - Hide the organisation tab (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
@@ -120,15 +134,15 @@
 - Switch to Plone5
 
 
 6.0.15 (2018-07-13)
 -------------------
 
 - Bugfix for the "measures" report: Do not rely on the pre-computed
-  list of modules, since this can fail for a scenario with 
+  list of modules, since this can fail for a scenario with
   module->module->Optional module
 
 6.0.14 (2017-11-01)
 -------------------
 
 - Another bugfix for the "measures" report. Correctly compute the
   future months
```

### Comparing `tno.euphorie-9.0.4/docs/conf.py` & `tno.euphorie-9.0.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"tno.euphorie"
-copyright = u"2012, Wichert Akkerman - Simplon B.V."
+project = "tno.euphorie"
+copyright = "2012, Wichert Akkerman - Simplon B.V."
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "2.0"
@@ -178,16 +178,16 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
     (
         "index",
         "tnoeuphorie.tex",
-        u"tno.euphorie Documentation",
-        u"Wichert Akkerman - Simplon B.V.",
+        "tno.euphorie Documentation",
+        "Wichert Akkerman - Simplon B.V.",
         "manual",
     ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
@@ -213,16 +213,16 @@
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         "index",
         "tnoeuphorie",
-        u"tno.euphorie Documentation",
-        [u"Wichert Akkerman - Simplon B.V."],
+        "tno.euphorie Documentation",
+        ["Wichert Akkerman - Simplon B.V."],
         1,
     )
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
@@ -232,16 +232,16 @@
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         "index",
         "tnoeuphorie",
-        u"tno.euphorie Documentation",
-        u"Wichert Akkerman - Simplon B.V.",
+        "tno.euphorie Documentation",
+        "Wichert Akkerman - Simplon B.V.",
         "tnoeuphorie",
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
 
 # Documents to append as an appendix to all manuals.
```

### Comparing `tno.euphorie-9.0.4/docs/index.rst` & `tno.euphorie-9.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/picked-versions.cfg` & `tno.euphorie-9.0.5/picked-versions.cfg`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/setup.py` & `tno.euphorie-9.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "9.0.4"
+version = "9.0.5"
 
 setup(
     name="tno.euphorie",
     version=version,
     description="TNO specific extensions for Euphorie",
     long_description=open("README.rst").read()
     + "\n"
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/assets/od-logo.png` & `tno.euphorie-9.0.5/src/tno/euphorie/assets/od-logo.png`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/company.py` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/company.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,78 +13,76 @@
 
 
 TextSpan1 = FieldWidgetFactory("z3c.form.browser.text.TextFieldWidget", klass="span-1")
 TextSpan6 = FieldWidgetFactory("z3c.form.browser.text.TextFieldWidget", klass="span-6")
 
 
 class DutchCompanySchema(Schema):
-    title = schema.TextLine(title=u"Bedrijfsnaam", max_length=128, required=False)
+    title = schema.TextLine(title="Bedrijfsnaam", max_length=128, required=False)
 
-    address_visit_address = schema.TextLine(title=u"Adres", required=False)
+    address_visit_address = schema.TextLine(title="Adres", required=False)
     address_visit_postal = schema.TextLine(
-        title=u"Postcode", max_length=16, required=False
+        title="Postcode", max_length=16, required=False
     )
-    address_visit_city = schema.TextLine(title=u"Plaats", max_length=64, required=False)
+    address_visit_city = schema.TextLine(title="Plaats", max_length=64, required=False)
 
-    address_postal_address = schema.TextLine(title=u"Adres", required=False)
+    address_postal_address = schema.TextLine(title="Adres", required=False)
     address_postal_postal = schema.TextLine(
-        title=u"Postcode", max_length=16, required=False
+        title="Postcode", max_length=16, required=False
     )
-    address_postal_city = schema.TextLine(
-        title=u"Plaats", max_length=64, required=False
-    )
-    email = schema.ASCIILine(title=u"E-mailadres", max_length=128, required=False)
+    address_postal_city = schema.TextLine(title="Plaats", max_length=64, required=False)
+    email = schema.ASCIILine(title="E-mailadres", max_length=128, required=False)
     # widget(email="tno.euphorie.company.TextSpan6")
-    phone = schema.ASCIILine(title=u"Telefoonnummer", max_length=32, required=False)
+    phone = schema.ASCIILine(title="Telefoonnummer", max_length=32, required=False)
     activity = schema.TextLine(
-        title=u"Bedrijfsactiviteit", max_length=64, required=False
+        title="Bedrijfsactiviteit", max_length=64, required=False
     )
     submitter_name = schema.TextLine(
-        title=u"Naam invuller", max_length=64, required=False
+        title="Naam invuller", max_length=64, required=False
     )
     submitter_function = schema.TextLine(
-        title=u"Functie invuller", max_length=64, required=False
+        title="Functie invuller", max_length=64, required=False
     )
-    department = schema.TextLine(title=u"Afdeling", max_length=64, required=False)
-    location = schema.TextLine(title=u"Lokatie", max_length=64, required=False)
+    department = schema.TextLine(title="Afdeling", max_length=64, required=False)
+    location = schema.TextLine(title="Lokatie", max_length=64, required=False)
     submit_date = schema.Date(
-        title=u"Datum",
-        description=u"Datum waarop de gegevens verzameld zijn",
+        title="Datum",
+        description="Datum waarop de gegevens verzameld zijn",
         min=datetime.date(2000, 1, 1),
         required=False,
     )
     employees = schema.Choice(
-        title=u"Aantal werknemers",
+        title="Aantal werknemers",
         vocabulary=SimpleVocabulary(
             [
-                SimpleTerm(u"40h", title=u"Maximaal 40 uur betaalde arbeid per week"),
-                SimpleTerm(u"max25", title=u"Maximaal 25 werknemers"),
-                SimpleTerm(u"over25", title=u"Meer dan 25 werknemers"),
+                SimpleTerm("40h", title="Maximaal 40 uur betaalde arbeid per week"),
+                SimpleTerm("max25", title="Maximaal 25 werknemers"),
+                SimpleTerm("over25", title="Meer dan 25 werknemers"),
             ]
         ),
         required=False,
     )
     absentee_percentage = schema.Decimal(
-        title=u"Verzuimpercentage",
+        title="Verzuimpercentage",
         min=decimal.Decimal(0),
         max=decimal.Decimal(100),
         required=False,
     )
     # widget(absentee_percentage="tno.euphorie.company.TextSpan1")
-    accidents = schema.Int(title=u"Aantal ongevallen vorig jaar", required=False)
+    accidents = schema.Int(title="Aantal ongevallen vorig jaar", required=False)
     # widget(accidents="tno.euphorie.company.TextSpan1")
     incapacitated_workers = schema.Int(
-        title=u"Aantal mensen in de WIA vorig jaar", required=False
+        title="Aantal mensen in de WIA vorig jaar", required=False
     )
     # widget(incapacitated_workers="tno.euphorie.company.TextSpan1")
     arbo_expert = schema.TextLine(
-        title=u"Gegevens arbodienst/-deskundige", max_length=128, required=False
+        title="Gegevens arbodienst/-deskundige", max_length=128, required=False
     )
     works_council_approval = schema.Date(
-        title=u"Datum van akkoord OR/medewerkersvertegenwoordiging",
+        title="Datum van akkoord OR/medewerkersvertegenwoordiging",
         min=datetime.date(2000, 1, 1),
         required=False,
     )
 
 
 class Company(GenericCompany):
     """Update the company details.
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/configure.zcml` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <!-- Action Plan landing -->
       <browser:page
           name="actionplan"
           for="euphorie.client.adapters.session_traversal.ITraversedSurveySession"
           permission="euphorie.client.ViewSurvey"
           class="tno.euphorie.client.browser.session.ActionPlanView"
           template="templates/actionplan.pt"
-          layer="tno.euphorie.interfaces.ITnoContentSkinLayer"
+          layer="tno.euphorie.interfaces.ITnoClientSkinLayer"
           />
 
       <!-- Status -->
       <browser:page
           name="status"
           for="euphorie.client.adapters.session_traversal.ITraversedSurveySession"
           permission="euphorie.client.ViewSurvey"
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/docx_reports.py` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/docx_reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,43 +22,43 @@
         """This fills the workspace activity run with some text"""
         request = self.request
         doc = self.template
         header = doc.sections[0].header
         h_table = header.tables[0]
 
         h_table.cell(0, 0).paragraphs[0].text = data["heading"]
-        h_table.cell(0, 1).paragraphs[0].text = u"Datum download: {}".format(
+        h_table.cell(0, 1).paragraphs[0].text = "Datum download: {}".format(
             formatDate(request, date.today())
         )
 
         doc.paragraphs[0].text = data["heading"]
 
-        heading1 = self.t(_("plan_report_intro_header", default=u"Introduction"))
+        heading1 = self.t(_("plan_report_intro_header", default="Introduction"))
         intro = self.t(
             _(
                 "plan_report_intro_1",
-                default=u"By filling in the list of questions, you have "
-                u"completed a risk assessment. This assessment is used to "
-                u"draw up an action plan. The progress of this action "
-                u"plan must be discussed annually and a small report must "
-                u"be written on the progress. Certain subjects might have "
-                u"been completed and perhaps new subjects need to be "
-                u"added.",
+                default="By filling in the list of questions, you have "
+                "completed a risk assessment. This assessment is used to "
+                "draw up an action plan. The progress of this action "
+                "plan must be discussed annually and a small report must "
+                "be written on the progress. Certain subjects might have "
+                "been completed and perhaps new subjects need to be "
+                "added.",
             )
         )
 
         doc.add_paragraph(heading1, style="Heading 1")
         doc.add_paragraph(intro)
 
         survey = aq_parent(self.context)
         footer_txt = self.t(
             _(
                 "report_survey_revision",
-                default=u"This document was based on the OiRA Tool '${title}' "
-                u"of revision date ${date}.",
+                default="This document was based on the OiRA Tool '${title}' "
+                "of revision date ${date}.",
                 mapping={
                     "title": survey.published[1],
                     "date": formatDate(request, survey.published[2]),
                 },
             )
         )
         footer = doc.sections[0].footer
@@ -77,18 +77,18 @@
         # paragraph = table.cell(0, 0).paragraphs[0]
 
         paragraph.style = "Footer"
         paragraph.text = footer_txt
 
         doc.add_page_break()
         doc.add_paragraph(
-            self.t(_("plan_report_company_header", default=u"Company details")),
+            self.t(_("plan_report_company_header", default="Company details")),
             style="Heading 1",
         )
-        missing = self.t(_("missing_data", default=u"Not provided"))
+        missing = self.t(_("missing_data", default="Not provided"))
         company = self.session.dutch_company
         table = doc.add_table(rows=1, cols=2)
         total_width = table.columns[0].width + table.columns[1].width
         table.columns[0].width = int(total_width * 0.20)
         table.columns[1].width = int(total_width * 0.80)
 
         field = DutchCompanySchema["title"]
@@ -139,25 +139,25 @@
             row_cells[1].text = value if value else missing
 
         formatDecimal = request.locale.numbers.getFormatter("decimal").format
         field = DutchCompanySchema["absentee_percentage"]
         row_cells = table.add_row().cells
         row_cells[0].text = str(field.title)
         row_cells[1].text = (
-            u"%s %%" % formatDecimal(company.absentee_percentage)
-            if company and company.absentee_percentage
+            "%s %%" % formatDecimal(company.absentee_percentage)
+            if company and company.absentee_percentage is not None
             else missing
         )
 
         for key in ["accidents", "incapacitated_workers"]:
             field = DutchCompanySchema[key]
             value = getattr(company, key, None)
             row_cells = table.add_row().cells
             row_cells[0].text = str(field.title)
-            row_cells[1].text = "%d" % value if value else missing
+            row_cells[1].text = "%d" % value if value is not None else missing
 
         field = DutchCompanySchema["submit_date"]
         row_cells = table.add_row().cells
         row_cells[0].text = str(field.title)
         row_cells[1].text = (
             formatDate(request, company.submit_date)
             if company and company.submit_date
@@ -185,15 +185,14 @@
     def compile(self, data):
         """"""
         self.set_session_title_row(data)
         self.set_body(data, show_risk_state=True, always_print_description=True)
 
 
 class RIEActionPlanDocxView(ActionPlanDocxView):
-
     _compiler = RIEDocxCompiler
 
     def get_data(self, for_download=False):
         """Gets the data structure in a format suitable for `DocxCompiler`"""
         session = self.context.session
 
         data = {
@@ -207,37 +206,36 @@
             ],
         }
         return data
 
 
 class RIEIdentificationReportCompiler(RIEDocxCompiler):
     def set_session_title_row(self, data):
-
         request = self.request
         doc = self.template
 
         # Remove existing paragraphs
         for paragraph in doc.paragraphs:
             delete_paragraph(paragraph)
 
         header = doc.sections[0].header
         h_table = header.tables[0]
         h_table.cell(0, 0).paragraphs[0].text = data["heading"]
-        h_table.cell(0, 1).paragraphs[0].text = u"Datum download: {}".format(
+        h_table.cell(0, 1).paragraphs[0].text = "Datum download: {}".format(
             formatDate(request, date.today())
         )
 
         # doc.paragraphs[0].text = data['heading']
 
         survey = aq_parent(self.context)
         footer_txt = self.t(
             _(
                 "report_survey_revision",
-                default=u"This document was based on the OiRA Tool '${title}' "
-                u"of revision date ${date}.",
+                default="This document was based on the OiRA Tool '${title}' "
+                "of revision date ${date}.",
                 mapping={
                     "title": survey.published[1],
                     "date": formatDate(request, survey.published[2]),
                 },
             )
         )
         footer = doc.sections[0].footer
@@ -257,15 +255,14 @@
             skip_legal_references=False,
             skip_existing_measures=True,
             skip_planned_measures=True,
         )
 
 
 class RIEIdentificationReportDocxView(IdentificationReportDocxView):
-
     _compiler = RIEIdentificationReportCompiler
 
     def get_data(self, for_download=False):
         """Gets the data structure in a format suitable for `DocxCompiler`"""
         session = self.context.session
 
         data = {
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/overrides/euphorie.client.browser.templates.conditions-bare.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/overrides/euphorie.client.browser.templates.conditions-bare.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/session.py` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 from zope.i18nmessageid import MessageFactory
 
 
 PloneLocalesFactory = MessageFactory("plonelocales")
 
 
 class ActionPlanView(session.ActionPlanView):
-
     question_filter = sql.or_(
         model.MODULE_WITH_RISK_TOP5_TNO_FILTER,
         model.RISK_PRESENT_FILTER_TOP5_TNO_FILTER,
     )
     risk_filter = model.RISK_PRESENT_FILTER_TOP5_TNO_FILTER
 
 
 class Status(session.Status):
-
     show_high_risks = False
 
 
 class Start(session.Start):
     @property
     @memoize
     def sector(self):
@@ -66,18 +64,18 @@
                 callable(getattr(self.context, "Title", None))
                 and self.context.Title()
                 or ""
             )
         today = date.today()
         this_month = date(today.year, today.month, 1)
         self.label_page = translate(
-            _(u"label_page", default=u"Page"), target_language=lang
+            _("label_page", default="Page"), target_language=lang
         )
         self.label_page_of = translate(
-            _(u"label_page_of", default=u"of"), target_language=lang
+            _("label_page_of", default="of"), target_language=lang
         )
 
         def get_next_month(this_month):
             month = this_month.month + 1
             year = this_month.year
             if month == 13:
                 month = 1
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/measures_overview.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/measures_overview.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/report_company.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/report_company.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/report_landing.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/report_landing.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/browser/templates/rie.docx` & `tno.euphorie-9.0.5/src/tno/euphorie/client/browser/templates/rie.docx`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/client/client.py` & `tno.euphorie-9.0.5/src/tno/euphorie/client/client.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/configure.zcml` & `tno.euphorie-9.0.5/src/tno/euphorie/configure.zcml`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/content/browser/templates/survey_view.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/content/browser/templates/survey_view.pt`

 * *Files 11% similar despite different names*

```diff
@@ -44,20 +44,20 @@
 
       <tal:intro condition="python:context.introduction">
         <h2 i18n:translate="label_introduction">Introduction text</h2>
         <p tal:replace="structure context/introduction"></p>
       </tal:intro>
 
       <h2 i18n:translate="header_modules_and_profile_questions">Modules and Profile Questions</h2>
-      <p tal:condition="python:not view.children"
+      <p tal:condition="python:not view.modules_and_profile_questions"
          i18n:translate="no_profile_questions_or_modules"
       >This survey has no profile questions or modules.</p>
-      <tal:children condition="python:view.children">
-        <ol class="${python:'sortable' if can_edit and len(view.children)&gt;1 else None}">
+      <tal:children condition="python:view.modules_and_profile_questions">
+        <ol class="${python:'sortable' if can_edit and len(view.modules_and_profile_questions)&gt;1 else None}">
           <li id="child-${child/id}"
-              tal:repeat="child view/children"
+              tal:repeat="child view/modules_and_profile_questions"
           ><a href="${child/url}">${child/title}</a></li>
         </ol>
       </tal:children>
     </metal:content>
   </body>
 </html>
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/interfaces.py` & `tno.euphorie-9.0.5/src/tno/euphorie/interfaces.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/locales/nl/LC_MESSAGES/euphorie.po` & `tno.euphorie-9.0.5/src/tno/euphorie/locales/nl/LC_MESSAGES/euphorie.po`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/model.py` & `tno.euphorie-9.0.5/src/tno/euphorie/model.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/nuplone/configure.zcml` & `tno.euphorie-9.0.5/src/tno/euphorie/nuplone/configure.zcml`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/error_unauthorized.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/error_unauthorized.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/largetextarea_input.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/largetextarea_input.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/nuplone/templates/wysiwyg_input.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/nuplone/templates/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/nuplone/widget.py` & `tno.euphorie-9.0.5/src/tno/euphorie/nuplone/widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return FieldWidget(field, widget(request))
 
 
 @implementer_only(ILargeTextAreaWidget)
 class LargeTextAreaWidget(TextAreaWidget, Widget):
     """Textarea widget implementation."""
 
-    klass = u"textarea-widget"
-    value = u""
+    klass = "textarea-widget"
+    value = ""
 
 
 @adapter(IText, ITnoContentSkinLayer)
 @implementer(IFieldWidget)
 def LargeTextAreaFieldWidget(field, request):
     return FieldWidget(field, LargeTextAreaWidget(request))
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/schema.py` & `tno.euphorie-9.0.5/src/tno/euphorie/schema.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/templates/upload.pt` & `tno.euphorie-9.0.5/src/tno/euphorie/templates/upload.pt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/testing.py` & `tno.euphorie-9.0.5/src/tno/euphorie/testing.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_company.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_module.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_report.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
         return formatAddress(*a, **kw)
 
     def testEmptyAddress(self):
         self.assertEqual(self.formatAddress(None, None, None), None)
 
     def testAddressOnly(self):
-        self.assertEqual(self.formatAddress(u"Street", None, None), u"Street")
+        self.assertEqual(self.formatAddress("Street", None, None), "Street")
 
     def testPostalOnly(self):
-        self.assertEqual(self.formatAddress(None, u"Postal", None), u"Postal")
+        self.assertEqual(self.formatAddress(None, "Postal", None), "Postal")
 
     def testPostalAndCity(self):
-        self.assertEqual(self.formatAddress(None, u"Postal", u"City"), u"Postal City")
+        self.assertEqual(self.formatAddress(None, "Postal", "City"), "Postal City")
 
     def testFull(self):
         self.assertEqual(
-            self.formatAddress(u"Street", u"Postal", u"City"), u"Street\nPostal City"
+            self.formatAddress("Street", "Postal", "City"), "Street\nPostal City"
         )
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_risk.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_risk.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_session.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.assertEqual(self.attr_date(node, "date"), None)
         marker = []
         self.assertTrue(self.attr_date(node, "date", marker) is marker)
 
     def testEmptyValue(self):
         from lxml import etree
 
-        node = etree.Element("node", date=u"")
+        node = etree.Element("node", date="")
         self.assertEqual(self.attr_date(node, "date"), None)
 
 
 class UploadTests(testing.TnoEuphorieTestCase):
     BASE_SNIPPET = """
             <rieprogress>
               <gegevens
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/tests/test_survey.py` & `tno.euphorie-9.0.5/src/tno/euphorie/tests/test_survey.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/env.py` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/versions/203_.py` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/versions/203_.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     op.add_column("session", sa.Column("refreshed", sa.DateTime(), nullable=True))
     op.execute("UPDATE session SET refreshed = modified")
     op.add_column("risk", sa.Column("image_data", sa.LargeBinary(), nullable=True))
     op.add_column(
         "risk", sa.Column("image_data_scaled", sa.LargeBinary(), nullable=True)
     )
     op.add_column("risk", sa.Column("image_filename", sa.UnicodeText(), nullable=True))
-    op.drop_constraint(u"session_last_publisher_id_fkey", "session", type_="foreignkey")
-    op.drop_constraint(u"session_last_modifier_id_fkey", "session", type_="foreignkey")
+    op.drop_constraint("session_last_publisher_id_fkey", "session", type_="foreignkey")
+    op.drop_constraint("session_last_modifier_id_fkey", "session", type_="foreignkey")
     op.create_foreign_key(
         None,
         "session",
         "account",
         ["last_modifier_id"],
         ["id"],
         onupdate="CASCADE",
```

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/alembic/versions/204_.py` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/alembic/versions/204_.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/configure.zcml` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/configure.zcml`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/to_204/registry.xml` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/to_204/registry.xml`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/v1.py` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/v1.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno/euphorie/upgrade/v2.py` & `tno.euphorie-9.0.5/src/tno/euphorie/upgrade/v2.py`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/src/tno.euphorie.egg-info/PKG-INFO` & `tno.euphorie-9.0.5/src/tno.euphorie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.euphorie
-Version: 9.0.4
+Version: 9.0.5
 Summary: TNO specific extensions for Euphorie
 Home-page: http://readthedocs.org/docs/tnoeuphorie/en/latest/
 Author: Wichert Akkerman and Syslab.com
 Author-email: info@syslab.com
 License: GPL
 Keywords: Euphorie OIRA RIE
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,28 @@
 If you do not already have Euphorie installed it will be installed
 automatically.
 
 
 Changelog
 =========
 
+9.0.5 (2023-03-22)
+------------------
+
+- Adapt the survey-view template to the latest Euphorie
+  [ale-rt]
+- Fix for prioritiy risks being displayed though they were answered N/A.
+  https://github.com/syslabcom/scrum/issues/1020
+  [reinhardt]
+- Fix the ``@@plan_van_aanpak.docx`` report to display some numerical number as zeros and not
+  as not provided values.
+  Fixes `#1054 <https://github.com/syslabcom/scrum/issues/1054>`_
+  [ale-rt]
+
+
 9.0.4 (2023-02-28)
 ------------------
 
 - Add custom terms of service and condition (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
 - Hide the organisation tab (https://github.com/syslabcom/scrum/issues/519)
   [ale-rt]
@@ -181,15 +195,15 @@
 - Switch to Plone5
 
 
 6.0.15 (2018-07-13)
 -------------------
 
 - Bugfix for the "measures" report: Do not rely on the pre-computed
-  list of modules, since this can fail for a scenario with 
+  list of modules, since this can fail for a scenario with
   module->module->Optional module
 
 6.0.14 (2017-11-01)
 -------------------
 
 - Another bugfix for the "measures" report. Correctly compute the
   future months
```

### Comparing `tno.euphorie-9.0.4/src/tno.euphorie.egg-info/SOURCES.txt` & `tno.euphorie-9.0.5/src/tno.euphorie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tno.euphorie-9.0.4/templates/euphorie.ini` & `tno.euphorie-9.0.5/templates/euphorie.ini`

 * *Files identical despite different names*

