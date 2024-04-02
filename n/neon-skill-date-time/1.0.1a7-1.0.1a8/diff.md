# Comparing `tmp/neon-skill-date_time-1.0.1a7.tar.gz` & `tmp/neon-skill-date_time-1.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-date_time-1.0.1a7.tar", last modified: Mon Apr  1 21:46:13 2024, max compression
+gzip compressed data, was "neon-skill-date_time-1.0.1a8.tar", last modified: Mon Apr  1 23:48:26 2024, max compression
```

## Comparing `neon-skill-date_time-1.0.1a7.tar` & `neon-skill-date_time-1.0.1a8.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.119102 neon-skill-date_time-1.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 21:46:13.119102 neon-skill-date_time-1.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/ca-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ca-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/da-dk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/da-dk/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/da-dk/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/da-dk/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/da-dk/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/de-de/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.091102 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/date_time_in_location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/time.tz.not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_friday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_monday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_saturday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_sunday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_thursday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_tuesday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/dialog/word_wednesday.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/intent/what.day.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/intent/what.dow.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/intent/what.time.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/en-us/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/es-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/es-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/eu-eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/eu-eu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/eu-eu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/eu-eu/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/eu-eu/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/fa-ir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/fa-ir/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.095102 neon-skill-date_time-1.0.1a7/locale/fa-ir/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/fa-ir/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fa-ir/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/fr-fr/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/fr-fr/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/gl-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/gl-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.083102 neon-skill-date_time-1.0.1a7/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.099102 neon-skill-date_time-1.0.1a7/locale/hu-hu/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/hu-hu/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/it-it/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/it-it/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.083102 neon-skill-date_time-1.0.1a7/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/nl-nl/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/nl-nl/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/pl-pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/pl-pl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/pl-pl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/pl-pl/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pl-pl/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.103102 neon-skill-date_time-1.0.1a7/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/pt-br/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/pt-br/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.083102 neon-skill-date_time-1.0.1a7/locale/ro-ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ro-ro/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ro-ro/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ro-ro/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ro-ro/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.083102 neon-skill-date_time-1.0.1a7/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/ru-ru/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/ru-ru/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.107102 neon-skill-date_time-1.0.1a7/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/sv-se/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/sv-se/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.083102 neon-skill-date_time-1.0.1a7/locale/tr-tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/tr-tr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/tr-tr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/tr-tr/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/tr-tr/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.087102 neon-skill-date_time-1.0.1a7/locale/uk-ua/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/date_time_in_location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/time.tz.not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_friday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_monday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_saturday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_sunday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_thursday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_tuesday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/dialog/word_wednesday.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.111102 neon-skill-date_time-1.0.1a7/locale/uk-ua/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.115102 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/what.day.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/what.dow.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.115102 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 21:46:13.000000 neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:46:13.119102 neon-skill-date_time-1.0.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.115102 neon-skill-date_time-1.0.1a7/test/
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.115102 neon-skill-date_time-1.0.1a7/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/date.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/date2.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/idle.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:46:13.115102 neon-skill-date_time-1.0.1a7/ui/img/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/img/date-bg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/img/date-top.svg
--rw-r--r--   0 runner    (1001) docker     (127)  1061425 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/img/idle-background.png
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/ui/time.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 21:46:09.000000 neon-skill-date_time-1.0.1a7/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.082536 neon-skill-date_time-1.0.1a8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 23:48:26.078536 neon-skill-date_time-1.0.1a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/ca-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ca-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/da-dk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/da-dk/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/da-dk/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/da-dk/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/da-dk/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/de-de/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/date_time_in_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/time.tz.not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_friday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_monday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_saturday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_sunday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_thursday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_tuesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/dialog/word_wednesday.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.054536 neon-skill-date_time-1.0.1a8/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/intent/what.day.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/intent/what.dow.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/intent/what.time.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/en-us/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/es-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/es-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/eu-eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/eu-eu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/eu-eu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/eu-eu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/eu-eu/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/fa-ir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/fa-ir/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/fa-ir/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.058536 neon-skill-date_time-1.0.1a8/locale/fa-ir/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fa-ir/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/fr-fr/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/fr-fr/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/gl-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/gl-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.046536 neon-skill-date_time-1.0.1a8/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/hu-hu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/hu-hu/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.062536 neon-skill-date_time-1.0.1a8/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/it-it/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/it-it/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.046536 neon-skill-date_time-1.0.1a8/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/nl-nl/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/nl-nl/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/pl-pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/pl-pl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/pl-pl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/pl-pl/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pl-pl/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.066536 neon-skill-date_time-1.0.1a8/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/pt-br/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/pt-br/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.046536 neon-skill-date_time-1.0.1a8/locale/ro-ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ro-ro/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ro-ro/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ro-ro/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ro-ro/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.046536 neon-skill-date_time-1.0.1a8/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/ru-ru/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/ru-ru/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.070536 neon-skill-date_time-1.0.1a8/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/sv-se/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/sv-se/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.046536 neon-skill-date_time-1.0.1a8/locale/tr-tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/tr-tr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/tr-tr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/tr-tr/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/tr-tr/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.050536 neon-skill-date_time-1.0.1a8/locale/uk-ua/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/date_time_in_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/time.tz.not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_friday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_monday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_saturday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_sunday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_thursday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_tuesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/dialog/word_wednesday.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/uk-ua/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.074536 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/what.day.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/what.dow.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.078536 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 23:48:25.000000 neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 23:48:26.082536 neon-skill-date_time-1.0.1a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.078536 neon-skill-date_time-1.0.1a8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.078536 neon-skill-date_time-1.0.1a8/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/date.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/date2.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/idle.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:48:26.078536 neon-skill-date_time-1.0.1a8/ui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/img/date-bg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/img/date-top.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  1061425 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/img/idle-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/ui/time.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 23:48:23.000000 neon-skill-date_time-1.0.1a8/version.py
```

### Comparing `neon-skill-date_time-1.0.1a7/LICENSE` & `neon-skill-date_time-1.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/LICENSE.md` & `neon-skill-date_time-1.0.1a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/PKG-INFO` & `neon-skill-date_time-1.0.1a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-date_time
-Version: 1.0.1a7
+Version: 1.0.1a8
 Home-page: https://github.com/NeonGeckoCom/skill-date_time
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-date_time-1.0.1a7/README.md` & `neon-skill-date_time-1.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/__init__.py` & `neon-skill-date_time-1.0.1a8/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/what.dow.is.it.intent` & `neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/what.dow.is.it.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/locale/uk-ua/vocab/what.time.is.it.intent` & `neon-skill-date_time-1.0.1a8/locale/uk-ua/vocab/what.time.is.it.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/PKG-INFO` & `neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-date-time
-Version: 1.0.1a7
+Version: 1.0.1a8
 Home-page: https://github.com/NeonGeckoCom/skill-date_time
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-date_time-1.0.1a7/neon_skill_date_time.egg-info/SOURCES.txt` & `neon-skill-date_time-1.0.1a8/neon_skill_date_time.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/setup.py` & `neon-skill-date_time-1.0.1a8/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/skill.json` & `neon-skill-date_time-1.0.1a8/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/test/test_skill.py` & `neon-skill-date_time-1.0.1a8/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/ui/date.qml` & `neon-skill-date_time-1.0.1a8/ui/date.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/ui/date2.qml` & `neon-skill-date_time-1.0.1a8/ui/date2.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/ui/idle.qml` & `neon-skill-date_time-1.0.1a8/ui/idle.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/ui/img/idle-background.png` & `neon-skill-date_time-1.0.1a8/ui/img/idle-background.png`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/ui/time.qml` & `neon-skill-date_time-1.0.1a8/ui/time.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-1.0.1a7/version.py` & `neon-skill-date_time-1.0.1a8/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a7"
+__version__ = "1.0.1a8"
```

