# Comparing `tmp/oslo.log-5.4.0.tar.gz` & `tmp/oslo.log-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.log-5.4.0.tar", last modified: Tue Nov 14 09:58:27 2023, max compression
+gzip compressed data, was "oslo.log-5.5.0.tar", last modified: Thu Feb 22 20:10:53 2024, max compression
```

## Comparing `oslo.log-5.4.0.tar` & `oslo.log-5.5.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-11-14 09:58:01.000000 oslo.log-5.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-11-14 09:58:01.000000 oslo.log-5.4.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-11-14 09:58:01.000000 oslo.log-5.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-11-14 09:58:01.000000 oslo.log-5.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2023-11-14 09:58:01.000000 oslo.log-5.4.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7423 2023-11-14 09:58:27.000000 oslo.log-5.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-11-14 09:58:01.000000 oslo.log-5.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28714 2023-11-14 09:58:27.000000 oslo.log-5.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-11-14 09:58:01.000000 oslo.log-5.4.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-11-14 09:58:01.000000 oslo.log-5.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2312 2023-11-14 09:58:27.883485 oslo.log-5.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2023-11-14 09:58:01.000000 oslo.log-5.4.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/advanced_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/example_nova.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/journal.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/log_rotation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/admin/nova_sample.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4456 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/fixtures.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/formatters.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/handlers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/helpers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/log.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/versionutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/reference/watchers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/doc/source/user/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/doc/source/user/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/oslo_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/python_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/usage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/usage_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples/usage_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/examples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11454 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/guidelines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2023-11-14 09:58:01.000000 oslo.log-5.4.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo.log.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2312 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4699 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-11-14 09:58:27.000000 oslo.log-5.4.0/oslo.log.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11091 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/_options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/cmds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/cmds/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/cmds/convert_json.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/fixture/logging_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/fixture/setlevel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21644 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/oslo_log/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/oslo_log/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/oslo_log/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/oslo_log/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/oslo_log/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19417 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/pipe_mutex.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4762 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/rate_limit.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.879485 oslo.log-5.4.0/oslo_log/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/oslo_log/tests/unit/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/fixture/test_logging_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/fixture/test_setlevel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_convert_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_custom_loghandler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    79067 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6603 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_pipe_mutex.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_rate_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14051 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/tests/unit/test_versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10409 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2023-11-14 09:58:01.000000 oslo.log-5.4.0/oslo_log/watchers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/add-context-section-0b2f411ec64f42f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/add-facility-to-journal-e10bf7002cc19dd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/add-reno-e4fedb11ece56f1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/add-system_scope-to-logging_user_identity_format-0581ce5070740375.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/always-add-error-text-715022964364ffa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/deprecate-windows-support-75e6ac72310d5e72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/drop-python27-support-0fe4909a5468feb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/info-logging-7b7be9fc7a95aebc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/init-global-request-id-eb2031bc221e5fb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/is_debug_enabled-d7afee4c811a46df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/jsonformatter-repr-fd616eb6fa6caeb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/log-global_request_id-f97e6d663e8a80b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/log-rotation-595f8232cd987a6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/native-threads-logging-cc84f7288c4835a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/reload_log_config-743817192b1172b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/remove-log-format-b4b949701cee3315.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/remove-syslog-rfc-format-7a06772c0bb48e9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/remove-verbose-option-d0d1381e182d1be1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/systemd-journal-support-fcbc34b3c5ce93ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/use-json-option-96f71da54a3b9a18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/use-project-in-user-identity-93fd6e0a2e434a6f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/use_stderr_default_false-50d846b88cf2be90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/notes/windows-eventlog-2beb0a6010e342eb.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10458 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.875485 oslo.log-5.4.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-14 09:58:27.883485 oslo.log-5.4.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-14 09:58:01.000000 oslo.log-5.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-11-14 09:58:01.000000 oslo.log-5.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2023-11-14 09:58:27.887485 oslo.log-5.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-11-14 09:58:01.000000 oslo.log-5.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2023-11-14 09:58:01.000000 oslo.log-5.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2023-11-14 09:58:01.000000 oslo.log-5.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-02-22 20:10:17.000000 oslo.log-5.5.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-02-22 20:10:17.000000 oslo.log-5.5.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2024-02-22 20:10:17.000000 oslo.log-5.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-02-22 20:10:17.000000 oslo.log-5.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2024-02-22 20:10:17.000000 oslo.log-5.5.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7468 2024-02-22 20:10:53.000000 oslo.log-5.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-02-22 20:10:17.000000 oslo.log-5.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28842 2024-02-22 20:10:53.000000 oslo.log-5.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-22 20:10:17.000000 oslo.log-5.5.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-02-22 20:10:17.000000 oslo.log-5.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-02-22 20:10:53.970188 oslo.log-5.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-02-22 20:10:17.000000 oslo.log-5.5.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/advanced_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/example_nova.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/journal.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/log_rotation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/admin/nova_sample.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4456 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.950188 oslo.log-5.5.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/fixtures.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/formatters.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/handlers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/helpers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/log.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/versionutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/reference/watchers.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.954188 oslo.log-5.5.0/doc/source/user/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.954188 oslo.log-5.5.0/doc/source/user/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/oslo_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/python_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/usage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/usage_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples/usage_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/examples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11454 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2024-02-22 20:10:17.000000 oslo.log-5.5.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.954188 oslo.log-5.5.0/oslo.log.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4699 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-02-22 20:10:53.000000 oslo.log-5.5.0/oslo.log.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11091 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/_options.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/cmds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/cmds/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/cmds/convert_json.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/fixture/logging_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/fixture/setlevel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21644 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.942188 oslo.log-5.5.0/oslo_log/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.942188 oslo.log-5.5.0/oslo_log/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.942188 oslo.log-5.5.0/oslo_log/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.942188 oslo.log-5.5.0/oslo_log/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.958188 oslo.log-5.5.0/oslo_log/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.942188 oslo.log-5.5.0/oslo_log/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.962188 oslo.log-5.5.0/oslo_log/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19417 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/pipe_mutex.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4762 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/rate_limit.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.962188 oslo.log-5.5.0/oslo_log/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.962188 oslo.log-5.5.0/oslo_log/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.962188 oslo.log-5.5.0/oslo_log/tests/unit/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/fixture/test_logging_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/fixture/test_setlevel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_convert_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_custom_loghandler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79067 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6603 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_pipe_mutex.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_rate_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14051 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/tests/unit/test_versionutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10409 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/versionutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2024-02-22 20:10:17.000000 oslo.log-5.5.0/oslo_log/watchers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.946188 oslo.log-5.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.966188 oslo.log-5.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/add-context-section-0b2f411ec64f42f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/add-facility-to-journal-e10bf7002cc19dd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/add-reno-e4fedb11ece56f1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/add-system_scope-to-logging_user_identity_format-0581ce5070740375.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/always-add-error-text-715022964364ffa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/deprecate-windows-support-75e6ac72310d5e72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/drop-python27-support-0fe4909a5468feb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/info-logging-7b7be9fc7a95aebc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/init-global-request-id-eb2031bc221e5fb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/is_debug_enabled-d7afee4c811a46df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/jsonformatter-repr-fd616eb6fa6caeb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/log-global_request_id-f97e6d663e8a80b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/log-rotation-595f8232cd987a6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/native-threads-logging-cc84f7288c4835a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/reload_log_config-743817192b1172b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/remove-log-format-b4b949701cee3315.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/remove-syslog-rfc-format-7a06772c0bb48e9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/remove-verbose-option-d0d1381e182d1be1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/systemd-journal-support-fcbc34b3c5ce93ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/use-json-option-96f71da54a3b9a18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/use-project-in-user-identity-93fd6e0a2e434a6f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/use_stderr_default_false-50d846b88cf2be90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/notes/windows-eventlog-2beb0a6010e342eb.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.946188 oslo.log-5.5.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.946188 oslo.log-5.5.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10458 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.946188 oslo.log-5.5.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 20:10:53.970188 oslo.log-5.5.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 20:10:17.000000 oslo.log-5.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-02-22 20:10:17.000000 oslo.log-5.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2024-02-22 20:10:53.974188 oslo.log-5.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 20:10:17.000000 oslo.log-5.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-02-22 20:10:17.000000 oslo.log-5.5.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2024-02-22 20:10:17.000000 oslo.log-5.5.0/tox.ini
```

### Comparing `oslo.log-5.4.0/.zuul.yaml` & `oslo.log-5.5.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/AUTHORS` & `oslo.log-5.5.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 Stanislav Kudriashev <skudriashev@griddynamics.com>
 Stephen Finucane <sfinucan@redhat.com>
 Stephen Finucane <stephenfin@redhat.com>
 Steve Martinelli <s.martinelli@gmail.com>
 Steve Martinelli <stevemar@ca.ibm.com>
 Stuart McLaren <stuart.mclaren@hp.com>
 Suff <dmitry.a.grachev@gmail.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Thomas Herve <therve@redhat.com>
 Thomas Herve <thomas.herve@enovance.com>
 Timur Sufiev <tsufiev@mirantis.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Tony Xu <hhktony@gmail.com>
