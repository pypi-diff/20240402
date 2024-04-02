# Comparing `tmp/invenio-formatter-2.0.2.tar.gz` & `tmp/invenio-formatter-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-formatter-2.0.2.tar", last modified: Thu Feb  1 13:30:19 2024, max compression
+gzip compressed data, was "dist/invenio-formatter-2.0.3.tar", last modified: Tue Apr  2 12:20:31 2024, max compression
```

## Comparing `invenio-formatter-2.0.2.tar` & `invenio-formatter-2.0.3.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/examples/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/context_processors/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/context_processors/badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/filters/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/filters/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/invenio_formatter/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 13:30:18.000000 invenio-formatter-2.0.2/invenio_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      577 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:30:19.000000 invenio-formatter-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_invenio_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_template_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-01 13:30:11.000000 invenio-formatter-2.0.2/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/examples/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/context_processors/badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/filters/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/filters/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/invenio_formatter/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 12:20:30.000000 invenio-formatter-2.0.3/invenio_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      577 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:20:31.000000 invenio-formatter-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_invenio_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_template_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-02 12:20:21.000000 invenio-formatter-2.0.3/tests/test_views.py
```

### Comparing `invenio-formatter-2.0.2/.editorconfig` & `invenio-formatter-2.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/.github/workflows/pypi-publish.yml` & `invenio-formatter-2.0.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/.github/workflows/tests.yml` & `invenio-formatter-2.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/.tx/config` & `invenio-formatter-2.0.3/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/CHANGES.rst` & `invenio-formatter-2.0.3/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.0.3 (released 2024-04-02)
+
+- escaped badge title and value on svg generation
+
 Version 2.0.2 (released 2024-02-01)
 
 - templates: replace reStructedText with reStructuredText
 
 Version 2.0.1 (released 2023-07-26)
 
 - badges: semantic html Fixes
```

### Comparing `invenio-formatter-2.0.2/CONTRIBUTING.rst` & `invenio-formatter-2.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/INSTALL.rst` & `invenio-formatter-2.0.3/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/LICENSE` & `invenio-formatter-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/MANIFEST.in` & `invenio-formatter-2.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/PKG-INFO` & `invenio-formatter-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 2.0.2
+Version: 2.0.3
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.3 (released 2024-04-02)
+        
+        - escaped badge title and value on svg generation
+        
         Version 2.0.2 (released 2024-02-01)
         
         - templates: replace reStructedText with reStructuredText
         
         Version 2.0.1 (released 2023-07-26)
         
         - badges: semantic html Fixes
```

### Comparing `invenio-formatter-2.0.2/README.rst` & `invenio-formatter-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/docs/Makefile` & `invenio-formatter-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/docs/api.rst` & `invenio-formatter-2.0.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/docs/conf.py` & `invenio-formatter-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/docs/index.rst` & `invenio-formatter-2.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/docs/make.bat` & `invenio-formatter-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/examples/app.py` & `invenio-formatter-2.0.3/examples/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 
     $ open http://127.0.0.1:5000/
 
 SPHINX-END
 
 """
 
-from __future__ import absolute_import, print_function
-
 import base64
 import datetime
 from os.path import dirname, join
 
 import jinja2
 from flask import Flask, render_template
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/__init__.py` & `invenio-formatter-2.0.3/invenio_formatter/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,12 @@
          title='isbn', value='9780399547331', ext='svg') }}"></img>
 
 Your badge will be visible on the page as before, and also directly accessible
 at `http://localhost:5000/badge/ISBN/9780399547331.svg
 <http://localhost:5000/badge/ISBN/9780399547331.svg>`_.
 """
 
-from __future__ import absolute_import, print_function
-
 from .ext import InvenioFormatter
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 __all__ = ("__version__", "InvenioFormatter")
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/config.py` & `invenio-formatter-2.0.3/invenio_formatter/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2016-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Configuration for Invenio-Formatter."""
 
-from __future__ import absolute_import, print_function
-
 FORMATTER_BADGES_ALLOWED_TITLES = ["DOI"]
 """List of allowed titles in badges."""
 
 FORMATTER_BADGES_TITLE_MAPPING = {}
 """Mapping of titles."""
 
 FORMATTER_BADGES_MAX_CACHE_AGE = 0
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/context_processors/badges.py` & `invenio-formatter-2.0.3/invenio_formatter/context_processors/badges.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 # Copyright (C) 2016-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Badges context processor."""
 
-from __future__ import absolute_import, print_function
-
+import html
 from base64 import b64encode
 
 import cairosvg
 from PIL import Image, ImageDraw, ImageFont
 
 
 def get_text_length(*args):
@@ -35,14 +34,16 @@
     """Generate the SVG.
 
     :param title: The badge title.
     :param value: The badge content.
     :param color: The badge color. (Default: ``'#007ec6'``)
     :returns: The SVG badge.
     """
