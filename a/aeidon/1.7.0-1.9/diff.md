# Comparing `tmp/aeidon-1.7.0.tar.gz` & `tmp/aeidon-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeidon-1.7.0.tar", last modified: Sun Jan 26 13:33:59 2020, max compression
+gzip compressed data, was "aeidon-1.9.tar", last modified: Thu Dec 31 16:42:17 2020, max compression
```

## Comparing `aeidon-1.7.0.tar` & `aeidon-1.9.tar`

### file list

```diff
@@ -1,123 +1,118 @@
--rw-r--r--   0        0        0     4978 2020-01-26 13:07:32.656387 aeidon-1.7.0/aeidon/__init__.py
--rw-r--r--   0        0        0     1322 2020-01-26 13:07:32.668388 aeidon-1.7.0/aeidon/agents/__init__.py
--rw-r--r--   0        0        0     2394 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/clipboard.py
--rw-r--r--   0        0        0     7452 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/edit.py
--rw-r--r--   0        0        0     6947 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/format.py
--rw-r--r--   0        0        0     8370 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/open.py
--rw-r--r--   0        0        0     8178 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/position.py
--rw-r--r--   0        0        0     4474 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/preview.py
--rw-r--r--   0        0        0     8250 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/register.py
--rw-r--r--   0        0        0     4320 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/save.py
--rw-r--r--   0        0        0    11284 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/search.py
--rw-r--r--   0        0        0     5396 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/set.py
--rw-r--r--   0        0        0        0 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/__init__.py
--rw-r--r--   0        0        0     1457 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_clipboard.py
--rw-r--r--   0        0        0     4460 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/test/test_edit.py
--rw-r--r--   0        0        0     9457 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_format.py
--rw-r--r--   0        0        0     2504 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_open.py
--rw-r--r--   0        0        0     6042 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_position.py
--rw-r--r--   0        0        0     2463 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_register.py
--rw-r--r--   0        0        0     1831 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_save.py
--rw-r--r--   0        0        0     4015 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_search.py
--rw-r--r--   0        0        0     2672 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/agents/test/test_set.py
--rw-r--r--   0        0        0     4178 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/agents/test/test_text.py
--rw-r--r--   0        0        0    15441 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/agents/text.py
--rw-r--r--   0        0        0     6026 2019-07-07 02:12:49.339339 aeidon-1.7.0/aeidon/agents/util.py
--rw-r--r--   0        0        0     8945 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/calculator.py
--rw-r--r--   0        0        0     1943 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/clipboard.py
--rw-r--r--   0        0        0     2622 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/containers.py
--rw-r--r--   0        0        0     2043 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/countries.py
--rw-r--r--   0        0        0     8146 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/deco.py
--rw-r--r--   0        0        0     1485 2017-08-29 00:51:52.157788 aeidon-1.7.0/aeidon/delegate.py
--rw-r--r--   0        0        0    11132 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/encodings.py
--rw-r--r--   0        0        0     3494 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/enum.py
--rw-r--r--   0        0        0     9561 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/enums.py
--rw-r--r--   0        0        0     1739 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/errors.py
--rw-r--r--   0        0        0     6122 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/file.py
--rw-r--r--   0        0        0     1728 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/__init__.py
--rw-r--r--   0        0        0     1999 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/ass.py
--rw-r--r--   0        0        0     2652 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/lrc.py
--rw-r--r--   0        0        0     2245 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/microdvd.py
--rw-r--r--   0        0        0     2087 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/mpl2.py
--rw-r--r--   0        0        0     5726 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/ssa.py
--rw-r--r--   0        0        0     4011 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/subrip.py
--rw-r--r--   0        0        0     2462 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/subviewer2.py
--rw-r--r--   0        0        0        0 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/__init__.py
--rw-r--r--   0        0        0     1285 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_ass.py
--rw-r--r--   0        0        0     1226 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_lrc.py
--rw-r--r--   0        0        0     1251 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_microdvd.py
--rw-r--r--   0        0        0     1243 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_mpl2.py
--rw-r--r--   0        0        0     1285 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_ssa.py
--rw-r--r--   0        0        0     1305 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_subrip.py
--rw-r--r--   0        0        0     1287 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_subviewer2.py
--rw-r--r--   0        0        0     1340 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_tmplayer.py
--rw-r--r--   0        0        0     1235 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/files/test/test_webvtt.py
--rw-r--r--   0        0        0     3522 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/tmplayer.py
--rw-r--r--   0        0        0     5358 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/files/webvtt.py
--rw-r--r--   0        0        0     6638 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/finder.py
--rw-r--r--   0        0        0     1981 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/i18n.py
--rw-r--r--   0        0        0     2041 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/languages.py
--rw-r--r--   0        0        0    11081 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/liner.py
--rw-r--r--   0        0        0     2247 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/locales.py
--rw-r--r--   0        0        0     9118 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markup.py
--rw-r--r--   0        0        0     1314 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markupconv.py
--rw-r--r--   0        0        0     1662 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/markups/__init__.py
--rw-r--r--   0        0        0     2128 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/ass.py
--rw-r--r--   0        0        0      930 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/lrc.py
--rw-r--r--   0        0        0     6472 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/microdvd.py
--rw-r--r--   0        0        0     3899 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/markups/mpl2.py
--rw-r--r--   0        0        0     7127 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/ssa.py
--rw-r--r--   0        0        0     3442 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/subrip.py
--rw-r--r--   0        0        0     1005 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/subviewer2.py
--rw-r--r--   0        0        0        0 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/__init__.py
--rw-r--r--   0        0        0     1853 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/test_ass.py
--rw-r--r--   0        0        0     5877 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/test_microdvd.py
--rw-r--r--   0        0        0     4140 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/markups/test/test_mpl2.py
--rw-r--r--   0        0        0     5734 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/test_ssa.py
--rw-r--r--   0        0        0     4893 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/test_subrip.py
--rw-r--r--   0        0        0     1276 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/test/test_webvtt.py
--rw-r--r--   0        0        0      960 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/tmplayer.py
--rw-r--r--   0        0        0     1841 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/markups/webvtt.py
--rw-r--r--   0        0        0     4567 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/metadata.py
--rw-r--r--   0        0        0     6470 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/mutables.py
--rw-r--r--   0        0        0     7285 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/observable.py
--rw-r--r--   0        0        0     6218 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/parser.py
--rw-r--r--   0        0        0     4110 2019-07-07 02:12:49.343339 aeidon-1.7.0/aeidon/paths.py
--rw-r--r--   0        0        0     1548 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/pattern.py
--rw-r--r--   0        0        0    10369 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/patternman.py
--rw-r--r--   0        0        0     1838 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/position.py
--rw-r--r--   0        0        0     6240 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/project.py
--rw-r--r--   0        0        0     3249 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/revertable.py
--rw-r--r--   0        0        0     2013 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/scripts.py
--rw-r--r--   0        0        0     1063 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/singleton.py
--rw-r--r--   0        0        0     9934 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/spell.py
--rw-r--r--   0        0        0    15053 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/subtitle.py
--rw-r--r--   0        0        0     1860 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/temp.py
--rw-r--r--   0        0        0        0 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/__init__.py
--rw-r--r--   0        0        0     5302 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_calculator.py
--rw-r--r--   0        0        0     1133 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_countries.py
--rw-r--r--   0        0        0     1119 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/test/test_deco.py
--rw-r--r--   0        0        0     1325 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_delegate.py
--rw-r--r--   0        0        0     4898 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_encodings.py
--rw-r--r--   0        0        0     2571 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_enum.py
--rw-r--r--   0        0        0     2448 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_file.py
--rw-r--r--   0        0        0     7210 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/test/test_finder.py
--rw-r--r--   0        0        0     1130 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_languages.py
--rw-r--r--   0        0        0     3194 2017-08-29 00:51:52.161788 aeidon-1.7.0/aeidon/test/test_liner.py
--rw-r--r--   0        0        0     2036 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_locales.py
--rw-r--r--   0        0        0     2116 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_markup.py
--rw-r--r--   0        0        0     3043 2019-07-07 02:12:49.347339 aeidon-1.7.0/aeidon/test/test_metadata.py
--rw-r--r--   0        0        0     4331 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_mutables.py
--rw-r--r--   0        0        0     3435 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_observable.py
--rw-r--r--   0        0        0     2873 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_parser.py
--rw-r--r--   0        0        0     1134 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_scripts.py
--rw-r--r--   0        0        0      884 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_singleton.py
--rw-r--r--   0        0        0     4701 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/test/test_spell.py
--rw-r--r--   0        0        0     9784 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_subtitle.py
--rw-r--r--   0        0        0     1713 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_temp.py
--rw-r--r--   0        0        0     5251 2017-08-29 00:51:52.165788 aeidon-1.7.0/aeidon/test/test_util.py
--rw-r--r--   0        0        0     3658 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/unittest.py
--rw-r--r--   0        0        0    16792 2020-01-26 13:07:32.672388 aeidon-1.7.0/aeidon/util.py
--rw-r--r--   0        0        0      758 2020-01-26 13:15:25.987013 aeidon-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      934 2020-01-26 13:34:00.030007 aeidon-1.7.0/setup.py
--rw-r--r--   0        0        0      897 2020-01-26 13:34:00.030269 aeidon-1.7.0/PKG-INFO
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.355082 aeidon-1.9/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2405 2020-12-31 16:42:17.355082 aeidon-1.9/PKG-INFO
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3278 2020-12-30 21:41:01.000000 aeidon-1.9/README.md
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.351082 aeidon-1.9/aeidon/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4978 2020-12-31 16:36:37.000000 aeidon-1.9/aeidon/__init__.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.351082 aeidon-1.9/aeidon/agents/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1322 2020-12-26 19:42:46.000000 aeidon-1.9/aeidon/agents/__init__.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2394 2020-12-26 19:45:44.000000 aeidon-1.9/aeidon/agents/clipboard.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     7452 2020-12-26 19:43:14.000000 aeidon-1.9/aeidon/agents/edit.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6947 2020-12-26 19:43:44.000000 aeidon-1.9/aeidon/agents/format.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8370 2020-12-26 19:42:52.000000 aeidon-1.9/aeidon/agents/open.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8178 2020-12-26 19:52:30.000000 aeidon-1.9/aeidon/agents/position.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4474 2020-12-26 19:43:49.000000 aeidon-1.9/aeidon/agents/preview.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8250 2020-12-26 19:52:58.000000 aeidon-1.9/aeidon/agents/register.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4320 2020-12-26 19:42:54.000000 aeidon-1.9/aeidon/agents/save.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    11284 2020-12-26 19:42:58.000000 aeidon-1.9/aeidon/agents/search.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     5396 2020-12-26 19:53:23.000000 aeidon-1.9/aeidon/agents/set.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    15500 2020-12-26 19:55:07.000000 aeidon-1.9/aeidon/agents/text.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6026 2020-12-26 19:43:09.000000 aeidon-1.9/aeidon/agents/util.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8945 2020-12-26 19:45:36.000000 aeidon-1.9/aeidon/calculator.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1943 2020-12-26 19:43:11.000000 aeidon-1.9/aeidon/clipboard.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2622 2020-12-26 19:46:00.000000 aeidon-1.9/aeidon/containers.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2043 2020-12-26 19:46:03.000000 aeidon-1.9/aeidon/countries.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.347082 aeidon-1.9/aeidon/data/
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.351082 aeidon-1.9/aeidon/data/headers/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      622 2020-12-26 19:45:15.000000 aeidon-1.9/aeidon/data/headers/ass
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        0 2020-12-26 19:50:39.000000 aeidon-1.9/aeidon/data/headers/lrc
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        0 2020-12-26 19:51:04.000000 aeidon-1.9/aeidon/data/headers/microdvd
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      521 2020-12-26 19:53:53.000000 aeidon-1.9/aeidon/data/headers/ssa
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      162 2020-12-26 19:54:14.000000 aeidon-1.9/aeidon/data/headers/subviewer2
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        7 2020-12-26 19:38:04.000000 aeidon-1.9/aeidon/data/headers/webvtt
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.355082 aeidon-1.9/aeidon/data/patterns/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      116 2020-12-26 19:39:11.000000 aeidon-1.9/aeidon/data/patterns/Latn-en-US.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      242 2020-12-26 19:39:14.000000 aeidon-1.9/aeidon/data/patterns/Latn-en-US.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      118 2020-12-26 19:39:15.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.capitalization.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      174 2020-12-26 19:39:17.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.capitalization.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      447 2020-12-26 19:39:18.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3086 2020-12-26 19:39:21.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      131 2020-12-26 19:39:22.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.hearing-impaired.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      300 2020-12-26 19:39:25.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.hearing-impaired.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      250 2020-12-26 19:39:27.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.line-break.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1440 2020-12-26 19:39:30.000000 aeidon-1.9/aeidon/data/patterns/Latn-en.line-break.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      127 2020-12-26 19:39:32.000000 aeidon-1.9/aeidon/data/patterns/Latn-fi.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      408 2020-12-26 19:39:36.000000 aeidon-1.9/aeidon/data/patterns/Latn-fi.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      188 2020-12-26 19:39:37.000000 aeidon-1.9/aeidon/data/patterns/Latn-fr.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1321 2020-12-26 19:39:40.000000 aeidon-1.9/aeidon/data/patterns/Latn-fr.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      151 2020-12-26 19:39:41.000000 aeidon-1.9/aeidon/data/patterns/Latn.capitalization.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      369 2020-12-26 19:39:43.000000 aeidon-1.9/aeidon/data/patterns/Latn.capitalization.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1069 2020-12-26 19:39:45.000000 aeidon-1.9/aeidon/data/patterns/Latn.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8250 2020-12-26 19:40:14.000000 aeidon-1.9/aeidon/data/patterns/Latn.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      520 2020-12-26 19:40:16.000000 aeidon-1.9/aeidon/data/patterns/Latn.hearing-impaired.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1125 2020-12-26 19:40:19.000000 aeidon-1.9/aeidon/data/patterns/Latn.hearing-impaired.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      199 2020-12-26 19:40:20.000000 aeidon-1.9/aeidon/data/patterns/Latn.line-break.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      991 2020-12-26 19:40:23.000000 aeidon-1.9/aeidon/data/patterns/Latn.line-break.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      294 2020-12-26 19:41:46.000000 aeidon-1.9/aeidon/data/patterns/Zyyy.common-error.conf
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2234 2020-12-26 19:42:02.000000 aeidon-1.9/aeidon/data/patterns/Zyyy.common-error.in
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     8146 2020-12-26 19:46:21.000000 aeidon-1.9/aeidon/deco.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1485 2020-12-26 19:46:23.000000 aeidon-1.9/aeidon/delegate.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    11132 2020-12-26 19:46:46.000000 aeidon-1.9/aeidon/encodings.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3494 2020-12-26 19:46:52.000000 aeidon-1.9/aeidon/enum.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    10099 2020-12-26 19:43:18.000000 aeidon-1.9/aeidon/enums.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1739 2020-12-26 19:43:21.000000 aeidon-1.9/aeidon/errors.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6122 2020-12-26 19:43:24.000000 aeidon-1.9/aeidon/file.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.355082 aeidon-1.9/aeidon/files/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1728 2020-12-26 19:47:09.000000 aeidon-1.9/aeidon/files/__init__.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1999 2020-12-26 19:47:12.000000 aeidon-1.9/aeidon/files/ass.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2652 2020-12-26 19:47:14.000000 aeidon-1.9/aeidon/files/lrc.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2245 2020-12-26 19:47:16.000000 aeidon-1.9/aeidon/files/microdvd.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2087 2020-12-26 19:47:19.000000 aeidon-1.9/aeidon/files/mpl2.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     5726 2020-12-26 19:47:21.000000 aeidon-1.9/aeidon/files/ssa.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4011 2020-12-26 19:47:24.000000 aeidon-1.9/aeidon/files/subrip.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2462 2020-12-26 19:47:26.000000 aeidon-1.9/aeidon/files/subviewer2.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3522 2020-12-26 19:47:41.000000 aeidon-1.9/aeidon/files/tmplayer.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     5358 2020-12-26 19:47:44.000000 aeidon-1.9/aeidon/files/webvtt.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6638 2020-12-26 19:47:46.000000 aeidon-1.9/aeidon/finder.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1981 2020-12-26 19:48:35.000000 aeidon-1.9/aeidon/i18n.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2041 2020-12-26 19:50:29.000000 aeidon-1.9/aeidon/languages.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    11081 2020-12-26 19:50:35.000000 aeidon-1.9/aeidon/liner.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2247 2020-12-26 19:50:37.000000 aeidon-1.9/aeidon/locales.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     9118 2020-12-26 19:50:45.000000 aeidon-1.9/aeidon/markup.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1314 2020-12-26 19:50:48.000000 aeidon-1.9/aeidon/markupconv.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.355082 aeidon-1.9/aeidon/markups/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1662 2020-12-26 19:50:50.000000 aeidon-1.9/aeidon/markups/__init__.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2128 2020-12-26 19:55:39.000000 aeidon-1.9/aeidon/markups/ass.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      930 2020-12-26 19:50:42.000000 aeidon-1.9/aeidon/markups/lrc.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6472 2020-12-26 19:51:07.000000 aeidon-1.9/aeidon/markups/microdvd.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3899 2020-12-26 19:51:10.000000 aeidon-1.9/aeidon/markups/mpl2.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     7127 2020-12-26 19:53:56.000000 aeidon-1.9/aeidon/markups/ssa.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3442 2020-12-26 19:54:06.000000 aeidon-1.9/aeidon/markups/subrip.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1005 2020-12-26 19:54:16.000000 aeidon-1.9/aeidon/markups/subviewer2.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      960 2020-12-26 19:55:10.000000 aeidon-1.9/aeidon/markups/tmplayer.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1841 2020-12-26 19:55:36.000000 aeidon-1.9/aeidon/markups/webvtt.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4567 2020-12-26 19:51:03.000000 aeidon-1.9/aeidon/metadata.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6470 2020-12-26 19:51:30.000000 aeidon-1.9/aeidon/mutables.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     7285 2020-12-26 19:51:33.000000 aeidon-1.9/aeidon/observable.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6218 2020-12-26 19:51:44.000000 aeidon-1.9/aeidon/parser.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     4463 2020-12-27 18:54:58.000000 aeidon-1.9/aeidon/paths.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1548 2020-12-26 19:52:08.000000 aeidon-1.9/aeidon/pattern.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    10369 2020-12-26 19:52:15.000000 aeidon-1.9/aeidon/patternman.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1838 2020-12-26 19:43:47.000000 aeidon-1.9/aeidon/position.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     6240 2020-12-26 19:52:53.000000 aeidon-1.9/aeidon/project.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3249 2020-12-26 19:53:06.000000 aeidon-1.9/aeidon/revertable.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2013 2020-12-26 19:53:15.000000 aeidon-1.9/aeidon/scripts.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1063 2020-12-26 19:53:39.000000 aeidon-1.9/aeidon/singleton.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     9934 2020-12-26 19:44:03.000000 aeidon-1.9/aeidon/spell.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    15053 2020-12-26 19:54:13.000000 aeidon-1.9/aeidon/subtitle.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1860 2020-12-26 19:38:15.000000 aeidon-1.9/aeidon/temp.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3658 2020-12-26 19:44:25.000000 aeidon-1.9/aeidon/unittest.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    16792 2020-12-26 19:44:30.000000 aeidon-1.9/aeidon/util.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-12-31 16:42:17.351082 aeidon-1.9/aeidon.egg-info/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2405 2020-12-31 16:42:17.000000 aeidon-1.9/aeidon.egg-info/PKG-INFO
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2878 2020-12-31 16:42:17.000000 aeidon-1.9/aeidon.egg-info/SOURCES.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        1 2020-12-31 16:42:17.000000 aeidon-1.9/aeidon.egg-info/dependency_links.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)       15 2020-12-31 16:42:17.000000 aeidon-1.9/aeidon.egg-info/requires.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        7 2020-12-31 16:42:17.000000 aeidon-1.9/aeidon.egg-info/top_level.txt
+-rwxr-xr-x   0 osmo      (1000) osmo      (1000)      965 2020-12-30 21:35:12.000000 aeidon-1.9/setup-aeidon.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)       38 2020-12-31 16:42:17.355082 aeidon-1.9/setup.cfg
+-rwxr-xr-x   0 osmo      (1000) osmo      (1000)    14915 2020-12-30 21:35:20.000000 aeidon-1.9/setup.py
```

### Comparing `aeidon-1.7.0/aeidon/__init__.py` & `aeidon-1.9/aeidon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 :var players: Enumerations for video player application types
 :var registers: Enumerations for action action reversion register types
 """
 
 import re
 import sys
 
-__version__ = "1.7"
+__version__ = "1.9"
 
 RUNNING_SPHINX = (sys.argv[0].endswith("autogen.py") or
                   sys.argv[0].endswith("sphinx-build"))
 
 RE_ANY_TAG = re.compile(r"(^[/\\_]+|<.*?>|\{.*?\})")
 
 try:
```

### Comparing `aeidon-1.7.0/aeidon/agents/__init__.py` & `aeidon-1.9/aeidon/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/clipboard.py` & `aeidon-1.9/aeidon/agents/clipboard.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/edit.py` & `aeidon-1.9/aeidon/agents/edit.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/format.py` & `aeidon-1.9/aeidon/agents/format.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/open.py` & `aeidon-1.9/aeidon/agents/open.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/position.py` & `aeidon-1.9/aeidon/agents/position.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/preview.py` & `aeidon-1.9/aeidon/agents/preview.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/register.py` & `aeidon-1.9/aeidon/agents/register.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/save.py` & `aeidon-1.9/aeidon/agents/save.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/search.py` & `aeidon-1.9/aeidon/agents/search.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/set.py` & `aeidon-1.9/aeidon/agents/set.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/agents/text.py` & `aeidon-1.9/aeidon/agents/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,17 @@
             subtitle = self.subtitles[index]
             text = subtitle.get_text(doc)
             text = re.sub(r" +", " ", text)
             navigator.reset(text)
             for pos, word in navigator:
                 # Skip capitalized words, which are usually names
                 # and thus not always found in dictionaries.
-                if word.istitle(): continue
+                if word.istitle():
+                    navigator.ignore()
+                    continue
                 suggestions = navigator.suggest()
                 suggestions = [x for x in suggestions if x.replace(" ", "") == word]
                 # Split word only if only one two-word suggestion found that
                 # has all the same characters as the original unsplit word.
                 if len(suggestions) == 1:
                     navigator.replace(suggestions[0])
                 else:
```

### Comparing `aeidon-1.7.0/aeidon/agents/util.py` & `aeidon-1.9/aeidon/agents/util.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/calculator.py` & `aeidon-1.9/aeidon/calculator.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/clipboard.py` & `aeidon-1.9/aeidon/clipboard.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/containers.py` & `aeidon-1.9/aeidon/containers.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/countries.py` & `aeidon-1.9/aeidon/countries.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/deco.py` & `aeidon-1.9/aeidon/deco.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/delegate.py` & `aeidon-1.9/aeidon/delegate.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/encodings.py` & `aeidon-1.9/aeidon/encodings.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/enum.py` & `aeidon-1.9/aeidon/enum.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/enums.py` & `aeidon-1.9/aeidon/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,19 +67,39 @@
     label = _("25.000 fps")
     value = 25.0
 
 class Framerate29970(aeidon.EnumerationItem):
     label = _("29.970 fps")
     value = 30 / 1.001
 
+class Framerate30000(aeidon.EnumerationItem):
+    label = _("30.000 fps")
+    value = 30.0
+
+class Framerate50000(aeidon.EnumerationItem):
+    label = _("50.000 fps")
+    value = 50.0
+
+class Framerate59940(aeidon.EnumerationItem):
+    label = _("59.940 fps")
+    value = 60 / 1.001
+
+class Framerate60000(aeidon.EnumerationItem):
+    label = _("60.000 fps")
+    value = 60.0
+
 framerates = aeidon.Enumeration()
 framerates.FPS_23_976 = Framerate23976()
 framerates.FPS_24_000 = Framerate24000()
 framerates.FPS_25_000 = Framerate25000()
 framerates.FPS_29_970 = Framerate29970()
+framerates.FPS_30_000 = Framerate30000()
+framerates.FPS_50_000 = Framerate50000()
+framerates.FPS_59_940 = Framerate59940()
+framerates.FPS_60_000 = Framerate60000()
 
 
 class ModeTime(aeidon.EnumerationItem): pass
 class ModeFrame(aeidon.EnumerationItem): pass
 class ModeSeconds(aeidon.EnumerationItem): pass
 
 modes = aeidon.Enumeration()
```

### Comparing `aeidon-1.7.0/aeidon/errors.py` & `aeidon-1.9/aeidon/errors.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/file.py` & `aeidon-1.9/aeidon/file.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/__init__.py` & `aeidon-1.9/aeidon/files/__init__.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/ass.py` & `aeidon-1.9/aeidon/files/ass.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/lrc.py` & `aeidon-1.9/aeidon/files/lrc.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/microdvd.py` & `aeidon-1.9/aeidon/files/microdvd.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/mpl2.py` & `aeidon-1.9/aeidon/files/mpl2.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/ssa.py` & `aeidon-1.9/aeidon/files/ssa.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/subrip.py` & `aeidon-1.9/aeidon/files/subrip.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/subviewer2.py` & `aeidon-1.9/aeidon/files/subviewer2.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/test/test_ass.py` & `aeidon-1.9/aeidon/markupconv.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+"""Subtitle text markup converter."""
+
 import aeidon
 
+__all__ = ("MarkupConverter",)
+
+
+class MarkupConverter:
+
+    """Subtitle text markup converter."""
 
-class TestSubStationAlpha(aeidon.TestCase):
+    def __init__(self, from_format, to_format):
+        """
+        Initialize a :class:`MarkupConverter` instance.
 