```

### Comparing `oslo.log-5.4.0/CONTRIBUTING.rst` & `oslo.log-5.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/ChangeLog` & `oslo.log-5.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+5.5.0
+-----
+
+* pre-commit: Integrate bandit
+* pre-commit: Bump versions
+* Bump hacking
+* Update python classifier in setup.cfg
+
 5.4.0
 -----
 
 * Deprecate Windows support
 * Update master for stable/2023.2
 
 5.3.0
```

### Comparing `oslo.log-5.4.0/LICENSE` & `oslo.log-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/PKG-INFO` & `oslo.log-5.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.log
-Version: 5.4.0
+Version: 5.5.0
 Summary: oslo.log library
 Home-page: https://docs.openstack.org/oslo.log/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -46,13 +46,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Provides-Extra: fixtures
 Provides-Extra: systemd
 Provides-Extra: test
```

### Comparing `oslo.log-5.4.0/README.rst` & `oslo.log-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/admin/advanced_config.rst` & `oslo.log-5.5.0/doc/source/admin/advanced_config.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/admin/example_nova.rst` & `oslo.log-5.5.0/doc/source/admin/example_nova.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/admin/journal.rst` & `oslo.log-5.5.0/doc/source/admin/journal.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/admin/log_rotation.rst` & `oslo.log-5.5.0/doc/source/admin/log_rotation.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/admin/nova_sample.conf` & `oslo.log-5.5.0/doc/source/admin/nova_sample.conf`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/conf.py` & `oslo.log-5.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/configuration/index.rst` & `oslo.log-5.5.0/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/index.rst` & `oslo.log-5.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/_i18n.py` & `oslo.log-5.5.0/doc/source/user/examples/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/oslo_logging.py` & `oslo.log-5.5.0/doc/source/user/examples/oslo_logging.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/python_logging.py` & `oslo.log-5.5.0/doc/source/user/examples/python_logging.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/usage.py` & `oslo.log-5.5.0/doc/source/user/examples/usage.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/usage_context.py` & `oslo.log-5.5.0/doc/source/user/examples/usage_context.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples/usage_helper.py` & `oslo.log-5.5.0/doc/source/user/examples/usage_helper.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/examples.rst` & `oslo.log-5.5.0/doc/source/user/examples.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/guidelines.rst` & `oslo.log-5.5.0/doc/source/user/guidelines.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/doc/source/user/usage.rst` & `oslo.log-5.5.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo.log.egg-info/PKG-INFO` & `oslo.log-5.5.0/oslo.log.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.log
-Version: 5.4.0
+Version: 5.5.0
 Summary: oslo.log library
 Home-page: https://docs.openstack.org/oslo.log/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -46,13 +46,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Provides-Extra: fixtures
 Provides-Extra: systemd
 Provides-Extra: test
```