+    title = html.escape(title)
+    value = html.escape(value)
     (title_length, value_length) = get_text_length(title, value)
     return """<svg xmlns="http://www.w3.org/2000/svg"
      width="{width}" height="20">
         <linearGradient id="b" x2="0" y2="100%">
             <stop offset="0" stop-color="#bbb" stop-opacity=".1"/>
             <stop offset="1" stop-opacity=".1"/>
         </linearGradient>
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/ext.py` & `invenio-formatter-2.0.3/invenio_formatter/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Jinja utilities for Invenio."""
 
-from __future__ import absolute_import, print_function
-
 from pkg_resources import DistributionNotFound, get_distribution
 
 from . import config
 from .filters.datetime import (
     format_arrow,
     from_isodate,
     from_isodatetime,
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/filters/datetime.py` & `invenio-formatter-2.0.3/invenio_formatter/filters/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Datetime Jinja filters."""
 
-from __future__ import absolute_import, print_function
-
 import arrow
 from flask_babel import to_user_timezone
 
 
 def from_isodate(value, strict=False):
     """Convert an ISO formatted date into a Date object.
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter/filters/html.py` & `invenio-formatter-2.0.3/invenio_formatter/filters/html.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/macros/badges.html` & `invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/macros/badges.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/templates/invenio_formatter/macros/meta.html` & `invenio-formatter-2.0.3/invenio_formatter/templates/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html` & `invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html` & `invenio-formatter-2.0.3/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/af/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/af/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ar/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/bg/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ca/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/cs/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/da/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/da/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/el/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/el/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/en/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/et/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/et/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fa/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/gl/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hu/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/it/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/it/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ja/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ka/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/lt/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/messages.pot` & `invenio-formatter-2.0.3/invenio_formatter/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ne/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/no/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/no/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/pl/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/pt/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ro/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/ru/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/rw/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sk/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sv/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/tr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/uk/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.3/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/invenio_formatter/views.py` & `invenio-formatter-2.0.3/invenio_formatter/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """View method for Invenio-Formatter."""
 
-from __future__ import absolute_import, print_function
-
 import hashlib
 from datetime import datetime as dt
 from datetime import timedelta
 
 from flask import Blueprint, Response, current_app, request
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter.egg-info/PKG-INFO` & `invenio-formatter-2.0.3/invenio_formatter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 2.0.2
+Version: 2.0.3
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.3 (released 2024-04-02)
+        
+        - escaped badge title and value on svg generation
+        
         Version 2.0.2 (released 2024-02-01)
         
         - templates: replace reStructedText with reStructuredText
         
         Version 2.0.1 (released 2023-07-26)
         
         - badges: semantic html Fixes
```

### Comparing `invenio-formatter-2.0.2/invenio_formatter.egg-info/SOURCES.txt` & `invenio-formatter-2.0.3/invenio_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/run-tests.sh` & `invenio-formatter-2.0.3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/setup.cfg` & `invenio-formatter-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/tests/conftest.py` & `invenio-formatter-2.0.3/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 """Pytest configuration."""
 
-from __future__ import absolute_import, print_function
-
 import pytest
 from flask import Flask
 from invenio_i18n import InvenioI18N
 
 from invenio_formatter import InvenioFormatter
```

### Comparing `invenio-formatter-2.0.2/tests/test_examples_app.py` & `invenio-formatter-2.0.3/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.2/tests/test_filters.py` & `invenio-formatter-2.0.3/tests/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for Jinja2 filters."""
 
-from __future__ import absolute_import, print_function
-
 from datetime import date, datetime
 
 import arrow
 import pytest
 from arrow.parser import ParserError
 from flask import render_template_string
```

### Comparing `invenio-formatter-2.0.2/tests/test_invenio_formatter.py` & `invenio-formatter-2.0.3/tests/test_invenio_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module tests."""
 
-from __future__ import absolute_import, print_function
-
 from flask import Flask
 from mock import patch
 from pkg_resources import DistributionNotFound
 
 from invenio_formatter import InvenioFormatter
```

### Comparing `invenio-formatter-2.0.2/tests/test_template_context_processors.py` & `invenio-formatter-2.0.3/tests/test_template_context_processors.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for template context processors."""
 
-from __future__ import absolute_import, print_function
-
 from flask import render_template_string
 
 
 def test_context_processor_badge_svg(app):
     """Test context processor badge generating a SVG."""
     template = r"""
     {{ badge_svg('DOI','10.1234/zenodo.12345')|safe }}
```

### Comparing `invenio-formatter-2.0.2/tests/test_template_macros.py` & `invenio-formatter-2.0.3/tests/test_template_macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for Jinja2 filters."""
 
-from __future__ import absolute_import, print_function
-
 from datetime import date
 
 from flask import render_template_string
 
 
 def test_meta_twittercard(app):
     """Test macro meta_twittercard."""
```

### Comparing `invenio-formatter-2.0.2/tests/test_views.py` & `invenio-formatter-2.0.3/tests/test_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for template context processors."""
 
-from __future__ import absolute_import, print_function
-
 from flask import Flask
 
 from invenio_formatter import InvenioFormatter
 
 
 def test_views_badge_svg(app):
     """Test context processor badge generating a SVG."""
```