-    format = aeidon.formats.ASS
+        `from_format` and `to_format` should be :attr:`aeidon.formats`
+        enumeration items.
+        """
+        self._from = aeidon.markups.new(from_format)
+        self._to = aeidon.markups.new(to_format)
 
-    def setup_method(self, method):
-        self.file = aeidon.files.new(self.format,
-                                     self.new_temp_file(self.format),
-                                     "ascii")
-
-    def test_read(self):
-        assert self.file.read()
-        assert self.file.header
-
-    def test_write(self):
-        self.file.write(self.file.read(), aeidon.documents.MAIN)
-        text = open(self.file.path, "r").read().strip()
-        assert text == self.get_sample_text(self.format)
+    def convert(self, text):
+        """Return `text` with markup converted."""
+        return self._to.encode(self._from.decode(text))
```

### Comparing `aeidon-1.7.0/aeidon/files/test/test_lrc.py` & `aeidon-1.9/aeidon/markups/lrc.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,26 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+"""Text markup for the LRC format."""
+
 import aeidon
 
+__all__ = ("LRC",)
 
-class TestLRC(aeidon.TestCase):
 
-    format = aeidon.formats.LRC
-    name = "lrc"
+class LRC(aeidon.Markup):
+
+    """
+    Text markup for the LRC format.
 