### Comparing `oslo.log-5.4.0/oslo.log.egg-info/SOURCES.txt` & `oslo.log-5.5.0/oslo.log.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/_i18n.py` & `oslo.log-5.5.0/oslo_log/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/_options.py` & `oslo.log-5.5.0/oslo_log/_options.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/cmds/convert_json.py` & `oslo.log-5.5.0/oslo_log/cmds/convert_json.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/fixture/__init__.py` & `oslo.log-5.5.0/oslo_log/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/fixture/logging_error.py` & `oslo.log-5.5.0/oslo_log/fixture/logging_error.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/fixture/setlevel.py` & `oslo.log-5.5.0/oslo_log/fixture/setlevel.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/formatters.py` & `oslo.log-5.5.0/oslo_log/formatters.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/handlers.py` & `oslo.log-5.5.0/oslo_log/handlers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/helpers.py` & `oslo.log-5.5.0/oslo_log/helpers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po` & `oslo.log-5.5.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po` & `oslo.log-5.5.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po` & `oslo.log-5.5.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po` & `oslo.log-5.5.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/log.py` & `oslo.log-5.5.0/oslo_log/log.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/pipe_mutex.py` & `oslo.log-5.5.0/oslo_log/pipe_mutex.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/rate_limit.py` & `oslo.log-5.5.0/oslo_log/rate_limit.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/__init__.py` & `oslo.log-5.5.0/oslo_log/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/fixture/__init__.py` & `oslo.log-5.5.0/oslo_log/tests/unit/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/fixture/test_logging_error.py` & `oslo.log-5.5.0/oslo_log/tests/unit/fixture/test_logging_error.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/fixture/test_setlevel.py` & `oslo.log-5.5.0/oslo_log/tests/unit/fixture/test_setlevel.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_convert_json.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_convert_json.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_custom_loghandler.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_custom_loghandler.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_formatters.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_helpers.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_log.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_pipe_mutex.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_pipe_mutex.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_rate_limit.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_rate_limit.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/tests/unit/test_versionutils.py` & `oslo.log-5.5.0/oslo_log/tests/unit/test_versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/version.py` & `oslo.log-5.5.0/oslo_log/version.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/versionutils.py` & `oslo.log-5.5.0/oslo_log/versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/oslo_log/watchers.py` & `oslo.log-5.5.0/oslo_log/watchers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/releasenotes/source/conf.py` & `oslo.log-5.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.log-5.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.log-5.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/setup.cfg` & `oslo.log-5.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	oslo_log
```

### Comparing `oslo.log-5.4.0/setup.py` & `oslo.log-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.4.0/tox.ini` & `oslo.log-5.5.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,18 @@
   -r{toxinidir}/test-requirements.txt
 commands =
   find . -type f -name "*.pyc" -delete
   stestr run {posargs}
   stestr slowest
 
 [testenv:pep8]
+deps =
+  pre-commit
 commands =
   pre-commit run -a
-  # Run security linter
-  bandit -r oslo_log -x tests -n5
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 allowlist_externals = rm
 deps =
@@ -47,17 +47,14 @@
   coverage erase
   {[testenv]commands}
   coverage combine
   coverage html -d cover
   coverage xml -o cover/coverage.xml
   coverage report --show-missing
 
-[testenv:bandit]
-commands = bandit -r oslo_log -x tests -n5
-
 [flake8]
 # E123, E125 skipped as they are invalid PEP-8.
 # W503, W504 skipped: https://www.python.org/dev/peps/pep-0008/#should-a-line-break-before-or-after-a-binary-operator
 show-source = True
 ignore = E123,E125,H405,W503,W504
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build,__init__.py
```