-    def setup_method(self, method):
-        path = self.new_temp_file(self.format, self.name)
-        self.file = aeidon.files.new(self.format, path, "ascii")
-
-    def test_read(self):
-        assert self.file.read()
-
-    def test_write(self):
-        self.file.write(self.file.read(), aeidon.documents.MAIN)
-        text = open(self.file.path, "r").read().strip()
-        assert text == self.get_sample_text(self.format, self.name)
+    LRC format is assumed to contain no markup.
+    """
+
+    format = aeidon.formats.LRC
```

### Comparing `aeidon-1.7.0/aeidon/files/test/test_microdvd.py` & `aeidon-1.9/aeidon/markups/tmplayer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2005 Osmo Salomaa
+# Copyright (C) 2006 Osmo Salomaa
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+"""Text markup for the TMPlayer format."""
+
 import aeidon
 
+__all__ = ("TMPlayer",)
+
+
+class TMPlayer(aeidon.Markup):
 
-class TestMicroDVD(aeidon.TestCase):
+    """
+    Text markup for the TMPlayer format.
 
-    format = aeidon.formats.MICRODVD
+    TMPlayer format is assumed to contain no markup.
+    """
 
-    def setup_method(self, method):
-        self.file = aeidon.files.new(self.format,
-                                     self.new_temp_file(self.format),
-                                     "ascii")
-
-    def test_read(self):
-        assert self.file.read()
-
-    def test_write(self):
-        self.file.write(self.file.read(), aeidon.documents.MAIN)
-        text = open(self.file.path, "r").read().strip()
-        assert text == self.get_sample_text(self.format)
+    format = aeidon.formats.TMPLAYER
```

### Comparing `aeidon-1.7.0/aeidon/files/test/test_mpl2.py` & `aeidon-1.9/aeidon/singleton.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2005 Osmo Salomaa
+# Copyright (C) 2007 Osmo Salomaa
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import aeidon
+"""Base class for single-instance classes."""
 
+__all__ = ("Singleton",)
 
-class TestMPL2(aeidon.TestCase):
 
-    format = aeidon.formats.MPL2
+class Singleton:
 
-    def setup_method(self, method):
-        self.file = aeidon.files.new(self.format,
-                                     self.new_temp_file(self.format),
-                                     "ascii")
+    """Base class for single-instance classes."""
 
-    def test_read(self):
-        assert self.file.read()
-
-    def test_write(self):
-        self.file.write(self.file.read(), aeidon.documents.MAIN)
-        text = open(self.file.path, "r").read().strip()
-        assert text == self.get_sample_text(self.format)
+    def __new__(cls, *args, **kwargs):
+        """Return possibly existing instance."""
+        if not "_instance" in cls.__dict__:
+            cls._instance = object.__new__(cls, *args, **kwargs)
+        return cls._instance
```

### Comparing `aeidon-1.7.0/aeidon/files/tmplayer.py` & `aeidon-1.9/aeidon/files/tmplayer.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/files/webvtt.py` & `aeidon-1.9/aeidon/files/webvtt.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/finder.py` & `aeidon-1.9/aeidon/finder.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/i18n.py` & `aeidon-1.9/aeidon/i18n.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/languages.py` & `aeidon-1.9/aeidon/languages.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/liner.py` & `aeidon-1.9/aeidon/liner.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/locales.py` & `aeidon-1.9/aeidon/locales.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markup.py` & `aeidon-1.9/aeidon/markup.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/__init__.py` & `aeidon-1.9/aeidon/markups/__init__.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/ass.py` & `aeidon-1.9/aeidon/markups/ass.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/microdvd.py` & `aeidon-1.9/aeidon/markups/microdvd.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/mpl2.py` & `aeidon-1.9/aeidon/markups/mpl2.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/ssa.py` & `aeidon-1.9/aeidon/markups/ssa.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/subrip.py` & `aeidon-1.9/aeidon/markups/subrip.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/subviewer2.py` & `aeidon-1.9/aeidon/markups/subviewer2.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/markups/webvtt.py` & `aeidon-1.9/aeidon/markups/webvtt.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/metadata.py` & `aeidon-1.9/aeidon/metadata.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/mutables.py` & `aeidon-1.9/aeidon/mutables.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/observable.py` & `aeidon-1.9/aeidon/observable.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/parser.py` & `aeidon-1.9/aeidon/parser.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/paths.py` & `aeidon-1.9/aeidon/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,30 @@
     directory = os.path.join(directory, "gaupol")
     return os.path.abspath(directory)
 
 def get_data_directory():
     """Return path to the global data directory."""
     if hasattr(sys, "frozen"):
         return get_data_directory_frozen()
+    if os.path.isdir(get_data_directory_package()):
+        return get_data_directory_package()
     return get_data_directory_source()
 
 def get_data_directory_frozen():
     """Return path to the global data directory on ``frozen``."""
     directory = os.path.dirname(sys.argv[0])
     directory = os.path.join(directory, "share", "gaupol")
     return os.path.abspath(directory)
 
+def get_data_directory_package():
+    """Return path to the global data directory when data in the package."""
+    directory = os.path.dirname(os.path.abspath(__file__))
+    directory = os.path.join(directory, "data")
+    return os.path.abspath(directory)
+
 def get_data_directory_source():
     """Return path to the global data directory when running from source."""
     directory = os.path.dirname(os.path.abspath(__file__))
     directory = os.path.abspath(os.path.join(directory, ".."))
     directory = os.path.join(directory, "data")
     return os.path.abspath(directory)
```

### Comparing `aeidon-1.7.0/aeidon/pattern.py` & `aeidon-1.9/aeidon/pattern.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/patternman.py` & `aeidon-1.9/aeidon/patternman.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/position.py` & `aeidon-1.9/aeidon/position.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/project.py` & `aeidon-1.9/aeidon/project.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/revertable.py` & `aeidon-1.9/aeidon/revertable.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/scripts.py` & `aeidon-1.9/aeidon/scripts.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/spell.py` & `aeidon-1.9/aeidon/spell.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/subtitle.py` & `aeidon-1.9/aeidon/subtitle.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/temp.py` & `aeidon-1.9/aeidon/temp.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/unittest.py` & `aeidon-1.9/aeidon/unittest.py`

 * *Files identical despite different names*

### Comparing `aeidon-1.7.0/aeidon/util.py` & `aeidon-1.9/aeidon/util.py`

 * *Files identical despite different names*

